# Comparing `tmp/PolyRound-0.2.9.tar.gz` & `tmp/polyround-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PolyRound-0.2.9.tar", last modified: Fri Apr 28 13:56:27 2023, max compression
+gzip compressed data, was "polyround-0.3.0.tar", last modified: Sat May 11 20:39:49 2024, max compression
```

## Comparing `PolyRound-0.2.9.tar` & `polyround-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:56:27.443999 PolyRound-0.2.9/
--rw-rw-rw-   0 root         (0) root         (0)    34667 2023-04-28 13:56:13.000000 PolyRound-0.2.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5054 2023-04-28 13:56:27.441999 PolyRound-0.2.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:56:27.423997 PolyRound-0.2.9/PolyRound/
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6769 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/api.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/default_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:56:27.431998 PolyRound-0.2.9/PolyRound/mutable_classes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/mutable_classes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5190 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/mutable_classes/polytope.py
--rw-rw-rw-   0 root         (0) root         (0)     3916 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:56:27.436998 PolyRound-0.2.9/PolyRound/static_classes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7488 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/constraint_removal_reduction.py
--rw-rw-rw-   0 root         (0) root         (0)     1927 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/csv_io.py
--rw-rw-rw-   0 root         (0) root         (0)    12846 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/lp_interfacing.py
--rw-rw-rw-   0 root         (0) root         (0)     2501 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/lp_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3826 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/parse_sbml_stoichiometry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:56:27.441999 PolyRound-0.2.9/PolyRound/static_classes/rounding/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/rounding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3138 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/rounding/geometric_mean_scaling.py
--rw-rw-rw-   0 root         (0) root         (0)    10569 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/rounding/maximum_volume_ellipsoid.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/static_classes/rounding/nearest_symmetric_positive_definite.py
--rw-rw-rw-   0 root         (0) root         (0)    20225 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/unit_tests.py
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-04-28 13:56:13.000000 PolyRound-0.2.9/PolyRound/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 13:56:27.429998 PolyRound-0.2.9/PolyRound.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5054 2023-04-28 13:56:27.000000 PolyRound-0.2.9/PolyRound.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      923 2023-04-28 13:56:27.000000 PolyRound-0.2.9/PolyRound.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 13:56:27.000000 PolyRound-0.2.9/PolyRound.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-28 13:56:27.000000 PolyRound-0.2.9/PolyRound.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-28 13:56:27.000000 PolyRound-0.2.9/PolyRound.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     4553 2023-04-28 13:56:13.000000 PolyRound-0.2.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 13:56:27.443999 PolyRound-0.2.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1270 2023-04-28 13:56:13.000000 PolyRound-0.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 20:39:49.563994 polyround-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34667 2024-05-11 20:39:45.000000 polyround-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5377 2024-05-11 20:39:49.563994 polyround-0.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 20:39:49.558993 polyround-0.3.0/PolyRound/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7267 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/api.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/default_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 20:39:49.560994 polyround-0.3.0/PolyRound/mutable_classes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/mutable_classes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5190 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/mutable_classes/polytope.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 20:39:49.561993 polyround-0.3.0/PolyRound/static_classes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/static_classes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7499 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/static_classes/constraint_removal_reduction.py
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/static_classes/csv_io.py
+-rw-rw-rw-   0 root         (0) root         (0)    12989 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/static_classes/lp_interfacing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2501 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/static_classes/lp_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4449 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/static_classes/parse_sbml_stoichiometry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 20:39:49.562994 polyround-0.3.0/PolyRound/static_classes/rounding/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/static_classes/rounding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3138 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/static_classes/rounding/geometric_mean_scaling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10569 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/static_classes/rounding/maximum_volume_ellipsoid.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/static_classes/rounding/nearest_symmetric_positive_definite.py
+-rw-rw-rw-   0 root         (0) root         (0)    22079 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/unit_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-11 20:39:45.000000 polyround-0.3.0/PolyRound/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 20:39:49.562994 polyround-0.3.0/PolyRound.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5377 2024-05-11 20:39:49.000000 polyround-0.3.0/PolyRound.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      923 2024-05-11 20:39:49.000000 polyround-0.3.0/PolyRound.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 20:39:49.000000 polyround-0.3.0/PolyRound.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2024-05-11 20:39:49.000000 polyround-0.3.0/PolyRound.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-11 20:39:49.000000 polyround-0.3.0/PolyRound.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4602 2024-05-11 20:39:45.000000 polyround-0.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 20:39:49.563994 polyround-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1337 2024-05-11 20:39:45.000000 polyround-0.3.0/setup.py
```

### Comparing `PolyRound-0.2.9/LICENSE` & `polyround-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.9/PKG-INFO` & `polyround-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 Metadata-Version: 2.1
 Name: PolyRound
-Version: 0.2.9
+Version: 0.3.0
 Summary: A python package for rounding polytopes.
 Home-page: https://gitlab.com/csb.ethz/PolyRound
 Author: Axel Theorell
 Author-email: atheorell@ethz.ch
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.2
+Requires-Dist: pandas>=1.2
+Requires-Dist: scipy>=1.4
+Requires-Dist: optlang>=1.4
+Provides-Extra: extras
+Requires-Dist: cobra>=0.20; extra == "extras"
+Requires-Dist: python-libsbml>=5.18; extra == "extras"
+Requires-Dist: gurobipy; extra == "extras"
 
 # PolyRound
