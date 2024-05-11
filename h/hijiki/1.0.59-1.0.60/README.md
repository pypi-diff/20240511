# Comparing `tmp/hijiki-1.0.59.tar.gz` & `tmp/hijiki-1.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hijiki-1.0.59.tar", last modified: Thu May  2 20:03:02 2024, max compression
+gzip compressed data, was "hijiki-1.0.60.tar", last modified: Fri May 10 14:44:57 2024, max compression
```

## Comparing `hijiki-1.0.59.tar` & `hijiki-1.0.60.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.988008 hijiki-1.0.59/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 20:01:32.000000 hijiki-1.0.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-02 20:03:02.988008 hijiki-1.0.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-02 20:01:32.000000 hijiki-1.0.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.984008 hijiki-1.0.59/hijiki/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.984008 hijiki-1.0.59/hijiki/broker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/broker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/broker/broker_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/broker/hijiki_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/broker/hijiki_rabbit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.984008 hijiki-1.0.59/hijiki/decorator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/decorator/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/hijiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.984008 hijiki-1.0.59/hijiki/publisher/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/publisher/Publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:01:32.000000 hijiki-1.0.59/hijiki/publisher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.988008 hijiki-1.0.59/hijiki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-02 20:03:02.000000 hijiki-1.0.59/hijiki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-02 20:03:02.000000 hijiki-1.0.59/hijiki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:03:02.000000 hijiki-1.0.59/hijiki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 20:03:02.000000 hijiki-1.0.59/hijiki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 20:03:02.000000 hijiki-1.0.59/hijiki.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:03:02.988008 hijiki-1.0.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-02 20:02:06.000000 hijiki-1.0.59/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:03:02.988008 hijiki-1.0.59/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-02 20:01:32.000000 hijiki-1.0.59/tests/test_broker_data_server_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-02 20:01:32.000000 hijiki-1.0.59/tests/test_broker_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-02 20:01:32.000000 hijiki-1.0.59/tests/test_publisher_consumer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:44:57.165484 hijiki-1.0.60/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-10 14:43:34.000000 hijiki-1.0.60/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-10 14:44:57.165484 hijiki-1.0.60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-10 14:43:34.000000 hijiki-1.0.60/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:44:57.161483 hijiki-1.0.60/hijiki/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:43:34.000000 hijiki-1.0.60/hijiki/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:44:57.161483 hijiki-1.0.60/hijiki/broker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:43:34.000000 hijiki-1.0.60/hijiki/broker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-10 14:43:34.000000 hijiki-1.0.60/hijiki/broker/broker_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-10 14:43:34.000000 hijiki-1.0.60/hijiki/broker/hijiki_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-10 14:43:34.000000 hijiki-1.0.60/hijiki/broker/hijiki_rabbit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:44:57.165484 hijiki-1.0.60/hijiki/decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:43:34.000000 hijiki-1.0.60/hijiki/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-10 14:43:34.000000 hijiki-1.0.60/hijiki/decorator/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:43:34.000000 hijiki-1.0.60/hijiki/hijiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:44:57.165484 hijiki-1.0.60/hijiki/publisher/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-10 14:43:34.000000 hijiki-1.0.60/hijiki/publisher/Publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:43:34.000000 hijiki-1.0.60/hijiki/publisher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:44:57.165484 hijiki-1.0.60/hijiki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-10 14:44:57.000000 hijiki-1.0.60/hijiki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-10 14:44:57.000000 hijiki-1.0.60/hijiki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:44:57.000000 hijiki-1.0.60/hijiki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 14:44:57.000000 hijiki-1.0.60/hijiki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 14:44:57.000000 hijiki-1.0.60/hijiki.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:44:57.165484 hijiki-1.0.60/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-10 14:44:02.000000 hijiki-1.0.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:44:57.165484 hijiki-1.0.60/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-10 14:43:34.000000 hijiki-1.0.60/tests/test_broker_data_server_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-10 14:43:34.000000 hijiki-1.0.60/tests/test_broker_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-10 14:43:34.000000 hijiki-1.0.60/tests/test_publisher_consumer_test.py
```

### Comparing `hijiki-1.0.59/LICENSE` & `hijiki-1.0.60/LICENSE`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.59/PKG-INFO` & `hijiki-1.0.60/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hijiki
-Version: 1.0.59
+Version: 1.0.60
 Summary: Python Rabbit wrapper library to simplify to use Exchanges and Queues with decorators
 Author: Leandro Vilson Battisti
 Keywords: Celery,Kombu,RabbitMQ,decorator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: celery==5.3.4
 Requires-Dist: urllib3<2.0
```

