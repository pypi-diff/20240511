# Comparing `tmp/iudex-0.4.5.tar.gz` & `tmp/iudex-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iudex-0.4.5.tar", max compression
+gzip compressed data, was "iudex-0.4.6.tar", max compression
```

## Comparing `iudex-0.4.5.tar` & `iudex-0.4.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-02-22 09:17:28.247197 iudex-0.4.5/LICENSE
--rw-r--r--   0        0        0     8426 2024-05-09 16:32:45.684025 iudex-0.4.5/README.md
--rw-r--r--   0        0        0       54 2024-02-22 09:17:28.247197 iudex-0.4.5/iudex/__init__.py
--rw-r--r--   0        0        0     7348 2024-03-20 10:03:47.436645 iudex-0.4.5/iudex/chat.py
--rw-r--r--   0        0        0     7295 2024-03-20 10:04:00.926644 iudex-0.4.5/iudex/client.py
--rw-r--r--   0        0        0     1653 2024-03-18 08:25:33.730610 iudex-0.4.5/iudex/functions.py
--rw-r--r--   0        0        0     1402 2024-05-10 18:23:20.390624 iudex-0.4.5/iudex/instrumentation/README.md
--rw-r--r--   0        0        0      106 2024-05-10 08:08:22.984691 iudex-0.4.5/iudex/instrumentation/__init__.py
--rw-r--r--   0        0        0     2821 2024-05-10 17:33:40.765835 iudex-0.4.5/iudex/instrumentation/attributes.py
--rw-r--r--   0        0        0     1790 2024-05-10 18:18:05.655854 iudex-0.4.5/iudex/instrumentation/fastapi.py
--rw-r--r--   0        0        0     5001 2024-05-10 09:50:14.706611 iudex-0.4.5/iudex/instrumentation/instrumentation.py
--rw-r--r--   0        0        0     1333 2024-05-10 18:18:35.037024 iudex-0.4.5/iudex/instrumentation/lambda.py
--rw-r--r--   0        0        0      236 2024-03-03 21:45:43.952527 iudex-0.4.5/iudex/resource.py
--rw-r--r--   0        0        0     4349 2024-03-18 08:25:33.730610 iudex-0.4.5/iudex/types/function.py
--rw-r--r--   0        0        0      137 2024-03-13 08:12:55.353436 iudex-0.4.5/iudex/utils.py
--rw-r--r--   0        0        0      667 2024-05-10 18:19:49.494609 iudex-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-05 02:32:42.683184 iudex-0.4.6/LICENSE
+-rw-r--r--   0        0        0     8426 2024-05-07 17:48:23.958486 iudex-0.4.6/README.md
+-rw-r--r--   0        0        0       54 2024-03-05 02:32:42.685374 iudex-0.4.6/iudex/__init__.py
+-rw-r--r--   0        0        0     7348 2024-03-22 23:11:09.655241 iudex-0.4.6/iudex/chat.py
+-rw-r--r--   0        0        0     7295 2024-03-22 23:11:09.655456 iudex-0.4.6/iudex/client.py
+-rw-r--r--   0        0        0     1653 2024-03-22 23:11:09.655988 iudex-0.4.6/iudex/functions.py
+-rw-r--r--   0        0        0     1402 2024-05-10 22:37:34.746644 iudex-0.4.6/iudex/instrumentation/README.md
+-rw-r--r--   0        0        0      136 2024-05-11 00:45:08.006406 iudex-0.4.6/iudex/instrumentation/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-10 22:37:34.746966 iudex-0.4.6/iudex/instrumentation/attributes.py
+-rw-r--r--   0        0        0     2010 2024-05-11 00:45:08.006569 iudex-0.4.6/iudex/instrumentation/fastapi.py
+-rw-r--r--   0        0        0     5729 2024-05-11 00:45:10.635897 iudex-0.4.6/iudex/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0     1461 2024-05-11 00:45:08.006873 iudex-0.4.6/iudex/instrumentation/lambda.py
+-rw-r--r--   0        0        0      236 2024-03-05 02:32:42.686766 iudex-0.4.6/iudex/resource.py
+-rw-r--r--   0        0        0     4349 2024-03-22 23:11:09.656442 iudex-0.4.6/iudex/types/function.py
+-rw-r--r--   0        0        0      137 2024-03-06 19:49:41.321305 iudex-0.4.6/iudex/utils.py
+-rw-r--r--   0        0        0      667 2024-05-11 00:45:08.007156 iudex-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     9170 1970-01-01 00:00:00.000000 iudex-0.4.6/PKG-INFO
```

### Comparing `iudex-0.4.5/LICENSE` & `iudex-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iudex-0.4.5/README.md` & `iudex-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.4.5/iudex/chat.py` & `iudex-0.4.6/iudex/chat.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.5/iudex/client.py` & `iudex-0.4.6/iudex/client.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.5/iudex/functions.py` & `iudex-0.4.6/iudex/functions.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.5/iudex/instrumentation/README.md` & `iudex-0.4.6/iudex/instrumentation/README.md`

 * *Files identical despite different names*

### Comparing `iudex-0.4.5/iudex/instrumentation/attributes.py` & `iudex-0.4.6/iudex/instrumentation/attributes.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.5/iudex/instrumentation/instrumentation.py` & `iudex-0.4.6/iudex/instrumentation/instrumentation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
-from typing import Optional, Union
+from typing import Optional, TypedDict, Union
+import subprocess
 
 from opentelemetry._logs import set_logger_provider
 from opentelemetry.exporter.otlp.proto.http._log_exporter import OTLPLogExporter
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk._logs import LoggerProvider, LoggingHandler
 from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
 from opentelemetry.sdk.environment_variables import (
@@ -30,57 +31,71 @@
     "DEBUG": logging.DEBUG,
     "INFO": logging.INFO,
     "WARNING": logging.WARNING,
     "ERROR": logging.ERROR,
     "CRITICAL": logging.CRITICAL,
     "NOTSET": logging.NOTSET,
 }
