# Comparing `tmp/pysyncon-1.4.0.tar.gz` & `tmp/pysyncon-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysyncon-1.4.0.tar", last modified: Sat Mar 30 11:01:20 2024, max compression
+gzip compressed data, was "pysyncon-1.5.0.tar", last modified: Sat May 11 20:36:01 2024, max compression
```

## Comparing `pysyncon-1.4.0.tar` & `pysyncon-1.5.0.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 11:01:20.366130 pysyncon-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-30 11:01:14.000000 pysyncon-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-03-30 11:01:20.366130 pysyncon-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-30 11:01:14.000000 pysyncon-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-30 11:01:14.000000 pysyncon-1.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 11:01:20.362130 pysyncon-1.4.0/pysyncon/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-30 11:01:14.000000 pysyncon-1.4.0/pysyncon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-03-30 11:01:14.000000 pysyncon-1.4.0/pysyncon/augsynth.py
--rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-03-30 11:01:14.000000 pysyncon-1.4.0/pysyncon/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13377 2024-03-30 11:01:14.000000 pysyncon-1.4.0/pysyncon/dataprep.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-03-30 11:01:14.000000 pysyncon-1.4.0/pysyncon/penalized.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-03-30 11:01:14.000000 pysyncon-1.4.0/pysyncon/robust.py
--rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-03-30 11:01:14.000000 pysyncon-1.4.0/pysyncon/synth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12485 2024-03-30 11:01:14.000000 pysyncon-1.4.0/pysyncon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 11:01:20.366130 pysyncon-1.4.0/pysyncon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-03-30 11:01:20.000000 pysyncon-1.4.0/pysyncon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-30 11:01:20.000000 pysyncon-1.4.0/pysyncon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 11:01:20.000000 pysyncon-1.4.0/pysyncon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-30 11:01:20.000000 pysyncon-1.4.0/pysyncon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-30 11:01:20.000000 pysyncon-1.4.0/pysyncon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-30 11:01:20.366130 pysyncon-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 11:01:20.366130 pysyncon-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-03-30 11:01:14.000000 pysyncon-1.4.0/tests/test_augsynth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-03-30 11:01:14.000000 pysyncon-1.4.0/tests/test_augsynth_basque.py
--rw-r--r--   0 runner    (1001) docker     (127)    19419 2024-03-30 11:01:14.000000 pysyncon-1.4.0/tests/test_dataprep.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-03-30 11:01:14.000000 pysyncon-1.4.0/tests/test_penalized.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-03-30 11:01:14.000000 pysyncon-1.4.0/tests/test_penalized_basque.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-03-30 11:01:14.000000 pysyncon-1.4.0/tests/test_robust.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-03-30 11:01:14.000000 pysyncon-1.4.0/tests/test_robust_basque.py
--rw-r--r--   0 runner    (1001) docker     (127)    10291 2024-03-30 11:01:14.000000 pysyncon-1.4.0/tests/test_synth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-03-30 11:01:14.000000 pysyncon-1.4.0/tests/test_synth_basque.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-03-30 11:01:14.000000 pysyncon-1.4.0/tests/test_synth_germany.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-03-30 11:01:14.000000 pysyncon-1.4.0/tests/test_synth_texas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-03-30 11:01:14.000000 pysyncon-1.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:36:01.797161 pysyncon-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 20:35:51.000000 pysyncon-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-11 20:36:01.793161 pysyncon-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-11 20:35:51.000000 pysyncon-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:36:01.793161 pysyncon-1.5.0/pysyncon/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/augsynth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13423 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/dataprep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/penalized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/robust.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/synth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:36:01.793161 pysyncon-1.5.0/pysyncon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-11 20:36:01.000000 pysyncon-1.5.0/pysyncon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-11 20:36:01.000000 pysyncon-1.5.0/pysyncon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 20:36:01.000000 pysyncon-1.5.0/pysyncon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-11 20:36:01.000000 pysyncon-1.5.0/pysyncon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 20:36:01.000000 pysyncon-1.5.0/pysyncon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-11 20:36:01.797161 pysyncon-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:36:01.793161 pysyncon-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_augsynth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_augsynth_basque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_conformal_interence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19419 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_dataprep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_linear_factor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_penalized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_penalized_basque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_robust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_robust_basque.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_synth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_synth_basque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_synth_germany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_synth_texas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_utils.py
```

### Comparing `pysyncon-1.4.0/LICENSE` & `pysyncon-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysyncon-1.4.0/PKG-INFO` & `pysyncon-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysyncon
-Version: 1.4.0
+Version: 1.5.0
 Home-page: https://github.com/sdfordham/pysyncon/
 Author: Stiofán Fordham
 License: MIT License
 Keywords: Synth,augsynth,synthetic-control-method,causal-inference
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -22,17 +22,17 @@
 A python module for the synthetic control method that provides implementations of:
 
 - Synthetic Control Method (Abadie & Gardeazabal 2003)
 - Robust Synthetic Control Method (Amjad, Shah & Shen 2018)
 - Augmented Synthetic Control Method (Ben-Michael, Feller & Rothstein 2021)
 - Penalized Synthetic Control Method (Abadie & L'Hour 2021)
 
-The package also provides methods for performing placebo tests with the above.
+The package also provides methods for performing placebo tests and generating confidence intervals.
 
-The implementations of the Synthetic Control method aims to be reconcilable with the R package [Synth](https://CRAN.R-project.org/package=Synth) and similarly the implementation of the Augmented Synthetic Control method and the R package [augsynth](https://github.com/ebenmichael/augsynth).
+The implementation of the synthetic control method aims to be reconcilable with the R package [Synth](https://CRAN.R-project.org/package=Synth) and similarly the implementation of the Augmented synthetic control method and the R package [augsynth](https://github.com/ebenmichael/augsynth).
 
 ## Installation
 Install it from PyPI using pip:
 
 ````bash
 python -m pip install pysyncon
 ````
```

### Comparing `pysyncon-1.4.0/README.md` & `pysyncon-1.5.0/pysyncon.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,38 @@
+Metadata-Version: 2.1
+Name: pysyncon
+Version: 1.5.0
+Home-page: https://github.com/sdfordham/pysyncon/
+Author: Stiofán Fordham
+License: MIT License
+Keywords: Synth,augsynth,synthetic-control-method,causal-inference
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.24.0
+Requires-Dist: matplotlib>=3.6.2
+Requires-Dist: pandas>=1.5.2
+Requires-Dist: scipy>=1.9.3
+Provides-Extra: dev
+Requires-Dist: black==23.10.1; extra == "dev"
+
 
 
 # pysyncon ![](https://img.shields.io/badge/python-3.8+-blue.svg) [![codecov](https://codecov.io/gh/sdfordham/pysyncon/graph/badge.svg?token=hmi7xHQ4OT)](https://codecov.io/gh/sdfordham/pysyncon)
 
 A python module for the synthetic control method that provides implementations of:
 
 - Synthetic Control Method (Abadie & Gardeazabal 2003)
 - Robust Synthetic Control Method (Amjad, Shah & Shen 2018)
 - Augmented Synthetic Control Method (Ben-Michael, Feller & Rothstein 2021)
 - Penalized Synthetic Control Method (Abadie & L'Hour 2021)
 
-The package also provides methods for performing placebo tests with the above.
+The package also provides methods for performing placebo tests and generating confidence intervals.
 
-The implementations of the Synthetic Control method aims to be reconcilable with the R package [Synth](https://CRAN.R-project.org/package=Synth) and similarly the implementation of the Augmented Synthetic Control method and the R package [augsynth](https://github.com/ebenmichael/augsynth).
+The implementation of the synthetic control method aims to be reconcilable with the R package [Synth](https://CRAN.R-project.org/package=Synth) and similarly the implementation of the Augmented synthetic control method and the R package [augsynth](https://github.com/ebenmichael/augsynth).
 
 ## Installation
 Install it from PyPI using pip:
 
 ````bash
 python -m pip install pysyncon
 ````
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pysyncon-1.4.0/pysyncon/augsynth.py` & `pysyncon-1.5.0/pysyncon/augsynth.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .dataprep import Dataprep
 from .base import BaseSynth, VanillaOptimMixin
 from .utils import HoldoutSplitter, CrossValidationResult
 
 
 class AugSynth(BaseSynth, VanillaOptimMixin):
     """Implementation of the augmented synthetic control method due to Ben-
-    Michael, Feller & Rothstein.
+    Michael, Feller & Rothstein :cite:`augsynth2021`.
 
     The implementation follows the augsynth R package with the option
     `progfunc="Ridge"`.
     """
 
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `pysyncon-1.4.0/pysyncon/dataprep.py` & `pysyncon-1.5.0/pysyncon/dataprep.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,16 +195,16 @@
     ) -> tuple[pd.DataFrame, Union[pd.Series, pd.DataFrame]]:
         """Generate the covariate matrices to use as input to the fit method
         of the synthetic control computation.
 
         Returns
         -------
         tuple[pandas.DataFrame, pandas.Series]
-            Returns the matrices X0, X1 (using the notation of the Abadie,
-            Diamond & Hainmueller paper).
+            Returns the matrices :math:`X_0`, :math:`X_1` (using the notation of Abadie
+            & Gardeazabal :cite:`basque2003`).
 
         :meta private:
         """
         X_nonspecial = (
             self.foo[self.foo[self.time_variable].isin(self.time_predictors_prior)]
             .groupby(self.unit_variable)[self.predictors]
             .agg(self.predictors_op)
@@ -260,28 +260,28 @@
             )
         X1 = pd.concat([X1_nonspecial, X1_special], axis=0)
         return X0, X1
 
     def make_outcome_mats(
         self, time_period: Optional[IsinArg_t] = None
     ) -> tuple[pd.DataFrame, Union[pd.Series, pd.DataFrame]]:
-        """Generates the time-series matrices to use as input to the fit
+        """Generates the time-series (outcome) matrices to use as input to the fit
         method of the synthetic control computation.
 
         Parameters
         ----------
         time_period : Iterable | pandas.Series | dict, optional
             Time period to use when generating the matrices, defaults to
             time_optimize_ssr set when initialising the class, by default None
 
         Returns
         -------
         tuple[pd.DataFrame, Union[pd.Series, pd.DataFrame]]
-            Returns the matrices Z0, Z1 (using the notation of the Abadie,
-            Diamond & Hainmueller paper).
+            Returns the matrices :math:`Z_0`, :math:`Z_1` (using the notation
+            of Abadie & Gardeazabal :cite:`basque2003`).
 
         :meta private:
         """
         time_period = time_period if time_period is not None else self.time_optimize_ssr
 
         Z = self.foo[self.foo[self.time_variable].isin(time_period)].pivot(
             index=self.time_variable, columns=self.unit_variable, values=self.dependent
```

### Comparing `pysyncon-1.4.0/pysyncon/penalized.py` & `pysyncon-1.5.0/pysyncon/penalized.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,16 @@
         V_mat: np.ndarray,
         X0: np.ndarray,
         X1: np.ndarray,
         lambda_: float,
         qp_method: Literal["SLSQP"] = "SLSQP",
         qp_options: dict = {"maxiter": 1000},
     ) -> tuple[np.ndarray, float]:
-        """Solves the weight optimisation problem in the penalized setting.
+        """Solves the weight optimisation problem in the penalized setting,
+        see Abadie & L'Hour :cite:`penalized2021`.
 
         Parameters
         ----------
         V_mat : numpy.ndarray, shape (c, c)
             The V matrix (using the notation of the Abadie, Diamond &
             Hainmueller paper, this matrix is denoted by Γ in the Abadie and
             L'Hour paper).
@@ -72,15 +73,15 @@
         )
         W, loss_W = res["x"], res["fun"]
         return W, loss_W.item()
 
 
 class PenalizedSynth(BaseSynth, PenalizedOptimMixin):
     """Implementation of the penalized synthetic control method due to
-    Abadie & L'Hourblack.
+    Abadie & L'Hour :cite:`penalized2021`.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.loss_W: Optional[float] = None
         self.lambda_: Optional[float] = None
```

### Comparing `pysyncon-1.4.0/pysyncon/robust.py` & `pysyncon-1.5.0/pysyncon/robust.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from .dataprep import Dataprep
 from .base import BaseSynth
 
 
 class RobustSynth(BaseSynth):
     """Implementation of the robust synthetic control method due to
-    `Amjad, Shah & Shen <https://www.jmlr.org/papers/volume19/17-777/17-777.pdf>`_.
+    Amjad, Shah & Shen :cite:`robust2018`.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.W: Optional[np.ndarray] = None
         self.lambda_: Optional[float] = None
 
@@ -68,33 +68,33 @@
 
     def _sv_decomposition(
         self,
         Y: np.ndarray,
         threshold: Optional[float] = None,
         sv_count: Optional[int] = None,
     ) -> np.ndarray:
-        """Calculate the M_hat matrix from the paper by carrying out
-        an SVD of the outcome matrix and remove the specified number
+        """Calculate the :math:`\hat{M}` matrix from the paper (see :cite:`robust2018`) by
+        carrying out an SVD of the outcome matrix and remove the specified number
         of singular values.
 
         Parameters
         ----------
         Y : np.ndarray
-            The outcome matrix (Y matrix in the notation of the paper).
+            The outcome matrix (:math:`Y` matrix in the notation of the paper).
         threshold : Optional[float], optional
             Remove singular values that are less that `threshold`,
             either this must be specified or `sv_count`, by default None
         sv_count : Optional[int], optional
             Keep this many of the largest singular values,
             either this must be specified or `threshold`, by default None
 
         Returns
         -------
         np.ndarray
-            The M_hat matrix from the paper.
+            The :math:`\hat{M}` matrix from the paper (see :cite:`robust2018`).
 
         Raises
         ------
         ValueError
             If neither `threshold` nor `sv_count` are supplied.
 
         :meta private:
```

### Comparing `pysyncon-1.4.0/pysyncon/utils.py` & `pysyncon-1.5.0/pysyncon/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,17 +123,15 @@
         plt.grid()
         plt.show()
 
 
 class PlaceboTest:
     """Class that carries out placebo tests by running a synthetic control
     study using each possible control unit as the treated unit and the
-    remaining control units as controls. See
-    `Abadie & Gardeazabal <https://www.aeaweb.org/articles?id=10.1257/000282803321455188>`_
-    for more details.
+    remaining control units as controls. See :cite:`germany2015` for more details.
     """
 
     def __init__(self) -> None:
         self.paths: Optional[pd.DataFrame] = None
         self.treated_path: Optional[pd.DataFrame] = None
         self.gaps: Optional[pd.DataFrame] = None
         self.treated_gap: Optional[pd.DataFrame] = None
@@ -247,16 +245,17 @@
         :meta private:
         """
         scm.fit(dataprep=dataprep, **scm_options)
 
         min_ = int(min(dataprep.foo[dataprep.time_variable]))
         max_ = int(max(dataprep.foo[dataprep.time_variable]))
 
-        synthetic = scm._synthetic(time_period=range(min_, max_))
-        gaps = scm._gaps(time_period=range(min_, max_))
+        Z0, Z1 = dataprep.make_outcome_mats(time_period=range(min_, max_))
+        synthetic = scm._synthetic(Z0=Z0)
+        gaps = scm._gaps(Z0=Z0, Z1=Z1)
         return synthetic.rename(dataprep.treatment_identifier), gaps.rename(
             dataprep.treatment_identifier
         )
 
     def gaps_plot(
         self,
         time_period: Optional[IsinArg_t] = None,
@@ -276,16 +275,16 @@
             None
         grid : bool, optional
             Whether or not to plot a grid, by default True
         treatment_time : int, optional
             If supplied, plot a vertical line at the time period that the
             treatment time occurred, by default None
         mspe_threshold : float, optional
-            Remove any non-treated units whose MSPE pre-treatment is <=
-            mspe_threshold x the MSPE of the treated unit pre-treatment.
+            Remove any non-treated units whose MSPE pre-treatment is :math:`>`
+            mspe_threshold :math:`\\times` the MSPE of the treated unit pre-treatment.
             This serves to exclude any non-treated units whose synthetic control
             had a poor pre-treatment match to the actual relative to how the
             actual treated unit matched pre-treatment.
 
         Raises
         ------
         ValueError
@@ -314,16 +313,16 @@
         if treatment_time:
             plt.axvline(x=treatment_time, ymin=0.05, ymax=0.95, linestyle="dashed")
         plt.grid(grid)
         plt.show()
 
     def pvalue(self, treatment_time: int) -> float:
         """Calculate p-value of Abadie et al's version of Fisher's
-        exact hypothesis test for no effect of treatment null. See also
-        Firpo & Possebom 2017.
+        exact hypothesis test for no effect of treatment null, see also
+        section 2.2. of :cite:`fp2018`.
 
         Parameters
         ----------
         treatment_time : int
             The time period that the treatment time occurred
 
         Returns
```

### Comparing `pysyncon-1.4.0/pysyncon.egg-info/PKG-INFO` & `pysyncon-1.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,21 @@
-Metadata-Version: 2.1
-Name: pysyncon
-Version: 1.4.0
-Home-page: https://github.com/sdfordham/pysyncon/
-Author: Stiofán Fordham
-License: MIT License
-Keywords: Synth,augsynth,synthetic-control-method,causal-inference
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.24.0
-Requires-Dist: matplotlib>=3.6.2
-Requires-Dist: pandas>=1.5.2
-Requires-Dist: scipy>=1.9.3
-Provides-Extra: dev
-Requires-Dist: black==23.10.1; extra == "dev"
-
 
 
 # pysyncon ![](https://img.shields.io/badge/python-3.8+-blue.svg) [![codecov](https://codecov.io/gh/sdfordham/pysyncon/graph/badge.svg?token=hmi7xHQ4OT)](https://codecov.io/gh/sdfordham/pysyncon)
 
 A python module for the synthetic control method that provides implementations of:
 
 - Synthetic Control Method (Abadie & Gardeazabal 2003)
 - Robust Synthetic Control Method (Amjad, Shah & Shen 2018)
 - Augmented Synthetic Control Method (Ben-Michael, Feller & Rothstein 2021)
 - Penalized Synthetic Control Method (Abadie & L'Hour 2021)
 
-The package also provides methods for performing placebo tests with the above.
+The package also provides methods for performing placebo tests and generating confidence intervals.
 
-The implementations of the Synthetic Control method aims to be reconcilable with the R package [Synth](https://CRAN.R-project.org/package=Synth) and similarly the implementation of the Augmented Synthetic Control method and the R package [augsynth](https://github.com/ebenmichael/augsynth).
+The implementation of the synthetic control method aims to be reconcilable with the R package [Synth](https://CRAN.R-project.org/package=Synth) and similarly the implementation of the Augmented synthetic control method and the R package [augsynth](https://github.com/ebenmichael/augsynth).
 
 ## Installation
 Install it from PyPI using pip:
 
 ````bash
 python -m pip install pysyncon
 ````
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pysyncon-1.4.0/pysyncon.egg-info/SOURCES.txt` & `pysyncon-1.5.0/pysyncon.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,26 +2,30 @@
 README.md
 pyproject.toml
 setup.cfg
 pysyncon/__init__.py
 pysyncon/augsynth.py
 pysyncon/base.py
 pysyncon/dataprep.py
+pysyncon/generator.py
+pysyncon/inference.py
 pysyncon/penalized.py
 pysyncon/robust.py
 pysyncon/synth.py
 pysyncon/utils.py
 pysyncon.egg-info/PKG-INFO
 pysyncon.egg-info/SOURCES.txt
 pysyncon.egg-info/dependency_links.txt
 pysyncon.egg-info/requires.txt
 pysyncon.egg-info/top_level.txt
 tests/test_augsynth.py
 tests/test_augsynth_basque.py
+tests/test_conformal_interence.py
 tests/test_dataprep.py
+tests/test_linear_factor_model.py
 tests/test_penalized.py
 tests/test_penalized_basque.py
 tests/test_robust.py
 tests/test_robust_basque.py
 tests/test_synth.py
 tests/test_synth_basque.py
 tests/test_synth_germany.py
```

### Comparing `pysyncon-1.4.0/setup.cfg` & `pysyncon-1.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pysyncon
-version = 1.4.0
+version = 1.5.0
 author = Stiofán Fordham
 url = https://github.com/sdfordham/pysyncon/
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = Synth,augsynth,synthetic-control-method,causal-inference,
 license = MIT License
```

### Comparing `pysyncon-1.4.0/tests/test_augsynth.py` & `pysyncon-1.5.0/tests/test_augsynth.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.4.0/tests/test_augsynth_basque.py` & `pysyncon-1.5.0/tests/test_augsynth_basque.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.4.0/tests/test_dataprep.py` & `pysyncon-1.5.0/tests/test_dataprep.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.4.0/tests/test_penalized.py` & `pysyncon-1.5.0/tests/test_penalized.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.4.0/tests/test_penalized_basque.py` & `pysyncon-1.5.0/tests/test_penalized_basque.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.4.0/tests/test_robust.py` & `pysyncon-1.5.0/tests/test_robust.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.4.0/tests/test_robust_basque.py` & `pysyncon-1.5.0/tests/test_robust_basque.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.4.0/tests/test_synth.py` & `pysyncon-1.5.0/tests/test_synth.py`

 * *Files 20% similar despite different names*

```diff
@@ -56,29 +56,27 @@
 
         dataprep = pysyncon.Dataprep(
             treatment_identifier=self.treatment_identifier,
             controls_identifier=self.controls_identifier,
             **kwargs,
         )
         synth = pysyncon.Synth()
-        try:
-            synth.fit(dataprep)
-        except Exception as e:
-            self.fail(f"Synth fit with single treated failed: {e}.")
+
+        # Run with normal controls list
+        synth.fit(dataprep)
 
         dataprep = pysyncon.Dataprep(
             treatment_identifier=[self.treatment_identifier],
             controls_identifier=self.controls_identifier,
             **kwargs,
         )
         synth = pysyncon.Synth()
-        try:
-            synth.fit(dataprep)
-        except Exception as e:
-            self.fail(f"Synth fit with single treated in list failed: {e}.")
+
+        # Run with a list of treatment identifiers
+        synth.fit(dataprep)
 
     def test_X0_X1_fit(self):
         synth = pysyncon.Synth()
 
         # Neither dataprep nor matrices set
         self.assertRaises(ValueError, synth.fit)
 
@@ -272,7 +270,115 @@
 
         synth = pysyncon.Synth()
         synth.dataprep = dataprep
         # No weights availble/fit not run available
         self.assertRaises(ValueError, synth.mspe)
         self.assertRaises(ValueError, synth.mape)
         self.assertRaises(ValueError, synth.mae)
+
+    def test_confidence_intervals(self):
+        kwargs = {
+            "foo": self.foo,
+            "predictors": self.predictors,
+            "predictors_op": self.predictors_op,
+            "dependent": self.dependent,
+            "unit_variable": self.unit_variable,
+            "time_variable": self.time_variable,
+            "treatment_identifier": self.treatment_identifier,
+            "controls_identifier": self.controls_identifier,
+            "time_predictors_prior": self.time_predictors_prior,
+            "time_optimize_ssr": self.time_optimize_ssr,
+            "special_predictors": self.special_predictors,
+        }
+
+        dataprep = pysyncon.Dataprep(**kwargs)
+        synth = pysyncon.Synth()
+        synth.fit(dataprep=dataprep)
+
+        # Bad option
+        self.assertRaises(
+            ValueError,
+            synth.confidence_interval,
+            alpha=0.5,
+            time_periods=[4],
+            tol=0.01,
+            method="foo",
+        )
+
+        # Run with dataprep supplied
+        synth.confidence_interval(
+            alpha=0.5, time_periods=[4], dataprep=dataprep, tol=0.01
+        )
+
+        # Too few time periods for alpha value
+        self.assertRaises(
+            ValueError,
+            synth.confidence_interval,
+            alpha=0.05,
+            time_periods=[4],
+            tol=0.01,
+            dataprep=dataprep,
+        )
+
+        # Run without dataprep supplied
+        synth.confidence_interval(alpha=0.5, time_periods=[4], tol=0.01)
+
+        # Too few time periods for alpha value
+        self.assertRaises(
+            ValueError,
+            synth.confidence_interval,
+            alpha=0.05,
+            time_periods=[4],
+            tol=0.01,
+        )
+
+        # Without dataprep supplied or matrices
+        synth.dataprep = None
+        self.assertRaises(
+            ValueError, synth.confidence_interval, alpha=0.5, time_periods=[4], tol=0.01
+        )
+
+        # No pre-periods supplied
+        synth.dataprep = None
+        X0, X1 = dataprep.make_covariate_mats()
+        Z0, Z1 = dataprep.make_outcome_mats(time_period=[1, 2, 3, 4])
+        self.assertRaises(
+            ValueError,
+            synth.confidence_interval,
+            alpha=0.5,
+            time_periods=[4],
+            tol=0.01,
+            X0=X0,
+            X1=X1,
+            Z0=Z0,
+            Z1=Z1,
+        )
+
+        # Bad alpha value
+        self.assertRaises(
+            ValueError,
+            synth.confidence_interval,
+            alpha=0.05,
+            time_periods=[4],
+            pre_periods=[1, 2, 3],
+            tol=0.01,
+            X0=X0,
+            X1=X1,
+            Z0=Z0,
+            Z1=Z1,
+        )
+
+        # Dataframes supplied instead of series
+        X1 = X1.to_frame()
+        Z1 = Z1.to_frame()
+        self.assertRaises(
+            TypeError,
+            synth.confidence_interval,
+            alpha=0.5,
+            time_periods=[4],
+            pre_periods=[1, 2, 3],
+            tol=0.01,
+            X0=X0,
+            X1=X1,
+            Z0=Z0,
+            Z1=Z1,
+        )
```

### Comparing `pysyncon-1.4.0/tests/test_synth_basque.py` & `pysyncon-1.5.0/tests/test_synth_basque.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.4.0/tests/test_synth_germany.py` & `pysyncon-1.5.0/tests/test_synth_germany.py`

 * *Files 26% similar despite different names*

```diff
@@ -100,14 +100,70 @@
             "Portugal": 0.0,
             "Spain": 0.0,
             "Australia": 0.0,
             "New Zealand": 0.0,
         }
         self.att = {"att": -1555.1346777620479, "se": 317.6469306023242}
         self.att_time_period = range(1990, 2004)
+        self.cis = {
+            "value": {
+                1991: 279.09685975333196,
+                1992: 99.76203427529981,
+                1993: -631.5437231770848,
+                1994: -1050.2679900905205,
+                1995: -1205.2549226793199,
+                1996: -1467.2491625958974,
+                1997: -1954.3741689815615,
+                1998: -2008.3960300490326,
+                1999: -2160.627036515649,
+                2000: -2620.7330909274606,
+            },
+            "lower_ci": {
+                1991: 43.148688105431994,
+                1992: -136.18613737260014,
+                1993: -867.4918948249846,
+                1994: -1286.2161617384206,
+                1995: -1441.20309432722,
+                1996: -1703.1973342437975,
+                1997: -2190.3223406294615,
+                1998: -2244.3442016969325,
+                1999: -2396.5752081635487,
+                2000: -2856.6812625753605,
+            },
+            "upper_ci": {
+                1991: 515.0450314012319,
+                1992: 335.7102059231998,
+                1993: -395.59555152918483,
+                1994: -814.3198184426207,
+                1995: -969.3067510314198,
+                1996: -1231.3009909479972,
+                1997: -1718.4259973336614,
+                1998: -1772.4478584011324,
+                1999: -1924.6788648677486,
+                2000: -2384.7849192795607,
+            },
+        }
+        self.ci_args = {
+            "alpha": 0.05,
+            "time_periods": [
+                1991,
+                1992,
+                1993,
+                1994,
+                1995,
+                1996,
+                1997,
+                1998,
+                1999,
+                2000,
+            ],
+            "max_iter": 50,
+            "tol": 0.1,
+            "verbose": False,
+        }
 
     def test_weights(self):
         synth = Synth()
         synth.fit(
             dataprep=self.dataprep,
             optim_method=self.optim_method,
             optim_initial=self.optim_initial,
@@ -131,7 +187,25 @@
         # Allow a tolerance of 2.5%
         att_perc_delta = abs(1.0 - self.att["att"] / synth_att["att"])
         self.assertLessEqual(att_perc_delta, 0.025)
 
         # Allow a tolerance of 2.5%
         se_perc_delta = abs(1.0 - self.att["se"] / synth_att["se"])
         self.assertLessEqual(se_perc_delta, 0.025)
+
+    def test_cis(self):
+        synth = Synth()
+        synth.fit(
+            dataprep=self.dataprep,
+            optim_method=self.optim_method,
+            optim_initial=self.optim_initial,
+            custom_V=self.custom_V,
+        )
+
+        cis = pd.DataFrame.from_dict(self.cis)
+        cis.index.name = "time"
+        pd.testing.assert_frame_equal(
+            cis,
+            synth.confidence_interval(custom_V=self.custom_V, **self.ci_args),
+            check_exact=False,
+            atol=0.025,
+        )
```

### Comparing `pysyncon-1.4.0/tests/test_synth_texas.py` & `pysyncon-1.5.0/tests/test_synth_texas.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.4.0/tests/test_utils.py` & `pysyncon-1.5.0/tests/test_utils.py`

 * *Files identical despite different names*

