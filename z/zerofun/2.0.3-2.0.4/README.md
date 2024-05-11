# Comparing `tmp/zerofun-2.0.3.tar.gz` & `tmp/zerofun-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerofun-2.0.3.tar", last modified: Fri May 10 23:37:14 2024, max compression
+gzip compressed data, was "zerofun-2.0.4.tar", last modified: Fri May 10 23:51:00 2024, max compression
```

## Comparing `zerofun-2.0.3.tar` & `zerofun-2.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:37:14.393214 zerofun-2.0.3/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1054 2024-05-10 21:22:12.000000 zerofun-2.0.3/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)       25 2024-05-10 21:22:12.000000 zerofun-2.0.3/MANIFEST.in
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 23:37:14.393214 zerofun-2.0.3/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3347 2024-05-10 21:22:12.000000 zerofun-2.0.3/README.md
--rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-10 22:33:14.000000 zerofun-2.0.3/requirements.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-10 23:37:14.393214 zerofun-2.0.3/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1094 2024-05-10 21:22:12.000000 zerofun-2.0.3/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:37:14.389214 zerofun-2.0.3/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2956 2024-05-10 21:22:12.000000 zerofun-2.0.3/tests/test_process.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    17816 2024-05-10 23:37:05.000000 zerofun-2.0.3/tests/test_server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2198 2024-05-10 21:22:12.000000 zerofun-2.0.3/tests/test_thread.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:37:14.393214 zerofun-2.0.3/zerofun/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      575 2024-05-10 23:37:07.000000 zerofun-2.0.3/zerofun/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4839 2024-05-10 22:25:55.000000 zerofun-2.0.3/zerofun/client.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3753 2024-05-10 21:22:12.000000 zerofun-2.0.3/zerofun/proc_server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3240 2024-05-10 21:24:11.000000 zerofun-2.0.3/zerofun/process.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6273 2024-05-10 23:36:54.000000 zerofun-2.0.3/zerofun/server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7435 2024-05-10 22:22:24.000000 zerofun-2.0.3/zerofun/sockets.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2555 2024-05-10 21:24:04.000000 zerofun-2.0.3/zerofun/thread.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3628 2024-05-10 22:03:53.000000 zerofun-2.0.3/zerofun/utils.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:37:14.393214 zerofun-2.0.3/zerofun.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 23:37:14.000000 zerofun-2.0.3/zerofun.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      425 2024-05-10 23:37:14.000000 zerofun-2.0.3/zerofun.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-10 23:37:14.000000 zerofun-2.0.3/zerofun.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-10 23:37:14.000000 zerofun-2.0.3/zerofun.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        8 2024-05-10 23:37:14.000000 zerofun-2.0.3/zerofun.egg-info/top_level.txt
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:51:00.375347 zerofun-2.0.4/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1054 2024-05-10 21:22:12.000000 zerofun-2.0.4/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       25 2024-05-10 21:22:12.000000 zerofun-2.0.4/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 23:51:00.375347 zerofun-2.0.4/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3347 2024-05-10 21:22:12.000000 zerofun-2.0.4/README.md
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-10 22:33:14.000000 zerofun-2.0.4/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-10 23:51:00.379346 zerofun-2.0.4/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1094 2024-05-10 21:22:12.000000 zerofun-2.0.4/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:51:00.367346 zerofun-2.0.4/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2956 2024-05-10 21:22:12.000000 zerofun-2.0.4/tests/test_process.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    18944 2024-05-10 23:42:48.000000 zerofun-2.0.4/tests/test_server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2198 2024-05-10 21:22:12.000000 zerofun-2.0.4/tests/test_thread.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:51:00.371346 zerofun-2.0.4/zerofun/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      575 2024-05-10 23:50:43.000000 zerofun-2.0.4/zerofun/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4839 2024-05-10 22:25:55.000000 zerofun-2.0.4/zerofun/client.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3861 2024-05-10 23:50:39.000000 zerofun-2.0.4/zerofun/proc_server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3240 2024-05-10 21:24:11.000000 zerofun-2.0.4/zerofun/process.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6232 2024-05-10 23:46:28.000000 zerofun-2.0.4/zerofun/server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7435 2024-05-10 22:22:24.000000 zerofun-2.0.4/zerofun/sockets.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2555 2024-05-10 21:24:04.000000 zerofun-2.0.4/zerofun/thread.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3628 2024-05-10 22:03:53.000000 zerofun-2.0.4/zerofun/utils.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:51:00.375347 zerofun-2.0.4/zerofun.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 23:51:00.000000 zerofun-2.0.4/zerofun.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      425 2024-05-10 23:51:00.000000 zerofun-2.0.4/zerofun.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-10 23:51:00.000000 zerofun-2.0.4/zerofun.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-10 23:51:00.000000 zerofun-2.0.4/zerofun.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        8 2024-05-10 23:51:00.000000 zerofun-2.0.4/zerofun.egg-info/top_level.txt
```

### Comparing `zerofun-2.0.3/LICENSE` & `zerofun-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.3/PKG-INFO` & `zerofun-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerofun
-Version: 2.0.3
+Version: 2.0.4
 Summary: Remote function calls for array data using ZMQ
 Home-page: http://github.com/danijar/zerofun
 Author: Danijar Hafner
 Author-email: mail@danijar.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zerofun-2.0.3/README.md` & `zerofun-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.3/setup.py` & `zerofun-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.3/tests/test_process.py` & `zerofun-2.0.4/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.3/tests/test_server.py` & `zerofun-2.0.4/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -476,14 +476,47 @@
     with server:
       client.connect(retry=False, timeout=1)
       outdata = client.function(data).result()
       assert tree_equal(outdata, data)
 
   @pytest.mark.parametrize('Server', SERVERS)
   @pytest.mark.parametrize('addr', ADDRESSES)