+DEFAULT_LOG_LEVEL = logging.INFO
 
 IUDEX_CONFIGURED = False
 
+class IudexConfig(TypedDict):
+    iudex_api_key: Optional[str] = None,
+    service_name: Optional[str] = None,
+    instance_id: Optional[str] = None,
+    logs_endpoint: Optional[str] = None,
+    traces_endpoint: Optional[str] = None,
+    log_level: Optional[Union[str, int]] = None,
+    git_commit: Optional[str] = None,
+    github_url: Optional[str] = None,
 
-class IudexConfig:
+class _IudexConfig(IudexConfig):
     def __init__(
         self,
-        iudex_api_key: Optional[str] = None,
-        service_name: Optional[str] = None,
-        instance_id: Optional[str] = None,
-        logs_endpoint: Optional[str] = None,
-        traces_endpoint: Optional[str] = None,
-        log_level: Optional[Union[str, int]] = logging.NOTSET,
+        **kwargs: IudexConfig,
     ):
-        self.iudex_api_key = iudex_api_key or os.getenv("IUDEX_API_KEY")
+        self.iudex_api_key = kwargs.iudex_api_key or os.getenv("IUDEX_API_KEY")
         if not self.iudex_api_key:
             _logger.warning(
                 "Missing API key, no telemetry will be sent to Iudex. "
                 + "Provide the iudex_api_key parameter or set the IUDEX_API_KEY environment variable."
             )
             return
 
         self.service_name = (
-            service_name or os.getenv(OTEL_SERVICE_NAME) or DEFAULT_SERVICE_NAME
+            kwargs.service_name or os.getenv(OTEL_SERVICE_NAME) or DEFAULT_SERVICE_NAME
         )
-        self.instance_id = instance_id
+        self.instance_id = kwargs.instance_id
 
         self.logs_endpoint = (
-            logs_endpoint
+            kwargs.logs_endpoint
             or os.getenv(OTEL_EXPORTER_OTLP_LOGS_ENDPOINT)
             or DEFAULT_IUDEX_LOGS_ENDPOINT
         )
 
         self.traces_endpoint = (
-            traces_endpoint
+            kwargs.traces_endpoint
             or os.getenv(OTEL_EXPORTER_OTLP_TRACES_ENDPOINT)
             or DEFAULT_IUDEX_TRACES_ENDPOINT
         )
 
         log_level = log_level or os.getenv(OTEL_LOG_LEVEL)
         if isinstance(log_level, str):
             log_level = LOG_LEVEL_ATOI.get(log_level.upper())
-        self.log_level = log_level or logging.NOTSET
+        self.log_level = log_level or DEFAULT_LOG_LEVEL
+
+        self.git_commit = kwargs.git_commit or os.getenv("GIT_COMMIT")
+        if not self.git_commit:
+            try:
+                self.git_commit = subprocess.check_output(['git', 'rev-parse', 'HEAD']).strip()
+            except:
+                pass
+
+        self.github_url = kwargs.github_url or os.getenv("GITHUB_URL")
 
     def configure(self):
         if not self.iudex_api_key:
             _logger.warning(
                 "Missing API key, no telemetry will be sent to Iudex. "
                 + "Provide the iudex_api_key parameter or set the IUDEX_API_KEY environment variable."
             )
