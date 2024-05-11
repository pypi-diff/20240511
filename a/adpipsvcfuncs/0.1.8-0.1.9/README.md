# Comparing `tmp/adpipsvcfuncs-0.1.8.tar.gz` & `tmp/adpipsvcfuncs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adpipsvcfuncs-0.1.8.tar", last modified: Wed May  8 19:30:20 2024, max compression
+gzip compressed data, was "adpipsvcfuncs-0.1.9.tar", last modified: Thu May  9 21:33:18 2024, max compression
```

## Comparing `adpipsvcfuncs-0.1.8.tar` & `adpipsvcfuncs-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 19:30:20.251427 adpipsvcfuncs-0.1.8/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-05-08 19:29:37.000000 adpipsvcfuncs-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      329 2024-05-08 19:30:20.251427 adpipsvcfuncs-0.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       74 2024-05-08 19:29:37.000000 adpipsvcfuncs-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 19:30:20.247427 adpipsvcfuncs-0.1.8/adpipsvcfuncs/
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-08 19:29:37.000000 adpipsvcfuncs-0.1.8/adpipsvcfuncs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2560 2024-05-08 19:29:37.000000 adpipsvcfuncs-0.1.8/adpipsvcfuncs/adpipsvcfuncs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 19:30:20.251427 adpipsvcfuncs-0.1.8/adpipsvcfuncs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      329 2024-05-08 19:30:20.000000 adpipsvcfuncs-0.1.8/adpipsvcfuncs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      267 2024-05-08 19:30:20.000000 adpipsvcfuncs-0.1.8/adpipsvcfuncs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 19:30:20.000000 adpipsvcfuncs-0.1.8/adpipsvcfuncs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2024-05-08 19:30:20.000000 adpipsvcfuncs-0.1.8/adpipsvcfuncs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-08 19:30:20.000000 adpipsvcfuncs-0.1.8/adpipsvcfuncs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 19:30:20.251427 adpipsvcfuncs-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      511 2024-05-08 19:29:37.000000 adpipsvcfuncs-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 21:33:18.865650 adpipsvcfuncs-0.1.9/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-09 21:32:33.000000 adpipsvcfuncs-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      329 2024-05-09 21:33:18.865650 adpipsvcfuncs-0.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       74 2024-05-09 21:32:33.000000 adpipsvcfuncs-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 21:33:18.861649 adpipsvcfuncs-0.1.9/adpipsvcfuncs/
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-09 21:32:33.000000 adpipsvcfuncs-0.1.9/adpipsvcfuncs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3316 2024-05-09 21:32:33.000000 adpipsvcfuncs-0.1.9/adpipsvcfuncs/adpipsvcfuncs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 21:33:18.861649 adpipsvcfuncs-0.1.9/adpipsvcfuncs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      329 2024-05-09 21:33:18.000000 adpipsvcfuncs-0.1.9/adpipsvcfuncs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-09 21:33:18.000000 adpipsvcfuncs-0.1.9/adpipsvcfuncs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 21:33:18.000000 adpipsvcfuncs-0.1.9/adpipsvcfuncs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2024-05-09 21:33:18.000000 adpipsvcfuncs-0.1.9/adpipsvcfuncs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-09 21:33:18.000000 adpipsvcfuncs-0.1.9/adpipsvcfuncs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 21:33:18.865650 adpipsvcfuncs-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-09 21:32:33.000000 adpipsvcfuncs-0.1.9/setup.py
```

### Comparing `adpipsvcfuncs-0.1.8/LICENSE` & `adpipsvcfuncs-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adpipsvcfuncs-0.1.8/adpipsvcfuncs/adpipsvcfuncs.py` & `adpipsvcfuncs-0.1.9/adpipsvcfuncs/adpipsvcfuncs.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,8 +60,29 @@
 def load_valid_json(string) -> dict:
     try:
         loaded_json = json.loads(string)
         return loaded_json
     except Exception as e:
         logger.error(f"JSON validation failed: {str(e)}, string: {string}")
         return None
+    
+def load_current_pipeline_data(pipeline_id: str):
+    api_url = fetch_gcp_secret('adaptive-pipeline-persistence-layer-url')
+    api_key = fetch_gcp_secret('adaptive-pipeline-API-token')
+
+    if not api_url:
+        logger.error("Failed to fetch the API URL")
+        return None
+    headers = {
+            "Authorization": api_key
+        }
+    try:
+        response = requests.get(f"{api_url}/read/{pipeline_id}", headers=headers)
+        if response.status_code != 200:
+            logger.error(f"Failed to fetch the pipeline data. Response: {response.text}")
+            return None
+        pipeline_data = response.json()
+        return pipeline_data
+    except Exception as e:
+        logger.error(f"Error: {str(e)}")
+        return None
```

