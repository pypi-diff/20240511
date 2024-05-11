# Comparing `tmp/pymycobot-3.4.6b1.tar.gz` & `tmp/pymycobot-3.4.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymycobot-3.4.6b1.tar", last modified: Thu Apr 18 11:14:01 2024, max compression
+gzip compressed data, was "pymycobot-3.4.7b1.tar", last modified: Sat May 11 02:02:17 2024, max compression
```

## Comparing `pymycobot-3.4.6b1.tar` & `pymycobot-3.4.7b1.tar`

### file list

```diff
@@ -1,55 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 11:14:01.391361 pymycobot-3.4.6b1/
--rw-rw-rw-   0        0        0     1096 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/LICENSE
--rw-rw-rw-   0        0        0       51 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/MANIFEST.in
--rw-rw-rw-   0        0        0    63944 2024-04-18 11:14:01.389362 pymycobot-3.4.6b1/PKG-INFO
--rw-rw-rw-   0        0        0     1884 2024-01-12 01:20:44.000000 pymycobot-3.4.6b1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 11:14:01.349795 pymycobot-3.4.6b1/pymycobot/
--rw-rw-rw-   0        0        0    35096 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/Interface.py
--rw-rw-rw-   0        0        0     2171 2024-04-18 11:13:40.000000 pymycobot-3.4.6b1/pymycobot/__init__.py
--rw-rw-rw-   0        0        0     1968 2023-09-16 05:58:39.000000 pymycobot-3.4.6b1/pymycobot/bluet.py
--rw-rw-rw-   0        0        0    24930 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/common.py
--rw-rw-rw-   0        0        0    12178 2024-02-21 09:54:15.000000 pymycobot-3.4.6b1/pymycobot/elephantrobot.py
--rw-rw-rw-   0        0        0    16504 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/error.py
--rw-rw-rw-   0        0        0    42593 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/generate.py
--rw-rw-rw-   0        0        0      236 2024-02-21 09:54:15.000000 pymycobot-3.4.6b1/pymycobot/genre.py
--rw-rw-rw-   0        0        0      557 2023-09-16 05:58:39.000000 pymycobot-3.4.6b1/pymycobot/log.py
--rw-rw-rw-   0        0        0      250 2024-02-21 09:57:39.000000 pymycobot-3.4.6b1/pymycobot/mecharm.py
--rw-rw-rw-   0        0        0     8459 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mecharmsocket.py
--rw-rw-rw-   0        0        0     7695 2024-04-12 11:33:10.000000 pymycobot-3.4.6b1/pymycobot/mercury.py
--rw-rw-rw-   0        0        0    16852 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mercury_api.py
--rw-rw-rw-   0        0        0     6394 2024-03-01 10:10:12.000000 pymycobot-3.4.6b1/pymycobot/mercurychassis.py
--rw-rw-rw-   0        0        0     2211 2024-03-21 08:57:25.000000 pymycobot-3.4.6b1/pymycobot/mercurychassisocket.py
--rw-rw-rw-   0        0        0     6944 2024-03-12 09:17:38.000000 pymycobot-3.4.6b1/pymycobot/mercurysocket.py
--rw-rw-rw-   0        0        0    14031 2024-04-08 09:08:30.000000 pymycobot-3.4.6b1/pymycobot/myagv.py
--rw-rw-rw-   0        0        0    11294 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/myarm.py
--rw-rw-rw-   0        0        0    16331 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/myarm_api.py
--rw-rw-rw-   0        0        0      273 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/myarmc.py
--rw-rw-rw-   0        0        0     3186 2024-04-18 11:13:01.000000 pymycobot-3.4.6b1/pymycobot/myarmm.py
--rw-rw-rw-   0        0        0     8871 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/myarmsocket.py
--rw-rw-rw-   0        0        0    15120 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mybuddy.py
--rw-rw-rw-   0        0        0     6123 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mybuddybluetooth.py
--rw-rw-rw-   0        0        0     4544 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mybuddyemoticon.py
--rw-rw-rw-   0        0        0     9844 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mybuddysocket.py
--rw-rw-rw-   0        0        0     9524 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mycobot.py
--rw-rw-rw-   0        0        0    85159 2024-04-18 01:28:43.000000 pymycobot-3.4.6b1/pymycobot/mycobotpro630.py
--rw-rw-rw-   0        0        0     8955 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mycobotsocket.py
--rw-rw-rw-   0        0        0     9916 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mypalletizer.py
--rw-rw-rw-   0        0        0     8607 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/mypalletizersocket.py
--rw-rw-rw-   0        0        0     1932 2023-10-10 06:41:29.000000 pymycobot-3.4.6b1/pymycobot/public.py
--rw-rw-rw-   0        0        0     4052 2024-03-21 08:57:25.000000 pymycobot-3.4.6b1/pymycobot/robot_limit.json
--rw-rw-rw-   0        0        0    22021 2024-04-09 09:54:07.000000 pymycobot-3.4.6b1/pymycobot/ultraArm.py
--rw-rw-rw-   0        0        0      674 2023-09-16 05:58:39.000000 pymycobot-3.4.6b1/pymycobot/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:14:01.388356 pymycobot-3.4.6b1/pymycobot.egg-info/
--rw-rw-rw-   0        0        0    63944 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1126 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 11:14:01.000000 pymycobot-3.4.6b1/pymycobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       53 2024-04-09 09:54:24.000000 pymycobot-3.4.6b1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 11:14:01.392361 pymycobot-3.4.6b1/setup.cfg
--rw-rw-rw-   0        0        0     3229 2024-04-09 09:57:20.000000 pymycobot-3.4.6b1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:14:01.386801 pymycobot-3.4.6b1/tests/
--rw-rw-rw-   0        0        0     8555 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/tests/test_api.py
--rw-rw-rw-   0        0        0     2556 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/tests/test_generator.py
--rw-rw-rw-   0        0        0      544 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/tests/test_socket.py
--rw-rw-rw-   0        0        0      322 2023-09-01 03:07:13.000000 pymycobot-3.4.6b1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:02:17.635812 pymycobot-3.4.7b1/
+-rw-rw-rw-   0        0        0     1096 2023-09-01 03:07:13.000000 pymycobot-3.4.7b1/LICENSE
+-rw-rw-rw-   0        0        0       51 2023-09-01 03:07:13.000000 pymycobot-3.4.7b1/MANIFEST.in
+-rw-rw-rw-   0        0        0    63944 2024-05-11 02:02:17.633812 pymycobot-3.4.7b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1884 2024-01-12 01:20:44.000000 pymycobot-3.4.7b1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 02:02:17.593803 pymycobot-3.4.7b1/pymycobot/
+-rw-rw-rw-   0        0        0    35096 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/Interface.py
+-rw-rw-rw-   0        0        0     2171 2024-05-11 02:02:09.000000 pymycobot-3.4.7b1/pymycobot/__init__.py
+-rw-rw-rw-   0        0        0     1968 2023-09-16 05:58:39.000000 pymycobot-3.4.7b1/pymycobot/bluet.py
+-rw-rw-rw-   0        0        0    24941 2024-04-25 03:16:52.000000 pymycobot-3.4.7b1/pymycobot/common.py
+-rw-rw-rw-   0        0        0    12842 2024-05-11 02:01:09.000000 pymycobot-3.4.7b1/pymycobot/elephantrobot.py
+-rw-rw-rw-   0        0        0    16504 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/error.py
+-rw-rw-rw-   0        0        0    42593 2024-04-18 11:13:01.000000 pymycobot-3.4.7b1/pymycobot/generate.py
+-rw-rw-rw-   0        0        0      236 2024-02-21 09:54:15.000000 pymycobot-3.4.7b1/pymycobot/genre.py
+-rw-rw-rw-   0        0        0      557 2023-09-16 05:58:39.000000 pymycobot-3.4.7b1/pymycobot/log.py
+-rw-rw-rw-   0        0        0      250 2024-02-21 09:57:39.000000 pymycobot-3.4.7b1/pymycobot/mecharm.py
+-rw-rw-rw-   0        0        0     8459 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mecharmsocket.py
+-rw-rw-rw-   0        0        0     7695 2024-04-12 11:33:10.000000 pymycobot-3.4.7b1/pymycobot/mercury.py
+-rw-rw-rw-   0        0        0    16855 2024-04-23 03:10:49.000000 pymycobot-3.4.7b1/pymycobot/mercury_api.py
+-rw-rw-rw-   0        0        0     6460 2024-04-25 03:16:52.000000 pymycobot-3.4.7b1/pymycobot/mercurychassis.py
+-rw-rw-rw-   0        0        0     6944 2024-03-12 09:17:38.000000 pymycobot-3.4.7b1/pymycobot/mercurysocket.py
+-rw-rw-rw-   0        0        0    14031 2024-04-08 09:08:30.000000 pymycobot-3.4.7b1/pymycobot/myagv.py
+-rw-rw-rw-   0        0        0    11294 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/myarm.py
+-rw-rw-rw-   0        0        0    16475 2024-05-07 11:28:46.000000 pymycobot-3.4.7b1/pymycobot/myarm_api.py
+-rw-rw-rw-   0        0        0      273 2024-04-22 09:29:51.000000 pymycobot-3.4.7b1/pymycobot/myarmc.py
+-rw-rw-rw-   0        0        0     3186 2024-04-18 11:13:01.000000 pymycobot-3.4.7b1/pymycobot/myarmm.py
+-rw-rw-rw-   0        0        0     8871 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/myarmsocket.py
+-rw-rw-rw-   0        0        0    15120 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mybuddy.py
+-rw-rw-rw-   0        0        0     6123 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mybuddybluetooth.py
+-rw-rw-rw-   0        0        0     4544 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mybuddyemoticon.py
+-rw-rw-rw-   0        0        0     9844 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mybuddysocket.py
+-rw-rw-rw-   0        0        0     9524 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mycobot.py
+-rw-rw-rw-   0        0        0    87447 2024-05-11 02:01:09.000000 pymycobot-3.4.7b1/pymycobot/mycobotpro630.py
+-rw-rw-rw-   0        0        0     8955 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mycobotsocket.py
+-rw-rw-rw-   0        0        0     9916 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mypalletizer.py
+-rw-rw-rw-   0        0        0     8607 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/mypalletizersocket.py
+-rw-rw-rw-   0        0        0     1932 2023-10-10 06:41:29.000000 pymycobot-3.4.7b1/pymycobot/public.py
+-rw-rw-rw-   0        0        0     4052 2024-03-21 08:57:25.000000 pymycobot-3.4.7b1/pymycobot/robot_limit.json
+-rw-rw-rw-   0        0        0    22021 2024-04-09 09:54:07.000000 pymycobot-3.4.7b1/pymycobot/ultraArm.py
+-rw-rw-rw-   0        0        0      674 2023-09-16 05:58:39.000000 pymycobot-3.4.7b1/pymycobot/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:02:17.632811 pymycobot-3.4.7b1/pymycobot.egg-info/
+-rw-rw-rw-   0        0        0    63944 2024-05-11 02:02:17.000000 pymycobot-3.4.7b1/pymycobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1093 2024-05-11 02:02:17.000000 pymycobot-3.4.7b1/pymycobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 02:02:17.000000 pymycobot-3.4.7b1/pymycobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-11 02:02:17.000000 pymycobot-3.4.7b1/pymycobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-11 02:02:17.000000 pymycobot-3.4.7b1/pymycobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       53 2024-04-09 09:54:24.000000 pymycobot-3.4.7b1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 02:02:17.635812 pymycobot-3.4.7b1/setup.cfg
+-rw-rw-rw-   0        0        0     3229 2024-04-09 09:57:20.000000 pymycobot-3.4.7b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:02:17.629810 pymycobot-3.4.7b1/tests/
+-rw-rw-rw-   0        0        0     8555 2023-09-01 03:07:13.000000 pymycobot-3.4.7b1/tests/test_api.py
+-rw-rw-rw-   0        0        0     2556 2023-09-01 03:07:13.000000 pymycobot-3.4.7b1/tests/test_generator.py
+-rw-rw-rw-   0        0        0      544 2023-09-01 03:07:13.000000 pymycobot-3.4.7b1/tests/test_socket.py
+-rw-rw-rw-   0        0        0      322 2023-09-01 03:07:13.000000 pymycobot-3.4.7b1/tests/test_utils.py
```

### Comparing `pymycobot-3.4.6b1/LICENSE` & `pymycobot-3.4.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/PKG-INFO` & `pymycobot-3.4.7b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.4.6b1
+Version: 3.4.7b1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pymycobot-3.4.6b1/README.md` & `pymycobot-3.4.7b1/README.md`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/Interface.py` & `pymycobot-3.4.7b1/pymycobot/Interface.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/__init__.py` & `pymycobot-3.4.7b1/pymycobot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 ]
 
 
 if sys.platform == "linux":
     from pymycobot.mybuddyemoticon import MyBuddyEmoticon
     __all__.append("MyBuddyEmoticon")
 
-__version__ = "3.4.6b1"
+__version__ = "3.4.7b1"
 __author__ = "Elephantrobotics"
 __email__ = "weiquan.xu@elephantrobotics.com"
 __git_url__ = "https://github.com/elephantrobotics/pymycobot"
 __copyright__ = "CopyRight (c) 2020-{0} Shenzhen Elephantrobotics technology".format(
     datetime.datetime.now().year
 )
```

