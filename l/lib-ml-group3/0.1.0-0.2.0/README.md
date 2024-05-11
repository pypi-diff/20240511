# Comparing `tmp/lib_ml_group3-0.1.0.tar.gz` & `tmp/lib_ml_group3-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_ml_group3-0.1.0.tar", max compression
+gzip compressed data, was "lib_ml_group3-0.2.0.tar", max compression
```

## Comparing `lib_ml_group3-0.1.0.tar` & `lib_ml_group3-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1070 2024-05-08 06:47:01.192376 lib_ml_group3-0.1.0/LICENSE
--rw-r--r--   0        0        0        8 2024-05-08 06:47:01.192461 lib_ml_group3-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-08 06:50:12.792566 lib_ml_group3-0.1.0/lib_ml_group3/__init__.py
--rw-r--r--   0        0        0     2564 2024-05-08 14:08:23.688732 lib_ml_group3-0.1.0/lib_ml_group3/preprocessing.py
--rw-r--r--   0        0        0      511 2024-05-10 07:45:32.473629 lib_ml_group3-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 lib_ml_group3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-11 12:03:36.542933 lib_ml_group3-0.2.0/LICENSE
+-rw-r--r--   0        0        0        8 2024-05-11 12:03:36.542933 lib_ml_group3-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 12:03:36.542933 lib_ml_group3-0.2.0/lib_ml_group3/__init__.py
+-rw-r--r--   0        0        0     1606 2024-05-11 12:03:36.542933 lib_ml_group3-0.2.0/lib_ml_group3/load_model.py
+-rw-r--r--   0        0        0     2564 2024-05-11 12:03:36.542933 lib_ml_group3-0.2.0/lib_ml_group3/preprocessing.py
+-rw-r--r--   0        0        0      598 2024-05-11 12:03:36.542933 lib_ml_group3-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      900 1970-01-01 00:00:00.000000 lib_ml_group3-0.2.0/PKG-INFO
```

### Comparing `lib_ml_group3-0.1.0/LICENSE` & `lib_ml_group3-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_ml_group3-0.1.0/lib_ml_group3/preprocessing.py` & `lib_ml_group3-0.2.0/lib_ml_group3/preprocessing.py`

 * *Files identical despite different names*

### Comparing `lib_ml_group3-0.1.0/PKG-INFO` & `lib_ml_group3-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: lib-ml-group3
-Version: 0.1.0
+Version: 0.2.0
 Summary: A library for pre-processing data used in machine learning models
 Home-page: https://github.com/remla24-team3/lib-ml
 License: MIT
 Author: Jasper Bruin
 Author-email: j.jasperbruin@tudelft.nl
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: keras (>=3.3.3,<4.0.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: pylint (==3.1.0)
+Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
+Requires-Dist: tensorflow (>=2.16.1,<3.0.0)
 Project-URL: Repository, https://github.com/remla24-team3/lib-ml
 Description-Content-Type: text/markdown
 
 # lib-ml
```

