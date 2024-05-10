# Comparing `tmp/zerofun-2.0.2.tar.gz` & `tmp/zerofun-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerofun-2.0.2.tar", last modified: Fri May 10 23:32:38 2024, max compression
+gzip compressed data, was "zerofun-2.0.3.tar", last modified: Fri May 10 23:37:14 2024, max compression
```

## Comparing `zerofun-2.0.2.tar` & `zerofun-2.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:32:38.325873 zerofun-2.0.2/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1054 2024-05-10 21:22:12.000000 zerofun-2.0.2/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)       25 2024-05-10 21:22:12.000000 zerofun-2.0.2/MANIFEST.in
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 23:32:38.325873 zerofun-2.0.2/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3347 2024-05-10 21:22:12.000000 zerofun-2.0.2/README.md
--rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-10 22:33:14.000000 zerofun-2.0.2/requirements.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-10 23:32:38.325873 zerofun-2.0.2/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1094 2024-05-10 21:22:12.000000 zerofun-2.0.2/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:32:38.321874 zerofun-2.0.2/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2956 2024-05-10 21:22:12.000000 zerofun-2.0.2/tests/test_process.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    17320 2024-05-10 22:28:45.000000 zerofun-2.0.2/tests/test_server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2198 2024-05-10 21:22:12.000000 zerofun-2.0.2/tests/test_thread.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:32:38.325873 zerofun-2.0.2/zerofun/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      575 2024-05-10 23:32:25.000000 zerofun-2.0.2/zerofun/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4839 2024-05-10 22:25:55.000000 zerofun-2.0.2/zerofun/client.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3753 2024-05-10 21:22:12.000000 zerofun-2.0.2/zerofun/proc_server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3240 2024-05-10 21:24:11.000000 zerofun-2.0.2/zerofun/process.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6273 2024-05-10 23:32:22.000000 zerofun-2.0.2/zerofun/server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7435 2024-05-10 22:22:24.000000 zerofun-2.0.2/zerofun/sockets.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2555 2024-05-10 21:24:04.000000 zerofun-2.0.2/zerofun/thread.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3628 2024-05-10 22:03:53.000000 zerofun-2.0.2/zerofun/utils.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:32:38.325873 zerofun-2.0.2/zerofun.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 23:32:38.000000 zerofun-2.0.2/zerofun.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      425 2024-05-10 23:32:38.000000 zerofun-2.0.2/zerofun.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-10 23:32:38.000000 zerofun-2.0.2/zerofun.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-10 23:32:38.000000 zerofun-2.0.2/zerofun.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        8 2024-05-10 23:32:38.000000 zerofun-2.0.2/zerofun.egg-info/top_level.txt
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:37:14.393214 zerofun-2.0.3/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1054 2024-05-10 21:22:12.000000 zerofun-2.0.3/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       25 2024-05-10 21:22:12.000000 zerofun-2.0.3/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 23:37:14.393214 zerofun-2.0.3/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3347 2024-05-10 21:22:12.000000 zerofun-2.0.3/README.md
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-10 22:33:14.000000 zerofun-2.0.3/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-10 23:37:14.393214 zerofun-2.0.3/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1094 2024-05-10 21:22:12.000000 zerofun-2.0.3/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:37:14.389214 zerofun-2.0.3/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2956 2024-05-10 21:22:12.000000 zerofun-2.0.3/tests/test_process.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    17816 2024-05-10 23:37:05.000000 zerofun-2.0.3/tests/test_server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2198 2024-05-10 21:22:12.000000 zerofun-2.0.3/tests/test_thread.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:37:14.393214 zerofun-2.0.3/zerofun/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      575 2024-05-10 23:37:07.000000 zerofun-2.0.3/zerofun/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4839 2024-05-10 22:25:55.000000 zerofun-2.0.3/zerofun/client.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3753 2024-05-10 21:22:12.000000 zerofun-2.0.3/zerofun/proc_server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3240 2024-05-10 21:24:11.000000 zerofun-2.0.3/zerofun/process.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6273 2024-05-10 23:36:54.000000 zerofun-2.0.3/zerofun/server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7435 2024-05-10 22:22:24.000000 zerofun-2.0.3/zerofun/sockets.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2555 2024-05-10 21:24:04.000000 zerofun-2.0.3/zerofun/thread.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3628 2024-05-10 22:03:53.000000 zerofun-2.0.3/zerofun/utils.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 23:37:14.393214 zerofun-2.0.3/zerofun.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 23:37:14.000000 zerofun-2.0.3/zerofun.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      425 2024-05-10 23:37:14.000000 zerofun-2.0.3/zerofun.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-10 23:37:14.000000 zerofun-2.0.3/zerofun.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-10 23:37:14.000000 zerofun-2.0.3/zerofun.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        8 2024-05-10 23:37:14.000000 zerofun-2.0.3/zerofun.egg-info/top_level.txt
```

### Comparing `zerofun-2.0.2/LICENSE` & `zerofun-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.2/PKG-INFO` & `zerofun-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerofun
-Version: 2.0.2
+Version: 2.0.3
 Summary: Remote function calls for array data using ZMQ
 Home-page: http://github.com/danijar/zerofun
 Author: Danijar Hafner
 Author-email: mail@danijar.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zerofun-2.0.2/README.md` & `zerofun-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.2/setup.py` & `zerofun-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.2/tests/test_process.py` & `zerofun-2.0.3/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.2/tests/test_server.py` & `zerofun-2.0.3/tests/test_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,7 +473,21 @@
       assert tree_equal(indata, data)
       return indata
     server.bind('function', workfn)
     with server:
       client.connect(retry=False, timeout=1)
       outdata = client.function(data).result()
       assert tree_equal(outdata, data)
