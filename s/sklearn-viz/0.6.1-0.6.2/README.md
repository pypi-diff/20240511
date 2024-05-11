# Comparing `tmp/sklearn_viz-0.6.1.tar.gz` & `tmp/sklearn_viz-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_viz-0.6.1.tar", max compression
+gzip compressed data, was "sklearn_viz-0.6.2.tar", max compression
```

## Comparing `sklearn_viz-0.6.1.tar` & `sklearn_viz-0.6.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/LICENSE
--rw-r--r--   0        0        0      354 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/README.md
--rw-r--r--   0        0        0      165 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/components/__init__.py
--rw-r--r--   0        0        0     5912 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/components/estimators.py
--rw-r--r--   0        0        0      811 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/components/kfold.py
--rw-r--r--   0        0        0      329 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/features/__init__.py
--rw-r--r--   0        0        0     8306 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/features/importance.py
--rw-r--r--   0        0        0     4633 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/features/outlier_detection.py
--rw-r--r--   0        0        0     2403 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/features/parallel_coordinates.py
--rw-r--r--   0        0        0    16590 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/features/principal_components.py
--rw-r--r--   0        0        0      643 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/features/scatter_matrix.py
--rw-r--r--   0        0        0      129 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/__init__.py
--rw-r--r--   0        0        0    11248 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/cross_validation.py
--rw-r--r--   0        0        0     6079 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/learning_curve.py
--rw-r--r--   0        0        0     1572 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/metrics.py
--rw-r--r--   0        0        0    13278 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/model_selection.py
--rw-r--r--   0        0        0     2497 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/models.py
--rw-r--r--   0        0        0      508 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/scorers.py
--rw-r--r--   0        0        0       21 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/residuals/__init__.py
--rw-r--r--   0        0        0     2058 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/residuals/error.py
--rw-r--r--   0        0        0       28 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/utils/__init__.py
--rw-r--r--   0        0        0      544 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/utils/file.py
--rw-r--r--   0        0        0     3033 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/utils/plotly.py
--rw-r--r--   0        0        0     3111 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/utils/timer.py
--rw-r--r--   0        0        0      977 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 sklearn_viz-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/LICENSE
+-rw-r--r--   0        0        0      354 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/README.md
+-rw-r--r--   0        0        0      165 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/components/__init__.py
+-rw-r--r--   0        0        0     5912 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/components/estimators.py
+-rw-r--r--   0        0        0      811 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/components/kfold.py
+-rw-r--r--   0        0        0      329 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/features/__init__.py
+-rw-r--r--   0        0        0     8306 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/features/importance.py
+-rw-r--r--   0        0        0     4633 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/features/outlier_detection.py
+-rw-r--r--   0        0        0     2403 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/features/parallel_coordinates.py
+-rw-r--r--   0        0        0    16590 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/features/principal_components.py
+-rw-r--r--   0        0        0      643 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/features/scatter_matrix.py
+-rw-r--r--   0        0        0      129 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/model_selection/__init__.py
+-rw-r--r--   0        0        0    11800 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/model_selection/cross_validation.py
+-rw-r--r--   0        0        0     6079 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/model_selection/learning_curve.py
+-rw-r--r--   0        0        0     1572 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/model_selection/metrics.py
+-rw-r--r--   0        0        0    13673 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/model_selection/model_selection.py
+-rw-r--r--   0        0        0     2497 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/model_selection/models.py
+-rw-r--r--   0        0        0      508 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/model_selection/scorers.py
+-rw-r--r--   0        0        0       21 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/residuals/__init__.py
+-rw-r--r--   0        0        0     2058 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/residuals/error.py
+-rw-r--r--   0        0        0       28 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/utils/__init__.py
+-rw-r--r--   0        0        0      544 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/utils/file.py
+-rw-r--r--   0        0        0     3033 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/utils/plotly.py
+-rw-r--r--   0        0        0     3111 2024-05-10 22:57:45.616284 sklearn_viz-0.6.2/elphick/sklearn_viz/utils/timer.py
+-rw-r--r--   0        0        0      977 2024-05-10 22:57:45.620284 sklearn_viz-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 sklearn_viz-0.6.2/PKG-INFO
```

### Comparing `sklearn_viz-0.6.1/LICENSE` & `sklearn_viz-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/components/estimators.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/components/estimators.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/components/kfold.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/components/kfold.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/features/importance.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/features/importance.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/features/outlier_detection.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/features/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/features/parallel_coordinates.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/features/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/features/principal_components.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/features/principal_components.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/features/scatter_matrix.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/features/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/cross_validation.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/model_selection/cross_validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import logging
+import math
+import multiprocessing
+import time
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
+from datetime import datetime
 from typing import Dict, Any, Union, Optional
 from typing import List
 
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator, is_classifier, is_regressor
 from sklearn.model_selection import KFold, cross_validate
