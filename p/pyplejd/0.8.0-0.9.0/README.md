# Comparing `tmp/pyplejd-0.8.0.tar.gz` & `tmp/pyplejd-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplejd-0.8.0.tar", last modified: Sat Jan 27 23:11:11 2024, max compression
+gzip compressed data, was "pyplejd-0.9.0.tar", last modified: Tue Feb 20 22:00:31 2024, max compression
```

## Comparing `pyplejd-0.8.0.tar` & `pyplejd-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-01-27 23:11:11.938502 pyplejd-0.8.0/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-07-15 23:38:48.000000 pyplejd-0.8.0/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2024-01-27 23:11:11.938502 pyplejd-0.8.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      528 2023-10-11 18:49:48.000000 pyplejd-0.8.0/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-01-27 23:11:11.938502 pyplejd-0.8.0/pyplejd/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3637 2024-01-02 23:16:05.000000 pyplejd-0.8.0/pyplejd/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-01-27 23:11:11.938502 pyplejd-0.8.0/pyplejd/ble/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13175 2024-01-02 20:00:14.000000 pyplejd-0.8.0/pyplejd/ble/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1056 2023-08-04 07:28:17.000000 pyplejd-0.8.0/pyplejd/ble/crypto.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-01-27 23:11:11.938502 pyplejd-0.8.0/pyplejd/cloud/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8906 2024-01-03 20:22:48.000000 pyplejd-0.8.0/pyplejd/cloud/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4735 2023-11-09 21:49:21.000000 pyplejd-0.8.0/pyplejd/cloud/site_details.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      305 2023-10-11 18:38:57.000000 pyplejd-0.8.0/pyplejd/cloud/site_list.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1606 2024-01-27 18:54:55.000000 pyplejd-0.8.0/pyplejd/const.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      135 2023-12-29 13:03:03.000000 pyplejd-0.8.0/pyplejd/errors.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4059 2024-01-03 20:22:24.000000 pyplejd-0.8.0/pyplejd/interface.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-01-27 23:11:11.938502 pyplejd-0.8.0/pyplejd.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2024-01-27 23:11:11.000000 pyplejd-0.8.0/pyplejd.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      395 2024-01-27 23:11:11.000000 pyplejd-0.8.0/pyplejd.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-01-27 23:11:11.000000 pyplejd-0.8.0/pyplejd.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       45 2024-01-27 23:11:11.000000 pyplejd-0.8.0/pyplejd.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2024-01-27 23:11:11.000000 pyplejd-0.8.0/pyplejd.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       79 2024-01-27 23:11:11.938502 pyplejd-0.8.0/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)      677 2024-01-27 23:10:40.000000 pyplejd-0.8.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-20 22:00:31.297539 pyplejd-0.9.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-07-15 23:38:48.000000 pyplejd-0.9.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2024-02-20 22:00:31.297539 pyplejd-0.9.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      528 2023-10-11 18:49:48.000000 pyplejd-0.9.0/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-20 22:00:31.297539 pyplejd-0.9.0/pyplejd/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3659 2024-02-20 21:16:41.000000 pyplejd-0.9.0/pyplejd/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-20 22:00:31.297539 pyplejd-0.9.0/pyplejd/ble/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14780 2024-02-20 20:57:24.000000 pyplejd-0.9.0/pyplejd/ble/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1056 2023-08-04 07:28:17.000000 pyplejd-0.9.0/pyplejd/ble/crypto.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-20 22:00:31.297539 pyplejd-0.9.0/pyplejd/cloud/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9006 2024-02-20 21:57:22.000000 pyplejd-0.9.0/pyplejd/cloud/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4769 2024-02-20 21:05:57.000000 pyplejd-0.9.0/pyplejd/cloud/site_details.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      305 2023-10-11 18:38:57.000000 pyplejd-0.9.0/pyplejd/cloud/site_list.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1660 2024-02-20 21:55:49.000000 pyplejd-0.9.0/pyplejd/const.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      135 2023-12-29 13:03:03.000000 pyplejd-0.9.0/pyplejd/errors.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4069 2024-02-20 21:54:42.000000 pyplejd-0.9.0/pyplejd/interface.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-02-20 22:00:31.297539 pyplejd-0.9.0/pyplejd.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2024-02-20 22:00:31.000000 pyplejd-0.9.0/pyplejd.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      395 2024-02-20 22:00:31.000000 pyplejd-0.9.0/pyplejd.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-02-20 22:00:31.000000 pyplejd-0.9.0/pyplejd.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       45 2024-02-20 22:00:31.000000 pyplejd-0.9.0/pyplejd.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2024-02-20 22:00:31.000000 pyplejd-0.9.0/pyplejd.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       79 2024-02-20 22:00:31.297539 pyplejd-0.9.0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      677 2024-02-20 21:59:54.000000 pyplejd-0.9.0/setup.py
```

### Comparing `pyplejd-0.8.0/LICENSE` & `pyplejd-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplejd-0.8.0/README.md` & `pyplejd-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyplejd-0.8.0/pyplejd/__init__.py` & `pyplejd-0.9.0/pyplejd/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TYPE_CHECKING
 
 from bleak_retry_connector import close_stale_connections
 
 from .ble import PlejdMesh
 from .cloud import PlejdCloudSite
 
