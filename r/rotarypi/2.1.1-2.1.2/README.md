# Comparing `tmp/rotarypi-2.1.1.tar.gz` & `tmp/rotarypi-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotarypi-2.1.1.tar", last modified: Mon Nov 27 12:06:36 2023, max compression
+gzip compressed data, was "rotarypi-2.1.2.tar", last modified: Sat May 11 18:11:56 2024, max compression
```

## Comparing `rotarypi-2.1.1.tar` & `rotarypi-2.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-11-27 12:06:36.838339 rotarypi-2.1.1/
--rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-07-17 12:49:36.000000 rotarypi-2.1.1/MANIFEST.in
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1053 2023-11-27 12:06:36.838339 rotarypi-2.1.1/PKG-INFO
--rw-r--r--   0 dinu      (1000) dinu      (1000)      525 2023-11-27 12:01:38.000000 rotarypi-2.1.1/README.md
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-11-27 12:06:36.837339 rotarypi-2.1.1/rotarypi/
--rw-r--r--   0 dinu      (1000) dinu      (1000)      174 2023-07-17 13:35:20.000000 rotarypi-2.1.1/rotarypi/__init__.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      410 2023-09-28 08:47:51.000000 rotarypi-2.1.1/rotarypi/dialconfig.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)      633 2023-09-25 12:18:46.000000 rotarypi-2.1.1/rotarypi/dialdata.py
--rw-r--r--   0 dinu      (1000) dinu      (1000)     4037 2023-10-26 18:18:40.000000 rotarypi-2.1.1/rotarypi/rotaryreader.py
-drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2023-11-27 12:06:36.838339 rotarypi-2.1.1/rotarypi.egg-info/
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1053 2023-11-27 12:06:36.000000 rotarypi-2.1.1/rotarypi.egg-info/PKG-INFO
--rw-r--r--   0 dinu      (1000) dinu      (1000)      279 2023-11-27 12:06:36.000000 rotarypi-2.1.1/rotarypi.egg-info/SOURCES.txt
--rw-r--r--   0 dinu      (1000) dinu      (1000)        1 2023-11-27 12:06:36.000000 rotarypi-2.1.1/rotarypi.egg-info/dependency_links.txt
--rw-r--r--   0 dinu      (1000) dinu      (1000)       29 2023-11-27 12:06:36.000000 rotarypi-2.1.1/rotarypi.egg-info/requires.txt
--rw-r--r--   0 dinu      (1000) dinu      (1000)        9 2023-11-27 12:06:36.000000 rotarypi-2.1.1/rotarypi.egg-info/top_level.txt
--rw-r--r--   0 dinu      (1000) dinu      (1000)       38 2023-11-27 12:06:36.838339 rotarypi-2.1.1/setup.cfg
--rw-r--r--   0 dinu      (1000) dinu      (1000)     1032 2023-11-27 12:03:59.000000 rotarypi-2.1.1/setup.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-11 18:11:56.767699 rotarypi-2.1.2/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        0 2023-07-17 12:49:36.000000 rotarypi-2.1.2/MANIFEST.in
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1053 2024-05-11 18:11:56.767699 rotarypi-2.1.2/PKG-INFO
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      525 2023-11-27 12:01:38.000000 rotarypi-2.1.2/README.md
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-11 18:11:56.766699 rotarypi-2.1.2/rotarypi/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      174 2023-07-17 13:35:20.000000 rotarypi-2.1.2/rotarypi/__init__.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      594 2024-05-11 18:05:42.000000 rotarypi-2.1.2/rotarypi/dialconfig.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1088 2024-05-11 18:05:42.000000 rotarypi-2.1.2/rotarypi/dialdata.py
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     4414 2024-05-11 18:05:42.000000 rotarypi-2.1.2/rotarypi/rotaryreader.py
+drwxr-xr-x   0 dinu      (1000) dinu      (1000)        0 2024-05-11 18:11:56.767699 rotarypi-2.1.2/rotarypi.egg-info/
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1053 2024-05-11 18:11:56.000000 rotarypi-2.1.2/rotarypi.egg-info/PKG-INFO
+-rw-r--r--   0 dinu      (1000) dinu      (1000)      279 2024-05-11 18:11:56.000000 rotarypi-2.1.2/rotarypi.egg-info/SOURCES.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        1 2024-05-11 18:11:56.000000 rotarypi-2.1.2/rotarypi.egg-info/dependency_links.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       29 2024-05-11 18:11:56.000000 rotarypi-2.1.2/rotarypi.egg-info/requires.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)        9 2024-05-11 18:11:56.000000 rotarypi-2.1.2/rotarypi.egg-info/top_level.txt
+-rw-r--r--   0 dinu      (1000) dinu      (1000)       38 2024-05-11 18:11:56.767699 rotarypi-2.1.2/setup.cfg
+-rw-r--r--   0 dinu      (1000) dinu      (1000)     1032 2024-05-11 18:05:42.000000 rotarypi-2.1.2/setup.py
```

### Comparing `rotarypi-2.1.1/PKG-INFO` & `rotarypi-2.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotarypi
-Version: 2.1.1
+Version: 2.1.2
 Summary: Reading the rotary dial of an old phone with a RaspberryPi
 Home-page: https://gitlab.com/rotaryphone/rotarypi
 Author: Martin Obrist
 Author-email: dev@obrist.email
 License: MIT
 Project-URL: Documentation, https://rotarypi.readthedocs.io
 Project-URL: Source Code, https://gitlab.com/rotaryphone/rotarypi
