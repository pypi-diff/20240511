# Comparing `tmp/valeralib-1.4.1.tar.gz` & `tmp/valeralib-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valeralib-1.4.1.tar", last modified: Tue May  7 13:06:52 2024, max compression
+gzip compressed data, was "valeralib-1.4.2.tar", last modified: Sat May 11 20:30:22 2024, max compression
```

## Comparing `valeralib-1.4.1.tar` & `valeralib-1.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0      411 2023-08-23 20:42:10.000000 valeralib-1.4.1/README.md
--rwxr-xr-x   0        0        0     6524 2023-10-24 22:19:30.534392 valeralib-1.4.1/ValeraLib/Binance.py
--rwxr-xr-x   0        0        0     3720 2023-08-15 12:26:40.000000 valeralib-1.4.1/ValeraLib/DataScience.py
--rwxr-xr-x   0        0        0     7251 2023-10-27 19:22:08.113453 valeralib-1.4.1/ValeraLib/Valera.py
--rwxr-xr-x   0        0        0      402 2024-03-13 20:16:05.523601 valeralib-1.4.1/ValeraLib/__init__.py
--rw-r--r--   0        0        0      216 2024-03-13 22:50:35.900945 valeralib-1.4.1/ValeraLib/prelude.py
--rwxr-xr-x   0        0        0     7883 2024-03-12 13:13:57.313243 valeralib-1.4.1/ValeraLib/utils/DuckTypes.py
--rwxr-xr-x   0        0        0     6587 2022-03-26 20:22:20.000000 valeralib-1.4.1/ValeraLib/utils/Notification.mp3
--rwxr-xr-x   0        0        0        0 2024-03-12 13:12:13.224838 valeralib-1.4.1/ValeraLib/utils/__init__.py
--rw-r--r--   0        0        0     8688 2024-03-14 02:04:55.644812 valeralib-1.4.1/ValeraLib/utils/rust_types.py
--rw-r--r--   0        0        0     1460 2024-05-07 13:06:52.456505 valeralib-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2324 2024-03-14 01:59:46.813834 valeralib-1.4.1/tests/rust_types/test_option.py
--rw-r--r--   0        0        0     1622 2024-03-14 02:05:09.954856 valeralib-1.4.1/tests/rust_types/test_result.py
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 valeralib-1.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0      411 2023-08-23 20:42:10.000000 valeralib-1.4.2/README.md
+-rwxr-xr-x   0        0        0     6524 2023-10-24 22:19:30.534392 valeralib-1.4.2/ValeraLib/Binance.py
+-rwxr-xr-x   0        0        0     3720 2023-08-15 12:26:40.000000 valeralib-1.4.2/ValeraLib/DataScience.py
+-rwxr-xr-x   0        0        0     7251 2023-10-27 19:22:08.113453 valeralib-1.4.2/ValeraLib/Valera.py
+-rwxr-xr-x   0        0        0      402 2024-03-13 20:16:05.523601 valeralib-1.4.2/ValeraLib/__init__.py
+-rw-r--r--   0        0        0      216 2024-03-13 22:50:35.900945 valeralib-1.4.2/ValeraLib/prelude.py
+-rwxr-xr-x   0        0        0     7883 2024-03-12 13:13:57.313243 valeralib-1.4.2/ValeraLib/utils/DuckTypes.py
+-rwxr-xr-x   0        0        0     6587 2022-03-26 20:22:20.000000 valeralib-1.4.2/ValeraLib/utils/Notification.mp3
+-rwxr-xr-x   0        0        0        0 2024-03-12 13:12:13.224838 valeralib-1.4.2/ValeraLib/utils/__init__.py
+-rw-r--r--   0        0        0     8688 2024-03-14 02:04:55.644812 valeralib-1.4.2/ValeraLib/utils/rust_types.py
+-rw-r--r--   0        0        0     1474 2024-05-11 20:30:22.917020 valeralib-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2324 2024-03-14 01:59:46.813834 valeralib-1.4.2/tests/rust_types/test_option.py
+-rw-r--r--   0        0        0     1622 2024-03-14 02:05:09.954856 valeralib-1.4.2/tests/rust_types/test_result.py
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 valeralib-1.4.2/PKG-INFO
```

### Comparing `valeralib-1.4.1/ValeraLib/Binance.py` & `valeralib-1.4.2/ValeraLib/Binance.py`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.1/ValeraLib/DataScience.py` & `valeralib-1.4.2/ValeraLib/DataScience.py`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.1/ValeraLib/Valera.py` & `valeralib-1.4.2/ValeraLib/Valera.py`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.1/ValeraLib/utils/DuckTypes.py` & `valeralib-1.4.2/ValeraLib/utils/DuckTypes.py`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.1/ValeraLib/utils/Notification.mp3` & `valeralib-1.4.2/ValeraLib/utils/Notification.mp3`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.1/ValeraLib/utils/rust_types.py` & `valeralib-1.4.2/ValeraLib/utils/rust_types.py`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.1/pyproject.toml` & `valeralib-1.4.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ValeraLib"
-version = "1.4.1"
+version = "1.4.2"
 description = "The library goes brrrrrr"
 keywords = [
     "The greatest package to ever exist",
 ]
 readme = "README.md"
 authors = [
     { name = "Valera", email = "v79166789533@gmail.com" },
@@ -20,20 +20,20 @@
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 requires-python = ">=3.6"
 dependencies = [
-    "numpy>=1.24.3,<2.0.0",
-    "pandas>=1.5.3,<2.0.0",
-    "playsound>=1.2.2,<2.0.0",
-    "plotly>=5.14.1,<6.0.0",
+    "numpy>=1.26.4,<2.0.0",
+    "pandas>=2.2.2,<3.0.0",
+    "playsound>=1.3.0,<2.0.0",
+    "plotly>=5.22.0,<6.0.0",
     "requests>=2.31.0,<3.0.0",
-    "telebot",
+    "telebot>=0.0.5,<1.0.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Valera6/ValeraLib"
 
 [build-system]
 requires = [
```

### Comparing `valeralib-1.4.1/tests/rust_types/test_option.py` & `valeralib-1.4.2/tests/rust_types/test_option.py`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.1/tests/rust_types/test_result.py` & `valeralib-1.4.2/tests/rust_types/test_result.py`

 * *Files identical despite different names*

### Comparing `valeralib-1.4.1/PKG-INFO` & `valeralib-1.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ValeraLib
-Version: 1.4.1
+Version: 1.4.2
 Summary: The library goes brrrrrr
 Keywords: The greatest package to ever exist
 Author-Email: Valera <v79166789533@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,20 +13,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Project-URL: Homepage, https://github.com/Valera6/ValeraLib
 Requires-Python: >=3.6
-Requires-Dist: numpy<2.0.0,>=1.24.3
-Requires-Dist: pandas<2.0.0,>=1.5.3
-Requires-Dist: playsound<2.0.0,>=1.2.2
-Requires-Dist: plotly<6.0.0,>=5.14.1
+Requires-Dist: numpy<2.0.0,>=1.26.4
+Requires-Dist: pandas<3.0.0,>=2.2.2
+Requires-Dist: playsound<2.0.0,>=1.3.0
+Requires-Dist: plotly<6.0.0,>=5.22.0
 Requires-Dist: requests<3.0.0,>=2.31.0
-Requires-Dist: telebot
+Requires-Dist: telebot<1.0.0,>=0.0.5
 Description-Content-Type: text/markdown
 
 # Example:
 
 ```python
 from ValeraLib import Binance, DataScience as ds
 from ValeraLib.utils.DuckTypes import *
```