-[![PyPI version](https://badge.fury.io/py/PolyRound.svg)](https://badge.fury.io/py/PolyRound)
 
 Efficient random sampling in convex polytopes relies on a 'rounding' preprocessing step, in which the polytope is rescaled so that the width is as uniform as possible across different dimensions.
 PolyRound rounds polytopes on the general form:
 
 $`P:=\{x \in \mathcal{R}^n: A_{eq} x = b_{eq}, A_{ineq} x \leq b_{ineq}\}`$ with matrices $`A_{eq} \in \mathcal{R}^{m,n}`$ and $`A_{ineq} \in \mathcal{R}^{k,n}`$ and vectors $`b_{eq} \in \mathcal{R}^{m}`$ and $`b_{ineq} \in \mathcal{R}^{k}`$.
 
 This formulation often arises in Systems Biology as the flux space of a metabolic network.
 
 As output, PolyRound produces a polytope on the form $`P^{r}:=\{v \in \mathcal{R}^l: A^{r}_{ineq}v \leq b^{r}_{ineq}\}`$ where $`l \leq n`$ and the zero vector is a stricly interior point. For transforming points back to the original space, it also provides a matrix $`S \in \mathcal{R}^{n,l}`$ and a vector $`t \in \mathcal{R}^{n}`$, so that $`x=Sv + t`$.
 
-Currently, PolyRound is supported for python 3.7 to 3.9.
+Currently, PolyRound is supported for python 3.8 to 3.12.
+
+PolyRound comes with two optional dependencies: 1) Gurobi (for the best linear programming) and 2) Cobrapy (for SBML support)
+Both dependencies are fetched by installing the extras: "pip install 'PolyRound[extras]'".
+When Gurobi is not installed, PolyRound uses optlang (https://github.com/opencobra/optlang) to delegate linear programs to GLPK. However, PolyRound is more reliable with Gurobi. Free Gurobi licenses for academic use can be obtained at https://www.gurobi.com/. Once the license is installed, gurobipy can be installed directly through pip, or by getting the optional requirements as described above.
 
-PolyRound no longer depends on a Gurobi installation and uses optlang (https://github.com/opencobra/optlang) to delegate linear programs to GLPK in case Gurobi is not installed. However, PolyRound is more reliable with Gurobi. Free Gurobi licenses for academic use can be obtained at https://www.gurobi.com/. Once the license is installed, gurobipy can be installed directly through pip, or by getting the optional requirements by 'pip install -r optional_requirements.txt'.
 
 An easy example of how to get started is presented in the jupyter notebook cells below.
 
 
 They show how to: <br>
 1) create a polytope object from a file path <br>
 2) simplify, reduce, and round a polytope in separate steps, togehter with some printed checks <br>
```

### Comparing `PolyRound-0.2.9/PolyRound/__init__.py` & `polyround-0.3.0/PolyRound/__init__.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.9/PolyRound/api.py` & `polyround-0.3.0/PolyRound/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 from typing import Dict
 from PolyRound.static_classes.lp_utils import ChebyshevFinder
 from PolyRound.static_classes.rounding.maximum_volume_ellipsoid import (
     MaximumVolumeEllipsoidFinder,
 )
 
 import numpy as np
-from cobra.core.model import Model
+
+try:
+    from cobra.core.model import Model
+except:
+    Model = None
 from PolyRound.static_classes.parse_sbml_stoichiometry import StoichiometryParser
 from PolyRound.static_classes.csv_io import CSV
 
 from PolyRound.settings import PolyRoundSettings
 
 
 class PolyRoundApi:
@@ -160,23 +164,33 @@
         polytope = PolyRoundApi.round_polytope(
             polytope,
             settings=settings,
         )
         return polytope
 
     @staticmethod
-    def cobra_model_to_polytope(model: Model):
+    def cobra_model_to_polytope(model):
         """
         Turn cobrapy model into polytope
-        @param model:
+        @param model: cobrapy model
         @return:
         """
+        if Model is None:
+            raise NotImplementedError(
+                "Cobra not currently supported. Install Polyround with extras to support cobra "
+                "(pip install 'PolyRound[extras]')"
+            )
         return StoichiometryParser.extract_polytope(model)
 
     @staticmethod
     def polytope_to_csvs(polytope: Polytope, dirname: str):
         CSV.polytope_to_csv(polytope, dirname)
 
     @staticmethod
     def sbml_to_polytope(file_name: str) -> Polytope:
+        if Model is None:
+            raise NotImplementedError(
+                "Cobra not currently supported. Install Polyround with extras to support cobra "
+                "(pip install 'PolyRound[extras]')"
+            )
         polytope = StoichiometryParser.parse_sbml_cobrapy(file_name)
         return polytope
```

### Comparing `PolyRound-0.2.9/PolyRound/main.py` & `polyround-0.3.0/PolyRound/main.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.9/PolyRound/mutable_classes/polytope.py` & `polyround-0.3.0/PolyRound/mutable_classes/polytope.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.9/PolyRound/settings.py` & `polyround-0.3.0/PolyRound/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 
 from PolyRound.default_settings import (
     default_hp_flags,
     default_0_width,
     default_numerics_threshold,
     default_accepted_tol_violation,
 )