+  @pytest.mark.parametrize('data', (
+      {'a': np.zeros((3, 2), np.float32), 'b': np.ones((1,), np.uint8)},
+      {'a': 12, 'b': [np.ones((1,), np.uint8), 13]},
+      {'a': 12, 'b': ['c', [1, 2, 3]]},
+      [],
+      {},
+      12,
+      [[{}, []]],
+  ))
+  def test_tree_data_batched(self, Server, addr, data):
+    data = elements.tree.map(np.asarray, data)
+    print(data)
+    def tree_equal(tree1, tree2):
+      try:
+        comps = elements.tree.map(lambda x, y: np.all(x == y), tree1, tree2)
+        comps, _ = elements.tree.flatten(comps)
+        return all(comps)
+      except TypeError:
+        return False
+    addr = addr.format(port=zerofun.get_free_port())
+    client = zerofun.Client(addr, pings=0, maxage=1)
+    server = Server(addr)
+    def workfn(indata):
+      return indata
+    server.bind('function', workfn, batch=4)
+    with server:
+      client.connect(retry=False, timeout=1)
+      futures = [client.function(data) for _ in range(4)]
+      for future in futures:
+        assert tree_equal(future.result(), data)
+
+  @pytest.mark.parametrize('Server', SERVERS)
+  @pytest.mark.parametrize('addr', ADDRESSES)
   def test_tree_none_result(self, Server, addr):
     addr = addr.format(port=zerofun.get_free_port())
     client = zerofun.Client(addr, pings=0, maxage=1)
     server = Server(addr)
     def workfn(indata):
       pass  # No return value
     server.bind('function', workfn)
```

### Comparing `zerofun-2.0.3/tests/test_thread.py` & `zerofun-2.0.4/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.3/zerofun/__init__.py` & `zerofun-2.0.4/zerofun/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.0.3'
+__version__ = '2.0.4'
 
 import multiprocessing as mp
 try:
   mp.set_start_method('spawn')
 except RuntimeError:
   pass
```

### Comparing `zerofun-2.0.3/zerofun/client.py` & `zerofun-2.0.4/zerofun/client.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.3/zerofun/proc_server.py` & `zerofun-2.0.4/zerofun/proc_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,25 +14,25 @@
   def __init__(
       self, address, name='Server', ipv6=False, workers=1, errors=True):
     self.address = address
     self.inner = f'ipc:///tmp/inner{np.random.randint(2 ** 32)}'
     self.name = name
     self.ipv6 = ipv6
     self.server = server.Server(self.inner, name, ipv6, workers, errors)
-    self.batches = {}
+    self.batchsizes = {}
     self.batcher = None
 
   def bind(self, name, workfn, logfn=None, workers=0, batch=0):
-    self.batches[name] = batch
+    self.batchsizes[name] = batch
     self.server.bind(name, workfn, logfn, workers, batch=0)
 
   def start(self):
     self.batcher = process.StoppableProcess(
         self._batcher, self.address, self.inner,
-        self.batches, self.name, self.ipv6, name='batcher', start=True)
+        self.batchsizes, self.name, self.ipv6, name='batcher', start=True)
     self.server.start()
 
   def check(self):
     self.batcher.check()
     self.server.check()
 
   def close(self):
@@ -55,72 +55,74 @@
     self.start()
     return self
 
   def __exit__(self, type, value, traceback):
     self.close()
 
   @staticmethod
