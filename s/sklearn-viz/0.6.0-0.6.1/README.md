# Comparing `tmp/sklearn_viz-0.6.0.tar.gz` & `tmp/sklearn_viz-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_viz-0.6.0.tar", max compression
+gzip compressed data, was "sklearn_viz-0.6.1.tar", max compression
```

## Comparing `sklearn_viz-0.6.0.tar` & `sklearn_viz-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2024-05-10 13:31:23.533871 sklearn_viz-0.6.0/LICENSE
--rw-r--r--   0        0        0      354 2024-05-10 13:31:23.533871 sklearn_viz-0.6.0/README.md
--rw-r--r--   0        0        0      165 2024-05-10 13:31:23.533871 sklearn_viz-0.6.0/elphick/sklearn_viz/__init__.py
--rw-r--r--   0        0        0        0 2024-05-10 13:31:23.533871 sklearn_viz-0.6.0/elphick/sklearn_viz/components/__init__.py
--rw-r--r--   0        0        0     5912 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/components/estimators.py
--rw-r--r--   0        0        0      811 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/components/kfold.py
--rw-r--r--   0        0        0      329 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/features/__init__.py
--rw-r--r--   0        0        0     8306 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/features/importance.py
--rw-r--r--   0        0        0     4633 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/features/outlier_detection.py
--rw-r--r--   0        0        0     2403 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/features/parallel_coordinates.py
--rw-r--r--   0        0        0    16590 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/features/principal_components.py
--rw-r--r--   0        0        0      643 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/features/scatter_matrix.py
--rw-r--r--   0        0        0      129 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/__init__.py
--rw-r--r--   0        0        0    11404 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/cross_validation.py
--rw-r--r--   0        0        0     6079 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/learning_curve.py
--rw-r--r--   0        0        0     1572 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/metrics.py
--rw-r--r--   0        0        0    13278 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/model_selection.py
--rw-r--r--   0        0        0     2497 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/models.py
--rw-r--r--   0        0        0      508 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/scorers.py
--rw-r--r--   0        0        0       21 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/residuals/__init__.py
--rw-r--r--   0        0        0     2058 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/residuals/error.py
--rw-r--r--   0        0        0       28 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/utils/__init__.py
--rw-r--r--   0        0        0      544 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/utils/file.py
--rw-r--r--   0        0        0     3033 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/utils/plotly.py
--rw-r--r--   0        0        0     3111 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/elphick/sklearn_viz/utils/timer.py
--rw-r--r--   0        0        0      977 2024-05-10 13:31:23.537871 sklearn_viz-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 sklearn_viz-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/LICENSE
+-rw-r--r--   0        0        0      354 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/README.md
+-rw-r--r--   0        0        0      165 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/components/__init__.py
+-rw-r--r--   0        0        0     5912 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/components/estimators.py
+-rw-r--r--   0        0        0      811 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/components/kfold.py
+-rw-r--r--   0        0        0      329 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/features/__init__.py
+-rw-r--r--   0        0        0     8306 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/features/importance.py
+-rw-r--r--   0        0        0     4633 2024-05-10 21:38:53.296376 sklearn_viz-0.6.1/elphick/sklearn_viz/features/outlier_detection.py
+-rw-r--r--   0        0        0     2403 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/features/parallel_coordinates.py
+-rw-r--r--   0        0        0    16590 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/features/principal_components.py
+-rw-r--r--   0        0        0      643 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/features/scatter_matrix.py
+-rw-r--r--   0        0        0      129 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/__init__.py
+-rw-r--r--   0        0        0    11248 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/cross_validation.py
+-rw-r--r--   0        0        0     6079 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/learning_curve.py
+-rw-r--r--   0        0        0     1572 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/metrics.py
+-rw-r--r--   0        0        0    13278 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/model_selection.py
+-rw-r--r--   0        0        0     2497 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/models.py
+-rw-r--r--   0        0        0      508 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/scorers.py
+-rw-r--r--   0        0        0       21 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/residuals/__init__.py
+-rw-r--r--   0        0        0     2058 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/residuals/error.py
+-rw-r--r--   0        0        0       28 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/utils/__init__.py
+-rw-r--r--   0        0        0      544 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/utils/file.py
+-rw-r--r--   0        0        0     3033 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/utils/plotly.py
+-rw-r--r--   0        0        0     3111 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/elphick/sklearn_viz/utils/timer.py
+-rw-r--r--   0        0        0      977 2024-05-10 21:38:53.300376 sklearn_viz-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 sklearn_viz-0.6.1/PKG-INFO
```

### Comparing `sklearn_viz-0.6.0/LICENSE` & `sklearn_viz-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/components/estimators.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/components/estimators.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/components/kfold.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/components/kfold.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/features/importance.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/features/importance.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/features/outlier_detection.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/features/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/features/parallel_coordinates.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/features/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/features/principal_components.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/features/principal_components.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/features/scatter_matrix.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/features/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/cross_validation.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/cross_validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,17 +48,15 @@
         self.is_classifier = all(is_classifier(estimator) for estimator in estimators.values())
         self.is_regressor = all(is_regressor(estimator) for estimator in estimators.values())
 
         if not self.is_classifier and not self.is_regressor:
             raise ValueError("All estimators must be either classifiers or regressors.")
 
         if scorer is None:
-            default_scorer = 'accuracy' if self.is_classifier else 'r2'
-            scorer_dict = classification_scorers if self.is_classifier else regression_scorers
-            scorer = scorer_dict.get(default_scorer)
+            scorer = 'accuracy' if self.is_classifier else 'r2'
 
         if metrics is None:
             default_metrics = {
                 'classification': classification_metrics,
                 'regression': regression_metrics
             }
             metrics_type = 'classification' if self.is_classifier else 'regression'
```

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/learning_curve.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/learning_curve.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/metrics.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/metrics.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/model_selection.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/model_selection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/model_selection/models.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/model_selection/models.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/residuals/error.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/residuals/error.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/utils/file.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/utils/file.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/utils/plotly.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/utils/plotly.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/elphick/sklearn_viz/utils/timer.py` & `sklearn_viz-0.6.1/elphick/sklearn_viz/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.0/pyproject.toml` & `sklearn_viz-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sklearn-viz"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 authors = ["Greg <11791585+elphick@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "elphick/sklearn_viz" }]
 
 [[tool.poetry.source]]
 name = "PyPI"
```

### Comparing `sklearn_viz-0.6.0/PKG-INFO` & `sklearn_viz-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-viz
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 Author: Greg
 Author-email: 11791585+elphick@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

