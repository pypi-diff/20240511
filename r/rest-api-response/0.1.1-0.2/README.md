# Comparing `tmp/rest_api_response-0.1.1.tar.gz` & `tmp/rest_api_response-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_api_response-0.1.1.tar", last modified: Wed Jun 28 12:06:57 2023, max compression
+gzip compressed data, was "rest_api_response-0.2.tar", last modified: Sat May 11 18:09:09 2024, max compression
```

## Comparing `rest_api_response-0.1.1.tar` & `rest_api_response-0.2.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:06:57.354719 rest_api_response-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-28 12:06:44.000000 rest_api_response-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-28 12:06:57.354719 rest_api_response-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-28 12:06:44.000000 rest_api_response-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-28 12:06:44.000000 rest_api_response-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:06:57.354719 rest_api_response-0.1.1/rest_api_response/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-28 12:06:44.000000 rest_api_response-0.1.1/rest_api_response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:06:57.354719 rest_api_response-0.1.1/rest_api_response.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-28 12:06:57.000000 rest_api_response-0.1.1/rest_api_response.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-28 12:06:57.000000 rest_api_response-0.1.1/rest_api_response.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 12:06:57.000000 rest_api_response-0.1.1/rest_api_response.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-28 12:06:57.000000 rest_api_response-0.1.1/rest_api_response.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-28 12:06:57.354719 rest_api_response-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-28 12:06:44.000000 rest_api_response-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:06:57.354719 rest_api_response-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:06:44.000000 rest_api_response-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-28 12:06:44.000000 rest_api_response-0.1.1/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:09:09.870139 rest_api_response-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-11 18:09:05.000000 rest_api_response-0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-11 18:09:09.870139 rest_api_response-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-11 18:09:05.000000 rest_api_response-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-11 18:09:05.000000 rest_api_response-0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:09:09.870139 rest_api_response-0.2/rest_api_response/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-11 18:09:05.000000 rest_api_response-0.2/rest_api_response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-11 18:09:05.000000 rest_api_response-0.2/rest_api_response/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 18:09:09.870139 rest_api_response-0.2/rest_api_response.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-11 18:09:09.000000 rest_api_response-0.2/rest_api_response.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-11 18:09:09.000000 rest_api_response-0.2/rest_api_response.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 18:09:09.000000 rest_api_response-0.2/rest_api_response.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-11 18:09:09.000000 rest_api_response-0.2/rest_api_response.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-11 18:09:09.870139 rest_api_response-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-11 18:09:05.000000 rest_api_response-0.2/setup.py
```

### Comparing `rest_api_response-0.1.1/LICENSE.txt` & `rest_api_response-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rest_api_response-0.1.1/PKG-INFO` & `rest_api_response-0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,11 @@
-Metadata-Version: 2.1
-Name: rest_api_response
-Version: 0.1.1
-Summary: A go-to production API response with an easy format for building APIs with Python.
-Home-page: https://github.com/aybruhm/api-response
-Author: Abram
-Author-email: israelvictory87@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/aybruhm/api-response/issues
-Keywords: api,response,custom api response
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Production API Response
 
+[![Package Code Quality](https://github.com/aybruhm/api-response/actions/workflows/package-test.yml/badge.svg)](https://github.com/aybruhm/api-response/actions/workflows/package-test.yml) [![Package Published to PypI](https://github.com/aybruhm/api-response/actions/workflows/package-publish.yml/badge.svg)](https://github.com/aybruhm/api-response/actions/workflows/package-publish.yml)
+
 A go-to production API response with an easy format for building APIs with Python.
 
 ## Quickstart
 
 To get it running, follow the steps below:
 
 1). Pip install the package in your project terminal:
```

### Comparing `rest_api_response-0.1.1/rest_api_response/__init__.py` & `rest_api_response-0.2/rest_api_response/responses.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# Typing Imports
-from typing import Dict, Union
+# Stdlib Imports
+from typing import Dict, Union, List, Any
 
 
-def error_response(
-    message: str, meta: dict = {}
-) -> Dict[str, Union[bool, str, dict]]:
+def error_response(message: str, meta: dict = {}) -> Dict[str, Any]:
     """
     Custom error response
 
     :param message: The error message you want to send to the user
     :type message: str
 
     :param meta: Additional information/context to the error
@@ -19,25 +17,24 @@
     """
 
     response = {"status": False, "message": message, "meta": meta}
     return response
 
 
 def success_response(
-    message: str, data: dict = {}
-) -> Dict[str, Union[bool, str, dict]]:
+    message: str, data: Union[List[Any], Dict[str, Any]] = {}
+) -> Dict[str, Any]:
     """
     Custom success response
 
     :param message: The success message you want to send to the user
     :type message: str
 
     :param data: Data that you would be returned to the client
-    :type data: dict
+    :type data: dict or list
 
     :return: response
     :rtype: dict
     """
 
     response = {"status": True, "message": message, "data": data}
     return response
-
```

### Comparing `rest_api_response-0.1.1/rest_api_response.egg-info/PKG-INFO` & `rest_api_response-0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: rest-api-response
-Version: 0.1.1
+Name: rest_api_response
+Version: 0.2
 Summary: A go-to production API response with an easy format for building APIs with Python.
 Home-page: https://github.com/aybruhm/api-response
-Author: Abram
+Author: Abraham 'Abram' Israel
 Author-email: israelvictory87@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/aybruhm/api-response/issues
 Keywords: api,response,custom api response
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Production API Response
 
+[![Package Code Quality](https://github.com/aybruhm/api-response/actions/workflows/package-test.yml/badge.svg)](https://github.com/aybruhm/api-response/actions/workflows/package-test.yml) [![Package Published to PypI](https://github.com/aybruhm/api-response/actions/workflows/package-publish.yml/badge.svg)](https://github.com/aybruhm/api-response/actions/workflows/package-publish.yml)
+
 A go-to production API response with an easy format for building APIs with Python.
 
 ## Quickstart
 
 To get it running, follow the steps below:
 
 1). Pip install the package in your project terminal:
```

### Comparing `rest_api_response-0.1.1/setup.cfg` & `rest_api_response-0.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rest-api-response
-version = 0.1.1
+version = 0.2
 author = Abram
 author_email = israelvictory87@gmail.com
 description = A go-to production API response with an easy format for building APIs with Python.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/aybruhm/api-response
 project_urls =
```

### Comparing `rest_api_response-0.1.1/setup.py` & `rest_api_response-0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 
 setup(
     name="rest_api_response",
-    version="0.1.1",
+    version="0.2",
     description="A go-to production API response with an easy format for building APIs with Python.", # noqa: E501
     long_description_content_type="text/markdown",
     long_description=open("README.md").read(),
     url="https://github.com/aybruhm/api-response",
-    author="Abram",
+    author="Abraham 'Abram' Israel",
     author_email="israelvictory87@gmail.com",
     license="MIT",
     classifiers=classifiers,
     keywords=["api", "response", "custom api response"],
     packages=find_packages(),
 )
```

