# Comparing `tmp/addemongo-0.0.4.tar.gz` & `tmp/addemongo-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addemongo-0.0.4.tar", last modified: Fri May 10 03:56:06 2024, max compression
+gzip compressed data, was "addemongo-0.0.7.tar", last modified: Fri May 10 05:11:42 2024, max compression
```

## Comparing `addemongo-0.0.4.tar` & `addemongo-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,27 @@
--rw-r--r--   0        0        0      115 2024-05-10 03:55:56.812131 addemongo-0.0.4/LICENSE
--rw-r--r--   0        0        0      128 2024-05-10 03:55:56.812131 addemongo-0.0.4/README.md
--rw-r--r--   0        0        0     3133 2024-05-10 03:56:06.644127 addemongo-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       65 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/__init__.py
--rw-r--r--   0        0        0       22 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/__version__.py
--rw-r--r--   0        0        0     1421 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/_base_client.py
--rw-r--r--   0        0        0        0 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/_motor/__init__.py
--rw-r--r--   0        0        0     4088 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/_motor/_client.py
--rw-r--r--   0        0        0        0 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/_pymongo/__init__.py
--rw-r--r--   0        0        0     4010 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/_pymongo/_client.py
--rw-r--r--   0        0        0      267 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/_types.py
--rw-r--r--   0        0        0      126 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/builders/__init__.py
--rw-r--r--   0        0        0     3079 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/builders/aggregation.py
--rw-r--r--   0        0        0     3508 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/builders/query.py
--rw-r--r--   0        0        0     1407 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/connection.py
--rw-r--r--   0        0        0        0 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/models/__init__.py
--rw-r--r--   0        0        0      193 2024-05-10 03:55:56.812131 addemongo-0.0.4/src/addemongo/models/pagination.py
--rw-r--r--   0        0        0        0 2024-05-10 03:55:56.812131 addemongo-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     3802 2024-05-10 03:55:56.812131 addemongo-0.0.4/tests/addemongo/test_async_functions.py
--rw-r--r--   0        0        0      960 2024-05-10 03:55:56.812131 addemongo-0.0.4/tests/addemongo/test_client.py
--rw-r--r--   0        0        0     2482 2024-05-10 03:55:56.812131 addemongo-0.0.4/tests/addemongo/test_sync_functions.py
--rw-r--r--   0        0        0      216 2024-05-10 03:55:56.812131 addemongo-0.0.4/tests/motor/test_motor.py
--rw-r--r--   0        0        0      227 2024-05-10 03:55:56.812131 addemongo-0.0.4/tests/pymongo/test_pymongo.py
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 addemongo-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2258 2024-05-10 05:11:10.663596 addemongo-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      115 2024-05-10 05:11:10.663596 addemongo-0.0.7/LICENSE
+-rw-r--r--   0        0        0      115 2024-05-10 05:11:10.663596 addemongo-0.0.7/LICENSE
+-rw-r--r--   0        0        0      128 2024-05-10 05:11:10.663596 addemongo-0.0.7/README.md
+-rw-r--r--   0        0        0      128 2024-05-10 05:11:10.663596 addemongo-0.0.7/README.md
+-rw-r--r--   0        0        0     3134 2024-05-10 05:11:42.791616 addemongo-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       65 2024-05-10 05:11:10.663596 addemongo-0.0.7/src/addemongo/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-10 05:11:10.663596 addemongo-0.0.7/src/addemongo/__version__.py
+-rw-r--r--   0        0        0     1421 2024-05-10 05:11:10.663596 addemongo-0.0.7/src/addemongo/_base_client.py
+-rw-r--r--   0        0        0        0 2024-05-10 05:11:10.663596 addemongo-0.0.7/src/addemongo/_motor/__init__.py
+-rw-r--r--   0        0        0     4088 2024-05-10 05:11:10.663596 addemongo-0.0.7/src/addemongo/_motor/_client.py
+-rw-r--r--   0        0        0        0 2024-05-10 05:11:10.663596 addemongo-0.0.7/src/addemongo/_pymongo/__init__.py
+-rw-r--r--   0        0        0     4010 2024-05-10 05:11:10.663596 addemongo-0.0.7/src/addemongo/_pymongo/_client.py
+-rw-r--r--   0        0        0      267 2024-05-10 05:11:10.663596 addemongo-0.0.7/src/addemongo/_types.py
+-rw-r--r--   0        0        0      126 2024-05-10 05:11:10.663596 addemongo-0.0.7/src/addemongo/builders/__init__.py
+-rw-r--r--   0        0        0     3079 2024-05-10 05:11:10.663596 addemongo-0.0.7/src/addemongo/builders/aggregation.py
+-rw-r--r--   0        0        0     3508 2024-05-10 05:11:10.663596 addemongo-0.0.7/src/addemongo/builders/query.py
+-rw-r--r--   0        0        0     1407 2024-05-10 05:11:10.663596 addemongo-0.0.7/src/addemongo/connection.py
+-rw-r--r--   0        0        0        0 2024-05-10 05:11:10.667596 addemongo-0.0.7/src/addemongo/models/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-10 05:11:10.667596 addemongo-0.0.7/src/addemongo/models/pagination.py
+-rw-r--r--   0        0        0        0 2024-05-10 05:11:10.667596 addemongo-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     3802 2024-05-10 05:11:10.667596 addemongo-0.0.7/tests/addemongo/test_async_functions.py
+-rw-r--r--   0        0        0      960 2024-05-10 05:11:10.667596 addemongo-0.0.7/tests/addemongo/test_client.py
+-rw-r--r--   0        0        0     2482 2024-05-10 05:11:10.667596 addemongo-0.0.7/tests/addemongo/test_sync_functions.py
+-rw-r--r--   0        0        0      216 2024-05-10 05:11:10.667596 addemongo-0.0.7/tests/motor/test_motor.py
+-rw-r--r--   0        0        0      227 2024-05-10 05:11:10.667596 addemongo-0.0.7/tests/pymongo/test_pymongo.py
+-rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 addemongo-0.0.7/PKG-INFO
```

### Comparing `addemongo-0.0.4/pyproject.toml` & `addemongo-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     { name = "Victor Gabriel", email = "victordeonroyale@gmail.com" },
 ]
 maintainers = [
     { name = "Gabriel Silva", email = "gabrieltkdnobrega63@gmail.com" },
     { name = "Victor Gabriel", email = "victordeonroyale@gmail.com" },
 ]
 dynamic = []
