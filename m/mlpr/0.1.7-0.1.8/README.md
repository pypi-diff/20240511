# Comparing `tmp/mlpr-0.1.7.tar.gz` & `tmp/mlpr-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpr-0.1.7.tar", max compression
+gzip compressed data, was "mlpr-0.1.8.tar", max compression
```

## Comparing `mlpr-0.1.7.tar` & `mlpr-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      289 2024-05-11 02:18:39.159292 mlpr-0.1.7/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2024-04-27 16:49:57.314542 mlpr-0.1.7/LICENSE
--rw-r--r--   0        0        0    30224 2024-05-11 11:17:49.752969 mlpr-0.1.7/README.md
--rw-r--r--   0        0        0      256 2024-05-11 02:24:23.791737 mlpr-0.1.7/SECURITY.md
--rw-r--r--   0        0        0     2502 2024-05-11 16:01:24.031457 mlpr-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       70 2024-05-11 16:01:21.023407 mlpr-0.1.7/src/mlpr/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.7/src/mlpr/ml/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 18:27:54.717513 mlpr-0.1.7/src/mlpr/ml/supervisioned/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 18:28:38.701333 mlpr-0.1.7/src/mlpr/ml/supervisioned/classification/__init__.py
--rw-r--r--   0        0        0    12544 2024-05-11 15:17:49.862210 mlpr-0.1.7/src/mlpr/ml/supervisioned/classification/metrics.py
--rw-r--r--   0        0        0     5103 2024-05-11 02:06:39.037536 mlpr-0.1.7/src/mlpr/ml/supervisioned/classification/uncertainty.py
--rw-r--r--   0        0        0     2242 2024-05-11 01:58:21.065745 mlpr-0.1.7/src/mlpr/ml/supervisioned/classification/utils.py
--rw-r--r--   0        0        0        0 2024-04-27 18:28:52.537279 mlpr-0.1.7/src/mlpr/ml/supervisioned/forecasting/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 23:35:52.450714 mlpr-0.1.7/src/mlpr/ml/supervisioned/regression/__init__.py
--rw-r--r--   0        0        0    18436 2024-05-05 00:35:48.981115 mlpr-0.1.7/src/mlpr/ml/supervisioned/regression/metrics.py
--rw-r--r--   0        0        0    18464 2024-05-05 00:20:45.686332 mlpr-0.1.7/src/mlpr/ml/supervisioned/regression/plots.py
--rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.7/src/mlpr/ml/supervisioned/tunning/__init__.py
--rw-r--r--   0        0        0     6314 2024-05-10 23:01:04.220209 mlpr-0.1.7/src/mlpr/ml/supervisioned/tunning/grid_search.py
--rw-r--r--   0        0        0       62 2024-04-27 21:43:09.387068 mlpr-0.1.7/src/mlpr/reports/__init__.py
--rw-r--r--   0        0        0     1742 2024-05-04 23:35:34.703861 mlpr-0.1.7/src/mlpr/reports/create.py
--rw-r--r--   0        0        0    32185 1970-01-01 00:00:00.000000 mlpr-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      289 2024-05-11 02:18:39.159292 mlpr-0.1.8/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2024-04-27 16:49:57.314542 mlpr-0.1.8/LICENSE
+-rw-r--r--   0        0        0    30200 2024-05-11 16:06:30.324399 mlpr-0.1.8/README.md
+-rw-r--r--   0        0        0      256 2024-05-11 02:24:23.791737 mlpr-0.1.8/SECURITY.md
+-rw-r--r--   0        0        0     2502 2024-05-11 16:49:47.333980 mlpr-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-05-11 16:49:50.565708 mlpr-0.1.8/src/mlpr/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.8/src/mlpr/ml/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:27:54.717513 mlpr-0.1.8/src/mlpr/ml/supervisioned/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:28:38.701333 mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/__init__.py
+-rw-r--r--   0        0        0    13901 2024-05-11 16:38:36.531053 mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/metrics.py
+-rw-r--r--   0        0        0     5103 2024-05-11 02:06:39.037536 mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/uncertainty.py
+-rw-r--r--   0        0        0     2242 2024-05-11 01:58:21.065745 mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:28:52.537279 mlpr-0.1.8/src/mlpr/ml/supervisioned/forecasting/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 23:35:52.450714 mlpr-0.1.8/src/mlpr/ml/supervisioned/regression/__init__.py
+-rw-r--r--   0        0        0    18436 2024-05-05 00:35:48.981115 mlpr-0.1.8/src/mlpr/ml/supervisioned/regression/metrics.py
+-rw-r--r--   0        0        0    18464 2024-05-05 00:20:45.686332 mlpr-0.1.8/src/mlpr/ml/supervisioned/regression/plots.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.8/src/mlpr/ml/supervisioned/tunning/__init__.py
+-rw-r--r--   0        0        0     6314 2024-05-10 23:01:04.220209 mlpr-0.1.8/src/mlpr/ml/supervisioned/tunning/grid_search.py
+-rw-r--r--   0        0        0       62 2024-04-27 21:43:09.387068 mlpr-0.1.8/src/mlpr/reports/__init__.py
+-rw-r--r--   0        0        0     1742 2024-05-04 23:35:34.703861 mlpr-0.1.8/src/mlpr/reports/create.py
+-rw-r--r--   0        0        0    32161 1970-01-01 00:00:00.000000 mlpr-0.1.8/PKG-INFO
```

### Comparing `mlpr-0.1.7/LICENSE` & `mlpr-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.7/README.md` & `mlpr-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 
 MLPR for model selection.
 
 ## Importing the Library
 First, import the necessary modules from the library:
 
 ```python
-from typing import Dict
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
 from sklearn.base import BaseEstimator
 from sklearn.ensemble import RandomForestClassifier, GradientBoostingClassifier
 from sklearn.linear_model import LogisticRegression
@@ -156,15 +155,15 @@
 ```
 
 [![fig0](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/tunning_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/tunning_scatter.png)
 
 ## Cross-validtion
 
 ```python
-models: Dict[BaseEstimator, Dict] = {
+models: dict[BaseEstimator, dict] = {
     RandomForestClassifier: {
         'n_estimators': [10, 50, 100, 200],
         'max_depth': [None, 5, 10, 15],
         'min_samples_split': [2, 5, 10],
         'min_samples_leaf': [1, 2, 4],
         'random_state': [random_state]
     },
@@ -463,15 +462,15 @@
 
 [![fig1](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/classification_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/classification_scatter.png)
 
 
 ## Cross-validation
 
 ```python
-models: Dict[BaseEstimator, Dict] = {
+models: dict[BaseEstimator, dict] = {
     RandomForestClassifier: {
         'n_estimators': [10, 50, 100, 200],
         'max_depth': [None, 5, 10, 15],
         'min_samples_split': [2, 5, 10],
         'min_samples_leaf': [1, 2, 4],
         'random_state': [random_state]
     },
```

#### html2text {}

```diff
@@ -19,22 +19,22 @@
 their needs. # Using the MLPR Library The MLPR library is a powerful tool for
 machine learning and data analysis. Here's a brief guide on how to use it. ##
 Installation Before you start, make sure you have installed the MLPR library.
 You can do this by running pip install mlpr. ```bash pip install mlpr ``` #
 Tunning Click [here](https://github.com/Manuelfjr/mlpr/tree/develop/notebooks/
 supervisioned/tunning/) for contents. MLPR for model selection. ## Importing
 the Library First, import the necessary modules from the library: ```python
-from typing import Dict import numpy as np import pandas as pd import
-matplotlib.pyplot as plt from sklearn.base import BaseEstimator from
-sklearn.ensemble import RandomForestClassifier, GradientBoostingClassifier from
-sklearn.linear_model import LogisticRegression from sklearn.naive_bayes import
-GaussianNB from sklearn.neighbors import KNeighborsClassifier from sklearn.svm
-import SVC from sklearn.tree import DecisionTreeClassifier from
-sklearn.datasets import make_blobs from sklearn.metrics import accuracy_score,
-precision_score, recall_score, f1_score, cohen_kappa_score from
+import numpy as np import pandas as pd import matplotlib.pyplot as plt from
+sklearn.base import BaseEstimator from sklearn.ensemble import
+RandomForestClassifier, GradientBoostingClassifier from sklearn.linear_model
+import LogisticRegression from sklearn.naive_bayes import GaussianNB from
+sklearn.neighbors import KNeighborsClassifier from sklearn.svm import SVC from
+sklearn.tree import DecisionTreeClassifier from sklearn.datasets import
+make_blobs from sklearn.metrics import accuracy_score, precision_score,
+recall_score, f1_score, cohen_kappa_score from
 mlpr.ml.supervisioned.tunning.grid_search import GridSearch ``` ## Methods Here
 we have a custom method for accuracy to use in model selection. Thus: ```python
 def custom_accuracy_score(y_true: np.ndarray, y_pred: np.ndarray) -> float:
 return accuracy_score(y_true, y_pred, normalize=False) ``` ## Loading the Data
 Load your dataset. In this example, we're generating a dataset for
 classification using sklearn: ```python n_samples = 1000 centers = [(0, 0), (3,
 4.5)] n_features = 2 cluster_std = 1.3 random_state = 42 ``` ```python
@@ -42,16 +42,16 @@
 ( n_samples=n_samples, centers=centers, n_features=n_features,
 cluster_std=cluster_std, random_state=random_state ) ``` ## Plot the dataset
 ```python fig, ax = plt.subplots(1, 1, figsize=(14, 6)) ax.plot(X[:, 0][y ==
 0], X[:, 1][y == 0], "bs") ax.plot(X[:, 0][y == 1], X[:, 1][y == 1], "g^")
 ax.set_title("Dataset") ax.set_frame_on(False) ax.set_xticks([]) ax.set_yticks(
 []) fig.tight_layout() ``` [![fig0](https://raw.githack.com/Manuelfjr/mlpr/
 develop/assets/tunning_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/
-develop/assets/tunning_scatter.png) ## Cross-validtion ```python models: Dict
-[BaseEstimator, Dict] = { RandomForestClassifier: { 'n_estimators': [10, 50,
+develop/assets/tunning_scatter.png) ## Cross-validtion ```python models: dict
+[BaseEstimator, dict] = { RandomForestClassifier: { 'n_estimators': [10, 50,
 100, 200], 'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5, 10],
 'min_samples_leaf': [1, 2, 4], 'random_state': [random_state] },
 GradientBoostingClassifier: { 'n_estimators': [50, 100, 200], 'learning_rate':
 [0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0], 'random_state':
 [random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0, 10.0], 'penalty':
 ['l1', 'l2'], 'solver': ['liblinear', 'saga'], 'random_state': [random_state]
 }, GaussianNB: { 'var_smoothing': [1e-9, 1e-8, 1e-7, 1e-6, 1e-5] },
@@ -124,15 +124,15 @@
 [y == k], marker=markers[i % len(markers)], color=colors[i], label=f"c{i}")
 ax.set_title("Dataset") ax.set_frame_on(False) ax.set_xticks([]) ax.set_yticks(
 []) for center, color in zip(centers, colors): ax.scatter( center[0], center
 [1], color="white", linewidths=3, marker="o", edgecolor="black", s=120 )
 plt.legend() fig.tight_layout() ``` [![fig1](https://raw.githack.com/Manuelfjr/
 mlpr/develop/assets/classification_scatter.png)](https://raw.githack.com/
 Manuelfjr/mlpr/develop/assets/classification_scatter.png) ## Cross-validation
-```python models: Dict[BaseEstimator, Dict] = { RandomForestClassifier:
+```python models: dict[BaseEstimator, dict] = { RandomForestClassifier:
 { 'n_estimators': [10, 50, 100, 200], 'max_depth': [None, 5, 10, 15],
 'min_samples_split': [2, 5, 10], 'min_samples_leaf': [1, 2, 4], 'random_state':
 [random_state] }, GradientBoostingClassifier: { 'n_estimators': [50, 100, 200],
 'learning_rate': [0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0],
 'random_state': [random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0,
 10.0], 'penalty': ['l1', 'l2'], 'solver': ['liblinear', 'saga'],
 'random_state': [random_state], 'max_iter': [10000] }, GaussianNB:
```

### Comparing `mlpr-0.1.7/pyproject.toml` & `mlpr-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlpr"
-version = "0.1.7"
+version = "0.1.8"
 authors = ["Manuel Ferreira Junior <ferreira.jr.ufpb@gmail.com>"]
 description = "A library for machine learning pipeline and creation of reports."
 readme = "README.md"
 maintainers = [
     "Manuel Ferreira Junior <ferreira.jr.ufpb@gmail.com>"
 ]
 classifiers=[
```

### Comparing `mlpr-0.1.7/src/mlpr/ml/supervisioned/classification/metrics.py` & `mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,22 @@
-from typing import List, Union, Callable, Dict, Optional
-import pandas as pd
+"""
+Metrics module for supervisioned learning.
+"""
+
+from typing import Callable, Dict, List, Optional, Union
+
 import numpy as np
+import pandas as pd
 import pyspark.sql
+from pyspark.ml.evaluation import (
+    BinaryClassificationEvaluator,
+    MulticlassClassificationEvaluator,
+)
+from pyspark.mllib.evaluation import MulticlassMetrics
 from sklearn import metrics as skmetrics
-from pyspark.ml import evaluation as spark_eval
 
 
 class ClassificationMetrics:
     """
     Compute classification metrics for pandas and PySpark dataframes.
 
     Parameters
@@ -23,35 +32,35 @@
     ----------
     results_ : dict
         A dictionary where the keys are the names of the metrics and the
         values are the computed metrics.
     """
 
     def __init__(
-            self,
-            metrics: Optional[Union[List[str], Callable]] = None,
-            true_target: Optional[str] = "y_true",
-            pred_target: Optional[str] = "y_pred"
-        ):
+        self,
+        metrics: Optional[Union[List[str], Callable]] = None,
+        true_target: Optional[str] = "y_true",
+        pred_target: Optional[str] = "y_pred",
+    ):
         self.metrics = metrics
         self.results_: Dict[str, float] = {}
         self.true_target: str = true_target
         self.pred_target: str = pred_target
 
     def add_metric(
-            self,
-            name: str,
-            metric_fn: Callable[
-                [
-                    Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-                    Union[pd.DataFrame, pyspark.sql.DataFrame]
-                ],
-                float
-            ]
-        ) -> 'ClassificationMetrics':
+        self,
+        name: str,
+        metric_fn: Callable[
+            [
+                Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+                Union[pd.DataFrame, pyspark.sql.DataFrame],
+            ],
+            float,
+        ],
+    ) -> "ClassificationMetrics":
         """
         Add a custom metric to the metrics dictionary.
 
         Parameters
         ----------
         name : str
             The name of the metric.
@@ -60,19 +69,19 @@
         """
         if not callable(metric_fn):
             raise ValueError("metric_fn should be a callable function")
         setattr(self, name, metric_fn)
         return self
 
     def accuracy_score(
-            self,
-            y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-            y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-            **kwargs
-        ) -> float:
+        self,
+        y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+        y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+        **kwargs,
+    ) -> float:
         """
         Compute the accuracy score.
 
         Parameters
         ----------
         y_true : pandas.DataFrame or pyspark.sql.DataFrame
             The ground truth labels.
@@ -80,37 +89,42 @@
             The predicted labels.
 
         Returns
         -------
         float
             The computed accuracy score.
         """
-        if (
-            isinstance(y_true, pd.DataFrame) and isinstance(y_pred, pd.DataFrame)
-        ) or (
-            isinstance(y_true, pd.Series) and isinstance(y_pred, pd.Series)
-        ) or (
-            isinstance(y_true, np.ndarray) and isinstance(y_pred, np.ndarray)
-        ):
+        is_dataframe: bool = isinstance(y_true, pd.DataFrame) and isinstance(y_pred, pd.DataFrame)
+        is_series: bool = isinstance(y_true, pd.Series) and isinstance(y_pred, pd.Series)
+        is_ndarray: bool = isinstance(y_true, np.ndarray) and isinstance(y_pred, np.ndarray)
+
+        if is_dataframe or is_series or is_ndarray:
             return skmetrics.accuracy_score(y_true, y_pred, **kwargs)
-        elif isinstance(y_true, pyspark.sql.DataFrame) and isinstance(y_pred, pyspark.sql.DataFrame):
-            evaluator = spark_eval.MulticlassClassificationEvaluator(
-                labelCol=self.true_target,
-                predictionCol=self.pred_target,
-                metricName="accuracy",
-                **kwargs
+        if isinstance(y_true, pyspark.sql.DataFrame) and isinstance(y_pred, pyspark.sql.DataFrame):
+            evaluator = MulticlassClassificationEvaluator(
+                labelCol=self.true_target, predictionCol=self.pred_target, metricName="accuracy", **kwargs
             )
             return evaluator.evaluate(y_pred)
+        raise ValueError(
+            """
+            y_true and y_pred arguments are not supported.
+            Must be of type:
+                pandas.DataFrame
+                pandas.Series
+                numpy.ndarray
+                pyspark.sql.DataFrame
+            """
+        )
 
     def precision_score(
-            self,
-            y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-            y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-            **kwargs
-        ) -> float:
+        self,
+        y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+        y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+        **kwargs,
+    ) -> float:
         """
         Compute the precision score.
 
         Parameters
         ----------
         y_true : pandas.DataFrame or pyspark.sql.DataFrame
             The ground truth labels.
@@ -118,37 +132,42 @@
             The predicted labels.
 
         Returns
         -------
         float
             The computed precision score.
         """
-        if (
-            isinstance(y_true, pd.DataFrame) and isinstance(y_pred, pd.DataFrame)
-        ) or (
-            isinstance(y_true, pd.Series) and isinstance(y_pred, pd.Series)
-        ) or (
-            isinstance(y_true, np.ndarray) and isinstance(y_pred, np.ndarray)
-        ):
+        is_dataframe = isinstance(y_true, pd.DataFrame) and isinstance(y_pred, pd.DataFrame)
+        is_series = isinstance(y_true, pd.Series) and isinstance(y_pred, pd.Series)
+        is_ndarray = isinstance(y_true, np.ndarray) and isinstance(y_pred, np.ndarray)
+
+        if is_dataframe or is_series or is_ndarray:
             return skmetrics.precision_score(y_true, y_pred, **kwargs)
-        elif isinstance(y_true, pyspark.sql.DataFrame) and isinstance(y_pred, pyspark.sql.DataFrame):
-            evaluator = spark_eval.MulticlassClassificationEvaluator(
-                labelCol=self.true_target,
-                predictionCol=self.pred_target,
-                metricName="weightedPrecision",
-                **kwargs
+        if isinstance(y_true, pyspark.sql.DataFrame) and isinstance(y_pred, pyspark.sql.DataFrame):
+            evaluator = MulticlassClassificationEvaluator(
+                labelCol=self.true_target, predictionCol=self.pred_target, metricName="weightedPrecision", **kwargs
             )
             return evaluator.evaluate(y_pred)
+        raise ValueError(
+            """
+            y_true and y_pred arguments are not supported.
+            Must be of type:
+                pandas.DataFrame
+                pandas.Series
+                numpy.ndarray
+                pyspark.sql.DataFrame
+            """
+        )
 
     def recall_score(
-            self,
-            y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-            y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-            **kwargs
-        ) -> float:
+        self,
+        y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+        y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+        **kwargs,
+    ) -> float:
         """
         Compute the recall score.
 
         Parameters
         ----------
         y_true : pandas.DataFrame or pyspark.sql.DataFrame
             The ground truth labels.
@@ -156,37 +175,42 @@
             The predicted labels.
 
         Returns
         -------
         float
             The computed recall score.
         """
-        if (
-            isinstance(y_true, pd.DataFrame) and isinstance(y_pred, pd.DataFrame)
-        ) or (
-            isinstance(y_true, pd.Series) and isinstance(y_pred, pd.Series)
-        ) or (
-            isinstance(y_true, np.ndarray) and isinstance(y_pred, np.ndarray)
-        ):
+        is_dataframe = isinstance(y_true, pd.DataFrame) and isinstance(y_pred, pd.DataFrame)
+        is_series = isinstance(y_true, pd.Series) and isinstance(y_pred, pd.Series)
+        is_ndarray = isinstance(y_true, np.ndarray) and isinstance(y_pred, np.ndarray)
+
+        if is_dataframe or is_series or is_ndarray:
             return skmetrics.recall_score(y_true, y_pred, **kwargs)
-        elif isinstance(y_true, pyspark.sql.DataFrame) and isinstance(y_pred, pyspark.sql.DataFrame):
-            evaluator = spark_eval.MulticlassClassificationEvaluator(
-                labelCol=self.true_target, 
-                predictionCol=self.pred_target,
-                metricName="weightedRecall",
-                **kwargs
+        if isinstance(y_true, pyspark.sql.DataFrame) and isinstance(y_pred, pyspark.sql.DataFrame):
+            evaluator = MulticlassClassificationEvaluator(
+                labelCol=self.true_target, predictionCol=self.pred_target, metricName="weightedRecall", **kwargs
             )
             return evaluator.evaluate(y_pred)
+        raise ValueError(
+            """
+            y_true and y_pred arguments are not supported.
+            Must be of type:
+                pandas.DataFrame
+                pandas.Series
+                numpy.ndarray
+                pyspark.sql.DataFrame
+            """
+        )
 
     def f1_score(
-            self,
-            y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-            y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-            **kwargs
-        ) -> float:
+        self,
+        y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+        y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+        **kwargs,
+    ) -> float:
         """
         Compute the F1 score.
 
         Parameters
         ----------
         y_true : pandas.DataFrame or pyspark.sql.DataFrame
             The ground truth labels.
@@ -194,37 +218,42 @@
             The predicted labels.
 
         Returns
         -------
         float
             The computed F1 score.
         """
-        if (
-            isinstance(y_true, pd.DataFrame) and isinstance(y_pred, pd.DataFrame)
-        ) or (
-            isinstance(y_true, pd.Series) and isinstance(y_pred, pd.Series)
-        ) or (
-            isinstance(y_true, np.ndarray) and isinstance(y_pred, np.ndarray)
-        ):
+        is_dataframe = isinstance(y_true, pd.DataFrame) and isinstance(y_pred, pd.DataFrame)
+        is_series = isinstance(y_true, pd.Series) and isinstance(y_pred, pd.Series)
+        is_ndarray = isinstance(y_true, np.ndarray) and isinstance(y_pred, np.ndarray)
+
+        if is_dataframe or is_series or is_ndarray:
             return skmetrics.f1_score(y_true, y_pred, **kwargs)
-        elif isinstance(y_true, pyspark.sql.DataFrame) and isinstance(y_pred, pyspark.sql.DataFrame):
-            evaluator = spark_eval.MulticlassClassificationEvaluator(
-                labelCol=self.true_target,
-                predictionCol=self.pred_target,
-                metricName="f1",
-                **kwargs
+        if isinstance(y_true, pyspark.sql.DataFrame) and isinstance(y_pred, pyspark.sql.DataFrame):
+            evaluator = MulticlassClassificationEvaluator(
+                labelCol=self.true_target, predictionCol=self.pred_target, metricName="f1", **kwargs
             )
             return evaluator.evaluate(y_pred)
+        raise ValueError(
+            """
+            y_true and y_pred arguments are not supported.
+            Must be of type:
+                pandas.DataFrame
+                pandas.Series
+                numpy.ndarray
+                pyspark.sql.DataFrame
+            """
+        )
 
     def roc_auc_score(
-            self,
-            y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-            y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-            **kwargs
-        ) -> float:
+        self,
+        y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+        y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+        **kwargs,
+    ) -> float:
         """
         Compute the ROC AUC score.
 
         Parameters
         ----------
         y_true : pandas.DataFrame or pyspark.sql.DataFrame
             The ground truth labels.
@@ -232,37 +261,42 @@
             The predicted labels.
 
         Returns
         -------
         float
             The computed ROC AUC score.
         """
-        if (
-            isinstance(y_true, pd.DataFrame) and isinstance(y_pred, pd.DataFrame)
-        ) or (
-            isinstance(y_true, pd.Series) and isinstance(y_pred, pd.Series)
-        ) or (
-            isinstance(y_true, np.ndarray) and isinstance(y_pred, np.ndarray)
-        ):
+        is_dataframe = isinstance(y_true, pd.DataFrame) and isinstance(y_pred, pd.DataFrame)
+        is_series = isinstance(y_true, pd.Series) and isinstance(y_pred, pd.Series)
+        is_ndarray = isinstance(y_true, np.ndarray) and isinstance(y_pred, np.ndarray)
+
+        if is_dataframe or is_series or is_ndarray:
             return skmetrics.roc_auc_score(y_true, y_pred, **kwargs)
-        elif isinstance(y_true, pyspark.sql.DataFrame) and isinstance(y_pred, pyspark.sql.DataFrame):
-            evaluator = spark_eval.BinaryClassificationEvaluator(
-                labelCol=self.true_target,
-                rawPredictionCol=self.pred_target,
-                metricName="areaUnderROC",
-                **kwargs
+        if isinstance(y_true, pyspark.sql.DataFrame) and isinstance(y_pred, pyspark.sql.DataFrame):
+            evaluator = BinaryClassificationEvaluator(
+                labelCol=self.true_target, rawPredictionCol=self.pred_target, metricName="areaUnderROC", **kwargs
             )
             return evaluator.evaluate(y_pred)
+        raise ValueError(
+            """
+            y_true and y_pred arguments are not supported.
+            Must be of type:
+                pandas.DataFrame
+                pandas.Series
+                numpy.ndarray
+                pyspark.sql.DataFrame
+            """
+        )
 
     def confusion_matrix(
-            self,
-            y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-            y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-            **kwargs
-        ) -> np.ndarray:
+        self,
+        y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+        y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+        **kwargs,
+    ) -> np.ndarray:
         """
         Compute the confusion matrix.
 
         Parameters
         ----------
         y_true : pandas.DataFrame or pyspark.sql.DataFrame
             The ground truth labels.
@@ -270,46 +304,45 @@
             The predicted labels.
 
         Returns
         -------
         numpy.ndarray
             The confusion matrix.
         """
-        if (
-            isinstance(y_true, pd.DataFrame) and isinstance(y_pred, pd.DataFrame)
-        ) or (
-            isinstance(y_true, pd.Series) and isinstance(y_pred, pd.Series)
-        ) or (
-            isinstance(y_true, np.ndarray) and isinstance(y_pred, np.ndarray)
-        ):
+        is_dataframe = isinstance(y_true, pd.DataFrame) and isinstance(y_pred, pd.DataFrame)
+        is_series = isinstance(y_true, pd.Series) and isinstance(y_pred, pd.Series)
+        is_ndarray = isinstance(y_true, np.ndarray) and isinstance(y_pred, np.ndarray)
+
+        if is_dataframe or is_series or is_ndarray:
             return skmetrics.confusion_matrix(y_true, y_pred, **kwargs)
-        elif isinstance(y_true, pyspark.sql.DataFrame) and isinstance(y_pred, pyspark.sql.DataFrame):
+        if isinstance(y_true, pyspark.sql.DataFrame) and isinstance(y_pred, pyspark.sql.DataFrame):
             predictionAndLabels = (
-                y_pred
-                .select(self.pred_target)
-                .rdd
-                .map(lambda x: float(x[0]))
-                .zip(
-                    y_true
-                    .select(self.true_target)
-                    .rdd
-                    .map(lambda x: float(x[0]))
-                )
+                y_pred.select(self.pred_target)
+                .rdd.map(lambda x: float(x[0]))
+                .zip(y_true.select(self.true_target).rdd.map(lambda x: float(x[0])))
             )
-            metrics = spark_eval.MulticlassMetrics(predictionAndLabels)
+            metrics = MulticlassMetrics(predictionAndLabels)
             confusion_matrix = metrics.confusionMatrix().toArray()
             return confusion_matrix
-        else:
-            raise ValueError("y_true and y_pred should be either pandas.DataFrame or pyspark.sql.DataFrame")
+        raise ValueError(
+            """
+            y_true and y_pred arguments are not supported.
+            Must be of type:
+                pandas.DataFrame
+                pandas.Series
+                numpy.ndarray
+                pyspark.sql.DataFrame
+            """
+        )
 
     def compute_metrics(
-            self,
-            y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
-            y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame]
-        ) -> 'ClassificationMetrics':
+        self,
+        y_true: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+        y_pred: Union[pd.DataFrame, pyspark.sql.DataFrame, pd.Series, np.ndarray],
+    ) -> "ClassificationMetrics":
         """
         Compute all the specified classification metrics.
 
         Parameters
         ----------
         y_true : pandas.DataFrame or pyspark.sql.DataFrame
             The ground truth labels.
@@ -319,19 +352,19 @@
         Returns
         -------
         self
             The ClassificationMetrics object with the computed metrics.
         """
         if self.metrics is None:
             self.metrics: dict[str, dict] = {
-                'accuracy_score': {},
-                'precision_score': {},
-                'recall_score': {},
-                'f1_score': {},
-                'roc_auc_score': {}
+                "accuracy_score": {},
+                "precision_score": {},
+                "recall_score": {},
+                "f1_score": {},
+                "roc_auc_score": {},
             }
 
         for metric, params in self.metrics.items():
             if callable(metric):
                 self.results_[metric.__name__] = metric(y_true, y_pred, **params)
                 if isinstance(self.results_[metric.__name__], (float, int)):
                     self.results_[metric.__name__] = [self.results_[metric.__name__]]
@@ -339,8 +372,9 @@
                 if hasattr(self, metric):
                     self.results_[metric] = getattr(self, metric)(y_true, y_pred, **params)
                     if isinstance(self.results_[metric], (float, int)):
                         self.results_[metric] = [self.results_[metric]]
                 else:
                     raise ValueError(f"Invalid metric: {metric}")
             else:
-                raise ValueError("Metrics should be either callable or a dictionary of str and parameters")
+                raise ValueError("Metrics should be either callable or a dictionary of str and parameters")
+        return self
```

### Comparing `mlpr-0.1.7/src/mlpr/ml/supervisioned/classification/uncertainty.py` & `mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/uncertainty.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.7/src/mlpr/ml/supervisioned/classification/utils.py` & `mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/utils.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.7/src/mlpr/ml/supervisioned/regression/metrics.py` & `mlpr-0.1.8/src/mlpr/ml/supervisioned/regression/metrics.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.7/src/mlpr/ml/supervisioned/regression/plots.py` & `mlpr-0.1.8/src/mlpr/ml/supervisioned/regression/plots.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.7/src/mlpr/ml/supervisioned/tunning/grid_search.py` & `mlpr-0.1.8/src/mlpr/ml/supervisioned/tunning/grid_search.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.7/src/mlpr/reports/create.py` & `mlpr-0.1.8/src/mlpr/reports/create.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.7/PKG-INFO` & `mlpr-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpr
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library for machine learning pipeline and creation of reports.
 Author: Manuel Ferreira Junior
 Author-email: ferreira.jr.ufpb@gmail.com
 Maintainer: Manuel Ferreira Junior
 Maintainer-email: ferreira.jr.ufpb@gmail.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
@@ -127,15 +127,14 @@
 
 MLPR for model selection.
 
 ## Importing the Library
 First, import the necessary modules from the library:
 
 ```python
-from typing import Dict
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
 from sklearn.base import BaseEstimator
 from sklearn.ensemble import RandomForestClassifier, GradientBoostingClassifier
 from sklearn.linear_model import LogisticRegression
@@ -199,15 +198,15 @@
 ```
 
 [![fig0](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/tunning_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/tunning_scatter.png)
 
 ## Cross-validtion
 
 ```python
-models: Dict[BaseEstimator, Dict] = {
+models: dict[BaseEstimator, dict] = {
     RandomForestClassifier: {
         'n_estimators': [10, 50, 100, 200],
         'max_depth': [None, 5, 10, 15],
         'min_samples_split': [2, 5, 10],
         'min_samples_leaf': [1, 2, 4],
         'random_state': [random_state]
     },
@@ -506,15 +505,15 @@
 
 [![fig1](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/classification_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/classification_scatter.png)
 
 
 ## Cross-validation
 
 ```python
-models: Dict[BaseEstimator, Dict] = {
+models: dict[BaseEstimator, dict] = {
     RandomForestClassifier: {
         'n_estimators': [10, 50, 100, 200],
         'max_depth': [None, 5, 10, 15],
         'min_samples_split': [2, 5, 10],
         'min_samples_leaf': [1, 2, 4],
         'random_state': [random_state]
     },
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mlpr Version: 0.1.7 Summary: A library for machine
+Metadata-Version: 2.1 Name: mlpr Version: 0.1.8 Summary: A library for machine
 learning pipeline and creation of reports. Author: Manuel Ferreira Junior
 Author-email: ferreira.jr.ufpb@gmail.com Maintainer: Manuel Ferreira Junior
 Maintainer-email: ferreira.jr.ufpb@gmail.com Requires-Python: >=3.9 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: MacOS Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: Unix
@@ -45,22 +45,22 @@
 their needs. # Using the MLPR Library The MLPR library is a powerful tool for
 machine learning and data analysis. Here's a brief guide on how to use it. ##
 Installation Before you start, make sure you have installed the MLPR library.
 You can do this by running pip install mlpr. ```bash pip install mlpr ``` #
 Tunning Click [here](https://github.com/Manuelfjr/mlpr/tree/develop/notebooks/
 supervisioned/tunning/) for contents. MLPR for model selection. ## Importing
 the Library First, import the necessary modules from the library: ```python
-from typing import Dict import numpy as np import pandas as pd import
-matplotlib.pyplot as plt from sklearn.base import BaseEstimator from
-sklearn.ensemble import RandomForestClassifier, GradientBoostingClassifier from
-sklearn.linear_model import LogisticRegression from sklearn.naive_bayes import
-GaussianNB from sklearn.neighbors import KNeighborsClassifier from sklearn.svm
-import SVC from sklearn.tree import DecisionTreeClassifier from
-sklearn.datasets import make_blobs from sklearn.metrics import accuracy_score,
-precision_score, recall_score, f1_score, cohen_kappa_score from
+import numpy as np import pandas as pd import matplotlib.pyplot as plt from
+sklearn.base import BaseEstimator from sklearn.ensemble import
+RandomForestClassifier, GradientBoostingClassifier from sklearn.linear_model
+import LogisticRegression from sklearn.naive_bayes import GaussianNB from
+sklearn.neighbors import KNeighborsClassifier from sklearn.svm import SVC from
+sklearn.tree import DecisionTreeClassifier from sklearn.datasets import
+make_blobs from sklearn.metrics import accuracy_score, precision_score,
+recall_score, f1_score, cohen_kappa_score from
 mlpr.ml.supervisioned.tunning.grid_search import GridSearch ``` ## Methods Here
 we have a custom method for accuracy to use in model selection. Thus: ```python
 def custom_accuracy_score(y_true: np.ndarray, y_pred: np.ndarray) -> float:
 return accuracy_score(y_true, y_pred, normalize=False) ``` ## Loading the Data
 Load your dataset. In this example, we're generating a dataset for
 classification using sklearn: ```python n_samples = 1000 centers = [(0, 0), (3,
 4.5)] n_features = 2 cluster_std = 1.3 random_state = 42 ``` ```python
@@ -68,16 +68,16 @@
 ( n_samples=n_samples, centers=centers, n_features=n_features,
 cluster_std=cluster_std, random_state=random_state ) ``` ## Plot the dataset
 ```python fig, ax = plt.subplots(1, 1, figsize=(14, 6)) ax.plot(X[:, 0][y ==
 0], X[:, 1][y == 0], "bs") ax.plot(X[:, 0][y == 1], X[:, 1][y == 1], "g^")
 ax.set_title("Dataset") ax.set_frame_on(False) ax.set_xticks([]) ax.set_yticks(
 []) fig.tight_layout() ``` [![fig0](https://raw.githack.com/Manuelfjr/mlpr/
 develop/assets/tunning_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/
-develop/assets/tunning_scatter.png) ## Cross-validtion ```python models: Dict
-[BaseEstimator, Dict] = { RandomForestClassifier: { 'n_estimators': [10, 50,
+develop/assets/tunning_scatter.png) ## Cross-validtion ```python models: dict
+[BaseEstimator, dict] = { RandomForestClassifier: { 'n_estimators': [10, 50,
 100, 200], 'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5, 10],
 'min_samples_leaf': [1, 2, 4], 'random_state': [random_state] },
 GradientBoostingClassifier: { 'n_estimators': [50, 100, 200], 'learning_rate':
 [0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0], 'random_state':
 [random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0, 10.0], 'penalty':
 ['l1', 'l2'], 'solver': ['liblinear', 'saga'], 'random_state': [random_state]
 }, GaussianNB: { 'var_smoothing': [1e-9, 1e-8, 1e-7, 1e-6, 1e-5] },
@@ -150,15 +150,15 @@
 [y == k], marker=markers[i % len(markers)], color=colors[i], label=f"c{i}")
 ax.set_title("Dataset") ax.set_frame_on(False) ax.set_xticks([]) ax.set_yticks(
 []) for center, color in zip(centers, colors): ax.scatter( center[0], center
 [1], color="white", linewidths=3, marker="o", edgecolor="black", s=120 )
 plt.legend() fig.tight_layout() ``` [![fig1](https://raw.githack.com/Manuelfjr/
 mlpr/develop/assets/classification_scatter.png)](https://raw.githack.com/
 Manuelfjr/mlpr/develop/assets/classification_scatter.png) ## Cross-validation
-```python models: Dict[BaseEstimator, Dict] = { RandomForestClassifier:
+```python models: dict[BaseEstimator, dict] = { RandomForestClassifier:
 { 'n_estimators': [10, 50, 100, 200], 'max_depth': [None, 5, 10, 15],
 'min_samples_split': [2, 5, 10], 'min_samples_leaf': [1, 2, 4], 'random_state':
 [random_state] }, GradientBoostingClassifier: { 'n_estimators': [50, 100, 200],
 'learning_rate': [0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0],
 'random_state': [random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0,
 10.0], 'penalty': ['l1', 'l2'], 'solver': ['liblinear', 'saga'],
 'random_state': [random_state], 'max_iter': [10000] }, GaussianNB:
```

