# Comparing `tmp/iudex-0.4.4.tar.gz` & `tmp/iudex-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.4.4.tar", max compression
+gzip compressed data, was "iudex-0.4.5.tar", max compression
```

## Comparing `iudex-0.4.4.tar` & `iudex-0.4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.4.4/LICENSE
--rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.4.4/README.md
--rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.4.4/iudex/__init__.py
--rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.4.4/iudex/chat.py
--rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.4.4/iudex/client.py
--rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.4.4/iudex/functions.py
--rw-r--r--   0        0        0     1483 2024-05-09 22:16:04.387303 iudex-0.4.4/iudex/instrumentation/README.md
--rw-r--r--   0        0        0      106 2024-05-10 08:08:22.984691 iudex-0.4.4/iudex/instrumentation/__init__.py
--rw-r--r--   0        0        0     2821 2024-05-10 17:33:40.765835 iudex-0.4.4/iudex/instrumentation/attributes.py
--rw-r--r--   0        0        0     1622 2024-05-10 08:08:22.984691 iudex-0.4.4/iudex/instrumentation/fastapi.py
--rw-r--r--   0        0        0     5001 2024-05-10 09:50:14.706611 iudex-0.4.4/iudex/instrumentation/instrumentation.py
--rw-r--r--   0        0        0     1165 2024-05-10 08:08:22.984691 iudex-0.4.4/iudex/instrumentation/lambda.py
--rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.4.4/iudex/resource.py
--rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.4.4/iudex/types/function.py
--rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.4.4/iudex/utils.py
--rw-r--r--   0        0        0      667 2024-05-10 17:33:52.285815 iudex-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.4.5/LICENSE
+-rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.4.5/README.md
+-rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.4.5/iudex/__init__.py
+-rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.4.5/iudex/chat.py
+-rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.4.5/iudex/client.py
+-rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.4.5/iudex/functions.py
+-rw-r--r--   0        0        0     1402 2024-05-10 18:23:20.390624 iudex-0.4.5/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0      106 2024-05-10 08:08:22.984691 iudex-0.4.5/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-10 17:33:40.765835 iudex-0.4.5/iudex/instrumentation/attributes.py
+-rw-r--r--   0        0        0     1790 2024-05-10 18:18:05.655854 iudex-0.4.5/iudex/instrumentation/fastapi.py
+-rw-r--r--   0        0        0     5001 2024-05-10 09:50:14.706611 iudex-0.4.5/iudex/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0     1333 2024-05-10 18:18:35.037024 iudex-0.4.5/iudex/instrumentation/lambda.py
+-rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.4.5/iudex/resource.py
+-rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.4.5/iudex/types/function.py
+-rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.4.5/iudex/utils.py
+-rw-r--r--   0        0        0      667 2024-05-10 18:19:49.494609 iudex-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.5/PKG-INFO
```

### Comparing `iudex-0.4.4/LICENSE` & `iudex-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.4.4/README.md` & `iudex-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.4.4/iudex/chat.py` & `iudex-0.4.5/iudex/chat.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.4/iudex/client.py` & `iudex-0.4.5/iudex/client.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.4/iudex/functions.py` & `iudex-0.4.5/iudex/functions.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.4/iudex/instrumentation/README.md` & `iudex-0.4.5/iudex/instrumentation/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-To instrument IUDEX you need to prep 2 things, code and environment variables
+Instrumenting your Python service to send logs to Iudex just takes a few steps.
 
 # FastAPI
 
 1. Pip install dependencies
 ```bash
 pip install iudex
 ```
