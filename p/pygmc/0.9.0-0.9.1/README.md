# Comparing `tmp/pygmc-0.9.0.tar.gz` & `tmp/pygmc-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmc-0.9.0.tar", last modified: Mon Jan  8 01:42:56 2024, max compression
+gzip compressed data, was "pygmc-0.9.1.tar", last modified: Sun Jan 21 01:54:38 2024, max compression
```

## Comparing `pygmc-0.9.0.tar` & `pygmc-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 01:42:56.899553 pygmc-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-08 01:42:48.000000 pygmc-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-01-08 01:42:56.899553 pygmc-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-01-08 01:42:48.000000 pygmc-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 01:42:56.895553 pygmc-0.9.0/pygmc/
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 01:42:56.895553 pygmc-0.9.0/pygmc/connection/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/connection/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/connection/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/connection/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/connection/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 01:42:56.895553 pygmc-0.9.0/pygmc/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/devices/auto_get_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/devices/device_rfc1201.py
--rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/devices/device_rfc1801.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/devices/gmc300.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/devices/gmc320.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/devices/gmc500.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/devices/gmc600.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/devices/gmc800.py
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-01-08 01:42:48.000000 pygmc-0.9.0/pygmc/history.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 01:42:56.899553 pygmc-0.9.0/pygmc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-01-08 01:42:56.000000 pygmc-0.9.0/pygmc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-01-08 01:42:56.000000 pygmc-0.9.0/pygmc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 01:42:56.000000 pygmc-0.9.0/pygmc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-08 01:42:56.000000 pygmc-0.9.0/pygmc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-08 01:42:56.000000 pygmc-0.9.0/pygmc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-01-08 01:42:48.000000 pygmc-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 01:42:56.899553 pygmc-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 01:42:56.899553 pygmc-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-01-08 01:42:48.000000 pygmc-0.9.0/tests/test_connection_mock_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-08 01:42:48.000000 pygmc-0.9.0/tests/test_correct_pygmc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-01-08 01:42:48.000000 pygmc-0.9.0/tests/test_gmc300s_device_rfc1201.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-01-08 01:42:48.000000 pygmc-0.9.0/tests/test_gmc320_plus_device_rfc1201.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-01-08 01:42:48.000000 pygmc-0.9.0/tests/test_gmc500_plus_device_rfc_1801.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 01:54:38.082017 pygmc-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-21 01:54:29.000000 pygmc-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-01-21 01:54:38.082017 pygmc-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-01-21 01:54:29.000000 pygmc-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 01:54:38.074016 pygmc-0.9.1/pygmc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 01:54:38.078017 pygmc-0.9.1/pygmc/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12731 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/connection/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/connection/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/connection/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/connection/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 01:54:38.078017 pygmc-0.9.1/pygmc/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/devices/auto_get_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/devices/device_rfc1201.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/devices/device_rfc1801.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/devices/gmc300.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/devices/gmc320.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/devices/gmc500.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/devices/gmc600.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/devices/gmc800.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-01-21 01:54:29.000000 pygmc-0.9.1/pygmc/history.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 01:54:38.082017 pygmc-0.9.1/pygmc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-01-21 01:54:38.000000 pygmc-0.9.1/pygmc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-21 01:54:38.000000 pygmc-0.9.1/pygmc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 01:54:38.000000 pygmc-0.9.1/pygmc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-21 01:54:38.000000 pygmc-0.9.1/pygmc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-21 01:54:38.000000 pygmc-0.9.1/pygmc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-01-21 01:54:29.000000 pygmc-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-21 01:54:38.082017 pygmc-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 01:54:38.082017 pygmc-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-01-21 01:54:29.000000 pygmc-0.9.1/tests/test_connection_mock_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-21 01:54:29.000000 pygmc-0.9.1/tests/test_correct_pygmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-01-21 01:54:29.000000 pygmc-0.9.1/tests/test_device_get_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-01-21 01:54:29.000000 pygmc-0.9.1/tests/test_gmc300s_device_rfc1201.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-01-21 01:54:29.000000 pygmc-0.9.1/tests/test_gmc320_plus_device_rfc1201.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-01-21 01:54:29.000000 pygmc-0.9.1/tests/test_gmc500_plus_device_rfc_1801.py
```

### Comparing `pygmc-0.9.0/LICENSE` & `pygmc-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygmc-0.9.0/PKG-INFO` & `pygmc-0.9.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmc
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python package for Geiger–Müller Counter (GMC)
 Author: Thomaz
 License: MIT License
         
         Copyright (c) 2023 Thomaz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,19 +41,19 @@
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial>=3.4
 
 # PyGMC
