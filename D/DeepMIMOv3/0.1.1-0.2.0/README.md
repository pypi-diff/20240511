# Comparing `tmp/deepmimov3-0.1.1.tar.gz` & `tmp/deepmimov3-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepmimov3-0.1.1.tar", last modified: Sat May 11 16:53:50 2024, max compression
+gzip compressed data, was "deepmimov3-0.2.0.tar", last modified: Sat May 11 20:54:15 2024, max compression
```

## Comparing `deepmimov3-0.1.1.tar` & `deepmimov3-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 16:53:50.013807 deepmimov3-0.1.1/
--rw-r--r--   0 joao      (1000) joao      (1000)      428 2024-05-11 16:53:50.013807 deepmimov3-0.1.1/PKG-INFO
--rw-rw-r--   0 joao      (1000) joao      (1000)     3396 2024-05-11 15:36:00.000000 deepmimov3-0.1.1/README.md
--rw-rw-r--   0 joao      (1000) joao      (1000)       38 2024-05-11 16:53:50.013807 deepmimov3-0.1.1/setup.cfg
--rw-rw-r--   0 joao      (1000) joao      (1000)      892 2024-05-11 16:53:29.000000 deepmimov3-0.1.1/setup.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 16:53:50.013807 deepmimov3-0.1.1/src/
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 16:53:50.013807 deepmimov3-0.1.1/src/DeepMIMOv3/
--rw-rw-r--   0 joao      (1000) joao      (1000)      221 2024-05-11 15:36:00.000000 deepmimov3-0.1.1/src/DeepMIMOv3/__init__.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     2034 2024-05-11 15:36:00.000000 deepmimov3-0.1.1/src/DeepMIMOv3/ant_patterns.py
--rw-rw-r--   0 joao      (1000) joao      (1000)    14200 2024-05-11 15:36:00.000000 deepmimov3-0.1.1/src/DeepMIMOv3/construct_deepmimo.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     3362 2024-05-11 15:36:00.000000 deepmimov3-0.1.1/src/DeepMIMOv3/consts.py
--rw-rw-r--   0 joao      (1000) joao      (1000)    14821 2024-05-11 15:36:00.000000 deepmimov3-0.1.1/src/DeepMIMOv3/generator.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     3053 2024-05-11 15:36:00.000000 deepmimov3-0.1.1/src/DeepMIMOv3/params.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     7290 2024-05-11 15:36:00.000000 deepmimov3-0.1.1/src/DeepMIMOv3/raytracing_v2.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     8272 2024-05-11 15:36:00.000000 deepmimov3-0.1.1/src/DeepMIMOv3/raytracing_v3.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     5749 2024-05-11 15:36:00.000000 deepmimov3-0.1.1/src/DeepMIMOv3/sionna_adapter.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     2076 2024-05-11 15:36:00.000000 deepmimov3-0.1.1/src/DeepMIMOv3/utils.py
--rw-rw-r--   0 joao      (1000) joao      (1000)     3800 2024-05-11 16:45:47.000000 deepmimov3-0.1.1/src/DeepMIMOv3/visualization.py
-drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 16:53:50.013807 deepmimov3-0.1.1/src/DeepMIMOv3.egg-info/
--rw-r--r--   0 joao      (1000) joao      (1000)      428 2024-05-11 16:53:50.000000 deepmimov3-0.1.1/src/DeepMIMOv3.egg-info/PKG-INFO
--rw-rw-r--   0 joao      (1000) joao      (1000)      533 2024-05-11 16:53:50.000000 deepmimov3-0.1.1/src/DeepMIMOv3.egg-info/SOURCES.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)        1 2024-05-11 16:53:50.000000 deepmimov3-0.1.1/src/DeepMIMOv3.egg-info/dependency_links.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)       17 2024-05-11 16:53:50.000000 deepmimov3-0.1.1/src/DeepMIMOv3.egg-info/requires.txt
--rw-rw-r--   0 joao      (1000) joao      (1000)       11 2024-05-11 16:53:50.000000 deepmimov3-0.1.1/src/DeepMIMOv3.egg-info/top_level.txt
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 20:54:15.933889 deepmimov3-0.2.0/
+-rw-r--r--   0 joao      (1000) joao      (1000)      454 2024-05-11 20:54:15.933889 deepmimov3-0.2.0/PKG-INFO
+-rw-rw-r--   0 joao      (1000) joao      (1000)     3396 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/README.md
+-rw-rw-r--   0 joao      (1000) joao      (1000)       38 2024-05-11 20:54:15.933889 deepmimov3-0.2.0/setup.cfg
+-rw-rw-r--   0 joao      (1000) joao      (1000)      933 2024-05-11 20:53:52.000000 deepmimov3-0.2.0/setup.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 20:54:15.925889 deepmimov3-0.2.0/src/
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 20:54:15.933889 deepmimov3-0.2.0/src/DeepMIMOv3/
+-rw-rw-r--   0 joao      (1000) joao      (1000)      221 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/__init__.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     2034 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/ant_patterns.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)    14200 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/construct_deepmimo.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     3362 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/consts.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)    14786 2024-05-11 19:36:10.000000 deepmimov3-0.2.0/src/DeepMIMOv3/generator.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     3053 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/params.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     7290 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/raytracing_v2.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     8272 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/raytracing_v3.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     5749 2024-05-11 15:36:00.000000 deepmimov3-0.2.0/src/DeepMIMOv3/sionna_adapter.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)    10848 2024-05-11 20:32:46.000000 deepmimov3-0.2.0/src/DeepMIMOv3/utils.py
+-rw-rw-r--   0 joao      (1000) joao      (1000)     6644 2024-05-11 20:18:49.000000 deepmimov3-0.2.0/src/DeepMIMOv3/visualization.py
+drwxrwxr-x   0 joao      (1000) joao      (1000)        0 2024-05-11 20:54:15.933889 deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/
+-rw-r--r--   0 joao      (1000) joao      (1000)      454 2024-05-11 20:54:15.000000 deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/PKG-INFO
+-rw-rw-r--   0 joao      (1000) joao      (1000)      533 2024-05-11 20:54:15.000000 deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/SOURCES.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)        1 2024-05-11 20:54:15.000000 deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/dependency_links.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)       28 2024-05-11 20:54:15.000000 deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/requires.txt
+-rw-rw-r--   0 joao      (1000) joao      (1000)       11 2024-05-11 20:54:15.000000 deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/top_level.txt
```

### Comparing `deepmimov3-0.1.1/README.md` & `deepmimov3-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.1.1/src/DeepMIMOv3/ant_patterns.py` & `deepmimov3-0.2.0/src/DeepMIMOv3/ant_patterns.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.1.1/src/DeepMIMOv3/construct_deepmimo.py` & `deepmimov3-0.2.0/src/DeepMIMOv3/construct_deepmimo.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.1.1/src/DeepMIMOv3/consts.py` & `deepmimov3-0.2.0/src/DeepMIMOv3/consts.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.1.1/src/DeepMIMOv3/generator.py` & `deepmimov3-0.2.0/src/DeepMIMOv3/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 Description: Main generator script
 
 Authors: Umut Demirhan, Ahmed Alkhateeb
 Date: 12/10/2021
 """
 
 import os
+import copy
 import numpy as np
 
 import DeepMIMOv3.consts as c
 from DeepMIMOv3.construct_deepmimo import generate_MIMO_channel, generate_MIMO_channel_rx_ind
 from DeepMIMOv3.utils import safe_print
 from DeepMIMOv3.params import default_params
 
-
-def generate_data(params):
+def generate_data(ext_params):
     
     np.random.seed(1001)
     
-    params = validate_params(params)
+    params = validate_params(copy.deepcopy(ext_params))
     
     # If dynamic scenario
     if is_dynamic_scenario(params):
         scene_list = params[c.PARAMSET_DYNAMIC_SCENES]
         num_of_scenes = len(scene_list)
         dataset = []
         for scene_i in range(num_of_scenes):
@@ -95,18 +95,18 @@
                 if not params[c.PARAMSET_ANT_BS_DIFF]:
                     dataset[i][c.DICT_BS_IDX][c.OUT_CHANNEL], dataset[i][c.DICT_BS_IDX][c.OUT_LOS] = np.stack(dataset[i][c.DICT_BS_IDX][c.OUT_CHANNEL], axis=0)
     return dataset
 
 # TODO: Move validation into another script
 def validate_params(params):
 
-    # TODO: Show parameters that are not used in the generation - This allows 
-    # additional_keys = compare_two_params(params, default_params)
-    # print('Following parameters seems unnecessary:')
-    # print(additional_keys)
+    additional_keys = compare_two_dicts(params, default_params())
+    if len(additional_keys):
+        print('The following parameters seem unnecessary:')
+        print(additional_keys)
     
     params['dynamic_scenario'] = is_dynamic_scenario(params)
     if params['dynamic_scenario']:
         params['user_rows'] = np.array([0])
     params['data_version'] = check_data_version(params)
     params[c.PARAMSET_SCENARIO_PARAMS_PATH] = get_scenario_params_path(params)
     if params['data_version'] == 'v2':
@@ -254,17 +254,17 @@
                                    'params.mat'
                                   )
     else:
         raise NotImplementedError
         
     return params_path
 
-def compare_two_params(params, default_params):
+def compare_two_dicts(dict1, dict2):
     
-    additional_keys = params.keys() - default_params.keys()
-    for key, item in params.items():
+    additional_keys = dict1.keys() - dict2.keys()
+    for key, item in dict1.items():
         if isinstance(item, dict):
-            if key in default_params:
-                additional_keys += compare_two_params(params[key], default_params[key])
+            if key in dict2:
+                additional_keys = additional_keys | compare_two_dicts(dict1[key], dict2[key])
 
     return additional_keys
```

### Comparing `deepmimov3-0.1.1/src/DeepMIMOv3/params.py` & `deepmimov3-0.2.0/src/DeepMIMOv3/params.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.1.1/src/DeepMIMOv3/raytracing_v2.py` & `deepmimov3-0.2.0/src/DeepMIMOv3/raytracing_v2.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.1.1/src/DeepMIMOv3/raytracing_v3.py` & `deepmimov3-0.2.0/src/DeepMIMOv3/raytracing_v3.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.1.1/src/DeepMIMOv3/sionna_adapter.py` & `deepmimov3-0.2.0/src/DeepMIMOv3/sionna_adapter.py`

 * *Files identical despite different names*

### Comparing `deepmimov3-0.1.1/src/DeepMIMOv3.egg-info/SOURCES.txt` & `deepmimov3-0.2.0/src/DeepMIMOv3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