### Comparing `hijiki-1.0.59/README.md` & `hijiki-1.0.60/README.md`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.59/hijiki/broker/broker_data.py` & `hijiki-1.0.60/hijiki/broker/broker_data.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.59/hijiki/broker/hijiki_broker.py` & `hijiki-1.0.60/hijiki/broker/hijiki_broker.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 from typing import Optional
 
 from hijiki.broker.broker_data import get_broker_url, init_os_environ
 
 
 class HijikiBroker:
     celery_broker = None
+    heartbeat = None
 
     def __init__(self, app_name, host, username, password, port, cluster_hosts, heartbeat: Optional[float] = 60):
         init_os_environ(host, username, password, port, cluster_hosts)
-        self.celery_broker = Celery(app_name, broker=get_broker_url(), set_as_current=True, heartbeat=heartbeat)
+        self.heartbeat = heartbeat
+        self.celery_broker = Celery(app_name, broker=get_broker_url(), set_as_current=True)
+
 
     def get_celery_broker(self):
         return self.celery_broker
 
     def ping(self):
         try:
             success_ping = False
```

### Comparing `hijiki-1.0.59/hijiki/broker/hijiki_rabbit.py` & `hijiki-1.0.60/hijiki/broker/hijiki_rabbit.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.59/hijiki/decorator/worker.py` & `hijiki-1.0.60/hijiki/decorator/worker.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.59/hijiki/publisher/Publisher.py` & `hijiki-1.0.60/hijiki/publisher/Publisher.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 class Publisher():
 
     def __init__(self, host, username, password, port, cluster_hosts: str = None, heartbeat: Optional[float] = 60):
         self.client = HijikiBroker('client', host, username, password, port, cluster_hosts, heartbeat=heartbeat)
 
     def publish_message(self, event_name: str, data: str):
         payload = {"value": data}
-        connection = self.client.get_celery_broker().broker_connection()
+        connection = self.client.get_celery_broker().broker_connection(heartbeat=self.client.heartbeat)
         with producers[connection].acquire(block=True) as producer:
             task_exchange = Exchange(event_name, type='topic')
             producer.publish(payload,  exchange=task_exchange, declare=[task_exchange], routing_key='x')
```

### Comparing `hijiki-1.0.59/hijiki.egg-info/PKG-INFO` & `hijiki-1.0.60/hijiki.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hijiki
-Version: 1.0.59
+Version: 1.0.60
 Summary: Python Rabbit wrapper library to simplify to use Exchanges and Queues with decorators
 Author: Leandro Vilson Battisti
 Keywords: Celery,Kombu,RabbitMQ,decorator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: celery==5.3.4
 Requires-Dist: urllib3<2.0
```

### Comparing `hijiki-1.0.59/hijiki.egg-info/SOURCES.txt` & `hijiki-1.0.60/hijiki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.59/tests/test_broker_data_server_exists.py` & `hijiki-1.0.60/tests/test_broker_data_server_exists.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.59/tests/test_broker_ping.py` & `hijiki-1.0.60/tests/test_broker_ping.py`

 * *Files identical despite different names*

### Comparing `hijiki-1.0.59/tests/test_publisher_consumer_test.py` & `hijiki-1.0.60/tests/test_publisher_consumer_test.py`

 * *Files identical despite different names*