-version = "0.0.4"
+version = "0.0.7"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Company = "https://addebitare.com.br"
 Repository = "https://github.com/biellSilva/addemongo.git"
@@ -29,29 +29,29 @@
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
-[too.pdm.build]
+[tool.pdm]
+distribution = true
+
+[tool.pdm.build]
 excludes = [
     "./**/.git",
 ]
 package-dir = "src"
 source-includes = [
     "tests",
     "CHANGELOG.md",
     "LICENSE",
     "README.md",
 ]
 
-[tool.pdm]
-distribution = true
-
 [tool.pdm.version]
 source = "file"
 path = "src/addemongo/__version__.py"
 
 [tool.pdm.scripts]
 test = "pytest"
 test-watch = "ptw"
```

### Comparing `addemongo-0.0.4/src/addemongo/_base_client.py` & `addemongo-0.0.7/src/addemongo/_base_client.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.4/src/addemongo/_motor/_client.py` & `addemongo-0.0.7/src/addemongo/_motor/_client.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.4/src/addemongo/_pymongo/_client.py` & `addemongo-0.0.7/src/addemongo/_pymongo/_client.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.4/src/addemongo/builders/aggregation.py` & `addemongo-0.0.7/src/addemongo/builders/aggregation.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.4/src/addemongo/builders/query.py` & `addemongo-0.0.7/src/addemongo/builders/query.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.4/src/addemongo/connection.py` & `addemongo-0.0.7/src/addemongo/connection.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.4/tests/addemongo/test_async_functions.py` & `addemongo-0.0.7/tests/addemongo/test_async_functions.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.4/tests/addemongo/test_client.py` & `addemongo-0.0.7/tests/addemongo/test_client.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.4/tests/addemongo/test_sync_functions.py` & `addemongo-0.0.7/tests/addemongo/test_sync_functions.py`

 * *Files identical despite different names*

### Comparing `addemongo-0.0.4/PKG-INFO` & `addemongo-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: addemongo
-Version: 0.0.4
+Version: 0.0.7
 Summary: Private mongo repository for Addebitare company
 Author-Email: Gabriel Silva <gabrieltkdnobrega63@gmail.com>, Victor Gabriel <victordeonroyale@gmail.com>
 Maintainer-Email: Gabriel Silva <gabrieltkdnobrega63@gmail.com>, Victor Gabriel <victordeonroyale@gmail.com>
 License: All Rights Reserved.
         
         (c) Copyright 2024 Gabriel Nobrega, Victor Gabriel and Addebitare Team, all rights reserved.
 Project-URL: Company, https://addebitare.com.br
```

