# Comparing `tmp/rpi-lgpio-0.5.tar.gz` & `tmp/rpi_lgpio-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpi-lgpio-0.5.tar", last modified: Fri Apr 12 22:52:01 2024, max compression
+gzip compressed data, was "rpi_lgpio-0.6.tar", last modified: Sat May 11 16:07:23 2024, max compression
```

## Comparing `rpi-lgpio-0.5.tar` & `rpi_lgpio-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-04-12 22:52:01.433484 rpi-lgpio-0.5/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1130 2024-04-10 08:01:37.000000 rpi-lgpio-0.5/LICENSE.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     2251 2024-04-12 22:52:01.433484 rpi-lgpio-0.5/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     1138 2024-04-10 08:01:37.000000 rpi-lgpio-0.5/README.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-04-12 22:52:01.430484 rpi-lgpio-0.5/RPi/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-04-12 22:52:01.431484 rpi-lgpio-0.5/RPi/GPIO/
--rw-rw-r--   0 dave      (1000) dave      (1000)    29014 2024-04-10 08:01:37.000000 rpi-lgpio-0.5/RPi/GPIO/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2024-04-10 08:01:37.000000 rpi-lgpio-0.5/RPi/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-04-12 22:52:01.433484 rpi-lgpio-0.5/rpi_lgpio.egg-info/
--rw-r--r--   0 dave      (1000) dave      (1000)     2251 2024-04-12 22:52:01.000000 rpi-lgpio-0.5/rpi_lgpio.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      242 2024-04-12 22:52:01.000000 rpi-lgpio-0.5/rpi_lgpio.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2024-04-12 22:52:01.000000 rpi-lgpio-0.5/rpi_lgpio.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       63 2024-04-12 22:52:01.000000 rpi-lgpio-0.5/rpi_lgpio.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        4 2024-04-12 22:52:01.000000 rpi-lgpio-0.5/rpi_lgpio.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     1587 2024-04-12 22:52:01.434484 rpi-lgpio-0.5/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2024-04-10 08:01:37.000000 rpi-lgpio-0.5/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-11 16:07:23.058008 rpi_lgpio-0.6/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1130 2024-04-10 08:01:37.000000 rpi_lgpio-0.6/LICENSE.txt
+-rw-r--r--   0 dave      (1000) dave      (1000)     2449 2024-05-11 16:07:23.058008 rpi_lgpio-0.6/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1138 2024-04-10 08:01:37.000000 rpi_lgpio-0.6/README.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-11 16:07:23.052008 rpi_lgpio-0.6/RPi/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-11 16:07:23.053008 rpi_lgpio-0.6/RPi/GPIO/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    29956 2024-05-11 13:56:52.000000 rpi_lgpio-0.6/RPi/GPIO/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2024-04-10 08:01:37.000000 rpi_lgpio-0.6/RPi/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-05-11 16:07:23.056008 rpi_lgpio-0.6/rpi_lgpio.egg-info/
+-rw-r--r--   0 dave      (1000) dave      (1000)     2449 2024-05-11 16:07:22.000000 rpi_lgpio-0.6/rpi_lgpio.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      242 2024-05-11 16:07:23.000000 rpi_lgpio-0.6/rpi_lgpio.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2024-05-11 16:07:22.000000 rpi_lgpio-0.6/rpi_lgpio.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       72 2024-05-11 16:07:22.000000 rpi_lgpio-0.6/rpi_lgpio.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        4 2024-05-11 16:07:22.000000 rpi_lgpio-0.6/rpi_lgpio.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1596 2024-05-11 16:07:23.061008 rpi_lgpio-0.6/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2024-04-10 08:01:37.000000 rpi_lgpio-0.6/setup.py
```

### Comparing `rpi-lgpio-0.5/LICENSE.txt` & `rpi_lgpio-0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rpi-lgpio-0.5/PKG-INFO` & `rpi_lgpio-0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpi-lgpio
-Version: 0.5
+Version: 0.6
 Summary: A compatibility shim between RPi.GPIO and lgpio
 Home-page: https://rpi-lgpio.readthedocs.io/
 Author: Dave Jones
 Author-email: dave@waveform.org.uk
 License: BSD-3-Clause
 Project-URL: Documentation, https://rpi-lgpio.readthedocs.io/
 Project-URL: Source Code, https://github.com/waveform80/rpi-lgpio
@@ -18,17 +18,22 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Provides-Extra: doc
-Provides-Extra: test
 License-File: LICENSE.txt
+Requires-Dist: lgpio>=0.1.0.1
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Provides-Extra: doc
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
 
 ======
 README
 ======
 
 rpi-lgpio is a compatibility package intended to provide compatibility with
 the `rpi-gpio`_ (aka RPi.GPIO) library, on top of kernels that only support the