-from .const import PLEJD_SERVICE, LIGHT, SENSOR, SWITCH, UNKNOWN
+from .const import PLEJD_SERVICE, LIGHT, SENSOR, MOTION, SWITCH, UNKNOWN
 from .errors import AuthenticationError, ConnectionError
 from .interface import PlejdCloudCredentials
 
 if TYPE_CHECKING:
     from .interface import PlejdDevice, PlejdScene
 
 _LOGGER = logging.getLogger(__name__)
@@ -20,14 +20,15 @@
 __all__ = [
     "PlejdManager",
     "get_sites",
     "verify_credentials"
     "PLEJD_SERVICE",
     "LIGHT",
     "SENSOR",
+    "MOTION",
     "SWITCH",
     "UNKNOWN",
     "AuthenticationError",
     "ConnectionError",
     "PlejdCloudCredentials"
 ]
```

### Comparing `pyplejd-0.8.0/pyplejd/ble/__init__.py` & `pyplejd-0.9.0/pyplejd/ble/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from bleak.backends.device import BLEDevice
 from bleak_retry_connector import establish_connection
 
 from .crypto import auth_response, encrypt_decrypt
 from ..const import PLEJD_AUTH, PLEJD_LASTDATA, PLEJD_LIGHTLEVEL, PLEJD_PING, PLEJD_DATA
 
 _LOGGER = logging.getLogger(__name__)
+_DEVLOGGER = logging.getLogger("pyplejd.dev")
 
 
 class PlejdMesh:
     def __init__(self):
         self._seen_nodes: dict[BLEDevice, int] = {}
         self._expected_nodes = set()
         self._connectable_nodes = set()
@@ -331,25 +332,60 @@
                 self._publish(
                     self._scene_listeners,
                     {
                         "scene": scene,
                     },
                 )
             case b"\x04\x20":
-                colortemp = int.from_bytes(data[8:10], "big")
-                _LOGGER.debug("Address: %s Colortemp: %s", address, colortemp)
-                self._publish(
-                self._state_listeners,
-                    {
-                        "address": address,
-                        "colortemp": colortemp,
-                    },
-                )
+                if len(data) < 6:
+                    return
+                if data[6] == 1:
+                    colortemp = int.from_bytes(data[8:10], "big")
+                    _LOGGER.debug("Address: %s Colortemp: %s", address, colortemp)
+
+                    self._publish(
+                        self._state_listeners,
+                        {
+                            "address": address,
+                            "colortemp": colortemp,
+                        },
+                    )
+                elif data[6] == 3:
+                    luminosity = int.from_bytes(data[-2:], "big")
+                    _LOGGER.debug("Address: %s luminosity: %s", address, luminosity)
+                    self._publish(
+                        self._button_listeners,
+                        {
+                            "address": address,
+                            "button": 0,
+                        },
+                    )
+                else:
+                    if len(data) > 10:
+                        _DEVLOGGER.debug(
+                            "Unknown new-style LASTDATA command - address: %s - %s %s %s %s %s",
+                            address,
+                            data.hex()[0:2],
+                            data.hex()[2:6],
+                            data.hex()[6:10],
+                            data.hex()[10:16],
+                            data.hex()[16:]
+                        )
+                    else:
+                        _DEVLOGGER.debug(
+                            "Unknown new-style LASTDATA command - address: %s - %s %s %s %s",
+                            address,
+                            data.hex()[0:2],
+                            data.hex()[2:6],
+                            data.hex()[6:10],
+                            data.hex()[10:]
+                        )
             case _:
                 _LOGGER.debug("Unknown cmd (%s) to %s: %s", cmd, address, data[5:])
