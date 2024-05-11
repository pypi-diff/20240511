# Comparing `tmp/mke_sculib-2.5.2.tar.gz` & `tmp/mke_sculib-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-2.5.2.tar", last modified: Sat May 11 18:40:55 2024, max compression
+gzip compressed data, was "mke_sculib-2.5.3.tar", last modified: Sat May 11 19:38:55 2024, max compression
```

## Comparing `mke_sculib-2.5.2.tar` & `mke_sculib-2.5.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 18:40:55.038395 mke_sculib-2.5.2/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.5.2/LICENSE
--rw-rw-rw-   0        0        0     4120 2024-05-11 18:40:55.038395 mke_sculib-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.5.2/README.rst
--rw-rw-rw-   0        0        0     1017 2024-05-11 18:40:55.039400 mke_sculib-2.5.2/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-11 18:40:55.011230 mke_sculib-2.5.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-11 18:40:55.032915 mke_sculib-2.5.2/src/mke_sculib/
--rw-rw-rw-   0        0        0     1124 2024-05-11 18:40:02.000000 mke_sculib-2.5.2/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0   102025 2024-05-11 06:53:52.000000 mke_sculib-2.5.2/src/mke_sculib/acu.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.5.2/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.5.2/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.5.2/src/mke_sculib/helpers.py
--rw-rw-rw-   0        0        0    10152 2024-05-11 15:06:30.000000 mke_sculib-2.5.2/src/mke_sculib/js_helpers.py
--rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.5.2/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0   105990 2024-05-11 18:37:49.000000 mke_sculib-2.5.2/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.5.2/src/mke_sculib/sim.py
--rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.5.2/src/mke_sculib/stellarium_api.py
-drwxrwxrwx   0        0        0        0 2024-05-11 18:40:55.035918 mke_sculib-2.5.2/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4120 2024-05-11 18:40:54.000000 mke_sculib-2.5.2/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2024-05-11 18:40:54.000000 mke_sculib-2.5.2/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 18:40:54.000000 mke_sculib-2.5.2/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-11 18:40:54.000000 mke_sculib-2.5.2/src/mke_sculib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-11 18:40:54.000000 mke_sculib-2.5.2/src/mke_sculib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-11 18:40:55.036918 mke_sculib-2.5.2/tests/
--rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.5.2/tests/test_acu_sim.py
--rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.5.2/tests/test_scu.py
+drwxrwxrwx   0        0        0        0 2024-05-11 19:38:55.676667 mke_sculib-2.5.3/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.5.3/LICENSE
+-rw-rw-rw-   0        0        0     4120 2024-05-11 19:38:55.677667 mke_sculib-2.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.5.3/README.rst
+-rw-rw-rw-   0        0        0     1017 2024-05-11 19:38:55.677667 mke_sculib-2.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 19:38:55.658545 mke_sculib-2.5.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-11 19:38:55.671666 mke_sculib-2.5.3/src/mke_sculib/
+-rw-rw-rw-   0        0        0     1124 2024-05-11 19:38:34.000000 mke_sculib-2.5.3/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0   102025 2024-05-11 06:53:52.000000 mke_sculib-2.5.3/src/mke_sculib/acu.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.5.3/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.5.3/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.5.3/src/mke_sculib/helpers.py
+-rw-rw-rw-   0        0        0    10152 2024-05-11 15:06:30.000000 mke_sculib-2.5.3/src/mke_sculib/js_helpers.py
+-rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.5.3/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0   106616 2024-05-11 19:38:17.000000 mke_sculib-2.5.3/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.5.3/src/mke_sculib/sim.py
+-rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.5.3/src/mke_sculib/stellarium_api.py
+drwxrwxrwx   0        0        0        0 2024-05-11 19:38:55.675667 mke_sculib-2.5.3/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4120 2024-05-11 19:38:55.000000 mke_sculib-2.5.3/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2024-05-11 19:38:55.000000 mke_sculib-2.5.3/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 19:38:55.000000 mke_sculib-2.5.3/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-11 19:38:55.000000 mke_sculib-2.5.3/src/mke_sculib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-11 19:38:55.000000 mke_sculib-2.5.3/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 19:38:55.676667 mke_sculib-2.5.3/tests/
+-rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.5.3/tests/test_acu_sim.py
+-rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.5.3/tests/test_scu.py
```

### Comparing `mke_sculib-2.5.2/LICENSE` & `mke_sculib-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.2/PKG-INFO` & `mke_sculib-2.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 2.5.2
+Version: 2.5.3
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.5.2/README.rst` & `mke_sculib-2.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.2/setup.cfg` & `mke_sculib-2.5.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -52,13 +52,13 @@
 00000330: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
 00000340: 332e 380d 0a69 6e73 7461 6c6c 5f72 6571  3.8..install_req
 00000350: 7569 7265 7320 3d20 0d0a 0972 6571 7565  uires = ...reque
 00000360: 7374 730d 0a09 7079 7468 6f6e 2d64 6174  sts...python-dat
 00000370: 6575 7469 6c0d 0a09 6e75 6d70 790d 0a09  eutil...numpy...
 00000380: 7061 6e64 6173 0d0a 0961 7374 726f 7079  pandas...astropy
 00000390: 0d0a 0977 6562 736f 636b 6574 733e 3d31  ...websockets>=1
