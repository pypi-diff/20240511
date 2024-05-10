# Comparing `tmp/pyrainbird-5.0.0.tar.gz` & `tmp/pyrainbird-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrainbird-5.0.0.tar", last modified: Sun May  5 06:55:39 2024, max compression
+gzip compressed data, was "pyrainbird-6.0.0.tar", last modified: Fri May 10 23:38:15 2024, max compression
```

## Comparing `pyrainbird-5.0.0.tar` & `pyrainbird-6.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:55:39.508157 pyrainbird-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-05 06:55:39.508157 pyrainbird-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:55:39.504157 pyrainbird-5.0.0/pyrainbird/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18927 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    23102 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/rainbird.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:55:39.504157 pyrainbird-5.0.0/pyrainbird/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/resources/models.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/resources/sipcommands.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/pyrainbird/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:55:39.508157 pyrainbird-5.0.0/pyrainbird.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-05 06:55:39.000000 pyrainbird-5.0.0/pyrainbird.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 06:55:39.000000 pyrainbird-5.0.0/pyrainbird.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 06:55:39.000000 pyrainbird-5.0.0/pyrainbird.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-05 06:55:39.000000 pyrainbird-5.0.0/pyrainbird.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-05 06:55:39.000000 pyrainbird-5.0.0/pyrainbird.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-05 06:55:39.508157 pyrainbird-5.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       80 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 06:55:39.508157 pyrainbird-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    47508 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/tests/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-05 06:55:35.000000 pyrainbird-5.0.0/tests/test_rainbird.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:38:15.338696 pyrainbird-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-10 23:38:15.338696 pyrainbird-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:38:15.334696 pyrainbird-6.0.0/pyrainbird/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/pyrainbird/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18923 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/pyrainbird/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/pyrainbird/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23102 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/pyrainbird/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/pyrainbird/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/pyrainbird/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/pyrainbird/rainbird.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:38:15.334696 pyrainbird-6.0.0/pyrainbird/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/pyrainbird/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/pyrainbird/resources/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/pyrainbird/resources/sipcommands.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/pyrainbird/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:38:15.334696 pyrainbird-6.0.0/pyrainbird.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-10 23:38:15.000000 pyrainbird-6.0.0/pyrainbird.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-10 23:38:15.000000 pyrainbird-6.0.0/pyrainbird.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:38:15.000000 pyrainbird-6.0.0/pyrainbird.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 23:38:15.000000 pyrainbird-6.0.0/pyrainbird.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 23:38:15.000000 pyrainbird-6.0.0/pyrainbird.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-10 23:38:15.338696 pyrainbird-6.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       80 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:38:15.334696 pyrainbird-6.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    48240 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/tests/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-10 23:38:11.000000 pyrainbird-6.0.0/tests/test_rainbird.py
```

### Comparing `pyrainbird-5.0.0/LICENSE` & `pyrainbird-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrainbird-5.0.0/PKG-INFO` & `pyrainbird-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyrainbird
-Version: 5.0.0
+Version: 6.0.0
 Summary: Rain Bird Controller
 Home-page: https://github.com/allenporter/pyrainbird
 Author: J.J.Barrancos
 Author-email: jordy@fusion-ict.nl
 License: MIT
 Keywords: Rain Bird
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome>=3.16.0
 Requires-Dist: requests>=2.22.0
 Requires-Dist: PyYAML>=5.4
 Requires-Dist: mashumaro>=3.12
 Requires-Dist: python-dateutil>=2.8.2
```

### Comparing `pyrainbird-5.0.0/README.md` & `pyrainbird-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrainbird-5.0.0/pyrainbird/async_client.py` & `pyrainbird-6.0.0/pyrainbird/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,15 @@
         mask = (
             "%%0%dX"
             % RAINBIRD_COMMANDS["CurrentStationsActiveResponse"]["activeStations"][
                 LENGTH
             ]
         )
         return await self._process_command(
-            lambda resp: States((mask % resp["activeStations"])[:6]),
+            lambda resp: States((mask % resp["activeStations"])),
             "CurrentStationsActiveRequest",
             0,
         )
 
     async def get_zone_state(self, zone: int) -> bool:
         """Return the current state of the zone."""
         states = await self.get_zone_states()
