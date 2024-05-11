# Comparing `tmp/solarlog_cli-0.1.1.tar.gz` & `tmp/solarlog_cli-0.1.2.tar.gz`

## Comparing `solarlog_cli-0.1.1.tar` & `solarlog_cli-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/requirements.txt
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/.github/workflows/ruff.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/src/solarlog_cli/__init__.py
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/src/solarlog_cli/solarlog_client.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/src/solarlog_cli/solarlog_connector.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/src/solarlog_cli/solarlog_exceptions.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/src/solarlog_cli/utils.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/LICENSE
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/README.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 solarlog_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/src/solarlog_cli/__init__.py
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/src/solarlog_cli/solarlog_client.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/src/solarlog_cli/solarlog_connector.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/src/solarlog_cli/solarlog_exceptions.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/src/solarlog_cli/utils.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/LICENSE
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/README.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 solarlog_cli-0.1.2/PKG-INFO
```

### Comparing `solarlog_cli-0.1.1/.github/workflows/pylint.yml` & `solarlog_cli-0.1.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.1/.github/workflows/python-publish.yml` & `solarlog_cli-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.1/.github/workflows/ruff.yml` & `solarlog_cli-0.1.2/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.1/src/solarlog_cli/solarlog_client.py` & `solarlog_cli-0.1.2/src/solarlog_cli/solarlog_client.py`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.1/src/solarlog_cli/solarlog_connector.py` & `solarlog_cli-0.1.2/src/solarlog_cli/solarlog_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
             )
 
         data["last_updated"] = data["last_updated"].astimezone(self.timezone)
 
         # print(f"basic data updated: {data}")
         if self.extended_data:
             data |= await self.client.get_energy()
-            data |= {"devices": await self.update_inverter_data()}
+            if self._device_enabled is not {}:
+                data |= {"devices": await self.update_inverter_data()}
             # print(f"extended data updated: {data}")
 
         #calculated values (for downward compatibility)
         if data.get("power_dc") != 0:
             data |= {"efficiency": data.get("power_ac") / data.get("power_dc")}
         if data.get("power_ac") != 0:
             data |= {"usage": data.get("consumption_ac") / data.get("power_ac")}
@@ -82,15 +83,15 @@
         """Update device specific data."""
         data: dict[int, dict[str, Any]] = {}
         # print(self._device_enabled)
         raw_data = await self.client.get_power_per_inverter()
         # print(f"power: {raw_data}")
         for key, value in raw_data.items():
             key = int(key)
-            if self._device_enabled[key]:
+            if self._device_enabled.get(key, False):
                 data |= {key: {"current_power": float(value)}}
 
         raw_data = await self.client.get_energy_per_inverter()
         # print(f"energy: {raw_data}")
         for key, value in raw_data.items():
             # print(f"key: {key}, value: {value}, enabled: {self._device_enabled[key]}")
             if self._device_enabled[key]:
```

### Comparing `solarlog_cli-0.1.1/src/solarlog_cli/utils.py` & `solarlog_cli-0.1.2/src/solarlog_cli/utils.py`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.1/LICENSE` & `solarlog_cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `solarlog_cli-0.1.1/pyproject.toml` & `solarlog_cli-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "solarlog_cli"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="dontinelli", email="73341522+dontinelli@users.noreply.github.com" },
 ]
 description = "Python library to access the Solar-Log"
 readme = "README.md"
 requires-python = ">=3.12"
 dependencies = [
```

### Comparing `solarlog_cli-0.1.1/PKG-INFO` & `solarlog_cli-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: solarlog_cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library to access the Solar-Log
 Project-URL: Repository, https://github.com/dontinelli/solarlog_cli.git
 Project-URL: Issues, https://github.com/dontinelli/solarlog_cli/issues
 Project-URL: Changelog, https://github.com/dontinelli/solarlog_cli/blob/master/CHANGELOG.md
 Project-URL: Solar-Log homepage, https://www.solar-log.com/
 Project-URL: API Documentation (inofficial), https://github.com/iobroker-community-adapters/ioBroker.solarlog/blob/master/docs/solarlog_dataobjects.md
 Author-email: dontinelli <73341522+dontinelli@users.noreply.github.com>
```

