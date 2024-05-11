# Comparing `tmp/mke_sculib-2.5.0.tar.gz` & `tmp/mke_sculib-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-2.5.0.tar", last modified: Sat May 11 16:04:48 2024, max compression
+gzip compressed data, was "mke_sculib-2.5.1.tar", last modified: Sat May 11 16:17:14 2024, max compression
```

## Comparing `mke_sculib-2.5.0.tar` & `mke_sculib-2.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 16:04:48.902173 mke_sculib-2.5.0/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.5.0/LICENSE
--rw-rw-rw-   0        0        0     4120 2024-05-11 16:04:48.902173 mke_sculib-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.5.0/README.rst
--rw-rw-rw-   0        0        0      921 2024-05-11 16:04:48.903173 mke_sculib-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-11 16:04:48.883751 mke_sculib-2.5.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-11 16:04:48.896172 mke_sculib-2.5.0/src/mke_sculib/
--rw-rw-rw-   0        0        0     1124 2024-05-11 15:56:07.000000 mke_sculib-2.5.0/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0   102025 2024-05-11 06:53:52.000000 mke_sculib-2.5.0/src/mke_sculib/acu.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.5.0/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.5.0/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.5.0/src/mke_sculib/helpers.py
--rw-rw-rw-   0        0        0    10152 2024-05-11 15:06:30.000000 mke_sculib-2.5.0/src/mke_sculib/js_helpers.py
--rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.5.0/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0   105947 2024-05-11 16:04:06.000000 mke_sculib-2.5.0/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.5.0/src/mke_sculib/sim.py
--rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.5.0/src/mke_sculib/stellarium_api.py
-drwxrwxrwx   0        0        0        0 2024-05-11 16:04:48.899173 mke_sculib-2.5.0/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4120 2024-05-11 16:04:48.000000 mke_sculib-2.5.0/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2024-05-11 16:04:48.000000 mke_sculib-2.5.0/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 16:04:48.000000 mke_sculib-2.5.0/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-11 16:04:48.000000 mke_sculib-2.5.0/src/mke_sculib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-11 16:04:48.902173 mke_sculib-2.5.0/tests/
--rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.5.0/tests/test_acu_sim.py
--rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.5.0/tests/test_scu.py
+drwxrwxrwx   0        0        0        0 2024-05-11 16:17:14.331081 mke_sculib-2.5.1/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.5.1/LICENSE
+-rw-rw-rw-   0        0        0     4120 2024-05-11 16:17:14.331081 mke_sculib-2.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.5.1/README.rst
+-rw-rw-rw-   0        0        0      921 2024-05-11 16:17:14.332062 mke_sculib-2.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 16:17:14.305147 mke_sculib-2.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-11 16:17:14.326063 mke_sculib-2.5.1/src/mke_sculib/
+-rw-rw-rw-   0        0        0     1124 2024-05-11 16:15:25.000000 mke_sculib-2.5.1/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0   102025 2024-05-11 06:53:52.000000 mke_sculib-2.5.1/src/mke_sculib/acu.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.5.1/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.5.1/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.5.1/src/mke_sculib/helpers.py
+-rw-rw-rw-   0        0        0    10152 2024-05-11 15:06:30.000000 mke_sculib-2.5.1/src/mke_sculib/js_helpers.py
+-rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.5.1/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0   106033 2024-05-11 16:15:15.000000 mke_sculib-2.5.1/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.5.1/src/mke_sculib/sim.py
+-rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.5.1/src/mke_sculib/stellarium_api.py
+drwxrwxrwx   0        0        0        0 2024-05-11 16:17:14.329106 mke_sculib-2.5.1/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4120 2024-05-11 16:17:14.000000 mke_sculib-2.5.1/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2024-05-11 16:17:14.000000 mke_sculib-2.5.1/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 16:17:14.000000 mke_sculib-2.5.1/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-11 16:17:14.000000 mke_sculib-2.5.1/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 16:17:14.330081 mke_sculib-2.5.1/tests/
+-rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.5.1/tests/test_acu_sim.py
+-rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.5.1/tests/test_scu.py
```

### Comparing `mke_sculib-2.5.0/LICENSE` & `mke_sculib-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.0/PKG-INFO` & `mke_sculib-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 2.5.0
+Version: 2.5.1
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.5.0/README.rst` & `mke_sculib-2.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.0/setup.cfg` & `mke_sculib-2.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.0/src/mke_sculib/__init__.py` & `mke_sculib-2.5.1/src/mke_sculib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.5.0'
+__version__ = '2.5.1'
 
 from mke_sculib.scu import scu as scu_api, plot_tt
 from mke_sculib.sim import scu_sim
 from mke_sculib.stellarium_api import stellarium_api as stellar_api
 from mke_sculib.sim import plot_motion_pyplot as plot_motion
