# Comparing `tmp/viessmann_gridbox_connector-1.3.7.tar.gz` & `tmp/viessmann_gridbox_connector-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viessmann_gridbox_connector-1.3.7.tar", last modified: Sat May  4 10:41:37 2024, max compression
+gzip compressed data, was "viessmann_gridbox_connector-1.3.8.tar", last modified: Fri May 10 05:51:28 2024, max compression
```

## Comparing `viessmann_gridbox_connector-1.3.7.tar` & `viessmann_gridbox_connector-1.3.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:37.866652 viessmann_gridbox_connector-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-04 10:41:28.000000 viessmann_gridbox_connector-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-04 10:41:37.866652 viessmann_gridbox_connector-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-04 10:41:28.000000 viessmann_gridbox_connector-1.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:37.862652 viessmann_gridbox_connector-1.3.7/gridbox_connector/
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-04 10:41:28.000000 viessmann_gridbox_connector-1.3.7/gridbox_connector/GridboxConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-04 10:41:28.000000 viessmann_gridbox_connector-1.3.7/gridbox_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-04 10:41:28.000000 viessmann_gridbox_connector-1.3.7/gridbox_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 10:41:37.866652 viessmann_gridbox_connector-1.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-04 10:41:28.000000 viessmann_gridbox_connector-1.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:41:37.866652 viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-04 10:41:37.000000 viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-04 10:41:37.000000 viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 10:41:37.000000 viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 10:41:37.000000 viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-04 10:41:37.000000 viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:51:28.262531 viessmann_gridbox_connector-1.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-10 05:51:24.000000 viessmann_gridbox_connector-1.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-10 05:51:28.262531 viessmann_gridbox_connector-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-10 05:51:24.000000 viessmann_gridbox_connector-1.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:51:28.262531 viessmann_gridbox_connector-1.3.8/gridbox_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-10 05:51:24.000000 viessmann_gridbox_connector-1.3.8/gridbox_connector/GridboxConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-10 05:51:24.000000 viessmann_gridbox_connector-1.3.8/gridbox_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-10 05:51:24.000000 viessmann_gridbox_connector-1.3.8/gridbox_connector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 05:51:28.262531 viessmann_gridbox_connector-1.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-10 05:51:24.000000 viessmann_gridbox_connector-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:51:28.262531 viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-10 05:51:28.000000 viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-10 05:51:28.000000 viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 05:51:28.000000 viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 05:51:28.000000 viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 05:51:28.000000 viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/top_level.txt
```

### Comparing `viessmann_gridbox_connector-1.3.7/LICENSE` & `viessmann_gridbox_connector-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `viessmann_gridbox_connector-1.3.7/PKG-INFO` & `viessmann_gridbox_connector-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viessmann-gridbox-connector
-Version: 1.3.7
+Version: 1.3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # Viessmann Gridbox Connector
 **This is not an official Viessmann library**
```

### Comparing `viessmann_gridbox_connector-1.3.7/README.md` & `viessmann_gridbox_connector-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `viessmann_gridbox_connector-1.3.7/gridbox_connector/GridboxConnector.py` & `viessmann_gridbox_connector-1.3.8/gridbox_connector/GridboxConnector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 import requests
 import time
+
+
 class GridboxConnector:
-    id_token = ""
-    gateways = []
+    id_token: str = ""
+    gateways: list[str] = []
 
-    def __init__(self,config):
+    def __init__(self, config):
         self.login_url = config["urls"]["login"]
         self.login_body = config["login"]
         self.gateway_url = config["urls"]["gateways"]
         self.live_url = config["urls"]["live"]
         self.init_auth()
-    
+
     def init_auth(self):
         self.get_token()
         self.generate_header()
         self.get_gateway_id()
 
     def get_token(self):
         response = requests.post(self.login_url, self.login_body)
         response_json = response.json()
         print(response_json)
         if "id_token" in response_json:
-            self.id_token  = response_json["id_token"]
+            self.id_token = response_json["id_token"]
         else:
             print("token not found")
             print(response_json)
-            time.wait(60)
+            time.sleep(60)
             self.get_token()
-       
+
     def generate_header(self):
         self.headers = {"Authorization": "Bearer {}".format(self.id_token)}
 
     def get_gateway_id(self):
         self.gateways.clear()
-        response = requests.get(self.gateway_url,headers=self.headers)
+        response = requests.get(self.gateway_url, headers=self.headers)
         response_json = response.json()
         for gateway in response_json:
             self.gateways.append(gateway["system"]["id"])
-        
 
     def retrieve_live_data(self):
         responses = []
         for id in self.gateways:
-            response = requests.get(self.live_url.format(self.id), headers=self.headers)
+            response = requests.get(
+                self.live_url.format(id), headers=self.headers)
             if response.status_code == 200:
                 response_json = response.json()
                 responses.append(response_json)
-                #print(response_json)
+                # print(response_json)
             else:
                 print("Status Code {}".format(response.status_code))
                 print("Response {}".format(response.json()))
                 time.sleep(60)
                 self.init_auth()
                 return self.retrieve_live_data()
         return responses
```

### Comparing `viessmann_gridbox_connector-1.3.7/viessmann_gridbox_connector.egg-info/PKG-INFO` & `viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viessmann-gridbox-connector
-Version: 1.3.7
+Version: 1.3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # Viessmann Gridbox Connector
 **This is not an official Viessmann library**
```

