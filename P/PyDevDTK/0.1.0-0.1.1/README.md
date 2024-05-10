# Comparing `tmp/pydevdtk-0.1.0.tar.gz` & `tmp/pydevdtk-0.1.1.tar.gz`

## Comparing `pydevdtk-0.1.0.tar` & `pydevdtk-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/.flake8
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/.gitattributes
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/.vscode/launch.json
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/docs/api.rst
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/docs/index.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/docs/make.bat
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/docs/_templates/custom-class-template.rst
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/examples/ble_example.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/examples/plotter_base_demo.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/examples/plotter_demo.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/examples/serial_example.py
--rw-r--r--   0        0        0    60154 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/images/icon.png
--rw-r--r--   0        0        0    16688 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/images/icon.svg
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/requirements/build.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/requirements/default.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/requirements/dev.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/requirements/doc.txt
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/src/pydevdtk/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/src/pydevdtk/coms/__init__.py
--rw-r--r--   0        0        0    19374 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/src/pydevdtk/coms/ble.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/src/pydevdtk/coms/serial.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/src/pydevdtk/plotting/__init__.py
--rw-r--r--   0        0        0     9524 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/src/pydevdtk/plotting/plotter.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/src/pydevdtk/plotting/plotter_base.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/src/pydevdtk/plotting/plotter_manager.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/LICENSE
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/README.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 pydevdtk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/.flake8
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/.gitattributes
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/.vscode/launch.json
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/docs/coms.rst
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/docs/examples.rst
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/docs/plotting.rst
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/docs/_templates/versions.html
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/examples/ble_example.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/examples/plotter_base_demo.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/examples/plotter_demo.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/examples/serial_example.py
+-rw-r--r--   0        0        0    60154 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/images/icon.png
+-rw-r--r--   0        0        0    16688 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/images/icon.svg
+-rw-r--r--   0        0        0  5041829 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/images/plotter_demo.gif
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/requirements/build.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/requirements/default.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/requirements/dev.txt
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/requirements/doc.txt
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/src/pydevdtk/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/src/pydevdtk/version.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/src/pydevdtk/coms/__init__.py
+-rw-r--r--   0        0        0    19586 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/src/pydevdtk/coms/ble.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/src/pydevdtk/coms/serial.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/src/pydevdtk/plotting/__init__.py
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/src/pydevdtk/plotting/plotter.py
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/src/pydevdtk/plotting/plotter_base.py
+-rw-r--r--   0        0        0     8964 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/src/pydevdtk/plotting/plotter_manager.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/README.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pydevdtk-0.1.1/PKG-INFO
```

### Comparing `pydevdtk-0.1.0/docs/Makefile` & `pydevdtk-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydevdtk-0.1.0/docs/conf.py` & `pydevdtk-0.1.1/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "PyDevDTK"
 copyright = "2024, Bojan Sofronievski"
 author = "Bojan Sofronievski"
-release = "0.1.0"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.duration",
     "sphinx.ext.viewcode",
     "sphinx.ext.githubpages",
+    "sphinx_multiversion",
+    "sphinx.ext.napoleon",
     "myst_parser",
 ]
 
 autodoc_mock_imports = ["serial", "bleak", "numpy", "matplotlib"]
 
 templates_path = ["_templates"]
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
```

### Comparing `pydevdtk-0.1.0/docs/make.bat` & `pydevdtk-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pydevdtk-0.1.0/examples/ble_example.py` & `pydevdtk-0.1.1/examples/ble_example.py`

 * *Files identical despite different names*

### Comparing `pydevdtk-0.1.0/examples/plotter_base_demo.py` & `pydevdtk-0.1.1/examples/plotter_base_demo.py`

 * *Files identical despite different names*

### Comparing `pydevdtk-0.1.0/examples/plotter_demo.py` & `pydevdtk-0.1.1/examples/plotter_demo.py`

 * *Files identical despite different names*

### Comparing `pydevdtk-0.1.0/examples/serial_example.py` & `pydevdtk-0.1.1/examples/serial_example.py`

 * *Files identical despite different names*

### Comparing `pydevdtk-0.1.0/images/icon.png` & `pydevdtk-0.1.1/images/icon.png`

 * *Files identical despite different names*

### Comparing `pydevdtk-0.1.0/images/icon.svg` & `pydevdtk-0.1.1/images/icon.svg`

 * *Files identical despite different names*

### Comparing `pydevdtk-0.1.0/src/pydevdtk/coms/ble.py` & `pydevdtk-0.1.1/src/pydevdtk/coms/ble.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,86 +13,112 @@
 
     Connecting = enum.auto()
     Connected = enum.auto()
     Disconnecting = enum.auto()
 
 
 class BleDevice:
