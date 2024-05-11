# Comparing `tmp/tezapi-0.0.4.tar.gz` & `tmp/tezapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tezapi-0.0.4.tar", last modified: Wed May  8 12:30:53 2024, max compression
+gzip compressed data, was "tezapi-0.0.5.tar", last modified: Sat May 11 11:14:00 2024, max compression
```

## Comparing `tezapi-0.0.4.tar` & `tezapi-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 12:30:53.204142 tezapi-0.0.4/
--rw-rw-rw-   0        0        0     1082 2024-05-08 06:46:06.000000 tezapi-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3841 2024-05-08 12:30:53.204142 tezapi-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3224 2024-05-08 12:30:16.000000 tezapi-0.0.4/README.md
--rw-rw-rw-   0        0        0      782 2024-05-08 12:30:43.000000 tezapi-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 12:30:53.204142 tezapi-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 12:30:53.125901 tezapi-0.0.4/tezapi/
--rw-rw-rw-   0        0        0       89 2024-05-08 09:18:11.000000 tezapi-0.0.4/tezapi/__init__.py
--rw-rw-rw-   0        0        0     2192 2024-05-08 11:05:29.000000 tezapi-0.0.4/tezapi/app.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:30:53.204142 tezapi-0.0.4/tezapi/exceptions/
--rw-rw-rw-   0        0        0       65 2024-05-07 20:41:03.000000 tezapi-0.0.4/tezapi/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1376 2024-05-07 21:36:55.000000 tezapi-0.0.4/tezapi/exceptions/apiexception.py
--rw-rw-rw-   0        0        0      215 2024-05-08 08:00:45.000000 tezapi-0.0.4/tezapi/exceptions/base_exceptions.py
--rw-rw-rw-   0        0        0     1394 2024-05-07 19:17:10.000000 tezapi-0.0.4/tezapi/responses.py
--rw-rw-rw-   0        0        0     2474 2024-05-08 12:07:58.000000 tezapi-0.0.4/tezapi/routes.py
--rw-rw-rw-   0        0        0      971 2024-05-08 12:12:02.000000 tezapi-0.0.4/tezapi/schemas.py
--rw-rw-rw-   0        0        0      419 2024-05-08 08:00:45.000000 tezapi-0.0.4/tezapi/templating.py
-drwxrwxrwx   0        0        0        0 2024-05-08 12:30:53.204142 tezapi-0.0.4/tezapi.egg-info/
--rw-rw-rw-   0        0        0     3841 2024-05-08 12:30:53.000000 tezapi-0.0.4/tezapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-05-08 12:30:53.000000 tezapi-0.0.4/tezapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 12:30:53.000000 tezapi-0.0.4/tezapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-08 12:30:53.000000 tezapi-0.0.4/tezapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-08 12:30:53.000000 tezapi-0.0.4/tezapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 11:14:00.084852 tezapi-0.0.5/
+-rw-rw-rw-   0        0        0     1082 2024-05-08 06:46:06.000000 tezapi-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3729 2024-05-11 11:14:00.084852 tezapi-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3112 2024-05-09 13:25:27.000000 tezapi-0.0.5/README.md
+-rw-rw-rw-   0        0        0      782 2024-05-11 11:11:36.000000 tezapi-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 11:14:00.084852 tezapi-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 11:13:59.974580 tezapi-0.0.5/tezapi/
+-rw-rw-rw-   0        0        0       89 2024-05-08 09:18:11.000000 tezapi-0.0.5/tezapi/__init__.py
+-rw-rw-rw-   0        0        0     2175 2024-05-08 12:49:26.000000 tezapi-0.0.5/tezapi/app.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:14:00.084852 tezapi-0.0.5/tezapi/exceptions/
+-rw-rw-rw-   0        0        0       65 2024-05-07 20:41:03.000000 tezapi-0.0.5/tezapi/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1376 2024-05-07 21:36:55.000000 tezapi-0.0.5/tezapi/exceptions/apiexception.py
+-rw-rw-rw-   0        0        0      215 2024-05-08 08:00:45.000000 tezapi-0.0.5/tezapi/exceptions/base_exceptions.py
+-rw-rw-rw-   0        0        0     1526 2024-05-10 16:40:11.000000 tezapi-0.0.5/tezapi/responses.py
+-rw-rw-rw-   0        0        0     2509 2024-05-08 13:45:41.000000 tezapi-0.0.5/tezapi/routes.py
+-rw-rw-rw-   0        0        0      971 2024-05-10 12:19:28.000000 tezapi-0.0.5/tezapi/schemas.py
+-rw-rw-rw-   0        0        0      419 2024-05-08 08:00:45.000000 tezapi-0.0.5/tezapi/templating.py
+drwxrwxrwx   0        0        0        0 2024-05-11 11:14:00.084852 tezapi-0.0.5/tezapi.egg-info/
+-rw-rw-rw-   0        0        0     3729 2024-05-11 11:13:59.000000 tezapi-0.0.5/tezapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-05-11 11:13:59.000000 tezapi-0.0.5/tezapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 11:13:59.000000 tezapi-0.0.5/tezapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-11 11:13:59.000000 tezapi-0.0.5/tezapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-11 11:13:59.000000 tezapi-0.0.5/tezapi.egg-info/top_level.txt
```

### Comparing `tezapi-0.0.4/LICENSE` & `tezapi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.4/PKG-INFO` & `tezapi-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 Metadata-Version: 2.1
 Name: tezapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: Asynchronous web framework for building powerful web APIs and applications with Python
 Author-email: dev-au <devaubusiness@gmail.com>
 Project-URL: Homepage, https://github.com/dev-au/tezapi
 Project-URL: Issues, https://github.com/dev-au/tezapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp~=3.9.5
 Requires-Dist: jinja2~=3.1.4
 
