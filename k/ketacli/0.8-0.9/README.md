# Comparing `tmp/ketacli-0.8.tar.gz` & `tmp/ketacli-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ketacli-0.8.tar", last modified: Fri Mar 15 02:50:44 2024, max compression
+gzip compressed data, was "ketacli-0.9.tar", last modified: Fri Mar 15 02:52:57 2024, max compression
```

## Comparing `ketacli-0.8.tar` & `ketacli-0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:50:44.918912 ketacli-0.8/
--rw-r--r--   0 cui       (1000) cui       (1000)     1146 2024-03-15 02:50:44.918912 ketacli-0.8/PKG-INFO
--rw-r--r--   0 cui       (1000) cui       (1000)      841 2024-03-14 09:31:57.000000 ketacli-0.8/README.md
-drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:50:44.908912 ketacli-0.8/ketacli/
--rw-r--r--   0 cui       (1000) cui       (1000)        0 2024-03-12 14:25:05.000000 ketacli-0.8/ketacli/__init__.py
--rw-r--r--   0 cui       (1000) cui       (1000)     6691 2024-03-14 10:15:36.000000 ketacli-0.8/ketacli/ketacli.py
-drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:50:44.908912 ketacli-0.8/ketacli/sdk/
--rw-r--r--   0 cui       (1000) cui       (1000)        0 2024-03-12 14:25:05.000000 ketacli-0.8/ketacli/sdk/__init__.py
-drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:50:44.908912 ketacli-0.8/ketacli/sdk/base/
--rw-r--r--   0 cui       (1000) cui       (1000)        0 2024-03-12 14:25:05.000000 ketacli-0.8/ketacli/sdk/base/__init__.py
--rw-r--r--   0 cui       (1000) cui       (1000)     4116 2024-03-14 09:12:07.000000 ketacli-0.8/ketacli/sdk/base/client.py
--rw-r--r--   0 cui       (1000) cui       (1000)     1707 2024-03-13 06:37:04.000000 ketacli-0.8/ketacli/sdk/base/search.py
-drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:50:44.918912 ketacli-0.8/ketacli/sdk/output/
--rw-r--r--   0 cui       (1000) cui       (1000)        0 2024-03-12 14:25:05.000000 ketacli-0.8/ketacli/sdk/output/__init__.py
--rw-r--r--   0 cui       (1000) cui       (1000)     2798 2024-03-14 08:00:50.000000 ketacli-0.8/ketacli/sdk/output/format.py
--rw-r--r--   0 cui       (1000) cui       (1000)     3061 2024-03-14 08:46:25.000000 ketacli-0.8/ketacli/sdk/output/output.py
-drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:50:44.918912 ketacli-0.8/ketacli/sdk/request/
--rw-r--r--   0 cui       (1000) cui       (1000)        0 2024-03-12 14:25:05.000000 ketacli-0.8/ketacli/sdk/request/__init__.py
--rw-r--r--   0 cui       (1000) cui       (1000)     5651 2024-03-15 02:48:19.000000 ketacli-0.8/ketacli/sdk/request/asset_map.py
--rw-r--r--   0 cui       (1000) cui       (1000)      475 2024-03-15 02:43:53.000000 ketacli-0.8/ketacli/sdk/request/create.py
--rw-r--r--   0 cui       (1000) cui       (1000)      602 2024-03-15 02:43:27.000000 ketacli-0.8/ketacli/sdk/request/get.py
--rw-r--r--   0 cui       (1000) cui       (1000)     1265 2024-03-14 10:02:05.000000 ketacli-0.8/ketacli/sdk/request/list.py
--rw-r--r--   0 cui       (1000) cui       (1000)      768 2024-03-12 14:25:05.000000 ketacli-0.8/ketacli/sdk/test.py
--rw-r--r--   0 cui       (1000) cui       (1000)      732 2024-03-13 02:56:47.000000 ketacli-0.8/ketacli/sdk/util.py
-drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:50:44.908912 ketacli-0.8/ketacli.egg-info/
--rw-r--r--   0 cui       (1000) cui       (1000)     1146 2024-03-15 02:50:44.000000 ketacli-0.8/ketacli.egg-info/PKG-INFO
--rw-r--r--   0 cui       (1000) cui       (1000)      631 2024-03-15 02:50:44.000000 ketacli-0.8/ketacli.egg-info/SOURCES.txt
--rw-r--r--   0 cui       (1000) cui       (1000)        1 2024-03-15 02:50:44.000000 ketacli-0.8/ketacli.egg-info/dependency_links.txt
--rw-r--r--   0 cui       (1000) cui       (1000)       49 2024-03-15 02:50:44.000000 ketacli-0.8/ketacli.egg-info/entry_points.txt
--rw-r--r--   0 cui       (1000) cui       (1000)       34 2024-03-15 02:50:44.000000 ketacli-0.8/ketacli.egg-info/requires.txt
--rw-r--r--   0 cui       (1000) cui       (1000)        8 2024-03-15 02:50:44.000000 ketacli-0.8/ketacli.egg-info/top_level.txt
--rw-r--r--   0 cui       (1000) cui       (1000)       38 2024-03-15 02:50:44.918912 ketacli-0.8/setup.cfg
--rw-r--r--   0 cui       (1000) cui       (1000)      587 2024-03-14 04:00:07.000000 ketacli-0.8/setup.py
+drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:52:57.895371 ketacli-0.9/
+-rw-r--r--   0 cui       (1000) cui       (1000)     1173 2024-03-15 02:52:57.895371 ketacli-0.9/PKG-INFO
+-rw-r--r--   0 cui       (1000) cui       (1000)      841 2024-03-14 09:31:57.000000 ketacli-0.9/README.md
+drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:52:57.885371 ketacli-0.9/ketacli/
+-rw-r--r--   0 cui       (1000) cui       (1000)        0 2024-03-12 14:25:05.000000 ketacli-0.9/ketacli/__init__.py
+-rw-r--r--   0 cui       (1000) cui       (1000)     6691 2024-03-14 10:15:36.000000 ketacli-0.9/ketacli/ketacli.py
+drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:52:57.895371 ketacli-0.9/ketacli/sdk/
+-rw-r--r--   0 cui       (1000) cui       (1000)        0 2024-03-12 14:25:05.000000 ketacli-0.9/ketacli/sdk/__init__.py
+drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:52:57.895371 ketacli-0.9/ketacli/sdk/base/
+-rw-r--r--   0 cui       (1000) cui       (1000)        0 2024-03-12 14:25:05.000000 ketacli-0.9/ketacli/sdk/base/__init__.py
+-rw-r--r--   0 cui       (1000) cui       (1000)     4116 2024-03-14 09:12:07.000000 ketacli-0.9/ketacli/sdk/base/client.py
+-rw-r--r--   0 cui       (1000) cui       (1000)     1707 2024-03-13 06:37:04.000000 ketacli-0.9/ketacli/sdk/base/search.py
+drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:52:57.895371 ketacli-0.9/ketacli/sdk/output/
+-rw-r--r--   0 cui       (1000) cui       (1000)        0 2024-03-12 14:25:05.000000 ketacli-0.9/ketacli/sdk/output/__init__.py
+-rw-r--r--   0 cui       (1000) cui       (1000)     2798 2024-03-14 08:00:50.000000 ketacli-0.9/ketacli/sdk/output/format.py
+-rw-r--r--   0 cui       (1000) cui       (1000)     3061 2024-03-14 08:46:25.000000 ketacli-0.9/ketacli/sdk/output/output.py
+drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:52:57.895371 ketacli-0.9/ketacli/sdk/request/
+-rw-r--r--   0 cui       (1000) cui       (1000)        0 2024-03-12 14:25:05.000000 ketacli-0.9/ketacli/sdk/request/__init__.py
+-rw-r--r--   0 cui       (1000) cui       (1000)     5651 2024-03-15 02:48:19.000000 ketacli-0.9/ketacli/sdk/request/asset_map.py
+-rw-r--r--   0 cui       (1000) cui       (1000)      475 2024-03-15 02:43:53.000000 ketacli-0.9/ketacli/sdk/request/create.py
+-rw-r--r--   0 cui       (1000) cui       (1000)      602 2024-03-15 02:43:27.000000 ketacli-0.9/ketacli/sdk/request/get.py
+-rw-r--r--   0 cui       (1000) cui       (1000)     1265 2024-03-14 10:02:05.000000 ketacli-0.9/ketacli/sdk/request/list.py
+-rw-r--r--   0 cui       (1000) cui       (1000)      768 2024-03-12 14:25:05.000000 ketacli-0.9/ketacli/sdk/test.py
+-rw-r--r--   0 cui       (1000) cui       (1000)      732 2024-03-13 02:56:47.000000 ketacli-0.9/ketacli/sdk/util.py
+drwxr-xr-x   0 cui       (1000) cui       (1000)        0 2024-03-15 02:52:57.885371 ketacli-0.9/ketacli.egg-info/
+-rw-r--r--   0 cui       (1000) cui       (1000)     1173 2024-03-15 02:52:57.000000 ketacli-0.9/ketacli.egg-info/PKG-INFO
+-rw-r--r--   0 cui       (1000) cui       (1000)      631 2024-03-15 02:52:57.000000 ketacli-0.9/ketacli.egg-info/SOURCES.txt
+-rw-r--r--   0 cui       (1000) cui       (1000)        1 2024-03-15 02:52:57.000000 ketacli-0.9/ketacli.egg-info/dependency_links.txt
+-rw-r--r--   0 cui       (1000) cui       (1000)       49 2024-03-15 02:52:57.000000 ketacli-0.9/ketacli.egg-info/entry_points.txt
+-rw-r--r--   0 cui       (1000) cui       (1000)       46 2024-03-15 02:52:57.000000 ketacli-0.9/ketacli.egg-info/requires.txt
+-rw-r--r--   0 cui       (1000) cui       (1000)        8 2024-03-15 02:52:57.000000 ketacli-0.9/ketacli.egg-info/top_level.txt
+-rw-r--r--   0 cui       (1000) cui       (1000)       38 2024-03-15 02:52:57.895371 ketacli-0.9/setup.cfg
+-rw-r--r--   0 cui       (1000) cui       (1000)      610 2024-03-15 02:52:31.000000 ketacli-0.9/setup.py
```

### Comparing `ketacli-0.8/PKG-INFO` & `ketacli-0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ketacli
-Version: 0.8
+Version: 0.9
 Summary: KetaDB Client
 Home-page: https://xishuhq.com
 Author: lvheyang
 Author-email: cuiwenzheng@ymail.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: prettytable
 Requires-Dist: pyyaml
 Requires-Dist: mando
