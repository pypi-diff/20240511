# Comparing `tmp/rest_client_micro-0.3.6.tar.gz` & `tmp/rest_client_micro-0.3.7.tar.gz`

## Comparing `rest_client_micro-0.3.6.tar` & `rest_client_micro-0.3.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 rest_client_micro-0.3.6/src/rest_client_micro/__init__.py
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 rest_client_micro-0.3.6/src/rest_client_micro/basic_auth.py
--rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 rest_client_micro-0.3.6/src/rest_client_micro/response.py
--rwxr-xr-x   0        0        0     7136 2020-02-02 00:00:00.000000 rest_client_micro-0.3.6/src/rest_client_micro/rest_client.py
--rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 rest_client_micro-0.3.6/src/rest_client_micro/rest_object.py
--rwxr-xr-x   0        0        0     1247 2020-02-02 00:00:00.000000 rest_client_micro-0.3.6/tests/flask_server.py
--rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 rest_client_micro-0.3.6/tests/test_rest_client.py
--rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 rest_client_micro-0.3.6/tests/test_auth/test_auth.py
--rwxr-xr-x   0        0        0     1852 2020-02-02 00:00:00.000000 rest_client_micro-0.3.6/.gitignore
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 rest_client_micro-0.3.6/LICENSE
--rwxr-xr-x   0        0        0     1421 2020-02-02 00:00:00.000000 rest_client_micro-0.3.6/README.md
--rwxr-xr-x   0        0        0      426 2020-02-02 00:00:00.000000 rest_client_micro-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 rest_client_micro-0.3.6/PKG-INFO
+-rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/src/rest_client_micro/__init__.py
+-rwxr-xr-x   0        0        0     1031 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/src/rest_client_micro/_utils.py
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/src/rest_client_micro/basic_auth.py
+-rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/src/rest_client_micro/response.py
+-rwxr-xr-x   0        0        0     7227 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/src/rest_client_micro/rest_client.py
+-rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/src/rest_client_micro/rest_object.py
+-rwxr-xr-x   0        0        0     1247 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/tests/flask_server.py
+-rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/tests/test_rest_client.py
+-rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/tests/test_auth/test_auth.py
+-rwxr-xr-x   0        0        0     1852 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/.gitignore
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/LICENSE
+-rwxr-xr-x   0        0        0     1421 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/README.md
+-rwxr-xr-x   0        0        0      426 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 rest_client_micro-0.3.7/PKG-INFO
```

### Comparing `rest_client_micro-0.3.6/src/rest_client_micro/response.py` & `rest_client_micro-0.3.7/src/rest_client_micro/response.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.6/src/rest_client_micro/rest_client.py` & `rest_client_micro-0.3.7/src/rest_client_micro/rest_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import time
 import requests
 
 from requests.auth import AuthBase
 from requests.auth import HTTPBasicAuth
 from .rest_object import RESTObject as RO
 from .response import Response as R
+from ._utils import file_not_old
 
 
 class RESTClient():
     """
     Wrapper class for requests calls
     """
 
@@ -173,15 +174,16 @@
             R: Response object, use `error` property to check if call was successful
         """
         self._debug("retrieve_file " + config.endpoint + " - " + file_name)
         config.operation = "file"
         result = self._execute_call(config)
         if result.error is not False:
             return result
-        self._overwrite_file(file_name, result.response)
+        if not file_not_old(file_name, self.cache_s):
+            self._overwrite_file(file_name, result.response)
         return result
 
     def execute(self, config: RO = False, return_outbound=False) -> R:
         """Runs a rest call with the provided RestObject
 
         Args:
             config (RO, optional): RestObject to determine the REST call,
```

### Comparing `rest_client_micro-0.3.6/src/rest_client_micro/rest_object.py` & `rest_client_micro-0.3.7/src/rest_client_micro/rest_object.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.6/tests/flask_server.py` & `rest_client_micro-0.3.7/tests/flask_server.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.6/tests/test_rest_client.py` & `rest_client_micro-0.3.7/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.6/tests/test_auth/test_auth.py` & `rest_client_micro-0.3.7/tests/test_auth/test_auth.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.6/.gitignore` & `rest_client_micro-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.6/LICENSE` & `rest_client_micro-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.6/README.md` & `rest_client_micro-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.6/PKG-INFO` & `rest_client_micro-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rest_client_micro
-Version: 0.3.6
+Version: 0.3.7
 Summary: A micro rest client
 Author: Samuel Shiels
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11.5
```