+
+  @pytest.mark.parametrize('Server', SERVERS)
+  @pytest.mark.parametrize('addr', ADDRESSES)
+  def test_tree_none_result(self, Server, addr):
+    addr = addr.format(port=zerofun.get_free_port())
+    client = zerofun.Client(addr, pings=0, maxage=1)
+    server = Server(addr)
+    def workfn(indata):
+      pass  # No return value
+    server.bind('function', workfn)
+    with server:
+      client.connect(retry=False, timeout=1)
+      result = client.function([]).result()
+      assert result == []
```

### Comparing `zerofun-2.0.2/tests/test_thread.py` & `zerofun-2.0.3/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.2/zerofun/__init__.py` & `zerofun-2.0.3/zerofun/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.0.2'
+__version__ = '2.0.3'
 
 import multiprocessing as mp
 try:
   mp.set_start_method('spawn')
 except RuntimeError:
   pass
```

### Comparing `zerofun-2.0.2/zerofun/client.py` & `zerofun-2.0.3/zerofun/client.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.2/zerofun/proc_server.py` & `zerofun-2.0.3/zerofun/proc_server.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.2/zerofun/process.py` & `zerofun-2.0.3/zerofun/process.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.2/zerofun/server.py` & `zerofun-2.0.3/zerofun/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     else:
       data = sockets.unpack(payload)
     if method.donefn:
       result, logs = method.workfn(data)
     else:
       result = method.workfn(data)
       if result is None:
-        result = {}
+        result = []
       logs = None
     if method.batched:
       results = [
           {k: v[i] for k, v in result.items()} for i in range(method.insize)]
       payload = [sockets.pack(x) for x in results]
     else:
       payload = sockets.pack(result)
```

### Comparing `zerofun-2.0.2/zerofun/sockets.py` & `zerofun-2.0.3/zerofun/sockets.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.2/zerofun/thread.py` & `zerofun-2.0.3/zerofun/thread.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.2/zerofun/utils.py` & `zerofun-2.0.3/zerofun/utils.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.2/zerofun.egg-info/PKG-INFO` & `zerofun-2.0.3/zerofun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerofun
-Version: 2.0.2
+Version: 2.0.3
 Summary: Remote function calls for array data using ZMQ
 Home-page: http://github.com/danijar/zerofun
 Author: Danijar Hafner
 Author-email: mail@danijar.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

