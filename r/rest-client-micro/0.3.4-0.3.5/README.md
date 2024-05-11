# Comparing `tmp/rest_client_micro-0.3.4.tar.gz` & `tmp/rest_client_micro-0.3.5.tar.gz`

## Comparing `rest_client_micro-0.3.4.tar` & `rest_client_micro-0.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/src/rest_client_micro/__init__.py
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/src/rest_client_micro/basic_auth.py
--rwxr-xr-x   0        0        0      362 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/src/rest_client_micro/response.py
--rwxr-xr-x   0        0        0     4318 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/src/rest_client_micro/rest_client.py
--rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/src/rest_client_micro/rest_object.py
--rwxr-xr-x   0        0        0     1247 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/tests/flask_server.py
--rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/tests/test_rest_client.py
--rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/tests/test_auth/test_auth.py
--rwxr-xr-x   0        0        0     1852 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/.gitignore
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/LICENSE
--rwxr-xr-x   0        0        0     1421 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/README.md
--rwxr-xr-x   0        0        0      426 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 rest_client_micro-0.3.4/PKG-INFO
+-rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 rest_client_micro-0.3.5/src/rest_client_micro/__init__.py
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 rest_client_micro-0.3.5/src/rest_client_micro/basic_auth.py
+-rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 rest_client_micro-0.3.5/src/rest_client_micro/response.py
+-rwxr-xr-x   0        0        0     4503 2020-02-02 00:00:00.000000 rest_client_micro-0.3.5/src/rest_client_micro/rest_client.py
+-rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 rest_client_micro-0.3.5/src/rest_client_micro/rest_object.py
+-rwxr-xr-x   0        0        0     1247 2020-02-02 00:00:00.000000 rest_client_micro-0.3.5/tests/flask_server.py
+-rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 rest_client_micro-0.3.5/tests/test_rest_client.py
+-rwxr-xr-x   0        0        0      882 2020-02-02 00:00:00.000000 rest_client_micro-0.3.5/tests/test_auth/test_auth.py
+-rwxr-xr-x   0        0        0     1852 2020-02-02 00:00:00.000000 rest_client_micro-0.3.5/.gitignore
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 rest_client_micro-0.3.5/LICENSE
+-rwxr-xr-x   0        0        0     1421 2020-02-02 00:00:00.000000 rest_client_micro-0.3.5/README.md
+-rwxr-xr-x   0        0        0      426 2020-02-02 00:00:00.000000 rest_client_micro-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 rest_client_micro-0.3.5/PKG-INFO
```

### Comparing `rest_client_micro-0.3.4/src/rest_client_micro/rest_client.py` & `rest_client_micro-0.3.5/src/rest_client_micro/rest_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,34 +76,38 @@
                     headers=headers,
                     data=payload,
                     timeout=10,
                     auth=auth
                 )
                 if response.status_code in rest_object.error_status:
                     return R(
+                        endpoint=endpoint,
                         error=True,
                         response=response.text,
                         status=response.status_code,
                         outbound=payload
                     )
                 else:
                     return R(
+                        endpoint=endpoint,
                         error=False,
                         response=response.text,
                         status=response.status_code,
                         outbound=payload
                     )
             return R(
+                endpoint=endpoint,
                 error=True,
                 error_text='REST Operation not supported or valid',
 
             )
 
         except Exception as e:
             return R(
+                endpoint=endpoint,
                 error=True,
                 error_text=str(e),
             )
 
     def _read_cache(self, config: RO) -> str:
         pass
 
@@ -123,12 +127,13 @@
             will only return the result of the rest call. Defaults to False.
 
         Returns:
             R: Response object, use `error` property to check if call was successful
         """
         if not config:
             return R(
+                endpoint="",
                 error=True,
                 error_text='RESTObject config not provided'
             )
 
         return self._execute_call(config, return_outbound=return_outbound)
```

### Comparing `rest_client_micro-0.3.4/src/rest_client_micro/rest_object.py` & `rest_client_micro-0.3.5/src/rest_client_micro/rest_object.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.4/tests/flask_server.py` & `rest_client_micro-0.3.5/tests/flask_server.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.4/tests/test_rest_client.py` & `rest_client_micro-0.3.5/tests/test_rest_client.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.4/tests/test_auth/test_auth.py` & `rest_client_micro-0.3.5/tests/test_auth/test_auth.py`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.4/.gitignore` & `rest_client_micro-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.4/LICENSE` & `rest_client_micro-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.4/README.md` & `rest_client_micro-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `rest_client_micro-0.3.4/PKG-INFO` & `rest_client_micro-0.3.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rest_client_micro
-Version: 0.3.4
+Version: 0.3.5
 Summary: A micro rest client
 Author: Samuel Shiels
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11.5
```

