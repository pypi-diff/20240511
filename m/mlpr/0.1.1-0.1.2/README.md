# Comparing `tmp/mlpr-0.1.1.tar.gz` & `tmp/mlpr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpr-0.1.1.tar", max compression
+gzip compressed data, was "mlpr-0.1.2.tar", max compression
```

## Comparing `mlpr-0.1.1.tar` & `mlpr-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      289 2024-05-11 02:18:39.159292 mlpr-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2024-04-27 16:49:57.314542 mlpr-0.1.1/LICENSE
--rw-r--r--   0        0        0    25844 2024-05-11 03:15:40.639069 mlpr-0.1.1/README.md
--rw-r--r--   0        0        0      256 2024-05-11 02:24:23.791737 mlpr-0.1.1/SECURITY.md
--rw-r--r--   0        0        0     2505 2024-05-11 03:16:02.959311 mlpr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       70 2024-05-11 03:15:55.495230 mlpr-0.1.1/src/mlpr/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.1/src/mlpr/ml/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 18:27:54.717513 mlpr-0.1.1/src/mlpr/ml/supervisioned/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 18:28:38.701333 mlpr-0.1.1/src/mlpr/ml/supervisioned/classification/__init__.py
--rw-r--r--   0        0        0     5103 2024-05-11 02:06:39.037536 mlpr-0.1.1/src/mlpr/ml/supervisioned/classification/uncertainty.py
--rw-r--r--   0        0        0     2242 2024-05-11 01:58:21.065745 mlpr-0.1.1/src/mlpr/ml/supervisioned/classification/utils.py
--rw-r--r--   0        0        0        0 2024-04-27 18:28:52.537279 mlpr-0.1.1/src/mlpr/ml/supervisioned/forecasting/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 23:35:52.450714 mlpr-0.1.1/src/mlpr/ml/supervisioned/regression/__init__.py
--rw-r--r--   0        0        0    18436 2024-05-05 00:35:48.981115 mlpr-0.1.1/src/mlpr/ml/supervisioned/regression/metrics.py
--rw-r--r--   0        0        0    18464 2024-05-05 00:20:45.686332 mlpr-0.1.1/src/mlpr/ml/supervisioned/regression/plots.py
--rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.1/src/mlpr/ml/supervisioned/tunning/__init__.py
--rw-r--r--   0        0        0     6314 2024-05-10 23:01:04.220209 mlpr-0.1.1/src/mlpr/ml/supervisioned/tunning/grid_search.py
--rw-r--r--   0        0        0       62 2024-04-27 21:43:09.387068 mlpr-0.1.1/src/mlpr/reports/__init__.py
--rw-r--r--   0        0        0     1742 2024-05-04 23:35:34.703861 mlpr-0.1.1/src/mlpr/reports/create.py
--rw-r--r--   0        0        0    27808 1970-01-01 00:00:00.000000 mlpr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      289 2024-05-11 02:18:39.159292 mlpr-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2024-04-27 16:49:57.314542 mlpr-0.1.2/LICENSE
+-rw-r--r--   0        0        0    27582 2024-05-11 03:28:46.346927 mlpr-0.1.2/README.md
+-rw-r--r--   0        0        0      256 2024-05-11 02:24:23.791737 mlpr-0.1.2/SECURITY.md
+-rw-r--r--   0        0        0     2502 2024-05-11 03:29:02.187076 mlpr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-05-11 03:29:08.883140 mlpr-0.1.2/src/mlpr/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.2/src/mlpr/ml/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:27:54.717513 mlpr-0.1.2/src/mlpr/ml/supervisioned/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:28:38.701333 mlpr-0.1.2/src/mlpr/ml/supervisioned/classification/__init__.py
+-rw-r--r--   0        0        0     5103 2024-05-11 02:06:39.037536 mlpr-0.1.2/src/mlpr/ml/supervisioned/classification/uncertainty.py
+-rw-r--r--   0        0        0     2242 2024-05-11 01:58:21.065745 mlpr-0.1.2/src/mlpr/ml/supervisioned/classification/utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:28:52.537279 mlpr-0.1.2/src/mlpr/ml/supervisioned/forecasting/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 23:35:52.450714 mlpr-0.1.2/src/mlpr/ml/supervisioned/regression/__init__.py
+-rw-r--r--   0        0        0    18436 2024-05-05 00:35:48.981115 mlpr-0.1.2/src/mlpr/ml/supervisioned/regression/metrics.py
+-rw-r--r--   0        0        0    18464 2024-05-05 00:20:45.686332 mlpr-0.1.2/src/mlpr/ml/supervisioned/regression/plots.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.2/src/mlpr/ml/supervisioned/tunning/__init__.py
+-rw-r--r--   0        0        0     6314 2024-05-10 23:01:04.220209 mlpr-0.1.2/src/mlpr/ml/supervisioned/tunning/grid_search.py
+-rw-r--r--   0        0        0       62 2024-04-27 21:43:09.387068 mlpr-0.1.2/src/mlpr/reports/__init__.py
+-rw-r--r--   0        0        0     1742 2024-05-04 23:35:34.703861 mlpr-0.1.2/src/mlpr/reports/create.py
+-rw-r--r--   0        0        0    29543 1970-01-01 00:00:00.000000 mlpr-0.1.2/PKG-INFO
```

### Comparing `mlpr-0.1.1/LICENSE` & `mlpr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.1/README.md` & `mlpr-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # MLPR Library
-[![TestPyPI version](https://img.shields.io/badge/dynamic/json?url=https://test.pypi.org/pypi/mlpr/json&label=TestPyPI%20version&query=$.info.version&color=blue)](https://test.pypi.org/project/mlpr/)
+
+[![PyPI version](https://img.shields.io/pypi/v/mlpr?color=blue)](https://pypi.org/project/mlpr/)
+[![License](https://img.shields.io/pypi/l/mlpr?color=blue)](https://pypi.org/project/mlpr/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mlpr)](https://pypi.org/project/mlpr/)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/mlpr)](https://pypi.org/project/mlpr/)
+[![PyPI - Status](https://img.shields.io/pypi/status/mlpr)](https://pypi.org/project/mlpr/)
+
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mlpr?style=flat-square&color=darkgreen)](https://pypi.org/project/mlpr/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dw/mlpr?style=flat-square&color=darkgreen)](https://pypi.org/project/mlpr/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dd/mlpr?style=flat-square&color=darkgreen)](https://pypi.org/project/mlpr/)
+
+[![Last Commit](https://img.shields.io/github/last-commit/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/commits)
+[![Open Issues](https://img.shields.io/github/issues-raw/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues)
+[![Closed Issues](https://img.shields.io/github/issues-closed-raw/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues?q=is%3Aissue+is%3Aclosed)
+[![Contributors](https://img.shields.io/github/contributors/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/graphs/contributors)
+[![Docs](https://img.shields.io/badge/docs-birtgd-blue?&logo)](https://github.com/Manuelfjr/birt-gd)
+
+[![Author](https://img.shields.io/badge/author-manuelfjr-blue?&logo=github)](https://github.com/Manuelfjr)
+[![https://badgen.net/github/open-issues/manuelfjr/mlpr](https://badgen.net/github/open-issues/manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues?q=is%3Aopen+is%3Aissue)
+[![https://badgen.net/github/closed-issues/manuelfjr/mlpr](https://badgen.net/github/closed-issues/manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues?q=is%3Aissue+is%3Aclosed)
 
 
 [![fig0](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/regression_plots.png)](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/regression_plots.png)
 
 This repository is a developing library named `MLPR` (Machine Learning Pipeline Report). It aims to facilitate the creation of machine learning models in various areas such as regression, forecasting, classification, and clustering. The library allows the user to perform tuning of these models, generate various types of plots for post-modeling analysis, and calculate various metrics.
 
 In addition, `MLPR` allows the creation of metric reports using [`Jinja2`](https://pypi.org/project/Jinja2/), including the obtained graphs. The user can customize the report template according to their needs.
```

### Comparing `mlpr-0.1.1/pyproject.toml` & `mlpr-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlpr"
-version = "0.1.1"
+version = "0.1.2"
 authors = ["Manuel Ferreira Junior <ferreira.jr.ufpb@gmail.com>"]
 description = "A library for machine learning pipeline and creation of reports."
 readme = "README.md"
 maintainers = [
     "Manuel Ferreira Junior <ferreira.jr.ufpb@gmail.com>"
 ]
 classifiers=[
@@ -12,15 +12,15 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Topic :: Software Development",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
   "Topic :: Scientific/Engineering :: Mathematics",
   "Topic :: Scientific/Engineering :: Visualization",
-  "Development Status :: 1 - Planning",
+  "Development Status :: 3 - Alpha",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: Unix",
   "Operating System :: MacOS",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
```

### Comparing `mlpr-0.1.1/src/mlpr/ml/supervisioned/classification/uncertainty.py` & `mlpr-0.1.2/src/mlpr/ml/supervisioned/classification/uncertainty.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.1/src/mlpr/ml/supervisioned/classification/utils.py` & `mlpr-0.1.2/src/mlpr/ml/supervisioned/classification/utils.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.1/src/mlpr/ml/supervisioned/regression/metrics.py` & `mlpr-0.1.2/src/mlpr/ml/supervisioned/regression/metrics.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.1/src/mlpr/ml/supervisioned/regression/plots.py` & `mlpr-0.1.2/src/mlpr/ml/supervisioned/regression/plots.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.1/src/mlpr/ml/supervisioned/tunning/grid_search.py` & `mlpr-0.1.2/src/mlpr/ml/supervisioned/tunning/grid_search.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.1/src/mlpr/reports/create.py` & `mlpr-0.1.2/src/mlpr/reports/create.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.1/PKG-INFO` & `mlpr-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mlpr
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for machine learning pipeline and creation of reports.
 Author: Manuel Ferreira Junior
 Author-email: ferreira.jr.ufpb@gmail.com
 Maintainer: Manuel Ferreira Junior
 Maintainer-email: ferreira.jr.ufpb@gmail.com
 Requires-Python: >=3.9
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
@@ -38,15 +38,34 @@
 Project-URL: issues, https://github.com/Manuelfjr/mlpr/issues
 Project-URL: repository, https://github.com/Manuelfjr/mlpr.git
 Project-URL: source, https://github.com/Manuelfjr/mlpr
 Project-URL: tracker, https://github.com/Manuelfjr/mlpr/tree/develop/issues
 Description-Content-Type: text/markdown
 
 # MLPR Library
-[![TestPyPI version](https://img.shields.io/badge/dynamic/json?url=https://test.pypi.org/pypi/mlpr/json&label=TestPyPI%20version&query=$.info.version&color=blue)](https://test.pypi.org/project/mlpr/)
+
+[![PyPI version](https://img.shields.io/pypi/v/mlpr?color=blue)](https://pypi.org/project/mlpr/)
+[![License](https://img.shields.io/pypi/l/mlpr?color=blue)](https://pypi.org/project/mlpr/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mlpr)](https://pypi.org/project/mlpr/)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/mlpr)](https://pypi.org/project/mlpr/)
+[![PyPI - Status](https://img.shields.io/pypi/status/mlpr)](https://pypi.org/project/mlpr/)
+
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mlpr?style=flat-square&color=darkgreen)](https://pypi.org/project/mlpr/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dw/mlpr?style=flat-square&color=darkgreen)](https://pypi.org/project/mlpr/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dd/mlpr?style=flat-square&color=darkgreen)](https://pypi.org/project/mlpr/)
+
+[![Last Commit](https://img.shields.io/github/last-commit/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/commits)
+[![Open Issues](https://img.shields.io/github/issues-raw/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues)
+[![Closed Issues](https://img.shields.io/github/issues-closed-raw/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues?q=is%3Aissue+is%3Aclosed)
+[![Contributors](https://img.shields.io/github/contributors/Manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/graphs/contributors)
+[![Docs](https://img.shields.io/badge/docs-birtgd-blue?&logo)](https://github.com/Manuelfjr/birt-gd)
+
+[![Author](https://img.shields.io/badge/author-manuelfjr-blue?&logo=github)](https://github.com/Manuelfjr)
+[![https://badgen.net/github/open-issues/manuelfjr/mlpr](https://badgen.net/github/open-issues/manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues?q=is%3Aopen+is%3Aissue)
+[![https://badgen.net/github/closed-issues/manuelfjr/mlpr](https://badgen.net/github/closed-issues/manuelfjr/mlpr)](https://github.com/Manuelfjr/mlpr/issues?q=is%3Aissue+is%3Aclosed)
 
 
 [![fig0](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/regression_plots.png)](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/regression_plots.png)
 
 This repository is a developing library named `MLPR` (Machine Learning Pipeline Report). It aims to facilitate the creation of machine learning models in various areas such as regression, forecasting, classification, and clustering. The library allows the user to perform tuning of these models, generate various types of plots for post-modeling analysis, and calculate various metrics.
 
 In addition, `MLPR` allows the creation of metric reports using [`Jinja2`](https://pypi.org/project/Jinja2/), including the obtained graphs. The user can customize the report template according to their needs.
```