```

### Comparing `rotarypi-2.1.1/README.md` & `rotarypi-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rotarypi-2.1.1/rotarypi/rotaryreader.py` & `rotarypi-2.1.2/rotarypi/rotaryreader.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import sys
 import time
 
 from rotarypi import DialPinout, DialConfiguration, EventType, HandsetState, DialEvent
 
 
 class RotaryReader:
+    """
+    Detect state changes of the handset and read the rotary dial
+    """
 
     def __init__(self, queue: Queue[DialEvent], pinout: Optional[DialPinout] = None, config: Optional[DialConfiguration] = None):
         self.queue: Queue[DialEvent] = queue
         self.pinout = pinout if pinout is not None else DialPinout()
         self.config = config if config is not None else DialConfiguration()
         self.logger = self._setup_logging()
         self.gpio = GPIO
@@ -80,14 +83,18 @@
                 type=EventType.HANDSET_EVENT,
                 data=HandsetState.PICKED_UP
             )
             self.logger.info("Handset was picked up")
         self.queue.put(msg)
 
     def start(self):
+        """
+        Start listening to events by attaching edge detection on
+        the GPIO pins. This method is non-blocking.
+        """
         self.gpio.add_event_detect(
             self.pinout.dial_pin, self.gpio.BOTH,
             callback=self._dialpin_callback,
             bouncetime=self.config.dial_debounce
         )
         self.gpio.add_event_detect(
             self.pinout.counter_pin, self.gpio.RISING,
@@ -98,14 +105,20 @@
             self.pinout.handset_pin, self.gpio.BOTH,
             callback=self._handset_callback,
             bouncetime=self.config.handset_debounce
         )
         self.logger.info("Callbacks attached, started listening")
 
     def stop(self):
+        """
+        Stop listening to events by detaching attached edge detection.
+        """
         self.gpio.remove_event_detect(self.pinout.dial_pin)
         self.gpio.remove_event_detect(self.pinout.counter_pin)
         self.gpio.remove_event_detect(self.pinout.handset_pin)
         self.logger.info("Callbacks detached, stopped listening")
 
     def cleanup(self):
+        """
+        Cleanup the used GPIO pins.
+        """
         self.gpio.cleanup()
```

### Comparing `rotarypi-2.1.1/rotarypi.egg-info/PKG-INFO` & `rotarypi-2.1.2/rotarypi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotarypi
-Version: 2.1.1
+Version: 2.1.2
 Summary: Reading the rotary dial of an old phone with a RaspberryPi
 Home-page: https://gitlab.com/rotaryphone/rotarypi
 Author: Martin Obrist
 Author-email: dev@obrist.email
 License: MIT
 Project-URL: Documentation, https://rotarypi.readthedocs.io
 Project-URL: Source Code, https://gitlab.com/rotaryphone/rotarypi
```

### Comparing `rotarypi-2.1.1/setup.py` & `rotarypi-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 
 setup(
     name='rotarypi',
-    version='2.1.1',
+    version='2.1.2',
     description="Reading the rotary dial of an old phone with a RaspberryPi",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT",
     author='Martin Obrist',
     author_email='dev@obrist.email',
     url='https://gitlab.com/rotaryphone/rotarypi',
```

