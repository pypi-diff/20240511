# Comparing `tmp/smartplug_energy_controller-0.0.3.tar.gz` & `tmp/smartplug_energy_controller-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartplug_energy_controller-0.0.3.tar", max compression
+gzip compressed data, was "smartplug_energy_controller-0.0.4.tar", max compression
```

## Comparing `smartplug_energy_controller-0.0.3.tar` & `smartplug_energy_controller-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2024-05-09 18:33:47.927961 smartplug_energy_controller-0.0.3/LICENSE
--rw-r--r--   0        0        0     4621 2024-05-09 18:33:47.927961 smartplug_energy_controller-0.0.3/README.md
--rw-r--r--   0        0        0      684 2024-05-09 18:33:47.927961 smartplug_energy_controller-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      511 2024-05-09 18:33:47.927961 smartplug_energy_controller-0.0.3/smartplug_energy_controller/__init__.py
--rw-r--r--   0        0        0     2059 2024-05-09 18:33:47.927961 smartplug_energy_controller-0.0.3/smartplug_energy_controller/app.py
--rw-r--r--   0        0        0     4039 2024-05-09 18:33:47.927961 smartplug_energy_controller-0.0.3/smartplug_energy_controller/plug_controller.py
--rw-r--r--   0        0        0     5431 1970-01-01 00:00:00.000000 smartplug_energy_controller-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-11 19:29:08.641430 smartplug_energy_controller-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4710 2024-05-11 19:29:08.641430 smartplug_energy_controller-0.0.4/README.md
+-rw-r--r--   0        0        0      684 2024-05-11 19:29:08.641430 smartplug_energy_controller-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      511 2024-05-11 19:29:08.641430 smartplug_energy_controller-0.0.4/smartplug_energy_controller/__init__.py
+-rw-r--r--   0        0        0     2462 2024-05-11 19:29:08.641430 smartplug_energy_controller-0.0.4/smartplug_energy_controller/app.py
+-rw-r--r--   0        0        0     4378 2024-05-11 19:29:08.641430 smartplug_energy_controller-0.0.4/smartplug_energy_controller/plug_controller.py
+-rw-r--r--   0        0        0     5520 1970-01-01 00:00:00.000000 smartplug_energy_controller-0.0.4/PKG-INFO
```

### Comparing `smartplug_energy_controller-0.0.3/LICENSE` & `smartplug_energy_controller-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smartplug_energy_controller-0.0.3/README.md` & `smartplug_energy_controller-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 TAPO_PLUG_IP='192.168.x.x'
 TAPO_CONTROL_USER='your_user'
 TAPO_CONTROL_PASSWD='your_passwd'
 
 # Following values can be considered as parameters, but have to be provided as env variables 
 # (see: https://fastapi.tiangolo.com/advanced/settings/#create-the-settings-object)
 EVAL_COUNT=10
-EXPECTED_CONSUMPTION=100
+EXPECTED_CONSUMPTION=200
+CONSUMER_EFFICIENCY=0.5
 LOG_FILE='path_to_file'
 LOG_LEVEL=20
 ```
 
 ## Autostart after reboot and on failure ##
 Create a systemd service by opening the file */etc/systemd/system/smartplug_energy_controller.service* and copy paste the following contents. Replace User/Group/ExecStart accordingly. 
 ```bash
@@ -55,18 +56,19 @@
 Type=simple
 User=ubuntu
 Group=ubuntu
 UMask=002
 Restart=on-failure
 RestartSec=5s
 Environment="EVAL_COUNT=10"
-Environment="EXPECTED_CONSUMPTION=100"
+Environment="EXPECTED_CONSUMPTION=200"
+Environment="CONSUMER_EFFICIENCY=0.5"
 Environment="LOG_FILE=/home/ubuntu/plug_controller.log"
 Environment="LOG_LEVEL=20"
-ExecStart=/usr/bin/bash -lc "source /home/ubuntu/smart_meter_py_env/bin/activate && uvicorn smartplug_energy_controller.app:app > /dev/null"
+ExecStart=/usr/bin/bash -lc "source /home/ubuntu/smart_meter_py_env/bin/activate && uvicorn --host 0.0.0.0 --port 8000 smartplug_energy_controller.app:app > /dev/null"
 
 [Install]
 WantedBy=multi-user.target
 ```
 
 Now execute the following commands to enable autostart:
 ```bash
```

### Comparing `smartplug_energy_controller-0.0.3/pyproject.toml` & `smartplug_energy_controller-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smartplug_energy_controller"
-version = "0.0.3"
+version = "0.0.4"
 description = "Turning Tapo smartplug on/off depending on current electricity consumption"
 authors = ["Heiko Bauer <heiko_bauer@icloud.com>"]
 repository = "https://github.com/die-bauerei/smartplug-energy-controller"
 readme = "README.md"
 packages = [
     {include = "smartplug_energy_controller"},
 ]
```

### Comparing `smartplug_energy_controller-0.0.3/smartplug_energy_controller/plug_controller.py` & `smartplug_energy_controller-0.0.4/smartplug_energy_controller/plug_controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 
 from plugp100.common.credentials import AuthCredential
 from plugp100.new.device_factory import connect, DeviceConnectConfiguration
 from plugp100.new.tapoplug import TapoPlug
 
 # TODO: use a redis timeseries db: https://redis.io/docs/latest/develop/data-types/timeseries/
 def _manage_rolling_list(list : List[Any], max_value_count : int, new_end_value : Any) -> List[Any]:
