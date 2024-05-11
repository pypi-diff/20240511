# Comparing `tmp/zerofun-2.0.4.tar.gz` & `tmp/zerofun-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerofun-2.0.4.tar", last modified: Fri May 10 23:51:00 2024, max compression
+gzip compressed data, was "zerofun-2.0.5.tar", last modified: Sat May 11 00:54:45 2024, max compression
```

## Comparing `zerofun-2.0.4.tar` & `zerofun-2.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:51:00.375347 zerofun-2.0.4/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1054 2024-05-10 21:22:12.000000 zerofun-2.0.4/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)       25 2024-05-10 21:22:12.000000 zerofun-2.0.4/MANIFEST.in
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 23:51:00.375347 zerofun-2.0.4/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3347 2024-05-10 21:22:12.000000 zerofun-2.0.4/README.md
--rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-10 22:33:14.000000 zerofun-2.0.4/requirements.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-10 23:51:00.379346 zerofun-2.0.4/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1094 2024-05-10 21:22:12.000000 zerofun-2.0.4/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:51:00.367346 zerofun-2.0.4/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2956 2024-05-10 21:22:12.000000 zerofun-2.0.4/tests/test_process.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    18944 2024-05-10 23:42:48.000000 zerofun-2.0.4/tests/test_server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2198 2024-05-10 21:22:12.000000 zerofun-2.0.4/tests/test_thread.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:51:00.371346 zerofun-2.0.4/zerofun/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      575 2024-05-10 23:50:43.000000 zerofun-2.0.4/zerofun/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4839 2024-05-10 22:25:55.000000 zerofun-2.0.4/zerofun/client.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3861 2024-05-10 23:50:39.000000 zerofun-2.0.4/zerofun/proc_server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3240 2024-05-10 21:24:11.000000 zerofun-2.0.4/zerofun/process.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6232 2024-05-10 23:46:28.000000 zerofun-2.0.4/zerofun/server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7435 2024-05-10 22:22:24.000000 zerofun-2.0.4/zerofun/sockets.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2555 2024-05-10 21:24:04.000000 zerofun-2.0.4/zerofun/thread.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3628 2024-05-10 22:03:53.000000 zerofun-2.0.4/zerofun/utils.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:51:00.375347 zerofun-2.0.4/zerofun.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 23:51:00.000000 zerofun-2.0.4/zerofun.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      425 2024-05-10 23:51:00.000000 zerofun-2.0.4/zerofun.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-10 23:51:00.000000 zerofun-2.0.4/zerofun.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-10 23:51:00.000000 zerofun-2.0.4/zerofun.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        8 2024-05-10 23:51:00.000000 zerofun-2.0.4/zerofun.egg-info/top_level.txt
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-11 00:54:45.175300 zerofun-2.0.5/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1054 2024-05-10 21:22:12.000000 zerofun-2.0.5/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       25 2024-05-10 21:22:12.000000 zerofun-2.0.5/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-11 00:54:45.175300 zerofun-2.0.5/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3347 2024-05-10 21:22:12.000000 zerofun-2.0.5/README.md
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-10 22:33:14.000000 zerofun-2.0.5/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-11 00:54:45.175300 zerofun-2.0.5/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1094 2024-05-10 21:22:12.000000 zerofun-2.0.5/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-11 00:54:45.171300 zerofun-2.0.5/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2956 2024-05-10 21:22:12.000000 zerofun-2.0.5/tests/test_process.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    18967 2024-05-11 00:54:29.000000 zerofun-2.0.5/tests/test_server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2198 2024-05-10 21:22:12.000000 zerofun-2.0.5/tests/test_thread.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-11 00:54:45.175300 zerofun-2.0.5/zerofun/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      575 2024-05-11 00:54:00.000000 zerofun-2.0.5/zerofun/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4839 2024-05-11 00:54:00.000000 zerofun-2.0.5/zerofun/client.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3861 2024-05-11 00:54:00.000000 zerofun-2.0.5/zerofun/proc_server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3240 2024-05-10 21:24:11.000000 zerofun-2.0.5/zerofun/process.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6232 2024-05-11 00:54:00.000000 zerofun-2.0.5/zerofun/server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7435 2024-05-10 22:22:24.000000 zerofun-2.0.5/zerofun/sockets.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2555 2024-05-10 21:24:04.000000 zerofun-2.0.5/zerofun/thread.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3628 2024-05-10 22:03:53.000000 zerofun-2.0.5/zerofun/utils.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-11 00:54:45.175300 zerofun-2.0.5/zerofun.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-11 00:54:45.000000 zerofun-2.0.5/zerofun.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      425 2024-05-11 00:54:45.000000 zerofun-2.0.5/zerofun.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-11 00:54:45.000000 zerofun-2.0.5/zerofun.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-11 00:54:45.000000 zerofun-2.0.5/zerofun.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        8 2024-05-11 00:54:45.000000 zerofun-2.0.5/zerofun.egg-info/top_level.txt
```

### Comparing `zerofun-2.0.4/LICENSE` & `zerofun-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.4/PKG-INFO` & `zerofun-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerofun
-Version: 2.0.4
+Version: 2.0.5
 Summary: Remote function calls for array data using ZMQ
 Home-page: http://github.com/danijar/zerofun
 Author: Danijar Hafner
 Author-email: mail@danijar.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zerofun-2.0.4/README.md` & `zerofun-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.4/setup.py` & `zerofun-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.4/tests/test_process.py` & `zerofun-2.0.5/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.4/tests/test_server.py` & `zerofun-2.0.5/tests/test_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,16 @@
       calls[0] += 1
       return data
     server = Server(addr)
     server.bind('function', function, batch=batch)
     with server:
       client = zerofun.Client(addr, pings=0, maxage=1)
       client.connect(retry=False, timeout=1)
