# Comparing `tmp/codex-engine-pyqt-0.1.0.tar.gz` & `tmp/codex_engine_pyqt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codex-engine-pyqt-0.1.0.tar", last modified: Wed Aug  2 04:29:07 2023, max compression
+gzip compressed data, was "codex_engine_pyqt-0.1.1.tar", last modified: Sat May 11 19:21:09 2024, max compression
```

## Comparing `codex-engine-pyqt-0.1.0.tar` & `codex_engine_pyqt-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 04:29:07.302837 codex-engine-pyqt-0.1.0/
--rw-rw-rw-   0        0        0     1090 2021-03-18 09:51:15.000000 codex-engine-pyqt-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1385 2023-08-02 04:29:07.302837 codex-engine-pyqt-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      423 2021-03-18 09:51:15.000000 codex-engine-pyqt-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 04:29:07.246340 codex-engine-pyqt-0.1.0/codex/
--rw-rw-rw-   0        0        0      519 2023-08-02 03:15:29.000000 codex-engine-pyqt-0.1.0/codex/__init__.py
--rw-rw-rw-   0        0        0     5156 2021-03-25 16:06:34.000000 codex-engine-pyqt-0.1.0/codex/bundles.py
--rw-rw-rw-   0        0        0      340 2021-03-25 16:06:34.000000 codex-engine-pyqt-0.1.0/codex/console_device.py
--rw-rw-rw-   0        0        0    10489 2023-03-03 07:13:57.000000 codex-engine-pyqt-0.1.0/codex/device_controls.py
--rw-rw-rw-   0        0        0     5451 2023-04-20 02:44:02.000000 codex-engine-pyqt-0.1.0/codex/device_manager.py
--rw-rw-rw-   0        0        0      797 2021-03-18 09:51:15.000000 codex-engine-pyqt-0.1.0/codex/dummy_serial.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:29:07.255840 codex-engine-pyqt-0.1.0/codex/filters/
--rw-rw-rw-   0        0        0      162 2021-03-25 03:47:34.000000 codex-engine-pyqt-0.1.0/codex/filters/__init__.py
--rw-rw-rw-   0        0        0      697 2021-03-25 03:47:34.000000 codex-engine-pyqt-0.1.0/codex/filters/delimiter_filter.py
--rw-rw-rw-   0        0        0      811 2021-03-25 03:47:34.000000 codex-engine-pyqt-0.1.0/codex/filters/judi_filter.py
--rw-rw-rw-   0        0        0      358 2021-03-25 03:47:34.000000 codex-engine-pyqt-0.1.0/codex/filters/newline_filter.py
--rw-rw-rw-   0        0        0      300 2021-03-25 03:47:34.000000 codex-engine-pyqt-0.1.0/codex/filters/null_filter.py
--rw-rw-rw-   0        0        0     1105 2021-03-25 03:47:34.000000 codex-engine-pyqt-0.1.0/codex/judi_mixin.py
--rw-rw-rw-   0        0        0      627 2021-03-18 09:51:15.000000 codex-engine-pyqt-0.1.0/codex/judi_responder.py
--rw-rw-rw-   0        0        0      980 2023-08-02 04:22:47.000000 codex-engine-pyqt-0.1.0/codex/local_serial.py
--rw-rw-rw-   0        0        0     1032 2022-05-01 00:26:31.000000 codex-engine-pyqt-0.1.0/codex/remote_serial.py
--rw-rw-rw-   0        0        0     3550 2023-08-02 03:15:29.000000 codex-engine-pyqt-0.1.0/codex/serial_device.py
--rw-rw-rw-   0        0        0     5543 2023-08-02 04:25:14.000000 codex-engine-pyqt-0.1.0/codex/serial_device_base.py
--rw-rw-rw-   0        0        0     4405 2021-03-25 16:06:34.000000 codex-engine-pyqt-0.1.0/codex/subscriptions.py
--rw-rw-rw-   0        0        0     3236 2022-12-09 04:35:48.000000 codex-engine-pyqt-0.1.0/codex/unknown_device.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:29:07.301338 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/
--rw-rw-rw-   0        0        0     1385 2023-08-02 04:29:07.000000 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      747 2023-08-02 04:29:07.000000 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 04:29:07.000000 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-09 04:36:59.000000 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2023-08-02 04:29:07.000000 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-02 04:29:07.000000 codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1151 2023-08-02 04:29:07.304840 codex-engine-pyqt-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       96 2022-12-09 04:23:09.000000 codex-engine-pyqt-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 19:21:09.585569 codex_engine_pyqt-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2021-03-18 09:51:15.000000 codex_engine_pyqt-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1812 2024-05-11 19:21:09.585070 codex_engine_pyqt-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      801 2024-04-03 18:07:53.000000 codex_engine_pyqt-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 19:21:09.548572 codex_engine_pyqt-0.1.1/codex/
+-rw-rw-rw-   0        0        0      519 2023-08-02 03:15:29.000000 codex_engine_pyqt-0.1.1/codex/__init__.py
+-rw-rw-rw-   0        0        0     5156 2021-03-25 16:06:34.000000 codex_engine_pyqt-0.1.1/codex/bundles.py
+-rw-rw-rw-   0        0        0      340 2021-03-25 16:06:34.000000 codex_engine_pyqt-0.1.1/codex/console_device.py
+-rw-rw-rw-   0        0        0    10489 2023-03-03 07:13:57.000000 codex_engine_pyqt-0.1.1/codex/device_controls.py
+-rw-rw-rw-   0        0        0     5451 2024-05-11 17:57:48.000000 codex_engine_pyqt-0.1.1/codex/device_manager.py
+-rw-rw-rw-   0        0        0      797 2021-03-18 09:51:15.000000 codex_engine_pyqt-0.1.1/codex/dummy_serial.py
+drwxrwxrwx   0        0        0        0 2024-05-11 19:21:09.554570 codex_engine_pyqt-0.1.1/codex/filters/
+-rw-rw-rw-   0        0        0      162 2021-03-25 03:47:34.000000 codex_engine_pyqt-0.1.1/codex/filters/__init__.py
+-rw-rw-rw-   0        0        0      697 2021-03-25 03:47:34.000000 codex_engine_pyqt-0.1.1/codex/filters/delimiter_filter.py
+-rw-rw-rw-   0        0        0      811 2021-03-25 03:47:34.000000 codex_engine_pyqt-0.1.1/codex/filters/judi_filter.py
+-rw-rw-rw-   0        0        0      358 2021-03-25 03:47:34.000000 codex_engine_pyqt-0.1.1/codex/filters/newline_filter.py
+-rw-rw-rw-   0        0        0      300 2021-03-25 03:47:34.000000 codex_engine_pyqt-0.1.1/codex/filters/null_filter.py
+-rw-rw-rw-   0        0        0     1105 2021-03-25 03:47:34.000000 codex_engine_pyqt-0.1.1/codex/judi_mixin.py
+-rw-rw-rw-   0        0        0      627 2021-03-18 09:51:15.000000 codex_engine_pyqt-0.1.1/codex/judi_responder.py
+-rw-rw-rw-   0        0        0      917 2024-05-11 18:18:04.000000 codex_engine_pyqt-0.1.1/codex/local_serial.py
+-rw-rw-rw-   0        0        0     1032 2022-05-01 00:26:31.000000 codex_engine_pyqt-0.1.1/codex/remote_serial.py
+-rw-rw-rw-   0        0        0     3550 2023-08-02 03:15:29.000000 codex_engine_pyqt-0.1.1/codex/serial_device.py
+-rw-rw-rw-   0        0        0     5750 2024-05-11 18:16:02.000000 codex_engine_pyqt-0.1.1/codex/serial_device_base.py
+-rw-rw-rw-   0        0        0     4405 2021-03-25 16:06:34.000000 codex_engine_pyqt-0.1.1/codex/subscriptions.py
+-rw-rw-rw-   0        0        0     3236 2022-12-09 04:35:48.000000 codex_engine_pyqt-0.1.1/codex/unknown_device.py
+drwxrwxrwx   0        0        0        0 2024-05-11 19:21:09.584070 codex_engine_pyqt-0.1.1/codex_engine_pyqt.egg-info/
+-rw-rw-rw-   0        0        0     1812 2024-05-11 19:21:09.000000 codex_engine_pyqt-0.1.1/codex_engine_pyqt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      747 2024-05-11 19:21:09.000000 codex_engine_pyqt-0.1.1/codex_engine_pyqt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 19:21:09.000000 codex_engine_pyqt-0.1.1/codex_engine_pyqt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-12-09 04:36:59.000000 codex_engine_pyqt-0.1.1/codex_engine_pyqt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2024-05-11 19:21:09.000000 codex_engine_pyqt-0.1.1/codex_engine_pyqt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-11 19:21:09.000000 codex_engine_pyqt-0.1.1/codex_engine_pyqt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1151 2024-05-11 19:21:09.588071 codex_engine_pyqt-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       96 2022-12-09 04:23:09.000000 codex_engine_pyqt-0.1.1/setup.py
```

### Comparing `codex-engine-pyqt-0.1.0/LICENSE` & `codex_engine_pyqt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/PKG-INFO` & `codex_engine_pyqt-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codex-engine-pyqt
-Version: 0.1.0
+Version: 0.1.1
 Summary: A universal translator for serial devices.
 Home-page: https://github.com/Codex-Engine/codex-engine-pyqt
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/Codex-Engine/codex-engine-pyqt
 Project-URL: Tracker, https://github.com/Codex-Engine/codex-engine-pyqt/issues
