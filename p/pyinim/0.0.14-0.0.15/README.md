# Comparing `tmp/pyinim-0.0.14.tar.gz` & `tmp/pyinim-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinim-0.0.14.tar", last modified: Sun May  5 13:43:52 2024, max compression
+gzip compressed data, was "pyinim-0.0.15.tar", last modified: Sat May 11 19:18:47 2024, max compression
```

## Comparing `pyinim-0.0.14.tar` & `pyinim-0.0.15.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:43:52.482346 pyinim-0.0.14/
--rw-r--r--   0 bertulla (1473677006) 52240112    35149 2024-04-27 20:46:49.000000 pyinim-0.0.14/LICENSE
--rw-r--r--   0 bertulla (1473677006) 52240112     3318 2024-05-05 13:43:52.482265 pyinim-0.0.14/PKG-INFO
--rw-r--r--   0 bertulla (1473677006) 52240112     2693 2024-05-05 13:43:43.000000 pyinim-0.0.14/README.md
--rw-r--r--   0 bertulla (1473677006) 52240112      621 2024-05-05 13:43:44.000000 pyinim-0.0.14/pyproject.toml
--rw-r--r--   0 bertulla (1473677006) 52240112      418 2024-05-05 13:43:52.482587 pyinim-0.0.14/setup.cfg
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:43:52.478743 pyinim-0.0.14/src/
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:43:52.480065 pyinim-0.0.14/src/pyinim/
--rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-04-27 20:46:49.000000 pyinim-0.0.14/src/pyinim/__init__.py
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:43:52.481141 pyinim-0.0.14/src/pyinim/cloud/
--rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-04-27 20:46:49.000000 pyinim-0.0.14/src/pyinim/cloud/__init__.py
--rw-r--r--   0 bertulla (1473677006) 52240112     2215 2024-05-05 13:11:55.000000 pyinim-0.0.14/src/pyinim/cloud/abc.py
--rw-r--r--   0 bertulla (1473677006) 52240112     2169 2024-05-05 13:11:55.000000 pyinim-0.0.14/src/pyinim/cloud/resolver.py
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:43:52.481512 pyinim-0.0.14/src/pyinim/cloud/types/
--rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-04-27 20:46:49.000000 pyinim-0.0.14/src/pyinim/cloud/types/__init__.py
--rw-r--r--   0 bertulla (1473677006) 52240112     2304 2024-04-27 20:46:49.000000 pyinim-0.0.14/src/pyinim/cloud/types/devices.py
--rw-r--r--   0 bertulla (1473677006) 52240112      489 2024-04-27 20:46:49.000000 pyinim-0.0.14/src/pyinim/cloud/types/token.py
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:43:52.481774 pyinim-0.0.14/src/pyinim/examples/
--rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-04-28 08:28:37.000000 pyinim-0.0.14/src/pyinim/examples/__init__.py
--rw-r--r--   0 bertulla (1473677006) 52240112     1390 2024-05-05 13:11:55.000000 pyinim-0.0.14/src/pyinim/examples/poc.py
--rw-r--r--   0 bertulla (1473677006) 52240112     1584 2024-05-05 13:11:55.000000 pyinim-0.0.14/src/pyinim/inim_cloud.py
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-05 13:43:52.481959 pyinim-0.0.14/src/pyinim.egg-info/
--rw-r--r--   0 bertulla (1473677006) 52240112     3318 2024-05-05 13:43:52.000000 pyinim-0.0.14/src/pyinim.egg-info/PKG-INFO
--rw-r--r--   0 bertulla (1473677006) 52240112      501 2024-05-05 13:43:52.000000 pyinim-0.0.14/src/pyinim.egg-info/SOURCES.txt
--rw-r--r--   0 bertulla (1473677006) 52240112        1 2024-05-05 13:43:52.000000 pyinim-0.0.14/src/pyinim.egg-info/dependency_links.txt
--rw-r--r--   0 bertulla (1473677006) 52240112       53 2024-05-05 13:43:52.000000 pyinim-0.0.14/src/pyinim.egg-info/requires.txt
--rw-r--r--   0 bertulla (1473677006) 52240112        7 2024-05-05 13:43:52.000000 pyinim-0.0.14/src/pyinim.egg-info/top_level.txt
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:18:47.365331 pyinim-0.0.15/
+-rw-r--r--   0 bertulla (1473677006) 52240112    35149 2024-04-27 20:46:49.000000 pyinim-0.0.15/LICENSE
+-rw-r--r--   0 bertulla (1473677006) 52240112     3471 2024-05-11 19:18:47.365268 pyinim-0.0.15/PKG-INFO
+-rw-r--r--   0 bertulla (1473677006) 52240112     2846 2024-05-07 11:00:54.000000 pyinim-0.0.15/README.md
+-rw-r--r--   0 bertulla (1473677006) 52240112      621 2024-05-07 10:55:00.000000 pyinim-0.0.15/pyproject.toml
+-rw-r--r--   0 bertulla (1473677006) 52240112      418 2024-05-11 19:18:47.365559 pyinim-0.0.15/setup.cfg
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:18:47.362209 pyinim-0.0.15/src/
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:18:47.363194 pyinim-0.0.15/src/pyinim/
+-rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-05-07 10:55:00.000000 pyinim-0.0.15/src/pyinim/__init__.py
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:18:47.364278 pyinim-0.0.15/src/pyinim/cloud/
+-rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-05-07 10:55:00.000000 pyinim-0.0.15/src/pyinim/cloud/__init__.py
+-rw-r--r--   0 bertulla (1473677006) 52240112     2465 2024-05-07 11:00:54.000000 pyinim-0.0.15/src/pyinim/cloud/abc.py
+-rw-r--r--   0 bertulla (1473677006) 52240112      195 2024-05-07 11:00:54.000000 pyinim-0.0.15/src/pyinim/cloud/exceptions.py
+-rw-r--r--   0 bertulla (1473677006) 52240112     2305 2024-05-07 11:07:15.000000 pyinim-0.0.15/src/pyinim/cloud/resolver.py
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:18:47.364613 pyinim-0.0.15/src/pyinim/cloud/types/
+-rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-05-07 10:55:00.000000 pyinim-0.0.15/src/pyinim/cloud/types/__init__.py
+-rw-r--r--   0 bertulla (1473677006) 52240112     2304 2024-05-07 10:55:00.000000 pyinim-0.0.15/src/pyinim/cloud/types/devices.py
+-rw-r--r--   0 bertulla (1473677006) 52240112      489 2024-05-07 10:55:00.000000 pyinim-0.0.15/src/pyinim/cloud/types/token.py
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:18:47.364844 pyinim-0.0.15/src/pyinim/examples/
+-rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-05-07 10:55:00.000000 pyinim-0.0.15/src/pyinim/examples/__init__.py
+-rw-r--r--   0 bertulla (1473677006) 52240112     1390 2024-05-07 10:55:00.000000 pyinim-0.0.15/src/pyinim/examples/poc.py
+-rw-r--r--   0 bertulla (1473677006) 52240112     1584 2024-05-07 10:55:00.000000 pyinim-0.0.15/src/pyinim/inim_cloud.py
+drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:18:47.364999 pyinim-0.0.15/src/pyinim.egg-info/
+-rw-r--r--   0 bertulla (1473677006) 52240112     3471 2024-05-11 19:18:47.000000 pyinim-0.0.15/src/pyinim.egg-info/PKG-INFO
+-rw-r--r--   0 bertulla (1473677006) 52240112      532 2024-05-11 19:18:47.000000 pyinim-0.0.15/src/pyinim.egg-info/SOURCES.txt
+-rw-r--r--   0 bertulla (1473677006) 52240112        1 2024-05-11 19:18:47.000000 pyinim-0.0.15/src/pyinim.egg-info/dependency_links.txt
+-rw-r--r--   0 bertulla (1473677006) 52240112       53 2024-05-11 19:18:47.000000 pyinim-0.0.15/src/pyinim.egg-info/requires.txt
+-rw-r--r--   0 bertulla (1473677006) 52240112        7 2024-05-11 19:18:47.000000 pyinim-0.0.15/src/pyinim.egg-info/top_level.txt
```

### Comparing `pyinim-0.0.14/LICENSE` & `pyinim-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.14/PKG-INFO` & `pyinim-0.0.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinim
-Version: 0.0.14
+Version: 0.0.15
 Summary: A Inim Cloud API client
 Home-page: https://github.com/nidble/pyinim
 Author: Antonino Bertulla
 Author-email: Antonino Bertulla <abertulla@email.address>
 Project-URL: Homepage, https://github.com/nidble/pyinim
 Project-URL: Issues, https://github.com/nidble/pyinim/issues
 Classifier: Programming Language :: Python :: 3
