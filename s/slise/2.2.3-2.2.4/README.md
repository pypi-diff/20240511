# Comparing `tmp/slise-2.2.3.tar.gz` & `tmp/slise-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slise-2.2.3.tar", last modified: Tue Dec 19 09:53:55 2023, max compression
+gzip compressed data, was "slise-2.2.4.tar", last modified: Sat May 11 12:01:11 2024, max compression
```

## Comparing `slise-2.2.3.tar` & `slise-2.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 09:53:55.930664 slise-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-12-19 09:53:42.000000 slise-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2023-12-19 09:53:55.930664 slise-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2023-12-19 09:53:42.000000 slise-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-12-19 09:53:42.000000 slise-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 09:53:55.930664 slise-2.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 09:53:55.930664 slise-2.2.3/slise/
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-19 09:53:42.000000 slise-2.2.3/slise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10496 2023-12-19 09:53:42.000000 slise-2.2.3/slise/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12486 2023-12-19 09:53:42.000000 slise-2.2.3/slise/initialisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25782 2023-12-19 09:53:42.000000 slise-2.2.3/slise/optimisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25022 2023-12-19 09:53:42.000000 slise-2.2.3/slise/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    43766 2023-12-19 09:53:42.000000 slise-2.2.3/slise/slise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2023-12-19 09:53:42.000000 slise-2.2.3/slise/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 09:53:55.930664 slise-2.2.3/slise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2023-12-19 09:53:55.000000 slise-2.2.3/slise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-19 09:53:55.000000 slise-2.2.3/slise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 09:53:55.000000 slise-2.2.3/slise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-12-19 09:53:55.000000 slise-2.2.3/slise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-19 09:53:55.000000 slise-2.2.3/slise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 09:53:55.930664 slise-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2023-12-19 09:53:42.000000 slise-2.2.3/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2023-12-19 09:53:42.000000 slise-2.2.3/tests/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-12-19 09:53:42.000000 slise-2.2.3/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2023-12-19 09:53:42.000000 slise-2.2.3/tests/test_slise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:01:11.896476 slise-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 12:01:07.000000 slise-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-11 12:01:11.892476 slise-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-11 12:01:07.000000 slise-2.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-11 12:01:07.000000 slise-2.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:01:11.896476 slise-2.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:01:11.892476 slise-2.2.4/slise/
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-11 12:01:07.000000 slise-2.2.4/slise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-05-11 12:01:07.000000 slise-2.2.4/slise/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12468 2024-05-11 12:01:07.000000 slise-2.2.4/slise/initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25862 2024-05-11 12:01:07.000000 slise-2.2.4/slise/optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25578 2024-05-11 12:01:07.000000 slise-2.2.4/slise/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44334 2024-05-11 12:01:07.000000 slise-2.2.4/slise/slise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-11 12:01:07.000000 slise-2.2.4/slise/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:01:11.892476 slise-2.2.4/slise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-11 12:01:11.000000 slise-2.2.4/slise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-11 12:01:11.000000 slise-2.2.4/slise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:01:11.000000 slise-2.2.4/slise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-11 12:01:11.000000 slise-2.2.4/slise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 12:01:11.000000 slise-2.2.4/slise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:01:11.892476 slise-2.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-11 12:01:07.000000 slise-2.2.4/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-05-11 12:01:07.000000 slise-2.2.4/tests/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-11 12:01:07.000000 slise-2.2.4/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8858 2024-05-11 12:01:07.000000 slise-2.2.4/tests/test_slise.py
```

### Comparing `slise-2.2.3/LICENSE` & `slise-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slise-2.2.3/PKG-INFO` & `slise-2.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slise
-Version: 2.2.3
+Version: 2.2.4
 Summary: The SLISE algorithm for robust regression and explanations of black box models
 Author-email: Anton Björklund <anton.bjorklund@helsinki.fi>
 License: MIT License
         
         Copyright (c) 2022 Anton Björklund
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,17 +40,19 @@
 Requires-Dist: numpy>=1.20
 Requires-Dist: scipy>=1.6
 Requires-Dist: numba>=0.53
 Requires-Dist: matplotlib>=3.3
 Requires-Dist: PyLBFGS>=0.2
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: IPython; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Provides-Extra: tbb
 Requires-Dist: tbb; extra == "tbb"
 
 ![PySLISE Banner Image](docs/pyslise_banner.webp)  
 [![PyPI](https://img.shields.io/pypi/v/slise)](https://pypi.org/project/slise/)
 [![Documentation](https://github.com/edahelsinki/pyslise/actions/workflows/python-docs.yml/badge.svg)](https://edahelsinki.github.io/pyslise/docs/slise/)
 [![Tests](https://github.com/edahelsinki/pyslise/actions/workflows/python-pytest.yml/badge.svg)](https://github.com/edahelsinki/pyslise/actions/workflows/python-pytest.yml)
```

### Comparing `slise-2.2.3/README.md` & `slise-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `slise-2.2.3/pyproject.toml` & `slise-2.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "slise"
-version = "2.2.3"
+version = "2.2.4"
 authors = [{ name = "Anton Björklund", email = "anton.bjorklund@helsinki.fi" }]
 description = "The SLISE algorithm for robust regression and explanations of black box models"
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = [
     "Robust regression",
     "Sparse Linear Regression",
@@ -24,15 +24,15 @@
     "scipy >= 1.6",
     "numba >= 0.53",
     "matplotlib >= 3.3",
     "PyLBFGS >= 0.2",
 ]
 
 [project.optional-dependencies]
-dev = ["pytest", "black[jupyter]", "pylint", "IPython"]
+dev = ["pytest", "pytest-cov", "black[jupyter]", "pylint", "IPython", "ruff"]
 tbb = ["tbb"]
 
 [project.urls]
 homepage = "https://edahelsinki.fi/pyslise"
 documentation = "https://edahelsinki.fi/pyslise/docs/slise/"
 repository = "https://github.com/edahelsinki/pyslise.git"
```

### Comparing `slise-2.2.3/slise/__init__.py` & `slise-2.2.4/slise/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 """
-    SLISE - Sparse Linear Subset Explanations
-    -----------------------------------------
+SLISE - Sparse Linear Subset Explanations
+-----------------------------------------
 
-    The SLISE algorithm can be used for both robust regression and to explain outcomes from black box models.
-    See [slise.slise.regression][] and [slise.slise.explain][] for referense.
+The SLISE algorithm can be used for both robust regression and to explain outcomes from black box models.
+See [slise.slise.regression][] and [slise.slise.explain][] for referense.
 
 
-    In robust regression we fit regression models that can handle data that
-    contains outliers. SLISE accomplishes this by fitting a model such that
-    the largest possible subset of the data items have an error less than a
-    given value. All items with an error larger than that are considered
-    potential outliers and do not affect the resulting model.
-
-    SLISE can also be used to provide local model-agnostic explanations for
-    outcomes from black box models. To do this we replace the ground truth
-    response vector with the predictions from the complex model. Furthermore, we
-    force the model to fit a selected item (making the explanation local). This
-    gives us a local approximation of the complex model with a simpler linear
-    model. In contrast to other methods SLISE creates explanations using real
-    data (not some discretised and randomly sampled data) so we can be sure that
-    all inputs are valid (i.e. in the correct data manifold, and follows the
-    constraints used to generate the data, e.g., the laws of physics).
-
-
-    More in-depth details about the algorithm can be found in the papers:
-
-    Björklund A., Henelius A., Oikarinen E., Kallonen K., Puolamäki K.
-    Sparse Robust Regression for Explaining Classifiers.
-    Discovery Science (DS 2019).
-    Lecture Notes in Computer Science, vol 11828, Springer.
-    https://doi.org/10.1007/978-3-030-33778-0_27
-
-    Björklund A., Henelius A., Oikarinen E., Kallonen K., Puolamäki K.
-    Robust regression via error tolerance.
-    Data Mining and Knowledge Discovery (2022).
-    https://doi.org/10.1007/s10618-022-00819-2
-
+In robust regression we fit regression models that can handle data that
+contains outliers. SLISE accomplishes this by fitting a model such that
+the largest possible subset of the data items have an error less than a
+given value. All items with an error larger than that are considered
+potential outliers and do not affect the resulting model.
+
+SLISE can also be used to provide local model-agnostic explanations for
+outcomes from black box models. To do this we replace the ground truth
+response vector with the predictions from the complex model. Furthermore, we
+force the model to fit a selected item (making the explanation local). This
+gives us a local approximation of the complex model with a simpler linear
+model. In contrast to other methods SLISE creates explanations using real
+data (not some discretised and randomly sampled data) so we can be sure that
+all inputs are valid (i.e. in the correct data manifold, and follows the
+constraints used to generate the data, e.g., the laws of physics).
+
+
+More in-depth details about the algorithm can be found in the papers:
+
+Björklund A., Henelius A., Oikarinen E., Kallonen K., Puolamäki K.
+Sparse Robust Regression for Explaining Classifiers.
+Discovery Science (DS 2019).
+Lecture Notes in Computer Science, vol 11828, Springer.
+https://doi.org/10.1007/978-3-030-33778-0_27
+
+Björklund A., Henelius A., Oikarinen E., Kallonen K., Puolamäki K.
+Robust regression via error tolerance.
+Data Mining and Knowledge Discovery (2022).
+https://doi.org/10.1007/s10618-022-00819-2
+
+Björklund A., Henelius A., Oikarinen E., Kallonen K., Puolamäki K.
+Explaining any black box model using real data.
+Frontiers in Computer Science 5:1143904 (2023).
+https://doi.org/10.3389/fcomp.2023.1143904
 """
 
-from slise.slise import (
+from slise.slise import (  # noqa: F401
     SliseRegression,
     regression,
     SliseExplainer,
     explain,
     SliseWarning,
 )
-from slise.utils import limited_logit as logit
-from slise.data import normalise_robust
+from slise.utils import limited_logit as logit  # noqa: F401
+from slise.data import normalise_robust  # noqa: F401
```

### Comparing `slise-2.2.3/slise/data.py` & `slise-2.2.4/slise/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-    This script contains functions for modifying data, mainly normalisation and PCA.
+This script contains functions for modifying data, mainly normalisation and PCA.
 """
 
 from typing import NamedTuple, Tuple, Union, Optional
 
 import numpy as np
```

### Comparing `slise-2.2.3/slise/initialisation.py` & `slise-2.2.4/slise/initialisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-    This script contains functions for initialising alpha and beta in SLISE.
+This script contains functions for initialising alpha and beta in SLISE.
 """
 
 from math import log
 from typing import Optional, Tuple, Union
 from warnings import catch_warnings
 
 import numpy as np
@@ -118,17 +118,15 @@
         min_beta_step (float, optional): Minimum beta. Defaults to 1e-8.
 
     Returns:
         Tuple[np.ndarray, float]: `(alpha, beta)`.
     """
     epsilon = epsilon**2
     beta_max = min(beta_max, beta_max_init) / epsilon
-    beta = next_beta(
-        Y**2, epsilon, 0, weight, beta_max, log(max_approx), min_beta_step
-    )
+    beta = next_beta(Y**2, epsilon, 0, weight, beta_max, log(max_approx), min_beta_step)
     return np.zeros(X.shape[1]), beta
 
 
 def initialise_fixed(
     init: Union[np.ndarray, Tuple[np.ndarray, float]],
     X: np.ndarray,
     Y: np.ndarray,
```

### Comparing `slise-2.2.3/slise/optimisation.py` & `slise-2.2.4/slise/optimisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-    This script contains the loss functions and optimisation functions for SLISE.
+This script contains the loss functions and optimisation functions for SLISE.
 """
 
 from math import log
 from typing import Callable, Optional, Tuple
 from warnings import catch_warnings, warn
 
 import numpy as np
@@ -498,19 +498,19 @@
     """
     X = np.ascontiguousarray(X, dtype=np.float64)
     Y = np.ascontiguousarray(Y, dtype=np.float64)
     lambda1 = float(lambda1)
     lambda2 = float(lambda2)
     assert X.shape[0] == len(Y), f"Different lengths {X.shape[0]} != {len(Y)}"
     if weight is None:
-        lf = lambda alpha: _ridge_numba(alpha, X, Y, lambda2)
+        lf = lambda alpha: _ridge_numba(alpha, X, Y, lambda2)  # noqa: E731
     else:
         weight = np.ascontiguousarray(weight, dtype=np.float64)
         assert Y.shape == weight.shape, f"Different shapes {Y.shape} != {weight.shape}"
-        lf = lambda alpha: _ridge_numbaw(alpha, X, Y, lambda2, weight)
+        lf = lambda alpha: _ridge_numbaw(alpha, X, Y, lambda2, weight)  # noqa: E731
     return owlqn(lf, np.zeros(X.shape[1], dtype=np.float64), lambda1, max_iterations)
 
 
 def optimise_loss(
     alpha: np.ndarray,
     X: np.ndarray,
     Y: np.ndarray,
@@ -543,19 +543,19 @@
     assert X.shape[0] == len(Y), f"Different lengths {X.shape[0]} != {len(Y)}"
     assert X.shape[1] == len(alpha), f"Different lengths {X.shape[0]} != {len(alpha)}"
     lambda1 = float(lambda1)
     lambda2 = float(lambda2)
     epsilon = float(epsilon)
     beta = float(beta)
     if weight is None:
-        lf = lambda alpha: _loss_grad(alpha, X, Y, epsilon, beta, lambda2)
+        lf = lambda alpha: _loss_grad(alpha, X, Y, epsilon, beta, lambda2)  # noqa: E731
     else:
         weight = np.ascontiguousarray(weight, dtype=np.float64)
         assert Y.shape == weight.shape, f"Different shapes {Y.shape} != {weight.shape}"
-        lf = lambda alpha: _loss_gradw(alpha, X, Y, epsilon, beta, lambda2, weight)
+        lf = lambda alpha: _loss_gradw(alpha, X, Y, epsilon, beta, lambda2, weight)  # noqa: E731
     return owlqn(lf, alpha, lambda1, max_iterations)
 
 
 def log_approximation_ratio(
     residuals2: np.ndarray,
     epsilon2: float,
     beta1: float,
@@ -572,16 +572,16 @@
         weight (Optional[np.ndarray], optional): Weight vector. Defaults to None.
 
     Returns:
         float: log of the approximation ratio between `beta1` and `beta2` for the current solution.
     """
     if beta1 >= beta2:
         return 0
-    log_f = lambda r, beta: log_sigmoid(beta * (epsilon2 - r))
-    dlog_g = lambda r: -beta1 * dlog_sigmoid(
+    log_f = lambda r, beta: log_sigmoid(beta * (epsilon2 - r))  # noqa: E731
+    dlog_g = lambda r: -beta1 * dlog_sigmoid(  # noqa: E731
         beta1 * (epsilon2 - r)
     ) + beta2 * dlog_sigmoid(beta2 * (epsilon2 - r))
     if dlog_g(0) < 0:
         a = brentq(dlog_g, 0, epsilon2)
         log_k = min(
             log_f(0, beta1) - log_f(0, beta2), log_f(a, beta1) - log_f(a, beta2)
         )
@@ -624,15 +624,15 @@
     """
     if beta >= beta_max:
         return beta
     log_approx = log_approximation_ratio(residuals2, epsilon2, beta, beta_max, weight)
     if log_approx <= log_max_approx:
         return beta_max
     else:
-        f = (
+        f = (  # noqa: E731
             lambda b: log_approximation_ratio(residuals2, epsilon2, beta, b, weight)
             - log_max_approx
         )
         beta_min = beta + min_beta_step * (beta_max + beta)
         return max(brentq(f, beta, beta_max), beta_min)
 
 
@@ -677,17 +677,15 @@
     weight: Optional[np.ndarray] = None,
 ):
     """
     Print the log statement for a graduated optimisation step.
     """
     residuals = (X @ alpha - Y) ** 2
     loss = loss_sharp(alpha, X, Y, epsilon, lambda1, lambda2, weight)
-    bloss = loss_residuals(
-        alpha, residuals, epsilon**2, beta, lambda1, lambda2, weight
-    )
+    bloss = loss_residuals(alpha, residuals, epsilon**2, beta, lambda1, lambda2, weight)
     epss = matching_epsilon(residuals, epsilon**2, beta, weight)
     beta = beta * epsilon**2
     print(
         f"beta: {beta:5.3f}    epsilon*: {epss:.3f}    Loss: {loss:6.2f}    B-Loss: {bloss:6.2f}"
     )
```

### Comparing `slise-2.2.3/slise/plot.py` & `slise-2.2.4/slise/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
-    This script contains functions for plotting SLISE solutions.
+This script contains functions for plotting SLISE solutions.
 """
 
 from collections import OrderedDict
-from typing import List, Tuple, Union, Optional
+from typing import List, Sequence, Tuple, Union, Optional
 from warnings import warn
 
 import numpy as np
 from matplotlib import pyplot as plt
 from matplotlib.colors import LinearSegmentedColormap, Normalize
 from matplotlib.patches import Patch
 from matplotlib.pyplot import Figure
@@ -117,40 +117,45 @@
     if steps <= 2:
         return np.array([min - diff * extension, max + diff * extension])
     else:
         return np.linspace(min - diff * extension, max + diff * extension, steps)
 
 
 def get_explanation_order(
-    alpha: np.ndarray, intercept: bool = True, min: int = 5, th=1e-6
+    alpha: np.ndarray,
+    intercept: bool = True,
+    min: int = 5,
+    max: int = -1,
+    th: float = 1e-6,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Get the order in which to show the variables in the plots.
 
     Args:
         alpha (np.ndarray): Linear model.
         intercept (bool, optional): Does the model include an intercept. Defaults to True.
         min (int, optional): If the number of variables is larger than this, hide the zeroes. Defaults to 5.
+        max (int, optional): If `max > 0`, select the top variables. Defaults to -1.
         th ([type], optional): Threshold for zero. Defaults to 1e-6.
 
     Returns:
         Tuple[np.ndarray, np.ndarray]: The order of the variables in the explanation
     """
     if intercept:
         order = np.argsort(alpha[1:]) + 1
-        if len(order) > min:
-            order = order[np.nonzero(alpha[order])]
-            if len(order) > min:
-                order = order[np.abs(alpha[order]) > np.max(np.abs(alpha)) * th]
-        order = np.concatenate((order, np.zeros(1, order.dtype)))
     else:
         order = np.argsort(alpha)
+    if len(order) > min:
+        order = order[np.nonzero(alpha[order])]
         if len(order) > min:
-            order = order[np.nonzero(alpha[order])]
-            if len(order) > min:
-                order = order[np.abs(alpha[order]) > np.max(np.abs(alpha)) * th]
+            order = order[np.abs(alpha[order]) > np.max(np.abs(alpha)) * th]
+    if max > 0 and len(order) > max:
+        nth = -np.partition(-np.abs(alpha), max - 1)[max - 1]
+        order = order[np.abs(alpha[order]) >= nth]
+    if intercept:
+        order = np.concatenate((order, np.zeros(1, order.dtype)))
     return np.flip(order)
 
 
 def print_slise(
     coefficients: np.ndarray,
     intercept: bool,
     subset: np.ndarray,
@@ -210,16 +215,16 @@
     if scaled_terms is not None:
         rows["Normalised Term:"] = ["%%.%df" % decimals % a for a in scaled_terms]
     col_len = [
         max(8, *vs) + 1
         for vs in zip(*(tuple(len(v) for v in vs) for vs in rows.values()))
     ]
     if len(coefficients) > num_var:
-        col_len = [l if c != 0 else 0 for l, c in zip(col_len, coefficients)]
-    lab_len = max(len(l) for l in rows)
+        col_len = [cl if c != 0 else 0 for cl, c in zip(col_len, coefficients)]
+    lab_len = max(len(r) for r in rows)
     if title:
         print(title)
     if unscaled_y is not None:
         print(fill_prediction_str(unscaled_y, unscaled_preds, classes, decimals))
     for k in rows:
         print(
             f"{k:<{lab_len}}",
@@ -338,14 +343,15 @@
     alpha: Optional[np.ndarray] = None,
     x: Optional[np.ndarray] = None,
     y: Optional[float] = None,
     terms: Optional[np.ndarray] = None,
     norm_terms: Optional[np.ndarray] = None,
     title: str = "SLISE Explanation",
     variables: Optional[List[str]] = None,
+    order: Union[None, int, Sequence[int]] = None,
     decimals: int = 3,
     fig: Optional[Figure] = None,
 ):
     """Plot the SLISE result with density distributions for the dataset and barplot for the model.
 
     Args:
         X (np.ndarray): Data matrix.
@@ -354,30 +360,38 @@
         subset (np.ndarray): Selected subset.
         alpha (Optional[np.ndarray]): Scaled model. Defaults to None.
         x (Optional[np.ndarray], optional): The explained item (if it is an explanation). Defaults to None.
         y (Optional[float], optional): The explained outcome (if it is an explanation). Defaults to None.
         terms (Optional[np.ndarray], optional): Term vector (unscaled x*alpha), if available. Defaults to None.
         norm_terms (Optional[np.ndarray], optional): Term vector (scaled x*alpha), if available. Defaults to None.
         title (str, optional): Title of the plot. Defaults to "SLISE Explanation".
+        order (Union[None, int, Sequence[int]], optional): Select variables (None: all, int: largest, selected). Defaults to all.
         variables (Optional[List[str]], optional): Names for the (columns/) variables. Defaults to None.
         decimals (int, optional): Number of decimals when writing numbers. Defaults to 3.
         fig (Optional[Figure], optional): Pyplot figure to plot on, if None then a new plot is created and shown. Defaults to None.
     """
     # Values and order
     variables = fill_column_names(variables, X.shape[1], True)
     if alpha is None:
         noalpha = True
         alpha = model
     else:
         noalpha = False
+    order_offset = 0
     if len(model) == X.shape[1]:
         model = np.concatenate((np.zeros(1, model.dtype), model))
         alpha = np.concatenate((np.zeros(1, model.dtype), alpha))
+        order_offset = 1
         variables[0] = ""
-    order = get_explanation_order(np.abs(alpha), True)
+    if order is None:
+        order = get_explanation_order(np.abs(alpha), True)
+    elif isinstance(order, int):
+        order = get_explanation_order(np.abs(alpha), True, max=order)
+    else:
+        order = [0] + [i + order_offset for i in order if i + order_offset != 0]
     model = model[order]
     alpha = alpha[order]
     if terms is not None:
         terms = terms[order]
     if norm_terms is not None:
         norm_terms = norm_terms[order]
     variables = [variables[i] for i in order]
@@ -397,15 +411,15 @@
     def fill_density(ax, X, x, n):
         if np.var(X) == 0:
             X = np.random.normal(X[0], 1e-8, len(X))
         kde1 = gaussian_kde(X, 0.2)
         if np.sum(subset) > 1:
             kde2 = gaussian_kde(X[subset], 0.2)
         else:
-            kde2 = lambda x: x * 0
+            kde2 = lambda x: x * 0  # noqa: E731
         lim = extended_limits(X, 0.1, 100)
         ax.plot(lim, kde1(lim), color="black", label="Dataset")
         ax.plot(
             lim,
             kde2(lim) * subsize,
             color=SLISE_PURPLE,
             label=f"Subset: {subsize * 100:.0f}%",
@@ -420,16 +434,16 @@
 
     if x is None and y is None:
         fill_density(axs[0, 0], Y, y, "Response")
     else:
         fill_density(axs[0, 0], Y, y, "Prediction")
     axs[0, 0].legend()
     axs[0, 0].set_title("Dataset Distribution")
-    for i, k, n in zip(range(1, len(order)), order[1:] - 1, variables[1:]):
-        fill_density(axs[i, 0], X[:, k], x[k] if x is not None else None, n)
+    for i, k, n in zip(range(1, len(order)), order[1:], variables[1:]):
+        fill_density(axs[i, 0], X[:, k - 1], x[k - 1] if x is not None else None, n)
 
     # Bar plots
     def text(x, y, v):
         if v != 0:
             axbig.text(
                 x,
                 y,
```

### Comparing `slise-2.2.3/slise/slise.py` & `slise-2.2.4/slise/slise.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
-    This script contains the main SLISE functions, and classes.
+This script contains the main SLISE functions, and classes.
 
-    The library can both be used "sk-learn" style with `SliseRegression(...).fit(X, y)`
-    and `SliseExplanation(...).explain(index)`, or in a more functional style with
-    `regression(...)` and `explain(...)`.
+The library can both be used "sk-learn" style with `SliseRegression(...).fit(X, y)`
+and `SliseExplanation(...).explain(index)`, or in a more functional style with
+`regression(...)` and `explain(...)`.
 """
 
 from __future__ import annotations
 
-from typing import Callable, List, Optional, Tuple, Union
+from typing import Callable, List, Optional, Sequence, Tuple, Union
 from warnings import warn
 
 import numpy as np
 from matplotlib.pyplot import Figure
 from scipy.special import expit as sigmoid
 
 from slise.data import (
@@ -507,39 +507,42 @@
             fig,
         )
 
     def plot_dist(
         self,
         title: str = "SLISE Regression",
         variables: list = None,
+        order: Union[None, int, Sequence[int]] = None,
         decimals: int = 3,
         fig: Union[Figure, None] = None,
     ) -> SliseExplainer:
         """Plot the regression with density distributions for the dataset and a barplot for the model.
 
         Args:
             title (str, optional): Title of the plot. Defaults to "SLISE Explanation".
             variables (list, optional): Names for the variables. Defaults to None.
+            order (Union[None, int, Sequence[int]], optional): Select variables (None: all, int: largest, selected). Defaults to all.
             decimals (int, optional): Number of decimals to write. Defaults to 3.
             fig (Union[Figure, None], optional): Pyplot figure to plot on, if None then a new plot is created and shown. Defaults to None.
         """
         plot_dist(
-            self._X,
-            self._Y,
-            self.coefficients,
-            self.subset(),
-            self.normalised(),
-            None,
-            None,
-            None,
-            None,
-            title,
-            variables,
-            decimals,
-            fig,
+            X=self._X,
+            Y=self._Y,
+            model=self.coefficients,
+            subset=self.subset(),
+            alpha=self.normalised(),
+            x=None,
+            y=None,
+            terms=None,
+            norm_terms=None,
+            title=title,
+            variables=variables,
+            order=order,
+            decimals=decimals,
+            fig=fig,
         )
 
     def plot_subset(
         self,
         title: str = "Response Distribution",
         decimals: int = 0,
         fig: Union[Figure, None] = None,
@@ -1008,42 +1011,45 @@
             fig,
         )
 
     def plot_dist(
         self,
         title: str = "SLISE Explanation",
         variables: list = None,
+        order: Union[None, int, Sequence[int]] = None,
         decimals: int = 3,
         fig: Union[Figure, None] = None,
     ) -> SliseExplainer:
         """Plot the current explanation with density distributions for the dataset and a barplot for the model.
 
         The barplot contains both the approximating linear model (where the weights can be loosely interpreted as the importance of the different variables and their sign) and the "terms", which is the (scaled) model time the (scaled) item values.
         The terms demonstrates how the explained item interacts with the approximating linear model, since a negative weight times a negative value actually supports a positive prediction.
 
         Args:
             title (str, optional): Title of the plot. Defaults to "SLISE Explanation".
             variables (list, optional): Names for the variables. Defaults to None.
+            order (Union[None, int, Sequence[int]], optional): Select variables (None: all, int: largest, selected). Defaults to all.
             decimals (int, optional): Number of decimals to write. Defaults to 3.
             fig (Union[Figure, None], optional): Pyplot figure to plot on, if None then a new plot is created and shown. Defaults to None.
         """
         plot_dist(
-            self._X,
-            self._Y,
-            self.coefficients,
-            self.subset(),
-            self.normalised(),
-            self._x,
-            self._y,
-            self.get_terms(False),
-            self.get_terms(True) if self._normalise else None,
-            title,
-            variables,
-            decimals,
-            fig,
+            X=self._X,
+            Y=self._Y,
+            model=self.coefficients,
+            subset=self.subset(),
+            alpha=self.normalised(),
+            x=self._x,
+            y=self._y,
+            terms=self.get_terms(False),
+            norm_terms=self.get_terms(True) if self._normalise else None,
+            title=title,
+            variables=variables,
+            order=order,
+            decimals=decimals,
+            fig=fig,
         )
 
     def plot_subset(
         self,
         title: str = "Prediction Distribution",
         decimals: int = 0,
         fig: Union[Figure, None] = None,
```

### Comparing `slise-2.2.3/slise/utils.py` & `slise-2.2.4/slise/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-    This script contains some utility functions.
+This script contains some utility functions.
 """
 
 from typing import Union
 
 import numpy as np
 from scipy.special import expit as sigmoid
```

### Comparing `slise-2.2.3/slise.egg-info/PKG-INFO` & `slise-2.2.4/slise.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slise
-Version: 2.2.3
+Version: 2.2.4
 Summary: The SLISE algorithm for robust regression and explanations of black box models
 Author-email: Anton Björklund <anton.bjorklund@helsinki.fi>
 License: MIT License
         
         Copyright (c) 2022 Anton Björklund
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,17 +40,19 @@
 Requires-Dist: numpy>=1.20
 Requires-Dist: scipy>=1.6
 Requires-Dist: numba>=0.53
 Requires-Dist: matplotlib>=3.3
 Requires-Dist: PyLBFGS>=0.2
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: IPython; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
 Provides-Extra: tbb
 Requires-Dist: tbb; extra == "tbb"
 
 ![PySLISE Banner Image](docs/pyslise_banner.webp)  
 [![PyPI](https://img.shields.io/pypi/v/slise)](https://pypi.org/project/slise/)
 [![Documentation](https://github.com/edahelsinki/pyslise/actions/workflows/python-docs.yml/badge.svg)](https://edahelsinki.github.io/pyslise/docs/slise/)
 [![Tests](https://github.com/edahelsinki/pyslise/actions/workflows/python-pytest.yml/badge.svg)](https://github.com/edahelsinki/pyslise/actions/workflows/python-pytest.yml)
```

### Comparing `slise-2.2.3/tests/test_data.py` & `slise-2.2.4/tests/test_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     add_constant_columns,
     normalise_robust,
     scale_same,
     unscale_model,
 )
 from slise.utils import mat_mul_inter
 
-from .utils import *
+from .utils import data_create2, data_create
 
 
 def test_scaling():
     print("Testing scaling")
     for i in (4, 6, 8):
         X, Y = data_create(i * 30, i, 100000)
         X2, center, scale = normalise_robust(X)
@@ -64,8 +64,7 @@
     X3 = np.concatenate((X * 2, X), 1)
     assert pca_simple(X3, 10)[1].shape == (5, 10)
     assert np.allclose(X[0, :], pca_invert(pca_rotate(X[0, :], v), v))
     mod = np.random.normal(size=5)
     assert np.allclose(X @ mod, X2 @ pca_rotate_model(mod, v))
     assert np.allclose(X @ pca_invert_model(mod, v), X2 @ mod)
     X4, v = pca_simple(X.T, 4)
-
```

### Comparing `slise-2.2.3/tests/test_optim.py` & `slise-2.2.4/tests/test_optim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import pytest
 from pytest import approx
 from slise.optimisation import (
     check_threading_layer,
     graduated_optimisation,
     log_approximation_ratio,
     loss_grad,
     loss_sharp,
@@ -11,15 +10,15 @@
     matching_epsilon,
     next_beta,
     optimise_loss,
     regularised_regression,
 )
 from slise.utils import log_sigmoid, log_sum_exp, log_sum_special, sigmoid, sparsity
 
-from .utils import *
+from .utils import data_create, data_create2, numeric_grad
 
 
 def test_utils():
     print("Testing util functions")
     x = np.arange(-6, 6)
     assert np.allclose(np.log(sigmoid(x)), log_sigmoid(x))
     assert sparsity(x) == len(x) - 1
@@ -135,15 +134,15 @@
     ) >= loss_smooth(alpha2, X, Y, 0.1, beta=100, lambda2=0.5, weight=w)
 
 
 def test_gradopt():
     print("Testing graduated optimisation")
     X, Y = data_create(20, 5)
     alpha = np.random.normal(size=5)
-    alpha2 = graduated_optimisation(alpha, X, Y, 0.1, beta=100)
+    alpha2 = graduated_optimisation(alpha, X, Y, 0.1, beta=100, debug=True)
     assert loss_smooth(alpha, X, Y, 0.1, beta=100) >= loss_smooth(
         alpha2, X, Y, 0.1, beta=100
     )
     alpha2 = graduated_optimisation(alpha, X, Y, 0.1, beta=100, lambda1=0.5)
     assert loss_smooth(alpha, X, Y, 0.1, beta=100, lambda1=0.5) >= loss_smooth(
         alpha2, X, Y, 0.1, beta=100, lambda1=0.5
     )
@@ -248,13 +247,13 @@
     assert np.allclose(
         regularised_regression(X, Y, 1e-4, 1e-4, weight=w1),
         regularised_regression(X, Y, 1e-4, 1e-4, weight=w2),
     )
     assert np.allclose(
         regularised_regression(X2, Y2, 1e-4, 1e-4, weight=w1),
         regularised_regression(X, Y, 1e-4, 1e-4, weight=w3),
-        atol=1e-5
+        atol=1e-5,
     )
 
 
 def test_check_threading_layer():
     check_threading_layer()
```

### Comparing `slise-2.2.3/tests/test_slise.py` & `slise-2.2.4/tests/test_slise.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     initialise_lasso,
     initialise_ols,
     initialise_zeros,
 )
 from slise.optimisation import loss_smooth
 from slise.utils import mat_mul_inter
 
-from .utils import *
+from .utils import data_create, data_create2
 
 
 def test_initialise_simple():
     print("Testing old initialisations")
     X, Y = data_create(20, 5)
     w = np.random.uniform(size=20)
     alpha, beta = initialise_lasso(X, Y, 0.1, w)
@@ -119,17 +119,16 @@
 def test_slise_reg():
     print("Testing slise regression")
     X, Y, mod = data_create2(40, 5)
     w = np.random.uniform(size=40) + 0.5
     reg1 = regression(
         X, Y, epsilon=0.1, lambda1=1e-4, lambda2=1e-4, intercept=True, normalise=True
     )
-    reg1.print()
     Yp = mat_mul_inter(X, reg1.coefficients)
-    Yn = reg1._scale.scale_y(Y)
+    # Yn = reg1._scale.scale_y(Y)
     Ynp = mat_mul_inter(reg1._scale.scale_x(X), reg1._alpha)
     Ypn = reg1._scale.scale_y(Yp)
     # S = (Y - Yp) ** 2 < reg1.epsilon ** 2
     # Sn = (Yn - Ynp) ** 2 < reg1.epsilon_orig ** 2
     assert np.allclose(
         Ypn, Ynp
     ), f"The predicted Y's are not the same {np.max(np.abs(Ynp - Ypn))}"
@@ -140,88 +139,78 @@
         Y,
         epsilon=0.1,
         lambda1=1e-4,
         lambda2=1e-4,
         intercept=True,
         normalise=False,
     )
-    reg2.print()
     assert reg2.score() <= 0, f"SLISE loss should be negative ({reg2.score()})"
     assert 1.0 >= reg2.subset().mean() > 0.5
     reg3 = regression(
         X,
         Y,
         epsilon=0.1,
         lambda1=0,
         lambda2=0,
         intercept=True,
         normalise=False,
     )
-    reg3.print()
     assert reg3.score() <= 0, f"SLISE loss should be negative ({reg3.score()})"
     assert 1.0 >= reg3.subset().mean() > 0.5
     reg4 = regression(
         X,
         Y,
         epsilon=0.1,
         lambda1=1e-4,
         lambda2=1e-4,
         intercept=True,
         normalise=False,
         weight=w,
     )
-    reg4.print()
     assert reg4.score() <= 0, f"SLISE loss should be negative ({reg4.score()})"
     assert 1.0 >= reg4.subset().mean() > 0.4
 
 
 def test_slise_exp():
     print("Testing slise explanation")
     np.random.seed(49)
     X, Y, mod = data_create2(100, 5)
     Y2 = sigmoid(Y)
     w = np.random.uniform(size=100) + 0.5
     x = np.random.normal(size=5)
     y = np.random.normal()
     reg = explain(X, Y, 0.1, x, y, lambda1=1e-4, lambda2=1e-4, normalise=True)
-    reg.print()
     assert reg.score() <= 0, f"Slise loss should usually be <=0 ({reg.score():.2f})"
     assert y == approx(reg.predict(x))
     assert 1.0 >= reg.subset().mean() > 0.0
     reg = explain(X, Y, 0.1, 17, lambda1=0.01, lambda2=0.01, normalise=True)
-    reg.print()
     assert reg.score() <= 0, f"Slise loss should usually be <=0 ({reg.score():.2f})"
     assert Y[17] == approx(reg.predict(X[17]))
     assert 1.0 >= reg.subset().mean() > 0.0
     reg = explain(X, Y, 0.1, x, y, lambda1=0.01, lambda2=0.01, normalise=False)
     assert reg.score() <= 0, f"Slise loss should usually be <=0 ({reg.score():.2f})"
     assert y == approx(reg.predict(x))
     assert 1.0 >= reg.subset().mean() > 0.0
     reg = explain(X, Y, 0.1, x, y, lambda1=0, lambda2=0, normalise=False)
-    reg.print()
     assert reg.score() <= 0, f"Slise loss should usually be <=0 ({reg.score():.2f})"
     assert y == approx(reg.predict(x))
     assert 1.0 >= reg.subset().mean() > 0.0
     reg = explain(X, Y, 0.1, 18, lambda1=0.01, lambda2=0.01, normalise=False)
-    reg.print()
     assert reg.score() <= 0, f"Slise loss should usually be <=0 ({reg.score():.2f})"
     assert Y[18] == approx(reg.predict(X[18]))
     assert 1.0 >= reg.subset().mean() > 0.0
     reg = explain(X, Y, 0.1, 19, lambda1=0, lambda2=0, normalise=False)
-    reg.print()
     assert reg.score() <= 0, f"Slise loss should usually be <=0 ({reg.score():.2f})"
     assert Y[19] == approx(reg.predict(X[19]))
     assert 1.0 >= reg.subset().mean() > 0.0
     reg = explain(X, Y, 0.1, 19, lambda1=0.01, lambda2=0.01, weight=w, normalise=False)
-    reg.print()
     assert reg.score() <= 0, f"Slise loss should usually be <=0 ({reg.score():.2f})"
     assert Y[19] == approx(reg.predict(X[19]))
     assert 1.0 >= reg.subset().mean() > 0.0
     reg = explain(X, Y2, 0.5, 20, weight=w, normalise=True, logit=True)
-    reg.print()
     assert reg.score() <= 0, f"Slise loss should usually be <=0 ({reg.score():.2f})"
     assert Y2[20] == approx(reg.predict(X[20]))
     assert 1.0 >= reg.subset().mean() > 0.0
 
 
 def test_normalised():
     np.random.seed(49)
@@ -231,15 +220,15 @@
     reg = explain(X, Y, 0.1, x, y, lambda1=1e-4, lambda2=1e-4, normalise=True)
     assert reg.coefficients.shape == reg.normalised(True).shape
     assert reg.coefficients.shape[0] > reg.normalised(False).shape[0]
     assert np.allclose(
         reg.coefficients, reg._scale.unscale_model(reg.normalised(False))
     )
     threads = numba.get_num_threads()
-    reg1 = regression(
+    regression(
         X,
         Y,
         epsilon=0.1,
         lambda1=1e-4,
         lambda2=1e-4,
         intercept=True,
         normalise=True,
```

