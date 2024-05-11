# Comparing `tmp/rest_client_micro-0.3.8.tar.gz` & `tmp/rest_client_micro-0.3.9.tar.gz`

## Comparing `rest_client_micro-0.3.8.tar` & `rest_client_micro-0.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/src/rest_client_micro/__init__.py
--rwxr-xr-x   0        0        0     1026 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/src/rest_client_micro/_utils.py
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/src/rest_client_micro/basic_auth.py
--rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/src/rest_client_micro/response.py
--rwxr-xr-x   0        0        0     7227 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/src/rest_client_micro/rest_client.py
--rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/src/rest_client_micro/rest_object.py
--rwxr-xr-x   0        0        0     1247 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/tests/flask_server.py
--rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/tests/test_rest_client.py
--rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/tests/test_auth/test_auth.py
--rwxr-xr-x   0        0        0     1852 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/.gitignore
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/LICENSE
--rwxr-xr-x   0        0        0     1421 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/README.md
--rwxr-xr-x   0        0        0      426 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 rest_client_micro-0.3.8/PKG-INFO
+-rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/src/rest_client_micro/__init__.py
+-rwxr-xr-x   0        0        0     1026 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/src/rest_client_micro/_utils.py
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/src/rest_client_micro/basic_auth.py
+-rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/src/rest_client_micro/response.py
+-rwxr-xr-x   0        0        0     7239 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/src/rest_client_micro/rest_client.py
+-rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/src/rest_client_micro/rest_object.py
+-rwxr-xr-x   0        0        0     1247 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/tests/flask_server.py
+-rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/tests/test_rest_client.py
+-rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/tests/test_auth/test_auth.py
+-rwxr-xr-x   0        0        0     1852 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/.gitignore
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/LICENSE
+-rwxr-xr-x   0        0        0     1421 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/README.md
+-rwxr-xr-x   0        0        0      426 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 rest_client_micro-0.3.9/PKG-INFO
```

### Comparing `rest_client_micro-0.3.8/src/rest_client_micro/_utils.py` & `rest_client_micro-0.3.9/src/rest_client_micro/_utils.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.8/src/rest_client_micro/response.py` & `rest_client_micro-0.3.9/src/rest_client_micro/response.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.8/src/rest_client_micro/rest_client.py` & `rest_client_micro-0.3.9/src/rest_client_micro/rest_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,18 +171,18 @@
             will only return the result of the rest call. Defaults to False.
 
         Returns:
             R: Response object, use `error` property to check if call was successful
         """
         self._debug("retrieve_file " + config.endpoint + " - " + file_name)
         config.operation = "file"
-        result = self._execute_call(config)
-        if result.error is not False:
-            return result
         if not file_not_old(file_name, self.cache_s):
+            result = self._execute_call(config)
+            if result.error is not False:
+                return result
             self._overwrite_file(file_name, result.response)
         return result
 
     def execute(self, config: RO = False, return_outbound=False) -> R:
         """Runs a rest call with the provided RestObject
 
         Args:
```

### Comparing `rest_client_micro-0.3.8/src/rest_client_micro/rest_object.py` & `rest_client_micro-0.3.9/src/rest_client_micro/rest_object.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.8/tests/flask_server.py` & `rest_client_micro-0.3.9/tests/flask_server.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.8/tests/test_rest_client.py` & `rest_client_micro-0.3.9/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.8/tests/test_auth/test_auth.py` & `rest_client_micro-0.3.9/tests/test_auth/test_auth.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.8/.gitignore` & `rest_client_micro-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.8/LICENSE` & `rest_client_micro-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.8/README.md` & `rest_client_micro-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.8/PKG-INFO` & `rest_client_micro-0.3.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rest_client_micro
-Version: 0.3.8
+Version: 0.3.9
 Summary: A micro rest client
 Author: Samuel Shiels
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11.5
```

