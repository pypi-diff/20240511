# Comparing `tmp/mlpr-0.1.6.tar.gz` & `tmp/mlpr-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpr-0.1.6.tar", max compression
+gzip compressed data, was "mlpr-0.1.7.tar", max compression
```

## Comparing `mlpr-0.1.6.tar` & `mlpr-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0      289 2024-05-11 02:18:39.159292 mlpr-0.1.6/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2024-04-27 16:49:57.314542 mlpr-0.1.6/LICENSE
--rw-r--r--   0        0        0    30224 2024-05-11 11:17:49.752969 mlpr-0.1.6/README.md
--rw-r--r--   0        0        0      256 2024-05-11 02:24:23.791737 mlpr-0.1.6/SECURITY.md
--rw-r--r--   0        0        0     2502 2024-05-11 11:18:25.373302 mlpr-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       70 2024-05-11 11:18:28.441331 mlpr-0.1.6/src/mlpr/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.6/src/mlpr/ml/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 18:27:54.717513 mlpr-0.1.6/src/mlpr/ml/supervisioned/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 18:28:38.701333 mlpr-0.1.6/src/mlpr/ml/supervisioned/classification/__init__.py
--rw-r--r--   0        0        0     5103 2024-05-11 02:06:39.037536 mlpr-0.1.6/src/mlpr/ml/supervisioned/classification/uncertainty.py
--rw-r--r--   0        0        0     2242 2024-05-11 01:58:21.065745 mlpr-0.1.6/src/mlpr/ml/supervisioned/classification/utils.py
--rw-r--r--   0        0        0        0 2024-04-27 18:28:52.537279 mlpr-0.1.6/src/mlpr/ml/supervisioned/forecasting/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 23:35:52.450714 mlpr-0.1.6/src/mlpr/ml/supervisioned/regression/__init__.py
--rw-r--r--   0        0        0    18436 2024-05-05 00:35:48.981115 mlpr-0.1.6/src/mlpr/ml/supervisioned/regression/metrics.py
--rw-r--r--   0        0        0    18464 2024-05-05 00:20:45.686332 mlpr-0.1.6/src/mlpr/ml/supervisioned/regression/plots.py
--rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.6/src/mlpr/ml/supervisioned/tunning/__init__.py
--rw-r--r--   0        0        0     6314 2024-05-10 23:01:04.220209 mlpr-0.1.6/src/mlpr/ml/supervisioned/tunning/grid_search.py
--rw-r--r--   0        0        0       62 2024-04-27 21:43:09.387068 mlpr-0.1.6/src/mlpr/reports/__init__.py
--rw-r--r--   0        0        0     1742 2024-05-04 23:35:34.703861 mlpr-0.1.6/src/mlpr/reports/create.py
--rw-r--r--   0        0        0    32185 1970-01-01 00:00:00.000000 mlpr-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      289 2024-05-11 02:18:39.159292 mlpr-0.1.7/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2024-04-27 16:49:57.314542 mlpr-0.1.7/LICENSE
+-rw-r--r--   0        0        0    30224 2024-05-11 11:17:49.752969 mlpr-0.1.7/README.md
+-rw-r--r--   0        0        0      256 2024-05-11 02:24:23.791737 mlpr-0.1.7/SECURITY.md
+-rw-r--r--   0        0        0     2502 2024-05-11 16:01:24.031457 mlpr-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-05-11 16:01:21.023407 mlpr-0.1.7/src/mlpr/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.7/src/mlpr/ml/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:27:54.717513 mlpr-0.1.7/src/mlpr/ml/supervisioned/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:28:38.701333 mlpr-0.1.7/src/mlpr/ml/supervisioned/classification/__init__.py
+-rw-r--r--   0        0        0    12544 2024-05-11 15:17:49.862210 mlpr-0.1.7/src/mlpr/ml/supervisioned/classification/metrics.py
+-rw-r--r--   0        0        0     5103 2024-05-11 02:06:39.037536 mlpr-0.1.7/src/mlpr/ml/supervisioned/classification/uncertainty.py
+-rw-r--r--   0        0        0     2242 2024-05-11 01:58:21.065745 mlpr-0.1.7/src/mlpr/ml/supervisioned/classification/utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:28:52.537279 mlpr-0.1.7/src/mlpr/ml/supervisioned/forecasting/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 23:35:52.450714 mlpr-0.1.7/src/mlpr/ml/supervisioned/regression/__init__.py
+-rw-r--r--   0        0        0    18436 2024-05-05 00:35:48.981115 mlpr-0.1.7/src/mlpr/ml/supervisioned/regression/metrics.py
+-rw-r--r--   0        0        0    18464 2024-05-05 00:20:45.686332 mlpr-0.1.7/src/mlpr/ml/supervisioned/regression/plots.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.7/src/mlpr/ml/supervisioned/tunning/__init__.py
+-rw-r--r--   0        0        0     6314 2024-05-10 23:01:04.220209 mlpr-0.1.7/src/mlpr/ml/supervisioned/tunning/grid_search.py
+-rw-r--r--   0        0        0       62 2024-04-27 21:43:09.387068 mlpr-0.1.7/src/mlpr/reports/__init__.py
+-rw-r--r--   0        0        0     1742 2024-05-04 23:35:34.703861 mlpr-0.1.7/src/mlpr/reports/create.py
+-rw-r--r--   0        0        0    32185 1970-01-01 00:00:00.000000 mlpr-0.1.7/PKG-INFO
```

### Comparing `mlpr-0.1.6/LICENSE` & `mlpr-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.6/README.md` & `mlpr-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.6/pyproject.toml` & `mlpr-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlpr"
-version = "0.1.6"
+version = "0.1.7"
 authors = ["Manuel Ferreira Junior <ferreira.jr.ufpb@gmail.com>"]
 description = "A library for machine learning pipeline and creation of reports."
 readme = "README.md"
 maintainers = [
     "Manuel Ferreira Junior <ferreira.jr.ufpb@gmail.com>"
 ]
 classifiers=[
```

### Comparing `mlpr-0.1.6/src/mlpr/ml/supervisioned/classification/uncertainty.py` & `mlpr-0.1.7/src/mlpr/ml/supervisioned/classification/uncertainty.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.6/src/mlpr/ml/supervisioned/classification/utils.py` & `mlpr-0.1.7/src/mlpr/ml/supervisioned/classification/utils.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.6/src/mlpr/ml/supervisioned/regression/metrics.py` & `mlpr-0.1.7/src/mlpr/ml/supervisioned/regression/metrics.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.6/src/mlpr/ml/supervisioned/regression/plots.py` & `mlpr-0.1.7/src/mlpr/ml/supervisioned/regression/plots.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.6/src/mlpr/ml/supervisioned/tunning/grid_search.py` & `mlpr-0.1.7/src/mlpr/ml/supervisioned/tunning/grid_search.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.6/src/mlpr/reports/create.py` & `mlpr-0.1.7/src/mlpr/reports/create.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.6/PKG-INFO` & `mlpr-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpr
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library for machine learning pipeline and creation of reports.
 Author: Manuel Ferreira Junior
 Author-email: ferreira.jr.ufpb@gmail.com
 Maintainer: Manuel Ferreira Junior
 Maintainer-email: ferreira.jr.ufpb@gmail.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mlpr Version: 0.1.6 Summary: A library for machine
+Metadata-Version: 2.1 Name: mlpr Version: 0.1.7 Summary: A library for machine
 learning pipeline and creation of reports. Author: Manuel Ferreira Junior
 Author-email: ferreira.jr.ufpb@gmail.com Maintainer: Manuel Ferreira Junior
 Maintainer-email: ferreira.jr.ufpb@gmail.com Requires-Python: >=3.9 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: MacOS Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: Unix
```

