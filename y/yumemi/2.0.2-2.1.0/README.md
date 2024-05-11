# Comparing `tmp/yumemi-2.0.2.tar.gz` & `tmp/yumemi-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yumemi-2.0.2.tar", max compression
+gzip compressed data, was "yumemi-2.1.0.tar", max compression
```

## Comparing `yumemi-2.0.2.tar` & `yumemi-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1071 2023-12-02 13:24:19.721197 yumemi-2.0.2/LICENSE
--rw-r--r--   0        0        0      416 2023-12-02 13:24:19.721197 yumemi-2.0.2/README.rst
--rw-r--r--   0        0        0      921 2023-12-02 13:24:19.721197 yumemi-2.0.2/docs/api.rst
--rw-r--r--   0        0        0       70 2023-12-02 13:24:19.721197 yumemi-2.0.2/docs/cli.rst
--rw-r--r--   0        0        0     1326 2023-12-02 13:24:19.721197 yumemi-2.0.2/docs/conf.py
--rw-r--r--   0        0        0      491 2023-12-02 13:24:19.721197 yumemi-2.0.2/docs/index.rst
--rw-r--r--   0        0        0     1643 2023-12-02 13:24:19.721197 yumemi-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      284 2023-12-02 13:24:19.721197 yumemi-2.0.2/src/yumemi/__init__.py
--rw-r--r--   0        0        0     2120 2023-12-02 13:24:19.721197 yumemi-2.0.2/src/yumemi/_rhash/__init__.py
--rw-r--r--   0        0        0      423 2023-12-02 13:24:19.721197 yumemi-2.0.2/src/yumemi/_rhash/libname.py
--rw-r--r--   0        0        0    13359 2023-12-02 13:24:19.725197 yumemi-2.0.2/src/yumemi/_rhash/rhash.py
--rw-r--r--   0        0        0    10557 2023-12-02 13:24:19.725197 yumemi-2.0.2/src/yumemi/anidb.py
--rw-r--r--   0        0        0     4145 2023-12-02 13:24:19.725197 yumemi-2.0.2/src/yumemi/cli.py
--rw-r--r--   0        0        0      592 2023-12-02 13:24:19.725197 yumemi-2.0.2/src/yumemi/exceptions.py
--rw-r--r--   0        0        0        0 2023-12-02 13:24:19.725197 yumemi-2.0.2/src/yumemi/py.typed
--rw-r--r--   0        0        0        0 2023-12-02 13:24:19.725197 yumemi-2.0.2/tests/__init__.py
--rw-r--r--   0        0        0     3351 2023-12-02 13:24:19.725197 yumemi-2.0.2/tests/test_anidb.py
--rw-r--r--   0        0        0     2529 2023-12-02 13:24:19.725197 yumemi-2.0.2/tests/test_cli.py
--rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 yumemi-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-11 13:16:35.607317 yumemi-2.1.0/LICENSE
+-rw-r--r--   0        0        0      432 2024-05-11 13:16:35.607317 yumemi-2.1.0/README.rst
+-rw-r--r--   0        0        0      921 2024-05-11 13:16:35.607317 yumemi-2.1.0/docs/api.rst
+-rw-r--r--   0        0        0      480 2024-05-11 13:16:35.607317 yumemi-2.1.0/docs/cli.rst
+-rw-r--r--   0        0        0     1326 2024-05-11 13:16:35.607317 yumemi-2.1.0/docs/conf.py
+-rw-r--r--   0        0        0      491 2024-05-11 13:16:35.607317 yumemi-2.1.0/docs/index.rst
+-rw-r--r--   0        0        0     1643 2024-05-11 13:16:35.611317 yumemi-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      284 2024-05-11 13:16:35.611317 yumemi-2.1.0/src/yumemi/__init__.py
+-rw-r--r--   0        0        0     2120 2024-05-11 13:16:35.611317 yumemi-2.1.0/src/yumemi/_rhash/__init__.py
+-rw-r--r--   0        0        0      423 2024-05-11 13:16:35.611317 yumemi-2.1.0/src/yumemi/_rhash/libname.py
+-rw-r--r--   0        0        0    13359 2024-05-11 13:16:35.611317 yumemi-2.1.0/src/yumemi/_rhash/rhash.py
+-rw-r--r--   0        0        0    10557 2024-05-11 13:16:35.611317 yumemi-2.1.0/src/yumemi/anidb.py
+-rw-r--r--   0        0        0     7054 2024-05-11 13:16:35.611317 yumemi-2.1.0/src/yumemi/cli.py
+-rw-r--r--   0        0        0      592 2024-05-11 13:16:35.611317 yumemi-2.1.0/src/yumemi/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-11 13:16:35.611317 yumemi-2.1.0/src/yumemi/py.typed
+-rw-r--r--   0        0        0        0 2024-05-11 13:16:35.611317 yumemi-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3351 2024-05-11 13:16:35.611317 yumemi-2.1.0/tests/test_anidb.py
+-rw-r--r--   0        0        0     2529 2024-05-11 13:16:35.611317 yumemi-2.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 yumemi-2.1.0/PKG-INFO
```

### Comparing `yumemi-2.0.2/LICENSE` & `yumemi-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yumemi-2.0.2/docs/api.rst` & `yumemi-2.1.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `yumemi-2.0.2/docs/conf.py` & `yumemi-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yumemi-2.0.2/pyproject.toml` & `yumemi-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yumemi"
-version = "2.0.2"
+version = "2.1.0"
 description = "AniDB API library for Python and simple CLI client"
 readme = "README.rst"
 authors = ["Filip Pobořil <tsuki@fpob.cz>"]
 license = "MIT"
 repository = "https://github.com/fpob/yumemi"
 documentation = "https://yumemi.readthedocs.io/"
 keywords = ["AniDB"]
```