### Comparing `pymycobot-3.4.6b1/pymycobot/bluet.py` & `pymycobot-3.4.7b1/pymycobot/bluet.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/common.py` & `pymycobot-3.4.7b1/pymycobot/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,15 +307,15 @@
         command_data = self._process_data_command(genre, self.__class__.__name__, args)
         if genre == 178:
             # 修改wifi端口
             command_data = self._encode_int16(command_data)
             
         elif genre in [76, 77]:
             command_data = [command_data[0]] + self._encode_int16(command_data[1]*10)
-        elif genre == 115 and self.__class__.__name__ not in  ["MyArmC", "MyArmM"]:
+        elif genre == 115 and self.__class__.__name__ not in  ["MyArmC", "MyArmM", "Mercury"]:
             command_data = [command_data[1],command_data[3]]
         LEN = len(command_data) + 2
         
         command = [
                 ProtocolCode.HEADER,
                 ProtocolCode.HEADER,
                 LEN,
```

### Comparing `pymycobot-3.4.6b1/pymycobot/elephantrobot.py` & `pymycobot-3.4.7b1/pymycobot/elephantrobot.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,15 @@
             try:
                 coords_1 = float(data_arr[0])
                 coords_2 = float(data_arr[1])
                 coords_3 = float(data_arr[2])
                 coords_4 = float(data_arr[3])
                 coords_5 = float(data_arr[4])
                 coords_6 = float(data_arr[5])
-                coords = [coords_1, coords_2, coords_3,
-                          coords_4, coords_5, coords_6]
+                coords = [coords_1, coords_2, coords_3, coords_4, coords_5, coords_6]
                 return coords
             except:
                 return self.invalid_coords()
         return self.invalid_coords()
 
     def string_to_double(self, data):
         try:
@@ -118,20 +117,22 @@
 
     def state_check(self):
         command = "state_check()\n"
         res = self.send_command(command)
         return res == "1"
 
     def upload_file(self, local_filename, remote_filename):
-        """Base64 encode local file, send it over socket and save it on robot
-           as remote_filename.
+        """Upload local file to robot via socket. Permissions are checked before
+           upload so it cannot overwrite system files (owned by root).
 
         Args:
-            local_filename (str): file to send
-            remote_filename (str): save remote file name
+            local_filename (str): absolute or relative path to a file to send
+            remote_filename (str): absolute or relative file path to where
+                                   to upload a file. If path is relative, it is
+                                   relative to ~/RoboFlow/upload folder.
 
         Returns:
             str: ok if success or error message otherwise
         """
         with open(local_filename, "rb") as f:
             content = f.read().encode()
         content_base64 = base64.b64encode(content).decode()
@@ -195,15 +196,15 @@
         up = "1"
         if up_down:
             up = "0"
         command = "set_upside_down(" + up + ")\n"
         self.send_command(command)
 
     def set_payload(self, payload):
-        command = "set_speed(" + str(payload) + ")\n"
+        command = "set_payload(" + str(payload) + ")\n"
         self.send_command(command)
 
     def state_on(self):
         command = "state_on()\n"
         self.send_command(command)
 
     def state_off(self):
@@ -212,23 +213,21 @@
 
     def task_stop(self):
         command = "task_stop()\n"
         self.send_command(command)
 
     def jog_angle(self, joint_str, direction, speed):
         command = (
-            "jog_angle(" + joint_str + "," + str(direction) +
-            "," + str(speed) + ")\n"
+            "jog_angle(" + joint_str + "," + str(direction) + "," + str(speed) + ")\n"
         )
         self.send_command(command)
 
     def jog_coord(self, axis_str, direction, speed):
         command = (
-            "jog_coord(" + axis_str + "," + str(direction) +
-            "," + str(speed) + ")\n"
+            "jog_coord(" + axis_str + "," + str(direction) + "," + str(speed) + ")\n"
         )
         self.send_command(command)
 
     def get_digital_in(self, pin_number):
         command = "get_digital_in(" + str(pin_number) + ")\n"
         self.send_command(command)
 
@@ -276,41 +275,54 @@
         command = 'assign_variable("' + str(var_name) + '",' + str(var_value) + ")\n"
         self.send_command(command)
 
     def get_variable(self, var_name):
         command = 'get_variable("' + str(var_name) + '")\n'
         return self.send_command(command)
 
-    def jog_relative(self, joint_id, angle, speed):
-        command = 'SendJogIncrement("{}","{}","{}")\n'.format(
-            joint_id, angle, speed)
+    def jog_relative(self, joint_id, angle, speed, mode):
+        """Relative jog.
+
+        Example:
+            jog_relative('J1', 5, 600, 1)
+
+        Args:
+            joint_id (str): 'J1' - 'J6', 'X', 'Y', 'Z', 'RX', 'RY', 'RZ'
+            angle (float): relative angle or coord value to move, can be negative
+                           to move to other direction
+            speed (int): speed value
+            mode (int): 0 (coord mode) or 1 (joint mode)
+
+        Returns:
+            str: return data from socket
+        """
+        command = "jog_increment({},{},{},{})\n".format(joint_id, angle, speed, mode)
         return self.send_command(command)
 
     def set_init_gripper(self, gripper_type):
         """
         gripper_type:CAG-1
         """
         command = "set_init_gripper(" + str(gripper_type) + ")\n"
         return self.send_command(command)
 
     def set_cag_gripper_mode(self, mode):
         """
         mode:0 / 1
         """
 
-        command = "set_cag_gripper_mode("+str(mode) + ")\n"
+        command = "set_cag_gripper_mode(" + str(mode) + ")\n"
         return self.send_command(command)
 
     def set_cag_gripper_value(self, value, speed):
         """
         value: 0-100
         speed: 1-100
         """
-        command = "set_cag_gripper_value( " + \
-            str(value) + ',' + str(speed) + "  )\n"
+        command = "set_cag_gripper_value( " + str(value) + "," + str(speed) + "  )\n"
         return self.send_command(command)
 
     def get_cag_gripper_value(self):
         command = "get_cag_gripper_value()\n"
         return self.send_command(command)
 
     def set_cag_gripper_enabled(self, mode):
```

### Comparing `pymycobot-3.4.6b1/pymycobot/error.py` & `pymycobot-3.4.7b1/pymycobot/error.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/generate.py` & `pymycobot-3.4.7b1/pymycobot/generate.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/log.py` & `pymycobot-3.4.7b1/pymycobot/log.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/mecharmsocket.py` & `pymycobot-3.4.7b1/pymycobot/mecharmsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/mercury.py` & `pymycobot-3.4.7b1/pymycobot/mercury.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/mercury_api.py` & `pymycobot-3.4.7b1/pymycobot/mercury_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,23 +187,23 @@
         Args:
             axis (_type_): _description_
             direction (_type_): _description_
             speed (_type_): _description_
         """
         return self._mesg(ProtocolCode.MERCURY_JOG_BASE_COORD, axis, direction, speed)
     
-    def drag_tech_save(self):
+    def drag_teach_save(self):
         """Start recording the dragging teaching point. In order to show the best sports effect, the recording time should not exceed 90 seconds."""
         return self._mesg(ProtocolCode.MERCURY_DRAG_TECH_SAVE)
     
-    def drag_tech_execute(self):
+    def drag_teach_execute(self):
         """Start dragging the teaching point and only execute it once."""
         return self._mesg(ProtocolCode.MERCURY_DRAG_TECH_EXECUTE)
     
-    def drag_tech_pause(self):
+    def drag_teach_pause(self):
         """Pause recording of dragging teaching point"""
         self._mesg(ProtocolCode.MERCURY_DRAG_TECH_PAUSE)
         
     def is_gripper_moving(self, mode=None):
         """Judge whether the gripper is moving or not
         
         Args:
```

### Comparing `pymycobot-3.4.6b1/pymycobot/mercurychassis.py` & `pymycobot-3.4.7b1/pymycobot/mercurychassis.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 import threading
 import struct
 
 class MercuryChassisError(Exception):
     pass
 
 class MercuryChassis:
+    """
+    Mercury X1 mobile chassis car socket class
+    """
     def __init__(self, ip=None):
         self.ifname = b"wlan0"
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         if ip is not None:
             self.host = ip
         else:
             import fcntl
```

### Comparing `pymycobot-3.4.6b1/pymycobot/mercurychassisocket.py` & `pymycobot-3.4.7b1/pymycobot/public.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,139 +1,121 @@
-00000000: 2321 2f75 7372 2f62 696e 2f70 7974 686f  #!/usr/bin/pytho
-00000010: 6e0d 0a23 202d 2a2d 2063 6f64 696e 673a  n..# -*- coding:
-00000020: 7574 662d 3820 2d2a 2d0d 0a69 6d70 6f72  utf-8 -*-..impor
-00000030: 7420 6a73 6f6e 0d0a 696d 706f 7274 2073  t json..import s
-00000040: 6f63 6b65 740d 0a69 6d70 6f72 7420 7468  ocket..import th
-00000050: 7265 6164 696e 670d 0a69 6d70 6f72 7420  reading..import 
-00000060: 7469 6d65 0d0a 696d 706f 7274 2074 7261  time..import tra
-00000070: 6365 6261 636b 0d0a 0d0a 0d0a 636c 6173  ceback......clas
-00000080: 7320 4d65 7263 7572 7943 6861 7373 6973  s MercuryChassis
-00000090: 536f 636b 6574 286f 626a 6563 7429 3a0d  Socket(object):.
-000000a0: 0a20 2020 2022 2222 0d0a 2020 2020 4d65  .    """..    Me
-000000b0: 7263 7572 7920 5831 206d 6f62 696c 6520  rcury X1 mobile 
-000000c0: 6368 6173 7369 7320 6361 7220 736f 636b  chassis car sock
-000000d0: 6574 2063 6c61 7373 0d0a 2020 2020 2222  et class..    ""
-000000e0: 220d 0a0d 0a20 2020 2064 6566 205f 5f69  "....    def __i
-000000f0: 6e69 745f 5f28 7365 6c66 2c20 7365 7276  nit__(self, serv
-00000100: 6572 5f68 6f73 742c 2073 6572 7665 725f  er_host, server_
-00000110: 706f 7274 2c20 6465 6275 673d 4661 6c73  port, debug=Fals
-00000120: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
-00000130: 0d0a 2020 2020 2020 2020 4172 6773 3a0d  ..        Args:.
-00000140: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
-00000150: 7665 725f 686f 7374 3a20 5365 7276 6572  ver_host: Server
-00000160: 2069 700d 0a20 2020 2020 2020 2020 2020   ip..           
-00000170: 2073 6572 7665 725f 706f 7274 3a20 5365   server_port: Se
-00000180: 7276 6572 2070 6f72 740d 0a20 2020 2020  rver port..     
-00000190: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000001a0: 7375 7065 7228 4d65 7263 7572 7943 6861  super(MercuryCha
-000001b0: 7373 6973 536f 636b 6574 2c20 7365 6c66  ssisSocket, self
-000001c0: 292e 5f5f 696e 6974 5f5f 2829 0d0a 2020  ).__init__()..  
-000001d0: 2020 2020 2020 7365 6c66 2e53 4552 5645        self.SERVE
-000001e0: 525f 484f 5354 203d 2073 6572 7665 725f  R_HOST = server_
-000001f0: 686f 7374 0d0a 2020 2020 2020 2020 7365  host..        se
-00000200: 6c66 2e53 4552 5645 525f 504f 5254 203d  lf.SERVER_PORT =
-00000210: 2073 6572 7665 725f 706f 7274 0d0a 2020   server_port..  
-00000220: 2020 2020 2020 7365 6c66 2e73 6f63 6b20        self.sock 
-00000230: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
-00000240: 7365 6c66 2e64 6562 7567 203d 2064 6562  self.debug = deb
-00000250: 7567 0d0a 2020 2020 2020 2020 7365 6c66  ug..        self
-00000260: 2e6c 6f63 6b20 3d20 7468 7265 6164 696e  .lock = threadin
-00000270: 672e 4c6f 636b 2829 0d0a 2020 2020 2020  g.Lock()..      
-00000280: 2020 7365 6c66 2e63 6f6e 6e65 6374 5f74    self.connect_t
-00000290: 6f5f 7365 7276 6572 5f62 2829 0d0a 0d0a  o_server_b()....
-000002a0: 2020 2020 6465 6620 636f 6e6e 6563 745f      def connect_
-000002b0: 746f 5f73 6572 7665 725f 6228 7365 6c66  to_server_b(self
-000002c0: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
-000002d0: 2e73 6f63 6b20 3d20 736f 636b 6574 2e73  .sock = socket.s
-000002e0: 6f63 6b65 7428 736f 636b 6574 2e41 465f  ocket(socket.AF_
-000002f0: 494e 4554 2c20 736f 636b 6574 2e53 4f43  INET, socket.SOC
-00000300: 4b5f 5354 5245 414d 290d 0a20 2020 2020  K_STREAM)..     
-00000310: 2020 2073 656c 662e 736f 636b 2e63 6f6e     self.sock.con
-00000320: 6e65 6374 2828 7365 6c66 2e53 4552 5645  nect((self.SERVE
-00000330: 525f 484f 5354 2c20 7365 6c66 2e53 4552  R_HOST, self.SER
-00000340: 5645 525f 504f 5254 2929 0d0a 0d0a 2020  VER_PORT))....  
-00000350: 2020 6465 6620 7365 6e64 5f63 6f6d 6d61    def send_comma
-00000360: 6e64 2873 656c 662c 2063 6f6d 6d61 6e64  nd(self, command
-00000370: 2c20 6461 7461 3d4e 6f6e 6529 3a0d 0a20  , data=None):.. 
-00000380: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
-00000390: 2e6c 6f63 6b3a 0d0a 2020 2020 2020 2020  .lock:..        
-000003a0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-000003b0: 2020 2020 2020 2020 2020 7061 796c 6f61            payloa
-000003c0: 6420 3d20 7b63 6f6d 6d61 6e64 3a20 6461  d = {command: da
-000003d0: 7461 7d0d 0a20 2020 2020 2020 2020 2020  ta}..           
-000003e0: 2020 2020 2073 6572 6961 6c69 7a65 645f       serialized_
-000003f0: 6461 7461 203d 206a 736f 6e2e 6475 6d70  data = json.dump
-00000400: 7328 7061 796c 6f61 6429 2e65 6e63 6f64  s(payload).encod
-00000410: 6528 2775 7466 2d38 2729 0d0a 2020 2020  e('utf-8')..    
-00000420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000430: 2e73 6f63 6b2e 7365 6e64 616c 6c28 7365  .sock.sendall(se
-00000440: 7269 616c 697a 6564 5f64 6174 6129 0d0a  rialized_data)..
-00000450: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000460: 2020 6966 2073 656c 662e 6465 6275 673a    if self.debug:
-00000470: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000480: 2020 2020 2020 6375 7272 656e 745f 7469        current_ti
-00000490: 6d65 203d 2074 696d 652e 7374 7266 7469  me = time.strfti
-000004a0: 6d65 2822 2559 2d25 6d2d 2564 2025 483a  me("%Y-%m-%d %H:
-000004b0: 254d 3a25 5322 2c20 7469 6d65 2e6c 6f63  %M:%S", time.loc
-000004c0: 616c 7469 6d65 2829 290d 0a20 2020 2020  altime())..     
-000004d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000004e0: 7269 6e74 2822 5b7b 7d5d 2053 656e 7420  rint("[{}] Sent 
-000004f0: 636f 6d6d 616e 643a 207b 7d2c 2044 6174  command: {}, Dat
-00000500: 613a 207b 7d22 2e66 6f72 6d61 7428 6375  a: {}".format(cu
-00000510: 7272 656e 745f 7469 6d65 2c20 636f 6d6d  rrent_time, comm
-00000520: 616e 642c 2064 6174 6129 290d 0a20 2020  and, data))..   
-00000530: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00000540: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
-00000550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000560: 2070 7269 6e74 2822 4572 726f 7220 7365   print("Error se
-00000570: 6e64 696e 6720 636f 6d6d 616e 643a 222c  nding command:",
-00000580: 2073 7472 2874 7261 6365 6261 636b 2e66   str(traceback.f
-00000590: 6f72 6d61 745f 6578 6328 2929 290d 0a0d  ormat_exc()))...
-000005a0: 0a20 2020 2064 6566 2067 6f53 7472 6169  .    def goStrai
-000005b0: 6768 7428 7365 6c66 2c20 7469 6d65 2c20  ght(self, time, 
-000005c0: 7370 6565 6429 3a0d 0a20 2020 2020 2020  speed):..       
-000005d0: 2063 6f6d 6d61 6e64 203d 2027 676f 5374   command = 'goSt
-000005e0: 7261 6967 6874 270d 0a20 2020 2020 2020  raight'..       
-000005f0: 2064 6174 6120 3d20 7b27 7469 6d65 273a   data = {'time':
-00000600: 2074 696d 652c 2027 7370 6565 6427 3a20   time, 'speed': 
-00000610: 7370 6565 647d 0d0a 2020 2020 2020 2020  speed}..        
-00000620: 7365 6c66 2e73 656e 645f 636f 6d6d 616e  self.send_comman
-00000630: 6428 636f 6d6d 616e 642c 2064 6174 6129  d(command, data)
-00000640: 0d0a 0d0a 2020 2020 6465 6620 676f 4261  ....    def goBa
-00000650: 636b 2873 656c 662c 2074 696d 652c 2073  ck(self, time, s
-00000660: 7065 6564 293a 0d0a 2020 2020 2020 2020  peed):..        
-00000670: 636f 6d6d 616e 6420 3d20 2767 6f42 6163  command = 'goBac
-00000680: 6b27 0d0a 2020 2020 2020 2020 6461 7461  k'..        data
-00000690: 203d 207b 2774 696d 6527 3a20 7469 6d65   = {'time': time
-000006a0: 2c20 2773 7065 6564 273a 2073 7065 6564  , 'speed': speed
-000006b0: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
-000006c0: 7365 6e64 5f63 6f6d 6d61 6e64 2863 6f6d  send_command(com
-000006d0: 6d61 6e64 2c20 6461 7461 290d 0a0d 0a20  mand, data).... 
-000006e0: 2020 2064 6566 2074 7572 6e52 6967 6874     def turnRight
-000006f0: 2873 656c 662c 2074 696d 652c 2073 7065  (self, time, spe
-00000700: 6564 293a 0d0a 2020 2020 2020 2020 636f  ed):..        co
-00000710: 6d6d 616e 6420 3d20 2774 7572 6e52 6967  mmand = 'turnRig
-00000720: 6874 270d 0a20 2020 2020 2020 2064 6174  ht'..        dat
-00000730: 6120 3d20 7b27 7469 6d65 273a 2074 696d  a = {'time': tim
-00000740: 652c 2027 7370 6565 6427 3a20 7370 6565  e, 'speed': spee
-00000750: 647d 0d0a 2020 2020 2020 2020 7365 6c66  d}..        self
-00000760: 2e73 656e 645f 636f 6d6d 616e 6428 636f  .send_command(co
-00000770: 6d6d 616e 642c 2064 6174 6129 0d0a 0d0a  mmand, data)....
-00000780: 2020 2020 6465 6620 7475 726e 4c65 6674      def turnLeft
-00000790: 2873 656c 662c 2074 696d 652c 2073 7065  (self, time, spe
-000007a0: 6564 293a 0d0a 2020 2020 2020 2020 636f  ed):..        co
-000007b0: 6d6d 616e 6420 3d20 2774 7572 6e4c 6566  mmand = 'turnLef
-000007c0: 7427 0d0a 2020 2020 2020 2020 6461 7461  t'..        data
-000007d0: 203d 207b 2774 696d 6527 3a20 7469 6d65   = {'time': time
-000007e0: 2c20 2773 7065 6564 273a 2073 7065 6564  , 'speed': speed
-000007f0: 7d0d 0a20 2020 2020 2020 2073 656c 662e  }..        self.
-00000800: 7365 6e64 5f63 6f6d 6d61 6e64 2863 6f6d  send_command(com
-00000810: 6d61 6e64 2c20 6461 7461 290d 0a0d 0a20  mand, data).... 
-00000820: 2020 2064 6566 2073 746f 7028 7365 6c66     def stop(self
-00000830: 293a 0d0a 2020 2020 2020 2020 636f 6d6d  ):..        comm
-00000840: 616e 6420 3d20 2773 746f 7027 0d0a 2020  and = 'stop'..  
-00000850: 2020 2020 2020 6461 7461 203d 207b 2773        data = {'s
-00000860: 746f 7027 3a20 5472 7565 2c20 2773 7065  top': True, 'spe
-00000870: 6564 273a 2030 7d0d 0a20 2020 2020 2020  ed': 0}..       
-00000880: 2073 656c 662e 7365 6e64 5f63 6f6d 6d61   self.send_comma
-00000890: 6e64 2863 6f6d 6d61 6e64 2c20 6461 7461  nd(command, data
-000008a0: 290d 0a                                  )..
+00000000: 0d0a 0d0a 696d 706f 7274 2073 7973 0d0a  ....import sys..
+00000010: 696d 706f 7274 206c 6f67 6769 6e67 0d0a  import logging..
+00000020: 696d 706f 7274 2074 696d 650d 0a0d 0a66  import time....f
+00000030: 726f 6d20 7079 6d79 636f 626f 742e 6c6f  rom pymycobot.lo
+00000040: 6720 696d 706f 7274 2073 6574 7570 5f6c  g import setup_l
+00000050: 6f67 6769 6e67 0d0a 6672 6f6d 2070 796d  ogging..from pym
+00000060: 7963 6f62 6f74 2e65 7272 6f72 2069 6d70  ycobot.error imp
+00000070: 6f72 7420 6361 6c69 6272 6174 696f 6e5f  ort calibration_
+00000080: 7061 7261 6d65 7465 7273 0d0a 6672 6f6d  parameters..from
+00000090: 2070 796d 7963 6f62 6f74 2e63 6f6d 6d6f   pymycobot.commo
+000000a0: 6e20 696d 706f 7274 2050 726f 746f 636f  n import Protoco
+000000b0: 6c43 6f64 652c 2044 6174 6150 726f 6365  lCode, DataProce
+000000c0: 7373 6f72 0d0a 0d0a 0d0a 636c 6173 7320  ssor......class 
+000000d0: 5075 626c 6963 436f 6d6d 616e 6447 656e  PublicCommandGen
+000000e0: 6572 6174 6f72 2844 6174 6150 726f 6365  erator(DataProce
+000000f0: 7373 6f72 293a 0d0a 2020 2020 2320 6465  ssor):..    # de
+00000100: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00000110: 2064 6562 7567 3d46 616c 7365 293a 0d0a   debug=False):..
+00000120: 2020 2020 2320 2020 2020 2222 220d 0a20      #     """.. 
+00000130: 2020 2023 2020 2020 2041 7267 733a 0d0a     #     Args:..
+00000140: 2020 2020 2320 2020 2020 2020 2020 6465      #         de
+00000150: 6275 6720 2020 203a 2077 6865 7468 6572  bug    : whether
+00000160: 2073 686f 7720 6465 6275 6720 696e 666f   show debug info
+00000170: 0d0a 2020 2020 2320 2020 2020 2222 220d  ..    #     """.
+00000180: 0a20 2020 2023 2020 2020 2073 656c 662e  .    #     self.
+00000190: 5f76 6572 7369 6f6e 203d 2073 7973 2e76  _version = sys.v
+000001a0: 6572 7369 6f6e 5f69 6e66 6f5b 3a32 5d5b  ersion_info[:2][
+000001b0: 305d 0d0a 2020 2020 2320 2020 2020 7365  0]..    #     se
+000001c0: 6c66 2e64 6562 7567 203d 2064 6562 7567  lf.debug = debug
+000001d0: 0d0a 2020 2020 2320 2020 2020 7365 7475  ..    #     setu
+000001e0: 705f 6c6f 6767 696e 6728 7365 6c66 2e64  p_logging(self.d
+000001f0: 6562 7567 290d 0a20 2020 2023 2020 2020  ebug)..    #    
+00000200: 2073 656c 662e 6c6f 6720 3d20 6c6f 6767   self.log = logg
+00000210: 696e 672e 6765 744c 6f67 6765 7228 5f5f  ing.getLogger(__
+00000220: 6e61 6d65 5f5f 290d 0a20 2020 2023 2020  name__)..    #  
+00000230: 2020 2073 656c 662e 6361 6c69 6272 6174     self.calibrat
+00000240: 696f 6e5f 7061 7261 6d65 7465 7273 203d  ion_parameters =
+00000250: 2063 616c 6962 7261 7469 6f6e 5f70 6172   calibration_par
+00000260: 616d 6574 6572 730d 0a0d 0a20 2020 2023  ameters....    #
+00000270: 2064 6566 205f 6d65 7367 2873 656c 662c   def _mesg(self,
+00000280: 2067 656e 7265 2c20 2a61 7267 732c 202a   genre, *args, *
+00000290: 2a6b 7761 7267 7329 3a0d 0a20 2020 2023  *kwargs):..    #
+000002a0: 2020 2020 2022 2222 0d0a 2020 2020 2320       """..    # 
+000002b0: 2020 2020 4172 6773 3a0d 0a20 2020 2023      Args:..    #
+000002c0: 2020 2020 2020 2020 2067 656e 7265 3a20           genre: 
+000002d0: 636f 6d6d 616e 6420 7479 7065 2028 436f  command type (Co
+000002e0: 6d6d 616e 6429 0d0a 2020 2020 2320 2020  mmand)..    #   
+000002f0: 2020 2020 2020 2a61 7267 733a 206f 7468        *args: oth
+00000300: 6572 2064 6174 612e 0d0a 2020 2020 2320  er data...    # 
+00000310: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+00000320: 7420 6973 2063 6f6e 7665 7274 6564 2074  t is converted t
+00000330: 6f20 6f63 7461 6c20 6279 2064 6566 6175  o octal by defau
+00000340: 6c74 2e0d 0a20 2020 2023 2020 2020 2020  lt...    #      
+00000350: 2020 2020 2020 2020 2020 4966 2074 6865            If the
+00000360: 2064 6174 6120 6e65 6564 7320 746f 2062   data needs to b
+00000370: 6520 656e 6361 7073 756c 6174 6564 2069  e encapsulated i
+00000380: 6e74 6f20 6865 7861 6465 6369 6d61 6c2c  nto hexadecimal,
+00000390: 0d0a 2020 2020 2320 2020 2020 2020 2020  ..    #         
+000003a0: 2020 2020 2020 2074 6865 2061 7272 6179         the array
+000003b0: 2069 7320 7573 6564 2074 6f20 696e 636c   is used to incl
+000003c0: 7564 6520 7468 656d 2e20 2844 6174 6120  ude them. (Data 
+000003d0: 6361 6e6e 6f74 2062 6520 6e65 7374 6564  cannot be nested
+000003e0: 290d 0a20 2020 2023 2020 2020 2020 2020  )..    #        
+000003f0: 202a 2a6b 7761 7267 733a 2073 7570 706f   **kwargs: suppo
+00000400: 7274 2060 6861 735f 7265 706c 7960 0d0a  rt `has_reply`..
+00000410: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+00000420: 2020 6861 735f 7265 706c 793a 2057 6865    has_reply: Whe
+00000430: 7468 6572 2074 6865 7265 2069 7320 6120  ther there is a 
+00000440: 7265 7475 726e 2076 616c 7565 2074 6f20  return value to 
+00000450: 6163 6365 7074 2e0d 0a20 2020 2023 2020  accept...    #  
+00000460: 2020 2022 2222 0d0a 2020 2020 2320 2020     """..    #   
+00000470: 2020 636f 6d6d 616e 645f 6461 7461 203d    command_data =
+00000480: 2073 656c 662e 5f70 726f 6365 7373 5f64   self._process_d
+00000490: 6174 615f 636f 6d6d 616e 6428 6765 6e72  ata_command(genr
+000004a0: 652c 2061 7267 7329 0d0a 0d0a 2020 2020  e, args)....    
+000004b0: 2320 2020 2020 6966 2067 656e 7265 203d  #     if genre =
+000004c0: 3d20 3137 383a 0d0a 2020 2020 2320 2020  = 178:..    #   
+000004d0: 2020 2020 2020 636f 6d6d 616e 645f 6461        command_da
+000004e0: 7461 203d 2073 656c 662e 5f65 6e63 6f64  ta = self._encod
+000004f0: 655f 696e 7431 3628 636f 6d6d 616e 645f  e_int16(command_
+00000500: 6461 7461 290d 0a20 2020 2020 2020 2020  data)..         
+00000510: 2020 200d 0a20 2020 2023 2020 2020 2065     ..    #     e
+00000520: 6c69 6620 6765 6e72 6520 696e 205b 3736  lif genre in [76
+00000530: 2c20 3737 5d3a 0d0a 2020 2020 2320 2020  , 77]:..    #   
+00000540: 2020 2020 2020 636f 6d6d 616e 645f 6461        command_da
+00000550: 7461 203d 205b 636f 6d6d 616e 645f 6461  ta = [command_da
+00000560: 7461 5b30 5d5d 202b 2073 656c 662e 5f65  ta[0]] + self._e
+00000570: 6e63 6f64 655f 696e 7431 3628 636f 6d6d  ncode_int16(comm
+00000580: 616e 645f 6461 7461 5b31 5d2a 3130 290d  and_data[1]*10).
+00000590: 0a20 2020 2023 2020 2020 2065 6c69 6620  .    #     elif 
+000005a0: 6765 6e72 6520 3d3d 2031 3135 3a0d 0a20  genre == 115:.. 
+000005b0: 2020 2023 2020 2020 2020 2020 2063 6f6d     #         com
+000005c0: 6d61 6e64 5f64 6174 6120 3d20 5b63 6f6d  mand_data = [com
+000005d0: 6d61 6e64 5f64 6174 615b 315d 2c63 6f6d  mand_data[1],com
+000005e0: 6d61 6e64 5f64 6174 615b 335d 5d0d 0a0d  mand_data[3]]...
+000005f0: 0a20 2020 2023 2020 2020 204c 454e 203d  .    #     LEN =
+00000600: 206c 656e 2863 6f6d 6d61 6e64 5f64 6174   len(command_dat
+00000610: 6129 202b 2032 0d0a 2020 2020 2320 2020  a) + 2..    #   
+00000620: 2020 636f 6d6d 616e 6420 3d20 5b0d 0a20    command = [.. 
+00000630: 2020 2023 2020 2020 2020 2020 2050 726f     #         Pro
+00000640: 746f 636f 6c43 6f64 652e 4845 4144 4552  tocolCode.HEADER
+00000650: 2c0d 0a20 2020 2023 2020 2020 2020 2020  ,..    #        
+00000660: 2050 726f 746f 636f 6c43 6f64 652e 4845   ProtocolCode.HE
+00000670: 4144 4552 2c0d 0a20 2020 2023 2020 2020  ADER,..    #    
+00000680: 2020 2020 204c 454e 2c0d 0a20 2020 2023       LEN,..    #
+00000690: 2020 2020 2020 2020 2067 656e 7265 2c0d           genre,.
+000006a0: 0a20 2020 2023 2020 2020 2020 2020 2063  .    #         c
+000006b0: 6f6d 6d61 6e64 5f64 6174 612c 0d0a 2020  ommand_data,..  
+000006c0: 2020 2320 2020 2020 2020 2020 5072 6f74    #         Prot
+000006d0: 6f63 6f6c 436f 6465 2e46 4f4f 5445 522c  ocolCode.FOOTER,
+000006e0: 0d0a 2020 2020 2320 2020 2020 5d0d 0a0d  ..    #     ]...
+000006f0: 0a20 2020 2023 2020 2020 2072 6561 6c5f  .    #     real_
+00000700: 636f 6d6d 616e 6420 3d20 7365 6c66 2e5f  command = self._
+00000710: 666c 6174 7465 6e28 636f 6d6d 616e 6429  flatten(command)
+00000720: 0d0a 2020 2020 2320 2020 2020 6861 735f  ..    #     has_
+00000730: 7265 706c 7920 3d20 6b77 6172 6773 2e67  reply = kwargs.g
+00000740: 6574 2822 6861 735f 7265 706c 7922 2c20  et("has_reply", 
+00000750: 4661 6c73 6529 0d0a 2020 2020 2320 2020  False)..    #   
+00000760: 2020 7265 7475 726e 2072 6561 6c5f 636f    return real_co
+00000770: 6d6d 616e 642c 2068 6173 5f72 6570 6c79  mmand, has_reply
+00000780: 0d0a 2020 2020 7061 7373 0d0a            ..    pass..
```

### Comparing `pymycobot-3.4.6b1/pymycobot/mercurysocket.py` & `pymycobot-3.4.7b1/pymycobot/mercurysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/myagv.py` & `pymycobot-3.4.7b1/pymycobot/myagv.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/myarm.py` & `pymycobot-3.4.7b1/pymycobot/myarm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/myarm_api.py` & `pymycobot-3.4.7b1/pymycobot/myarm_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,18 @@
                 ProtocolCode.GET_RECV_QUEUE_SIZE,
                 ProtocolCode.GET_RECV_QUEUE_LENGTH,
                 ProtocolCode.COBOTX_GET_ANGLE,
                 ProtocolCode.GET_ENCODER,
                 ProtocolCode.SERVO_RESTORE,
                 ProtocolCode.GET_ERROR_DETECT_MODE,
                 ProtocolCode.GET_SERVO_MOTOR_CLOCKWISE,
-                ProtocolCode.GET_SERVO_MOTOR_CONFIG
+                ProtocolCode.GET_SERVO_MOTOR_CONFIG,
+                ProtocolCode.POWER_ON,
+                ProtocolCode.GET_MASTER_PIN_STATUS,
+                ProtocolCode.GET_ATOM_PIN_STATUS
             ]
 
             if genre in return_single_genres:
                 return self._process_single(res)
             elif genre in [ProtocolCode.GET_ANGLES, ProtocolCode.GET_JOINT_MAX_ANGLE, ProtocolCode.GET_JOINT_MIN_ANGLE]:
                 return [self._int2angle(angle) for angle in res]
             elif genre in [ProtocolCode.GET_SERVO_VOLTAGES]:
```

### Comparing `pymycobot-3.4.6b1/pymycobot/myarmm.py` & `pymycobot-3.4.7b1/pymycobot/myarmm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/myarmsocket.py` & `pymycobot-3.4.7b1/pymycobot/myarmsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/mybuddy.py` & `pymycobot-3.4.7b1/pymycobot/mybuddy.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/mybuddybluetooth.py` & `pymycobot-3.4.7b1/pymycobot/mybuddybluetooth.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/mybuddyemoticon.py` & `pymycobot-3.4.7b1/pymycobot/mybuddyemoticon.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/mybuddysocket.py` & `pymycobot-3.4.7b1/pymycobot/mybuddysocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/mycobot.py` & `pymycobot-3.4.7b1/pymycobot/mycobot.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/mycobotpro630.py` & `pymycobot-3.4.7b1/pymycobot/mycobotpro630.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,34 +5,54 @@
 import platform
 import time
 import math
 from enum import Enum
 import subprocess
 import logging
 import os
+import sys
 
 from pymycobot.log import setup_logging
 
 
+def check_python_version():
+    if sys.version_info.major == 2:
+        return 2
+    elif sys.version_info.major == 3:
+        return 3
+    else:
+        return -1
+
+
 def is_debian_os():
     try:
         # 执行 lsb_release -a 命令，并捕获输出
-        result = subprocess.run(
-            ["lsb_release", "-a"], capture_output=True, text=True, check=True
-        )
+        py_version = check_python_version()
+        if py_version == 3:
+            result = subprocess.run(
+                ["lsb_release", "-a"], capture_output=True, text=True, check=True
+            )
+
+            # 解析输出，获取 Distributor ID 的信息
+            lines = result.stdout.split("\n")
+
+        elif py_version == 2:
+            result = subprocess.Popen(
+                ["lsb_release", "-a"], stdout=subprocess.PIPE
+            ).communicate()[0]
+
+            # 解析输出，获取 Distributor ID 的信息
+            lines = result.split("\n")
 
-        # 解析输出，获取 Distributor ID 的信息
-        lines = result.stdout.split("\n")
         for line in lines:
             if line.startswith("Distributor ID:"):
                 distributor_id = line.split(":", 1)[1].strip()
                 if distributor_id != "Debian":
                     return False
                 return True
-
     except subprocess.CalledProcessError as e:
         print("Error executing lsb_release -a: {}".format(e))
         return False
 
     return None
 
 
@@ -49,15 +69,19 @@
 from time import sleep
 
 try:
     from gpiozero import CPUTemperature
 except ImportError:
 
     def CPUTemperature():
-        return 0
+        class Temp:
+            def __init__(self, temperature):
+                self.temperature = temperature
+
+        return Temp(0)
 
 
 COORDS_EPSILON = 0.50
 MAX_JOINTS = 6
 MAX_CARTE = 3
 jog_velocity = 1.0  # 100.0/60.0
 angular_jog_velocity = 3600 / 60
@@ -558,15 +582,15 @@
             msg = self.can_reader.get_message()
             if end_time < time.time():
                 break
         return msg
 
     def init_robot(self):
         """Initializes robot parameters."""
-        self.detect_robot()
+        self._detect_robot()
         self._set_free_move(False)
 
         self.set_carte_torque_limit(Axis.X, DEFAULT_XY_TORQUE_LIMIT)
         self.set_carte_torque_limit(Axis.Y, DEFAULT_XY_TORQUE_LIMIT)
         self.set_carte_torque_limit(Axis.Z, DEFAULT_Z_TORQUE_LIMIT)
 
         self.set_acceleration(400)
@@ -582,16 +606,14 @@
         self.set_joint_torque_limit(Joint.J1, 0.15)
         self.set_joint_torque_limit(Joint.J2, 0.15)
         self.set_joint_torque_limit(Joint.J3, 0.12)
         self.set_joint_torque_limit(Joint.J4, 0.10)
         self.set_joint_torque_limit(Joint.J5, 0.10)
         self.set_joint_torque_limit(Joint.J6, 0.10)
 
-        self.set_payload(1.0)
-
         # joint angle limits
         self.set_joint_min_pos_limit(Joint.J1, -180)
         self.set_joint_min_pos_limit(Joint.J2, -270)
         self.set_joint_min_pos_limit(Joint.J3, -150)
         self.set_joint_min_pos_limit(Joint.J4, -260)
         self.set_joint_min_pos_limit(Joint.J5, -168)
         self.set_joint_min_pos_limit(Joint.J6, -174)
@@ -601,15 +623,15 @@
         self.set_joint_max_pos_limit(Joint.J3, 150)
         self.set_joint_max_pos_limit(Joint.J4, 80)
         self.set_joint_max_pos_limit(Joint.J5, 168)
         self.set_joint_max_pos_limit(Joint.J6, 174)
 
         self.set_motion_flexible(0)
 
-    def detect_robot(self):
+    def _detect_robot(self):
         """Detects robot from Analog Input HAL pin."""
         robot = Robots(self.get_analog_in(AI.ROBOT))
         if robot == Robots.ELEPHANT:
             self.current_robot = 0
         elif robot == Robots.PANDA_3:
             self.current_robot = 1
         elif robot == Robots.PANDA_5:
@@ -631,27 +653,30 @@
         Args:
             power_on_only (bool, optional): Only do power on. Defaults to False.
 
         Returns:
             bool: True if start successful, False otherwise.
         """
         self._power_off()
-        time.sleep(1.0)
+        time.sleep(5.0)
+        self.enable_manual_brake_control(False)
         power_on_ok = self.is_power_on()
         power_on_retry_count = 0
         while (not power_on_ok) and (power_on_retry_count <= 10):
             if power_on_only:
                 self._power_on_only()
             else:
                 self._power_on()
             power_on_retry_count += 1
             power_on_ok = self.is_power_on()
             time.sleep(1)
         power_on_ok = self.is_power_on()
-        if not power_on_ok:
+        if power_on_ok and power_on_only:
+            return True
+        elif not power_on_ok:
             print("power_on_ok is false")
             return False
         # power on ok
         servo_enable_ok = False
         servo_enable_retry_count = 0
         while (not servo_enable_ok) and (servo_enable_retry_count <= 30):
             servo_enable_ok = self.is_all_servo_enabled()
@@ -751,14 +776,25 @@
         """
         self.set_digital_out(DO.POWER_ON_RELAY_1, 0)
         self.set_digital_out(DO.POWER_ON_RELAY_2, 0)
         if self.current_robot != Robots.ELEPHANT.value:
             self.set_digital_out(DO.BRAKE_ACTIVE_AUTO, 0)
         return True
 
+    def _check_speed(self, speed):
+        """Returns True if speed is within limits [0, 100], False otherwise.
+
+        Args:
+            speed (float): speed value to be checked
+
+        Returns:
+            bool: True if speed is within limits [0, 100], False otherwise
+        """
+        return speed >= 0 and speed <= 100
+
     def get_coords(self):
         """Returns current robot coordinates as list[X, Y, Z, RX, RY, RZ].
 
         Returns:
             list[float]: list of 6 float values for each axis
         """
         c = self._get_actual_position()
@@ -770,14 +806,16 @@
 
         Args:
             coords (list[float]): coords to set, list[float] of size 6
             speed (float): speed percentage (0 ~ 100 %)
         """
         if self.is_in_position(coords, True):
             return True
+        if not self._check_speed(speed):
+            return False
         self._set_robot_move_state(RobotMoveState.MOVE_AXIS_STATE, 0, 0)
         return self.send_mdi(
             "G01F" + str(speed * MAX_LINEAR_SPEED / 100) + self.coords_to_gcode(coords)
         )
 
     def get_coord(self, axis):
         """Returns current coord of specified axis.
@@ -794,17 +832,19 @@
         """Moves robot's given coordinate to specified value with set speed.
 
         Args:
             axis (Axis): Axis.X ~ Axis.RZ
             coord (float): coord value
             speed (float): speed percentage (1 ~ 100 %)
         """
+        if not self._check_speed(speed):
+            return False
         coords = self.get_coords()
         coords[axis.value] = coord
-        self.set_coords(coords, speed)
+        return self.set_coords(coords, speed)
 
     def get_angles(self):
         """Returns robot's current joint angle values.
 
         Returns:
             list[float]: current angles list[float] of size MAX_JOINTS
         """
@@ -814,17 +854,19 @@
         """Moves robot's joints angles to specified value with given speed.
 
         Args:
             angles (list[float]): joint angles, list[float] of size MAX_JOINTS
             speed (float): speed percentage (1 ~ 100 %)
         """
         if self.is_in_position(angles, False):
-            return
+            return True
+        if not self._check_speed(speed):
+            return False
         self._set_robot_move_state(RobotMoveState.MOVE_JOINT_STATE, 0, 0)
-        self.send_mdi(
+        return self.send_mdi(
             "G38.3F"
             + str(speed * MAX_ANGULAR_SPEED / 100)
             + self.angles_to_gcode(angles)
         )
 
     def get_angle(self, joint):
         """Returns robot's specified joint's current angle.
@@ -841,20 +883,22 @@
         """Moves robot's specified joint's angle to given value with passed speed.
 
         Args:
             joint (Joint): 0 ~ 5 or Joint.J1 ~ Joint.J6
             angle (float): angle to set
             speed (float): speed percentage (0 ~ 100 %)
         """
+        if not self._check_speed(speed):
+            return False
         angles = self.get_angles()
         if isinstance(joint, int):
             angles[joint] = angle
         elif isinstance(joint, Joint):
             angles[joint.value] = angle
-        self.set_angles(angles, speed)
+        return self.set_angles(angles, speed)
 
     def get_speed(self):
         """Returns current robot's speed.
 
         Returns:
             float: current robot's speed
         """
@@ -1120,14 +1164,15 @@
     def set_estop_reset(self):
         """Resets E-Stop (Emergency Stop) state of the robot."""
         self.c.state(elerob.STATE_ESTOP_RESET)
         self.c.wait_complete()
 
     def set_estop(self):
         """Puts robot into E-Stop (Emergency Stop) state."""
+        self.tool_set_led_color(255, 0, 0)
         self.c.state(elerob.STATE_ESTOP)
         self.c.wait_complete()
 
     def get_acceleration(self):
         """Returns acceleration value of robot.
 
         Returns:
@@ -1147,14 +1192,24 @@
         self.s.poll()
         if self.s.task_mode == task_mode.value:
             return True
         self.c.mode(task_mode.value)
         self.c.wait_complete()
         return True
 
+    def enable_manual_brake_control(self, enable=True):
+        """Enables or disables manual brake control.
+
+        Args:
+            enable (bool, optional): enable (True) or disable (False) manual
+                                     brake control. Defaults to True.
+        """
+        self.set_digital_out(DO.BRAKE_MANUAL_MODE_ENABLE, enable)
+        time.sleep(0.05)
+
     def release_joint_brake(self, joint, release=True):
         """Releases or focuses (enables) specified joint's brake.
 
         Args:
             joint (Joint): joint Joint.J1 ~ Joint.J6
             release (bool): True to release, False to enable brake. Defaults to True.
         """
@@ -1192,15 +1247,16 @@
         self.c.teleop_enable(enable)
         self.c.wait_complete()
 
     def get_robot_status(self):
         """Returns robot status.
 
         Returns:
-            bool: True if OK, False if disabled / error / cannot move
+            bool: True if robot started in normal mode, False if free move mode,
+                  disabled, error or cannot move
         """
         return self.state_check()
 
     def get_robot_temperature(self):
         """Returns robot's (currently CPU) temperature.
 
         Returns:
@@ -1254,26 +1310,15 @@
 
         Args:
             joint (Joint): joint enum value (Joint.J1 ~ Joint.J6)
 
         Returns:
             bool: True if joint communication is OK, False otherwise
         """
-        return not self.get_digital_in(DI(DI.J1_COMMUNICATION.value + joint.value))
-
-    def get_joint_voltage(self, joint):
-        """Returns specified joint's voltage.
-
-        Args:
-            joint (Joint): joint enum value (Joint.J1 ~ Joint.J6)
-
-        Returns:
-            float: voltage
-        """
-        return self.get_analog_in(AI(AI.J1_VOLTAGE.value + joint.value))
+        return bool(self.get_digital_in(DI(DI.J1_COMMUNICATION.value + joint.value)))
 
     def get_joint_current(self, joint):
         """Returns specified joint's current.
 
         Args:
             joint (Joint): joint enum value (Joint.J1 ~ Joint.J6)
 
@@ -1432,14 +1477,16 @@
             direction (JogDirection): JogDirection.POSITIVE (1) or
                                       JogDirection.NEGATIVE (-1) (1增大，-1减小)
             speed (float): speed percentage (0 ~ 100 %)
 
         Returns:
             bool: True if jog started successfully, False otherwise
         """
+        if not self._check_speed(speed):
+            return False
         self._set_robot_move_state(RobotMoveState.JOG_JOINT_STATE, joint, direction)
         self.command_id += 1
         return self._jog_continuous(
             JogMode.JOG_JOINT, joint, direction, speed, self.command_id
         )
 
     def jog_coord(self, axis, direction, speed):
@@ -1450,14 +1497,16 @@
             direction (JogDirection): JogDirection.POSITIVE (1) 增大,
                                       JogDirection.NEGATIVE (-1) 减小
             speed (float): speed percentage (1 ~ 100 %)
 
         Returns:
             bool: True if jog started successfully, False otherwise
         """
+        if not self._check_speed(speed):
+            return False
         self._set_robot_move_state(RobotMoveState.JOG_AXIS_STATE, axis, direction)
         self.command_id += 1
         return self._jog_continuous(
             JogMode.JOG_TELEOP, axis, direction, speed, self.command_id
         )
 
     def _jog_continuous(self, jog_mode, joint_or_axis, direction, speed, jog_id):
@@ -1510,27 +1559,31 @@
             joint (Joint): joint
             increment (float): angle
             speed (float): speed percentage (0 ~ 100 %)
 
         Returns:
             bool: True if jog successfully started, False otherwise
         """
+        if not self._check_speed(speed):
+            return False
         return self._jog_increment(JogMode.JOG_JOINT, joint, increment, speed)
 
     def jog_increment_coord(self, axis, increment, speed):
         """Move specified axis by given increment value with speed.
 
         Args:
             axis (Axis): axis
             increment (float): increment
             speed (float): speed percentage % (0 ~ 100)
 
         Returns:
             bool: True if jog successfully started, False otherwise
         """
+        if not self._check_speed(speed):
+            return False
         return self._jog_increment(JogMode.JOG_TELEOP, axis, increment, speed)
 
     def _jog_increment(self, jog_mode, joint_or_axis, incr, speed):
         """Move joint or axis by specified value.
 
         Args:
             jog_mode (JogMode): move by axis(0) or joint(1)
@@ -1577,27 +1630,31 @@
             joint (Joint): joint
             position (float): position
             speed (float): speed percentage (0 ~ 100 %)
 
         Returns:
             bool: True if jog started successfully, False otherwise
         """
+        if not self._check_speed(speed):
+            return False
         return self._jog_absolute(joint, JogMode.JOG_JOINT, position, speed)
 
     def jog_absolute_coord(self, axis, position, speed):
         """Jog given axis to the specified position with passed speed.
 
         Args:
             axis (Axis): axis
             position (float): position
             speed (float): speed percentage (0 ~ 100 %)
 
         Returns:
             bool: True if jog started successfully, False otherwise
         """
+        if not self._check_speed(speed):
+            return False
         return self._jog_absolute(axis, JogMode.JOG_TELEOP, position, speed)
 
     def _jog_absolute(self, joint_or_axis, jog_mode, pos, speed):
         """Jog joint or axis to specified position.
 
         Args:
             joint_or_axis (Joint | Axis): joint or axis
@@ -2578,17 +2635,20 @@
     def tool_get_firmware_version(self):
         """Returns ESP32 Pico firmware version.
 
         Returns:
             float: firmware version
         """
         self.send_can(data=[0x01, 0x09])
-        msg = self.receive_can()
-        print("msg.data = " + str(msg.data))
-        version = msg.data[2] / 10
+        version = 0.0
+        for _ in range(100):
+            msg = self.receive_can()
+            if msg.data[0] == 0x02 and msg.data[1] == 0x09:
+                version = msg.data[2] / 10
+                break
         return version
 
     def tool_set_digital_out(self, pin_no, pin_value):
         """Sets digital output pin on ESP32.
 
         Args:
             pin_no (int): pin number
@@ -2624,20 +2684,24 @@
         """
         self.send_can(data=[0x04, 0x70, r, g, b])
 
     def tool_is_btn_clicked(self):
         """Returns True if ESP32 button is pressed.
 
         Returns:
-            bool: True if button is pressed, False otherwise
+            bool: True if button is pressed, False otherwise, None if failed to get button status
         """
         self.send_can([0x01, 0x71])
-        msg = self.receive_can()
-        button_state = msg.data[2]
-        return bool(button_state)
+        button_state = None
+        for _ in range(100):
+            msg = self.receive_can()
+            if msg.data[0] == 0x02 and msg.data[1] == 0x71:
+                button_state = bool(msg.data[2])
+                break
+        return button_state
 
     def tool_set_gripper_state(self, state, speed):
         """Sets gripper state.
 
         Args:
             state (int): state
             speed (int): speed
```

### Comparing `pymycobot-3.4.6b1/pymycobot/mycobotsocket.py` & `pymycobot-3.4.7b1/pymycobot/mycobotsocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/mypalletizer.py` & `pymycobot-3.4.7b1/pymycobot/mypalletizer.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/mypalletizersocket.py` & `pymycobot-3.4.7b1/pymycobot/mypalletizersocket.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/robot_limit.json` & `pymycobot-3.4.7b1/pymycobot/robot_limit.json`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/ultraArm.py` & `pymycobot-3.4.7b1/pymycobot/ultraArm.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot/utils.py` & `pymycobot-3.4.7b1/pymycobot/utils.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/pymycobot.egg-info/PKG-INFO` & `pymycobot-3.4.7b1/pymycobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymycobot
-Version: 3.4.6b1
+Version: 3.4.7b1
 Summary: Python API for serial communication of MyCobot.
 Home-page: https://github.com/elephantrobotics/pymycobot
 Author: Elephantrobotics
 Author-email: weiquan.xu@elephantrobotics.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pymycobot-3.4.6b1/pymycobot.egg-info/SOURCES.txt` & `pymycobot-3.4.7b1/pymycobot.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 pymycobot/genre.py
 pymycobot/log.py
 pymycobot/mecharm.py
 pymycobot/mecharmsocket.py
 pymycobot/mercury.py
 pymycobot/mercury_api.py
 pymycobot/mercurychassis.py
-pymycobot/mercurychassisocket.py
 pymycobot/mercurysocket.py
 pymycobot/myagv.py
 pymycobot/myarm.py
 pymycobot/myarm_api.py
 pymycobot/myarmc.py
 pymycobot/myarmm.py
 pymycobot/myarmsocket.py
```

### Comparing `pymycobot-3.4.6b1/setup.py` & `pymycobot-3.4.7b1/setup.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/tests/test_api.py` & `pymycobot-3.4.7b1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/tests/test_generator.py` & `pymycobot-3.4.7b1/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pymycobot-3.4.6b1/tests/test_socket.py` & `pymycobot-3.4.7b1/tests/test_socket.py`

 * *Files identical despite different names*