-    """BLE device advertisement data and connection related objects"""
+    """
+    BLE device advertisement data and connection related objects.
+
+    Parameters
+    ----------
+    name : str or None
+        The name of the device. Can be None.
+    address : str
+        The address of the device.
+    rssi : int
+        The received signal strength indicator (RSSI) of the device.
+    uuids : list of str
+        A list of UUIDs associated with the device.
+    manufacturer_data : dict of int to bytes
+        A dictionary containing manufacturer-specific data.
+
+    Attributes
+    ----------
+    name : str or None
+        The name of the device. Can be None.
+    address : str
+        The address of the device.
+    rssi : int
+        The received signal strength indicator (RSSI) of the device.
+    uuids : list of str
+        A list of UUIDs associated with the device.
+    manufacturer_data : dict of int to bytes
+        A dictionary containing manufacturer-specific data.
+    """
 
     def __init__(
         self,
         name: str | None,
         address: str,
         rssi: int,
         uuids: list[str],
         manufacturer_data: dict[int, bytes],
     ):
-        """
-        Initializes a new instance of the BleDevice class.
-
-        Parameters
-        ----------
-        name : str or None
-            The name of the device. Can be None.
-        address : str
-            The address of the device.
-        rssi : int
-            The received signal strength indicator (RSSI) of the device.
-        uuids : list of str
-            A list of UUIDs associated with the device.
-        manufacturer_data : dict of int to bytes
-            A dictionary containing manufacturer-specific data.
-        """
         self.name = name
         self.address = address
         self.rssi = rssi
         self.uuids = uuids
         self.manufacturer_data = manufacturer_data
         self._device_hndl = None
         self._client = None
 
     def __str__(self) -> str:
         return self.name if self.name is not None else ""
 
 
 class BleCharacteristic:
-    """BLE characteristic description"""
+    """
+    BLE characteristic description.
 
-    def __init__(self, uuid: str, properties: list[str]):
-        """
-        Initializes a new instance of the BleCharacteristic class.
+    Parameters
+    ----------
+    uuid : str
+        The UUID of the characteristic.
+    properties : list of str
+        The properties of the characteristic. It can be a list of one or more
+        strings, which can be 'read', 'write', 'write-without-response',
+        'notify' or 'indicate'.
+
+    Attributes
+    ----------
+    uuid : str
+        The UUID of the characteristic.
+    properties : list of str
+        The properties of the characteristic.
+    """
 
-        Parameters
-        ----------
-        uuid : str
-            The UUID of the characteristic.
-        properties : list of str
-            The properties of the characteristic, which can be one or more of:
-            'read', 'write', 'write-without-response', 'notify' or 'indicate'.
-        """
+    def __init__(self, uuid: str, properties: list[str]):
         self.uuid = uuid
         self.properties = properties
 
 
 class BleService:
-    """BLE service description"""
+    """
+    BLE service description.
 
-    def __init__(self, uuid: str, characteristics: list[BleCharacteristic]):
-        """
-        Initializes a new instance of the BleService class.
+    Parameters
+    ----------
+    uuid : str
+        The UUID of the service.
+    characteristics : List[BleCharacteristic]
+        A list of BleCharacteristic objects representing the
+        characteristics of the service.
+
+    Attributes
+    ----------
+    uuid : str
+        The UUID of the service.
+    characteristics : List[BleCharacteristic]
+        A list of BleCharacteristic objects representing the
+        characteristics of the service.
+    """
 
-        Parameters
-        ----------
-        uuid : str
-            The UUID of the service.
-        characteristics : list of BleCharacteristic
-            A list of BleCharacteristic objects representing the
-            characteristics of the service.
-        """
+    def __init__(self, uuid: str, characteristics: list[BleCharacteristic]):
         self.uuid = uuid
         self.characteristics = characteristics
 
 
 class Ble:
     """
     A class that allows to utilize the BLE module of the device,
@@ -104,22 +130,14 @@
         """
         Initializes a new instance allowing to utilize the BLE module of the
         device, including scanning for BLE devices, connecting to BLE devices,
         and data operations including read, write and notify.
 
         Runs asyncio event loop in a separate thread which handles all BLE
         events.