### Comparing `yumemi-2.0.2/src/yumemi/_rhash/__init__.py` & `yumemi-2.1.0/src/yumemi/_rhash/__init__.py`

 * *Files identical despite different names*

### Comparing `yumemi-2.0.2/src/yumemi/_rhash/rhash.py` & `yumemi-2.1.0/src/yumemi/_rhash/rhash.py`

 * *Files identical despite different names*

### Comparing `yumemi-2.0.2/src/yumemi/anidb.py` & `yumemi-2.1.0/src/yumemi/anidb.py`

 * *Files identical despite different names*

### Comparing `yumemi-2.0.2/src/yumemi/exceptions.py` & `yumemi-2.1.0/src/yumemi/exceptions.py`

 * *Files identical despite different names*

### Comparing `yumemi-2.0.2/tests/test_anidb.py` & `yumemi-2.1.0/tests/test_anidb.py`

 * *Files identical despite different names*

### Comparing `yumemi-2.0.2/tests/test_cli.py` & `yumemi-2.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `yumemi-2.0.2/PKG-INFO` & `yumemi-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yumemi
-Version: 2.0.2
+Version: 2.1.0
 Summary: AniDB API library for Python and simple CLI client
 Home-page: https://github.com/fpob/yumemi
 License: MIT
 Keywords: AniDB
 Author: Filip Pobořil
 Author-email: tsuki@fpob.cz
 Requires-Python: >=3.9,<4.0
@@ -25,15 +25,16 @@
 Project-URL: Documentation, https://yumemi.readthedocs.io/
 Project-URL: Repository, https://github.com/fpob/yumemi
 Description-Content-Type: text/x-rst
 
 Yumemi
 ======
 
-AniDB API library for Python and simple CLI client to add files to mylist.
+AniDB API library for Python and simple CLI client to add files to mylist and
+rename them.
 
 
 Installation
 ------------
 
 I recommend using pipx_ to install the CLI client ::
```

