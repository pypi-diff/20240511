# Comparing `tmp/jubtools-0.5.5.tar.gz` & `tmp/jubtools-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jubtools-0.5.5.tar", last modified: Sat May  4 23:08:30 2024, max compression
+gzip compressed data, was "jubtools-0.5.6.tar", last modified: Sat May 11 11:09:06 2024, max compression
```

## Comparing `jubtools-0.5.5.tar` & `jubtools-0.5.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 23:08:30.699041 jubtools-0.5.5/
--rw-r--r--   0 andy       (501) staff       (20)    35149 2023-11-25 11:26:03.000000 jubtools-0.5.5/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-04 23:08:30.698806 jubtools-0.5.5/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      183 2024-05-03 12:01:13.000000 jubtools-0.5.5/README.md
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 23:08:30.697008 jubtools-0.5.5/jubtools/
--rw-r--r--   0 andy       (501) staff       (20)        0 2023-11-25 11:26:03.000000 jubtools-0.5.5/jubtools/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     1695 2024-05-04 19:58:54.000000 jubtools-0.5.5/jubtools/config.py
--rw-r--r--   0 andy       (501) staff       (20)     1295 2024-05-04 19:57:40.000000 jubtools-0.5.5/jubtools/httptools.py
--rw-r--r--   0 andy       (501) staff       (20)      370 2024-05-03 13:10:41.000000 jubtools-0.5.5/jubtools/misctools.py
--rw-r--r--   0 andy       (501) staff       (20)     4861 2024-05-04 22:46:34.000000 jubtools-0.5.5/jubtools/psql.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-05-01 16:00:18.000000 jubtools-0.5.5/jubtools/py.typed
--rw-r--r--   0 andy       (501) staff       (20)     1143 2024-05-03 11:07:09.000000 jubtools-0.5.5/jubtools/sqlt.py
--rw-r--r--   0 andy       (501) staff       (20)     3961 2024-05-04 23:08:00.000000 jubtools-0.5.5/jubtools/systemtools.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 23:08:30.698395 jubtools-0.5.5/jubtools.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-04 23:08:30.000000 jubtools-0.5.5/jubtools.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      422 2024-05-04 23:08:30.000000 jubtools-0.5.5/jubtools.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-04 23:08:30.000000 jubtools-0.5.5/jubtools.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       64 2024-05-04 23:08:30.000000 jubtools-0.5.5/jubtools.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)        9 2024-05-04 23:08:30.000000 jubtools-0.5.5/jubtools.egg-info/top_level.txt
--rw-r--r--   0 andy       (501) staff       (20)      597 2024-05-04 23:07:38.000000 jubtools-0.5.5/pyproject.toml
--rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-04 23:08:30.699079 jubtools-0.5.5/setup.cfg
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-04 23:08:30.698228 jubtools-0.5.5/tests/
--rw-r--r--   0 andy       (501) staff       (20)     1214 2024-05-01 16:00:18.000000 jubtools-0.5.5/tests/test_config.py
--rw-r--r--   0 andy       (501) staff       (20)      260 2024-05-03 13:16:29.000000 jubtools-0.5.5/tests/test_misctools.py
--rw-r--r--   0 andy       (501) staff       (20)      352 2024-05-03 13:31:23.000000 jubtools-0.5.5/tests/test_systemtools.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-11 11:09:06.224435 jubtools-0.5.6/
+-rw-r--r--   0 andy       (501) staff       (20)    35149 2023-11-25 11:26:03.000000 jubtools-0.5.6/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-11 11:09:06.224213 jubtools-0.5.6/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      183 2024-05-03 12:01:13.000000 jubtools-0.5.6/README.md
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-11 11:09:06.222280 jubtools-0.5.6/jubtools/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2023-11-25 11:26:03.000000 jubtools-0.5.6/jubtools/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     1695 2024-05-04 19:58:54.000000 jubtools-0.5.6/jubtools/config.py
+-rw-r--r--   0 andy       (501) staff       (20)     1295 2024-05-04 19:57:40.000000 jubtools-0.5.6/jubtools/httptools.py
+-rw-r--r--   0 andy       (501) staff       (20)      370 2024-05-03 13:10:41.000000 jubtools-0.5.6/jubtools/misctools.py
+-rw-r--r--   0 andy       (501) staff       (20)     4861 2024-05-04 22:46:34.000000 jubtools-0.5.6/jubtools/psql.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-05-01 16:00:18.000000 jubtools-0.5.6/jubtools/py.typed
+-rw-r--r--   0 andy       (501) staff       (20)     1143 2024-05-03 11:07:09.000000 jubtools-0.5.6/jubtools/sqlt.py
+-rw-r--r--   0 andy       (501) staff       (20)     4301 2024-05-11 11:07:59.000000 jubtools-0.5.6/jubtools/systemtools.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-11 11:09:06.223754 jubtools-0.5.6/jubtools.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)    41184 2024-05-11 11:09:06.000000 jubtools-0.5.6/jubtools.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)      422 2024-05-11 11:09:06.000000 jubtools-0.5.6/jubtools.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-05-11 11:09:06.000000 jubtools-0.5.6/jubtools.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       64 2024-05-11 11:09:06.000000 jubtools-0.5.6/jubtools.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)        9 2024-05-11 11:09:06.000000 jubtools-0.5.6/jubtools.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)      597 2024-05-11 11:08:29.000000 jubtools-0.5.6/pyproject.toml
+-rw-r--r--   0 andy       (501) staff       (20)       38 2024-05-11 11:09:06.224481 jubtools-0.5.6/setup.cfg
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-05-11 11:09:06.223492 jubtools-0.5.6/tests/
+-rw-r--r--   0 andy       (501) staff       (20)     1214 2024-05-01 16:00:18.000000 jubtools-0.5.6/tests/test_config.py
+-rw-r--r--   0 andy       (501) staff       (20)      260 2024-05-03 13:16:29.000000 jubtools-0.5.6/tests/test_misctools.py
+-rw-r--r--   0 andy       (501) staff       (20)      352 2024-05-03 13:31:23.000000 jubtools-0.5.6/tests/test_systemtools.py
```

### Comparing `jubtools-0.5.5/LICENSE` & `jubtools-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.5/PKG-INFO` & `jubtools-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jubtools
-Version: 0.5.5
+Version: 0.5.6
 Summary: Shared tools for my own work
 Author-email: Andrew Morcom <jubulani@fastmail.fm>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `jubtools-0.5.5/jubtools/config.py` & `jubtools-0.5.6/jubtools/config.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.5/jubtools/httptools.py` & `jubtools-0.5.6/jubtools/httptools.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.5/jubtools/psql.py` & `jubtools-0.5.6/jubtools/psql.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.5/jubtools/sqlt.py` & `jubtools-0.5.6/jubtools/sqlt.py`

 * *Files identical despite different names*

