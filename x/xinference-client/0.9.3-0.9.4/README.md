# Comparing `tmp/xinference-client-0.9.3.tar.gz` & `tmp/xinference-client-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xinference-client-0.9.3.tar", last modified: Fri Mar 15 06:40:38 2024, max compression
+gzip compressed data, was "xinference-client-0.9.4.tar", last modified: Thu Mar 21 07:10:33 2024, max compression
```

## Comparing `xinference-client-0.9.3.tar` & `xinference-client-0.9.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:40:38.623671 xinference-client-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-15 06:40:33.000000 xinference-client-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-15 06:40:33.000000 xinference-client-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-03-15 06:40:38.623671 xinference-client-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-15 06:40:33.000000 xinference-client-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-15 06:40:33.000000 xinference-client-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-15 06:40:38.623671 xinference-client-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-03-15 06:40:33.000000 xinference-client-0.9.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-03-15 06:40:33.000000 xinference-client-0.9.3/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:40:38.623671 xinference-client-0.9.3/xinference_client/
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-15 06:40:33.000000 xinference-client-0.9.3/xinference_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-03-15 06:40:34.000000 xinference-client-0.9.3/xinference_client/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-15 06:40:38.623671 xinference-client-0.9.3/xinference_client/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:40:38.623671 xinference-client-0.9.3/xinference_client/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:40:38.000000 xinference-client-0.9.3/xinference_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-15 06:40:34.000000 xinference-client-0.9.3/xinference_client/client/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:40:38.623671 xinference-client-0.9.3/xinference_client/client/restful/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-15 06:40:34.000000 xinference-client-0.9.3/xinference_client/client/restful/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41044 2024-03-15 06:40:34.000000 xinference-client-0.9.3/xinference_client/client/restful/restful_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-03-15 06:40:34.000000 xinference-client-0.9.3/xinference_client/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    11812 2024-03-15 06:40:34.000000 xinference-client-0.9.3/xinference_client/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:40:38.623671 xinference-client-0.9.3/xinference_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-03-15 06:40:38.000000 xinference-client-0.9.3/xinference_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-15 06:40:38.000000 xinference-client-0.9.3/xinference_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 06:40:38.000000 xinference-client-0.9.3/xinference_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 06:40:38.000000 xinference-client-0.9.3/xinference_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-15 06:40:38.000000 xinference-client-0.9.3/xinference_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-15 06:40:38.000000 xinference-client-0.9.3/xinference_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 07:10:33.322747 xinference-client-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-21 07:10:28.000000 xinference-client-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-21 07:10:28.000000 xinference-client-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-03-21 07:10:33.322747 xinference-client-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-21 07:10:28.000000 xinference-client-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-21 07:10:28.000000 xinference-client-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-21 07:10:33.326747 xinference-client-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-03-21 07:10:28.000000 xinference-client-0.9.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-03-21 07:10:28.000000 xinference-client-0.9.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 07:10:33.322747 xinference-client-0.9.4/xinference_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-21 07:10:28.000000 xinference-client-0.9.4/xinference_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-03-21 07:10:29.000000 xinference-client-0.9.4/xinference_client/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-21 07:10:33.326747 xinference-client-0.9.4/xinference_client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 07:10:33.322747 xinference-client-0.9.4/xinference_client/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 07:10:33.000000 xinference-client-0.9.4/xinference_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-21 07:10:29.000000 xinference-client-0.9.4/xinference_client/client/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 07:10:33.322747 xinference-client-0.9.4/xinference_client/client/restful/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-21 07:10:29.000000 xinference-client-0.9.4/xinference_client/client/restful/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41044 2024-03-21 07:10:29.000000 xinference-client-0.9.4/xinference_client/client/restful/restful_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-03-21 07:10:29.000000 xinference-client-0.9.4/xinference_client/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11812 2024-03-21 07:10:29.000000 xinference-client-0.9.4/xinference_client/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 07:10:33.322747 xinference-client-0.9.4/xinference_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-03-21 07:10:33.000000 xinference-client-0.9.4/xinference_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-21 07:10:33.000000 xinference-client-0.9.4/xinference_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 07:10:33.000000 xinference-client-0.9.4/xinference_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 07:10:32.000000 xinference-client-0.9.4/xinference_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-21 07:10:33.000000 xinference-client-0.9.4/xinference_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-21 07:10:33.000000 xinference-client-0.9.4/xinference_client.egg-info/top_level.txt
```

### Comparing `xinference-client-0.9.3/LICENSE` & `xinference-client-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xinference-client-0.9.3/PKG-INFO` & `xinference-client-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xinference-client
-Version: 0.9.3
+Version: 0.9.4
 Summary: Client for Xinference
 Home-page: https://github.com/xorbitsai/inference-client
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
```

### Comparing `xinference-client-0.9.3/README.md` & `xinference-client-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `xinference-client-0.9.3/setup.cfg` & `xinference-client-0.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `xinference-client-0.9.3/setup.py` & `xinference-client-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `xinference-client-0.9.3/versioneer.py` & `xinference-client-0.9.4/versioneer.py`

 * *Files identical despite different names*

### Comparing `xinference-client-0.9.3/xinference_client/__init__.py` & `xinference-client-0.9.4/xinference_client/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-client-0.9.3/xinference_client/_compat.py` & `xinference-client-0.9.4/xinference_client/_compat.py`

 * *Files identical despite different names*

### Comparing `xinference-client-0.9.3/xinference_client/client/common.py` & `xinference-client-0.9.4/xinference_client/client/common.py`

 * *Files identical despite different names*

### Comparing `xinference-client-0.9.3/xinference_client/client/restful/__init__.py` & `xinference-client-0.9.4/xinference_client/client/restful/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-client-0.9.3/xinference_client/client/restful/restful_client.py` & `xinference-client-0.9.4/xinference_client/client/restful/restful_client.py`

 * *Files identical despite different names*

### Comparing `xinference-client-0.9.3/xinference_client/fields.py` & `xinference-client-0.9.4/xinference_client/fields.py`

 * *Files identical despite different names*

### Comparing `xinference-client-0.9.3/xinference_client/types.py` & `xinference-client-0.9.4/xinference_client/types.py`

 * *Files identical despite different names*

### Comparing `xinference-client-0.9.3/xinference_client.egg-info/PKG-INFO` & `xinference-client-0.9.4/xinference_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xinference-client
-Version: 0.9.3
+Version: 0.9.4
 Summary: Client for Xinference
 Home-page: https://github.com/xorbitsai/inference-client
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
```

### Comparing `xinference-client-0.9.3/xinference_client.egg-info/SOURCES.txt` & `xinference-client-0.9.4/xinference_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

