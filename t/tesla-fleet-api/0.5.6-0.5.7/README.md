# Comparing `tmp/tesla_fleet_api-0.5.6.tar.gz` & `tmp/tesla_fleet_api-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesla_fleet_api-0.5.6.tar", last modified: Sat Mar 30 11:29:45 2024, max compression
+gzip compressed data, was "tesla_fleet_api-0.5.7.tar", last modified: Sat May 11 21:35:01 2024, max compression
```

## Comparing `tesla_fleet_api-0.5.6.tar` & `tesla_fleet_api-0.5.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 11:29:45.484852 tesla_fleet_api-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-03-30 11:29:45.484852 tesla_fleet_api-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 11:29:45.484852 tesla_fleet_api-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 11:29:45.484852 tesla_fleet_api-0.5.6/tesla_fleet_api/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/charging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/energyspecific.py
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/partner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/teslafleetapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/teslafleetoauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/teslemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/tessie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    32696 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (127)    21361 2024-03-30 11:29:42.000000 tesla_fleet_api-0.5.6/tesla_fleet_api/vehiclespecific.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 11:29:45.484852 tesla_fleet_api-0.5.6/tesla_fleet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-03-30 11:29:45.000000 tesla_fleet_api-0.5.6/tesla_fleet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-30 11:29:45.000000 tesla_fleet_api-0.5.6/tesla_fleet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 11:29:45.000000 tesla_fleet_api-0.5.6/tesla_fleet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-30 11:29:45.000000 tesla_fleet_api-0.5.6/tesla_fleet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-30 11:29:45.000000 tesla_fleet_api-0.5.6/tesla_fleet_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:35:01.992143 tesla_fleet_api-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-11 21:35:01.992143 tesla_fleet_api-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 21:35:01.992143 tesla_fleet_api-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:35:01.992143 tesla_fleet_api-0.5.7/tesla_fleet_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/charging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/energyspecific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/partner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/teslafleetapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/teslafleetoauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/teslemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/tessie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32835 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21492 2024-05-11 21:34:58.000000 tesla_fleet_api-0.5.7/tesla_fleet_api/vehiclespecific.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:35:01.992143 tesla_fleet_api-0.5.7/tesla_fleet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-11 21:35:01.000000 tesla_fleet_api-0.5.7/tesla_fleet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-11 21:35:01.000000 tesla_fleet_api-0.5.7/tesla_fleet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 21:35:01.000000 tesla_fleet_api-0.5.7/tesla_fleet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-11 21:35:01.000000 tesla_fleet_api-0.5.7/tesla_fleet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 21:35:01.000000 tesla_fleet_api-0.5.7/tesla_fleet_api.egg-info/top_level.txt
```

### Comparing `tesla_fleet_api-0.5.6/LICENSE` & `tesla_fleet_api-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.6/PKG-INFO` & `tesla_fleet_api-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesla_fleet_api
-Version: 0.5.6
+Version: 0.5.7
 Summary: Tesla Fleet API library for Python
 Home-page: https://github.com/Teslemetry/tesla_fleet_api
 Author: Brett Adams
 Author-email: admin@teslemetry.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `tesla_fleet_api-0.5.6/README.md` & `tesla_fleet_api-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.6/setup.py` & `tesla_fleet_api-0.5.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tesla_fleet_api",
-    version="0.5.6",
+    version="0.5.7",
     author="Brett Adams",
     author_email="admin@teslemetry.com",
     description="Tesla Fleet API library for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Teslemetry/tesla_fleet_api",
     packages=setuptools.find_packages(),
```

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api/charging.py` & `tesla_fleet_api-0.5.7/tesla_fleet_api/charging.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api/const.py` & `tesla_fleet_api-0.5.7/tesla_fleet_api/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Tesla Fleet API constants."""
 
 from enum import Enum
 import logging
 
-VERSION = "0.5.6"
+VERSION = "0.5.7"
 LOGGER = logging.getLogger(__package__)
 SERVERS = {
     "na": "https://fleet-api.prd.na.vn.cloud.tesla.com",
     "eu": "https://fleet-api.prd.eu.vn.cloud.tesla.com",
     "cn": "https://fleet-api.prd.cn.vn.cloud.tesla.cn",
 }
```

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api/energy.py` & `tesla_fleet_api-0.5.7/tesla_fleet_api/energy.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             },
         )
 
     async def grid_import_export(
         self,
         energy_site_id: int,
         disallow_charge_from_grid_with_solar_installed: bool | None = None,
-        customer_preferred_export_rule: EnergyExportMode|str | None = None,
+        customer_preferred_export_rule: EnergyExportMode | str | None = None,
     ) -> dict[str, Any]:
         """Allow/disallow charging from the grid and exporting energy to the grid."""
         return await self._request(
             Method.POST,
             f"api/1/energy_sites/{energy_site_id}/grid_import_export",
             json={
                 "disallow_charge_from_grid_with_solar_installed": disallow_charge_from_grid_with_solar_installed,
```

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api/energyspecific.py` & `tesla_fleet_api-0.5.7/tesla_fleet_api/energyspecific.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api/exceptions.py` & `tesla_fleet_api-0.5.7/tesla_fleet_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 
 
 class Forbidden(TeslaFleetError):
     """Access to this resource is not authorized, developers should check required Scope."""
 
     message = "Access to this resource is not authorized, developers should check required Scope."
     status = 403
+    key = "Unauthorized missing scopes"
 
 
 class UnsupportedVehicle(TeslaFleetError):
     """The vehicle is unsupported."""
 
     message = "The vehicle is unsupported."
     status = 403
```

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api/partner.py` & `tesla_fleet_api-0.5.7/tesla_fleet_api/partner.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api/teslafleetapi.py` & `tesla_fleet_api-0.5.7/tesla_fleet_api/teslafleetapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,40 +11,41 @@
 from .vehicle import Vehicle
 
 
 # Based on https://developer.tesla.com/docs/fleet-api
 class TeslaFleetApi:
     """Class describing the Tesla Fleet API."""
 
-    server: str
+    server: str | None = None
     session: aiohttp.ClientSession
     headers: dict[str, str]
     raise_for_status: bool
 
     def __init__(
         self,
         session: aiohttp.ClientSession,
-        access_token: str,
+        access_token: str | None = None,
         region: str | None = None,
         server: str | None = None,
         raise_for_status: bool = True,
         charging_scope: bool = True,
         energy_scope: bool = True,
         partner_scope: bool = True,
         user_scope: bool = True,
         vehicle_scope: bool = True,
     ):
         """Initialize the Tesla Fleet API."""
 
         self.session = session
         self.access_token = access_token
 
-        if region and not server and region not in SERVERS:
-            raise ValueError(f"Region must be one of {', '.join(SERVERS.keys())}")
-        self.server = server or SERVERS.get(region)
+        if region is not None:
+            if not server and region not in SERVERS:
+                raise ValueError(f"Region must be one of {', '.join(SERVERS.keys())}")
+            self.server = server or SERVERS.get(region)
         self.raise_for_status = raise_for_status
 
         LOGGER.debug("Using server %s", self.server)
 
         if charging_scope:
             self.charging = Charging(self)
         if energy_scope:
@@ -57,30 +58,31 @@
             self.vehicle = Vehicle(self)
 
     async def find_server(self) -> str:
         """Find the server URL for the Tesla Fleet API."""
         for server in SERVERS.values():
             self.server = server
             try:
-                response = await (self.user.region()).get("response")
+                region_response = await self.user.region()
+                response = region_response.get("response")
                 if response:
                     self.server = response["fleet_api_base_url"]
                     LOGGER.debug("Using server %s", self.server)
                     return response["region"]
             except InvalidRegion:
                 continue
         raise LibraryError("Could not find a valid Tesla API server.")
 
     async def _request(
         self,
         method: Method,
         path: str,
-        params: dict[str:Any] | None = None,
-        json: dict[str:Any] | None = None,
-    ):
+        params: dict[str, Any] | None = None,
+        json: dict[str, Any] | None = None,
+    ) -> dict[str, Any] | str:
         """Send a request to the Tesla Fleet API."""
 
         if not self.server:
             raise ValueError("Server was not set at init. Call find_server() first.")
 
         if method == Method.GET and json is not None:
             raise ValueError("GET requests cannot have a body.")
@@ -121,15 +123,15 @@
                 LOGGER.debug("Response JSON: %s", data)
                 return data
 
             data = await resp.text()
             LOGGER.debug("Response Text: %s", data)
             return data
 
-    async def status(self):
+    async def status(self) -> str:
         """This endpoint returns the string "ok" if the API is operating normally. No HTTP headers are required."""
         if not self.server:
             raise ValueError("Server was not set at init. Call find_server() first.")
         async with self.session.get(f"{self.server}/status") as resp:
             return await resp.text()
 
     async def products(self) -> dict[str, Any]:
```

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api/teslafleetoauth.py` & `tesla_fleet_api-0.5.7/tesla_fleet_api/teslafleetoauth.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,17 @@
 
     def get_login_url(
         self, redirect_uri: str, scopes: list[Scope], state: str = "login"
     ) -> str:
         """Get the login URL."""
         return f"https://auth.tesla.com/oauth2/v3/authorize?response_type=code&client_id={self.client_id}&redirect_uri={redirect_uri}&scope={' '.join(scopes)}&state={state}"
 
-    async def get_refresh_token(self, client_secret: str, code: str, redirect_uri: str):
+    async def get_refresh_token(
+        self, client_secret: str, code: str, redirect_uri: str
+    ) -> None:
         """Get the refresh token."""
         async with self.session.post(
             "https://auth.tesla.com/oauth2/v3/token",
             data={
                 "grant_type": "authorization_code",
                 "client_id": self.client_id,
                 "client_secret": client_secret,
@@ -59,21 +61,21 @@
                 data = await resp.json()
                 self.refresh_token = data["refresh_token"]
                 self.access_token = data["access_token"]
                 self.expires = int(time.time()) + data["expires_in"]
                 region = code.split("_")[0].lower()
                 self.server = SERVERS.get(region)
 
-    async def check_access_token(self) -> str | None:
+    async def check_access_token(self) -> dict[str, Any] | None:
         """Get the access token."""
         if self.access_token and self.expires > time.time():
-            return
+            return None
         return await self.refresh_access_token()
 
-    async def refresh_access_token(self) -> str:
+    async def refresh_access_token(self) -> dict[str, Any]:
         """Refresh the access token."""
         if not self.refresh_token:
             raise ValueError("Refresh token is missing")
         async with self.session.post(
             "https://auth.tesla.com/oauth2/v3/token",
             data={
                 "grant_type": "refresh_token",
@@ -89,13 +91,13 @@
                 return {"refresh_token": self.refresh_token, "expires": self.expires}
             raise ValueError(data)
 
     async def _request(
         self,
         method: Method,
         path: str,
-        params: dict | None = None,
-        data: dict | None = None,
-    ):
+        params: dict[str, Any] | None = None,
+        data: dict[str, Any] | None = None,
+    ) -> str | dict[str, Any]:
         """Send a request to the Tesla Fleet API."""
         await self.check_access_token()
         return await super()._request(method, path, params, data)
```

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api/teslemetry.py` & `tesla_fleet_api-0.5.7/tesla_fleet_api/teslemetry.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,21 +48,22 @@
         )
         if update_region and "region" in resp:
             self.region = resp["region"].lower()
             self.server = f"https://{self.region}.teslemetry.com"
             LOGGER.debug("Using server %s", self.server)
         return resp
 
-    async def find_server(self):
+    # TODO: type this properly, it probably should return something
+    async def find_server(self) -> None:
         """Find the server URL for the Tesla Fleet API."""
         await self.metadata(True)
 
     async def _request(
         self,
         method: Method,
         path: str,
-        params: dict[str:Any] | None = None,
-        json: dict[str:Any] | None = None,
-    ):
+        params: dict[str, Any] | None = None,
+        json: dict[str, Any] | None = None,
+    ) -> str | dict[str, Any]:
         """Send a request to the Teslemetry API."""
         async with rate_limit:
             return await super()._request(method, path, params, json)
```

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api/tessie.py` & `tesla_fleet_api-0.5.7/tesla_fleet_api/tessie.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import aiohttp
 from typing import Any
 from .teslafleetapi import TeslaFleetApi
 from .const import Method
-from .vehiclespecific import VehicleSpecific
 
 
 class Tessie(TeslaFleetApi):
     def __init__(
         self,
         session: aiohttp.ClientSession,
         access_token: str,
@@ -19,15 +18,15 @@
             server="https://api.tessie.com",
             raise_for_status=raise_for_status,
             partner_scope=False,
             user_scope=False,
             energy_scope=False,
         )
 
-    async def find_server(self):
+    async def find_server(self) -> str:
         """Find the server URL for the Tesla Fleet API."""
         raise NotImplementedError("Do not use this function for Tessie.")
 
     async def vehicles(self, only_active: bool = False) -> Any:
         """Get vehicles."""
         return await self._request(
             Method.GET, "vehicles", params={"only_active": only_active}
```

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api/user.py` & `tesla_fleet_api-0.5.7/tesla_fleet_api/user.py`

 * *Files identical despite different names*

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api/vehicle.py` & `tesla_fleet_api-0.5.7/tesla_fleet_api/vehicle.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     def __init__(self, parent):
         self._parent = parent
         self._request = parent._request
 
     def specific(self, vehicle_tag: str | int) -> VehicleSpecific:
         """Creates a class for each vehicle."""
         return VehicleSpecific(self, vehicle_tag)
+    
+    def pre2021(self, vin: str) -> bool:
+        """Checks if a vehicle is pre-2021."""
+        return vin[9] <= "L"
 
     async def actuate_trunk(
         self, vehicle_tag: str | int, which_trunk: Trunk | str
     ) -> dict[str, Any]:
         """Controls the front or rear trunk."""
         return await self._request(
             Method.POST,
@@ -563,15 +567,15 @@
         self,
         vehicle_tag: str | int,
         token: str | None = None,
         lat: float | None = None,
         lon: float | None = None,
     ) -> dict[str, Any]:
         """Turns on HomeLink (used to open and close garage doors)."""
-        data = {}
+        data: dict[str, str | float] = {}
         if token:
             data["token"] = token
         if lat and lon:
             data["lat"] = lat
             data["lon"] = lon
         return await self._request(
             Method.POST,
@@ -738,20 +742,19 @@
 
     async def vehicle_data(
         self,
         vehicle_tag: str | int,
         endpoints: List[VehicleDataEndpoint] | List[str] | None = None,
     ) -> dict[str, Any]:
         """Makes a live call to the vehicle. This may return cached data if the vehicle is offline. For vehicles running firmware versions 2023.38+, location_data is required to fetch vehicle location. This will result in a location sharing icon to show on the vehicle UI."""
-        if isinstance(endpoints, list):
-            endpoints = ";".join(endpoints)
+        endpoint_payload = ";".join(endpoints) if endpoints else None
         return await self._request(
             Method.GET,
             f"api/1/vehicles/{vehicle_tag}/vehicle_data",
-            {"endpoints": endpoints},
+            {"endpoints": endpoint_payload},
         )
 
     async def vehicle_subscriptions(
         self, device_token: str, device_type: DeviceType | str
     ) -> dict[str, Any]:
         """Returns the list of vehicles for which this mobile device currently subscribes to push notifications."""
         return await self._request(
```

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api/vehiclespecific.py` & `tesla_fleet_api-0.5.7/tesla_fleet_api/vehiclespecific.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,22 @@
     DeviceType,
 )
 
 
 class VehicleSpecific:
     """Class describing the Tesla Fleet API vehicle endpoints and commands for a specific vehicle."""
 
-    def __init__(self, parent, vin: str | None = None):
+    def __init__(self, parent, vin: str | int | None = None):
         self._parent = parent
         self.vin = vin
 
+    def pre2021(self) -> bool:
+        """Checks if a vehicle is pre-2021."""
+        return self._parent.pre2021(self.vin)
+
     async def actuate_trunk(self, which_trunk: Trunk | str) -> dict[str, Any]:
         """Controls the front or rear trunk."""
         return await self._parent.actuate_trunk(self.vin, which_trunk)
 
     async def adjust_volume(self, volume: float) -> dict[str, Any]:
         """Adjusts vehicle media playback volume."""
         return await self._parent.adjust_volume(self.vin, volume)
```

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api.egg-info/PKG-INFO` & `tesla_fleet_api-0.5.7/tesla_fleet_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesla_fleet_api
-Version: 0.5.6
+Version: 0.5.7
 Summary: Tesla Fleet API library for Python
 Home-page: https://github.com/Teslemetry/tesla_fleet_api
 Author: Brett Adams
 Author-email: admin@teslemetry.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `tesla_fleet_api-0.5.6/tesla_fleet_api.egg-info/SOURCES.txt` & `tesla_fleet_api-0.5.7/tesla_fleet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