-      futures = [client.function({'foo': [i]}) for i in range(batch)]
+      futures = [
+          client.function({'foo': np.asarray([i])}) for i in range(batch)]
       results = [future.result()['foo'][0] for future in futures]
       assert calls[0] == 1
       assert results == list(range(batch))
 
   @pytest.mark.parametrize('Server', SERVERS)
   @pytest.mark.parametrize('addr', ADDRESSES)
   @pytest.mark.parametrize('batch', (1, 2, 4))
```

### Comparing `zerofun-2.0.4/tests/test_thread.py` & `zerofun-2.0.5/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.4/zerofun/__init__.py` & `zerofun-2.0.5/zerofun/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.0.4'
+__version__ = '2.0.5'
 
 import multiprocessing as mp
 try:
   mp.set_start_method('spawn')
 except RuntimeError:
   pass
```

### Comparing `zerofun-2.0.4/zerofun/client.py` & `zerofun-2.0.5/zerofun/client.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.4/zerofun/proc_server.py` & `zerofun-2.0.5/zerofun/proc_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
               queue.clear()
               datas = [sockets.unpack(x) for x in payloads]
               if name not in buffers:
                 buffers[name] = buffer = elements.tree.map(
                     lambda *xs: np.stack(xs), *datas)
               else:
                 buffers[name] = buffer = elements.tree.map(
-                    lambda buf, *xs: np.stack(xs, buf=buf),
+                    lambda buf, *xs: np.stack(xs, out=buf),
                     buffers[name], *datas)
               payload = sockets.pack(buffer)
               rid = inbound.send_call(name, payload)
               pending[rid] = (name, addrs, rids)
           else:
             inner_rid = inbound.send_call(name, payload)
             pending[inner_rid] = (name, addr, rid)
```

### Comparing `zerofun-2.0.4/zerofun/process.py` & `zerofun-2.0.5/zerofun/process.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.4/zerofun/server.py` & `zerofun-2.0.5/zerofun/server.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.4/zerofun/sockets.py` & `zerofun-2.0.5/zerofun/sockets.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.4/zerofun/thread.py` & `zerofun-2.0.5/zerofun/thread.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.4/zerofun/utils.py` & `zerofun-2.0.5/zerofun/utils.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.4/zerofun.egg-info/PKG-INFO` & `zerofun-2.0.5/zerofun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerofun
-Version: 2.0.4
+Version: 2.0.5
 Summary: Remote function calls for array data using ZMQ
 Home-page: http://github.com/danijar/zerofun
 Author: Danijar Hafner
 Author-email: mail@danijar.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

