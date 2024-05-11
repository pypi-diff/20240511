# Comparing `tmp/vdg-0.1.3.tar.gz` & `tmp/vdg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdg-0.1.3.tar", last modified: Sat May 11 10:47:29 2024, max compression
+gzip compressed data, was "vdg-0.2.0.tar", last modified: Sat May 11 10:55:39 2024, max compression
```

## Comparing `vdg-0.1.3.tar` & `vdg-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:47:29.938262 vdg-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-11 10:47:27.000000 vdg-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-11 10:47:27.000000 vdg-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-11 10:47:29.938262 vdg-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-11 10:47:27.000000 vdg-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 10:47:29.938262 vdg-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-11 10:47:27.000000 vdg-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:47:29.938262 vdg-0.1.3/vdg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 10:47:27.000000 vdg-0.1.3/vdg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-11 10:47:27.000000 vdg-0.1.3/vdg/core.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1019 2024-05-11 10:47:27.000000 vdg-0.1.3/vdg/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:47:29.938262 vdg-0.1.3/vdg/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-11 10:47:27.000000 vdg-0.1.3/vdg/templates/html.template
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-11 10:47:27.000000 vdg-0.1.3/vdg/templates/main.template
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-11 10:47:27.000000 vdg-0.1.3/vdg/templates/titles.template
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-11 10:47:27.000000 vdg-0.1.3/vdg/templates/yaml.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:47:29.938262 vdg-0.1.3/vdg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-11 10:47:29.000000 vdg-0.1.3/vdg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-11 10:47:29.000000 vdg-0.1.3/vdg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 10:47:29.000000 vdg-0.1.3/vdg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 10:47:29.000000 vdg-0.1.3/vdg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-11 10:47:29.000000 vdg-0.1.3/vdg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:39.630514 vdg-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-11 10:55:36.000000 vdg-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-11 10:55:36.000000 vdg-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-11 10:55:39.630514 vdg-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-11 10:55:36.000000 vdg-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 10:55:39.630514 vdg-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-11 10:55:36.000000 vdg-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:39.626514 vdg-0.2.0/vdg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/core.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1019 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:39.626514 vdg-0.2.0/vdg/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/templates/html.template
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/templates/main.template
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/templates/titles.template
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-11 10:55:36.000000 vdg-0.2.0/vdg/templates/yaml.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:55:39.626514 vdg-0.2.0/vdg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-11 10:55:39.000000 vdg-0.2.0/vdg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-11 10:55:39.000000 vdg-0.2.0/vdg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 10:55:39.000000 vdg-0.2.0/vdg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 10:55:39.000000 vdg-0.2.0/vdg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-11 10:55:39.000000 vdg-0.2.0/vdg.egg-info/top_level.txt
```

### Comparing `vdg-0.1.3/LICENSE` & `vdg-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vdg-0.1.3/PKG-INFO` & `vdg-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdg
-Version: 0.1.3
+Version: 0.2.0
 Summary: VCB-Studio Draft Generator 发布稿生成器
 Author: diazchika
 Author-email: halberd-civic.0c@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `vdg-0.1.3/README.md` & `vdg-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vdg-0.1.3/setup.py` & `vdg-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="vdg",
-    version="0.1.3",
+    version="0.2.0",
     author="diazchika",
     author_email="halberd-civic.0c@icloud.com",
     description="VCB-Studio Draft Generator 发布稿生成器",
     long_description=read('README.md'),
     packages=find_packages(),
     include_package_data=True,
     package_data={
```

### Comparing `vdg-0.1.3/vdg/core.py` & `vdg-0.2.0/vdg/core.py`

 * *Files identical despite different names*

### Comparing `vdg-0.1.3/vdg/main.py` & `vdg-0.2.0/vdg/main.py`

 * *Files identical despite different names*

### Comparing `vdg-0.1.3/vdg/templates/html.template` & `vdg-0.2.0/vdg/templates/html.template`

 * *Files identical despite different names*

### Comparing `vdg-0.1.3/vdg/templates/main.template` & `vdg-0.2.0/vdg/templates/main.template`

 * *Files identical despite different names*

### Comparing `vdg-0.1.3/vdg/templates/yaml.template` & `vdg-0.2.0/vdg/templates/yaml.template`

 * *Files identical despite different names*

### Comparing `vdg-0.1.3/vdg.egg-info/PKG-INFO` & `vdg-0.2.0/vdg.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdg
-Version: 0.1.3
+Version: 0.2.0
 Summary: VCB-Studio Draft Generator 发布稿生成器
 Author: diazchika
 Author-email: halberd-civic.0c@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