-
-        Parameters
-        ----------
-        None
-
-        Returns
-        -------
-        None
         """
         self.found_devices: dict[str, BleDevice] = {}
         self.on_device: Callable[[BleDevice], None] | None = None
         self.scanning = False
         self.scan_stop_event = asyncio.Event()
 
         self.on_connect: dict[str, Callable[[], None]] = {}
@@ -146,52 +164,36 @@
 
         Parameters
         ----------
         on_device : Callable[[BleDevice], None] or None, optional
             Optional callback function to be called when a BLE device is found.
             The callback function should take a `BleDevice` object as its
             parameter.
-
-        Returns
-        -------
-        None
         """
         self.found_devices = {}  # clear previously found devices
         self.on_device = on_device
         self.scan_stop_event.clear()
         asyncio.run_coroutine_threadsafe(
             self._bluetooth_scan(self.scan_stop_event), self.event_loop
         )
         self.scanning = True
 
     def stop_scan(self):
         """
         Stops the ongoing Bluetooth Low Energy (BLE) scan if it is currently
         running.
-
-        Parameters
-        ----------
-        None
-
-        Returns
-        -------
-        None
         """
         if self.scanning:
             self.event_loop.call_soon_threadsafe(self.scan_stop_event.set)
             self.scanning = False
 
     def is_scanning(self) -> bool:
         """
         Returns the scanning status.
 
-        Parameters
-        ----------
-        None
-
         Returns
         -------
         bool
             The scanning status (True if scanning, False otherwise).
         """
         return self.scanning
 
@@ -220,18 +222,14 @@
         ----------
         dev : BleDevice
             The BLE device to connect to.
         on_connect : Callable[[], None] or None, optional
             Callback for when the connection is established. Defaults to None.
         on_disconnect : Callable[[], None] or None, optional
             Callback for when the connection is terminated. Defaults to None.
-
-        Returns
-        -------
-        None
         """
         if not self.is_connected(dev):
             if on_connect is not None:
                 self.on_connect[dev.address] = on_connect
             if on_disconnect is not None:
                 self.on_disconnect[dev.address] = on_disconnect
             self.disconnect_events[dev.address] = asyncio.Event()
@@ -247,18 +245,14 @@
         """
         Disconnects a BLE device if it is currently connected to it.
 
         Parameters
         ----------
         dev : BleDevice
             The BLE device to disconnect.
