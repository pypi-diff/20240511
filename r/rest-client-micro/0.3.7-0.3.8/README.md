# Comparing `tmp/rest_client_micro-0.3.7.tar.gz` & `tmp/rest_client_micro-0.3.8.tar.gz`

## Comparing `rest_client_micro-0.3.7.tar` & `rest_client_micro-0.3.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/src/rest_client_micro/__init__.py
--rwxr-xr-x   0        0        0     1031 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/src/rest_client_micro/_utils.py
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/src/rest_client_micro/basic_auth.py
--rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/src/rest_client_micro/response.py
--rwxr-xr-x   0        0        0     7227 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/src/rest_client_micro/rest_client.py
--rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/src/rest_client_micro/rest_object.py
--rwxr-xr-x   0        0        0     1247 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/tests/flask_server.py
--rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/tests/test_rest_client.py
--rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/tests/test_auth/test_auth.py
--rwxr-xr-x   0        0        0     1852 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/.gitignore
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/LICENSE
--rwxr-xr-x   0        0        0     1421 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/README.md
--rwxr-xr-x   0        0        0      426 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/PKG-INFO
+-rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/src/rest_client_micro/__init__.py
+-rwxr-xr-x   0        0        0     1026 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/src/rest_client_micro/_utils.py
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/src/rest_client_micro/basic_auth.py
+-rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/src/rest_client_micro/response.py
+-rwxr-xr-x   0        0        0     7227 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/src/rest_client_micro/rest_client.py
+-rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/src/rest_client_micro/rest_object.py
+-rwxr-xr-x   0        0        0     1247 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/tests/flask_server.py
+-rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/tests/test_rest_client.py
+-rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/tests/test_auth/test_auth.py
+-rwxr-xr-x   0        0        0     1852 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/.gitignore
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/LICENSE
+-rwxr-xr-x   0        0        0     1421 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/README.md
+-rwxr-xr-x   0        0        0      426 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/PKG-INFO
```

### Comparing `rest_client_micro-0.3.7/src/rest_client_micro/_utils.py` & `rest_client_micro-0.3.8/src/rest_client_micro/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import time
 
 
-def file_not_old(file, age_minutes=5):
+def file_not_old(file, age_seconds=5):
     try:
         if file_exists(file):
             file_age_mtime = _get_time(time.time()) - _get_time(file_age(file))
-            if file_age_mtime / 60 > age_minutes:
+            if file_age_mtime > age_seconds:
                 return False
             else:
                 return True
         return False
     except Exception as e:
         print(f'caught {type(e)}: e')
         return False
```

### Comparing `rest_client_micro-0.3.7/src/rest_client_micro/response.py` & `rest_client_micro-0.3.8/src/rest_client_micro/response.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.7/src/rest_client_micro/rest_client.py` & `rest_client_micro-0.3.8/src/rest_client_micro/rest_client.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.7/src/rest_client_micro/rest_object.py` & `rest_client_micro-0.3.8/src/rest_client_micro/rest_object.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.7/tests/flask_server.py` & `rest_client_micro-0.3.8/tests/flask_server.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.7/tests/test_rest_client.py` & `rest_client_micro-0.3.8/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.7/tests/test_auth/test_auth.py` & `rest_client_micro-0.3.8/tests/test_auth/test_auth.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.7/.gitignore` & `rest_client_micro-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.7/LICENSE` & `rest_client_micro-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.7/README.md` & `rest_client_micro-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.7/PKG-INFO` & `rest_client_micro-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rest_client_micro
-Version: 0.3.7
+Version: 0.3.8
 Summary: A micro rest client
 Author: Samuel Shiels
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11.5
```