@@ -30,15 +34,18 @@
                  datasets: Union[pd.DataFrame, Dict[str, pd.DataFrame]],
                  target: str,
                  pre_processor: Optional[Any],
                  cv: Union[int, Any],
                  scorer: Any,
                  metrics: Optional[Dict[str, Any]],
                  group: Any,
-                 random_state: int):
+                 random_state: int,
+                 n_jobs: Union[int, str] = 1):
+
+        self._logger = logging.getLogger(self.__class__.__name__)
 
         # If algorithms is not a dictionary, convert it into a dictionary with a default key
         if not isinstance(estimators, dict):
             estimators = {'estimator': estimators}
 
         # If datasets is not a dictionary, convert it into a dictionary with a default key
         if not isinstance(datasets, dict):
@@ -67,32 +74,38 @@
         self.target: str = target
         self.pre_processor: Optional[Any] = pre_processor
         self.cv: Union[int, Any] = cv
         self.scorer: Any = scorer
         self.metrics: Dict[str, Any] = metrics
         self.group: Any = group
         self.random_state: int = random_state
+        self.n_jobs: int = n_jobs
 
         self._logger: logging.Logger = logging.getLogger(self.__class__.__name__)
         self._results: Optional[CrossValidationResult] = None
 
         self.features_in: List[str] = [col for col in self.datasets[list(self.datasets.keys())[0]] if
                                        col != self.target]
 
         self._data: Optional[Dict] = None
         self._num_algorithms: int = len(list(self.estimators.keys()))
         self._num_datasets: int = len(list(self.datasets.keys()))
 
     @property
+    def n_cores(self) -> int:
+        n_cores = self.n_jobs
+        if self.n_jobs < 0:
+            n_cores = multiprocessing.cpu_count() + 1 + self.n_jobs
+        return n_cores
+
+    @property
     def results(self) -> Optional[Dict[str, Dict[str, CrossValidationResult]]]:
         if self._results is None:
-            if self.metrics is None:
-                cv_kwargs: Dict = dict()
-            else:
-                cv_kwargs: Dict = dict(return_estimator=True, return_indices=True, error_score=np.nan)
+
+            _tic = datetime.now()
 
             d_results: Dict = {data_key: {algo_key: {} for algo_key in self.estimators.keys()} for data_key in
                                self.datasets.keys()}
             for data_key, data in self.datasets.items():
                 self._logger.info(f"Commencing Cross Validation for dataset {data_key}")
                 d_results[data_key] = {}
                 # Ensure that only the features present in the dataset are used