@@ -22,29 +22,34 @@
 ## Usage
 
 ```sh
 python3 -m venv venv
 source venv/bin/activate.fish
 python3 -m pip install aiohttp==3.9.5
 # python3 -m pip install python-dotenv==1.0.1
-python3 -m pip install --index-url https://test.pypi.org/simple/ pyinim-nidble==0.0.14
+
+# deprecated: 
+#python3 -m pip install --index-url https://test.pypi.org/simple/ pyinim-nidble==0.0.x
 # python3 -m pip uninstall pyinim-nidble
+
+python3 -m pip install pyinim==0.0.x
+python3 -m pip uninstall pyinim
 ```
 
 ## Development
 
 ### Environment preparation
 ```sh
 python3 -m pip install pipenv
 pipenv install --dev #this generate Pipfile.lock
 ```
 
 ### Running
 ```sh
-cd src
+export PYTHONPATH="${PYTHONPATH}:$PWD" # or set --export PYTHONPATH ./src
 pipenv run python src/pyinim/examples/poc.py
 ```
 
 ### Adding new lib
 ```sh
 pipenv install python-dotenv
 ```
```

### Comparing `pyinim-0.0.14/README.md` & `pyinim-0.0.15/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 ## Usage
 
 ```sh
 python3 -m venv venv
 source venv/bin/activate.fish
 python3 -m pip install aiohttp==3.9.5
 # python3 -m pip install python-dotenv==1.0.1
-python3 -m pip install --index-url https://test.pypi.org/simple/ pyinim-nidble==0.0.14
+
+# deprecated: 
+#python3 -m pip install --index-url https://test.pypi.org/simple/ pyinim-nidble==0.0.x
 # python3 -m pip uninstall pyinim-nidble
+
+python3 -m pip install pyinim==0.0.x
+python3 -m pip uninstall pyinim
 ```
 
 ## Development
 
 ### Environment preparation
 ```sh
 python3 -m pip install pipenv
 pipenv install --dev #this generate Pipfile.lock
 ```
 
 ### Running
 ```sh
-cd src
+export PYTHONPATH="${PYTHONPATH}:$PWD" # or set --export PYTHONPATH ./src
 pipenv run python src/pyinim/examples/poc.py
 ```
 
 ### Adding new lib
 ```sh
 pipenv install python-dotenv
 ```
