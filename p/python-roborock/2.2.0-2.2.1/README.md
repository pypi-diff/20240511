# Comparing `tmp/python_roborock-2.2.0.tar.gz` & `tmp/python_roborock-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-2.2.0.tar", max compression
+gzip compressed data, was "python_roborock-2.2.1.tar", max compression
```

## Comparing `python_roborock-2.2.0.tar` & `python_roborock-2.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2024-05-09 22:02:21.121070 python_roborock-2.2.0/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-09 22:02:21.121070 python_roborock-2.2.0/README.md
--rw-r--r--   0        0        0     1677 2024-05-09 22:02:21.837068 python_roborock-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      165 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/__init__.py
--rw-r--r--   0        0        0     4123 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/api.py
--rw-r--r--   0        0        0     6826 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/cli.py
--rw-r--r--   0        0        0     7144 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/cloud_api.py
--rw-r--r--   0        0        0    14400 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/code_mappings.py
--rw-r--r--   0        0        0     7912 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/command_cache.py
--rw-r--r--   0        0        0     2386 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/const.py
--rw-r--r--   0        0        0    27991 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/containers.py
--rw-r--r--   0        0        0     1962 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/exceptions.py
--rw-r--r--   0        0        0     4367 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/local_api.py
--rw-r--r--   0        0        0    12315 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/protocol.py
--rw-r--r--   0        0        0        0 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/py.typed
--rw-r--r--   0        0        0      834 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/roborock_future.py
--rw-r--r--   0        0        0     5464 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/roborock_message.py
--rw-r--r--   0        0        0    23536 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/roborock_typing.py
--rw-r--r--   0        0        0     3465 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/util.py
--rw-r--r--   0        0        0      183 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_1_apis/__init__.py
--rw-r--r--   0        0        0    20099 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_1_apis/roborock_client_v1.py
--rw-r--r--   0        0        0     3477 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_1_apis/roborock_local_client_v1.py
--rw-r--r--   0        0        0     3358 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_1_apis/roborock_mqtt_client_v1.py
--rw-r--r--   0        0        0      111 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_a01_apis/__init__.py
--rw-r--r--   0        0        0     7424 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_a01_apis/roborock_client_a01.py
--rw-r--r--   0        0        0     3043 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/version_a01_apis/roborock_mqtt_client_a01.py
--rw-r--r--   0        0        0    13040 2024-05-09 22:02:21.125071 python_roborock-2.2.0/roborock/web_api.py
--rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 python_roborock-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-11 12:19:16.216947 python_roborock-2.2.1/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-11 12:19:16.216947 python_roborock-2.2.1/README.md
+-rw-r--r--   0        0        0     1677 2024-05-11 12:19:16.900956 python_roborock-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      165 2024-05-11 12:19:16.216947 python_roborock-2.2.1/roborock/__init__.py
+-rw-r--r--   0        0        0     4123 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/api.py
+-rw-r--r--   0        0        0     6826 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/cli.py
+-rw-r--r--   0        0        0     7144 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/cloud_api.py
+-rw-r--r--   0        0        0    14415 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/code_mappings.py
+-rw-r--r--   0        0        0     7912 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/command_cache.py
+-rw-r--r--   0        0        0     2386 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/const.py
+-rw-r--r--   0        0        0    27991 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/containers.py
+-rw-r--r--   0        0        0     1962 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/exceptions.py
+-rw-r--r--   0        0        0     4367 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/local_api.py
+-rw-r--r--   0        0        0    12315 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/protocol.py
+-rw-r--r--   0        0        0        0 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/py.typed
+-rw-r--r--   0        0        0      834 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/roborock_future.py
+-rw-r--r--   0        0        0     5464 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/roborock_message.py
+-rw-r--r--   0        0        0    23536 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/roborock_typing.py
+-rw-r--r--   0        0        0     3465 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/util.py
+-rw-r--r--   0        0        0      183 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/version_1_apis/__init__.py
+-rw-r--r--   0        0        0    20099 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/version_1_apis/roborock_client_v1.py
+-rw-r--r--   0        0        0     3477 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/version_1_apis/roborock_local_client_v1.py
+-rw-r--r--   0        0        0     3358 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/version_1_apis/roborock_mqtt_client_v1.py
+-rw-r--r--   0        0        0      111 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/version_a01_apis/__init__.py
+-rw-r--r--   0        0        0     7424 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/version_a01_apis/roborock_client_a01.py
+-rw-r--r--   0        0        0     3043 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/version_a01_apis/roborock_mqtt_client_a01.py
+-rw-r--r--   0        0        0    13040 2024-05-11 12:19:16.220947 python_roborock-2.2.1/roborock/web_api.py
+-rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 python_roborock-2.2.1/PKG-INFO
```

### Comparing `python_roborock-2.2.0/LICENSE` & `python_roborock-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/README.md` & `python_roborock-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/pyproject.toml` & `python_roborock-2.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "2.2.0"
+version = "2.2.1"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 documentation = "https://python-roborock.readthedocs.io/"
 classifiers = [
```

### Comparing `python_roborock-2.2.0/roborock/api.py` & `python_roborock-2.2.1/roborock/api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/cli.py` & `python_roborock-2.2.1/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/cloud_api.py` & `python_roborock-2.2.1/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/code_mappings.py` & `python_roborock-2.2.1/roborock/code_mappings.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,14 +319,15 @@
     custom_water_flow = 207
 
 
 class RoborockMopIntensityS8MaxVUltra(RoborockMopIntensityCode):
     off = 200
     low = 201
     medium = 202
+    high = 203
     smart_mode = 209
     custom_water_flow = 207
 
 
 class RoborockMopIntensityS5Max(RoborockMopIntensityCode):
     """Describes the mop intensity of the vacuum cleaner."""
```

### Comparing `python_roborock-2.2.0/roborock/command_cache.py` & `python_roborock-2.2.1/roborock/command_cache.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/const.py` & `python_roborock-2.2.1/roborock/const.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/containers.py` & `python_roborock-2.2.1/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/exceptions.py` & `python_roborock-2.2.1/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/local_api.py` & `python_roborock-2.2.1/roborock/local_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/protocol.py` & `python_roborock-2.2.1/roborock/protocol.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/roborock_future.py` & `python_roborock-2.2.1/roborock/roborock_future.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/roborock_message.py` & `python_roborock-2.2.1/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/roborock_typing.py` & `python_roborock-2.2.1/roborock/roborock_typing.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/util.py` & `python_roborock-2.2.1/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/version_1_apis/roborock_client_v1.py` & `python_roborock-2.2.1/roborock/version_1_apis/roborock_client_v1.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/version_1_apis/roborock_local_client_v1.py` & `python_roborock-2.2.1/roborock/version_1_apis/roborock_local_client_v1.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/version_1_apis/roborock_mqtt_client_v1.py` & `python_roborock-2.2.1/roborock/version_1_apis/roborock_mqtt_client_v1.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/version_a01_apis/roborock_client_a01.py` & `python_roborock-2.2.1/roborock/version_a01_apis/roborock_client_a01.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/version_a01_apis/roborock_mqtt_client_a01.py` & `python_roborock-2.2.1/roborock/version_a01_apis/roborock_mqtt_client_a01.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/roborock/web_api.py` & `python_roborock-2.2.1/roborock/web_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-2.2.0/PKG-INFO` & `python_roborock-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 2.2.0
+Version: 2.2.1
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Keywords: roborock,vacuum,homeassistant
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 2.2.0 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 2.2.1 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Keywords: roborock,vacuum,homeassistant
 Author: humbertogontijo Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
```

