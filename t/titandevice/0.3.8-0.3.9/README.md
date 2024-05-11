# Comparing `tmp/titandevice-0.3.8.tar.gz` & `tmp/titandevice-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titandevice-0.3.8.tar", last modified: Sun Apr 28 01:53:26 2024, max compression
+gzip compressed data, was "titandevice-0.3.9.tar", last modified: Sun Apr 28 08:06:46 2024, max compression
```

## Comparing `titandevice-0.3.8.tar` & `titandevice-0.3.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:53:26.565587 titandevice-0.3.8/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-28 01:53:26.565587 titandevice-0.3.8/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 titandevice-0.3.8/README.md
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-28 01:53:26.565587 titandevice-0.3.8/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-28 01:52:55.000000 titandevice-0.3.8/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:53:26.565587 titandevice-0.3.8/titandevice/
--rw-rw-r--   0 mark      (1000) mark      (1000)     4190 2024-04-28 01:51:38.000000 titandevice-0.3.8/titandevice/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1415 2024-04-26 10:24:31.000000 titandevice-0.3.8/titandevice/_device_exception.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     7089 2024-04-28 01:52:55.000000 titandevice-0.3.8/titandevice/_device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      559 2024-04-25 06:30:48.000000 titandevice-0.3.8/titandevice/_device_models.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 01:53:26.565587 titandevice-0.3.8/titandevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-28 01:53:26.000000 titandevice-0.3.8/titandevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      310 2024-04-28 01:53:26.000000 titandevice-0.3.8/titandevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-28 01:53:26.000000 titandevice-0.3.8/titandevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-28 01:53:26.000000 titandevice-0.3.8/titandevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       12 2024-04-28 01:53:26.000000 titandevice-0.3.8/titandevice.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:06:46.419641 titandevice-0.3.9/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-28 08:06:46.419641 titandevice-0.3.9/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      184 2024-04-23 06:54:15.000000 titandevice-0.3.9/README.md
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-04-28 08:06:46.419641 titandevice-0.3.9/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-04-28 08:05:29.000000 titandevice-0.3.9/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:06:46.419641 titandevice-0.3.9/titandevice/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4601 2024-04-28 08:04:48.000000 titandevice-0.3.9/titandevice/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1415 2024-04-26 10:24:31.000000 titandevice-0.3.9/titandevice/_device_exception.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7089 2024-04-28 01:52:55.000000 titandevice-0.3.9/titandevice/_device_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      559 2024-04-25 06:30:48.000000 titandevice-0.3.9/titandevice/_device_models.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-04-28 08:06:46.419641 titandevice-0.3.9/titandevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      596 2024-04-28 08:06:46.000000 titandevice-0.3.9/titandevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      310 2024-04-28 08:06:46.000000 titandevice-0.3.9/titandevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-04-28 08:06:46.000000 titandevice-0.3.9/titandevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-04-28 08:06:46.000000 titandevice-0.3.9/titandevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       12 2024-04-28 08:06:46.000000 titandevice-0.3.9/titandevice.egg-info/top_level.txt
```

### Comparing `titandevice-0.3.8/PKG-INFO` & `titandevice-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titandevice
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `titandevice-0.3.8/setup.py` & `titandevice-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="titandevice",
-    version="0.3.8",
+    version="0.3.9",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `titandevice-0.3.8/titandevice/__init__.py` & `titandevice-0.3.9/titandevice/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,82 @@
 from ._device_exception import *
 from ._device_manager import _DeviceManager
 from ._device_models import DeviceInfo, FridaInfo, PackageInfo, RunningAppInfo
 
+__FRIDA_SERVER_NAME = 'frida-server'
+__FRIDA_SERVER_PATH = '/data/local/tmp/frida-server'
+
 device_manager_list: list[_DeviceManager] = _DeviceManager.get_all_device_manager_list()
 
 
+def get_frida_server_name():
+    return __FRIDA_SERVER_NAME
+
+
+def get_frida_server_path():
+    return __FRIDA_SERVER_PATH
+
+
+def set_frida_server_name(frida_server_name):
+    global __FRIDA_SERVER_NAME
+    __FRIDA_SERVER_NAME = frida_server_name
+
+
+def set_frida_server_path(frida_server_path):
+    global __FRIDA_SERVER_PATH
+    __FRIDA_SERVER_PATH = frida_server_path
+
+
 def get_all_devices() -> list[DeviceInfo]:
     global device_manager_list
     device_manager_list = _DeviceManager.get_all_device_manager_list()
     return [device.get_device_info() for device in device_manager_list]
 
 
 def get_frida_info(
         device_serial: str,
-        frida_server_name='frida-server',
-        frida_server_path='/data/local/tmp/frida-server'
+        frida_server_name=__FRIDA_SERVER_NAME,
+        frida_server_path=__FRIDA_SERVER_PATH
 ) -> FridaInfo:
     for device in device_manager_list:
         if device.get_device_info().serial == device_serial:
             return device.get_frida_info(frida_server_path, frida_server_name)
     raise DeviceNoFoundException(device_serial)
 
 
 def install_frida(
         device_serial: str, frida_server_path: str,
-        dist_path='/data/local/tmp/frida-server'
+        dist_path=__FRIDA_SERVER_PATH
 ) -> FridaInfo:
     for device in device_manager_list:
         if device.get_device_info().serial == device_serial:
             return device.install_frida(frida_server_path, dist_path)
     raise DeviceNoFoundException(device_serial)
 
 
 def start_frida(
-        device_serial: str, frida_server_path='/data/local/tmp/frida-server'
+        device_serial: str, frida_server_path=__FRIDA_SERVER_PATH
 ) -> FridaInfo:
     for device in device_manager_list:
         if device.get_device_info().serial == device_serial:
             return device.start_frida(frida_server_path)
     raise DeviceNoFoundException(device_serial)
 
 
 def stop_frida(
-        device_serial: str, frida_server_path='/data/local/tmp/frida-server'
+        device_serial: str, frida_server_path=__FRIDA_SERVER_PATH
 ) -> FridaInfo:
     for device in device_manager_list:
         if device.get_device_info().serial == device_serial:
             return device.stop_frida(frida_server_path)
     raise DeviceNoFoundException(device_serial)
 
 
 def uninstall_frida(
-        device_serial: str, frida_server_path='/data/local/tmp/frida-server'
+        device_serial: str, frida_server_path=__FRIDA_SERVER_PATH
 ) -> FridaInfo:
     for device in device_manager_list:
         if device.get_device_info().serial == device_serial:
             return device.uninstall_frida(frida_server_path)
     raise DeviceNoFoundException(device_serial)
```

### Comparing `titandevice-0.3.8/titandevice/_device_exception.py` & `titandevice-0.3.9/titandevice/_device_exception.py`

 * *Files identical despite different names*

### Comparing `titandevice-0.3.8/titandevice/_device_manager.py` & `titandevice-0.3.9/titandevice/_device_manager.py`

 * *Files identical despite different names*

### Comparing `titandevice-0.3.8/titandevice/_device_models.py` & `titandevice-0.3.9/titandevice/_device_models.py`

 * *Files identical despite different names*

### Comparing `titandevice-0.3.8/titandevice.egg-info/PKG-INFO` & `titandevice-0.3.9/titandevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titandevice
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

