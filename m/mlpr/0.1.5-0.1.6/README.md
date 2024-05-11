# Comparing `tmp/mlpr-0.1.5.tar.gz` & `tmp/mlpr-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpr-0.1.5.tar", max compression
+gzip compressed data, was "mlpr-0.1.6.tar", max compression
```

## Comparing `mlpr-0.1.5.tar` & `mlpr-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      289 2024-05-11 02:18:39.159292 mlpr-0.1.5/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2024-04-27 16:49:57.314542 mlpr-0.1.5/LICENSE
--rw-r--r--   0        0        0    30231 2024-05-11 03:50:25.744186 mlpr-0.1.5/README.md
--rw-r--r--   0        0        0      256 2024-05-11 02:24:23.791737 mlpr-0.1.5/SECURITY.md
--rw-r--r--   0        0        0     2502 2024-05-11 03:50:45.279950 mlpr-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       70 2024-05-11 03:50:41.867990 mlpr-0.1.5/src/mlpr/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.5/src/mlpr/ml/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 18:27:54.717513 mlpr-0.1.5/src/mlpr/ml/supervisioned/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 18:28:38.701333 mlpr-0.1.5/src/mlpr/ml/supervisioned/classification/__init__.py
--rw-r--r--   0        0        0     5103 2024-05-11 02:06:39.037536 mlpr-0.1.5/src/mlpr/ml/supervisioned/classification/uncertainty.py
--rw-r--r--   0        0        0     2242 2024-05-11 01:58:21.065745 mlpr-0.1.5/src/mlpr/ml/supervisioned/classification/utils.py
--rw-r--r--   0        0        0        0 2024-04-27 18:28:52.537279 mlpr-0.1.5/src/mlpr/ml/supervisioned/forecasting/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 23:35:52.450714 mlpr-0.1.5/src/mlpr/ml/supervisioned/regression/__init__.py
--rw-r--r--   0        0        0    18436 2024-05-05 00:35:48.981115 mlpr-0.1.5/src/mlpr/ml/supervisioned/regression/metrics.py
--rw-r--r--   0        0        0    18464 2024-05-05 00:20:45.686332 mlpr-0.1.5/src/mlpr/ml/supervisioned/regression/plots.py
--rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.5/src/mlpr/ml/supervisioned/tunning/__init__.py
--rw-r--r--   0        0        0     6314 2024-05-10 23:01:04.220209 mlpr-0.1.5/src/mlpr/ml/supervisioned/tunning/grid_search.py
--rw-r--r--   0        0        0       62 2024-04-27 21:43:09.387068 mlpr-0.1.5/src/mlpr/reports/__init__.py
--rw-r--r--   0        0        0     1742 2024-05-04 23:35:34.703861 mlpr-0.1.5/src/mlpr/reports/create.py
--rw-r--r--   0        0        0    32192 1970-01-01 00:00:00.000000 mlpr-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      289 2024-05-11 02:18:39.159292 mlpr-0.1.6/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2024-04-27 16:49:57.314542 mlpr-0.1.6/LICENSE
+-rw-r--r--   0        0        0    30224 2024-05-11 11:17:49.752969 mlpr-0.1.6/README.md
+-rw-r--r--   0        0        0      256 2024-05-11 02:24:23.791737 mlpr-0.1.6/SECURITY.md
+-rw-r--r--   0        0        0     2502 2024-05-11 11:18:25.373302 mlpr-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-05-11 11:18:28.441331 mlpr-0.1.6/src/mlpr/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.6/src/mlpr/ml/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:27:54.717513 mlpr-0.1.6/src/mlpr/ml/supervisioned/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:28:38.701333 mlpr-0.1.6/src/mlpr/ml/supervisioned/classification/__init__.py
+-rw-r--r--   0        0        0     5103 2024-05-11 02:06:39.037536 mlpr-0.1.6/src/mlpr/ml/supervisioned/classification/uncertainty.py
+-rw-r--r--   0        0        0     2242 2024-05-11 01:58:21.065745 mlpr-0.1.6/src/mlpr/ml/supervisioned/classification/utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:28:52.537279 mlpr-0.1.6/src/mlpr/ml/supervisioned/forecasting/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 23:35:52.450714 mlpr-0.1.6/src/mlpr/ml/supervisioned/regression/__init__.py
+-rw-r--r--   0        0        0    18436 2024-05-05 00:35:48.981115 mlpr-0.1.6/src/mlpr/ml/supervisioned/regression/metrics.py
+-rw-r--r--   0        0        0    18464 2024-05-05 00:20:45.686332 mlpr-0.1.6/src/mlpr/ml/supervisioned/regression/plots.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.6/src/mlpr/ml/supervisioned/tunning/__init__.py
+-rw-r--r--   0        0        0     6314 2024-05-10 23:01:04.220209 mlpr-0.1.6/src/mlpr/ml/supervisioned/tunning/grid_search.py
+-rw-r--r--   0        0        0       62 2024-04-27 21:43:09.387068 mlpr-0.1.6/src/mlpr/reports/__init__.py
+-rw-r--r--   0        0        0     1742 2024-05-04 23:35:34.703861 mlpr-0.1.6/src/mlpr/reports/create.py
+-rw-r--r--   0        0        0    32185 1970-01-01 00:00:00.000000 mlpr-0.1.6/PKG-INFO
```

### Comparing `mlpr-0.1.5/LICENSE` & `mlpr-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.5/README.md` & `mlpr-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
       <a href="https://pypi.org/project/mlpr/"><img src="https://img.shields.io/pypi/dd/mlpr?style=flat-square&color=darkgreen" alt="PyPI - Downloads"></a>
     </td>
     <td>
       <a href="https://github.com/Manuelfjr/mlpr/commits"><img src="https://img.shields.io/github/last-commit/Manuelfjr/mlpr" alt="Last Commit"></a>
       <a href="https://github.com/Manuelfjr/mlpr/issues"><img src="https://img.shields.io/github/issues-raw/Manuelfjr/mlpr" alt="Open Issues"></a>
       <a href="https://github.com/Manuelfjr/mlpr/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed-raw/Manuelfjr/mlpr" alt="Closed Issues"></a>
       <a href="https://github.com/Manuelfjr/mlpr/graphs/contributors"><img src="https://img.shields.io/github/contributors/Manuelfjr/mlpr" alt="Contributors"></a>
