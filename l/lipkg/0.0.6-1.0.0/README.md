# Comparing `tmp/lipkg-0.0.6.tar.gz` & `tmp/lipkg-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lipkg-0.0.6.tar", last modified: Sun Mar 10 15:03:08 2024, max compression
+gzip compressed data, was "lipkg-1.0.0.tar", last modified: Sat May 11 19:46:54 2024, max compression
```

## Comparing `lipkg-0.0.6.tar` & `lipkg-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,16 @@
-drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-03-10 15:03:08.635592 lipkg-0.0.6/
--rw-r--r--   0 lizhankang   (501) staff       (20)     1091 2024-02-27 09:03:31.000000 lipkg-0.0.6/LICENSE
--rw-r--r--   0 lizhankang   (501) staff       (20)      968 2024-03-10 15:03:08.635383 lipkg-0.0.6/PKG-INFO
--rw-r--r--   0 lizhankang   (501) staff       (20)      346 2024-02-28 08:50:32.000000 lipkg-0.0.6/README.md
--rw-r--r--   0 lizhankang   (501) staff       (20)      725 2024-03-10 15:02:56.000000 lipkg-0.0.6/pyproject.toml
--rw-r--r--   0 lizhankang   (501) staff       (20)       38 2024-03-10 15:03:08.635653 lipkg-0.0.6/setup.cfg
-drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-03-10 15:03:08.628991 lipkg-0.0.6/src/
-drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-03-10 15:03:08.630518 lipkg-0.0.6/src/lipkg/
--rw-r--r--   0 lizhankang   (501) staff       (20)      986 2024-03-10 15:02:19.000000 lipkg-0.0.6/src/lipkg/__init__.py
-drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-03-10 15:03:08.631810 lipkg-0.0.6/src/lipkg/http/
--rw-r--r--   0 lizhankang   (501) staff       (20)       26 2024-02-28 08:50:32.000000 lipkg-0.0.6/src/lipkg/http/__init__.py
--rw-r--r--   0 lizhankang   (501) staff       (20)      127 2024-02-28 08:50:32.000000 lipkg-0.0.6/src/lipkg/http/api.py
-drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-03-10 15:03:08.633154 lipkg-0.0.6/src/lipkg/pack/
--rw-r--r--   0 lizhankang   (501) staff       (20)      702 2024-02-27 09:03:31.000000 lipkg-0.0.6/src/lipkg/pack/__init__.py
--rw-r--r--   0 lizhankang   (501) staff       (20)      161 2024-02-27 09:03:31.000000 lipkg-0.0.6/src/lipkg/pack/dog.py
-drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-03-10 15:03:08.633998 lipkg-0.0.6/src/lipkg/pack/game/
--rw-r--r--   0 lizhankang   (501) staff       (20)       45 2024-02-27 09:03:31.000000 lipkg-0.0.6/src/lipkg/pack/game/__init__.py
-drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-03-10 15:03:08.634182 lipkg-0.0.6/src/lipkg/pack/game/chiji/
--rw-r--r--   0 lizhankang   (501) staff       (20)       94 2024-02-27 09:03:31.000000 lipkg-0.0.6/src/lipkg/pack/game/chiji/__init__.py
-drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-03-10 15:03:08.634372 lipkg-0.0.6/src/lipkg/pack/game/csgo2/
--rw-r--r--   0 lizhankang   (501) staff       (20)       47 2024-02-27 09:03:31.000000 lipkg-0.0.6/src/lipkg/pack/game/csgo2/__init__.py
--rw-r--r--   0 lizhankang   (501) staff       (20)       71 2024-02-27 09:03:31.000000 lipkg-0.0.6/src/lipkg/pack/game/dou_di_zhu.py
--rw-r--r--   0 lizhankang   (501) staff       (20)      138 2024-02-27 09:03:31.000000 lipkg-0.0.6/src/lipkg/pack/game/yxlm.py
--rw-r--r--   0 lizhankang   (501) staff       (20)      157 2024-02-27 09:03:31.000000 lipkg-0.0.6/src/lipkg/pack/human.py
-drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-03-10 15:03:08.634597 lipkg-0.0.6/src/lipkg/pack/learn/
--rw-r--r--   0 lizhankang   (501) staff       (20)      108 2024-02-27 09:03:31.000000 lipkg-0.0.6/src/lipkg/pack/learn/__init__.py
-drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-03-10 15:03:08.634806 lipkg-0.0.6/src/lipkg/pack/learn/chinese/
--rw-r--r--   0 lizhankang   (501) staff       (20)        0 2024-02-27 09:03:31.000000 lipkg-0.0.6/src/lipkg/pack/learn/chinese/__init__.py
-drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-03-10 15:03:08.634913 lipkg-0.0.6/src/lipkg/pack/learn/english/
--rw-r--r--   0 lizhankang   (501) staff       (20)       41 2024-02-27 09:03:31.000000 lipkg-0.0.6/src/lipkg/pack/learn/english/__init__.py
--rw-r--r--   0 lizhankang   (501) staff       (20)     4317 2024-03-05 05:35:54.000000 lipkg-0.0.6/src/lipkg/rsa.py
-drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-03-10 15:03:08.635131 lipkg-0.0.6/src/lipkg.egg-info/
--rw-r--r--   0 lizhankang   (501) staff       (20)      968 2024-03-10 15:03:08.000000 lipkg-0.0.6/src/lipkg.egg-info/PKG-INFO
--rw-r--r--   0 lizhankang   (501) staff       (20)      642 2024-03-10 15:03:08.000000 lipkg-0.0.6/src/lipkg.egg-info/SOURCES.txt
--rw-r--r--   0 lizhankang   (501) staff       (20)        1 2024-03-10 15:03:08.000000 lipkg-0.0.6/src/lipkg.egg-info/dependency_links.txt
--rw-r--r--   0 lizhankang   (501) staff       (20)       57 2024-03-10 15:03:08.000000 lipkg-0.0.6/src/lipkg.egg-info/requires.txt
--rw-r--r--   0 lizhankang   (501) staff       (20)        6 2024-03-10 15:03:08.000000 lipkg-0.0.6/src/lipkg.egg-info/top_level.txt
+drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-05-11 19:46:54.154329 lipkg-1.0.0/
+-rw-r--r--   0 lizhankang   (501) staff       (20)     1091 2024-05-11 19:13:14.000000 lipkg-1.0.0/LICENSE
+-rw-r--r--   0 lizhankang   (501) staff       (20)      959 2024-05-11 19:46:54.154173 lipkg-1.0.0/PKG-INFO
+-rw-r--r--   0 lizhankang   (501) staff       (20)      346 2024-05-11 19:13:14.000000 lipkg-1.0.0/README.md
+-rw-r--r--   0 lizhankang   (501) staff       (20)      716 2024-05-11 19:38:58.000000 lipkg-1.0.0/pyproject.toml
+-rw-r--r--   0 lizhankang   (501) staff       (20)       38 2024-05-11 19:46:54.154364 lipkg-1.0.0/setup.cfg
+drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-05-11 19:46:54.152497 lipkg-1.0.0/src/
+drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-05-11 19:46:54.153246 lipkg-1.0.0/src/lipkg/
+-rw-r--r--   0 lizhankang   (501) staff       (20)      984 2024-05-11 19:13:14.000000 lipkg-1.0.0/src/lipkg/__init__.py
+-rw-r--r--   0 lizhankang   (501) staff       (20)     1293 2024-05-11 19:38:58.000000 lipkg-1.0.0/src/lipkg/rsa.py
+drwxr-xr-x   0 lizhankang   (501) staff       (20)        0 2024-05-11 19:46:54.154028 lipkg-1.0.0/src/lipkg.egg-info/
+-rw-r--r--   0 lizhankang   (501) staff       (20)      959 2024-05-11 19:46:54.000000 lipkg-1.0.0/src/lipkg.egg-info/PKG-INFO
+-rw-r--r--   0 lizhankang   (501) staff       (20)      235 2024-05-11 19:46:54.000000 lipkg-1.0.0/src/lipkg.egg-info/SOURCES.txt
+-rw-r--r--   0 lizhankang   (501) staff       (20)        1 2024-05-11 19:46:54.000000 lipkg-1.0.0/src/lipkg.egg-info/dependency_links.txt
+-rw-r--r--   0 lizhankang   (501) staff       (20)       57 2024-05-11 19:46:54.000000 lipkg-1.0.0/src/lipkg.egg-info/requires.txt
+-rw-r--r--   0 lizhankang   (501) staff       (20)        6 2024-05-11 19:46:54.000000 lipkg-1.0.0/src/lipkg.egg-info/top_level.txt
```

### Comparing `lipkg-0.0.6/LICENSE` & `lipkg-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lipkg-0.0.6/PKG-INFO` & `lipkg-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lipkg
-Version: 0.0.6
+Version: 1.0.0
 Summary: A small example package
