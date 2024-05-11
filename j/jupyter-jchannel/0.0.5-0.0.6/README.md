# Comparing `tmp/jupyter_jchannel-0.0.5.tar.gz` & `tmp/jupyter_jchannel-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_jchannel-0.0.5.tar", max compression
+gzip compressed data, was "jupyter_jchannel-0.0.6.tar", max compression
```

## Comparing `jupyter_jchannel-0.0.5.tar` & `jupyter_jchannel-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    14198 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/LICENSE
--rw-r--r--   0        0        0      538 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/README.md
--rw-r--r--   0        0        0      201 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/__init__.py
--rw-r--r--   0        0        0       60 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/channel.py
--rw-r--r--   0        0        0       85 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/frontend/__init__.py
--rw-r--r--   0        0        0     1370 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/frontend/abstract.py
--rw-r--r--   0        0        0      509 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/frontend/ipython.py
--rw-r--r--   0        0        0      266 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/registry.py
--rw-r--r--   0        0        0    13189 2024-05-09 19:04:09.199670 jupyter_jchannel-0.0.5/jchannel/server.py
--rw-r--r--   0        0        0      731 2024-05-09 19:04:09.203670 jupyter_jchannel-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 jupyter_jchannel-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    14198 2024-05-11 14:54:20.086931 jupyter_jchannel-0.0.6/LICENSE
+-rw-r--r--   0        0        0      538 2024-05-11 14:54:20.086931 jupyter_jchannel-0.0.6/README.md
+-rw-r--r--   0        0        0      186 2024-05-11 14:54:20.086931 jupyter_jchannel-0.0.6/jchannel/__init__.py
+-rw-r--r--   0        0        0     2223 2024-05-11 14:54:20.086931 jupyter_jchannel-0.0.6/jchannel/channel.py
+-rw-r--r--   0        0        0       83 2024-05-11 14:54:20.086931 jupyter_jchannel-0.0.6/jchannel/error.py
+-rw-r--r--   0        0        0       85 2024-05-11 14:54:20.086931 jupyter_jchannel-0.0.6/jchannel/frontend/__init__.py
+-rw-r--r--   0        0        0     1370 2024-05-11 14:54:20.090931 jupyter_jchannel-0.0.6/jchannel/frontend/abstract.py
+-rw-r--r--   0        0        0      509 2024-05-11 14:54:20.090931 jupyter_jchannel-0.0.6/jchannel/frontend/ipython.py
+-rw-r--r--   0        0        0      266 2024-05-11 14:54:20.090931 jupyter_jchannel-0.0.6/jchannel/registry.py
+-rw-r--r--   0        0        0    13152 2024-05-11 14:54:20.090931 jupyter_jchannel-0.0.6/jchannel/server.py
+-rw-r--r--   0        0        0      731 2024-05-11 14:54:20.090931 jupyter_jchannel-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 jupyter_jchannel-0.0.6/PKG-INFO
```

### Comparing `jupyter_jchannel-0.0.5/LICENSE` & `jupyter_jchannel-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_jchannel-0.0.5/README.md` & `jupyter_jchannel-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_jchannel-0.0.5/jchannel/frontend/abstract.py` & `jupyter_jchannel-0.0.6/jchannel/frontend/abstract.py`

 * *Files identical despite different names*

### Comparing `jupyter_jchannel-0.0.5/jchannel/server.py` & `jupyter_jchannel-0.0.6/jchannel/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 import json
 import asyncio
 import logging
 
 from enum import Enum, auto
 from inspect import isawaitable
 from aiohttp import web, WSMsgType
+from jchannel.error import StateError, JavascriptError
 from jchannel.registry import registry
 from jchannel.frontend import frontend
 from jchannel.channel import Channel
 
 
-class StateError(Exception):
-    pass
-
-
-class JavascriptError(Exception):
-    pass
-
-
 class DebugScenario(Enum):
     STOP_BEFORE_RESTART = auto()
     STOP_AFTER_BREAK = auto()
     CONNECT_BEFORE_BREAK = auto()
     CONNECT_BEFORE_CLEAN = auto()
     RECEIVE_BEFORE_CLEAN = auto()
     CATCH_BEFORE_CLEAN = auto()