+Requires-Dist: argcomplete
 
 # ketadb 工具
 
 ## 示例
 
 ```shell
 ketacli login --name <username> --endpoint http://localhost:9000 --token <yourtoken>
```

### Comparing `ketacli-0.8/README.md` & `ketacli-0.9/README.md`

 * *Files identical despite different names*

### Comparing `ketacli-0.8/ketacli/ketacli.py` & `ketacli-0.9/ketacli/ketacli.py`

 * *Files identical despite different names*

### Comparing `ketacli-0.8/ketacli/sdk/base/client.py` & `ketacli-0.9/ketacli/sdk/base/client.py`

 * *Files identical despite different names*

### Comparing `ketacli-0.8/ketacli/sdk/base/search.py` & `ketacli-0.9/ketacli/sdk/base/search.py`

 * *Files identical despite different names*

### Comparing `ketacli-0.8/ketacli/sdk/output/format.py` & `ketacli-0.9/ketacli/sdk/output/format.py`

 * *Files identical despite different names*

### Comparing `ketacli-0.8/ketacli/sdk/output/output.py` & `ketacli-0.9/ketacli/sdk/output/output.py`

 * *Files identical despite different names*

### Comparing `ketacli-0.8/ketacli/sdk/request/asset_map.py` & `ketacli-0.9/ketacli/sdk/request/asset_map.py`

 * *Files identical despite different names*