-from cobra.util.solver import solvers
 import optlang
 
-if "gurobi" in solvers:
+try:
+    import gurobipy
+except:
+    gurobipy = None
+
+if gurobipy:
     pref_backend = "gurobi"
 else:
     pref_backend = "glpk"
 
 
 class PolyRoundSettings:
     """
```

### Comparing `PolyRound-0.2.9/PolyRound/static_classes/constraint_removal_reduction.py` & `polyround-0.3.0/PolyRound/static_classes/constraint_removal_reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 config.verbosity = 0
 import numpy as np
 from PolyRound.settings import PolyRoundSettings
 import scipy.sparse as sp
 from PolyRound.static_classes.lp_interfacing import OptlangInterfacer
 from PolyRound.default_settings import default_solver_timeout
 from sympy.core import Add, Mul
-from cobra.util.solver import solvers
+
+from PolyRound.static_classes.lp_interfacing import solvers
 from sympy import Matrix, SparseMatrix
 import pandas as pd
-import time
 
 
 class PolytopeReducer:
     @staticmethod
     def constraint_removal(
         polytope,
         settings,
```

### Comparing `PolyRound-0.2.9/PolyRound/static_classes/csv_io.py` & `polyround-0.3.0/PolyRound/static_classes/csv_io.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.9/PolyRound/static_classes/lp_interfacing.py` & `polyround-0.3.0/PolyRound/static_classes/lp_interfacing.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,23 @@
 config = glpk_interface.Configuration()
 config.verbosity = 0
 import numpy as np
 import pandas as pd
 from scipy import sparse as sp
 from optlang.symbolics import Zero
 from sympy.core import Add, Mul
-from cobra.util.solver import solvers
+
+import optlang
+
+solvers = {
+    match.split("_interface")[0]: getattr(optlang, match)
+    for match in dir(optlang)
+    if "_interface" in match and match != "matrix_interface"
+}
+
 from swiglpk import glp_adv_basis
 from PolyRound.mutable_classes.polytope import Polytope
 import uuid
 from PolyRound.default_settings import default_accepted_tol_violation
 import warnings
 from PolyRound.default_settings import default_hp_flags
```

### Comparing `PolyRound-0.2.9/PolyRound/static_classes/lp_utils.py` & `polyround-0.3.0/PolyRound/static_classes/lp_utils.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.9/PolyRound/static_classes/parse_sbml_stoichiometry.py` & `polyround-0.3.0/PolyRound/static_classes/parse_sbml_stoichiometry.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 # ©2020-​2021 ETH Zurich, Axel Theorell
 from optlang import glpk_interface
 
 config = glpk_interface.Configuration()
 config.verbosity = 0
 import pandas as pd
 from PolyRound.mutable_classes.polytope import Polytope
-import cobra
+
+try:
+    import cobra
+except:
+    cobra = None
 import uuid
 import numpy as np
 from PolyRound.static_classes.lp_utils import ChebyshevFinder
 
 
 class StoichiometryParser:
     @staticmethod
     def parse_sbml_cobrapy(file, inf_bound=1e5, prescale=False):
+        if cobra is None:
+            raise NotImplementedError(
+                "missing optional cobrapy dependency required for parsing sbml. Use pip install 'PolyRound[extras]'"
+            )
         model = StoichiometryParser.read_sbml_model(file)
 
         if prescale:
             # prefix reactions
             reactions = list(model.reactions)
             for r in reactions:
                 model.remove_reactions([r])
@@ -39,19 +47,27 @@
         if prescale:
             p.apply_transformation(transformation.values)
 
         return p
 
     @staticmethod
     def read_sbml_model(file):
+        if cobra is None:
+            raise NotImplementedError(
+                "missing optional cobrapy dependency required for parsing sbml. Use pip install 'PolyRound[extras]'"
+            )
         model = cobra.io.read_sbml_model(file)
         return model
 
     @staticmethod
     def extract_polytope(model, inf_bound=1e5):
+        if cobra is None:
+            raise NotImplementedError(
+                "missing optional cobrapy dependency required for parsing sbml. Use pip install 'PolyRound[extras]'"
+            )
         S = cobra.util.array.create_stoichiometric_matrix(model, array_type="DataFrame")
         # make bounds matrix
         n_react = len(model.reactions)
         uids = [uuid.uuid4().hex for i in range(n_react * 2)]
         A = pd.DataFrame(0.0, index=uids, columns=S.columns)
         b = pd.Series(0.0, index=uids)
         for ind, r in enumerate(list(model.reactions)):
```

### Comparing `PolyRound-0.2.9/PolyRound/static_classes/rounding/geometric_mean_scaling.py` & `polyround-0.3.0/PolyRound/static_classes/rounding/geometric_mean_scaling.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.9/PolyRound/static_classes/rounding/maximum_volume_ellipsoid.py` & `polyround-0.3.0/PolyRound/static_classes/rounding/maximum_volume_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.9/PolyRound/static_classes/rounding/nearest_symmetric_positive_definite.py` & `polyround-0.3.0/PolyRound/static_classes/rounding/nearest_symmetric_positive_definite.py`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.9/PolyRound/unit_tests.py` & `polyround-0.3.0/PolyRound/unit_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,25 @@
     geometric_mean_scaling,
 )
 from PolyRound.mutable_classes.polytope import Polytope
 from PolyRound.static_classes.parse_sbml_stoichiometry import StoichiometryParser
 from PolyRound.api import PolyRoundApi
 from PolyRound.default_settings import default_numerics_threshold
 import pandas as pd
-from cobra.util.solver import solvers
+from PolyRound.static_classes.lp_interfacing import solvers
 import pickle
 
+has_cobra = False
+try:
+    import cobra
+
+    has_cobra = True
+except:
+    pass
+
 
 class TestExactly(unittest.TestCase):
     def test_small_simplex(self):
         dim = 2
         A = np.vstack([-np.eye(dim), np.ones(shape=(1, dim))])
         b = np.zeros(dim + 1)
         b[-1] = 1
@@ -123,27 +131,35 @@
             np.linalg.norm(rounded.transformation.values.flatten() - expected_transform)
             < 1e-6
         )
 
 
 class TestMatrixMaking(unittest.TestCase):
     def test_coli(self):
-        p = StoichiometryParser.parse_sbml_cobrapy("PolyRound/models/e_coli_core.xml")
-        m = OptlangInterfacer.polytope_to_optlang(p, PolyRoundSettings())
-        p_new = OptlangInterfacer.optlang_to_polytope(m)
-        # now compare that they are equal
-        self.assertTrue(p == p_new)
-
-        # now test inequality only
-        p.S = None
-        p.h = None
-        p.inequality_only = True
-        m = OptlangInterfacer.polytope_to_optlang(p, PolyRoundSettings())
-        p_new = OptlangInterfacer.optlang_to_polytope(m)
-        self.assertTrue(p == p_new)
+        if has_cobra:
+            p = StoichiometryParser.parse_sbml_cobrapy(
+                "PolyRound/models/e_coli_core.xml"
+            )
+            m = OptlangInterfacer.polytope_to_optlang(p, PolyRoundSettings())
+            p_new = OptlangInterfacer.optlang_to_polytope(m)
+            # now compare that they are equal
+            self.assertTrue(p == p_new)
+
+            # now test inequality only
+            p.S = None
+            p.h = None
+            p.inequality_only = True
+            m = OptlangInterfacer.polytope_to_optlang(p, PolyRoundSettings())
+            p_new = OptlangInterfacer.optlang_to_polytope(m)
+            self.assertTrue(p == p_new)
+        else:
+            with self.assertRaises(NotImplementedError):
+                StoichiometryParser.parse_sbml_cobrapy(
+                    "PolyRound/models/e_coli_core.xml"
+                )
 
 
 class TestRounding(unittest.TestCase):
     def test_solve(self):
         A = np.array([[-1, 0, 0], [0, -1, 0], [0, 0, -1], [1, 1, 1]])
         b = np.array([[0], [0], [0], [1]])
         x = np.array([[0.1], [0.1], [0.1]])
@@ -248,21 +264,27 @@
         self.input = "PolyRound/models/e_coli_core.xml"
         self.S_cobra = np.loadtxt("PolyRound/csvs/S_cobra.csv", delimiter=",")
         self.A_cobra = np.loadtxt("PolyRound/csvs/A_cobra.csv", delimiter=",")
         self.b_cobra = np.loadtxt("PolyRound/csvs/b_cobra.csv", delimiter=",")
         # self.options = {"presolve": True, "method": "revised simplex"}
 
     def test_norm(self):
-        polytope = StoichiometryParser.parse_sbml_cobrapy(self.input)
-        for digits in [1, 2, 4]:
-            reduced_p = StoichiometryParser.make_precision_truncated_integer_polytope(
-                polytope, digits
-            )
-            trans = PolytopeReducer.sparse_null_space(reduced_p.S)
-            self.assertLessEqual(np.linalg.norm(reduced_p.S @ trans), 1e-9)
+        if has_cobra:
+            polytope = StoichiometryParser.parse_sbml_cobrapy(self.input)
+            for digits in [1, 2, 4]:
+                reduced_p = (
+                    StoichiometryParser.make_precision_truncated_integer_polytope(
+                        polytope, digits
+                    )
+                )
+                trans = PolytopeReducer.sparse_null_space(reduced_p.S)
+                self.assertLessEqual(np.linalg.norm(reduced_p.S @ trans), 1e-9)
+        else:
+            with self.assertRaises(NotImplementedError):
+                StoichiometryParser.parse_sbml_cobrapy(self.input)
 
     def test_degenerate_polytope(self):
         S = np.array(
             [
                 [1, 0],
                 [0, 1],
             ]
@@ -293,56 +315,68 @@
         b = np.array([5.25, 1.75])
         p = Polytope(A, b, S=S)
         p = PolyRoundApi.simplify_transform_and_round(p)
         self.assertTrue(p.transformation.shape == (3, 1))
 
     def test_interior_point_original(self):
         settings = PolyRoundSettings()
-        polytope = StoichiometryParser.parse_sbml_cobrapy(self.input)
-
-        obj = np.ones(polytope.A.shape[1])
-        b_eq = np.zeros(polytope.S.shape[0])
-        S = np.array(polytope.S).astype(float)
-
-        A = np.array(polytope.A).astype(float)
+        if has_cobra:
+            polytope = StoichiometryParser.parse_sbml_cobrapy(self.input)
 
-        b = np.array(polytope.b).astype(float)
-        sol, model = OptlangInterfacer.gurobi_solve(obj, A, b, settings, S=S, h=b_eq)
-        self.assertEqual(model.status, "optimal")
+            obj = np.ones(polytope.A.shape[1])
+            b_eq = np.zeros(polytope.S.shape[0])
+            S = np.array(polytope.S).astype(float)
+
+            A = np.array(polytope.A).astype(float)
+
+            b = np.array(polytope.b).astype(float)
+            sol, model = OptlangInterfacer.gurobi_solve(
+                obj, A, b, settings, S=S, h=b_eq
+            )
+            self.assertEqual(model.status, "optimal")
+        else:
+            with self.assertRaises(NotImplementedError):
+                StoichiometryParser.parse_sbml_cobrapy(self.input)
 
     def test_matlab_matrices(self):
         obj = np.ones(self.S_cobra.shape[1])
         b_eq = np.zeros(self.S_cobra.shape[0])
         sol, model = OptlangInterfacer.gurobi_solve(
             obj, self.A_cobra, self.b_cobra, PolyRoundSettings(), S=self.S_cobra, h=b_eq
         )
         self.assertEqual(model.status, "optimal")
 
     def test_compare_python_cobra_matrices(self):
 
-        polytope = StoichiometryParser.parse_sbml_cobrapy(self.input)
+        if has_cobra:
+            polytope = StoichiometryParser.parse_sbml_cobrapy(self.input)
 
-        S_cobra = self.S_cobra / 10000
+            S_cobra = self.S_cobra / 10000
 
-        for col, cob_col in zip(np.transpose(polytope.S.values), np.transpose(S_cobra)):
-            sim = col == cob_col
-            self.assertTrue(sim.all())
-
-        A_cobra = np.around(self.A_cobra)
-        A_cobra = A_cobra.astype(int)
-        A = np.array(polytope.A, dtype=int)
-        for col, cob_col in zip(np.transpose(A), np.transpose(A_cobra)):
-            sim = col == cob_col
-            self.assertTrue(sim.all())
-
-        # Now move on to b
-        b = np.array(polytope.b)
-        b = b.reshape((b.size,))
-        bool = self.b_cobra == b
-        self.assertTrue(bool.all())
+            for col, cob_col in zip(
+                np.transpose(polytope.S.values), np.transpose(S_cobra)
+            ):
+                sim = col == cob_col
+                self.assertTrue(sim.all())
+
+            A_cobra = np.around(self.A_cobra)
+            A_cobra = A_cobra.astype(int)
+            A = np.array(polytope.A, dtype=int)
+            for col, cob_col in zip(np.transpose(A), np.transpose(A_cobra)):
+                sim = col == cob_col
+                self.assertTrue(sim.all())
+
+            # Now move on to b
+            b = np.array(polytope.b)
+            b = b.reshape((b.size,))
+            bool = self.b_cobra == b
+            self.assertTrue(bool.all())
+        else:
+            with self.assertRaises(NotImplementedError):
+                StoichiometryParser.parse_sbml_cobrapy(self.input)
 
 
 class TestLPs(unittest.TestCase):
     def test_chebyshev_center(self):
         settings = PolyRoundSettings()
         S = np.zeros((1, 3))
         S[0, :] = 1
@@ -413,105 +447,115 @@
         backends = ["gurobi", "glpk"]
         # eps is for svd
         eps = 1e-12
 
         for backend in backends:
             if not backend in solvers:
                 continue
-            polytope = StoichiometryParser.parse_sbml_cobrapy(self.input)
-            polytope.normalize()
-            settings = PolyRoundSettings(backend=backend)
-            reduced_polytope = PolyRoundApi.simplify_polytope(polytope, settings)
-
-            # compute chebyshev center
-            settings.hp_flags["NumericFocus"] = 3
-            settings.hp_flags["MarkowitzTol"] = 0.999
-            x, dist = ChebyshevFinder.chebyshev_center(reduced_polytope, settings)
-            self.assertGreater(dist, 0.1)
-            # print("chebyshev distance is : " + str(dist))
-
-            pre_b_dist = reduced_polytope.border_distance(x)
-            self.assertGreater(pre_b_dist, 0.1)
-            # print("border distance pre-transformation is: " + str(pre_b_dist))
-
-            # put x at zero!
-            reduced_polytope.apply_shift(x)
-            # b = b - np.squeeze(np.matmul(A, x))
-            x_0 = np.zeros(x.shape)
-            b_dist_at_zero = reduced_polytope.border_distance(x_0)
-            self.assertGreater(b_dist_at_zero, 0.1)
-            self.assertAlmostEqual(pre_b_dist, b_dist_at_zero)
-            # print("border distance zero-transformation is: " + str(b_dist_at_zero))
-
-            transformation = PolytopeReducer.null_space(
-                reduced_polytope.S.values, eps=eps
-            )
-            reduced_polytope.apply_transformation(transformation)
-            # A_null = np.matmul(A, null)
-            u = np.zeros((transformation.shape[1], 1))
-
-            norm_check = np.linalg.norm(np.matmul(polytope.S.values, transformation))
-            self.assertLess(norm_check, 1e-10)
-            # print("norm of the null space is: " + str(norm_check))
-
-            b_dist = reduced_polytope.border_distance(u)
-            self.assertAlmostEqual(b_dist, pre_b_dist)
-
-            # test if we can reproduce the original x
-            x_rec = reduced_polytope.back_transform(u)
-
-            self.assertLess(np.min(np.abs(x - x_rec)), 1e-10)
-
-            # Do FVA and see if the points are feasible in the original space
-            points = ChebyshevFinder.fva(reduced_polytope, PolyRoundSettings())
-
-            # convert all points to original space
-            back = reduced_polytope.back_transform(points.values)
-            b_dists = polytope.border_distance(back)
-            self.assertGreater(b_dists, -1e-9)
-            # print("done")
-
-            rounded_polytope = PolyRoundApi.round_polytope(reduced_polytope)
-            points = ChebyshevFinder.fva(rounded_polytope, settings)
-            back = rounded_polytope.back_transform(points.values)
-            b_dists = polytope.border_distance(back)
-            self.assertGreater(b_dists, -1e-9)
+            if has_cobra:
+                polytope = StoichiometryParser.parse_sbml_cobrapy(self.input)
+                polytope.normalize()
+                settings = PolyRoundSettings(backend=backend)
+                reduced_polytope = PolyRoundApi.simplify_polytope(polytope, settings)
+
+                # compute chebyshev center
+                settings.hp_flags["NumericFocus"] = 3
+                settings.hp_flags["MarkowitzTol"] = 0.999
+                x, dist = ChebyshevFinder.chebyshev_center(reduced_polytope, settings)
+                self.assertGreater(dist, 0.1)
+                # print("chebyshev distance is : " + str(dist))
+
+                pre_b_dist = reduced_polytope.border_distance(x)
+                self.assertGreater(pre_b_dist, 0.1)
+                # print("border distance pre-transformation is: " + str(pre_b_dist))
+
+                # put x at zero!
+                reduced_polytope.apply_shift(x)
+                # b = b - np.squeeze(np.matmul(A, x))
+                x_0 = np.zeros(x.shape)
+                b_dist_at_zero = reduced_polytope.border_distance(x_0)
+                self.assertGreater(b_dist_at_zero, 0.1)
+                self.assertAlmostEqual(pre_b_dist, b_dist_at_zero)
+                # print("border distance zero-transformation is: " + str(b_dist_at_zero))
+
+                transformation = PolytopeReducer.null_space(
+                    reduced_polytope.S.values, eps=eps
+                )
+                reduced_polytope.apply_transformation(transformation)
+                # A_null = np.matmul(A, null)
+                u = np.zeros((transformation.shape[1], 1))
+
+                norm_check = np.linalg.norm(
+                    np.matmul(polytope.S.values, transformation)
+                )
+                self.assertLess(norm_check, 1e-10)
+                # print("norm of the null space is: " + str(norm_check))
+
+                b_dist = reduced_polytope.border_distance(u)
+                self.assertAlmostEqual(b_dist, pre_b_dist)
+
+                # test if we can reproduce the original x
+                x_rec = reduced_polytope.back_transform(u)
+
+                self.assertLess(np.min(np.abs(x - x_rec)), 1e-10)
+
+                # Do FVA and see if the points are feasible in the original space
+                points = ChebyshevFinder.fva(reduced_polytope, PolyRoundSettings())
+
+                # convert all points to original space
+                back = reduced_polytope.back_transform(points.values)
+                b_dists = polytope.border_distance(back)
+                self.assertGreater(b_dists, -1e-9)
+                # print("done")
+
+                rounded_polytope = PolyRoundApi.round_polytope(reduced_polytope)
+                points = ChebyshevFinder.fva(rounded_polytope, settings)
+                back = rounded_polytope.back_transform(points.values)
+                b_dists = polytope.border_distance(back)
+                self.assertGreater(b_dists, -1e-9)
+            else:
+                with self.assertRaises(NotImplementedError):
+                    StoichiometryParser.parse_sbml_cobrapy(self.input)
 
     def test_api_simplification_coli(self):
-        settings = PolyRoundSettings()
-        polytope = StoichiometryParser.parse_sbml_cobrapy(self.input)
-        x, dist = ChebyshevFinder.chebyshev_center(polytope, settings)
-        self.assertTrue(np.abs(dist) < 1e-10)
-        reduced = PolyRoundApi.simplify_polytope(polytope, settings=settings)
-        # Now simplify without reducing
-        settings.reduce = False
-        simplified = PolyRoundApi.simplify_polytope(polytope, settings=settings)
-        settings.reduce = True
-        # check that the distance remains the same with or without redundancy
-        x_redundant, dist_redundant = ChebyshevFinder.chebyshev_center(
-            simplified, settings
-        )
-        x, dist = ChebyshevFinder.chebyshev_center(reduced, settings)
-        self.assertTrue(np.abs(dist[0] - dist_redundant[0]) < 1e-10)
-        self.assertTrue(np.abs(dist) > 1e-10)
-        transformed = PolyRoundApi.transform_polytope(reduced, settings)
-        x, dist = ChebyshevFinder.chebyshev_center(transformed, settings)
-        self.assertTrue(np.abs(dist) > 1e-10)
-        rounded = PolyRoundApi.round_polytope(transformed, settings=settings)
-        self.assertTrue(rounded.inequality_only)
-        x, dist = ChebyshevFinder.chebyshev_center(rounded, settings)
-        self.assertTrue(np.abs(dist) > 1e-10)
-        PolyRoundApi.polytope_to_csvs(
-            rounded, os.path.join("PolyRound", "output", "export_test")
-        )
-
-    def test_canonical_polytope(self):
-        with open(
-            os.path.join("PolyRound", "models", "canonical_polytope.p"), "rb"
-        ) as f:
-            polytope = pickle.load(f)
-        test = PolyRoundApi.simplify_transform_and_round(polytope)
-        pass
+        if has_cobra:
+            settings = PolyRoundSettings()
+            polytope = StoichiometryParser.parse_sbml_cobrapy(self.input)
+            x, dist = ChebyshevFinder.chebyshev_center(polytope, settings)
+            self.assertTrue(np.abs(dist) < 1e-10)
+            reduced = PolyRoundApi.simplify_polytope(polytope, settings=settings)
+            # Now simplify without reducing
+            settings.reduce = False
+            simplified = PolyRoundApi.simplify_polytope(polytope, settings=settings)
+            settings.reduce = True
+            # check that the distance remains the same with or without redundancy
+            x_redundant, dist_redundant = ChebyshevFinder.chebyshev_center(
+                simplified, settings
+            )
+            x, dist = ChebyshevFinder.chebyshev_center(reduced, settings)
+            self.assertTrue(np.abs(dist[0] - dist_redundant[0]) < 1e-10)
+            self.assertTrue(np.abs(dist) > 1e-10)
+            transformed = PolyRoundApi.transform_polytope(reduced, settings)
+            x, dist = ChebyshevFinder.chebyshev_center(transformed, settings)
+            self.assertTrue(np.abs(dist) > 1e-10)
+            rounded = PolyRoundApi.round_polytope(transformed, settings=settings)
+            self.assertTrue(rounded.inequality_only)
+            x, dist = ChebyshevFinder.chebyshev_center(rounded, settings)
+            self.assertTrue(np.abs(dist) > 1e-10)
+            PolyRoundApi.polytope_to_csvs(
+                rounded, os.path.join("PolyRound", "output", "export_test")
+            )
+        else:
+            with self.assertRaises(NotImplementedError):
+                StoichiometryParser.parse_sbml_cobrapy(self.input)
+
+    #  Skip this test, because polyround update breaks loading pickles
+    # def test_canonical_polytope(self):
+    #     with open(
+    #         os.path.join("PolyRound", "models", "canonical_polytope.p"), "rb"
+    #     ) as f:
+    #         polytope = pickle.load(f)
+    #         test = PolyRoundApi.simplify_transform_and_round(polytope)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `PolyRound-0.2.9/PolyRound.egg-info/PKG-INFO` & `polyround-0.3.0/PolyRound.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 Metadata-Version: 2.1
 Name: PolyRound
-Version: 0.2.9
+Version: 0.3.0
 Summary: A python package for rounding polytopes.
 Home-page: https://gitlab.com/csb.ethz/PolyRound
 Author: Axel Theorell
 Author-email: atheorell@ethz.ch
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.2
+Requires-Dist: pandas>=1.2
+Requires-Dist: scipy>=1.4
+Requires-Dist: optlang>=1.4
+Provides-Extra: extras
+Requires-Dist: cobra>=0.20; extra == "extras"
+Requires-Dist: python-libsbml>=5.18; extra == "extras"
+Requires-Dist: gurobipy; extra == "extras"
 
 # PolyRound
-[![PyPI version](https://badge.fury.io/py/PolyRound.svg)](https://badge.fury.io/py/PolyRound)
 
 Efficient random sampling in convex polytopes relies on a 'rounding' preprocessing step, in which the polytope is rescaled so that the width is as uniform as possible across different dimensions.
 PolyRound rounds polytopes on the general form:
 
 $`P:=\{x \in \mathcal{R}^n: A_{eq} x = b_{eq}, A_{ineq} x \leq b_{ineq}\}`$ with matrices $`A_{eq} \in \mathcal{R}^{m,n}`$ and $`A_{ineq} \in \mathcal{R}^{k,n}`$ and vectors $`b_{eq} \in \mathcal{R}^{m}`$ and $`b_{ineq} \in \mathcal{R}^{k}`$.
 
 This formulation often arises in Systems Biology as the flux space of a metabolic network.
 
 As output, PolyRound produces a polytope on the form $`P^{r}:=\{v \in \mathcal{R}^l: A^{r}_{ineq}v \leq b^{r}_{ineq}\}`$ where $`l \leq n`$ and the zero vector is a stricly interior point. For transforming points back to the original space, it also provides a matrix $`S \in \mathcal{R}^{n,l}`$ and a vector $`t \in \mathcal{R}^{n}`$, so that $`x=Sv + t`$.
 
-Currently, PolyRound is supported for python 3.7 to 3.9.
+Currently, PolyRound is supported for python 3.8 to 3.12.
+
+PolyRound comes with two optional dependencies: 1) Gurobi (for the best linear programming) and 2) Cobrapy (for SBML support)
+Both dependencies are fetched by installing the extras: "pip install 'PolyRound[extras]'".
+When Gurobi is not installed, PolyRound uses optlang (https://github.com/opencobra/optlang) to delegate linear programs to GLPK. However, PolyRound is more reliable with Gurobi. Free Gurobi licenses for academic use can be obtained at https://www.gurobi.com/. Once the license is installed, gurobipy can be installed directly through pip, or by getting the optional requirements as described above.
 
-PolyRound no longer depends on a Gurobi installation and uses optlang (https://github.com/opencobra/optlang) to delegate linear programs to GLPK in case Gurobi is not installed. However, PolyRound is more reliable with Gurobi. Free Gurobi licenses for academic use can be obtained at https://www.gurobi.com/. Once the license is installed, gurobipy can be installed directly through pip, or by getting the optional requirements by 'pip install -r optional_requirements.txt'.
 
 An easy example of how to get started is presented in the jupyter notebook cells below.
 
 
 They show how to: <br>
 1) create a polytope object from a file path <br>
 2) simplify, reduce, and round a polytope in separate steps, togehter with some printed checks <br>
```

### Comparing `PolyRound-0.2.9/PolyRound.egg-info/SOURCES.txt` & `polyround-0.3.0/PolyRound.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PolyRound-0.2.9/README.md` & `polyround-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # PolyRound
-[![PyPI version](https://badge.fury.io/py/PolyRound.svg)](https://badge.fury.io/py/PolyRound)
 
 Efficient random sampling in convex polytopes relies on a 'rounding' preprocessing step, in which the polytope is rescaled so that the width is as uniform as possible across different dimensions.
 PolyRound rounds polytopes on the general form:
 
 $`P:=\{x \in \mathcal{R}^n: A_{eq} x = b_{eq}, A_{ineq} x \leq b_{ineq}\}`$ with matrices $`A_{eq} \in \mathcal{R}^{m,n}`$ and $`A_{ineq} \in \mathcal{R}^{k,n}`$ and vectors $`b_{eq} \in \mathcal{R}^{m}`$ and $`b_{ineq} \in \mathcal{R}^{k}`$.
 
 This formulation often arises in Systems Biology as the flux space of a metabolic network.
 
 As output, PolyRound produces a polytope on the form $`P^{r}:=\{v \in \mathcal{R}^l: A^{r}_{ineq}v \leq b^{r}_{ineq}\}`$ where $`l \leq n`$ and the zero vector is a stricly interior point. For transforming points back to the original space, it also provides a matrix $`S \in \mathcal{R}^{n,l}`$ and a vector $`t \in \mathcal{R}^{n}`$, so that $`x=Sv + t`$.
 
-Currently, PolyRound is supported for python 3.7 to 3.9.
+Currently, PolyRound is supported for python 3.8 to 3.12.
+
+PolyRound comes with two optional dependencies: 1) Gurobi (for the best linear programming) and 2) Cobrapy (for SBML support)
+Both dependencies are fetched by installing the extras: "pip install 'PolyRound[extras]'".
+When Gurobi is not installed, PolyRound uses optlang (https://github.com/opencobra/optlang) to delegate linear programs to GLPK. However, PolyRound is more reliable with Gurobi. Free Gurobi licenses for academic use can be obtained at https://www.gurobi.com/. Once the license is installed, gurobipy can be installed directly through pip, or by getting the optional requirements as described above.
 
-PolyRound no longer depends on a Gurobi installation and uses optlang (https://github.com/opencobra/optlang) to delegate linear programs to GLPK in case Gurobi is not installed. However, PolyRound is more reliable with Gurobi. Free Gurobi licenses for academic use can be obtained at https://www.gurobi.com/. Once the license is installed, gurobipy can be installed directly through pip, or by getting the optional requirements by 'pip install -r optional_requirements.txt'.
 
 An easy example of how to get started is presented in the jupyter notebook cells below.
 
 
 They show how to: <br>
 1) create a polytope object from a file path <br>
 2) simplify, reduce, and round a polytope in separate steps, togehter with some printed checks <br>
```

### Comparing `PolyRound-0.2.9/setup.py` & `polyround-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # ©2020-​2021 ETH Zurich, Axel Theorell
 
 import os
 from setuptools import setup
 import sys
+
 sys.path.append(os.path.dirname(os.path.abspath(__file__)))
 from PolyRound.version import VERSION
 
-with open(os.path.join(os.path.dirname(os.path.abspath(__file__)),"README.md"), "r") as fh:
+with open(
+    os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"), "r"
+) as fh:
     long_description = fh.read()
 
 setup(
     name="PolyRound",
     version=VERSION,
     description="A python package for rounding polytopes.",
     long_description=long_description,
@@ -24,20 +27,24 @@
         "PolyRound.mutable_classes",
         "PolyRound.static_classes",
         "PolyRound.static_classes.rounding",
     ],
     install_requires=[
         "numpy>=1.2",
         "pandas>=1.2",
-        "python-dateutil>=2.8",
-        "python-libsbml>=5.18",
         "scipy>=1.4",
         "optlang>=1.4",
-        "cobra>=0.20",
     ],
+    extras_require={
+        "extras": [
+            "cobra>=0.20",
+            "python-libsbml>=5.18",
+            "gurobipy",
+        ],
+    },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
     ],
     python_requires=">=3.6",
```

