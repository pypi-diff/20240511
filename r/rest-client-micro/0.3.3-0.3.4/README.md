# Comparing `tmp/rest_client_micro-0.3.3.tar.gz` & `tmp/rest_client_micro-0.3.4.tar.gz`

## Comparing `rest_client_micro-0.3.3.tar` & `rest_client_micro-0.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 rest_client_micro-0.3.3/src/rest_client_micro/__init__.py
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 rest_client_micro-0.3.3/src/rest_client_micro/basic_auth.py
--rwxr-xr-x   0        0        0      362 2020-02-02 00:00:00.000000 rest_client_micro-0.3.3/src/rest_client_micro/response.py
--rwxr-xr-x   0        0        0     3516 2020-02-02 00:00:00.000000 rest_client_micro-0.3.3/src/rest_client_micro/rest_client.py
--rwxr-xr-x   0        0        0      554 2020-02-02 00:00:00.000000 rest_client_micro-0.3.3/src/rest_client_micro/rest_object.py
--rwxr-xr-x   0        0        0     1247 2020-02-02 00:00:00.000000 rest_client_micro-0.3.3/tests/flask_server.py
--rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 rest_client_micro-0.3.3/tests/test_rest_client.py
--rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 rest_client_micro-0.3.3/tests/test_auth/test_auth.py
--rwxr-xr-x   0        0        0     1852 2020-02-02 00:00:00.000000 rest_client_micro-0.3.3/.gitignore
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 rest_client_micro-0.3.3/LICENSE
--rwxr-xr-x   0        0        0     1421 2020-02-02 00:00:00.000000 rest_client_micro-0.3.3/README.md
--rwxr-xr-x   0        0        0      426 2020-02-02 00:00:00.000000 rest_client_micro-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 rest_client_micro-0.3.3/PKG-INFO
+-rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/src/rest_client_micro/__init__.py
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/src/rest_client_micro/basic_auth.py
+-rwxr-xr-x   0        0        0      362 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/src/rest_client_micro/response.py
+-rwxr-xr-x   0        0        0     4318 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/src/rest_client_micro/rest_client.py
+-rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/src/rest_client_micro/rest_object.py
+-rwxr-xr-x   0        0        0     1247 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/tests/flask_server.py
+-rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/tests/test_rest_client.py
+-rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/tests/test_auth/test_auth.py
+-rwxr-xr-x   0        0        0     1852 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/.gitignore
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/LICENSE
+-rwxr-xr-x   0        0        0     1421 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/README.md
+-rwxr-xr-x   0        0        0      426 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/PKG-INFO
```

### Comparing `rest_client_micro-0.3.3/src/rest_client_micro/rest_client.py` & `rest_client_micro-0.3.4/src/rest_client_micro/rest_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,32 +16,30 @@
 class RESTClient():
     """
     Wrapper class for requests calls
     """
 
     logging.basicConfig(
         format='%(asctime)s | %(levelname)s | %(message)s', level=logging.DEBUG)
-    DEBUG = False
     __app_name = 'rest_client_micro'
     root_dir: str
     output_file: str
-    cache_dir: str = os.path.join(
+    config_dir: str = os.path.join(
         str(Path.home()), ".config/", __app_name)
     cache_file: str = os.path.join(
         str(Path.home()), ".cache/", __app_name, "app")
     log_dir: str = os.path.join(
         str(Path.home()), ".cache/", __app_name, "logs")
     log_file: str = "log.db"
 
     cache_s: int = 600
     sleep_ms: int = 1000
 
     def _debug(self, message):
-        if self.DEBUG:
-            logging.debug(str(message))
+        logging.debug(str(message))
 
     def __init__(self) -> None:
         pass
 
     def _get_short_string(self, content):
         if len(str(content)) < 110:
             return content
@@ -76,20 +74,28 @@
                     url=endpoint,
                     params=params,
                     headers=headers,
                     data=payload,
                     timeout=10,
                     auth=auth
                 )
-                return R(
-                    error=False,
-                    response=response.text,
-                    status=response.status_code,
-                    outbound=payload
-                )
+                if response.status_code in rest_object.error_status:
+                    return R(
+                        error=True,
+                        response=response.text,
+                        status=response.status_code,
+                        outbound=payload
+                    )
+                else:
+                    return R(
+                        error=False,
+                        response=response.text,
+                        status=response.status_code,
+                        outbound=payload
+                    )
             return R(
                 error=True,
                 error_text='REST Operation not supported or valid',
 
             )
 
         except Exception as e:
@@ -104,14 +110,25 @@
     def _write_cache(self, config: RO, text: str) -> None:
         pass
 
     def _set_cache(self, config: RO) -> None:
         pass
 
     def execute(self, config: RO = False, return_outbound=False) -> R:
+        """Runs a rest call with the provided RestObject
+
+        Args:
+            config (RO, optional): RestObject to determine the REST call, 
+            if not provided will return an error Response. Defaults to False.
+            return_outbound (bool, optional): Returns the outbound call, otherwise 
+            will only return the result of the rest call. Defaults to False.
+
+        Returns:
+            R: Response object, use `error` property to check if call was successful
+        """
         if not config:
             return R(
                 error=True,
                 error_text='RESTObject config not provided'
             )
 
         return self._execute_call(config, return_outbound=return_outbound)
```

### Comparing `rest_client_micro-0.3.3/src/rest_client_micro/rest_object.py` & `rest_client_micro-0.3.4/src/rest_client_micro/rest_object.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 
     operation: str
     endpoint: str
     params: dict
     headers: dict
     payload: str
     basic_auth: BasicAuth
+    error_status: list[int]
 
     def __init__(self, **kwargs) -> None:
         self.operation = 'get'
         self.params = {}
         self.payload = ''
         self.headers = {}
         self.basic_auth = None
+        self.error_status = [403, 404, ]
         self.__dict__.update(kwargs)
```

### Comparing `rest_client_micro-0.3.3/tests/flask_server.py` & `rest_client_micro-0.3.4/tests/flask_server.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.3/tests/test_rest_client.py` & `rest_client_micro-0.3.4/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.3/tests/test_auth/test_auth.py` & `rest_client_micro-0.3.4/tests/test_auth/test_auth.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.3/.gitignore` & `rest_client_micro-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.3/LICENSE` & `rest_client_micro-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.3/README.md` & `rest_client_micro-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.3/PKG-INFO` & `rest_client_micro-0.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rest_client_micro
-Version: 0.3.3
+Version: 0.3.4
 Summary: A micro rest client
 Author: Samuel Shiels
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11.5
```