@@ -16,26 +16,36 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
+Requires-Dist: pyserial
+Requires-Dist: qtstrap
 
 # Codex Engine for PyQt
 
+[![license](https://img.shields.io/pypi/l/codex-engine-pyqt.svg)](./LICENSE)
+[![pypi version](https://img.shields.io/pypi/v/codex-engine-pyqt.svg)](https://pypi.org/project/codex-engine-pyqt/)
+[![PyPI status](https://img.shields.io/pypi/status/codex-engine-pyqt.svg)](https://github.com/DaelonSuzuka/codex-engine-pyqt/)
+
 A universal translator for serial devices.
 
 # Description
 
 This is the reference implementation of Codex, a framework for managing serial communication with physical devices. 
 
 # Features
 - serial port detection
 - automatic handshaking
 - device profiles as drop-in plugins
 - supports many styles of serial communication
 - extensible
 
+# Installation
+
+`pip install codex-engine-pyqt`
+
 ## Requirements
 - pyserial
 - PyQt5 or PySide2
```

### Comparing `codex-engine-pyqt-0.1.0/codex/__init__.py` & `codex_engine_pyqt-0.1.1/codex/__init__.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/codex/bundles.py` & `codex_engine_pyqt-0.1.1/codex/bundles.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/codex/device_controls.py` & `codex_engine_pyqt-0.1.1/codex/device_controls.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/codex/device_manager.py` & `codex_engine_pyqt-0.1.1/codex/device_manager.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/codex/dummy_serial.py` & `codex_engine_pyqt-0.1.1/codex/dummy_serial.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/codex/filters/delimiter_filter.py` & `codex_engine_pyqt-0.1.1/codex/filters/delimiter_filter.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/codex/filters/judi_filter.py` & `codex_engine_pyqt-0.1.1/codex/filters/judi_filter.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/codex/judi_mixin.py` & `codex_engine_pyqt-0.1.1/codex/judi_mixin.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/codex/judi_responder.py` & `codex_engine_pyqt-0.1.1/codex/judi_responder.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/codex/local_serial.py` & `codex_engine_pyqt-0.1.1/codex/local_serial.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from qtpy.QtSerialPort import QSerialPort
-import logging
+from serial import Serial
 
 
+class LocalSerial2:
+    def __init__(self, *args, **kwargs):
+        self.ser = Serial(*args, **kwargs)
+
+    def __getattr__(self, name):
+        return getattr(self.ser, name)
+    
+
 class LocalSerial:
     def __init__(self, port='', baudrate=9600):
-        self.log = logging.getLogger(__name__)
-
         self.ser = QSerialPort()
         self.ser.setPortName(port)
         self.ser.setBaudRate(baudrate)
-        self.log.info(f'creating LocalSerial: {port}@{baudrate}')
 
         self.open()
 
     def open(self) -> bool:
         return self.ser.open(QSerialPort.ReadWrite)
 
     def close(self):
@@ -21,19 +26,13 @@
 
     def write(self, string):
         self.ser.write(string)
 
     def read(self, number=1):
         return bytes(self.ser.read(number))
 
-    @property
-    def baudrate(self):
-        return self.ser.baudRate()
-
-    @baudrate.setter
     def set_baudrate(self, baudrate):
-        self.log.info(f'setting baudrate {baudrate}')
-        self.ser.setBaudRate(baudrate)
+        return self.ser.setBaudRate(baudrate)
 
     @property
     def in_waiting(self):
         return self.ser.bytesAvailable()
```

### Comparing `codex-engine-pyqt-0.1.0/codex/remote_serial.py` & `codex_engine_pyqt-0.1.1/codex/remote_serial.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/codex/serial_device.py` & `codex_engine_pyqt-0.1.1/codex/serial_device.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/codex/serial_device_base.py` & `codex_engine_pyqt-0.1.1/codex/serial_device_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,19 +41,22 @@
         else:
             self.port = port    
 
         if self.port:
             self.open()
 
     def set_baud_rate(self, baud):
-        try:
-            self.ser.baudrate = baud
+        self.log.debug(f'{self.port}: setting baud to: {baud}')
+        result = self.ser.ser.setBaudRate(baud)
+        
+        if result:
             self.baud = baud
-        except:
-            return False
+        else:
+            self.log.debug(f'{self.port}: setting baud failed! {self.ser.ser.error()}')
+
         return True
 
     def connect_socket(self, socket):
         socket.textMessageReceived.connect(self.send)
 
         def send_text_message(s):
             try:
@@ -112,15 +115,15 @@
         self.active = False
 
     def send(self, string):
         """ add a string to the outbound queue """
         if not self.active:
             return
 
-        self.log.debug(f"TX: {string}")
+        self.log.debug(f"TX [{self.port}@{self.baud}]: {string}")
         self.queue.put(string)
         
     def transmit_next_message(self):
         """
         Pull a message from the outbound queue and transmit it to the serial port.
 
         This operation is rate limited by self.transmit_rate_limit.
@@ -133,15 +136,15 @@
                 self.ser.write(self.queue.get().encode())
                 self.last_transmit_time = time.time()
             except SerialException:
                 self.log.exception('serial write failed')
 
     def receive(self, string):
         """ do something when a complete string is captured in self.communicate() """
-        self.log.debug(f"RX: {string}")
+        self.log.debug(f"RX [{self.port}@{self.baud}]: {string}")
         self.base_signals.msg_completed.emit(string)
 
     def check_incoming_data(self):
         try:
             if self.ser.in_waiting:
                 # grab everything
                 data = self.ser.read(self.ser.in_waiting).decode(errors='ignore')
```

### Comparing `codex-engine-pyqt-0.1.0/codex/subscriptions.py` & `codex_engine_pyqt-0.1.1/codex/subscriptions.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/codex/unknown_device.py` & `codex_engine_pyqt-0.1.1/codex/unknown_device.py`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/PKG-INFO` & `codex_engine_pyqt-0.1.1/codex_engine_pyqt.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codex-engine-pyqt
-Version: 0.1.0
+Version: 0.1.1
 Summary: A universal translator for serial devices.
 Home-page: https://github.com/Codex-Engine/codex-engine-pyqt
 Author: David Kincaid
 Author-email: dlkincaid0@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/Codex-Engine/codex-engine-pyqt
 Project-URL: Tracker, https://github.com/Codex-Engine/codex-engine-pyqt/issues
@@ -16,26 +16,36 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
+Requires-Dist: pyserial
+Requires-Dist: qtstrap
 
 # Codex Engine for PyQt
 
+[![license](https://img.shields.io/pypi/l/codex-engine-pyqt.svg)](./LICENSE)
+[![pypi version](https://img.shields.io/pypi/v/codex-engine-pyqt.svg)](https://pypi.org/project/codex-engine-pyqt/)
+[![PyPI status](https://img.shields.io/pypi/status/codex-engine-pyqt.svg)](https://github.com/DaelonSuzuka/codex-engine-pyqt/)
+
 A universal translator for serial devices.
 
 # Description
 
 This is the reference implementation of Codex, a framework for managing serial communication with physical devices. 
 
 # Features
 - serial port detection
 - automatic handshaking
 - device profiles as drop-in plugins
 - supports many styles of serial communication
 - extensible
 
+# Installation
+
+`pip install codex-engine-pyqt`
+
 ## Requirements
 - pyserial
 - PyQt5 or PySide2
```

### Comparing `codex-engine-pyqt-0.1.0/codex_engine_pyqt.egg-info/SOURCES.txt` & `codex_engine_pyqt-0.1.1/codex_engine_pyqt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codex-engine-pyqt-0.1.0/setup.cfg` & `codex_engine_pyqt-0.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f64 6578 2d65 6e67 696e 652d   = codex-engine-
 00000020: 7079 7174 0d0a 7665 7273 696f 6e20 3d20  pyqt..version = 
-00000030: 302e 312e 300d 0a64 6573 6372 6970 7469  0.1.0..descripti
+00000030: 302e 312e 310d 0a64 6573 6372 6970 7469  0.1.1..descripti
 00000040: 6f6e 203d 2041 2075 6e69 7665 7273 616c  on = A universal
 00000050: 2074 7261 6e73 6c61 746f 7220 666f 7220   translator for 
 00000060: 7365 7269 616c 2064 6576 6963 6573 2e0d  serial devices..
 00000070: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
 00000080: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
 00000090: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
 000000a0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
```