@@ -104,15 +117,16 @@
 
                 for estimator_key, estimator in self.estimators.items():
                     if isinstance(self.cv, int):
                         cv = KFold(n_splits=self.cv, random_state=self.random_state, shuffle=True)
                     else:
                         cv = self.cv
                     res = cross_validate(estimator, x, y, cv=cv, scoring=self.scorer, return_train_score=True,
-                                         **cv_kwargs)
+                                         return_estimator=True, return_indices=True, error_score=np.nan,
+                                         n_jobs=self.n_jobs)
                     if self.metrics is not None:
                         res['metrics'], res['metrics_group'] = self.calculate_metrics(x=x, y=y,
                                                                                       estimators=res['estimator'],
                                                                                       indices=res['indices'],
                                                                                       group=self.group)
                     # Convert the results to a CrossValidationResult instance and assign it
                     d_results[data_key][estimator_key] = CrossValidationResult(
@@ -128,14 +142,18 @@
                     res_mean = res[f"test_score"].mean()
                     res_std = res[f"test_score"].std()
 
                     self._logger.info(f"CV Results for {estimator_key}: Mean = {res_mean}, SD = {res_std}")
 
             self._results = d_results
 
+            self._logger.info(
+                f"Cross Validation complete in {datetime.now() - _tic} using {self.n_cores} "
+                f"worker{'s' if self.n_cores > 1 else ''}")
+
         return self._results
 
     @abstractmethod
     def get_cv_scores(self):
         chunks: List = []
         for data_key, data in self.datasets.items():
             for estimator_key, estimator in self.estimators.items():
```

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/learning_curve.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/model_selection/learning_curve.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/metrics.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/model_selection/metrics.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/model_selection.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/model_selection/model_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,34 +51,39 @@
                  datasets: Union[pd.DataFrame, Dict[str, pd.DataFrame]],
                  target: str,
                  pre_processor: Optional[Pipeline] = None,
                  k_folds: int = 10,
                  scorer: Optional[Union[str, Callable]] = None,
                  metrics: Optional[Dict[str, Callable]] = None,
                  group: Optional[pd.Series] = None,
-                 random_state: Optional[int] = None):
+                 random_state: Optional[int] = None,
+                 n_jobs: Union[int, str] = 1):
         """
 
         Args:
             estimators: sklearn estimator or a Dict of algorithms to cross-validate, keyed by string name/code.
             datasets: pandas DataFrame or a dict of DataFrames, keyed by string name/code.
             target: target column
             pre_processor: Optional pipeline used to pre-process the datasets.
             k_folds: The number of cross validation folds.
             scorer: Optional callable scorers which the model will be fitted using
             metrics: Optional Dict of callable metrics to calculate post-fitting
             group: Optional group variable by which to partition/group metrics.  The same group applies across all
              datasets, so is more useful when testing different algorithms.
             random_state: Optional random seed
+            n_jobs: Number of parallel jobs to run.  If -1, then the number of jobs is set to the number of CPU cores.
+             Recommend setting to -2 for large jobs to retain a core for system interaction.  If set to 'auto' and `cv`
+             is an integer, the optimum number of jobs is calculated.
         """
 
         self._logger = logging.getLogger(name=__class__.__name__)
 
         super().__init__(estimators=estimators, datasets=datasets, target=target, pre_processor=pre_processor,
-                         cv=k_folds, scorer=scorer, metrics=metrics, group=group, random_state=random_state)
+                         cv=k_folds, scorer=scorer, metrics=metrics, group=group, random_state=random_state,
+                         n_jobs=n_jobs)
 
     def plot(self,
              metrics: Optional[Union[str, List[str]]] = None,
              show_group: bool = False,
              title: Optional[str] = None,
              col_wrap: Optional[int] = None) -> go.Figure:
         """Create the plot
```

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/models.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/model_selection/models.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/residuals/error.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/residuals/error.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/utils/file.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/utils/file.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/utils/plotly.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/utils/plotly.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/elphick/sklearn_viz/utils/timer.py` & `sklearn_viz-0.6.2/elphick/sklearn_viz/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.1/pyproject.toml` & `sklearn_viz-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sklearn-viz"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 authors = ["Greg <11791585+elphick@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "elphick/sklearn_viz" }]
 
 [[tool.poetry.source]]
 name = "PyPI"
```

### Comparing `sklearn_viz-0.6.1/PKG-INFO` & `sklearn_viz-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-viz
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 Author: Greg
 Author-email: 11791585+elphick@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

