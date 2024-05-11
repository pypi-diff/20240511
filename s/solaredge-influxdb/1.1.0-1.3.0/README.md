# Comparing `tmp/solaredge_influxdb-1.1.0.tar.gz` & `tmp/solaredge_influxdb-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solaredge_influxdb-1.1.0.tar", max compression
+gzip compressed data, was "solaredge_influxdb-1.3.0.tar", max compression
```

## Comparing `solaredge_influxdb-1.1.0.tar` & `solaredge_influxdb-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2024-02-19 21:13:23.129959 solaredge_influxdb-1.1.0/LICENSE
--rw-r--r--   0        0        0      133 2024-02-19 21:13:23.129959 solaredge_influxdb-1.1.0/README.md
--rw-r--r--   0        0        0      840 2024-02-19 21:13:23.133959 solaredge_influxdb-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       21 2024-02-19 21:13:23.133959 solaredge_influxdb-1.1.0/solaredge_influxdb/__init__.py
--rw-r--r--   0        0        0      757 2024-02-19 21:13:23.133959 solaredge_influxdb-1.1.0/solaredge_influxdb/__main__.py
--rw-r--r--   0        0        0     3315 2024-02-19 21:13:23.133959 solaredge_influxdb-1.1.0/solaredge_influxdb/app.py
--rw-r--r--   0        0        0       93 2024-02-19 21:13:23.133959 solaredge_influxdb-1.1.0/solaredge_influxdb/config.toml
--rw-r--r--   0        0        0       35 2024-02-19 21:13:23.133959 solaredge_influxdb-1.1.0/solaredge_influxdb/influxdb/__init__.py
--rw-r--r--   0        0        0     1151 2024-02-19 21:13:23.133959 solaredge_influxdb-1.1.0/solaredge_influxdb/influxdb/client.py
--rw-r--r--   0        0        0      137 2024-02-19 21:13:23.133959 solaredge_influxdb-1.1.0/solaredge_influxdb/solaredge/__init__.py
--rw-r--r--   0        0        0     1642 2024-02-19 21:13:23.133959 solaredge_influxdb-1.1.0/solaredge_influxdb/solaredge/client.py
--rw-r--r--   0        0        0    12236 2024-02-19 21:13:23.133959 solaredge_influxdb-1.1.0/solaredge_influxdb/solaredge/equipment.py
--rw-r--r--   0        0        0     2229 2024-02-19 21:13:23.133959 solaredge_influxdb-1.1.0/solaredge_influxdb/solaredge/meters.py
--rw-r--r--   0        0        0     3572 2024-02-19 21:13:23.133959 solaredge_influxdb-1.1.0/solaredge_influxdb/solaredge/models.py
--rw-r--r--   0        0        0      545 2024-02-19 21:13:23.133959 solaredge_influxdb-1.1.0/solaredge_influxdb/solaredge/site.py
--rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 solaredge_influxdb-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/LICENSE
+-rw-r--r--   0        0        0      133 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/README.md
+-rw-r--r--   0        0        0      857 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/solaredge_influxdb/__init__.py
+-rw-r--r--   0        0        0      757 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/solaredge_influxdb/__main__.py
+-rw-r--r--   0        0        0     3616 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/solaredge_influxdb/app.py
+-rw-r--r--   0        0        0       93 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/solaredge_influxdb/config.toml
+-rw-r--r--   0        0        0       35 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/solaredge_influxdb/influxdb/__init__.py
+-rw-r--r--   0        0        0     1151 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/solaredge_influxdb/influxdb/client.py
+-rw-r--r--   0        0        0      137 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/solaredge_influxdb/solaredge/__init__.py
+-rw-r--r--   0        0        0     1642 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/solaredge_influxdb/solaredge/client.py
+-rw-r--r--   0        0        0    12236 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/solaredge_influxdb/solaredge/equipment.py
+-rw-r--r--   0        0        0     2229 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/solaredge_influxdb/solaredge/meters.py
+-rw-r--r--   0        0        0     3562 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/solaredge_influxdb/solaredge/models.py
+-rw-r--r--   0        0        0      545 2024-05-11 09:24:43.758227 solaredge_influxdb-1.3.0/solaredge_influxdb/solaredge/site.py
+-rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 solaredge_influxdb-1.3.0/PKG-INFO
```

### Comparing `solaredge_influxdb-1.1.0/LICENSE` & `solaredge_influxdb-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solaredge_influxdb-1.1.0/pyproject.toml` & `solaredge_influxdb-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "solaredge-influxdb"
-version = "1.1.0"
+version = "1.3.0"
 description = "Ability to get data from the solar edge api into a influxdb"
 authors = ["Yorick Fredrix <yorick.fredrix@outlook.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
 influxdb-client = "^1.40.0"
 pydantic = "^2.6.1"
 loguru = "^0.7.2"
 suntime = "^1.2.5"
+pytz = "^2024.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 pytest = "^8.0.1"
 flake8 = "^7.0.0"
 
 [tool.semantic_release]
```

### Comparing `solaredge_influxdb-1.1.0/solaredge_influxdb/__main__.py` & `solaredge_influxdb-1.3.0/solaredge_influxdb/__main__.py`

 * *Files identical despite different names*

### Comparing `solaredge_influxdb-1.1.0/solaredge_influxdb/app.py` & `solaredge_influxdb-1.3.0/solaredge_influxdb/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 from suntime import Sun, SunTimeException
 from datetime import datetime, timedelta, timezone
+import pytz
 from loguru import logger
 
 from solaredge_influxdb.solaredge import Equipment, Meter
 from solaredge_influxdb.influxdb import InfluxDBClient
 
 
 def app(
     config_path: str = "./solaredge_influxdb/config.toml",
     latitude: float = os.getenv("LATITUDE", 52.3676),
     longitude: float = os.getenv("LONGITUDE", 4.9041),
     api_key: str = os.getenv("API_KEY"),
-    additional_time_window: int = 30,
+    additional_time_window: int = 60,
+    timezone_str: str = "Europe/Amsterdam",
 ):
     sun = Sun(latitude, longitude)
     current_time = datetime.now(timezone.utc)
     logger.debug(f"Current time: {current_time}")
     try:
         sunrise = sun.get_sunrise_time()
         sunset = sun.get_sunset_time()
@@ -24,23 +26,25 @@
 
     except SunTimeException:
         logger.error("Failed to retrieve sunrise/sunset times")
         raise Exception(
             "Application requires sunset and sunrise times to prevent unnecessary API calls"
         )
     InfluxClient = InfluxDBClient(config_path)
+    _timezone = pytz.timezone(timezone_str)
 
     if (
         sunrise - timedelta(minutes=additional_time_window)
         < current_time
         < sunset + timedelta(minutes=additional_time_window)
     ):
+        logger.debug("The Sun is shining bright, let's collect some data!")
         EquipmentClient = Equipment(api_key)
         MeterClient = Meter(api_key)
-
+        current_time = current_time.astimezone(_timezone)
         for inverter in EquipmentClient.inverters:
             tech_data = EquipmentClient.get_technical_data(
                 inverter.serialNumber,
                 current_time - timedelta(minutes=15),
                 current_time,
             )
             if tech_data is None:
@@ -50,32 +54,33 @@
             for telemetry in tech_data.telemetries:
                 tags = [
                     ("serial_number", inverter.serialNumber),
                     ("model", inverter.model),
                     ("operation_mode", telemetry.operationMode),
                     ("inverter_mode", telemetry.inverterMode),
                 ]
+                telemetry_date = _timezone.localize(telemetry.date)
                 energy_point = InfluxClient.convert_to_point(
-                    telemetry.date,
+                    telemetry_date,
                     "solar",
                     [
                         ("total_energy", telemetry.totalEnergy / 1000),
                     ],
                     tags,
                 )
                 power_point = InfluxClient.convert_to_point(
-                    telemetry.date,
+                    telemetry_date,
                     "solar",
                     [
                         ("ac_power", telemetry.totalActivePower / 1000),
                     ],
                     tags,
                 )
                 voltage_point = InfluxClient.convert_to_point(
-                    telemetry.date,
+                    telemetry_date,
                     "solar",
                     [
                         ("dc_voltage", telemetry.dcVoltage),
                         ("voltage_l1_to_2", telemetry.vL1To2),
                         ("voltage_l2_to_3", telemetry.vL2To3),
                         ("voltage_l3_to_1", telemetry.vL3To1),
                     ],
```

### Comparing `solaredge_influxdb-1.1.0/solaredge_influxdb/influxdb/client.py` & `solaredge_influxdb-1.3.0/solaredge_influxdb/influxdb/client.py`

 * *Files identical despite different names*

### Comparing `solaredge_influxdb-1.1.0/solaredge_influxdb/solaredge/client.py` & `solaredge_influxdb-1.3.0/solaredge_influxdb/solaredge/client.py`

 * *Files identical despite different names*

### Comparing `solaredge_influxdb-1.1.0/solaredge_influxdb/solaredge/equipment.py` & `solaredge_influxdb-1.3.0/solaredge_influxdb/solaredge/equipment.py`

 * *Files identical despite different names*

### Comparing `solaredge_influxdb-1.1.0/solaredge_influxdb/solaredge/meters.py` & `solaredge_influxdb-1.3.0/solaredge_influxdb/solaredge/meters.py`

 * *Files identical despite different names*

### Comparing `solaredge_influxdb-1.1.0/solaredge_influxdb/solaredge/models.py` & `solaredge_influxdb-1.3.0/solaredge_influxdb/solaredge/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from datetime import datetime
 from typing import List, Optional
-from pydantic import BaseModel
+from pydantic import BaseModel, NaiveDatetime
 
 
 class TelemetryData(BaseModel):
-    date: datetime
+    date: NaiveDatetime
     totalActivePower: Optional[float]
     dcVoltage: Optional[float]
     groundFaultResistance: Optional[float] = None
     powerLimit: float
     totalEnergy: float
     temperature: Optional[float] = None
     inverterMode: str
```

### Comparing `solaredge_influxdb-1.1.0/solaredge_influxdb/solaredge/site.py` & `solaredge_influxdb-1.3.0/solaredge_influxdb/solaredge/site.py`

 * *Files identical despite different names*

