# Comparing `tmp/SQLibEngine-0.1.1.tar.gz` & `tmp/SQLibEngine-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLibEngine-0.1.1.tar", last modified: Fri May 10 15:11:20 2024, max compression
+gzip compressed data, was "SQLibEngine-0.1.2.tar", last modified: Sat May 11 10:55:35 2024, max compression
```

## Comparing `SQLibEngine-0.1.1.tar` & `SQLibEngine-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:20.891151 SQLibEngine-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-10 15:11:20.891151 SQLibEngine-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:20.887151 SQLibEngine-0.1.1/SQLib-Engine/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:20.891151 SQLibEngine-0.1.1/SQLib-Engine/Database/
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/Database/Connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/Database/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/Database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:20.891151 SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:20.891151 SQLibEngine-0.1.1/SQLibEngine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-10 15:11:20.000000 SQLibEngine-0.1.1/SQLibEngine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-10 15:11:20.000000 SQLibEngine-0.1.1/SQLibEngine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:11:20.000000 SQLibEngine-0.1.1/SQLibEngine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 15:11:20.000000 SQLibEngine-0.1.1/SQLibEngine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:11:20.891151 SQLibEngine-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:35.731509 SQLibEngine-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-11 10:55:26.000000 SQLibEngine-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-11 10:55:35.727509 SQLibEngine-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-11 10:55:26.000000 SQLibEngine-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:35.727509 SQLibEngine-0.1.2/SQLib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:35.727509 SQLibEngine-0.1.2/SQLib/Database/
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-11 10:55:26.000000 SQLibEngine-0.1.2/SQLib/Database/Connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-11 10:55:26.000000 SQLibEngine-0.1.2/SQLib/Database/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:26.000000 SQLibEngine-0.1.2/SQLib/Database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:35.727509 SQLibEngine-0.1.2/SQLib/SQLEngine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:26.000000 SQLibEngine-0.1.2/SQLib/SQLEngine/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:26.000000 SQLibEngine-0.1.2/SQLib/SQLEngine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-11 10:55:26.000000 SQLibEngine-0.1.2/SQLib/SQLEngine/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:26.000000 SQLibEngine-0.1.2/SQLib/SQLEngine/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-11 10:55:26.000000 SQLibEngine-0.1.2/SQLib/SQLEngine/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-11 10:55:26.000000 SQLibEngine-0.1.2/SQLib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:35.727509 SQLibEngine-0.1.2/SQLibEngine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-11 10:55:35.000000 SQLibEngine-0.1.2/SQLibEngine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-11 10:55:35.000000 SQLibEngine-0.1.2/SQLibEngine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 10:55:35.000000 SQLibEngine-0.1.2/SQLibEngine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 10:55:35.000000 SQLibEngine-0.1.2/SQLibEngine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 10:55:35.731509 SQLibEngine-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-11 10:55:26.000000 SQLibEngine-0.1.2/setup.py
```

### Comparing `SQLibEngine-0.1.1/LICENSE` & `SQLibEngine-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.1.1/PKG-INFO` & `SQLibEngine-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLibEngine
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple SQLite3 wrapper for Python
 Home-page: https://github.com/TRC-Loop/SQLib
 Author: AK
 Author-email: ak@stellar-code.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -22,19 +22,15 @@
 ![GitHub Release](https://img.shields.io/github/v/release/TRC-Loop/SQLib)
 ![PyPI - Version](https://img.shields.io/pypi/v/SQLibEngine)
 ![GitHub forks](https://img.shields.io/github/forks/TRC-Loop/SQLib?style=flat)
 ![GitHub Repo stars](https://img.shields.io/github/stars/TRC-Loop/SQLib?style=flat)
 ![GitHub License](https://img.shields.io/github/license/TRC-Loop/SQLib?style=flat)
 
 ## Installation
-![Install using pip:](https://pypi.org/project/SQLibEngine/)
-
-```bash
-pip3 install SQLibEngine
-```
+https://github.com/TRC-Loop/SQLib/wiki/Installation
 
 ## Features
 
 - Connect to a SQLite3 DB
 - Create or Delete Tables
 - Add, Edit or Delete Records
 - Query
@@ -42,7 +38,8 @@
 ## Quick Start
 
 Coming Soon
 
 ## Contact Me
 Email: ak@stellar-code.com
 
+
```

### Comparing `SQLibEngine-0.1.1/README.md` & `SQLibEngine-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,26 +6,22 @@
 ![GitHub Release](https://img.shields.io/github/v/release/TRC-Loop/SQLib)
 ![PyPI - Version](https://img.shields.io/pypi/v/SQLibEngine)
 ![GitHub forks](https://img.shields.io/github/forks/TRC-Loop/SQLib?style=flat)
 ![GitHub Repo stars](https://img.shields.io/github/stars/TRC-Loop/SQLib?style=flat)
 ![GitHub License](https://img.shields.io/github/license/TRC-Loop/SQLib?style=flat)
 
 ## Installation
-![Install using pip:](https://pypi.org/project/SQLibEngine/)
-
-```bash
-pip3 install SQLibEngine
-```
+https://github.com/TRC-Loop/SQLib/wiki/Installation
 
 ## Features
 
 - Connect to a SQLite3 DB
 - Create or Delete Tables
 - Add, Edit or Delete Records
 - Query
 
 ## Quick Start
 
 Coming Soon
 
 ## Contact Me
-Email: ak@stellar-code.com
+Email: ak@stellar-code.com
```

### Comparing `SQLibEngine-0.1.1/SQLib-Engine/Database/Connection.py` & `SQLibEngine-0.1.2/SQLib/Database/Connection.py`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/operations.py` & `SQLibEngine-0.1.2/SQLib/SQLEngine/operations.py`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/tables.py` & `SQLibEngine-0.1.2/SQLib/SQLEngine/tables.py`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.1.1/SQLibEngine.egg-info/PKG-INFO` & `SQLibEngine-0.1.2/SQLibEngine.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLibEngine
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple SQLite3 wrapper for Python
 Home-page: https://github.com/TRC-Loop/SQLib
 Author: AK
 Author-email: ak@stellar-code.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -22,19 +22,15 @@
 ![GitHub Release](https://img.shields.io/github/v/release/TRC-Loop/SQLib)
 ![PyPI - Version](https://img.shields.io/pypi/v/SQLibEngine)
 ![GitHub forks](https://img.shields.io/github/forks/TRC-Loop/SQLib?style=flat)
 ![GitHub Repo stars](https://img.shields.io/github/stars/TRC-Loop/SQLib?style=flat)
 ![GitHub License](https://img.shields.io/github/license/TRC-Loop/SQLib?style=flat)
 
 ## Installation
-![Install using pip:](https://pypi.org/project/SQLibEngine/)
-
-```bash
-pip3 install SQLibEngine
-```
+https://github.com/TRC-Loop/SQLib/wiki/Installation
 
 ## Features
 
 - Connect to a SQLite3 DB
 - Create or Delete Tables
 - Add, Edit or Delete Records
 - Query
@@ -42,7 +38,8 @@
 ## Quick Start
 
 Coming Soon
 
 ## Contact Me
 Email: ak@stellar-code.com
 
+
```

### Comparing `SQLibEngine-0.1.1/setup.py` & `SQLibEngine-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the README.md file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="SQLibEngine",
-    version="0.1.1",
+    version="0.1.2",
     author="AK",
     author_email="ak@stellar-code.com",
     url="https://github.com/TRC-Loop/SQLib",
     description="A simple SQLite3 wrapper for Python",
     long_description=long_description,  # Set the long description
     long_description_content_type="text/markdown",  # Specify the content type
     packages=find_packages(),
```