-  def _batcher(context, address, inner, batches, name, ipv6):
+  def _batcher(context, address, inner, batchsizes, name, ipv6):
 
     socket = sockets.ServerSocket(address, ipv6)
     inbound = sockets.ClientSocket(identity=0, pings=0, maxage=0)
     inbound.connect(inner, timeout=120)
     queues = collections.defaultdict(list)
-    buffers = collections.defaultdict(dict)
+    buffers = {}
     pending = {}
     elements.print(f'[{name}] Listening at {address}')
 
     while context.running:
 
       result = socket.receive()
       if result:
         addr, rid, name, payload = result
-        batch = batches.get(name, None)
+        batch = batchsizes.get(name, None)
         if batch is not None:
           if batch:
             queue = queues[name]
             queue.append((addr, rid, payload))
             if len(queue) == batch:
               addrs, rids, payloads = zip(*queue)
               queue.clear()
               datas = [sockets.unpack(x) for x in payloads]
-              idx = range(batch)
-              bufs = buffers[name]
-              for key, value in datas[0].items():
-                bufs[key] = np.stack(
-                    [datas[i][key] for i in idx], out=bufs.get(key, None))
-              payload = sockets.pack(bufs)
+              if name not in buffers:
+                buffers[name] = buffer = elements.tree.map(
+                    lambda *xs: np.stack(xs), *datas)
+              else:
+                buffers[name] = buffer = elements.tree.map(
+                    lambda buf, *xs: np.stack(xs, buf=buf),
+                    buffers[name], *datas)
+              payload = sockets.pack(buffer)
               rid = inbound.send_call(name, payload)
               pending[rid] = (name, addrs, rids)
           else:
             inner_rid = inbound.send_call(name, payload)
             pending[inner_rid] = (name, addr, rid)
         else:
           socket.send_error(addr, rid, f'Unknown method {name}.')
 
       try:
         result = inbound.receive()
         if result:
           inner_rid, payload = result
           name, addr, rid = pending.pop(inner_rid)
-          if batches[name]:
+          if batchsizes[name]:
             addrs, rids = addr, rid
             result = sockets.unpack(payload)
             results = [
-                {k: v[i] for k, v in result.items()}
-                for i in range(batches[name])]
+                elements.tree.map(lambda x: x[i], result)
+                for i in range(batchsizes[name])]
             payloads = [sockets.pack(x) for x in results]
             for addr, rid, payload in zip(addrs, rids, payloads):
               socket.send_result(addr, rid, payload)
           else:
             socket.send_result(addr, rid, payload)
       except sockets.RemoteError as e:
         inner_rid, msg = e.args[:2]
         name, addr, rid = pending.pop(inner_rid)
-        if batches[name]:
+        if batchsizes[name]:
           addrs, rids = addr, rid
           for addr, rid in zip(addrs, rids):
             socket.send_error(addr, rid, msg)
         else:
           socket.send_error(addr, rid, msg)
 
     socket.close()
```

### Comparing `zerofun-2.0.3/zerofun/process.py` & `zerofun-2.0.4/zerofun/process.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.3/zerofun/server.py` & `zerofun-2.0.4/zerofun/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -177,29 +177,28 @@
       future = self.done_proms.popleft()
       future.result()
       future.method.inprog[0] -= 1
 
   def _work(self, method, addr, rid, payload, recvd):
     if method.batched:
       data = [sockets.unpack(x) for x in payload]
-      data = {
-          k: np.stack([data[i][k] for i in range(method.insize)])
-          for k, v in data[0].items()}
+      data = elements.tree.map(lambda *xs: np.stack(xs), *data)
     else:
       data = sockets.unpack(payload)
     if method.donefn:
       result, logs = method.workfn(data)
     else:
       result = method.workfn(data)
       if result is None:
         result = []
       logs = None
     if method.batched:
       results = [
-          {k: v[i] for k, v in result.items()} for i in range(method.insize)]
+          elements.tree.map(lambda x: x[i], result)
+          for i in range(method.insize)]
       payload = [sockets.pack(x) for x in results]
     else:
       payload = sockets.pack(result)
     return addr, rid, payload, logs, recvd
 
   def _print(self, text):
     elements.print(f'[{self.name}] {text}')
```

### Comparing `zerofun-2.0.3/zerofun/sockets.py` & `zerofun-2.0.4/zerofun/sockets.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.3/zerofun/thread.py` & `zerofun-2.0.4/zerofun/thread.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.3/zerofun/utils.py` & `zerofun-2.0.4/zerofun/utils.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.3/zerofun.egg-info/PKG-INFO` & `zerofun-2.0.4/zerofun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerofun
-Version: 2.0.3
+Version: 2.0.4
 Summary: Remote function calls for array data using ZMQ
 Home-page: http://github.com/danijar/zerofun
 Author: Danijar Hafner
 Author-email: mail@danijar.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