@@ -89,16 +104,19 @@
         global IUDEX_CONFIGURED
         if IUDEX_CONFIGURED:
             return
 
         # configure common
         attributes = {}
         attributes["service.name"] = self.service_name
-        if self.instance_id:
-            attributes["service.instance.id"] = self.instance_id
+        attributes["service.instance.id"] = self.instance_id
+        attributes["git.commit"] = self.git_commit
+        attributes["github.url"] = self.github_url
+        # clean attributes
+        attributes = {key: value for key, value in attributes.items() if value is not None}
         resource = Resource.create(attributes)
 
         # set default headers to send iudex api key
         headers = {"x-api-key": self.iudex_api_key}
         os.environ[OTEL_EXPORTER_OTLP_HEADERS] = f"x-api-key:{self.iudex_api_key}"
 
         # configure logger
@@ -117,24 +135,24 @@
         set_tracer_provider(trace_provider)
 
         IUDEX_CONFIGURED = True
 
 
 def configure_logger(
     logger_name: Optional[str] = None,
-    log_level: Optional[Union[str, int]] = logging.NOTSET,
+    log_level: Optional[Union[str, int]] = None,
 ):
     """Instruments a named logger.
 
     Useful for non-root loggers with propagate=False.
     This way, the logger still has the instrumented handler to send logs to Iudex.
     """
     if isinstance(log_level, str):
         log_level = LOG_LEVEL_ATOI.get(log_level.upper())
-    log_level = log_level or logging.NOTSET
+    log_level = log_level or DEFAULT_LOG_LEVEL
 
     logger = logging.getLogger(logger_name)
     logger.setLevel(log_level)
     logger_handler = LoggingHandler(level=log_level)
     logger_handler._get_attributes = get_attributes
     logger.addHandler(logger_handler)
```

### Comparing `iudex-0.4.5/iudex/instrumentation/lambda.py` & `iudex-0.4.6/iudex/instrumentation/lambda.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import Optional, Union
 
-from .instrumentation import IudexConfig
+from .instrumentation import _IudexConfig, IudexConfig
 
 
 def instrument(
     service_name: Optional[str] = None,
     instance_id: Optional[str] = None,
     iudex_api_key: Optional[str] = None,
     log_level: Optional[Union[int, str]] = None,
+    git_commit: Optional[str] = None,
+    github_url: Optional[str] = None,
     config: Optional[IudexConfig] = None,
 ):
     """Auto-instruments app to send OTel signals to Iudex.
 
     Invoke this function in your Lambda entrypoint.
 
     Args:
@@ -20,21 +22,22 @@
         instance_id: ID of the service instance, e.g. container id, pod name.
         iudex_api_key: Your Iudex API key.
             If not supplied, env var IUDEX_API_KEY will be used.
         log_level: Logging level for the root logger.
         config: IudexConfig object with more granular options.
             Will override all other args, so provide them to the object instead.
     """
-    kwargs = {}
-    if service_name:
-        kwargs["service_name"] = service_name
-    if instance_id:
-        kwargs["instance_id"] = instance_id
-    if iudex_api_key:
-        kwargs["iudex_api_key"] = iudex_api_key
-    if log_level:
-        kwargs["log_level"] = log_level
-    config = config or IudexConfig(**kwargs)
+    kwargs: IudexConfig = {
+        "iudex_api_key": iudex_api_key,
+        "service_name": service_name,
+        "instance_id": instance_id,
+        "logs_endpoint": None,
+        "traces_endpoint": None,
+        "log_level": log_level,
+        "git_commit": git_commit,
+        "github_url": github_url,
+    }
+    config = config or _IudexConfig(**kwargs)
 
     config.configure()
 
     return config
```

### Comparing `iudex-0.4.5/iudex/types/function.py` & `iudex-0.4.6/iudex/types/function.py`

 * *Files identical despite different names*

### Comparing `iudex-0.4.5/pyproject.toml` & `iudex-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iudex"
-version = "0.4.5"
+version = "0.4.6"
 description = ""
 authors = ["Drake Wong <drake@iudex.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^1.12.0"
```

### Comparing `iudex-0.4.5/PKG-INFO` & `iudex-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iudex
-Version: 0.4.5
+Version: 0.4.6
 Summary: 
 Author: Drake Wong
 Author-email: drake@iudex.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

