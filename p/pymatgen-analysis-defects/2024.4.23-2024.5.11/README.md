# Comparing `tmp/pymatgen_analysis_defects-2024.4.23.tar.gz` & `tmp/pymatgen_analysis_defects-2024.5.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatgen_analysis_defects-2024.4.23.tar", last modified: Mon Apr 22 22:38:52 2024, max compression
+gzip compressed data, was "pymatgen_analysis_defects-2024.5.11.tar", last modified: Sat May 11 18:04:09 2024, max compression
```

## Comparing `pymatgen_analysis_defects-2024.4.23.tar` & `pymatgen_analysis_defects-2024.5.11.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:52.462129 pymatgen_analysis_defects-2024.4.23/
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-04-22 22:38:52.462129 pymatgen_analysis_defects-2024.4.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:52.454129 pymatgen_analysis_defects-2024.4.23/pymatgen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:52.454129 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:52.458129 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    26337 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/ccd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    40256 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:52.458129 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/corrections/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/corrections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15690 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/corrections/freysoldt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/corrections/kumagai.py
--rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    21880 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:52.458129 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/plotting/optics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/plotting/phases.py
--rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/recombination.py
--rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/supercells.py
--rw-r--r--   0 runner    (1001) docker     (127)    51742 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/thermo.py
--rw-r--r--   0 runner    (1001) docker     (127)    41845 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:38:52.462129 pymatgen_analysis_defects-2024.4.23/pymatgen_analysis_defects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-04-22 22:38:52.000000 pymatgen_analysis_defects-2024.4.23/pymatgen_analysis_defects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-22 22:38:52.000000 pymatgen_analysis_defects-2024.4.23/pymatgen_analysis_defects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:38:52.000000 pymatgen_analysis_defects-2024.4.23/pymatgen_analysis_defects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-22 22:38:52.000000 pymatgen_analysis_defects-2024.4.23/pymatgen_analysis_defects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-22 22:38:52.000000 pymatgen_analysis_defects-2024.4.23/pymatgen_analysis_defects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-22 22:38:46.000000 pymatgen_analysis_defects-2024.4.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:38:52.462129 pymatgen_analysis_defects-2024.4.23/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:04:09.889463 pymatgen_analysis_defects-2024.5.11/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-11 18:04:09.889463 pymatgen_analysis_defects-2024.5.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:04:09.881463 pymatgen_analysis_defects-2024.5.11/pymatgen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:04:09.881463 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:04:09.885463 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26337 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/ccd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41380 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:04:09.885463 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/corrections/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/corrections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15690 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/corrections/freysoldt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/corrections/kumagai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12760 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21880 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:04:09.885463 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/plotting/optics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/plotting/phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/recombination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/supercells.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51742 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41853 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:04:09.885463 pymatgen_analysis_defects-2024.5.11/pymatgen_analysis_defects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-11 18:04:09.000000 pymatgen_analysis_defects-2024.5.11/pymatgen_analysis_defects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-11 18:04:09.000000 pymatgen_analysis_defects-2024.5.11/pymatgen_analysis_defects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 18:04:09.000000 pymatgen_analysis_defects-2024.5.11/pymatgen_analysis_defects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-11 18:04:09.000000 pymatgen_analysis_defects-2024.5.11/pymatgen_analysis_defects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-11 18:04:09.000000 pymatgen_analysis_defects-2024.5.11/pymatgen_analysis_defects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-11 18:04:00.000000 pymatgen_analysis_defects-2024.5.11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 18:04:09.889463 pymatgen_analysis_defects-2024.5.11/setup.cfg
```

### Comparing `pymatgen_analysis_defects-2024.4.23/LICENSE` & `pymatgen_analysis_defects-2024.5.11/LICENSE`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/PKG-INFO` & `pymatgen_analysis_defects-2024.5.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2024.4.23
+Version: 2024.5.11
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
@@ -31,20 +31,20 @@
 Provides-Extra: docs
 Requires-Dist: jupyter-book>=0.13.1; extra == "docs"
 Provides-Extra: optional
 Requires-Dist: pydefect>=0.6.2; extra == "optional"
 Requires-Dist: dscribe>=2.0.0; extra == "optional"
 Requires-Dist: numba; extra == "optional"
 Provides-Extra: strict
-Requires-Dist: pymatgen==2024.3.1; extra == "strict"
+Requires-Dist: pymatgen==2024.5.1; extra == "strict"
 Requires-Dist: dscribe==2.1.0; extra == "strict"
 Requires-Dist: scikit-image==0.22.0; extra == "strict"
 Requires-Dist: mp-pyrho==0.4.4; extra == "strict"
 Provides-Extra: tests
-Requires-Dist: pytest==8.1.1; extra == "tests"
+Requires-Dist: pytest==8.2.0; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0; extra == "tests"
 Requires-Dist: nbmake==1.5.3; extra == "tests"
 
 # pymatgen-analysis-defects
 
 [![testing](https://github.com/materialsproject/pymatgen-analysis-defects/actions/workflows/testing.yml/badge.svg?branch=main)](https://github.com/materialsproject/pymatgen-analysis-defects/actions/workflows/testing.yml)
 [![codecov](https://codecov.io/gh/materialsproject/pymatgen-analysis-defects/branch/main/graph/badge.svg?token=FOKXRCZTXZ)](https://codecov.io/gh/materialsproject/pymatgen-analysis-defects)
```

