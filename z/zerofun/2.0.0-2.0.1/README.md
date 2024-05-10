# Comparing `tmp/zerofun-2.0.0.tar.gz` & `tmp/zerofun-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerofun-2.0.0.tar", last modified: Fri May 10 22:29:39 2024, max compression
+gzip compressed data, was "zerofun-2.0.1.tar", last modified: Fri May 10 22:50:12 2024, max compression
```

## Comparing `zerofun-2.0.0.tar` & `zerofun-2.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:29:39.649948 zerofun-2.0.0/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1054 2024-05-10 21:22:12.000000 zerofun-2.0.0/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)       25 2024-05-10 21:22:12.000000 zerofun-2.0.0/MANIFEST.in
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 22:29:39.649948 zerofun-2.0.0/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3347 2024-05-10 21:22:12.000000 zerofun-2.0.0/README.md
--rw-r-----   0 danijar  (322066) primarygroup (89939)       48 2024-05-10 22:03:51.000000 zerofun-2.0.0/requirements.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-10 22:29:39.649948 zerofun-2.0.0/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1094 2024-05-10 21:22:12.000000 zerofun-2.0.0/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:29:39.645948 zerofun-2.0.0/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2956 2024-05-10 21:22:12.000000 zerofun-2.0.0/tests/test_process.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    17320 2024-05-10 22:28:45.000000 zerofun-2.0.0/tests/test_server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2198 2024-05-10 21:22:12.000000 zerofun-2.0.0/tests/test_thread.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:29:39.649948 zerofun-2.0.0/zerofun/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      575 2024-05-10 22:29:02.000000 zerofun-2.0.0/zerofun/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4839 2024-05-10 22:25:55.000000 zerofun-2.0.0/zerofun/client.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3753 2024-05-10 21:22:12.000000 zerofun-2.0.0/zerofun/proc_server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3240 2024-05-10 21:24:11.000000 zerofun-2.0.0/zerofun/process.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6228 2024-05-10 22:28:32.000000 zerofun-2.0.0/zerofun/server.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7435 2024-05-10 22:22:24.000000 zerofun-2.0.0/zerofun/sockets.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2555 2024-05-10 21:24:04.000000 zerofun-2.0.0/zerofun/thread.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3628 2024-05-10 22:03:53.000000 zerofun-2.0.0/zerofun/utils.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:29:39.649948 zerofun-2.0.0/zerofun.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 22:29:39.000000 zerofun-2.0.0/zerofun.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      425 2024-05-10 22:29:39.000000 zerofun-2.0.0/zerofun.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-10 22:29:39.000000 zerofun-2.0.0/zerofun.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       48 2024-05-10 22:29:39.000000 zerofun-2.0.0/zerofun.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        8 2024-05-10 22:29:39.000000 zerofun-2.0.0/zerofun.egg-info/top_level.txt
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:50:12.055336 zerofun-2.0.1/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1054 2024-05-10 21:22:12.000000 zerofun-2.0.1/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       25 2024-05-10 21:22:12.000000 zerofun-2.0.1/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 22:50:12.055336 zerofun-2.0.1/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3347 2024-05-10 21:22:12.000000 zerofun-2.0.1/README.md
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-10 22:33:14.000000 zerofun-2.0.1/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-10 22:50:12.055336 zerofun-2.0.1/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1094 2024-05-10 21:22:12.000000 zerofun-2.0.1/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:50:12.051336 zerofun-2.0.1/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2956 2024-05-10 21:22:12.000000 zerofun-2.0.1/tests/test_process.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    17320 2024-05-10 22:28:45.000000 zerofun-2.0.1/tests/test_server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2198 2024-05-10 21:22:12.000000 zerofun-2.0.1/tests/test_thread.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:50:12.051336 zerofun-2.0.1/zerofun/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      575 2024-05-10 22:33:21.000000 zerofun-2.0.1/zerofun/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4839 2024-05-10 22:25:55.000000 zerofun-2.0.1/zerofun/client.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3753 2024-05-10 21:22:12.000000 zerofun-2.0.1/zerofun/proc_server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3240 2024-05-10 21:24:11.000000 zerofun-2.0.1/zerofun/process.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6228 2024-05-10 22:28:32.000000 zerofun-2.0.1/zerofun/server.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7435 2024-05-10 22:22:24.000000 zerofun-2.0.1/zerofun/sockets.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2555 2024-05-10 21:24:04.000000 zerofun-2.0.1/zerofun/thread.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3628 2024-05-10 22:03:53.000000 zerofun-2.0.1/zerofun/utils.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:50:12.055336 zerofun-2.0.1/zerofun.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3765 2024-05-10 22:50:11.000000 zerofun-2.0.1/zerofun.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      425 2024-05-10 22:50:12.000000 zerofun-2.0.1/zerofun.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-10 22:50:11.000000 zerofun-2.0.1/zerofun.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       55 2024-05-10 22:50:11.000000 zerofun-2.0.1/zerofun.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        8 2024-05-10 22:50:11.000000 zerofun-2.0.1/zerofun.egg-info/top_level.txt
```

### Comparing `zerofun-2.0.0/LICENSE` & `zerofun-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.0/PKG-INFO` & `zerofun-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerofun
-Version: 2.0.0
+Version: 2.0.1
 Summary: Remote function calls for array data using ZMQ
 Home-page: http://github.com/danijar/zerofun
 Author: Danijar Hafner
 Author-email: mail@danijar.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zerofun-2.0.0/README.md` & `zerofun-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.0/setup.py` & `zerofun-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.0/tests/test_process.py` & `zerofun-2.0.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.0/tests/test_server.py` & `zerofun-2.0.1/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.0/tests/test_thread.py` & `zerofun-2.0.1/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.0/zerofun/__init__.py` & `zerofun-2.0.1/zerofun/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 
 import multiprocessing as mp
 try:
   mp.set_start_method('spawn')
 except RuntimeError:
   pass
```

### Comparing `zerofun-2.0.0/zerofun/client.py` & `zerofun-2.0.1/zerofun/client.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.0/zerofun/proc_server.py` & `zerofun-2.0.1/zerofun/proc_server.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.0/zerofun/process.py` & `zerofun-2.0.1/zerofun/process.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.0/zerofun/server.py` & `zerofun-2.0.1/zerofun/server.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.0/zerofun/sockets.py` & `zerofun-2.0.1/zerofun/sockets.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.0/zerofun/thread.py` & `zerofun-2.0.1/zerofun/thread.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.0/zerofun/utils.py` & `zerofun-2.0.1/zerofun/utils.py`

 * *Files identical despite different names*

### Comparing `zerofun-2.0.0/zerofun.egg-info/PKG-INFO` & `zerofun-2.0.1/zerofun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerofun
-Version: 2.0.0
+Version: 2.0.1
 Summary: Remote function calls for array data using ZMQ
 Home-page: http://github.com/danijar/zerofun
 Author: Danijar Hafner
 Author-email: mail@danijar.com
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

