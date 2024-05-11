# Comparing `tmp/flops_utils-0.3.6.tar.gz` & `tmp/flops_utils-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.3.6.tar", max compression
+gzip compressed data, was "flops_utils-0.3.7.tar", max compression
```

## Comparing `flops_utils-0.3.6.tar` & `flops_utils-0.3.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.3.6/README.md
--rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.3.6/flops_utils/logging.py
--rw-r--r--   0        0        0      782 2024-05-05 12:55:14.703088 flops_utils-0.3.6/flops_utils/ml_model_flavor_wrapper.py
--rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.3.6/flops_utils/ml_repo_files_wrapper.py
--rw-r--r--   0        0        0     2632 2024-05-05 10:09:52.795212 flops_utils-0.3.6/flops_utils/ml_repo_templates.py
--rw-r--r--   0        0        0     1393 2024-04-24 16:17:22.077103 flops_utils-0.3.6/flops_utils/notifications.py
--rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.3.6/flops_utils/types.py
--rw-r--r--   0        0        0      435 2024-05-05 12:55:23.499088 flops_utils-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.3.7/README.md
+-rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.3.7/flops_utils/logging.py
+-rw-r--r--   0        0        0      782 2024-05-05 12:55:14.703088 flops_utils-0.3.7/flops_utils/ml_model_flavor_wrapper.py
+-rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.3.7/flops_utils/ml_repo_files_wrapper.py
+-rw-r--r--   0        0        0     2632 2024-05-05 10:09:52.795212 flops_utils-0.3.7/flops_utils/ml_repo_templates.py
+-rw-r--r--   0        0        0     1441 2024-05-11 09:55:30.969946 flops_utils-0.3.7/flops_utils/notifications.py
+-rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.3.7/flops_utils/types.py
+-rw-r--r--   0        0        0      435 2024-05-11 09:55:37.385946 flops_utils-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.3.7/PKG-INFO
```

### Comparing `flops_utils-0.3.6/flops_utils/logging.py` & `flops_utils-0.3.7/flops_utils/logging.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.3.6/flops_utils/ml_model_flavor_wrapper.py` & `flops_utils-0.3.7/flops_utils/ml_model_flavor_wrapper.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.3.6/flops_utils/ml_repo_templates.py` & `flops_utils-0.3.7/flops_utils/ml_repo_templates.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.3.6/flops_utils/notifications.py` & `flops_utils-0.3.7/flops_utils/notifications.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import socket
 import sys
 
 import paho.mqtt.client as paho_mqtt
 from flops_utils.logging import logger
 
 
-def notify_flops_ui(flops_ui_ip: str, msg: str) -> None:
-    logger.debug(f"Sending message to FLOps UI: {msg}")
+def notify_project_observer(project_observer_ip: str, msg: str) -> None:
+    logger.debug(f"Sending message to the project observer: {msg}")
     client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    client_socket.connect((flops_ui_ip, 2727))
+    client_socket.connect((project_observer_ip, 2727))
     client_socket.send(msg.encode())
     client_socket.close()
-    logger.debug(f"Send message to FLOps UI: {msg}")
+    logger.debug(f"Send message to the project observer: {msg}")
     sys.stdout.flush()
 
 
 def notify_flops_manager(
     flops_project_id: str,
     mqtt_ip: str,
     topic: str,
```

