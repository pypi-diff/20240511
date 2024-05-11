# Comparing `tmp/mke_sculib-2.4.9.tar.gz` & `tmp/mke_sculib-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-2.4.9.tar", last modified: Fri May 10 14:01:58 2024, max compression
+gzip compressed data, was "mke_sculib-2.5.0.tar", last modified: Sat May 11 16:04:48 2024, max compression
```

## Comparing `mke_sculib-2.4.9.tar` & `mke_sculib-2.5.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 14:01:58.119278 mke_sculib-2.4.9/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.4.9/LICENSE
--rw-rw-rw-   0        0        0     4120 2024-05-10 14:01:58.119278 mke_sculib-2.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.4.9/README.rst
--rw-rw-rw-   0        0        0      921 2024-05-10 14:01:58.120782 mke_sculib-2.4.9/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.4.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:01:58.098258 mke_sculib-2.4.9/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 14:01:58.114277 mke_sculib-2.4.9/src/mke_sculib/
--rw-rw-rw-   0        0        0     1124 2024-05-10 14:01:08.000000 mke_sculib-2.4.9/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.4.9/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.4.9/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.4.9/src/mke_sculib/helpers.py
--rw-rw-rw-   0        0        0     9874 2024-05-09 20:02:32.000000 mke_sculib-2.4.9/src/mke_sculib/js_helpers.py
--rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.4.9/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0    99507 2024-05-10 14:00:52.000000 mke_sculib-2.4.9/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.4.9/src/mke_sculib/sim.py
--rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.4.9/src/mke_sculib/stellarium_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 14:01:58.117277 mke_sculib-2.4.9/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4120 2024-05-10 14:01:57.000000 mke_sculib-2.4.9/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2024-05-10 14:01:58.000000 mke_sculib-2.4.9/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 14:01:57.000000 mke_sculib-2.4.9/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-10 14:01:57.000000 mke_sculib-2.4.9/src/mke_sculib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 14:01:58.119278 mke_sculib-2.4.9/tests/
--rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.4.9/tests/test_acu_sim.py
--rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.4.9/tests/test_scu.py
+drwxrwxrwx   0        0        0        0 2024-05-11 16:04:48.902173 mke_sculib-2.5.0/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0     4120 2024-05-11 16:04:48.902173 mke_sculib-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.5.0/README.rst
+-rw-rw-rw-   0        0        0      921 2024-05-11 16:04:48.903173 mke_sculib-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 16:04:48.883751 mke_sculib-2.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-11 16:04:48.896172 mke_sculib-2.5.0/src/mke_sculib/
+-rw-rw-rw-   0        0        0     1124 2024-05-11 15:56:07.000000 mke_sculib-2.5.0/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0   102025 2024-05-11 06:53:52.000000 mke_sculib-2.5.0/src/mke_sculib/acu.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.5.0/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.5.0/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.5.0/src/mke_sculib/helpers.py
+-rw-rw-rw-   0        0        0    10152 2024-05-11 15:06:30.000000 mke_sculib-2.5.0/src/mke_sculib/js_helpers.py
+-rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.5.0/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0   105947 2024-05-11 16:04:06.000000 mke_sculib-2.5.0/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    19532 2024-04-10 07:02:06.000000 mke_sculib-2.5.0/src/mke_sculib/sim.py
+-rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.5.0/src/mke_sculib/stellarium_api.py
+drwxrwxrwx   0        0        0        0 2024-05-11 16:04:48.899173 mke_sculib-2.5.0/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4120 2024-05-11 16:04:48.000000 mke_sculib-2.5.0/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2024-05-11 16:04:48.000000 mke_sculib-2.5.0/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 16:04:48.000000 mke_sculib-2.5.0/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-11 16:04:48.000000 mke_sculib-2.5.0/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 16:04:48.902173 mke_sculib-2.5.0/tests/
+-rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.5.0/tests/test_acu_sim.py
+-rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.5.0/tests/test_scu.py
```

### Comparing `mke_sculib-2.4.9/LICENSE` & `mke_sculib-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.9/PKG-INFO` & `mke_sculib-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 2.4.9
+Version: 2.5.0
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.9/README.rst` & `mke_sculib-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.9/setup.cfg` & `mke_sculib-2.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.9/src/mke_sculib/__init__.py` & `mke_sculib-2.5.0/src/mke_sculib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.4.9'
+__version__ = '2.5.0'
 
 from mke_sculib.scu import scu as scu_api, plot_tt
 from mke_sculib.sim import scu_sim
 from mke_sculib.stellarium_api import stellarium_api as stellar_api
 from mke_sculib.sim import plot_motion_pyplot as plot_motion