+                _DEVLOGGER.debug("Unknown LASTDATA cmd (%s) to %s: %s", cmd, address, data[5:])
 
     def _parse_lightlevel(self, lightlevel: bytearray):
         _LOGGER.debug("Parsing LIGHTLEVEL: %s", lightlevel.hex())
         for i in range(0, len(lightlevel), 10):
             ll = lightlevel[i : i + 10]
             address = int(ll[0])
             state = bool(ll[1])
```

### Comparing `pyplejd-0.8.0/pyplejd/ble/crypto.py` & `pyplejd-0.9.0/pyplejd/ble/crypto.py`

 * *Files identical despite different names*

### Comparing `pyplejd-0.8.0/pyplejd/cloud/__init__.py` & `pyplejd-0.9.0/pyplejd/cloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,16 @@
 
             inputSettings = (s for s in details.inputSettings if s.deviceId == deviceId)
             for inpt in inputSettings:
                 if inpt.input is not None:
                     inputs = details.inputAddress.get(deviceId)
                     if inputs:
                         inputAddress.append(inputs[str(inpt.input)])
+                if inpt.motionSensorData is not None:
+                    outputType = const.MOTION
 
             room = next((r for r in details.rooms if r.roomId == device.roomId), None)
             if room is not None:
                 room = room.title
 
             retval.append(
                 PlejdDevice(
```

### Comparing `pyplejd-0.8.0/pyplejd/cloud/site_details.py` & `pyplejd-0.9.0/pyplejd/cloud/site_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     # diagnostics: str
 
 
 class PlejdDeviceInputSetting(PlejdObject):
     deviceId: str
     siteId: str
     input: int
+    motionSensorData: dict | None
     # buttonType: str = ""
     # dimSpeed: int = 0
     # doubleSidedDirectionButton: bool = False
     # singleClick: str | None = None
     # doubleClick: str | None = None
```

### Comparing `pyplejd-0.8.0/pyplejd/const.py` & `pyplejd-0.9.0/pyplejd/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 PLEJD_DATA = f"31ba0004-{BLE_UUID_SUFFIX}"
 PLEJD_LASTDATA = f"31ba0005-{BLE_UUID_SUFFIX}"
 PLEJD_AUTH = f"31ba0009-{BLE_UUID_SUFFIX}"
 PLEJD_PING = f"31ba000a-{BLE_UUID_SUFFIX}"
 
 LIGHT = "LIGHT"
 SENSOR = "SENSOR"
+MOTION = "MOTION"
 SWITCH = "RELAY"
 UNKNOWN = "UNKNOWN"
 
 
 class Device:
     def __init__(self, name, type, dimmable=False, colortemp=False):
         self.name = name
@@ -37,12 +38,13 @@
     "14": Device("DIM-01-LC", LIGHT, dimmable=True),
     "15": Device("DIM-02-LC", LIGHT, dimmable=True),
     "17": Device("REL-01-2P", SWITCH),
     "18": Device("REL-02", SWITCH),
     "19": Device("EXT-01", UNKNOWN),
     "20": Device("SPR-01", SWITCH),
     "36": Device("LED-75", LIGHT, dimmable=True),
+    "70": Device("WMS-01", MOTION),
     "167": Device("DWN-01", LIGHT, dimmable=True, colortemp=True),
     "199": Device("DWN-02", LIGHT, dimmable=True, colortemp=True),
 }
 
 HARDWARE_UNKNOWN = HARDWARE["0"]
```

### Comparing `pyplejd-0.8.0/pyplejd/interface.py` & `pyplejd-0.9.0/pyplejd/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     rxaddress: int | None
     BLEaddress: str
 
     name: str
     hardware: str
     dimmable: bool | None
     colortemp: list | bool
-    outputType: Literal["LIGHT", "SENSOR", "RELAY", "UNKNOWN"] | None
+    outputType: Literal["LIGHT", "SENSOR", "RELAY", "MOTION", "UNKNOWN"] | None
     room: str
     firmware: str
     inputAddress: list[int]
     hidden: bool
 
     _state: bool = PrivateAttr()
     _dim: int = PrivateAttr()
```

### Comparing `pyplejd-0.8.0/setup.py` & `pyplejd-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 MIN_PY_VERSION = "3.10"
 PACKAGES = find_packages()
-VERSION = "0.8.0"
+VERSION = "0.9.0"
 
 setup(
     name="pyplejd",
     packages=PACKAGES,
     version=VERSION,
     description="A python library for communicating with Plejd devices via bluetooth",
     author="Thomas Lovén",
```