```

### Comparing `mke_sculib-2.5.0/src/mke_sculib/acu.py` & `mke_sculib-2.5.1/src/mke_sculib/acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.0/src/mke_sculib/cam_sensors.py` & `mke_sculib-2.5.1/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.0/src/mke_sculib/chan_list_acu.py` & `mke_sculib-2.5.1/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.0/src/mke_sculib/helpers.py` & `mke_sculib-2.5.1/src/mke_sculib/helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.0/src/mke_sculib/js_helpers.py` & `mke_sculib-2.5.1/src/mke_sculib/js_helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.0/src/mke_sculib/mock_telescope.py` & `mke_sculib-2.5.1/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.0/src/mke_sculib/scu.py` & `mke_sculib-2.5.1/src/mke_sculib/scu.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,18 @@
 import aiohttp
 
 from io import StringIO
 
 
 import logging, websockets, asyncio, socket
 
-from websockets.sync.client import connect as ws_sync_connect
+if int(websockets.__version__.split('.')[0]) > 10:
+    from websockets.sync.client import connect as ws_sync_connect
+else:
+    from websockets import connect as ws_sync_connect
 
 import numpy as np
 import pandas as pd
 
 
 import mke_sculib.chan_list_acu as chans
 from mke_sculib.helpers import make_zulustr, match_zulutime, get_utcnow, parse_zulutime
@@ -2445,36 +2448,36 @@
 
     return f, (ax1, ax2)
         
         
 # if __name__ == '__main__':
 #     log("main")
 
-#     from astropy.time import Time
-#     from astropy import units as u
+    from astropy.time import Time
+    from astropy import units as u
 
-#     d119 = scu('http://10.96.66.10:8080/', debug=False, use_socket=True)
+    d119 = scu('http://10.96.66.10:8080/', debug=False, use_socket=True)
 
-#     d119.start()
-#     # # d119.unstow()
+    d119.start()
+    # # d119.unstow()
 
-#     az, el = np.random.randint(-180, -90), np.random.randint(15, 90)
-#     d119.move_to_azel(az, el)
-#     d119.wait_settle()
-#     print(d119.azel)
-#     d119.reset_dmc()
+    az, el = np.random.randint(-180, -90), np.random.randint(15, 90)
+    d119.move_to_azel(az, el)
+    d119.wait_settle()
+    print(d119.azel)
+    d119.reset_dmc()
 
-#     t = np.arange(0, 60) * u.s
-#     az = np.linspace(az, az+360, len(t))
-#     el = np.ones_like(t) * el
+    t = np.arange(0, 60) * u.s
+    az = np.linspace(az, az+360, len(t))
+    el = np.ones_like(t) * el
 
-#     d119.run_track_table((d119.t_internal + t).mjd, az, el, wait_start=False, verb=True)
+    d119.run_track_table((d119.t_internal + t).mjd, az, el, wait_start=False, verb=True)
 
-#     d119.wait_duration()
-#     d119.shutdown()
+    d119.wait_duration()
+    d119.shutdown()
 
 #     D119A.reset_dmc()
 #     D119A.stow()
 
     # D119A.move_to_azel(45, 80)
     # D119A.wait_settle()
     # print(D119A.azel)
```

### Comparing `mke_sculib-2.5.0/src/mke_sculib/sim.py` & `mke_sculib-2.5.1/src/mke_sculib/sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.0/src/mke_sculib/stellarium_api.py` & `mke_sculib-2.5.1/src/mke_sculib/stellarium_api.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.0/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-2.5.1/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 2.5.0
+Version: 2.5.1
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.5.0/tests/test_acu_sim.py` & `mke_sculib-2.5.1/tests/test_acu_sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.0/tests/test_scu.py` & `mke_sculib-2.5.1/tests/test_scu.py`

 * *Files identical despite different names*