-[![](https://img.shields.io/pypi/v/pygmc.svg)](https://pypi.org/project/pygmc/)
-[![Read the Docs](https://img.shields.io/readthedocs/pygmc)](https://pygmc.readthedocs.io/)
-[![](https://github.com/Wikilicious/pygmc/workflows/Python%20application/badge.svg)](https://github.com/Wikilicious/pygmc/actions)
-[![GitHub](https://img.shields.io/github/license/Wikilicious/pygmc)](https://github.com/Wikilicious/pygmc/blob/master/LICENSE)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/pygmc)](https://pypi.org/project/pygmc/)
+[![PyPI - Version](https://img.shields.io/pypi/v/pygmc?logo=python&color=green)](https://pypi.org/project/pygmc/)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/Wikilicious/pygmc/python-app.yml?branch=master&logo=github&label=Tests)](https://github.com/Wikilicious/pygmc/tree/master/tests)
+[![Read the Docs](https://img.shields.io/readthedocs/pygmc?logo=readthedocs)](https://pygmc.readthedocs.io/)
+[![codecov](https://codecov.io/gh/Wikilicious/pygmc/graph/badge.svg?token=9X2V5CWPDM)](https://codecov.io/gh/Wikilicious/pygmc)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pygmc?logo=pypi)](https://pypi.org/project/pygmc/)
 
 PyGMC is a Python API for Geiger–Müller Counters (GMCs) / Geiger Counters.
 It has just one dependency (pyserial) and works on multiple operating
 systems: Windows, OSX, Linux. PyGMC aims to be a minimalistic interface -
 lowering the installation requirements and allowing the user to build their
 own tools on top of a stable package.
 
@@ -86,15 +86,15 @@
 
 gc = pygmc.GMC320('/dev/ttyUSB0')
 
 cpm = gc.get_cpm()
 print(cpm)
 ```
 
-####Read device history into DataFrame
+#### Read device history into DataFrame
 ```pycon
 import pandas as pd
 import pygmc
 
 gc = pygmc.GMC320('/dev/ttyUSB0')
 
 history = gc.get_history_data()
```

### Comparing `pygmc-0.9.0/README.md` & `pygmc-0.9.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PyGMC
-[![](https://img.shields.io/pypi/v/pygmc.svg)](https://pypi.org/project/pygmc/)
-[![Read the Docs](https://img.shields.io/readthedocs/pygmc)](https://pygmc.readthedocs.io/)
-[![](https://github.com/Wikilicious/pygmc/workflows/Python%20application/badge.svg)](https://github.com/Wikilicious/pygmc/actions)
-[![GitHub](https://img.shields.io/github/license/Wikilicious/pygmc)](https://github.com/Wikilicious/pygmc/blob/master/LICENSE)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/pygmc)](https://pypi.org/project/pygmc/)
+[![PyPI - Version](https://img.shields.io/pypi/v/pygmc?logo=python&color=green)](https://pypi.org/project/pygmc/)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/Wikilicious/pygmc/python-app.yml?branch=master&logo=github&label=Tests)](https://github.com/Wikilicious/pygmc/tree/master/tests)
+[![Read the Docs](https://img.shields.io/readthedocs/pygmc?logo=readthedocs)](https://pygmc.readthedocs.io/)
+[![codecov](https://codecov.io/gh/Wikilicious/pygmc/graph/badge.svg?token=9X2V5CWPDM)](https://codecov.io/gh/Wikilicious/pygmc)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pygmc?logo=pypi)](https://pypi.org/project/pygmc/)
 
 PyGMC is a Python API for Geiger–Müller Counters (GMCs) / Geiger Counters.
 It has just one dependency (pyserial) and works on multiple operating
 systems: Windows, OSX, Linux. PyGMC aims to be a minimalistic interface -
 lowering the installation requirements and allowing the user to build their
 own tools on top of a stable package.
 
@@ -40,15 +40,15 @@
 
 gc = pygmc.GMC320('/dev/ttyUSB0')
 
 cpm = gc.get_cpm()
 print(cpm)
 ```
 
-####Read device history into DataFrame
+#### Read device history into DataFrame
 ```pycon
 import pandas as pd
 import pygmc
 
 gc = pygmc.GMC320('/dev/ttyUSB0')
 
 history = gc.get_history_data()
```

### Comparing `pygmc-0.9.0/pygmc/__init__.py` & `pygmc-0.9.1/pygmc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Python interface/API for GQ GMC Geiger Counter.
 
 github: https://github.com/Wikilicious/pygmc
 pypi: https://pypi.org/project/pygmc/
 readthedocs: https://pygmc.readthedocs.io/
 Thomaz - 2023
 """
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 __author__ = "Thomaz"
 __license__ = "MIT"
 
 
 import logging
 import time
```

### Comparing `pygmc-0.9.0/pygmc/connection/connection.py` & `pygmc-0.9.1/pygmc/connection/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,20 @@
         deets_port = deets["port"]
         ports = []
         port_info = None
         if deets_port:
             ports = list(
                 serial_list_ports.grep(regexp=f"^{deets_port}$", include_links=True)
             )
-        if deets_port is None and len(ports) != 1:
+        if deets_port is None:
             # port_info will be None which won't hasattr i.e. returns all None.
             logger.warning(f"Unable to identify USB info for {deets_port}")
+        elif len(ports) != 1:
+            # ports var may not exist. The if catches that.
+            logger.warning(f"Unable to identify USB info for {deets_port}")
         else:
             port_info = ports[0]
 
         for key in list(usb_info):
             if hasattr(port_info, key):
                 usb_info[key] = getattr(port_info, key)
 
@@ -310,15 +313,14 @@
         -------
         bytes
             Device response
         """
         logger.debug(f"get(cmd={cmd}, wait_sleep={wait_sleep})")
         self.write(cmd)
         result = self.read(wait_sleep=wait_sleep)
-        logger.debug(f"response={result}")
         return result
 
     def get_at_least(self, cmd, size, wait_sleep=0.05) -> bytes:
         """
         Write cmd, read at least <size> bytes then wait <wait_sleep> and read the buffer.
 
         Parameters
@@ -342,15 +344,14 @@
         -------
         bytes
             Device response
         """
         logger.debug(f"get(cmd={cmd}, wait_sleep={wait_sleep})")
         self.write(cmd)
         result = self.read_at_least(size=size, wait_sleep=wait_sleep)
-        logger.debug(f"response={result}")
         return result
 
     def get_exact(self, cmd, size=None, expected=b"") -> bytes:
         """
         Write and read exact.
 
         Write command to device, provide expected LF or size (bytes),
```

### Comparing `pygmc-0.9.0/pygmc/connection/discovery.py` & `pygmc-0.9.1/pygmc/connection/discovery.py`

 * *Files identical despite different names*

### Comparing `pygmc-0.9.0/pygmc/connection/utils.py` & `pygmc-0.9.1/pygmc/connection/utils.py`

 * *Files identical despite different names*

### Comparing `pygmc-0.9.0/pygmc/devices/auto_get_device.py` & `pygmc-0.9.1/pygmc/devices/auto_get_device.py`

 * *Files identical despite different names*

### Comparing `pygmc-0.9.0/pygmc/devices/device.py` & `pygmc-0.9.1/pygmc/devices/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
         Returns
         -------
         list:
             List of tuples, first row is column names.
 
         """
         data = self.get_raw_history()
-        h = HistoryParser(data)
+        h = HistoryParser(data=data)
         data = [h.get_columns()]
         data.extend(h.get_data())
         return data
 
     def get_version(self) -> str:
         """
         Get version of device.
```

### Comparing `pygmc-0.9.0/pygmc/devices/device_rfc1201.py` & `pygmc-0.9.1/pygmc/devices/device_rfc1201.py`

 * *Files identical despite different names*

### Comparing `pygmc-0.9.0/pygmc/devices/device_rfc1801.py` & `pygmc-0.9.1/pygmc/devices/device_rfc1801.py`

 * *Files identical despite different names*

### Comparing `pygmc-0.9.0/pygmc/devices/gmc300.py` & `pygmc-0.9.1/pygmc/devices/gmc300.py`

 * *Files identical despite different names*

### Comparing `pygmc-0.9.0/pygmc/devices/gmc320.py` & `pygmc-0.9.1/pygmc/devices/gmc320.py`

 * *Files identical despite different names*

### Comparing `pygmc-0.9.0/pygmc/devices/gmc500.py` & `pygmc-0.9.1/pygmc/devices/gmc500.py`

 * *Files identical despite different names*

### Comparing `pygmc-0.9.0/pygmc/devices/gmc600.py` & `pygmc-0.9.1/pygmc/devices/gmc600.py`

 * *Files identical despite different names*

### Comparing `pygmc-0.9.0/pygmc/devices/gmc800.py` & `pygmc-0.9.1/pygmc/devices/gmc800.py`

 * *Files identical despite different names*

### Comparing `pygmc-0.9.0/pygmc/history.py` & `pygmc-0.9.1/pygmc/history.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,32 +5,34 @@
 
 logger = logging.getLogger(__name__)
 
 
 class HistoryParser:
     """Parse GQ GMC device history data."""
 
-    def __init__(self, data):
+    def __init__(self, data=None, filename=None):
         """
         Parse GMC flash memory saved history data.
 
         Parameters
         ----------
-        data: bytes | str | BufferedIOBase
-            Input raw bytes of history, or file path as str, or an BufferedIOBase
-            i.e. open(file, 'rb')
+        data: bytes | None
+            Input raw bytes of history
+            If left None, filename must be provided.
+        filename: str | BufferedIOBase | None
+            Path to file to open or an BufferedIOBase i.e. open(file, 'rb')
+            data takes priority over filename.
 
         """
         if isinstance(data, bytes):
             self._raw = _BinFile(data)
-        elif isinstance(data, str) and len(data) < 32_767:
-            # Ugh...
-            self._raw = open(data, "rb")
-        elif isinstance(data, BufferedIOBase):
-            self._raw = data
+        elif isinstance(filename, BufferedIOBase):
+            self._raw = filename
+        elif filename:
+            self._raw = open(filename, "rb")
         else:
             raise TypeError
 
         self._datetime = None
         self._unit = None
         self._mode = None
         self._columns = [
@@ -172,14 +174,15 @@
         except UnicodeDecodeError:
             if self._eof_check > 5:
                 logger.warning(
                     "Possible end of file... unable to decode note: {}".format(note)
                 )
 
     def _parse(self):
+        """The core parser flow."""
         # The meat of the matter...
         try:
             while True:
                 # command
                 com_str = self._raw.read(1)
                 if len(com_str) == 0:
                     # nothing left to read...
@@ -240,22 +243,27 @@
         except EOFError:
             # we hit end of file
             logger.info("End of history data")
             self._raw.close()
 
     def get_data(self):
         """Get parsed data."""
+        if self._eof_check > 0:
+            # list[:-0] is empty
+            return self._data[: -self._eof_check]
         return self._data
 
     def get_columns(self):
         """Get column names."""
         return self._columns
 
 
 class _BinFile:
+    """A dummy class so raw bytes and BufferedIOBase can be treated the same."""
+
     def __init__(self, data):
         self.data = data
         self._i = 0
         self._len_data = len(data)
 
     def read(self, size):
         tmp = self.data[self._i : self._i + size]
```

### Comparing `pygmc-0.9.0/pygmc.egg-info/PKG-INFO` & `pygmc-0.9.1/pygmc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmc
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python package for Geiger–Müller Counter (GMC)
 Author: Thomaz
 License: MIT License
         
         Copyright (c) 2023 Thomaz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,19 +41,19 @@
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial>=3.4
 
 # PyGMC
-[![](https://img.shields.io/pypi/v/pygmc.svg)](https://pypi.org/project/pygmc/)
-[![Read the Docs](https://img.shields.io/readthedocs/pygmc)](https://pygmc.readthedocs.io/)
-[![](https://github.com/Wikilicious/pygmc/workflows/Python%20application/badge.svg)](https://github.com/Wikilicious/pygmc/actions)
-[![GitHub](https://img.shields.io/github/license/Wikilicious/pygmc)](https://github.com/Wikilicious/pygmc/blob/master/LICENSE)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/pygmc)](https://pypi.org/project/pygmc/)
+[![PyPI - Version](https://img.shields.io/pypi/v/pygmc?logo=python&color=green)](https://pypi.org/project/pygmc/)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/Wikilicious/pygmc/python-app.yml?branch=master&logo=github&label=Tests)](https://github.com/Wikilicious/pygmc/tree/master/tests)
+[![Read the Docs](https://img.shields.io/readthedocs/pygmc?logo=readthedocs)](https://pygmc.readthedocs.io/)
+[![codecov](https://codecov.io/gh/Wikilicious/pygmc/graph/badge.svg?token=9X2V5CWPDM)](https://codecov.io/gh/Wikilicious/pygmc)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pygmc?logo=pypi)](https://pypi.org/project/pygmc/)
 
 PyGMC is a Python API for Geiger–Müller Counters (GMCs) / Geiger Counters.
 It has just one dependency (pyserial) and works on multiple operating
 systems: Windows, OSX, Linux. PyGMC aims to be a minimalistic interface -
 lowering the installation requirements and allowing the user to build their
 own tools on top of a stable package.
 
@@ -86,15 +86,15 @@
 
 gc = pygmc.GMC320('/dev/ttyUSB0')
 
 cpm = gc.get_cpm()
 print(cpm)
 ```
 
-####Read device history into DataFrame
+#### Read device history into DataFrame
 ```pycon
 import pandas as pd
 import pygmc
 
 gc = pygmc.GMC320('/dev/ttyUSB0')
 
 history = gc.get_history_data()
```

### Comparing `pygmc-0.9.0/pygmc.egg-info/SOURCES.txt` & `pygmc-0.9.1/pygmc.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -22,10 +22,11 @@
 pygmc/devices/gmc300.py
 pygmc/devices/gmc320.py
 pygmc/devices/gmc500.py
 pygmc/devices/gmc600.py
 pygmc/devices/gmc800.py
 tests/test_connection_mock_serial.py
 tests/test_correct_pygmc.py
+tests/test_device_get_history.py
 tests/test_gmc300s_device_rfc1201.py
 tests/test_gmc320_plus_device_rfc1201.py
 tests/test_gmc500_plus_device_rfc_1801.py
```

### Comparing `pygmc-0.9.0/pyproject.toml` & `pygmc-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pygmc"
-version = "0.9.0"
+version = "0.9.1"
 authors = [
     {name = "Thomaz"},
 ]
 description = "Python package for Geiger–Müller Counter (GMC)"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 dependencies = ["pyserial>=3.4"]
```

### Comparing `pygmc-0.9.0/tests/test_gmc300s_device_rfc1201.py` & `pygmc-0.9.1/tests/test_gmc300s_device_rfc1201.py`

 * *Files identical despite different names*

### Comparing `pygmc-0.9.0/tests/test_gmc320_plus_device_rfc1201.py` & `pygmc-0.9.1/tests/test_gmc320_plus_device_rfc1201.py`

 * *Files identical despite different names*

### Comparing `pygmc-0.9.0/tests/test_gmc500_plus_device_rfc_1801.py` & `pygmc-0.9.1/tests/test_gmc500_plus_device_rfc_1801.py`

 * *Files identical despite different names*