-      <a href="https://github.com/Manuelfjr/birt-gd"><img src="https://img.shields.io/badge/docs-birtgd-blue?&logo" alt="Docs"></a>
+      <a href="https://github.com/Manuelfjr/mlpr"><img src="https://img.shields.io/badge/docs-mlpr-blue?&logo" alt="Docs"></a>
     </td>
     <td>
       <a href="https://github.com/Manuelfjr"><img src="https://img.shields.io/badge/author-manuelfjr-blue?&logo=github" alt="Author"></a>
       <a href="https://github.com/Manuelfjr/mlpr/issues?q=is%3Aopen+is%3Aissue"><img src="https://badgen.net/github/open-issues/manuelfjr/mlpr" alt="Open Issues"></a>
       <a href="https://github.com/Manuelfjr/mlpr/issues?q=is%3Aissue+is%3Aclosed"><img src="https://badgen.net/github/closed-issues/manuelfjr/mlpr" alt="Closed Issues"></a>
     </td>
   </tr>
@@ -47,15 +47,15 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/mlpr?style=flat-square&color=darkgreen)](https://pypi.org/project/mlpr/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dd/mlpr?style=flat-square&color=darkgreen)](https://pypi.org/project/mlpr/)
 
 [![Last Commit](https://img.shields.io/github/last-commit/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/commits)
 [![Open Issues](https://img.shields.io/github/issues-raw/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues)
 [![Closed Issues](https://img.shields.io/github/issues-closed-raw/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues?q=is%3Aissue+is%3Aclosed)
 [![Contributors](https://img.shields.io/github/contributors/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/graphs/contributors)
-[![Docs](https://img.shields.io/badge/docs-birtgd-blue?&logo)](https://github.com/Manuelfjr/birt-gd)
+[![Docs](https://img.shields.io/badge/docs-mlpr-blue?&logo)](https://github.com/Manuelfjr/birt-gd)
 
 [![Author](https://img.shields.io/badge/author-manuelfjr-blue?&logo=github)](https://github.com/Manuelfjr)
 [![https://badgen.net/github/open-issues/manuelfjr/mlpr](https://badgen.net/github/open-issues/manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues?q=is%3Aopen+is%3Aissue)
 [![https://badgen.net/github/closed-issues/manuelfjr/mlpr](https://badgen.net/github/closed-issues/manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues?q=is%3Aissue+is%3Aclosed) -->
 
 
 [![fig0](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/regression_plots.png)](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/regression_plots.png)
```

### Comparing `mlpr-0.1.5/pyproject.toml` & `mlpr-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlpr"
-version = "0.1.5"
+version = "0.1.6"
 authors = ["Manuel Ferreira Junior <ferreira.jr.ufpb@gmail.com>"]
 description = "A library for machine learning pipeline and creation of reports."
 readme = "README.md"
 maintainers = [
     "Manuel Ferreira Junior <ferreira.jr.ufpb@gmail.com>"
 ]
 classifiers=[
```

### Comparing `mlpr-0.1.5/src/mlpr/ml/supervisioned/classification/uncertainty.py` & `mlpr-0.1.6/src/mlpr/ml/supervisioned/classification/uncertainty.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.5/src/mlpr/ml/supervisioned/classification/utils.py` & `mlpr-0.1.6/src/mlpr/ml/supervisioned/classification/utils.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.5/src/mlpr/ml/supervisioned/regression/metrics.py` & `mlpr-0.1.6/src/mlpr/ml/supervisioned/regression/metrics.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.5/src/mlpr/ml/supervisioned/regression/plots.py` & `mlpr-0.1.6/src/mlpr/ml/supervisioned/regression/plots.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.5/src/mlpr/ml/supervisioned/tunning/grid_search.py` & `mlpr-0.1.6/src/mlpr/ml/supervisioned/tunning/grid_search.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.5/src/mlpr/reports/create.py` & `mlpr-0.1.6/src/mlpr/reports/create.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.5/PKG-INFO` & `mlpr-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpr
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library for machine learning pipeline and creation of reports.
 Author: Manuel Ferreira Junior
 Author-email: ferreira.jr.ufpb@gmail.com
 Maintainer: Manuel Ferreira Junior
 Maintainer-email: ferreira.jr.ufpb@gmail.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
@@ -66,15 +66,15 @@
       <a href="https://pypi.org/project/mlpr/"><img src="https://img.shields.io/pypi/dd/mlpr?style=flat-square&color=darkgreen" alt="PyPI - Downloads"></a>
     </td>
     <td>
       <a href="https://github.com/Manuelfjr/mlpr/commits"><img src="https://img.shields.io/github/last-commit/Manuelfjr/mlpr" alt="Last Commit"></a>
       <a href="https://github.com/Manuelfjr/mlpr/issues"><img src="https://img.shields.io/github/issues-raw/Manuelfjr/mlpr" alt="Open Issues"></a>
       <a href="https://github.com/Manuelfjr/mlpr/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed-raw/Manuelfjr/mlpr" alt="Closed Issues"></a>
       <a href="https://github.com/Manuelfjr/mlpr/graphs/contributors"><img src="https://img.shields.io/github/contributors/Manuelfjr/mlpr" alt="Contributors"></a>
-      <a href="https://github.com/Manuelfjr/birt-gd"><img src="https://img.shields.io/badge/docs-birtgd-blue?&logo" alt="Docs"></a>
+      <a href="https://github.com/Manuelfjr/mlpr"><img src="https://img.shields.io/badge/docs-mlpr-blue?&logo" alt="Docs"></a>
     </td>
     <td>
       <a href="https://github.com/Manuelfjr"><img src="https://img.shields.io/badge/author-manuelfjr-blue?&logo=github" alt="Author"></a>
       <a href="https://github.com/Manuelfjr/mlpr/issues?q=is%3Aopen+is%3Aissue"><img src="https://badgen.net/github/open-issues/manuelfjr/mlpr" alt="Open Issues"></a>
       <a href="https://github.com/Manuelfjr/mlpr/issues?q=is%3Aissue+is%3Aclosed"><img src="https://badgen.net/github/closed-issues/manuelfjr/mlpr" alt="Closed Issues"></a>
     </td>
   </tr>
@@ -90,15 +90,15 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/mlpr?style=flat-square&color=darkgreen)](https://pypi.org/project/mlpr/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dd/mlpr?style=flat-square&color=darkgreen)](https://pypi.org/project/mlpr/)
 
 [![Last Commit](https://img.shields.io/github/last-commit/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/commits)
 [![Open Issues](https://img.shields.io/github/issues-raw/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues)
 [![Closed Issues](https://img.shields.io/github/issues-closed-raw/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues?q=is%3Aissue+is%3Aclosed)
 [![Contributors](https://img.shields.io/github/contributors/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/graphs/contributors)
-[![Docs](https://img.shields.io/badge/docs-birtgd-blue?&logo)](https://github.com/Manuelfjr/birt-gd)
+[![Docs](https://img.shields.io/badge/docs-mlpr-blue?&logo)](https://github.com/Manuelfjr/birt-gd)
 
 [![Author](https://img.shields.io/badge/author-manuelfjr-blue?&logo=github)](https://github.com/Manuelfjr)
 [![https://badgen.net/github/open-issues/manuelfjr/mlpr](https://badgen.net/github/open-issues/manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues?q=is%3Aopen+is%3Aissue)
 [![https://badgen.net/github/closed-issues/manuelfjr/mlpr](https://badgen.net/github/closed-issues/manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues?q=is%3Aissue+is%3Aclosed) -->
 
 
 [![fig0](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/regression_plots.png)](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/regression_plots.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mlpr Version: 0.1.5 Summary: A library for machine
+Metadata-Version: 2.1 Name: mlpr Version: 0.1.6 Summary: A library for machine
 learning pipeline and creation of reports. Author: Manuel Ferreira Junior
 Author-email: ferreira.jr.ufpb@gmail.com Maintainer: Manuel Ferreira Junior
 Maintainer-email: ferreira.jr.ufpb@gmail.com Requires-Python: >=3.9 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: MacOS Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: Unix
```

