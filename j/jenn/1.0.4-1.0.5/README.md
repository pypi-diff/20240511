# Comparing `tmp/jenn-1.0.4.tar.gz` & `tmp/jenn-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenn-1.0.4.tar", last modified: Wed May  8 18:55:46 2024, max compression
+gzip compressed data, was "jenn-1.0.5.tar", last modified: Sat May 11 13:57:03 2024, max compression
```

## Comparing `jenn-1.0.4.tar` & `jenn-1.0.5.tar`

### file list

```diff
@@ -1,39 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.409620 jenn-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-08 18:53:37.000000 jenn-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-08 18:55:46.409620 jenn-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-05-08 18:53:37.000000 jenn-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-08 18:53:37.000000 jenn-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:55:46.409620 jenn-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.401620 jenn-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.405620 jenn-1.0.4/src/jenn/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.405620 jenn-1.0.4/src/jenn/core/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13672 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/core/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.409620 jenn-1.0.4/src/jenn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    18429 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-08 18:53:37.000000 jenn-1.0.4/src/jenn/utils/rbf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.409620 jenn-1.0.4/src/jenn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-08 18:55:46.000000 jenn-1.0.4/src/jenn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-08 18:55:46.000000 jenn-1.0.4/src/jenn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:55:46.000000 jenn-1.0.4/src/jenn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 18:55:46.000000 jenn-1.0.4/src/jenn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 18:55:46.000000 jenn-1.0.4/src/jenn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:55:46.409620 jenn-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-08 18:53:37.000000 jenn-1.0.4/tests/test_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-08 18:53:37.000000 jenn-1.0.4/tests/test_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-08 18:53:37.000000 jenn-1.0.4/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-08 18:53:37.000000 jenn-1.0.4/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-08 18:53:37.000000 jenn-1.0.4/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-08 18:53:37.000000 jenn-1.0.4/tests/test_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:57:03.909181 jenn-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-11 13:55:13.000000 jenn-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-11 13:55:13.000000 jenn-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-11 13:57:03.909181 jenn-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-05-11 13:55:13.000000 jenn-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-11 13:55:14.000000 jenn-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 13:57:03.909181 jenn-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:57:03.901181 jenn-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:57:03.905181 jenn-1.0.5/src/jenn/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:57:03.905181 jenn-1.0.5/src/jenn/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/core/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/core/cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/core/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13672 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/core/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/core/propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/core/schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/core/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8946 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:57:03.905181 jenn-1.0.5/src/jenn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18429 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-11 13:55:14.000000 jenn-1.0.5/src/jenn/utils/rbf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:57:03.909181 jenn-1.0.5/src/jenn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-05-11 13:57:03.000000 jenn-1.0.5/src/jenn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-11 13:57:03.000000 jenn-1.0.5/src/jenn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 13:57:03.000000 jenn-1.0.5/src/jenn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-11 13:57:03.000000 jenn-1.0.5/src/jenn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-11 13:57:03.000000 jenn-1.0.5/src/jenn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:57:03.909181 jenn-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-11 13:55:14.000000 jenn-1.0.5/tests/test_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-11 13:55:14.000000 jenn-1.0.5/tests/test_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-11 13:55:14.000000 jenn-1.0.5/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-11 13:55:14.000000 jenn-1.0.5/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-11 13:55:14.000000 jenn-1.0.5/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-11 13:55:14.000000 jenn-1.0.5/tests/test_propagation.py
```

### Comparing `jenn-1.0.4/LICENSE` & `jenn-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/PKG-INFO` & `jenn-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: jenn
-Version: 1.0.4
+Version: 1.0.5
 Summary: Jacobian-Enhanced Neural Nets (JENN)
 Author-email: "Steven H. Berguin" <stevenberguin@gmail.com>
 Project-URL: Documentation, https://shb84.github.io/JENN/
 Project-URL: Homepage, https://github.com/shb84/JENN
 Project-URL: Issues, https://github.com/shb84/JENN/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: jsonpointer>=2.4
+Requires-Dist: jsonschema>=4.22
 Requires-Dist: orjson>=3.9
 Requires-Dist: numpy>=1.22