-Certainly! Here's the full README.md file incorporating all the detailed explanations and examples:
-
 # TezAPI
 
-```markdown
 TezAPI is an asynchronous web framework for building powerful and efficient web APIs and applications with Python. It leverages the asyncio and aiohttp libraries to provide a seamless development experience for building high-performance web applications.
 
 ## Key Features
 
 - Asynchronous by design: Built on top of asyncio and aiohttp, TezAPI allows you to write highly concurrent and efficient web applications.
 - Simple and intuitive API: With minimal boilerplate and sensible defaults, TezAPI provides a clean and intuitive API for defining routes and handling requests.
 - Error handling made easy: TezAPI simplifies error handling with support for both simple and class-based error responses, making it straightforward to handle exceptions and provide meaningful feedback to clients.
 - Schema validation with SchemaModel: TezAPI makes form validation easy with the SchemaModel class, allowing you to validate incoming request data against defined schemas effortlessly.
 - Template rendering with Jinja2Template: TezAPI includes built-in support for Jinja2Template, allowing you to render HTML templates seamlessly.
 
 ## Installation
 
-You can install aiohttp-api via pip:
-
+You can install TezAPI via pip:
 
+```commandline
 pip install tezapi
 ```
 
 ## Quick Start
 
 ```python
 from tezapi import TezAPI
@@ -47,15 +44,15 @@
 render = Jinja2Template('templates')
 
 # Define routes and handlers
 @app.get("/")
 async def hello():
     return {'ok': True}
 
-# Run the aiohttp-api application
+# Run the TezAPI application
 app.run()
 ```
 
 ## Advanced Features and Best Practices
 
 In addition to the basic setup and usage, TezAPI offers advanced features and best practices for building robust web applications.
```

### Comparing `tezapi-0.0.4/README.md` & `tezapi-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-Certainly! Here's the full README.md file incorporating all the detailed explanations and examples:
-
 # TezAPI
 
-```markdown
 TezAPI is an asynchronous web framework for building powerful and efficient web APIs and applications with Python. It leverages the asyncio and aiohttp libraries to provide a seamless development experience for building high-performance web applications.
 
 ## Key Features
 
 - Asynchronous by design: Built on top of asyncio and aiohttp, TezAPI allows you to write highly concurrent and efficient web applications.
 - Simple and intuitive API: With minimal boilerplate and sensible defaults, TezAPI provides a clean and intuitive API for defining routes and handling requests.
 - Error handling made easy: TezAPI simplifies error handling with support for both simple and class-based error responses, making it straightforward to handle exceptions and provide meaningful feedback to clients.
 - Schema validation with SchemaModel: TezAPI makes form validation easy with the SchemaModel class, allowing you to validate incoming request data against defined schemas effortlessly.
 - Template rendering with Jinja2Template: TezAPI includes built-in support for Jinja2Template, allowing you to render HTML templates seamlessly.
 
 ## Installation
 
-You can install aiohttp-api via pip:
-
+You can install TezAPI via pip:
 
+```commandline
 pip install tezapi
 ```
 
 ## Quick Start
 
 ```python
 from tezapi import TezAPI
@@ -31,15 +28,15 @@
 render = Jinja2Template('templates')
 
 # Define routes and handlers
 @app.get("/")
 async def hello():
     return {'ok': True}
 
-# Run the aiohttp-api application
+# Run the TezAPI application
 app.run()
 ```
 
 ## Advanced Features and Best Practices
 
 In addition to the basic setup and usage, TezAPI offers advanced features and best practices for building robust web applications.
```

### Comparing `tezapi-0.0.4/pyproject.toml` & `tezapi-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 [project]
 dependencies = [
     "aiohttp~=3.9.5",
     "jinja2~=3.1.4"
 ]
 name = "tezapi"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "dev-au", email = "devaubusiness@gmail.com" },
 ]
 description = "Asynchronous web framework for building powerful web APIs and applications with Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tezapi-0.0.4/tezapi/app.py` & `tezapi-0.0.5/tezapi/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,10 +64,9 @@
         async def run_middleware(request, handler):
             return await func(request, handler)
 
         self.middlewares.append(run_middleware)
         return run_middleware
 
     def run(self):
