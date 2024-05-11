# Comparing `tmp/kagiapi-0.2.0.tar.gz` & `tmp/kagiapi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kagiapi-0.2.0.tar", last modified: Thu Dec 28 15:44:33 2023, max compression
+gzip compressed data, was "kagiapi-0.2.1.tar", last modified: Sat May 11 20:54:06 2024, max compression
```

## Comparing `kagiapi-0.2.0.tar` & `kagiapi-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-12-28 15:44:33.504072 kagiapi-0.2.0/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-17 21:01:33.000000 kagiapi-0.2.0/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)      302 2023-12-28 15:44:33.503669 kagiapi-0.2.0/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)    12255 2023-12-28 15:41:50.000000 kagiapi-0.2.0/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-12-28 15:44:33.501593 kagiapi-0.2.0/kagiapi/
--rw-r--r--   0 prelovac   (502) staff       (20)       28 2023-04-17 19:53:45.000000 kagiapi-0.2.0/kagiapi/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2835 2023-12-28 15:41:50.000000 kagiapi-0.2.0/kagiapi/api.py
--rw-r--r--   0 prelovac   (502) staff       (20)     1543 2023-12-28 15:41:50.000000 kagiapi-0.2.0/kagiapi/models.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-12-28 15:44:33.503304 kagiapi-0.2.0/kagiapi.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)      302 2023-12-28 15:44:33.000000 kagiapi-0.2.0/kagiapi.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      233 2023-12-28 15:44:33.000000 kagiapi-0.2.0/kagiapi.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-12-28 15:44:33.000000 kagiapi-0.2.0/kagiapi.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       27 2023-12-28 15:44:33.000000 kagiapi-0.2.0/kagiapi.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        8 2023-12-28 15:44:33.000000 kagiapi-0.2.0/kagiapi.egg-info/top_level.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-12-28 15:44:33.504168 kagiapi-0.2.0/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)      404 2023-12-28 15:42:04.000000 kagiapi-0.2.0/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2024-05-11 20:54:06.322212 kagiapi-0.2.1/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-17 21:01:33.000000 kagiapi-0.2.1/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)      302 2024-05-11 20:54:06.321826 kagiapi-0.2.1/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    12322 2024-05-11 20:53:22.000000 kagiapi-0.2.1/README.md
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2024-05-11 20:54:06.319717 kagiapi-0.2.1/kagiapi/
+-rw-r--r--   0 prelovac   (502) staff       (20)       28 2023-04-17 19:53:45.000000 kagiapi-0.2.1/kagiapi/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2915 2024-05-11 20:53:22.000000 kagiapi-0.2.1/kagiapi/api.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     1543 2023-12-28 15:41:50.000000 kagiapi-0.2.1/kagiapi/models.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2024-05-11 20:54:06.321457 kagiapi-0.2.1/kagiapi.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)      302 2024-05-11 20:54:06.000000 kagiapi-0.2.1/kagiapi.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      233 2024-05-11 20:54:06.000000 kagiapi-0.2.1/kagiapi.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2024-05-11 20:54:06.000000 kagiapi-0.2.1/kagiapi.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       27 2024-05-11 20:54:06.000000 kagiapi-0.2.1/kagiapi.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        8 2024-05-11 20:54:06.000000 kagiapi-0.2.1/kagiapi.egg-info/top_level.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2024-05-11 20:54:06.322302 kagiapi-0.2.1/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)      404 2024-05-11 20:53:49.000000 kagiapi-0.2.1/setup.py
```

### Comparing `kagiapi-0.2.0/LICENSE` & `kagiapi-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kagiapi-0.2.0/README.md` & `kagiapi-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Kagi API Python Package
 
 [![](https://dcbadge.vercel.app/api/server/aDNg6E9szy?compact=true&style=flat)](https://discord.gg/aDNg6E9szy) [![Twitter](https://img.shields.io/twitter/follow/KagiHQ?style=social)](https://twitter.com/KagiHQ) [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/license/mit/) 
 
-A Python package for interacting with the [Kagi API](https://help.kagi.com/kagi/api/overview.html).
+A Python package for interacting with the [Kagi API](https://help.kagi.com/kagi/api/overview.html). Get your Kagi API token [here](https://kagi.com/settings?p=api).
 
 ## Installation
 
 ```bash
 pip install kagiapi
 ```
 
@@ -19,15 +19,15 @@
 kagi = KagiClient(api_key)
 ```
 
 You can also define KAGI_API_KEY environment variable.
 
 ### Searh API
 ```py
-query = "steve jobs"
+query = "grand canyon"
 results = kagi.search(query, limit=10)
 
 for result in results["data"]:
     print(result["title"])
 ```
 
 #### Example Response
```

### Comparing `kagiapi-0.2.0/kagiapi/api.py` & `kagiapi-0.2.1/kagiapi/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,26 +59,26 @@
             raise ValueError(
                 "Parameters url and text are exclusive. You must pass one or the other."
             )
 
         if target_language:
             params["target_language"] = target_language
 
-        if cache:
-            params["cache"] = cache
+        if cache is not None:
+            params["cache"] = "true" if cache else "false"
 
         response = self.session.get(KagiClient.BASE_URL + "/summarize", params=params)
         response.raise_for_status()
         return response.json()
 
-    def fastgpt(self, query: str, cache: bool = True) -> FastGPTResponse:
+    def fastgpt(self, query: str, cache: Optional[bool] = True) -> FastGPTResponse:
         data: Dict[str, Union[int, str]] = {"query": query}
 
-        if cache:
-            data["cache"] = cache
+        if cache is not None:
+            data["cache"] = "true" if cache else "false"
 
         response = self.session.post(KagiClient.BASE_URL + "/fastgpt", json=data)
         response.raise_for_status()
         return response.json()
 
     def enrich(self, query: str) -> EnrichResponse:
         params: Dict[str, Union[int, str]] = {"q": query}
```

### Comparing `kagiapi-0.2.0/kagiapi/models.py` & `kagiapi-0.2.1/kagiapi/models.py`

 * *Files identical despite different names*

