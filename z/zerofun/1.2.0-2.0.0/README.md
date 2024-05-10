# Comparing `tmp/zerofun-1.2.0.tar.gz` & `tmp/zerofun-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerofun-1.2.0.tar", last modified: Thu Aug 31 22:01:49 2023, max compression
+gzip compressed data, was "zerofun-2.0.0.tar", last modified: Fri May 10 22:29:39 2024, max compression
```

## Comparing `zerofun-1.2.0.tar` & `zerofun-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-08-31 22:01:49.342181 zerofun-1.2.0/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1054 2023-08-27 19:09:02.000000 zerofun-1.2.0/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)       25 2023-08-30 18:59:04.000000 zerofun-1.2.0/MANIFEST.in
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2023-08-31 22:01:49.342181 zerofun-1.2.0/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3347 2023-08-30 19:48:59.000000 zerofun-1.2.0/README.md
--rw-r-----   0 danijar  (322066) primarygroup (89939)       41 2023-08-30 18:50:51.000000 zerofun-1.2.0/requirements.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2023-08-31 22:01:49.342181 zerofun-1.2.0/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1094 2023-08-30 18:55:02.000000 zerofun-1.2.0/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-08-31 22:01:49.342181 zerofun-1.2.0/zerofun/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      575 2023-08-31 21:58:43.000000 zerofun-1.2.0/zerofun/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4928 2023-08-31 21:59:22.000000 zerofun-1.2.0/zerofun/client.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3753 2023-08-31 21:59:56.000000 zerofun-1.2.0/zerofun/proc_server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3240 2023-08-31 21:56:38.000000 zerofun-1.2.0/zerofun/process.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6256 2023-08-31 22:00:20.000000 zerofun-1.2.0/zerofun/server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7253 2023-08-31 21:56:38.000000 zerofun-1.2.0/zerofun/sockets.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2583 2023-08-31 21:56:38.000000 zerofun-1.2.0/zerofun/thread.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3628 2023-08-31 22:00:39.000000 zerofun-1.2.0/zerofun/utils.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2023-08-31 22:01:49.342181 zerofun-1.2.0/zerofun.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2023-08-31 22:01:49.000000 zerofun-1.2.0/zerofun.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      361 2023-08-31 22:01:49.000000 zerofun-1.2.0/zerofun.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2023-08-31 22:01:49.000000 zerofun-1.2.0/zerofun.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       41 2023-08-31 22:01:49.000000 zerofun-1.2.0/zerofun.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        8 2023-08-31 22:01:49.000000 zerofun-1.2.0/zerofun.egg-info/top_level.txt
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:29:39.649948 zerofun-2.0.0/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1054 2024-05-10 21:22:12.000000 zerofun-2.0.0/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       25 2024-05-10 21:22:12.000000 zerofun-2.0.0/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 22:29:39.649948 zerofun-2.0.0/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3347 2024-05-10 21:22:12.000000 zerofun-2.0.0/README.md
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       48 2024-05-10 22:03:51.000000 zerofun-2.0.0/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-10 22:29:39.649948 zerofun-2.0.0/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1094 2024-05-10 21:22:12.000000 zerofun-2.0.0/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:29:39.645948 zerofun-2.0.0/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2956 2024-05-10 21:22:12.000000 zerofun-2.0.0/tests/test_process.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    17320 2024-05-10 22:28:45.000000 zerofun-2.0.0/tests/test_server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2198 2024-05-10 21:22:12.000000 zerofun-2.0.0/tests/test_thread.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:29:39.649948 zerofun-2.0.0/zerofun/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      575 2024-05-10 22:29:02.000000 zerofun-2.0.0/zerofun/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4839 2024-05-10 22:25:55.000000 zerofun-2.0.0/zerofun/client.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3753 2024-05-10 21:22:12.000000 zerofun-2.0.0/zerofun/proc_server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3240 2024-05-10 21:24:11.000000 zerofun-2.0.0/zerofun/process.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6228 2024-05-10 22:28:32.000000 zerofun-2.0.0/zerofun/server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7435 2024-05-10 22:22:24.000000 zerofun-2.0.0/zerofun/sockets.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2555 2024-05-10 21:24:04.000000 zerofun-2.0.0/zerofun/thread.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3628 2024-05-10 22:03:53.000000 zerofun-2.0.0/zerofun/utils.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:29:39.649948 zerofun-2.0.0/zerofun.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 22:29:39.000000 zerofun-2.0.0/zerofun.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      425 2024-05-10 22:29:39.000000 zerofun-2.0.0/zerofun.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-10 22:29:39.000000 zerofun-2.0.0/zerofun.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       48 2024-05-10 22:29:39.000000 zerofun-2.0.0/zerofun.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        8 2024-05-10 22:29:39.000000 zerofun-2.0.0/zerofun.egg-info/top_level.txt
```

### Comparing `zerofun-1.2.0/LICENSE` & `zerofun-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zerofun-1.2.0/PKG-INFO` & `zerofun-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerofun
-Version: 1.2.0
+Version: 2.0.0
 Summary: Remote function calls for array data using ZMQ
 Home-page: http://github.com/danijar/zerofun
 Author: Danijar Hafner
 Author-email: mail@danijar.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zerofun-1.2.0/README.md` & `zerofun-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `zerofun-1.2.0/setup.py` & `zerofun-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `zerofun-1.2.0/zerofun/__init__.py` & `zerofun-2.0.0/zerofun/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.2.0'
