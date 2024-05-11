# Comparing `tmp/shipper_shippy-2.36.8.tar.gz` & `tmp/shipper_shippy-2.37.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper_shippy-2.36.8.tar", last modified: Mon May  6 08:38:17 2024, max compression
+gzip compressed data, was "shipper_shippy-2.37.0.tar", last modified: Sat May 11 11:40:42 2024, max compression
```

## Comparing `shipper_shippy-2.36.8.tar` & `shipper_shippy-2.37.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:38:16.998952 shipper_shippy-2.36.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-06 08:38:16.994952 shipper_shippy-2.36.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-06 08:38:07.000000 shipper_shippy-2.36.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-06 08:38:07.000000 shipper_shippy-2.36.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 08:38:16.998952 shipper_shippy-2.36.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-06 08:38:07.000000 shipper_shippy-2.36.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:38:16.994952 shipper_shippy-2.36.8/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-06 08:38:16.000000 shipper_shippy-2.36.8/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-06 08:38:16.000000 shipper_shippy-2.36.8/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 08:38:16.000000 shipper_shippy-2.36.8/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-06 08:38:16.000000 shipper_shippy-2.36.8/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-06 08:38:16.000000 shipper_shippy-2.36.8/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 08:38:16.000000 shipper_shippy-2.36.8/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 08:38:16.994952 shipper_shippy-2.36.8/shippy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 08:38:07.000000 shipper_shippy-2.36.8/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-05-06 08:38:07.000000 shipper_shippy-2.36.8/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-05-06 08:38:07.000000 shipper_shippy-2.36.8/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-06 08:38:07.000000 shipper_shippy-2.36.8/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-06 08:38:07.000000 shipper_shippy-2.36.8/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 08:38:07.000000 shipper_shippy-2.36.8/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-06 08:38:07.000000 shipper_shippy-2.36.8/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-06 08:38:07.000000 shipper_shippy-2.36.8/shippy/server_compat_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 08:38:07.000000 shipper_shippy-2.36.8/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:40:42.708657 shipper_shippy-2.37.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-11 11:40:42.708657 shipper_shippy-2.37.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-11 11:40:35.000000 shipper_shippy-2.37.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-11 11:40:35.000000 shipper_shippy-2.37.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 11:40:42.708657 shipper_shippy-2.37.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-11 11:40:35.000000 shipper_shippy-2.37.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:40:42.704657 shipper_shippy-2.37.0/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-11 11:40:42.000000 shipper_shippy-2.37.0/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-11 11:40:42.000000 shipper_shippy-2.37.0/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 11:40:42.000000 shipper_shippy-2.37.0/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-11 11:40:42.000000 shipper_shippy-2.37.0/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-11 11:40:42.000000 shipper_shippy-2.37.0/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 11:40:42.000000 shipper_shippy-2.37.0/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:40:42.704657 shipper_shippy-2.37.0/shippy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 11:40:35.000000 shipper_shippy-2.37.0/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-05-11 11:40:35.000000 shipper_shippy-2.37.0/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13935 2024-05-11 11:40:35.000000 shipper_shippy-2.37.0/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-11 11:40:35.000000 shipper_shippy-2.37.0/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-11 11:40:35.000000 shipper_shippy-2.37.0/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-11 11:40:35.000000 shipper_shippy-2.37.0/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-11 11:40:35.000000 shipper_shippy-2.37.0/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-11 11:40:35.000000 shipper_shippy-2.37.0/shippy/server_compat_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 11:40:35.000000 shipper_shippy-2.37.0/shippy/version.py
```

### Comparing `shipper_shippy-2.36.8/PKG-INFO` & `shipper_shippy-2.37.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.36.8
+Version: 2.37.0
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/shipperstack/shipper/tree/master/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/shipperstack/shipper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: humanize==4.9.0
 Requires-Dist: loguru==0.7.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: semver==3.0.2
-Requires-Dist: sentry-sdk==2.0.1
+Requires-Dist: sentry-sdk==2.1.1
 Requires-Dist: setuptools==69.5.1
 
 # shippy
 
 [
 ![PyPI](https://img.shields.io/pypi/v/shipper-shippy)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/shipper-shippy)
```

### Comparing `shipper_shippy-2.36.8/README.md` & `shipper_shippy-2.37.0/README.md`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.8/setup.py` & `shipper_shippy-2.37.0/setup.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.8/shipper_shippy.egg-info/PKG-INFO` & `shipper_shippy-2.37.0/shipper_shippy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.36.8
+Version: 2.37.0
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/shipperstack/shipper/tree/master/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/shipperstack/shipper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: humanize==4.9.0
 Requires-Dist: loguru==0.7.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: semver==3.0.2
-Requires-Dist: sentry-sdk==2.0.1
+Requires-Dist: sentry-sdk==2.1.1
 Requires-Dist: setuptools==69.5.1
 
 # shippy
 
 [
 ![PyPI](https://img.shields.io/pypi/v/shipper-shippy)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/shipper-shippy)
```

### Comparing `shipper_shippy-2.36.8/shippy/__main__.py` & `shipper_shippy-2.37.0/shippy/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,14 +248,22 @@
 
         return builds
 
 
 def check_build(client, filename):
     """Makes sure the build is valid"""
     print(f"Validating build {filename}...")
+
+    # Check if the build already exists on the server
+    if client.duplicate_check(file_name=filename):
+        print_warning(
+            "This build already exists on the server. ", newline=False
+        )
+        return False
+
     # Validate that there is a matching checksum file
     has_checksum_file_type, has_sum_postfix = find_checksum_file(filename=filename)
 
     if has_checksum_file_type is None:
         print_warning(
             "This build does not have a matching checksum file. ", newline=False
         )
```

### Comparing `shipper_shippy-2.36.8/shippy/client.py` & `shipper_shippy-2.37.0/shippy/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,14 +136,18 @@
 
     def get_shippy_compat_version(self):
         return semver.VersionInfo.parse(self._get_info()["shippy_compat_version"])
 
     def get_shippy_upload_variants(self):
         return self._get_info()["shippy_upload_variants"]
 
+    def duplicate_check(self, file_name):
+        r = self._post(url="/api/v1/maintainers/build/duplicate_check/", data={"file_name": file_name})
+        return r.json()["exists"] == "true"
+
     def _get_info(self):
         r = self._get(url="/api/v2/system/info")
         if r.status_code == 200:
             return r.json()
         else:
             raise Exception(FAILED_TO_RETRIEVE_SERVER_VERSION_ERROR_MSG)
```

### Comparing `shipper_shippy-2.36.8/shippy/config.py` & `shipper_shippy-2.37.0/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.8/shippy/constants.py` & `shipper_shippy-2.37.0/shippy/constants.py`

 * *Files identical despite different names*

### Comparing `shipper_shippy-2.36.8/shippy/helper.py` & `shipper_shippy-2.37.0/shippy/helper.py`

 * *Files identical despite different names*