```

### Comparing `pyinim-0.0.14/pyproject.toml` & `pyinim-0.0.15/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyinim"
-version = "0.0.14"
+version = "0.0.15"
 authors = [
   { name="Antonino Bertulla", email="abertulla@email.address" },
 ]
 description = "A Inim Cloud API client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyinim-0.0.14/src/pyinim/cloud/abc.py` & `pyinim-0.0.15/src/pyinim/cloud/abc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Provide an abstract base class for easier requests."""
 import abc
 from typing import Optional as Mapping, Tuple, Mapping
 
+from pyinim.cloud.exceptions import MalformedResponseError
 from pyinim.cloud.resolver import CloudResolver
 from pyinim.cloud.types.token import Token
 from pyinim.cloud.types.devices import Devices
 
 class InimAPI(abc.ABC):
 
     """Provide an idiomatic API for making calls to Inim's API."""
@@ -32,15 +33,18 @@
 
     @abc.abstractmethod
     async def token(self) -> str:
         """Get the token string."""
 
     async def get_token(self) -> Tuple[int, Mapping[str, str], Token]:
         status, headers, raw_response = await self._request('GET', self.resolver.get_token_url(), headers={})
-        return status, headers, self.resolver.str_to_token(raw_response)
+        parsed_response = self.resolver.str_to_token(raw_response)
+        if parsed_response.Data is None:
+            raise MalformedResponseError(f"Failed to get Token with {status=} and payload {raw_response=}")
+        return status, headers, parsed_response
 
     async def get_request_poll(self, device_id: str) -> Tuple[int, Mapping[str, str], None]:
         status, headers, raw_response = await self._request('GET', self.resolver.get_request_poll_url(await self.token(), device_id), headers={})
         return status, headers, None
 
     async def get_devices_extended(self, device_id: str) -> Tuple[int, Mapping[str, str], Devices]:
         status, headers, raw_response = await self._request('GET', self.resolver.get_devices_extended_url(await self.token()), headers={})