+__version__ = '2.0.0'
 
 import multiprocessing as mp
 try:
   mp.set_start_method('spawn')
 except RuntimeError:
   pass
```

### Comparing `zerofun-1.2.0/zerofun/client.py` & `zerofun-2.0.0/zerofun/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,14 @@
           time.sleep(0.001)
     if self.errors:
       try:
         while self.queue[0].done():
           self.queue.popleft().result()
       except IndexError:
         pass
-    assert isinstance(data, dict)
-    data = {k: np.asarray(v) for k, v in data.items()}
     data = sockets.pack(data)
     rid = self.socket.send_call(method, data)
     self.send_per_sec.step(1)
     future = Future(self._receive, rid)
     self.futures[rid] = future
     if self.errors or self.maxinflight:
       self.queue.append(future)
```

### Comparing `zerofun-1.2.0/zerofun/proc_server.py` & `zerofun-2.0.0/zerofun/proc_server.py`

 * *Files identical despite different names*

### Comparing `zerofun-1.2.0/zerofun/process.py` & `zerofun-2.0.0/zerofun/process.py`

 * *Files identical despite different names*

### Comparing `zerofun-1.2.0/zerofun/server.py` & `zerofun-2.0.0/zerofun/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,14 @@
           for k, v in data[0].items()}
     else:
       data = sockets.unpack(payload)
     if method.donefn:
       result, logs = method.workfn(data)
     else:
       result = method.workfn(data)
-      result = result or {}
       logs = None
     if method.batched:
       results = [
           {k: v[i] for k, v in result.items()} for i in range(method.insize)]
       payload = [sockets.pack(x) for x in results]
     else:
       payload = sockets.pack(result)
```

### Comparing `zerofun-1.2.0/zerofun/sockets.py` & `zerofun-2.0.0/zerofun/sockets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import enum
 import itertools
 import msgpack
 import threading
 import time
 
+import elements
 import numpy as np
 import zmq
 
+
 DEBUG = False
 # DEBUG = True
 
 class Type(enum.Enum):
   PING   = int(1).to_bytes(1, 'big')  # rid
   PONG   = int(2).to_bytes(1, 'big')  # rid
   CALL   = int(3).to_bytes(1, 'big')  # rid, text, payload
@@ -199,40 +201,44 @@
     rid = next(self.rid).to_bytes(8, 'big')
     with self.lock:
       self.socket.send_multipart([addr, Type.PING.value, rid])
     return rid
 
   def send_result(self, addr, rid, payload):
     with self.lock:
-      self.socket.send_multipart([addr, Type.RESULT.value, rid, *payload])
+      self.socket.send_multipart(
+          [addr, Type.RESULT.value, rid, *payload], copy=False, track=True)
 
   def send_error(self, addr, rid, text):
     text = text.encode('utf-8')
     with self.lock:
       self.socket.send_multipart([addr, Type.ERROR.value, rid, text])
 
   def close(self):
     with self.lock:
       self.socket.close()
 
 
 def pack(data):
-  data = {k: np.asarray(v) for k, v in data.items()}
+  leaves, structure = elements.tree.flatten(data)
   dtypes, shapes, buffers = [], [], []
-  items = sorted(data.items(), key=lambda x: x[0])
-  keys, vals = zip(*items) if items else ((), ())
-  dtypes = [v.dtype.str for v in vals]
-  shapes = [v.shape for v in vals]
-  buffers = [v.tobytes() for v in vals]
-  meta = (keys, dtypes, shapes)
+  for value in leaves:
+    value = np.asarray(value)
+    assert value.data.c_contiguous, (
+        "Array is not contiguous in memory. Use np.asarray(arr, order='C') " +
+        "before passing the data into pack().")
+    dtypes.append(value.dtype.str)
+    shapes.append(value.shape)
+    buffers.append(value.data)
+  meta = (structure, dtypes, shapes)
   payload = [msgpack.packb(meta), *buffers]
   return payload
 
 
 def unpack(payload):
   meta, *buffers = payload
-  keys, dtypes, shapes = msgpack.unpackb(meta)
-  vals = [
+  structure, dtypes, shapes = msgpack.unpackb(meta)
+  leaves = [
       np.frombuffer(b, d).reshape(s)
       for i, (d, s, b) in enumerate(zip(dtypes, shapes, buffers))]
-  data = dict(zip(keys, vals))
+  data = elements.tree.unflatten(leaves, structure)
   return data
```

### Comparing `zerofun-1.2.0/zerofun/thread.py` & `zerofun-2.0.0/zerofun/thread.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 class Thread:
 
   def __init__(self, fn, *args, name=None, start=False):
     self.fn = fn
     self._exitcode = None
     self.exception = None
     name = name or fn.__name__
-    self.old_name = name[:]
     self.thread = threading.Thread(
         target=self._wrapper, args=args, name=name, daemon=True)
     self.started = False
     start and self.start()
 
   @property
   def name(self):
```

### Comparing `zerofun-1.2.0/zerofun/utils.py` & `zerofun-2.0.0/zerofun/utils.py`

 * *Files identical despite different names*

### Comparing `zerofun-1.2.0/zerofun.egg-info/PKG-INFO` & `zerofun-2.0.0/zerofun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerofun
-Version: 1.2.0
+Version: 2.0.0
 Summary: Remote function calls for array data using ZMQ
 Home-page: http://github.com/danijar/zerofun
 Author: Danijar Hafner
 Author-email: mail@danijar.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

