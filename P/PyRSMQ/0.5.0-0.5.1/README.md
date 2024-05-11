# Comparing `tmp/PyRSMQ-0.5.0.tar.gz` & `tmp/pyrsmq-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyRSMQ-0.5.0.tar", last modified: Sat Oct 14 04:04:40 2023, max compression
+gzip compressed data, was "pyrsmq-0.5.1.tar", last modified: Sat May 11 04:29:32 2024, max compression
```

## Comparing `PyRSMQ-0.5.0.tar` & `pyrsmq-0.5.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    18274 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    17803 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5391 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/examples/consumer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5685 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/examples/consumer_thread.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1382 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/examples/example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4016 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/examples/producer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      361 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/package.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1526 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/src/PyRSMQ.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18274 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/src/PyRSMQ.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      897 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/src/PyRSMQ.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/src/PyRSMQ.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/src/PyRSMQ.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/src/PyRSMQ.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/src/rsmq/
--rw-rw-r--   0 travis    (2000) travis    (2000)      271 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/src/rsmq/cmd/
--rw-rw-r--   0 travis    (2000) travis    (2000)      555 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7712 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/base_command.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      991 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/change_message_visibility.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1153 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/create_queue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      981 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/delete_message.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      840 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/delete_queue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1359 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1463 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/get_queue_attributes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      430 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/list_queues.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      769 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/pop_message.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      941 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/receive_message.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1561 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/send_message.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1139 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/set_queue_attributes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2578 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/cmd/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1905 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/const.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7945 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/consumer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5678 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/rsmq/rsmq.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-10-14 04:04:40.000000 PyRSMQ-0.5.0/src/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8205 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/tests/test_rsmq.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5207 2023-10-14 04:03:35.000000 PyRSMQ-0.5.0/src/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:29:32.405229 pyrsmq-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18369 2024-05-11 04:29:32.401229 pyrsmq-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:29:32.397229 pyrsmq-0.5.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/examples/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/examples/consumer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/examples/producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/package.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 04:29:32.405229 pyrsmq-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:29:32.397229 pyrsmq-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:29:32.401229 pyrsmq-0.5.1/src/PyRSMQ.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18369 2024-05-11 04:29:32.000000 pyrsmq-0.5.1/src/PyRSMQ.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-11 04:29:32.000000 pyrsmq-0.5.1/src/PyRSMQ.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 04:29:32.000000 pyrsmq-0.5.1/src/PyRSMQ.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 04:29:32.000000 pyrsmq-0.5.1/src/PyRSMQ.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 04:29:32.000000 pyrsmq-0.5.1/src/PyRSMQ.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:29:32.401229 pyrsmq-0.5.1/src/rsmq/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:29:32.401229 pyrsmq-0.5.1/src/rsmq/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/base_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/change_message_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/create_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/delete_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/delete_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/get_queue_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/list_queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/pop_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/receive_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/set_queue_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/cmd/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/rsmq/rsmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:29:32.401229 pyrsmq-0.5.1/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/tests/test_rsmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-11 04:29:18.000000 pyrsmq-0.5.1/src/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyRSMQ-0.5.0/LICENSE` & `pyrsmq-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/PKG-INFO` & `pyrsmq-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: PyRSMQ
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Implementation of Redis SMQ
 Home-page: https://mlasevich.github.io/PyRSMQ/
 Author: Michael Lasevich
 Author-email: mlasevich+pyrsmq@gmail.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: redis
 
 ![RSMQ: Redis Simple Message Queue for Node.js](https://img.webmart.de/rsmq_wide.png)
 
 [![Build Status](https://travis-ci.org/mlasevich/PyRSMQ.svg?branch=master)](https://travis-ci.org/mlasevich/PyRSMQ)
 [![Coverage Status](https://coveralls.io/repos/github/mlasevich/PyRSMQ/badge.svg?branch=master)](https://coveralls.io/github/mlasevich/PyRSMQ?branch=master)
 [![PyPI version](https://badge.fury.io/py/PyRSMQ.svg)](https://badge.fury.io/py/PyRSMQ)
 
@@ -23,14 +24,17 @@
 
 A lightweight message queue for Python that requires no dedicated queue server. Just a Redis server.
 
 This is a Python implementation of [https://github.com/smrchy/rsmq](https://github.com/smrchy/rsmq))
 
 
 ## PyRSMQ Release Notes
+* 0.5.1
+   * Bugfix: Fix crash on non-existent queue name (Thanks @rwl4)
+
 * 0.5.0
     * Require Python 3.6+
     * Code cleanup
     * Fix for scenario where consumer breaks if redis is restarted (#4)
 
 * 0.4.5
   * Re-release to push to PyPi
```

### Comparing `PyRSMQ-0.5.0/README.md` & `pyrsmq-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 A lightweight message queue for Python that requires no dedicated queue server. Just a Redis server.
 
 This is a Python implementation of [https://github.com/smrchy/rsmq](https://github.com/smrchy/rsmq))
 
 
 ## PyRSMQ Release Notes
+* 0.5.1
+   * Bugfix: Fix crash on non-existent queue name (Thanks @rwl4)
+
 * 0.5.0
     * Require Python 3.6+
     * Code cleanup
     * Fix for scenario where consumer breaks if redis is restarted (#4)
 
 * 0.4.5
   * Re-release to push to PyPi
```

### Comparing `PyRSMQ-0.5.0/examples/consumer.py` & `pyrsmq-0.5.1/examples/consumer.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/examples/consumer_thread.py` & `pyrsmq-0.5.1/examples/consumer_thread.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/examples/example.py` & `pyrsmq-0.5.1/examples/example.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/examples/producer.py` & `pyrsmq-0.5.1/examples/producer.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/setup.py` & `pyrsmq-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/PyRSMQ.egg-info/PKG-INFO` & `pyrsmq-0.5.1/src/PyRSMQ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: PyRSMQ
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Implementation of Redis SMQ
 Home-page: https://mlasevich.github.io/PyRSMQ/
 Author: Michael Lasevich
 Author-email: mlasevich+pyrsmq@gmail.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: redis
 
 ![RSMQ: Redis Simple Message Queue for Node.js](https://img.webmart.de/rsmq_wide.png)
 
 [![Build Status](https://travis-ci.org/mlasevich/PyRSMQ.svg?branch=master)](https://travis-ci.org/mlasevich/PyRSMQ)
 [![Coverage Status](https://coveralls.io/repos/github/mlasevich/PyRSMQ/badge.svg?branch=master)](https://coveralls.io/github/mlasevich/PyRSMQ?branch=master)
 [![PyPI version](https://badge.fury.io/py/PyRSMQ.svg)](https://badge.fury.io/py/PyRSMQ)
 
@@ -23,14 +24,17 @@
 
 A lightweight message queue for Python that requires no dedicated queue server. Just a Redis server.
 
 This is a Python implementation of [https://github.com/smrchy/rsmq](https://github.com/smrchy/rsmq))
 
 
 ## PyRSMQ Release Notes
+* 0.5.1
+   * Bugfix: Fix crash on non-existent queue name (Thanks @rwl4)
+
 * 0.5.0
     * Require Python 3.6+
     * Code cleanup
     * Fix for scenario where consumer breaks if redis is restarted (#4)
 
 * 0.4.5
   * Re-release to push to PyPi
```

### Comparing `PyRSMQ-0.5.0/src/PyRSMQ.egg-info/SOURCES.txt` & `pyrsmq-0.5.1/src/PyRSMQ.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/cmd/__init__.py` & `pyrsmq-0.5.1/src/rsmq/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/cmd/base_command.py` & `pyrsmq-0.5.1/src/rsmq/cmd/base_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
         tx = self.client.pipeline(transaction=True)
         tx.hmget(queue_key, "vt", "delay", "maxsize")
         tx.time()
 
         results = tx.execute()
 
         if not results or results[0][0] is None:
-            raise QueueDoesNotExist(self.get_queue)
+            raise QueueDoesNotExist(self.get_qname)
         stats = results[0]
         redis_time = results[1]
 
         ts_usec = redis_time[0] * 1000000 + redis_time[1]
         ts = int(ts_usec / 1000)
 
         return {
```

### Comparing `PyRSMQ-0.5.0/src/rsmq/cmd/change_message_visibility.py` & `pyrsmq-0.5.1/src/rsmq/cmd/change_message_visibility.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/cmd/create_queue.py` & `pyrsmq-0.5.1/src/rsmq/cmd/create_queue.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/cmd/delete_message.py` & `pyrsmq-0.5.1/src/rsmq/cmd/delete_message.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/cmd/delete_queue.py` & `pyrsmq-0.5.1/src/rsmq/cmd/delete_queue.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/cmd/exceptions.py` & `pyrsmq-0.5.1/src/rsmq/cmd/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/cmd/get_queue_attributes.py` & `pyrsmq-0.5.1/src/rsmq/cmd/get_queue_attributes.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/cmd/pop_message.py` & `pyrsmq-0.5.1/src/rsmq/cmd/pop_message.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/cmd/receive_message.py` & `pyrsmq-0.5.1/src/rsmq/cmd/receive_message.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/cmd/send_message.py` & `pyrsmq-0.5.1/src/rsmq/cmd/send_message.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/cmd/set_queue_attributes.py` & `pyrsmq-0.5.1/src/rsmq/cmd/set_queue_attributes.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/cmd/utils.py` & `pyrsmq-0.5.1/src/rsmq/cmd/utils.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/const.py` & `pyrsmq-0.5.1/src/rsmq/const.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/consumer.py` & `pyrsmq-0.5.1/src/rsmq/consumer.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/rsmq/rsmq.py` & `pyrsmq-0.5.1/src/rsmq/rsmq.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/tests/test_rsmq.py` & `pyrsmq-0.5.1/src/tests/test_rsmq.py`

 * *Files identical despite different names*

### Comparing `PyRSMQ-0.5.0/src/tests/test_utils.py` & `pyrsmq-0.5.1/src/tests/test_utils.py`

 * *Files identical despite different names*