-Provides-Extra: viz
-Requires-Dist: matplotlib>=3.7; extra == "viz"
+Provides-Extra: plt
+Requires-Dist: matplotlib>=3.7; extra == "plt"
 
 # Jacobian-Enhanced Neural Network (JENN)
 
 Jacobian-Enhanced Neural Networks (JENN) are fully connected multi-layer
 perceptrons, whose training process is modified to predict partial 
 derivatives accurately. This is accomplished by minimizing a modified version 
 of the Least Squares Estimator (LSE) that accounts for Jacobian prediction error (see [theory](https://github.com/shb84/JENN/blob/master/docs/theory.pdf)).
```

### Comparing `jenn-1.0.4/README.md` & `jenn-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/pyproject.toml` & `jenn-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jenn"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Steven H. Berguin", email="stevenberguin@gmail.com" },
 ]
 description = "Jacobian-Enhanced Neural Nets (JENN)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+  "jsonpointer>=2.4",
+  "jsonschema>=4.22",
   "orjson>=3.9",
   "numpy>=1.22",
 ]
 
 [project.optional-dependencies]
-viz = ["matplotlib>=3.7"]
+plt = ["matplotlib>=3.7"]
 
 [tool.setuptools.package-data]
 jenn = ["*.json"]
 
 [project.urls]
 Documentation = "https://shb84.github.io/JENN/"
 Homepage = "https://github.com/shb84/JENN"
```

### Comparing `jenn-1.0.4/src/jenn/core/activation.py` & `jenn-1.0.5/src/jenn/core/activation.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/src/jenn/core/cache.py` & `jenn-1.0.5/src/jenn/core/cache.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/src/jenn/core/cost.py` & `jenn-1.0.5/src/jenn/core/cost.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 compute the neural net cost function used for training. 
 It is a modified version of the Least Squared Estimator (LSE), 
 augmented with a penalty function for regularization and another 
 term which accounts for Jacobian prediction error. See
 `paper`_ for details and notation. 
 """  # noqa W291
 
-from typing import Union
+from typing import List, Union
 
 import numpy as np
 
 from .data import Dataset
 from .parameters import Parameters
 
 
@@ -78,15 +78,15 @@
                 cost += np.squeeze(dot_product)
         return np.float64(cost)
 
 
 class Regularization:
     """Compute regularization penalty."""
 
-    def __init__(self, weights: list[np.ndarray], lambd: float = 0.0) -> None:
+    def __init__(self, weights: List[np.ndarray], lambd: float = 0.0) -> None:
         r"""Compute L2 norm penalty.
 
         :param weights: neural parameters :math:`W^{[l]} \in
         \mathbb{R}^{n^{[l]} \times n^{[l-1]}}` associated with each
         layer
         """
         self.weights = weights
```

### Comparing `jenn-1.0.4/src/jenn/core/data.py` & `jenn-1.0.5/src/jenn/core/data.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/src/jenn/core/optimization.py` & `jenn-1.0.5/src/jenn/core/optimization.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/src/jenn/core/parameters.py` & `jenn-1.0.5/src/jenn/core/parameters.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/src/jenn/core/propagation.py` & `jenn-1.0.5/src/jenn/core/propagation.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/src/jenn/core/training.py` & `jenn-1.0.5/src/jenn/core/training.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/src/jenn/model.py` & `jenn-1.0.5/src/jenn/model.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/src/jenn/synthetic.py` & `jenn-1.0.5/src/jenn/synthetic.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     @classmethod
     def sample(
         cls,
         m_lhs: int,
         m_levels: int,
         lb: Union[np.ndarray, float],
         ub: Union[np.ndarray, float],
-        dx: float | None = 1e-6,
+        dx: Union[float, None] = 1e-6,
         random_state: Union[int, None] = None,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """Generate synthetic data by sampling the test function.
 
         :param m_lhs: number of latin hypercube samples
         :param m_levels: number of levels per factor for full factorial
         :param lb: lower bound on the factors