-    if len(list) < max_value_count:
+    if len(list) == 0:
+        return [new_end_value]*max_value_count
+    elif len(list) < max_value_count:
         return list+[new_end_value]
     else:
         return list[1:]+[new_end_value]
 
 class PlugController(ABC):
-    def __init__(self, logger : Logger, watt_consumption_eval_count : int, expected_watt_consumption : float) -> None:
+    def __init__(self, logger : Logger, watt_consumption_eval_count : int, expected_watt_consumption : float, consumer_efficiency : float) -> None:
         self._logger=logger
         self._watt_consumption_eval_count=watt_consumption_eval_count
         assert expected_watt_consumption >= 1
+        self._consumer_efficiency=consumer_efficiency
+        assert self._consumer_efficiency > 0 and self._consumer_efficiency < 1
         self._expected_watt_consumption=expected_watt_consumption
         self._watt_consumption_values : List[float] = []
 
     @abstractmethod
     def reset(self) -> None:
         pass
 
@@ -46,30 +50,30 @@
         try:
             self._watt_consumption_values=_manage_rolling_list(self._watt_consumption_values, 
                                                             self._watt_consumption_eval_count, 
                                                             value)
 
             await self.update()
             if len(self._watt_consumption_values) == self._watt_consumption_eval_count:
-                consumption_threshold=self._expected_watt_consumption if self.is_on() else 1
-                values_less_threshold=[value for value in self._watt_consumption_values if value < consumption_threshold]
+                obtained_from_provider_threshold=self._expected_watt_consumption*self._consumer_efficiency if await self.is_on() else 1
+                values_less_threshold=[value for value in self._watt_consumption_values if value < obtained_from_provider_threshold]
                 if len(values_less_threshold) > self._watt_consumption_eval_count/2:
                     await self.turn_on()
                 else:
                     await self.turn_off()
         except Exception as e:
             # Just log as warning since the plug could just be unconnected 
             self._logger.warning("Caught Exception while adding watt consumption. About to reset controller now.")
             self.reset()
 
 class TapoPlugController(PlugController):
 
-    def __init__(self, logger : Logger, watt_consumption_eval_count : int, expected_watt_consumption : float,
+    def __init__(self, logger : Logger, watt_consumption_eval_count : int, expected_watt_consumption : float,  consumer_efficiency : float,
                 tapo_user : str, tapo_passwd : str, tapo_plug_ip : str) -> None:
-        super().__init__(logger, watt_consumption_eval_count, expected_watt_consumption)
+        super().__init__(logger, watt_consumption_eval_count, expected_watt_consumption, consumer_efficiency)
         self._tapo_user=tapo_user
         self._tapo_passwd=tapo_passwd
         self._tapo_plug_ip=tapo_plug_ip
         assert self._tapo_user != ''
         assert self._tapo_passwd != ''
         assert self._tapo_plug_ip != ''
         self._plug : Optional[TapoPlug] = None
```

### Comparing `smartplug_energy_controller-0.0.3/PKG-INFO` & `smartplug_energy_controller-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartplug_energy_controller
-Version: 0.0.3
+Version: 0.0.4
 Summary: Turning Tapo smartplug on/off depending on current electricity consumption
 Home-page: https://github.com/die-bauerei/smartplug-energy-controller
 Author: Heiko Bauer
 Author-email: heiko_bauer@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -53,15 +53,16 @@
 TAPO_PLUG_IP='192.168.x.x'
 TAPO_CONTROL_USER='your_user'
 TAPO_CONTROL_PASSWD='your_passwd'
 
 # Following values can be considered as parameters, but have to be provided as env variables 
 # (see: https://fastapi.tiangolo.com/advanced/settings/#create-the-settings-object)
 EVAL_COUNT=10
-EXPECTED_CONSUMPTION=100
+EXPECTED_CONSUMPTION=200
+CONSUMER_EFFICIENCY=0.5
 LOG_FILE='path_to_file'
 LOG_LEVEL=20
 ```
 
 ## Autostart after reboot and on failure ##
 Create a systemd service by opening the file */etc/systemd/system/smartplug_energy_controller.service* and copy paste the following contents. Replace User/Group/ExecStart accordingly. 
 ```bash
@@ -74,18 +75,19 @@
 Type=simple
 User=ubuntu
 Group=ubuntu
 UMask=002
 Restart=on-failure
 RestartSec=5s
 Environment="EVAL_COUNT=10"
-Environment="EXPECTED_CONSUMPTION=100"
+Environment="EXPECTED_CONSUMPTION=200"
+Environment="CONSUMER_EFFICIENCY=0.5"
 Environment="LOG_FILE=/home/ubuntu/plug_controller.log"
 Environment="LOG_LEVEL=20"
-ExecStart=/usr/bin/bash -lc "source /home/ubuntu/smart_meter_py_env/bin/activate && uvicorn smartplug_energy_controller.app:app > /dev/null"
+ExecStart=/usr/bin/bash -lc "source /home/ubuntu/smart_meter_py_env/bin/activate && uvicorn --host 0.0.0.0 --port 8000 smartplug_energy_controller.app:app > /dev/null"
 
 [Install]
 WantedBy=multi-user.target
 ```
 
 Now execute the following commands to enable autostart:
 ```bash
```