```

### Comparing `pyinim-0.0.14/src/pyinim/cloud/resolver.py` & `pyinim-0.0.15/src/pyinim/cloud/resolver.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,32 @@
 class CloudResolver:
     def __init__(self, username, password, client_id):
         self.password = password
         self.username = username
         self.client_id = client_id
 
     def get_token_url(self):
-        return f'{API_CLOUD_BASEURL}?req={{"Node":"","Name":"AlienMobilePro","ClientIP":"","Method":"RegisterClient","ClientId":"","Token":"","Params":{{"Username":"{self.username}","Password":"{self.password}","ClientId":"{self.client_id}","ClientName":"GalaxyS7edge","ClientInfo":"{{"name":"com.inim.alienmobile","version":"3.1.0","device":"hero2lte","brand":"samsung","platform":"android","osversion":"Oreo+v8.0,+API+Level:+26"}}","Role":"1","Brand":"0"}}}}'
+        data = {
+            "Node": "",
+            "Name": "AlienMobilePro",
+            "ClientIP": "",
+            "Method": "RegisterClient",
+            "ClientId": "",
+            "Token": "",
+            "Params": {
+                "Username": f'{self.username}',
+                "Password": f'{self.password}',
+                "ClientId": f'{self.client_id}',
+                "ClientName": "Galaxy+S8+edge",
+                "ClientInfo": json.dumps({}),
+            "Role": "1",
+            "Brand": "0"
+            }
+        }
+        return f'{API_CLOUD_BASEURL}?req={json.dumps(data)}'
 
     def get_devices_extended_url(self, token):
         return f'{API_CLOUD_BASEURL}?req={{"Params":{{"Info":4223}},"Node":"","Name":"Inim Home","ClientIP":"","Method":"GetDevicesExtended","Token":"{token}","ClientId": "{self.client_id}","Context":"intrusion"}}'
 
     def get_request_poll_url(self, token, device_id):
         return  f'{API_CLOUD_BASEURL}?req={{"Params":{{"DeviceId":{device_id},"Type":5}},"Node":"","Name":"Inim Home","ClientIP":"","Method":"RequestPoll","Token":"{token}","ClientId":"{self.client_id}","Context":"intrusion"}}'
```

### Comparing `pyinim-0.0.14/src/pyinim/cloud/types/devices.py` & `pyinim-0.0.15/src/pyinim/cloud/types/devices.py`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.14/src/pyinim/examples/poc.py` & `pyinim-0.0.15/src/pyinim/examples/poc.py`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.14/src/pyinim/inim_cloud.py` & `pyinim-0.0.15/src/pyinim/inim_cloud.py`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.14/src/pyinim.egg-info/PKG-INFO` & `pyinim-0.0.15/src/pyinim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinim
-Version: 0.0.14
+Version: 0.0.15
 Summary: A Inim Cloud API client
 Home-page: https://github.com/nidble/pyinim
 Author: Antonino Bertulla
 Author-email: Antonino Bertulla <abertulla@email.address>
 Project-URL: Homepage, https://github.com/nidble/pyinim
 Project-URL: Issues, https://github.com/nidble/pyinim/issues
 Classifier: Programming Language :: Python :: 3
@@ -22,29 +22,34 @@
 ## Usage
 
 ```sh
 python3 -m venv venv
 source venv/bin/activate.fish
 python3 -m pip install aiohttp==3.9.5
 # python3 -m pip install python-dotenv==1.0.1
-python3 -m pip install --index-url https://test.pypi.org/simple/ pyinim-nidble==0.0.14
+
+# deprecated: 
+#python3 -m pip install --index-url https://test.pypi.org/simple/ pyinim-nidble==0.0.x
 # python3 -m pip uninstall pyinim-nidble
+
+python3 -m pip install pyinim==0.0.x
+python3 -m pip uninstall pyinim
 ```
 
 ## Development
 
 ### Environment preparation
 ```sh
 python3 -m pip install pipenv
 pipenv install --dev #this generate Pipfile.lock
 ```
 
 ### Running
 ```sh
-cd src
+export PYTHONPATH="${PYTHONPATH}:$PWD" # or set --export PYTHONPATH ./src
 pipenv run python src/pyinim/examples/poc.py
 ```
 
 ### Adding new lib
 ```sh
 pipenv install python-dotenv
 ```
```

