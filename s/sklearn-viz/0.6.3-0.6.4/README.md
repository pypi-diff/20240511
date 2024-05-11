# Comparing `tmp/sklearn_viz-0.6.3.tar.gz` & `tmp/sklearn_viz-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_viz-0.6.3.tar", max compression
+gzip compressed data, was "sklearn_viz-0.6.4.tar", max compression
```

## Comparing `sklearn_viz-0.6.3.tar` & `sklearn_viz-0.6.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/LICENSE
--rw-r--r--   0        0        0      354 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/README.md
--rw-r--r--   0        0        0      165 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/__init__.py
--rw-r--r--   0        0        0        0 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/components/__init__.py
--rw-r--r--   0        0        0     5912 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/components/estimators.py
--rw-r--r--   0        0        0      811 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/components/kfold.py
--rw-r--r--   0        0        0      329 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/features/__init__.py
--rw-r--r--   0        0        0     8306 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/features/importance.py
--rw-r--r--   0        0        0     4633 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/features/outlier_detection.py
--rw-r--r--   0        0        0     2403 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/features/parallel_coordinates.py
--rw-r--r--   0        0        0    16590 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/features/principal_components.py
--rw-r--r--   0        0        0      643 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/features/scatter_matrix.py
--rw-r--r--   0        0        0      129 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/model_selection/__init__.py
--rw-r--r--   0        0        0    12455 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/model_selection/cross_validation.py
--rw-r--r--   0        0        0     6079 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/model_selection/learning_curve.py
--rw-r--r--   0        0        0     1572 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/model_selection/metrics.py
--rw-r--r--   0        0        0    13742 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/model_selection/model_selection.py
--rw-r--r--   0        0        0     2497 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/model_selection/models.py
--rw-r--r--   0        0        0      508 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/model_selection/scorers.py
--rw-r--r--   0        0        0       21 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/residuals/__init__.py
--rw-r--r--   0        0        0     2058 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/residuals/error.py
--rw-r--r--   0        0        0       28 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/utils/__init__.py
--rw-r--r--   0        0        0      544 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/utils/file.py
--rw-r--r--   0        0        0     3033 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/utils/plotly.py
--rw-r--r--   0        0        0     3111 2024-05-11 03:59:23.508666 sklearn_viz-0.6.3/elphick/sklearn_viz/utils/timer.py
--rw-r--r--   0        0        0      977 2024-05-11 03:59:23.512667 sklearn_viz-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 sklearn_viz-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-11 06:16:51.563821 sklearn_viz-0.6.4/LICENSE
+-rw-r--r--   0        0        0      354 2024-05-11 06:16:51.563821 sklearn_viz-0.6.4/README.md
+-rw-r--r--   0        0        0      165 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/components/__init__.py
+-rw-r--r--   0        0        0     5912 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/components/estimators.py
+-rw-r--r--   0        0        0      811 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/components/kfold.py
+-rw-r--r--   0        0        0      329 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/features/__init__.py
+-rw-r--r--   0        0        0     8306 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/features/importance.py
+-rw-r--r--   0        0        0     4633 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/features/outlier_detection.py
+-rw-r--r--   0        0        0     2403 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/features/parallel_coordinates.py
+-rw-r--r--   0        0        0    16590 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/features/principal_components.py
+-rw-r--r--   0        0        0      643 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/features/scatter_matrix.py
+-rw-r--r--   0        0        0      129 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/__init__.py
+-rw-r--r--   0        0        0    12455 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/cross_validation.py
+-rw-r--r--   0        0        0     6079 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/learning_curve.py
+-rw-r--r--   0        0        0     1572 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/metrics.py
+-rw-r--r--   0        0        0    13742 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/model_selection.py
+-rw-r--r--   0        0        0     2497 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/models.py
+-rw-r--r--   0        0        0      508 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/scorers.py
+-rw-r--r--   0        0        0       21 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/residuals/__init__.py
+-rw-r--r--   0        0        0     4377 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/residuals/error.py
+-rw-r--r--   0        0        0       28 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/utils/__init__.py
+-rw-r--r--   0        0        0      544 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/utils/file.py
+-rw-r--r--   0        0        0     3033 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/utils/plotly.py
+-rw-r--r--   0        0        0     3111 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/utils/timer.py
+-rw-r--r--   0        0        0      977 2024-05-11 06:16:51.571821 sklearn_viz-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 sklearn_viz-0.6.4/PKG-INFO
```

### Comparing `sklearn_viz-0.6.3/LICENSE` & `sklearn_viz-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/components/estimators.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/components/estimators.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/components/kfold.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/components/kfold.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/features/importance.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/features/importance.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/features/outlier_detection.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/features/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/features/parallel_coordinates.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/features/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/features/principal_components.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/features/principal_components.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/features/scatter_matrix.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/features/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/model_selection/cross_validation.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/cross_validation.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/model_selection/learning_curve.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/learning_curve.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/model_selection/metrics.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/metrics.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/model_selection/model_selection.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/model_selection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/model_selection/models.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/models.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/utils/file.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/utils/file.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/utils/plotly.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/utils/plotly.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/elphick/sklearn_viz/utils/timer.py` & `sklearn_viz-0.6.4/elphick/sklearn_viz/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.3/pyproject.toml` & `sklearn_viz-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sklearn-viz"
-version = "0.6.3"
+version = "0.6.4"
 description = ""
 authors = ["Greg <11791585+elphick@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "elphick/sklearn_viz" }]
 
 [[tool.poetry.source]]
 name = "PyPI"
```

### Comparing `sklearn_viz-0.6.3/PKG-INFO` & `sklearn_viz-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-viz
-Version: 0.6.3
+Version: 0.6.4
 Summary: 
 Author: Greg
 Author-email: 11791585+elphick@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