@@ -174,15 +174,15 @@
     @classmethod
     def sample(
         cls,
         m_lhs: int = 100,
         m_levels: int = 0,
         lb: Union[np.ndarray, float] = -1.0,
         ub: Union[np.ndarray, float] = 1.0,
-        dx: float | None = 1e-6,
+        dx: Union[float, None] = 1e-6,
         random_state: Union[int, None] = None,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:  # noqa: D102
         return super().sample(m_lhs, m_levels, lb, ub, dx, random_state)
 
 
 class Parabola(TestFunction):
     r"""Parabolic function.
@@ -214,15 +214,15 @@
     @classmethod
     def sample(
         cls,
         m_lhs: int = 100,
         m_levels: int = 0,
         lb: Union[np.ndarray, float] = -1.0,
         ub: Union[np.ndarray, float] = 1.0,
-        dx: float | None = 1e-6,
+        dx: Union[float, None] = 1e-6,
         random_state: Union[int, None] = None,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:  # noqa: D102
         return super().sample(m_lhs, m_levels, lb, ub, dx, random_state)
 
 
 class Sinusoid(TestFunction):
     r"""Sinusoidal function.
@@ -250,15 +250,15 @@
     @classmethod
     def sample(
         cls,
         m_lhs: int = 100,
         m_levels: int = 0,
         lb: Union[np.ndarray, float] = -np.pi,
         ub: Union[np.ndarray, float] = np.pi,
-        dx: float | None = 1e-6,
+        dx: Union[float, None] = 1e-6,
         random_state: Union[int, None] = None,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:  # noqa: D102
         return super().sample(m_lhs, m_levels, lb, ub, dx, random_state)
 
 
 class Rastrigin(TestFunction):
     r"""Rastrigin function.
@@ -294,15 +294,15 @@
         * np.ones(
             2,
         ),
         ub: Union[np.ndarray, float] = 1.5
         * np.ones(
             2,
         ),
-        dx: float | None = 1e-6,
+        dx: Union[float, None] = 1e-6,
         random_state: Union[int, None] = None,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:  # noqa: D102
         return super().sample(m_lhs, m_levels, lb, ub, dx, random_state)
 
 
 class Rosenbrock(TestFunction):
     r"""Banana Rosenbrock function.
@@ -337,11 +337,11 @@
         * np.ones(
             2,
         ),
         ub: Union[np.ndarray, float] = 2.0
         * np.ones(
             2,
         ),
-        dx: float | None = 1e-6,
+        dx: Union[float, None] = 1e-6,
         random_state: Union[int, None] = None,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:  # noqa: D102
         return super().sample(m_lhs, m_levels, lb, ub, dx, random_state)
```

### Comparing `jenn-1.0.4/src/jenn/utils/metrics.py` & `jenn-1.0.5/src/jenn/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/src/jenn/utils/plot.py` & `jenn-1.0.5/src/jenn/utils/plot.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/src/jenn.egg-info/PKG-INFO` & `jenn-1.0.5/src/jenn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: jenn
-Version: 1.0.4
+Version: 1.0.5
 Summary: Jacobian-Enhanced Neural Nets (JENN)
 Author-email: "Steven H. Berguin" <stevenberguin@gmail.com>
 Project-URL: Documentation, https://shb84.github.io/JENN/
 Project-URL: Homepage, https://github.com/shb84/JENN
 Project-URL: Issues, https://github.com/shb84/JENN/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: jsonpointer>=2.4
+Requires-Dist: jsonschema>=4.22
 Requires-Dist: orjson>=3.9
 Requires-Dist: numpy>=1.22
-Provides-Extra: viz
-Requires-Dist: matplotlib>=3.7; extra == "viz"
+Provides-Extra: plt
+Requires-Dist: matplotlib>=3.7; extra == "plt"
 
 # Jacobian-Enhanced Neural Network (JENN)
 
 Jacobian-Enhanced Neural Networks (JENN) are fully connected multi-layer
 perceptrons, whose training process is modified to predict partial 
 derivatives accurately. This is accomplished by minimizing a modified version 
 of the Least Squares Estimator (LSE) that accounts for Jacobian prediction error (see [theory](https://github.com/shb84/JENN/blob/master/docs/theory.pdf)).
```

### Comparing `jenn-1.0.4/src/jenn.egg-info/SOURCES.txt` & `jenn-1.0.5/src/jenn.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 src/jenn/__init__.py
 src/jenn/model.py
 src/jenn/synthetic.py
 src/jenn.egg-info/PKG-INFO
 src/jenn.egg-info/SOURCES.txt
@@ -13,14 +14,15 @@
 src/jenn/core/activation.py
 src/jenn/core/cache.py
 src/jenn/core/cost.py
 src/jenn/core/data.py
 src/jenn/core/optimization.py
 src/jenn/core/parameters.py
 src/jenn/core/propagation.py
+src/jenn/core/schema.json
 src/jenn/core/training.py
 src/jenn/utils/__init__.py
 src/jenn/utils/metrics.py
 src/jenn/utils/plot.py
 src/jenn/utils/rbf.py
 tests/test_activation.py
 tests/test_cost.py
```

### Comparing `jenn-1.0.4/tests/test_activation.py` & `jenn-1.0.5/tests/test_activation.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/tests/test_cost.py` & `jenn-1.0.5/tests/test_cost.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/tests/test_model.py` & `jenn-1.0.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/tests/test_optimization.py` & `jenn-1.0.5/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/tests/test_parameters.py` & `jenn-1.0.5/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `jenn-1.0.4/tests/test_propagation.py` & `jenn-1.0.5/tests/test_propagation.py`

 * *Files identical despite different names*