-000003a0: 312e 300d 0a0d 0a5b 6f70 7469 6f6e 732e  1.0....[options.
+000003a0: 322e 300d 0a0d 0a5b 6f70 7469 6f6e 732e  2.0....[options.
 000003b0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
 000003c0: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
 000003d0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
 000003e0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
 000003f0: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `mke_sculib-2.5.2/src/mke_sculib/__init__.py` & `mke_sculib-2.5.3/src/mke_sculib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.5.2'
+__version__ = '2.5.3'
 
 from mke_sculib.scu import scu as scu_api, plot_tt
 from mke_sculib.sim import scu_sim
 from mke_sculib.stellarium_api import stellarium_api as stellar_api
 from mke_sculib.sim import plot_motion_pyplot as plot_motion
```

### Comparing `mke_sculib-2.5.2/src/mke_sculib/acu.py` & `mke_sculib-2.5.3/src/mke_sculib/acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.2/src/mke_sculib/cam_sensors.py` & `mke_sculib-2.5.3/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.2/src/mke_sculib/chan_list_acu.py` & `mke_sculib-2.5.3/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.2/src/mke_sculib/helpers.py` & `mke_sculib-2.5.3/src/mke_sculib/helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.2/src/mke_sculib/js_helpers.py` & `mke_sculib-2.5.3/src/mke_sculib/js_helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.2/src/mke_sculib/mock_telescope.py` & `mke_sculib-2.5.3/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.2/src/mke_sculib/scu.py` & `mke_sculib-2.5.3/src/mke_sculib/scu.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 #HN: 13/05/2021 Changed the way file name is defined by defining a start time 
 # 1.0 2022-05-26 added stowing / unstowing / taking /releasing command authorithy / (de)activating axis
 #                added logging
 #                changed the session saving function
 
 #Import of Python available libraries
 
+import os, inspect, sys
+current_dir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
+parent_dir = os.path.dirname(current_dir)
+if __name__ == '__main__':
+    sys.path.insert(0, parent_dir)
+
 import ctypes
 import sys
 import threading
 import warnings
 from io import StringIO
 import datetime
 import time
@@ -30,14 +36,16 @@
 from astropy.time import Time
 import astropy.units as u
 import numpy as np
 import pandas as pd
 
 import logging, websockets, asyncio, socket
 
+from websockets.sync.client import connect as ws_sync_connect
+
 import mke_sculib.chan_list_acu as chans
 from mke_sculib.helpers import make_zulustr, match_zulutime, get_utcnow, parse_zulutime
 
 class colors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKGREEN = '\033[92m'
@@ -196,15 +204,15 @@
         assert not self.parent is None, 'parent can not be None'
         if self.channels is None:
             self.channels = self.parent.get_channel_list()
         assert self.channels, 'channels must be iterable and not empty!'
         
         def statusupdate():
             
-            with websockets.sync.client(f'ws://{self.parent.ip}:{self.parent.port}/wsstatus') as ws:
+            with ws_sync_connect(f'ws://{self.parent.ip}:{self.parent.port}/wsstatus') as ws:
                 ws.send(json.dumps(self.channels))
                 while True:
                     data = json.loads(ws.recv())
                     self.t_last_remote = Time(data['timestamp'])
                     self.t_last_local = Time.now()
                     self.tickcount += 1
                     self.data = {k:v[0] for k, v in data['fields'].items()}
@@ -2208,15 +2216,15 @@
 
         url = f'ws://{host}:{port}/wsstatus'
 
         if not channels:
             channels = self.get_channel_list()
             _log.debug('Creating new connection...')
 
-        with websockets.sync.client(url) as ws:
+        with ws_sync_connect(url) as ws:
 
             out = json.dumps(channels)
             _log.info(f"{self} | requesting n={len(channels)} channels from ACU")
             _log.debug(f"{self} | requesting {out}")
             ws.send(out)
                 
             is_first = True
@@ -2440,42 +2448,56 @@
 
     return f, (ax1, ax2)
         
         
 if __name__ == '__main__':
     log("main")
 
-    with websockets.client.connect(f'ws://{"10.96.66.10"}:{8080}/wsstatus') as ws:
-        print('success!')
+    # print(websockets.__version__)
+    # with websockets.sync.client.connect(f'ws://{"10.96.66.10"}:{8080}/wsstatus') as ws:
+    #     print('success!')
 
     # from astropy.time import Time
     # from astropy import units as u
 
-    # d119 = scu('http://10.96.66.10:8080/', debug=False, use_socket=True)
+    d119 = scu('http://10.96.66.10:8080/', debug=False, use_socket=True)
 
-    # d119.start()
-    # # # d119.unstow()
+    # stream = DataStreamHandler(d119)
+    # stream.start()
+    # while 1:
+    #     print(f'{stream.t_last_local=} | {stream.t_last_remote=}')
+    # try:
 
-    # az, el = np.random.randint(-180, -90), np.random.randint(15, 90)
-    # d119.move_to_azel(az, el)
-    # d119.wait_settle()
-    # print(d119.azel)
-    # d119.reset_dmc()
 
-    # t = np.arange(0, 60) * u.s
-    # az = np.linspace(az, az+360, len(t))
-    # el = np.ones_like(t) * el
 
-    # d119.run_track_table((d119.t_internal + t).mjd, az, el, wait_start=False, verb=True)
+    el = 80
 
-    # d119.wait_duration()
-    # d119.shutdown()
 
-#     D119A.reset_dmc()
-#     D119A.stow()
+    azp = np.append(np.arange(-30, 0, 1.), np.arange(0, -30, 1.))
+    azs = azp.copy()
+    els = np.ones_like(azp) * el
+
+    for el in [70, 60, 50, 40, 30, 20]:
+        azs = np.append(azs, azp)
+        els = np.append(els, np.ones_like(azp) * el)
+    t = np.arange(0, len(azs)) * u.s
+
+    # d119.move_to_azel(azs[0], els[0])
+    # d119.wait_settle()
+    # d119.start()
+    print(d119.azel)
+    d119.reset_dmc()
+    d119.run_track_table((d119.t_internal + t).mjd, azs, els, wait_start=False, verb=True)
+
+    d119.wait_duration(10.)
+    d119.shutdown()
+    # finally:
+    #     d119.shutdown()
+    # D119A.reset_dmc()
+    # D119A.stow()
 
     # D119A.move_to_azel(45, 80)
     # D119A.wait_settle()
     # print(D119A.azel)
     # D119A.reset_dmc()
     # D119A.move_to_azel(40, 75)
     # print(D119A.azel)
```

### Comparing `mke_sculib-2.5.2/src/mke_sculib/sim.py` & `mke_sculib-2.5.3/src/mke_sculib/sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.2/src/mke_sculib/stellarium_api.py` & `mke_sculib-2.5.3/src/mke_sculib/stellarium_api.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.2/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-2.5.3/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 2.5.2
+Version: 2.5.3
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.5.2/src/mke_sculib.egg-info/SOURCES.txt` & `mke_sculib-2.5.3/src/mke_sculib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.2/tests/test_acu_sim.py` & `mke_sculib-2.5.3/tests/test_acu_sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.2/tests/test_scu.py` & `mke_sculib-2.5.3/tests/test_scu.py`

 * *Files identical despite different names*