-        app = self
-        app.add_routes(self.routes)
-        web.run_app(app, host=self.host, port=self.port)
+        self.add_routes(self.routes)
+        web.run_app(self, host=self.host, port=self.port)
```

### Comparing `tezapi-0.0.4/tezapi/exceptions/apiexception.py` & `tezapi-0.0.5/tezapi/exceptions/apiexception.py`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.4/tezapi/responses.py` & `tezapi-0.0.5/tezapi/responses.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,21 @@
     def __init__(self, html_content: str, status_code: int = 200, headers: dict = None):
         super().__init__(content=html_content, status_code=status_code, content_type='text/html',
                          headers=headers)
 
 
 class JSONResponse(Response):
     def __init__(self, json_content: dict, status_code: int = 200, headers: dict = None):
-        json_content = json.dumps(json_content)
-        super().__init__(content=json_content, status_code=status_code, content_type='application/json',
+        json_data = {
+            'error': {
+                'name': None,
+                'message': None
+            },
+            'data': json_content
+        }
+        super().__init__(content=json.dumps(json_data), status_code=status_code, content_type='application/json',
                          headers=headers)
 
 
 class FileResponse:
     def __init__(self, file_path: str, status_code: int = 200, headers: dict = None):
         self.__response__ = _FileResponse(file_path, status=status_code, headers=headers)
```

### Comparing `tezapi-0.0.4/tezapi/routes.py` & `tezapi-0.0.5/tezapi/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,22 +38,22 @@
                 return HTMLResponse(result).__response__
         except APIError as error:
             return error.__response__
         except ClassBaseError as error:
             return error.__response__
 
     async def _request_annotations(self, request: Request):
-        try:
-            json_data = await request.json()
-        except JSONDecodeException:
-            raise JSONDecodeError()
         data = {}
         for key, value in self.arguments.items():
             if issubclass(value, SchemaModel):
-                item = value(json_data)
+                try:
+                    json_data = await request.json()
+                    item = value(json_data)
+                except JSONDecodeException:
+                    raise JSONDecodeError()
             elif value == Request:
                 item = request
             else:
                 item = request.match_info.get(key)
                 if value == int:
                     try:
                         item = int(item)
@@ -62,8 +62,7 @@
                 elif value == float:
                     try:
                         item = float(item)
                     except ValueError:
                         raise APIError('PathValidationError', 400, f'{value.__name__} {key} must be a float')
             data[key] = item
         return data
-
```

### Comparing `tezapi-0.0.4/tezapi/schemas.py` & `tezapi-0.0.5/tezapi/schemas.py`

 * *Files identical despite different names*

### Comparing `tezapi-0.0.4/tezapi.egg-info/PKG-INFO` & `tezapi-0.0.5/tezapi.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 Metadata-Version: 2.1
 Name: tezapi
-Version: 0.0.4
+Version: 0.0.5
 Summary: Asynchronous web framework for building powerful web APIs and applications with Python
 Author-email: dev-au <devaubusiness@gmail.com>
 Project-URL: Homepage, https://github.com/dev-au/tezapi
 Project-URL: Issues, https://github.com/dev-au/tezapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp~=3.9.5
 Requires-Dist: jinja2~=3.1.4
 
-Certainly! Here's the full README.md file incorporating all the detailed explanations and examples:
-
 # TezAPI
 
-```markdown
 TezAPI is an asynchronous web framework for building powerful and efficient web APIs and applications with Python. It leverages the asyncio and aiohttp libraries to provide a seamless development experience for building high-performance web applications.
 
 ## Key Features
 
 - Asynchronous by design: Built on top of asyncio and aiohttp, TezAPI allows you to write highly concurrent and efficient web applications.
 - Simple and intuitive API: With minimal boilerplate and sensible defaults, TezAPI provides a clean and intuitive API for defining routes and handling requests.
 - Error handling made easy: TezAPI simplifies error handling with support for both simple and class-based error responses, making it straightforward to handle exceptions and provide meaningful feedback to clients.
 - Schema validation with SchemaModel: TezAPI makes form validation easy with the SchemaModel class, allowing you to validate incoming request data against defined schemas effortlessly.
 - Template rendering with Jinja2Template: TezAPI includes built-in support for Jinja2Template, allowing you to render HTML templates seamlessly.
 
 ## Installation
 
-You can install aiohttp-api via pip:
-
+You can install TezAPI via pip:
 
+```commandline
 pip install tezapi
 ```
 
 ## Quick Start
 
 ```python
 from tezapi import TezAPI
@@ -47,15 +44,15 @@
 render = Jinja2Template('templates')
 
 # Define routes and handlers
 @app.get("/")
 async def hello():
     return {'ok': True}
 
-# Run the aiohttp-api application
+# Run the TezAPI application
 app.run()
 ```
 
 ## Advanced Features and Best Practices
 
 In addition to the basic setup and usage, TezAPI offers advanced features and best practices for building robust web applications.
```