### Comparing `pymatgen_analysis_defects-2024.4.23/README.md` & `pymatgen_analysis_defects-2024.5.11/README.md`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/README.rst` & `pymatgen_analysis_defects-2024.5.11/README.rst`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/ccd.py` & `pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/ccd.py`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/constants.py` & `pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/constants.py`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/core.py` & `pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 import numpy as np
 from monty.json import MSONable
 from pymatgen.analysis.defects.supercells import get_sc_fromstruct
 from pymatgen.analysis.structure_matcher import ElementComparator, StructureMatcher
 from pymatgen.core import Element, PeriodicSite, Species
 from pymatgen.core.periodic_table import DummySpecies
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
-from typing_extensions import Self
 
 from .utils import get_plane_spacing
 
 if TYPE_CHECKING:
     from numpy.typing import ArrayLike
     from pymatgen.core import Structure
     from pymatgen.symmetry.structure import SymmetrizedStructure
+    from typing_extensions import Self
 
 # TODO Possible redesign idea: ``DefectSite`` class defined with a defect object.
 # This makes some of the accounting logic a bit harder since we will probably
 # just have one concrete ``Defect`` class so you can write custom multiplicity functions
 # but it makes the implementation of defect complexes trivial.
 # i.e. each defect will be defined by a structure and a collection of ``DefectSite``s
 
@@ -508,30 +508,47 @@
 
     def __init__(
         self,
         structure: Structure,
         site: PeriodicSite,
         multiplicity: int | None = None,
         oxi_state: float | None = None,
-        **kwargs,
+        equivalent_sites: list[PeriodicSite] | None = None,
+        symprec: float = 0.01,
+        angle_tolerance: float = 5,
+        user_charges: list[int] | None = None,
     ) -> None:
         """Initialize a substitutional defect object.
 
         The position of `site` determines the atom to be removed and the species of
         `site` determines the replacing species.
 
         Args:
             structure: The structure of the defect.
             site: Replace the nearest site with this one.
             multiplicity: The multiplicity of the defect.
             oxi_state: The oxidation state of the defect, if not specified,
                 this will be determined automatically.
-            **kwargs: Additional kwargs to pass to the Defect constructor.
+            equivalent_sites: A list of equivalent sites for the defect in the structure.
+            symprec: Tolerance for symmetry finding.
+            angle_tolerance: Angle tolerance for symmetry finding.
+            user_charges: User specified charge states. If specified,
+                ``get_charge_states`` will return this list. If ``None`` or empty list
+                the charge states will be determined automatically.
         """
-        super().__init__(structure, site, multiplicity, oxi_state, **kwargs)
+        super().__init__(
+            structure=structure,
+            site=site,
+            multiplicity=multiplicity,
+            oxi_state=oxi_state,
+            equivalent_sites=equivalent_sites,
+            symprec=symprec,
+            angle_tolerance=angle_tolerance,
+            user_charges=user_charges,
+        )
 
     def get_multiplicity(self) -> int:
         """Returns the multiplicity of a defect site within the structure.
 
         This is required for concentration analysis and confirms that defect_site is
         a site in bulk_structure.
         """
