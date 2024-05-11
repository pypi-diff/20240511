# Comparing `tmp/naja-atra-1.0.2.tar.gz` & `tmp/naja_atra-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naja-atra-1.0.2.tar", last modified: Wed Apr  3 08:02:02 2024, max compression
+gzip compressed data, was "naja_atra-1.1.0.tar", last modified: Sat May 11 09:58:35 2024, max compression
```

## Comparing `naja-atra-1.0.2.tar` & `naja_atra-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.256513 naja-atra-1.0.2/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1066 2023-01-29 02:07:01.000000 naja-atra-1.0.2/LICENSE
--rw-r--r--   0 keijack   (1000) keijack   (1000)     3012 2024-04-03 08:02:02.256513 naja-atra-1.0.2/PKG-INFO
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1031 2024-04-02 02:23:04.000000 naja-atra-1.0.2/README.md
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.236513 naja-atra-1.0.2/naja_atra/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1172 2024-04-03 08:01:09.000000 naja-atra-1.0.2/naja_atra/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     2049 2024-04-02 11:35:53.000000 naja-atra-1.0.2/naja_atra/__main__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    28716 2024-04-01 10:12:01.000000 naja-atra-1.0.2/naja_atra/app_conf.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.240513 naja-atra-1.0.2/naja_atra/http_servers/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-03-07 02:15:37.000000 naja-atra-1.0.2/naja_atra/http_servers/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     3740 2024-03-11 09:12:30.000000 naja-atra-1.0.2/naja_atra/http_servers/coroutine_http_server.py
--rwxrwxr-x   0 keijack   (1000) keijack   (1000)     5587 2024-03-12 01:27:45.000000 naja-atra-1.0.2/naja_atra/http_servers/http_server.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    17237 2024-03-11 09:43:12.000000 naja-atra-1.0.2/naja_atra/http_servers/routing_server.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     3337 2024-03-11 09:15:29.000000 naja-atra-1.0.2/naja_atra/http_servers/threading_http_server.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    18383 2024-03-11 09:38:20.000000 naja-atra-1.0.2/naja_atra/models.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.244513 naja-atra-1.0.2/naja_atra/request_handlers/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-03-07 02:12:14.000000 naja-atra-1.0.2/naja_atra/request_handlers/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    28102 2024-03-11 09:42:45.000000 naja-atra-1.0.2/naja_atra/request_handlers/http_controller_handler.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    17638 2024-03-11 09:39:40.000000 naja-atra-1.0.2/naja_atra/request_handlers/http_request_handler.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     5914 2024-03-11 09:39:40.000000 naja-atra-1.0.2/naja_atra/request_handlers/http_session_local_impl.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    14419 2024-03-11 09:39:40.000000 naja-atra-1.0.2/naja_atra/request_handlers/model_bindings.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    23851 2024-03-11 09:39:40.000000 naja-atra-1.0.2/naja_atra/request_handlers/websocket_controller_handler.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     8848 2024-03-11 09:58:15.000000 naja-atra-1.0.2/naja_atra/server.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.244513 naja-atra-1.0.2/naja_atra/utils/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-03-07 02:23:26.000000 naja-atra-1.0.2/naja_atra/utils/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     6987 2024-03-11 09:39:40.000000 naja-atra-1.0.2/naja_atra/utils/http_utils.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     6668 2024-03-07 03:33:13.000000 naja-atra-1.0.2/naja_atra/utils/logger.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.256513 naja-atra-1.0.2/naja_atra.egg-info/
--rw-r--r--   0 keijack   (1000) keijack   (1000)     3012 2024-04-03 08:02:02.000000 naja-atra-1.0.2/naja_atra.egg-info/PKG-INFO
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1077 2024-04-03 08:02:02.000000 naja-atra-1.0.2/naja_atra.egg-info/SOURCES.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)        1 2024-04-03 08:02:02.000000 naja-atra-1.0.2/naja_atra.egg-info/dependency_links.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       56 2024-04-03 08:02:02.000000 naja-atra-1.0.2/naja_atra.egg-info/requires.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       10 2024-04-03 08:02:02.000000 naja-atra-1.0.2/naja_atra.egg-info/top_level.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)      929 2024-03-08 09:12:59.000000 naja-atra-1.0.2/pyproject.toml
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       38 2024-04-03 08:02:02.256513 naja-atra-1.0.2/setup.cfg
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       62 2023-01-29 02:07:01.000000 naja-atra-1.0.2/setup.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.248513 naja-atra-1.0.2/tests/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)        0 2023-01-29 02:07:01.000000 naja-atra-1.0.2/tests/__init__.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-04-03 08:02:02.252513 naja-atra-1.0.2/tests/ctrls/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)        0 2023-01-29 02:07:01.000000 naja-atra-1.0.2/tests/ctrls/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     9970 2024-03-11 09:19:38.000000 naja-atra-1.0.2/tests/ctrls/my_controllers.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1890 2024-03-11 08:58:23.000000 naja-atra-1.0.2/tests/ctrls/my_controllers_model_binding.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     3538 2024-03-07 03:14:28.000000 naja-atra-1.0.2/tests/ctrls/ws_controllers.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     8064 2024-03-08 02:52:49.000000 naja-atra-1.0.2/tests/test_all_ctrls.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.282536 naja_atra-1.1.0/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1066 2023-01-29 02:07:01.000000 naja_atra-1.1.0/LICENSE
+-rw-r--r--   0 keijack   (1000) keijack   (1000)     3012 2024-05-11 09:58:35.282536 naja_atra-1.1.0/PKG-INFO
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1031 2024-04-02 02:23:04.000000 naja_atra-1.1.0/README.md
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.270536 naja_atra-1.1.0/naja_atra/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1172 2024-05-11 09:57:23.000000 naja_atra-1.1.0/naja_atra/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     2049 2024-04-02 11:35:53.000000 naja_atra-1.1.0/naja_atra/__main__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    28716 2024-04-01 10:12:01.000000 naja_atra-1.1.0/naja_atra/app_conf.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.274536 naja_atra-1.1.0/naja_atra/http_servers/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-04-16 12:02:34.000000 naja_atra-1.1.0/naja_atra/http_servers/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     3740 2024-03-11 09:12:30.000000 naja_atra-1.1.0/naja_atra/http_servers/coroutine_http_server.py
+-rwxrwxr-x   0 keijack   (1000) keijack   (1000)     5587 2024-03-12 01:27:45.000000 naja_atra-1.1.0/naja_atra/http_servers/http_server.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    17237 2024-03-11 09:43:12.000000 naja_atra-1.1.0/naja_atra/http_servers/routing_server.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     3337 2024-03-11 09:15:29.000000 naja_atra-1.1.0/naja_atra/http_servers/threading_http_server.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    18456 2024-05-11 06:54:42.000000 naja_atra-1.1.0/naja_atra/models.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.278536 naja_atra-1.1.0/naja_atra/request_handlers/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-03-07 02:12:14.000000 naja_atra-1.1.0/naja_atra/request_handlers/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    30633 2024-05-11 09:50:45.000000 naja_atra-1.1.0/naja_atra/request_handlers/http_controller_handler.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    17638 2024-05-11 09:07:29.000000 naja_atra-1.1.0/naja_atra/request_handlers/http_request_handler.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     5914 2024-03-11 09:39:40.000000 naja_atra-1.1.0/naja_atra/request_handlers/http_session_local_impl.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    14419 2024-03-11 09:39:40.000000 naja_atra-1.1.0/naja_atra/request_handlers/model_bindings.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    23851 2024-03-11 09:39:40.000000 naja_atra-1.1.0/naja_atra/request_handlers/websocket_controller_handler.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     8848 2024-04-16 12:02:50.000000 naja_atra-1.1.0/naja_atra/server.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.278536 naja_atra-1.1.0/naja_atra/utils/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-03-07 02:23:26.000000 naja_atra-1.1.0/naja_atra/utils/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     7276 2024-05-11 09:46:24.000000 naja_atra-1.1.0/naja_atra/utils/http_utils.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     6668 2024-03-07 03:33:13.000000 naja_atra-1.1.0/naja_atra/utils/logger.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.278536 naja_atra-1.1.0/naja_atra.egg-info/
+-rw-r--r--   0 keijack   (1000) keijack   (1000)     3012 2024-05-11 09:58:35.000000 naja_atra-1.1.0/naja_atra.egg-info/PKG-INFO
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1077 2024-05-11 09:58:35.000000 naja_atra-1.1.0/naja_atra.egg-info/SOURCES.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)        1 2024-05-11 09:58:35.000000 naja_atra-1.1.0/naja_atra.egg-info/dependency_links.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       56 2024-05-11 09:58:35.000000 naja_atra-1.1.0/naja_atra.egg-info/requires.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       10 2024-05-11 09:58:35.000000 naja_atra-1.1.0/naja_atra.egg-info/top_level.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)      929 2024-03-08 09:12:59.000000 naja_atra-1.1.0/pyproject.toml
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       38 2024-05-11 09:58:35.282536 naja_atra-1.1.0/setup.cfg
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       62 2023-01-29 02:07:01.000000 naja_atra-1.1.0/setup.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.278536 naja_atra-1.1.0/tests/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)        0 2023-01-29 02:07:01.000000 naja_atra-1.1.0/tests/__init__.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.278536 naja_atra-1.1.0/tests/ctrls/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)        0 2023-01-29 02:07:01.000000 naja_atra-1.1.0/tests/ctrls/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    10132 2024-05-11 09:30:50.000000 naja_atra-1.1.0/tests/ctrls/my_controllers.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1890 2024-03-11 08:58:23.000000 naja_atra-1.1.0/tests/ctrls/my_controllers_model_binding.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     3538 2024-03-07 03:14:28.000000 naja_atra-1.1.0/tests/ctrls/ws_controllers.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     8064 2024-03-08 02:52:49.000000 naja_atra-1.1.0/tests/test_all_ctrls.py
```

### Comparing `naja-atra-1.0.2/LICENSE` & `naja_atra-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/PKG-INFO` & `naja_atra-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naja-atra
-Version: 1.0.2
+Version: 1.1.0
 Summary: This is a simple http server, use MVC like design.
 Author-email: keijack <keijack.wu@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Keijack Wu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naja-atra-1.0.2/README.md` & `naja_atra-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/__init__.py` & `naja_atra-1.1.0/naja_atra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 SOFTWARE.
 """
 
 from .app_conf import *
 from .models import *
 
 name = "naja-atra"
-version = "1.0.2"
+version = "1.1.0"
```

### Comparing `naja-atra-1.0.2/naja_atra/__main__.py` & `naja_atra-1.1.0/naja_atra/__main__.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/app_conf.py` & `naja_atra-1.1.0/naja_atra/app_conf.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/http_servers/__init__.py` & `naja_atra-1.1.0/naja_atra/http_servers/__init__.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/http_servers/coroutine_http_server.py` & `naja_atra-1.1.0/naja_atra/http_servers/coroutine_http_server.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/http_servers/http_server.py` & `naja_atra-1.1.0/naja_atra/http_servers/http_server.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/http_servers/routing_server.py` & `naja_atra-1.1.0/naja_atra/http_servers/routing_server.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/http_servers/threading_http_server.py` & `naja_atra-1.1.0/naja_atra/http_servers/threading_http_server.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/models.py` & `naja_atra-1.1.0/naja_atra/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,17 @@
 
 class RequestBodyReader:
 
     @abstractmethod
     async def read(self, n: int = -1) -> bytes:
         return NotImplemented
 
+    async def read_to_end(self) -> bytes:
+        return NotImplemented
+
 
 class Request:
     """Request"""
 
     def __init__(self):
         self.method: str = ""  # GET, POST, PUT, DELETE, HEAD, etc.
         self.headers: Dict[str, str] = {}  # Request headers
```

### Comparing `naja-atra-1.0.2/naja_atra/request_handlers/__init__.py` & `naja_atra-1.1.0/naja_atra/request_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/request_handlers/http_controller_handler.py` & `naja_atra-1.1.0/naja_atra/request_handlers/http_controller_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,19 +53,21 @@
 class RequestBodyReaderWrapper(RequestBodyReader):
 
     def __init__(self, reader: StreamReader, content_length: int = None) -> None:
         self._content_length: int = content_length
         self._remain_length: int = content_length
         self._reader: StreamReader = reader
 
-    async def read(self, n: int = -1):
+    async def read(self, n: int = -1) -> bytes:
         data = b''
+        if not n:
+            return data
         if self._remain_length is not None and self._remain_length <= 0:
             return data
-        if not n or n < 0:
+        if n < 0:
             if self._remain_length:
                 data = await self._reader.read(self._remain_length)
             else:
                 data = await self._reader.read()
         else:
             if self._remain_length and n > self._remain_length:
                 data = await self._reader.read(self._remain_length)
@@ -73,14 +75,82 @@
                 data = await self._reader.read(n)
 
         if self._remain_length and self._remain_length > 0:
             self._remain_length -= len(data)
 
         return data
 
+    async def read_to_end(self) -> bytes:
+        return await self.read(self._remain_length)
+
+
+class RequestBodyReaderChunkedReader(RequestBodyReader):
+
+    def __init__(self, reader: StreamReader) -> None:
+        self._reader = reader
+        self._current_chunk_len: int = -1
+        self._buffer: bytes = b''
+        self._eof: bool = False
+        self._lock = asyncio.Lock()
+
+    async def _fill_buffer(self):
+        if self._eof:
+            return
+        if self._buffer:
+            return
+
+        if self._current_chunk_len > 0:
+            self._buffer = await self._reader.read(self._current_chunk_len)
+            self._current_chunk_len -= len(self._buffer)
+            return
+
+        if self._current_chunk_len == 0:
+            # Read \r\n at the end of a chunk
+            self._reader.read(2)
+
+        chunk_len = await self._reader.readline()
+        chunk_len = chunk_len.rstrip(b'\r\n')
+        self._current_chunk_len = int(chunk_len, 16)
+        _logger.debug(f"current chunk length: {self._current_chunk_len}")
+        if self._current_chunk_len == 0:
+            # Read \r\n at the end of the final chunk
+            await self._reader.read(2)
+            self._eof = True
+            return
+        if self._current_chunk_len < 0:
+            raise HttpError(400, "Invalid chunk length")
+        self._buffer = await self._reader.read(self._current_chunk_len)
+        self._current_chunk_len -= len(self._buffer)
+
+    async def _read(self, n: int = -1) -> bytes:
+        async with self._lock:
+            if not n:
+                return b''
+            await self._fill_buffer()
+            if len(self._buffer) > n:
+                data = self._buffer[:n]
+                self._buffer = self._buffer[n:]
+                return data
+            else:
+                data = self._buffer
+                self._buffer = b''
+                return data
+
+    async def read(self, n: int = -1) -> bytes:
+        if n >= 0:
+            return await self._read(n)
+        else:
+            data = b''
+            while not self._eof:
+                data += await self._read()
+            return data
+
+    async def read_to_end(self) -> bytes:
+        return await self._read(-1)
+
 
 class RequestWrapper(Request):
 
     def __init__(self):
         super().__init__()
         self._headers_keys_in_lowcase = {}
         self._path = ""
@@ -484,15 +554,15 @@
         path = self.request_path
         req = RequestWrapper()
         req.environment = self.environment or {}
         req.path = "/" + path
         req._path = path
         req._session_fac = self.routing_conf.session_factory
         headers = {}
-        _headers_keys_in_lowers = {}
+        _headers_keys_in_lowers: Dict[str, str] = {}
         for k in self.headers.keys():
             headers[k] = self.headers[k]
             _headers_keys_in_lowers[k.lower()] = self.headers[k]
         req.headers = headers
         req._headers_keys_in_lowcase = _headers_keys_in_lowers
 
         # cookies
@@ -501,35 +571,40 @@
 
         req.method = method
 
         req.parameters = self.query_parameters
 
         if "content-length" in _headers_keys_in_lowers.keys():
             content_length = int(_headers_keys_in_lowers["content-length"])
-
             req.reader = RequestBodyReaderWrapper(self.reader, content_length)
-
-            content_type = _headers_keys_in_lowers["content-type"]
-            if content_type.lower().startswith("application/x-www-form-urlencoded"):
-                req._body = await req.reader.read(content_length)
-                data_params = http_utils.decode_query_string(
-                    req._body.decode(DEFAULT_ENCODING))
-            elif content_type.lower().startswith("multipart/form-data"):
-                req._body = await req.reader.read(content_length)
-                data_params = self.__decode_multipart(
-                    content_type, req._body.decode("ISO-8859-1"))
-            elif content_type.lower().startswith("application/json"):
-                req._body = await req.reader.read(content_length)
-                req.json = json.loads(req._body.decode(DEFAULT_ENCODING))
-                data_params = {}
-            else:
-                data_params = {}
-            req.parameters = self.__merge(data_params, req.parameters)
+        elif _headers_keys_in_lowers.get("transfer-encoding", "").lower() == "chunked":
+            _logger.debug("chunked encoding")
+            req.reader = RequestBodyReaderChunkedReader(self.reader)
         else:
             req.reader = RequestBodyReaderWrapper(self.reader)
+
+        content_type = _headers_keys_in_lowers.get("content-type", "")
+        if content_type.lower().startswith("application/x-www-form-urlencoded"):
+            charset = http_utils.get_charset(content_type)
+            req._body = await req.reader.read_to_end()
+            body_decoded_params = http_utils.decode_query_string(
+                req._body.decode(charset))
+        elif content_type.lower().startswith("multipart/form-data"):
+            req._body = await req.reader.read_to_end()
+            body_decoded_params = self.__decode_multipart(
+                content_type, req._body.decode("ISO-8859-1"))
+        elif content_type.lower().startswith("application/json"):
+            charset = http_utils.get_charset(content_type)
+            req._body = await req.reader.read_to_end()
+            req.json = json.loads(req._body.decode(charset))
+            body_decoded_params = {}
+        else:
+            body_decoded_params = {}
+        req.parameters = self.__merge(body_decoded_params, req.parameters)
+
         return req
 
     def __merge(self, dic0: Dict[str, List[str]], dic1: Dict[str, List[str]]):
         """Merge tow dictionaries of which the structure is {k:[v1, v2]}"""
         dic = dic0
         for k, v in dic1.items():
             if k not in dic.keys():
```

### Comparing `naja-atra-1.0.2/naja_atra/request_handlers/http_request_handler.py` & `naja_atra-1.1.0/naja_atra/request_handlers/http_request_handler.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/request_handlers/http_session_local_impl.py` & `naja_atra-1.1.0/naja_atra/request_handlers/http_session_local_impl.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/request_handlers/model_bindings.py` & `naja_atra-1.1.0/naja_atra/request_handlers/model_bindings.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/request_handlers/websocket_controller_handler.py` & `naja_atra-1.1.0/naja_atra/request_handlers/websocket_controller_handler.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/server.py` & `naja_atra-1.1.0/naja_atra/server.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/utils/__init__.py` & `naja_atra-1.1.0/naja_atra/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra/utils/http_utils.py` & `naja_atra-1.1.0/naja_atra/utils/http_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,16 @@
 
 
 def get_function_kwargs(func, default_type=str):
     argspec = inspect.getfullargspec(func)
     if argspec.defaults is None:
         return []
 
-    kwargs = OrderedDict(zip(argspec.args[-len(argspec.defaults):], argspec.defaults))
+    kwargs = OrderedDict(
+        zip(argspec.args[-len(argspec.defaults):], argspec.defaults))
     kwarg_turples = []
     for k, v in kwargs.items():
         if k in argspec.annotations:
             k_anno = argspec.annotations[k]
         else:
             k_anno = default_type
         kwarg_turples.append((k, v, k_anno))
@@ -106,14 +107,23 @@
         if val is None:
             val = ""
         put_to(params, unquote(key), unquote(val))
 
     return params
 
 
+def get_charset(s: str) -> str:
+    pattern = re.compile(r"charset=([^;]+)")
+    m = pattern.search(s)
+    if m is not None:
+        return m.group(1)
+    else:
+        return DEFAULT_ENCODING
+
+
 def date_time_string(timestamp=None):
     if timestamp is None:
         timestamp = time.time()
     return email.utils.formatdate(timestamp, usegmt=True)
 
 
 def decode_response_body(raw_body: Any) -> Tuple[str, Union[str,  bytes, StaticFile]]:
@@ -131,15 +141,16 @@
             content_type = "text/html; charset=utf8"
         elif body.lower().startswith("<html") and body.endswith(">"):
             content_type = "text/html; charset=utf8"
         else:
             content_type = "text/plain; charset=utf8"
     elif isinstance(raw_body, StaticFile):
         if not os.path.isfile(raw_body.file_path):
-            _logger.error(f"Cannot find file[{raw_body.file_path}] specified in StaticFile body.")
+            _logger.error(
+                f"Cannot find file[{raw_body.file_path}] specified in StaticFile body.")
             raise HttpError(404, explain="Cannot find file for this url.")
         else:
             body = raw_body
             content_type = body.content_type
     elif isinstance(raw_body, bytes):
         body = raw_body
         content_type = "application/octet-stream"
@@ -159,43 +170,48 @@
     elif isinstance(body, StaticFile):
         with open(body.file_path, "rb") as in_file:
             byte_body = in_file.read()
     else:
         raise HttpError(400, explain="Cannot read body into bytes!")
     return content_type, byte_body
 
+
 def get_path_reg_pattern(url):
     _url: str = url
     path_names = re.findall("(?u)\\{\\w+\\}", _url)
     if len(path_names) == 0:
         if _url.startswith("**"):
-            _url = _url[2: ]
-            assert _url.find("*") < 0, "You can only config a * or ** at the start or end of a path."
+            _url = _url[2:]
+            assert _url.find(
+                "*") < 0, "You can only config a * or ** at the start or end of a path."
             _url = f'^([\\w%.\\-@!\\(\\)\\[\\]\\|\\$/]+){_url}$'
             return _url, [quote("__path_wildcard")]
         elif _url.startswith("*"):
-            _url = _url[1: ]
-            assert _url.find("*") < 0, "You can only config a * or ** at the start or end of a path."
+            _url = _url[1:]
+            assert _url.find(
+                "*") < 0, "You can only config a * or ** at the start or end of a path."
             _url = f'^([\\w%.\\-@!\\(\\)\\[\\]\\|\\$]+){_url}$'
             return _url, [quote("__path_wildcard")]
         elif _url.endswith("**"):
             _url = _url[0: -2]
-            assert _url.find("*") < 0, "You can only config a * or ** at the start or end of a path."
+            assert _url.find(
+                "*") < 0, "You can only config a * or ** at the start or end of a path."
             _url = f'^{_url}([\\w%.\\-@!\\(\\)\\[\\]\\|\\$/]+)$'
             return _url, [quote("__path_wildcard")]
         elif _url.endswith("*"):
             _url = _url[0: -1]
-            assert _url.find("*") < 0, "You can only config a * or ** at the start or end of a path."
+            assert _url.find(
+                "*") < 0, "You can only config a * or ** at the start or end of a path."
             _url = f'^{_url}([\\w%.\\-@!\\(\\)\\[\\]\\|\\$]+)$'
             return _url, [quote("__path_wildcard")]
         else:
             # normal url
             return None, path_names
     for name in path_names:
         _url = _url.replace(name, "([\\w%.\\-@!\\(\\)\\[\\]\\|\\$]+)")
     _url = f"^{_url}$"
 
     quoted_names = []
     for name in path_names:
         name = name[1: -1]
         quoted_names.append(quote(name))
-    return _url, quoted_names
+    return _url, quoted_names
```

### Comparing `naja-atra-1.0.2/naja_atra/utils/logger.py` & `naja_atra-1.1.0/naja_atra/utils/logger.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/naja_atra.egg-info/PKG-INFO` & `naja_atra-1.1.0/naja_atra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naja-atra
-Version: 1.0.2
+Version: 1.1.0
 Summary: This is a simple http server, use MVC like design.
 Author-email: keijack <keijack.wu@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Keijack Wu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naja-atra-1.0.2/naja_atra.egg-info/SOURCES.txt` & `naja_atra-1.1.0/naja_atra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/pyproject.toml` & `naja_atra-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/tests/ctrls/my_controllers.py` & `naja_atra-1.1.0/tests/ctrls/my_controllers.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,7 +327,12 @@
     def index_page(self):
         return "<!DOCTYPE html><html><head><title>你好</title></head><body>你好，世界！</body></html>"
 
 
 @route(url="/header_narrowing", method="POST", headers="Content-Type^=text/")
 def header_narrowing():
     return "a^=b"
+
+@route(url="/chunked", method=["POST", "PUT"])
+async def chunked(req: Request):
+    _logger.info(f"{req.parameter}")
+    return {"code": 0, "message": "success"}
```

### Comparing `naja-atra-1.0.2/tests/ctrls/my_controllers_model_binding.py` & `naja_atra-1.1.0/tests/ctrls/my_controllers_model_binding.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/tests/ctrls/ws_controllers.py` & `naja_atra-1.1.0/tests/ctrls/ws_controllers.py`

 * *Files identical despite different names*

### Comparing `naja-atra-1.0.2/tests/test_all_ctrls.py` & `naja_atra-1.1.0/tests/test_all_ctrls.py`

 * *Files identical despite different names*