-
-        Returns
-        -------
-        None
         """
         if self.is_connected(dev):
             self.status_devices[dev.address] = BleStatus.Disconnecting
             self.event_loop.call_soon_threadsafe(
                 self.disconnect_events[dev.address].set
             )
 
@@ -299,15 +293,16 @@
         ----------
         dev : BleDevice
             The BLE device for which to retrieve the status.
 
         Returns
         -------
         BleStatus or None
-            The connection status of the device.
+            The connection status of the device, if device is connected.
+            None if the device is not connected.
         """
         if dev.address in self.status_devices:
             return self.status_devices[dev.address]
         else:
             return None
 
     def get_services_and_characteristics(
@@ -407,20 +402,19 @@
         response : bool
             Whether to expect a response from the device.
 
         Returns
         -------
         bytearray or None
             The result of the write operation, or None if the write failed.
-
-        This function checks if the device is connected and if the
-        characteristic exists and is writable. If so, it writes the data to
-        the characteristic. The result of the write operation is returned.
-        If the device is not connected or the characteristic does not exist or
-        is not writable, None is returned.
+            This function checks if the device is connected and if the
+            characteristic exists and is writable. If so, it writes the data to
+            the characteristic. The result of the write operation is returned.
+            If the device is not connected or the characteristic does not
+            exist or is not writable, None is returned.
         """
         if self.is_connected(dev):
             client = self.connected_devices[dev.address]._client
             chars = list(client.services.characteristics.values())
             chars_uuids = [char.uuid for char in chars]
             chars_properties = [char.properties for char in chars]
             if char_uuid in chars_uuids:
```

### Comparing `pydevdtk-0.1.0/src/pydevdtk/coms/serial.py` & `pydevdtk-0.1.1/src/pydevdtk/coms/serial.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         Parameters
         ----------
         port : str
             The name of the serial port to open.
         on_data : Callable[[bytes], None]
             A callback function that will be called whenever new data is
             received from the serial port.
-        **port_kwargs
+        port_kwargs
             Additional keyword arguments to pass to the `serial.Serial`
             constructor, such as baud_rate, parity, etc. Check the
             `serial.Serial` documentation for more information.
 
         Returns
         -------
         bool
```

### Comparing `pydevdtk-0.1.0/.gitignore` & `pydevdtk-0.1.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -154,8 +154,11 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+#.idea/
+
+# Custom
+src/pydevdtk/version.py
```

### Comparing `pydevdtk-0.1.0/LICENSE` & `pydevdtk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydevdtk-0.1.0/PKG-INFO` & `pydevdtk-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 Metadata-Version: 2.3
 Name: PyDevDTK
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python device development toolkit
 Project-URL: Homepage, https://github.com/BojanSof/pydevdtk
 Project-URL: Bug Tracker, https://github.com/BojanSof/pydevdtk/issues
 Author-email: Bojan Sofronievski <bojan.drago@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: matplotlib>=3.5.2
 Requires-Dist: numpy>=1.23.3
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 
-<p align="center">
-<picture>
-<img src="https://raw.githubusercontent.com/BojanSof/PyDevDTK/main/images/icon.png" height="256">
-</picture>
-</p>
+.. image:: https://raw.githubusercontent.com/BojanSof/PyDevDTK/main/images/icon.png
+    :align: center
+    :width: 256
+
+PyDevDTK
+========
 
 Python package that provides basic tools for device development, including:
-- Communication protocols:
-	- UART
-	- BLE
-- Real-time visualizations:
-	- Line plots
-	- Scatter plots
-	- Bar plots
-	- Image plots
-	- *Fully customized figure
+
+Communication protocols:
+
+    - UART
+    - BLE
+
+Real-time visualizations, which can be fully customized, or use one of the following plots:
+
+    - Line plots
+    - Scatter plots
+    - Bar plots
+    - Image plots
 
 More communication protocols and plots are added iteratively.
 
-## Installing
+Installing
+----------
+
+The repository includes GitHub actions which publish the package to PyPI and TestPyPI. To install the latest release package, run:
 
-The repository includes github actions which publish the package to PyPI and TestPyPI.
-To install the latest release package, run:
-```
-pip install pydevdtk
-```
+.. code-block:: shell
 
+    pip install pydevdtk
 
 To install the latest development package, which is published on TestPyPI, run:
-```
-pip install --index-url https://test.pypi.org/simple pydevdtk
-```
+
+.. code-block:: shell
+
+    pip install --index-url https://test.pypi.org/simple pydevdtk
 
 If you need to install the package locally for development, run the following command in the root of the repository:
-```
-pip install -e .
-```
 
-## Examples
+.. code-block:: shell
 
-Examples can be found under `examples` folder.
+    pip install -e .
 
-## Requirements
+Requirements
+------------
 
-Requirements can be found under `requirements` directory, which includes:
+Requirements can be found under ``requirements`` directory, which includes:
 
-- `default.txt` - base requirements for the package
-- `build.txt` - requirements for building the package
-- `doc.txt` - requirements for building the documentation (WIP)
-- `dev.txt` - requirements for developing the package, including linters and formaters
+- ``default.txt`` - base requirements for the package
+- ``build.txt`` - requirements for building the package
+- ``doc.txt`` - requirements for building the documentation (WIP)
+- ``dev.txt`` - requirements for developing the package, including linters and formatters
```