@@ -639,36 +656,42 @@
     def __init__(
         self,
         structure: Structure,
         site: PeriodicSite,
         multiplicity: int = 1,
         oxi_state: float | None = None,
         equivalent_sites: list[PeriodicSite] | None = None,
-        **kwargs,
+        symprec: float = 0.01,
+        angle_tolerance: float = 5,
+        user_charges: list[int] | None = None,
     ) -> None:
         """Initialize an interstitial defect object.
 
         The interstitial defect effectively inserts the `site` object into the structure.
 
         Args:
             structure: The structure of the defect.
             site: Inserted site, also determines the species.
             multiplicity: The multiplicity of the defect.
             oxi_state: The oxidation state of the defect, if not specified,
                 this will be determined automatically.
             equivalent_sites: A list of equivalent sites for the defect in the structure.
-            **kwargs: Additional kwargs to pass to the Defect constructor.
+            symprec: Tolerance for symmetry finding.
+            angle_tolerance: Angle tolerance for symmetry finding.
+            user_charges: User specified charge states. If specified,
         """
         super().__init__(
-            structure,
-            site,
-            multiplicity,
-            oxi_state,
-            equivalent_sites,
-            **kwargs,
+            structure=structure,
+            site=site,
+            multiplicity=multiplicity,
+            oxi_state=oxi_state,
+            equivalent_sites=equivalent_sites,
+            symprec=symprec,
+            angle_tolerance=angle_tolerance,
+            user_charges=user_charges,
         )
 
     def get_multiplicity(self) -> int:
         """Determine the multiplicity of the defect site within the structure."""
         msg = "Interstitial multiplicity should be determined by the generator."
         raise NotImplementedError(
             msg,
```

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/corrections/freysoldt.py` & `pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/corrections/freysoldt.py`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/corrections/kumagai.py` & `pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/corrections/kumagai.py`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/finder.py` & `pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/finder.py`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/generators.py` & `pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/generators.py`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/plotting/optics.py` & `pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/plotting/optics.py`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/plotting/phases.py` & `pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/plotting/phases.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Plotting functions for competing phases."""
 
-# %%
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
 from matplotlib import pyplot as plt
 from matplotlib.patches import Polygon
```

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/recombination.py` & `pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/recombination.py`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/supercells.py` & `pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/supercells.py`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/thermo.py` & `pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/thermo.py`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen/analysis/defects/utils.py` & `pymatgen_analysis_defects-2024.5.11/pymatgen/analysis/defects/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,16 +419,16 @@
     def _dist_mat(pos_frac: npt.ArrayLike) -> npt.NDArray:
         # return a matrix that contains the distances
         aa = np.linspace(0, 1, len(chgcar.get_axis_grid(0)), endpoint=False)
         bb = np.linspace(0, 1, len(chgcar.get_axis_grid(1)), endpoint=False)
         cc = np.linspace(0, 1, len(chgcar.get_axis_grid(2)), endpoint=False)
         AA, BB, CC = np.meshgrid(aa, bb, cc, indexing="ij")
         dist_from_pos = chgcar.structure.lattice.get_all_distances(
-            fcoords1=np.vstack([AA.flatten(), BB.flatten(), CC.flatten()]).T,
-            fcoords2=pos_frac,
+            frac_coords1=np.vstack([AA.flatten(), BB.flatten(), CC.flatten()]).T,
+            frac_coords2=pos_frac,
         )
         return dist_from_pos.reshape(AA.shape)
 
     if np.any(fcoord < 0) or np.any(fcoord > 1):
         msg = "f_coords must be in [0,1)"
         raise ValueError(msg)
     mask = _dist_mat(fcoord) < radius
```

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen_analysis_defects.egg-info/PKG-INFO` & `pymatgen_analysis_defects-2024.5.11/pymatgen_analysis_defects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2024.4.23
+Version: 2024.5.11
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
@@ -31,20 +31,20 @@
 Provides-Extra: docs
 Requires-Dist: jupyter-book>=0.13.1; extra == "docs"
 Provides-Extra: optional
 Requires-Dist: pydefect>=0.6.2; extra == "optional"
 Requires-Dist: dscribe>=2.0.0; extra == "optional"
 Requires-Dist: numba; extra == "optional"
 Provides-Extra: strict
-Requires-Dist: pymatgen==2024.3.1; extra == "strict"
+Requires-Dist: pymatgen==2024.5.1; extra == "strict"
 Requires-Dist: dscribe==2.1.0; extra == "strict"
 Requires-Dist: scikit-image==0.22.0; extra == "strict"
 Requires-Dist: mp-pyrho==0.4.4; extra == "strict"
 Provides-Extra: tests
-Requires-Dist: pytest==8.1.1; extra == "tests"
+Requires-Dist: pytest==8.2.0; extra == "tests"
 Requires-Dist: pytest-cov==4.1.0; extra == "tests"
 Requires-Dist: nbmake==1.5.3; extra == "tests"
 
 # pymatgen-analysis-defects
 
 [![testing](https://github.com/materialsproject/pymatgen-analysis-defects/actions/workflows/testing.yml/badge.svg?branch=main)](https://github.com/materialsproject/pymatgen-analysis-defects/actions/workflows/testing.yml)
 [![codecov](https://codecov.io/gh/materialsproject/pymatgen-analysis-defects/branch/main/graph/badge.svg?token=FOKXRCZTXZ)](https://codecov.io/gh/materialsproject/pymatgen-analysis-defects)
```

### Comparing `pymatgen_analysis_defects-2024.4.23/pymatgen_analysis_defects.egg-info/SOURCES.txt` & `pymatgen_analysis_defects-2024.5.11/pymatgen_analysis_defects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymatgen_analysis_defects-2024.4.23/pyproject.toml` & `pymatgen_analysis_defects-2024.5.11/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 dev = ["pre-commit>=2.12.1"]
 docs = [
   "jupyter-book>=0.13.1",
 ]
 optional = ["pydefect>=0.6.2", "dscribe>=2.0.0", "numba"]
 
 strict = [
-  "pymatgen==2024.3.1",
+  "pymatgen==2024.5.1",
   "dscribe==2.1.0",
   "scikit-image==0.22.0",
   "mp-pyrho==0.4.4",
 ]
 
-tests = ["pytest==8.1.1", "pytest-cov==4.1.0", "nbmake==1.5.3"]
+tests = ["pytest==8.2.0", "pytest-cov==4.1.0", "nbmake==1.5.3"]
 
 [tool.setuptools.dynamic]
 readme = { file = ["README.md"] }
 
 [project.urls]
 documentation = "https://materialsproject.github.io/pymatgen-analysis-defects/"
 homepage = "https://materialsproject.github.io/pymatgen-analysis-defects/"
```