```

### Comparing `rpi-lgpio-0.5/README.rst` & `rpi_lgpio-0.6/README.rst`

 * *Files identical despite different names*

### Comparing `rpi-lgpio-0.5/RPi/GPIO/__init__.py` & `rpi_lgpio-0.6/RPi/GPIO/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
 import struct
 import warnings
 from time import sleep
+from pathlib import Path
 from threading import Event
 from weakref import WeakValueDictionary
 
 import lgpio
 
 try:
     # Patch several constants which changed incompatibly between 0.1.6.0
@@ -480,14 +481,44 @@
             4: '4GB',
             5: '8GB',
             6: '16GB',
         }.get(revision >> 20 & 0x7, 'Unknown'),
     }
 
 
+def _get_gpiochip_num():
+    """
+    Determines the number of the GPIO chip device to access.
+
+    If :envvar:`RPI_LGPIO_CHIP` is found in the environment, it will be used.
+    Otherwise, the routine will attempt to query sysfs to find a GPIO chip
+    device with a driver known to be used for userspace GPIO access. If none
+    can be found, returns 0 as a fallback.
+    """
+    try:
+        return int(os.environ['RPI_LGPIO_CHIP'])
+    except KeyError:
+        # The following are the driver names used for the GPIO chip devices
+        # intended for userspace control
+        user_gpio_drivers = frozenset((
+            'raspberrypi,rp1-gpio',
+            'raspberrypi,bcm2835-gpio',
+            'raspberrypi,bcm2711-gpio',
+        ))
+        for dev in Path('/sys/bus/gpio/devices').glob('gpiochip*'):
+            compatible = (dev / 'of_node/compatible')
+            try:
+                drivers = set(compatible.read_text().split('\0'))
+            except FileNotFoundError:
+                continue
+            if drivers & user_gpio_drivers:
+                return int(dev.name[len('gpiochip'):])
+    return 0
+
+
 def getmode():
     """
     Get the numbering mode used for the pins on the board. Returns
     :data:`BOARD`, :data:`BCM` or :data:`None`.
     """
 
     if _mode == UNKNOWN:
@@ -506,27 +537,23 @@
 
     If a numbering mode has already been set, and *new_mode* is not the same
     as the result of :func:`getmode`, a :exc:`ValueError` is raised.
 
     :param int new_mode:
         The new numbering mode to apply
     """
-    # TODO atexit cleanup of claimed GPIOs to input
     global _mode, _chip
 
     if _mode != UNKNOWN and new_mode != _mode:
         raise ValueError('A different mode has already been set!')
     if new_mode not in (BOARD, BCM):
         raise ValueError('An invalid mode was passed to setmode()')
 
     if _chip is None:
-        chip_num = os.environ.get('RPI_LGPIO_CHIP')
-        if chip_num is None:
-            chip_num = 4 if _get_rpi_info()['PROCESSOR'] == 'BCM2712' else 0
-        _chip = _check(lgpio.gpiochip_open(int(chip_num)))
+        _chip = _check(lgpio.gpiochip_open(_get_gpiochip_num()))
     _mode = new_mode
 
 
 def setwarnings(value):
     """
     Enable or disable warning messages. These are mostly produced when calling
     :func:`setup` or :func:`cleanup` to change channel modes.
```

### Comparing `rpi-lgpio-0.5/rpi_lgpio.egg-info/PKG-INFO` & `rpi_lgpio-0.6/rpi_lgpio.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpi-lgpio
-Version: 0.5
+Version: 0.6
 Summary: A compatibility shim between RPi.GPIO and lgpio
 Home-page: https://rpi-lgpio.readthedocs.io/
 Author: Dave Jones
 Author-email: dave@waveform.org.uk
 License: BSD-3-Clause
 Project-URL: Documentation, https://rpi-lgpio.readthedocs.io/
 Project-URL: Source Code, https://github.com/waveform80/rpi-lgpio
@@ -18,17 +18,22 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Provides-Extra: doc
-Provides-Extra: test
 License-File: LICENSE.txt
+Requires-Dist: lgpio>=0.1.0.1
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Provides-Extra: doc
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
 
 ======
 README
 ======
 
 rpi-lgpio is a compatibility package intended to provide compatibility with
 the `rpi-gpio`_ (aka RPi.GPIO) library, on top of kernels that only support the
```

### Comparing `rpi-lgpio-0.5/setup.cfg` & `rpi_lgpio-0.6/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rpi-lgpio
-version = 0.5
+version = 0.6
 description = A compatibility shim between RPi.GPIO and lgpio
 long_description = file:README.rst
 author = Dave Jones
 author_email = dave@waveform.org.uk
 url = https://rpi-lgpio.readthedocs.io/
 project_urls = 
 	Documentation = https://rpi-lgpio.readthedocs.io/
@@ -25,15 +25,15 @@
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	lgpio
+	lgpio>=0.1.0.1
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
 doc = 
 	sphinx
```