```

### Comparing `mke_sculib-2.4.9/src/mke_sculib/cam_sensors.py` & `mke_sculib-2.5.0/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.9/src/mke_sculib/chan_list_acu.py` & `mke_sculib-2.5.0/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.9/src/mke_sculib/helpers.py` & `mke_sculib-2.5.0/src/mke_sculib/helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.9/src/mke_sculib/js_helpers.py` & `mke_sculib-2.5.0/src/mke_sculib/js_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
     # <div id="live-update-graph-el" style="width:600px;height:250px;"></div>
     # <div id="live-update-graph-fi" style="width:600px;height:250px;"></div>
     # <div id="tester" style="width:600px;height:250px;"></div>
 
 TEMPLATE_POS_CHART_PAGE = """<head>
 
     <script src="https://cdn.plot.ly/plotly-2.32.0.min.js" charset="utf-8"></script>
-    <div id="live-update-graph-az"></div>
-    <div id="live-update-graph-el"></div>
-    <div id="live-update-graph-fi"></div>
+    <div id="live-update-graph-az" <REPLACEME_STYLE>></div>
+    <div id="live-update-graph-el" <REPLACEME_STYLE>></div>
+    <div id="live-update-graph-fi" <REPLACEME_STYLE>></div>
 
     <script>
         
 function makeChart(chans1, chans2, chans3, url_ws, element_ids) {
     
     const colors = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52'];
 
@@ -171,27 +171,29 @@
     </script>
 </head>"""
 
 def make_livepos_page(dish_ip, 
                       chans1=['acu.azimuth.p_set', 'acu.azimuth.p_shape', 'acu.azimuth.p_act'],
                       chans2=['acu.elevation.p_set', 'acu.elevation.p_shape', 'acu.elevation.p_act'],
                       chans3=['acu.general_management_and_controller.state', 'acu.azimuth.state', 'acu.elevation.state'],
-                      port = '8080'):
+                      port = '8080', style="width:600px;height:100px;"):
     
     page = TEMPLATE_POS_CHART_PAGE.replace('<REPLACEME:IP>:<REPLACEME:PORT>', f'{dish_ip}:{port}')
+    
+    page = page.replace('<REPLACEME_STYLE>', json.dumps(style))
     page = page.replace('<REPLACEME1>', json.dumps(chans1))
     page = page.replace('<REPLACEME2>', json.dumps(chans2))
     return page.replace('<REPLACEME3>', json.dumps(chans3))
 
 
 
 TEMPLATE_LIVEPLOT_PAGE = """<head>
 
     <script src="https://cdn.plot.ly/plotly-2.32.0.min.js" charset="utf-8"></script>
-    <div id="live-update-graph"></div>
+    <div id="live-update-graph" <REPLACEME_STYLE>></div>
 
     <script>
         
 function makeChart(channels, url_ws, element_id) {
     
     const colors = ['#636EFA', '#EF553B', '#00CC96', '#AB63FA', '#FFA15A', '#19D3F3', '#FF6692', '#B6E880', '#FF97FF', '#FECB52'];
     
@@ -294,16 +296,17 @@
 
     </script>
 </head>"""
 
 
 def make_liveplot_page(dish_ip, 
                       channels=['acu.azimuth.p_act', 'acu.elevation.p_act', 'acu.azimuth.p_act'],
-                      port = '8080'):
+                      port = '8080', style="width:600px;height:100px;"):
     
     page = TEMPLATE_LIVEPLOT_PAGE.replace('<REPLACEME:IP>:<REPLACEME:PORT>', f'{dish_ip}:{port}')
+    page = page.replace('<REPLACEME_STYLE>', json.dumps(style))
     return page.replace('<REPLACEME1>', json.dumps(channels))
 
 
 
 if __name__ == '__main__':
     print(make_liveplot_page('10.96.66.10'))
```

#### html2text {}

```diff
@@ -1,18 +1,24 @@
 import json #
 #
 #
 #
 TEMPLATE_POS_CHART_PAGE = """
+REPLACEME_STYLE>>
+REPLACEME_STYLE>>
+REPLACEME_STYLE>>
 """ def make_livepos_page(dish_ip, chans1=['acu.azimuth.p_set',
 'acu.azimuth.p_shape', 'acu.azimuth.p_act'], chans2=['acu.elevation.p_set',
 'acu.elevation.p_shape', 'acu.elevation.p_act'], chans3=
 ['acu.general_management_and_controller.state', 'acu.azimuth.state',
-'acu.elevation.state'], port = '8080'): page = TEMPLATE_POS_CHART_PAGE.replace
-(':', f'{dish_ip}:{port}') page = page.replace('', json.dumps(chans1)) page =
+'acu.elevation.state'], port = '8080', style="width:600px;height:100px;"): page
+= TEMPLATE_POS_CHART_PAGE.replace(':', f'{dish_ip}:{port}') page = page.replace
+('', json.dumps(style)) page = page.replace('', json.dumps(chans1)) page =
 page.replace('', json.dumps(chans2)) return page.replace('', json.dumps
 (chans3)) TEMPLATE_LIVEPLOT_PAGE = """
+REPLACEME_STYLE>>
 """ def make_liveplot_page(dish_ip, channels=['acu.azimuth.p_act',
-'acu.elevation.p_act', 'acu.azimuth.p_act'], port = '8080'): page =
-TEMPLATE_LIVEPLOT_PAGE.replace(':', f'{dish_ip}:{port}') return page.replace
-('', json.dumps(channels)) if __name__ == '__main__': print(make_liveplot_page
+'acu.elevation.p_act', 'acu.azimuth.p_act'], port = '8080', style="width:
+600px;height:100px;"): page = TEMPLATE_LIVEPLOT_PAGE.replace(':', f'{dish_ip}:
+{port}') page = page.replace('', json.dumps(style)) return page.replace('',
+json.dumps(channels)) if __name__ == '__main__': print(make_liveplot_page
 ('10.96.66.10'))