-2. Import `instrument_app` where you defined FastAPI (usually `main.py`) from `iudex`
+2. Import `instrument` where you defined FastAPI (usually `main.py`) from `iudex`
 ```python
 # Add this
-from iudex.instrumentation.fastapi_instrumentation import instrument_app
+from iudex.instrumentation.fastapi import instrument
 
 # Find this in your code base
 app = FastAPI()
 
 # Add this
-instrument_app(app=app, api_key=os.getenv("IUDEX_API_KEY"), service_name=__main__)
+instrument(
+  app=app,
+  service_name=__name__, # or any string describing your service
+)
 ```
 3. Make sure the app has access to the environment variable `IUDEX_API_KEY`
 4. You should be all set! Go to [https://app.iudex.ai/](https://app.iudex.ai/) and enter your API key
 5. Go to [https://app.iudex.ai/logs](https://app.iudex.ai/logs) and press `Search` to view your logs
 
 
 # Lambda / Serverless
 
 1. Pip install dependencies
 ```bash
 pip install iudex
 ```
-2. Import `instrument_app` from `iudex` and invoke it in your entrypoint (usually `main.py`)
+2. Import `instrument` from `iudex` and invoke it in your entrypoint (usually `main.py`)
 ```python
 # Add this in your lambda function file (likely lambda_function.py)
-from iudex.instrumentation.lambda_instrumentation import instrument_app
-instrument_app(
-  api_key=os.getenv("IUDEX_API_KEY"),
+from iudex.instrumentation.lambda import instrument
+instrument(
   service_name=__name__, # or any string describing your service
 )
 ```
 3. Make sure the app has access to the environment variable `IUDEX_API_KEY`
 4. You should be all set! Go to [https://app.iudex.ai/](https://app.iudex.ai/) and enter your API key
 5. Go to [https://app.iudex.ai/logs](https://app.iudex.ai/logs) and press `Search` to view your logs
```

### Comparing `iudex-0.4.4/iudex/instrumentation/attributes.py` & `iudex-0.4.5/iudex/instrumentation/attributes.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.4/iudex/instrumentation/fastapi.py` & `iudex-0.4.5/iudex/instrumentation/fastapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import Optional
+from typing import Optional, Union
 
 from fastapi import FastAPI
 from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
 
 from .instrumentation import IudexConfig
 
 
 def instrument(
     app: FastAPI,
     service_name: Optional[str] = None,
     instance_id: Optional[str] = None,
     iudex_api_key: Optional[str] = None,
+    log_level: Optional[Union[int, str]] = None,
     config: Optional[IudexConfig] = None,
 ):
     """Auto-instruments FastAPI app to send OTel signals to Iudex.
 
     Invoke this function in your FastAPI entrypoint.
 
     If you use Gunicorn, invoke it within a post_fork hook:
@@ -27,23 +28,26 @@
     Args:
         app: FastAPI app to instrument.
         service_name: Name of the service, e.g. "billing_service", __name__.
             If not supplied, env var OTEL_SERVICE_NAME will be used.
         instance_id: ID of the service instance, e.g. container id, pod name.
         iudex_api_key: Your Iudex API key.
             If not supplied, env var IUDEX_API_KEY will be used.
+        log_level: Logging level for the root logger.
         config: IudexConfig object with more granular options.
             Will override all other args, so provide them to the object instead.
     """
     kwargs = {}
     if service_name:
         kwargs["service_name"] = service_name
     if instance_id:
         kwargs["instance_id"] = instance_id
     if iudex_api_key:
         kwargs["iudex_api_key"] = iudex_api_key
+    if log_level:
+        kwargs["log_level"] = log_level
     config = config or IudexConfig(**kwargs)
 
     config.configure()
     FastAPIInstrumentor().instrument_app(app)
 
     return config
```

### Comparing `iudex-0.4.4/iudex/instrumentation/instrumentation.py` & `iudex-0.4.5/iudex/instrumentation/instrumentation.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.4/iudex/instrumentation/lambda.py` & `iudex-0.4.5/iudex/instrumentation/lambda.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from typing import Optional
+from typing import Optional, Union
 
 from .instrumentation import IudexConfig
 
 
 def instrument(
     service_name: Optional[str] = None,
     instance_id: Optional[str] = None,
     iudex_api_key: Optional[str] = None,
+    log_level: Optional[Union[int, str]] = None,
     config: Optional[IudexConfig] = None,
 ):
     """Auto-instruments app to send OTel signals to Iudex.
 
     Invoke this function in your Lambda entrypoint.
 
     Args:
         service_name: Name of the service, e.g. "billing_service", __name__.
             If not supplied, env var OTEL_SERVICE_NAME will be used.
         instance_id: ID of the service instance, e.g. container id, pod name.
         iudex_api_key: Your Iudex API key.
             If not supplied, env var IUDEX_API_KEY will be used.
+        log_level: Logging level for the root logger.
         config: IudexConfig object with more granular options.
             Will override all other args, so provide them to the object instead.
     """
     kwargs = {}
     if service_name:
         kwargs["service_name"] = service_name
     if instance_id:
         kwargs["instance_id"] = instance_id
     if iudex_api_key:
         kwargs["iudex_api_key"] = iudex_api_key
+    if log_level:
+        kwargs["log_level"] = log_level
     config = config or IudexConfig(**kwargs)
 
     config.configure()
 
     return config
```

### Comparing `iudex-0.4.4/iudex/types/function.py` & `iudex-0.4.5/iudex/types/function.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.4/pyproject.toml` & `iudex-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iudex"
-version = "0.4.4"
+version = "0.4.5"
 description = ""
 authors = ["Drake Wong <drake@iudex.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^1.12.0"
```

### Comparing `iudex-0.4.4/PKG-INFO` & `iudex-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iudex
-Version: 0.4.4
+Version: 0.4.5
 Summary: 
 Author: Drake Wong
 Author-email: drake@iudex.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