### Comparing `ketacli-0.8/ketacli/sdk/request/get.py` & `ketacli-0.9/ketacli/sdk/request/get.py`

 * *Files identical despite different names*

### Comparing `ketacli-0.8/ketacli/sdk/request/list.py` & `ketacli-0.9/ketacli/sdk/request/list.py`

 * *Files identical despite different names*

### Comparing `ketacli-0.8/ketacli/sdk/test.py` & `ketacli-0.9/ketacli/sdk/test.py`

 * *Files identical despite different names*

### Comparing `ketacli-0.8/ketacli/sdk/util.py` & `ketacli-0.9/ketacli/sdk/util.py`

 * *Files identical despite different names*

### Comparing `ketacli-0.8/ketacli.egg-info/PKG-INFO` & `ketacli-0.9/ketacli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ketacli
-Version: 0.8
+Version: 0.9
 Summary: KetaDB Client
 Home-page: https://xishuhq.com
 Author: lvheyang
 Author-email: cuiwenzheng@ymail.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: prettytable
 Requires-Dist: pyyaml
 Requires-Dist: mando
+Requires-Dist: argcomplete
 
 # ketadb 工具
 
 ## 示例
 
 ```shell
 ketacli login --name <username> --endpoint http://localhost:9000 --token <yourtoken>
```

### Comparing `ketacli-0.8/ketacli.egg-info/SOURCES.txt` & `ketacli-0.9/ketacli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ketacli-0.8/setup.py` & `ketacli-0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ketacli',
-    version='0.8',
+    version='0.9',
     packages=find_packages(),
     license='MIT',
     description='KetaDB Client',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='lvheyang',
     author_email='cuiwenzheng@ymail.com',
     url='https://xishuhq.com',
     install_requires=[
         "requests",
         "prettytable",
         "pyyaml",
         "mando",
+        "argcomplete",
     ],
     entry_points={
         'console_scripts': [
             'ketacli=ketacli.ketacli:main',
         ],
     },
 )
```