```

### Comparing `pyrainbird-5.0.0/pyrainbird/const.py` & `pyrainbird-6.0.0/pyrainbird/const.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-5.0.0/pyrainbird/data.py` & `pyrainbird-6.0.0/pyrainbird/data.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-5.0.0/pyrainbird/encryption.py` & `pyrainbird-6.0.0/pyrainbird/encryption.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-5.0.0/pyrainbird/rainbird.py` & `pyrainbird-6.0.0/pyrainbird/rainbird.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-5.0.0/pyrainbird/resources/__init__.py` & `pyrainbird-6.0.0/pyrainbird/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-5.0.0/pyrainbird/resources/models.yaml` & `pyrainbird-6.0.0/pyrainbird/resources/models.yaml`

 * *Files identical despite different names*

### Comparing `pyrainbird-5.0.0/pyrainbird/resources/sipcommands.yaml` & `pyrainbird-6.0.0/pyrainbird/resources/sipcommands.yaml`

 * *Files identical despite different names*

### Comparing `pyrainbird-5.0.0/pyrainbird/timeline.py` & `pyrainbird-6.0.0/pyrainbird/timeline.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-5.0.0/pyrainbird.egg-info/PKG-INFO` & `pyrainbird-6.0.0/pyrainbird.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyrainbird
-Version: 5.0.0
+Version: 6.0.0
 Summary: Rain Bird Controller
 Home-page: https://github.com/allenporter/pyrainbird
 Author: J.J.Barrancos
 Author-email: jordy@fusion-ict.nl
 License: MIT
 Keywords: Rain Bird
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome>=3.16.0
 Requires-Dist: requests>=2.22.0
 Requires-Dist: PyYAML>=5.4
 Requires-Dist: mashumaro>=3.12
 Requires-Dist: python-dateutil>=2.8.2
```

### Comparing `pyrainbird-5.0.0/pyrainbird.egg-info/SOURCES.txt` & `pyrainbird-6.0.0/pyrainbird.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrainbird-5.0.0/setup.cfg` & `pyrainbird-6.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
 name = pyrainbird
-version = 5.0.0
+version = 6.0.0
 description = Rain Bird Controller
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/pyrainbird
 author = J.J.Barrancos
 author_email = jordy@fusion-ict.nl
 license = MIT
 license_file = LICENSE
 keywords = Rain Bird
 
 [options]
 packages = find:
-python_requires = >=3.10
+python_requires = >=3.11
 install_requires = 
 	pycryptodome>=3.16.0
 	requests>=2.22.0
 	PyYAML>=5.4
 	mashumaro>=3.12
 	python-dateutil>=2.8.2
 	ical>=4.2.9
```

### Comparing `pyrainbird-5.0.0/tests/test_async_client.py` & `pyrainbird-6.0.0/tests/test_async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,14 +312,38 @@
     for i in range(1, 9):
         for j in range(1, 9):
             mask = (1 << (i - 1)) * 0x1000000
             api_response("BF", pageNumber=0, activeStations=mask)
             assert await controller.get_zone_state(j) == (i == j)
 
 
+@pytest.mark.parametrize(
+    ("sip_data", "active_zones"),
+    [
+        ("BF0000000000", []),
+        ("BF0000010000", [9]),
+        ("BF0000000001", [25]),
+        ("BF0000000002", [26]),
+        ("BF0000000004", [27]),
+        ("BF0000381000", [12, 13, 14, 21]),
+    ],
+)
+async def test_get_zone_state_lxivm(
+    rainbird_controller: Callable[[], Awaitable[AsyncRainbirdController]],
+    sip_data_responses: Callable[[list[str]], None],
+    sip_data: str,
+    active_zones: list[int],
+) -> None:
+    controller = await rainbird_controller()
+    sip_data_responses([sip_data])
+    zone_states = await controller.get_zone_states()
+    active_states = sorted(list(zone_states.active_set))
+    assert active_states == active_zones
+
+
 async def test_set_program(
     rainbird_controller: Callable[[], Awaitable[AsyncRainbirdController]],
     api_response: Callable[[...], Awaitable[None]],
 ) -> None:
     controller = await rainbird_controller()
     api_response("01", commandEcho=5)
     await controller.set_program(5)
@@ -1269,15 +1293,14 @@
     assert [event.start for event in events] == [
         datetime.datetime(2023, 1, 24, 4, 0, 0),
         datetime.datetime(2023, 1, 30, 4, 0, 0),
         datetime.datetime(2023, 2, 5, 4, 0, 0),
     ]
 
 
-
 @freeze_time("2023-01-25 20:00:00")
 async def test_get_schedule_parse_failure(
     rainbird_controller: Callable[[], Awaitable[AsyncRainbirdController]],
     api_response: Callable[[...], Awaitable[None]],
     sip_data_responses: Callable[[list[str]], None],
 ) -> None:
     """Test a schedule that fails to parse."""
```

### Comparing `pyrainbird-5.0.0/tests/test_data.py` & `pyrainbird-6.0.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-5.0.0/tests/test_rainbird.py` & `pyrainbird-6.0.0/tests/test_rainbird.py`

 * *Files identical despite different names*