@@ -115,26 +108,28 @@
         self.disconnection = None
 
         if __debug__:  # pragma: no cover
             self.sentinel = DebugSentinel()
 
         self.channels = {}
 
-    def open(self):
-        Channel(self)
-
-    def load(self):
-        frontend.run(f"jchannel.start('{self.url}')")
-
     def start(self):
         return asyncio.create_task(self._start())
 
     def stop(self):
         return asyncio.create_task(self._stop())
 
+    def load(self):
+        frontend.run(f"jchannel.start('{self.url}')")
+
+    def open(self, code):
+        channel = Channel(self, code)
+        channel.open()
+        return channel
+
     async def __aenter__(self):
         await self._start()
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self._stop()
         return False
@@ -196,19 +191,14 @@
             if __debug__:  # pragma: no cover
                 await self.sentinel.set_and_yield(DebugScenario.STOP_BEFORE_RESTART)
 
     async def _run(self, runner, site):
         restarting = True
 
         while restarting:
-            try:
-                await self.connection
-            except asyncio.CancelledError:
-                pass
-
             restarting = await self.disconnection
 
             if restarting:
                 if __debug__:  # pragma: no cover
                     await self.sentinel.wait_on_count(DebugScenario.STOP_BEFORE_RESTART, 1)
 
                 loop = asyncio.get_running_loop()
@@ -254,15 +244,15 @@
         try:
             if self.connection is None:
                 socket = None
             else:
                 self.load()
 
                 try:
-                    socket = await asyncio.wait_for(self.connection, timeout)
+                    socket = await asyncio.wait_for(asyncio.shield(self.connection), timeout)
                 except asyncio.TimeoutError:
                     raise StateError('Client not connected: check the browser console for details')
 
             if socket is None:
                 raise StateError('Server not running')
 
             if not socket.prepared:
@@ -276,14 +266,16 @@
             body = {
                 'future': registry.store(future),
                 'channel': channel_key,
                 'payload': payload,
             }
 
             await self._accept(socket, body_type, body)
+
+            return future
         finally:
             if __debug__:  # pragma: no cover
                 await self.sentinel.set_and_yield(DebugScenario.SEND_BEFORE_PREPARE)
 
     async def _on_shutdown(self, app):
         if app.socket is not None:
             await app.socket.close()
@@ -343,17 +335,18 @@
                                 channel = self.channels[channel_key]
 
                                 try:
                                     match body_type:
                                         case 'echo':
                                             body_type = 'result'
                                         case 'call':
-                                            output = channel.handle_call(input['name'], input['args'])
+                                            output = channel._handle_call(input['name'], input['args'])
                                             if isawaitable(output):
                                                 output = await output
+
                                             payload = json.dumps(output)
                                             body_type = 'result'
                                         case _:
                                             payload = f'Received unexpected body type {body_type}'
                                             body_type = 'exception'
                                 except Exception:
                                     logging.exception('Caught handler exception')
```

### Comparing `jupyter_jchannel-0.0.5/pyproject.toml` & `jupyter_jchannel-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jupyter-jchannel"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = [
     "Marcelo Hashimoto <marcelo.hashimoto@gmail.com>"
 ]
 readme = "README.md"
 repository = "https://github.com/hashiprobr/jupyter-jchannel"
 packages = [
@@ -12,15 +12,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.9.5"
 
 [tool.poetry.group.dev.dependencies]
-jupyterlab = "^4.1.8"
+jupyterlab = "^4.2.0"
 ipywidgets = "^8.1.2"
 autopep8 = "^2.1.0"
 pytest = "^8.2.0"
 pytest-asyncio = "~0.23.6"
 pytest-mock = "^3.14.0"
 pytest-cov = "^5.0.0"
 sphinx = "^7.3.7"
```

### Comparing `jupyter_jchannel-0.0.5/PKG-INFO` & `jupyter_jchannel-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-jchannel
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Home-page: https://github.com/hashiprobr/jupyter-jchannel
 Author: Marcelo Hashimoto
 Author-email: marcelo.hashimoto@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