### Comparing `jubtools-0.5.5/jubtools/systemtools.py` & `jubtools-0.5.6/jubtools/systemtools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime as dt
 from enum import Enum
 import logging
 import os
 from typing import Any
 
 from fastapi import FastAPI, Response
+from fastapi.middleware.cors import CORSMiddleware
 from pydantic import BaseModel
 
 # from errors import AuthError, FSError
 
 from jubtools import config, misctools
 
 logger = logging.getLogger(__name__)
@@ -37,14 +38,23 @@
     }
     if 'root_path' in config.get('fastapi'):
         fastapi_args["root_path"] = config.get("fastapi.root_path")
     if config.get("fastapi.disable_docs"):
         fastapi_args["openapi_url"] = None
     app = FastAPI(**fastapi_args)
 
+    if 'cors_allow_origin' in config.get('fastapi'):
+        app.add_middleware(
+            CORSMiddleware,
+            allow_origins=config.get('fastapi.cors_allow_origin'),
+            allow_credentials=True,
+            allow_methods=["*"],
+            allow_headers=["*"],
+        )
+
     APP_START_TIME = dt.datetime.now()
     app.add_api_route("/health", health_handler, methods=["GET"])
 
     if db_module is not None:
         init_db_module(db_module, app)
     # app.add_exception_handler(FSError, custom_exception_handler)
```

### Comparing `jubtools-0.5.5/jubtools.egg-info/PKG-INFO` & `jubtools-0.5.6/jubtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jubtools
-Version: 0.5.5
+Version: 0.5.6
 Summary: Shared tools for my own work
 Author-email: Andrew Morcom <jubulani@fastmail.fm>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `jubtools-0.5.5/pyproject.toml` & `jubtools-0.5.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "jubtools"
 description = "Shared tools for my own work"
 readme = "README.md"
 license = { file = "LICENSE" }
-version = "0.5.5"
+version = "0.5.6"
 authors = [{ name = "Andrew Morcom", email = "jubulani@fastmail.fm" }]
 requires-python = ">=3.10"
 dependencies = ["fastapi"]
 
 [project.optional-dependencies]
 test = [
     "async_asgi_testclient >= 1.4",
```

### Comparing `jubtools-0.5.5/tests/test_config.py` & `jubtools-0.5.6/tests/test_config.py`

 * *Files identical despite different names*