-Author-email: li zhankang <lizhankangde@outlook.com>
+Author-email: lipu <lizhankangde@gmail.com>
 Project-URL: Homepage, https://github.com/lizhankang/python-sdk
 Project-URL: Issues, https://github.com/lizhankang/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `lipkg-0.0.6/pyproject.toml` & `lipkg-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "lipkg"
-version = "0.0.6"
+version = "1.0.0"
 authors = [
-  { name="li zhankang", email="lizhankangde@outlook.com" },
+  { name="lipu", email="lizhankangde@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `lipkg-0.0.6/src/lipkg/__init__.py` & `lipkg-1.0.0/src/lipkg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# from . import pack
+from . import pack
 from . import rsa
 from . import http
 import json
 import requests
 
 
 # 读取JSON文件
```

### Comparing `lipkg-0.0.6/src/lipkg.egg-info/PKG-INFO` & `lipkg-1.0.0/src/lipkg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lipkg
-Version: 0.0.6
+Version: 1.0.0
 Summary: A small example package
-Author-email: li zhankang <lizhankangde@outlook.com>
+Author-email: lipu <lizhankangde@gmail.com>
 Project-URL: Homepage, https://github.com/lizhankang/python-sdk
 Project-URL: Issues, https://github.com/lizhankang/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