```

### Comparing `mke_sculib-2.4.9/src/mke_sculib/mock_telescope.py` & `mke_sculib-2.5.0/src/mke_sculib/mock_telescope.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.9/src/mke_sculib/scu.py` & `mke_sculib-2.5.0/src/mke_sculib/acu.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
 
 import logging, websockets, asyncio, socket
 
 import numpy as np
 import pandas as pd
 
+from struct import pack, unpack
+import enum
 
 import mke_sculib.chan_list_acu as chans
 from mke_sculib.helpers import make_zulustr, match_zulutime, get_utcnow, parse_zulutime
 
 class colors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
@@ -2295,16 +2297,110 @@
     ax2.grid()
 
     if do_show:
         plt.show()
 
     return f, (ax1, ax2)
         
+
+def make_packet(m:bytes):
+    assert isinstance(m, bytes)
+    start_flag = 0x1DFCCF1A
+    message_length = len(m)
+    source = 3
+    command_counter = Time.now().mjd
+    message_bytes = bytes(m)
+    end_flag = 0xA1FCCFD1
+
+    m = pack()
+    return pack(f'<IIId{len(m)}s', 
+            start_flag,
+            message_length,
+            source,
+            command_counter,
+            message_bytes,
+            end_flag)
+    
+def make_command(mid:np.uint32, cid:np.uint32, params:list) -> bytes:
+    form = [tp[0] for tp in params]
+    args = [tp[1] for tp in params]
+    return pack(f'<II' + form, mid, cid, *args)
+
+def make_message(mid:np.uint32, cid:np.uint32, params:list):
+    return make_packet(make_command(mid, cid, params))
+
+class MOD(enum.IntEnum):
+    VOID = 0
+    AZ = 1 # Azimuth Axis Modules
+    EL = 2 # Elevation Axis Modules
+    FI = 3 # Feed Indexer Modules
+    TIM = 10 # Time Controller
+    CMS = 20 # Command Arbiter
+    STPA = 21 # Stow Pin Controller Azimuth
+    STPE = 22 # Stow Pin Controller Elevation
+    SAF = 20 # Safety System Controller
+    TRX = 30 # Tracking Controller
+    POI = 40 # Pointing Controller
+    PWR = 50 # Power Distribution Controller
+    DMC = 100 # Dish Management Controller
+
+pathes = {
+    'c_auth.take': (MOD.CMS, 10, 1),
+    'c_auth.release': (MOD.CMS, 10, 2),
+    'c_active.az': (MOD.AZ, 1),
+    'c_active.el': (MOD.EL, 1),
+    'c_active.fi': (MOD.FI, 1),
+    
+}
+
+# errs = {
+#     'c_active': ['4 wrong mode', "Axis is interlocked.", "Axis is interlocked (e-stop or any other error). Refer to axis related error status for detailed information."],
+
+# Current command source has not the command authority.
+# not command authority
+# 4 wrong mode
+
+
+# }
+
+
+if __name__ == '__main__':
+
+    from websockets.sync.client import connect
+
+    host = "10.96.66.10"
+    HOST = "127.0.0.1"
+    port = 7101
+    
+    config= {
+        "acu.addr": "localhost",
+        "acu.status.port": 7101,
+        "acu.commands.port": 7100,
+        "commandsQueueTimeoutSeconds":  5,
+    }
+
+    import socket
+
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        s.connect((host, port))
+        
+
+        m1 = make_message(*pathes['take_c_auth'])
+        s.sendall(m1)
+        a = s.recv(1024)
+
+        time.sleep(10)
+        m2 = make_message(*pathes['release_c_auth'])
+        s.sendall(m1)
+        a = s.recv(1024)
+        
         
 # if __name__ == '__main__':
+
+
 #     log("main")
 
 #     D119A = scu('http://10.96.66.10:8080/', debug=True)
 #     D119A.reset_dmc()
 #     D119A.unstow()
 
 #     D119A.reset_dmc()
```

### Comparing `mke_sculib-2.4.9/src/mke_sculib/sim.py` & `mke_sculib-2.5.0/src/mke_sculib/sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.9/src/mke_sculib/stellarium_api.py` & `mke_sculib-2.5.0/src/mke_sculib/stellarium_api.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.9/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-2.5.0/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 2.4.9
+Version: 2.5.0
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.4.9/tests/test_acu_sim.py` & `mke_sculib-2.5.0/tests/test_acu_sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.4.9/tests/test_scu.py` & `mke_sculib-2.5.0/tests/test_scu.py`

 * *Files identical despite different names*

