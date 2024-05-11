# Comparing `tmp/dearwatson-0.9.7.tar.gz` & `tmp/dearwatson-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dearwatson-0.9.7.tar", last modified: Mon Jan 29 16:01:40 2024, max compression
+gzip compressed data, was "dearwatson-0.9.9.tar", last modified: Fri May  3 18:47:47 2024, max compression
```

## Comparing `dearwatson-0.9.7.tar` & `dearwatson-0.9.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:01:40.880061 dearwatson-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-29 16:01:29.000000 dearwatson-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-29 16:01:29.000000 dearwatson-0.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-01-29 16:01:40.880061 dearwatson-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-01-29 16:01:29.000000 dearwatson-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:01:40.876061 dearwatson-0.9.7/dearwatson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-01-29 16:01:40.000000 dearwatson-0.9.7/dearwatson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-29 16:01:40.000000 dearwatson-0.9.7/dearwatson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 16:01:40.000000 dearwatson-0.9.7/dearwatson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-29 16:01:40.000000 dearwatson-0.9.7/dearwatson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-29 16:01:40.000000 dearwatson-0.9.7/dearwatson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 16:01:40.880061 dearwatson-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-01-29 16:01:30.000000 dearwatson-0.9.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-29 16:01:30.000000 dearwatson-0.9.7/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:01:40.876061 dearwatson-0.9.7/watson/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-29 16:01:30.000000 dearwatson-0.9.7/watson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-29 16:01:30.000000 dearwatson-0.9.7/watson/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:01:40.876061 dearwatson-0.9.7/watson/data_validation_report/
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-01-29 16:01:30.000000 dearwatson-0.9.7/watson/data_validation_report/DvrPreparer.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-29 16:01:30.000000 dearwatson-0.9.7/watson/data_validation_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13705 2024-01-29 16:01:30.000000 dearwatson-0.9.7/watson/neighbours.py
--rw-r--r--   0 runner    (1001) docker     (127)    19373 2024-01-29 16:01:30.000000 dearwatson-0.9.7/watson/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:01:40.872061 dearwatson-0.9.7/watson/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:01:40.876061 dearwatson-0.9.7/watson/resources/images/
--rw-r--r--   0 runner    (1001) docker     (127)   524520 2024-01-29 16:01:30.000000 dearwatson-0.9.7/watson/resources/images/sherlock3.png
--rw-r--r--   0 runner    (1001) docker     (127)   738619 2024-01-29 16:01:30.000000 dearwatson-0.9.7/watson/resources/images/watson.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:01:40.876061 dearwatson-0.9.7/watson/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 16:01:31.000000 dearwatson-0.9.7/watson/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-01-29 16:01:31.000000 dearwatson-0.9.7/watson/tests/test_watson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 16:01:40.876061 dearwatson-0.9.7/watson/tpfplotterSub/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 16:01:32.000000 dearwatson-0.9.7/watson/tpfplotterSub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-01-29 16:01:32.000000 dearwatson-0.9.7/watson/tpfplotterSub/tpfplotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-01-29 16:01:32.000000 dearwatson-0.9.7/watson/tpfplotterSub/tpfplotter_py2.py
--rw-r--r--   0 runner    (1001) docker     (127)   112546 2024-01-29 16:01:32.000000 dearwatson-0.9.7/watson/watson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:47:47.153542 dearwatson-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-03 18:47:34.000000 dearwatson-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-03 18:47:34.000000 dearwatson-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-03 18:47:47.153542 dearwatson-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-03 18:47:34.000000 dearwatson-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:47:47.149542 dearwatson-0.9.9/dearwatson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-03 18:47:46.000000 dearwatson-0.9.9/dearwatson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-03 18:47:47.000000 dearwatson-0.9.9/dearwatson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:47:46.000000 dearwatson-0.9.9/dearwatson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-03 18:47:46.000000 dearwatson-0.9.9/dearwatson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 18:47:46.000000 dearwatson-0.9.9/dearwatson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 18:47:47.153542 dearwatson-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-03 18:47:35.000000 dearwatson-0.9.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-03 18:47:35.000000 dearwatson-0.9.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:47:47.149542 dearwatson-0.9.9/watson/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 18:47:35.000000 dearwatson-0.9.9/watson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-03 18:47:35.000000 dearwatson-0.9.9/watson/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:47:47.149542 dearwatson-0.9.9/watson/data_validation_report/
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-05-03 18:47:35.000000 dearwatson-0.9.9/watson/data_validation_report/DvrPreparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 18:47:35.000000 dearwatson-0.9.9/watson/data_validation_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13705 2024-05-03 18:47:35.000000 dearwatson-0.9.9/watson/neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19373 2024-05-03 18:47:35.000000 dearwatson-0.9.9/watson/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:47:47.149542 dearwatson-0.9.9/watson/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:47:47.153542 dearwatson-0.9.9/watson/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   524520 2024-05-03 18:47:35.000000 dearwatson-0.9.9/watson/resources/images/sherlock3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   738619 2024-05-03 18:47:35.000000 dearwatson-0.9.9/watson/resources/images/watson.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:47:47.153542 dearwatson-0.9.9/watson/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 18:47:36.000000 dearwatson-0.9.9/watson/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-05-03 18:47:36.000000 dearwatson-0.9.9/watson/tests/test_watson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:47:47.153542 dearwatson-0.9.9/watson/tpfplotterSub/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:47:37.000000 dearwatson-0.9.9/watson/tpfplotterSub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16155 2024-05-03 18:47:37.000000 dearwatson-0.9.9/watson/tpfplotterSub/tpfplotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-03 18:47:37.000000 dearwatson-0.9.9/watson/tpfplotterSub/tpfplotter_py2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112546 2024-05-03 18:47:37.000000 dearwatson-0.9.9/watson/watson.py
```

### Comparing `dearwatson-0.9.7/LICENSE` & `dearwatson-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dearwatson-0.9.7/PKG-INFO` & `dearwatson-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.9.7
+Version: 0.9.9
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.9.7/README.md` & `dearwatson-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `dearwatson-0.9.7/dearwatson.egg-info/PKG-INFO` & `dearwatson-0.9.9/dearwatson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearwatson
-Version: 0.9.7
+Version: 0.9.9
 Summary: Visual Vetting and Analysis of Transits from Space ObservatioNs
 Home-page: https://github.com/PlanetHunters/watson
 Author: M. Dévora-Pajares
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="350" src="https://github.com/PlanetHunters/watson/blob/main/images/watson.png?raw=true">
```

### Comparing `dearwatson-0.9.7/dearwatson.egg-info/SOURCES.txt` & `dearwatson-0.9.9/dearwatson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dearwatson-0.9.7/setup.py` & `dearwatson-0.9.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-version = "0.9.7"
+version = "0.9.9"
 setuptools.setup(
     name="dearwatson", # Replace with your own username
     version=version,
     author="M. Dévora-Pajares",
     author_email="mdevorapajares@protonmail.com",
     description="Visual Vetting and Analysis of Transits from Space ObservatioNs",
     long_description=long_description,
@@ -21,15 +21,15 @@
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.10',
     install_requires=[
                         "bokeh==2.4.2", # TPFPlotter dependency
                         'configparser==5.0.1',
                         "extension-helpers==0.1",
-                        "exoml==0.1.5",
+                        "exoml==0.1.7",
                         "imageio==2.9.0",
                         'pyparsing==2.4.7', # Matplotlib dependency
                         "pyyaml==6.0.1",
                         "pillow==9.5.0",
                         "reportlab==4.0.7",
                         'setuptools>=41.0.0'
     ]
```

### Comparing `dearwatson-0.9.7/watson/data_validation_report/DvrPreparer.py` & `dearwatson-0.9.9/watson/data_validation_report/DvrPreparer.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.9.7/watson/neighbours.py` & `dearwatson-0.9.9/watson/neighbours.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.9.7/watson/report.py` & `dearwatson-0.9.9/watson/report.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.9.7/watson/resources/images/sherlock3.png` & `dearwatson-0.9.9/watson/resources/images/sherlock3.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.9.7/watson/resources/images/watson.png` & `dearwatson-0.9.9/watson/resources/images/watson.png`

 * *Files identical despite different names*

### Comparing `dearwatson-0.9.7/watson/tests/test_watson.py` & `dearwatson-0.9.9/watson/tests/test_watson.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.9.7/watson/tpfplotterSub/tpfplotter.py` & `dearwatson-0.9.9/watson/tpfplotterSub/tpfplotter.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.9.7/watson/tpfplotterSub/tpfplotter_py2.py` & `dearwatson-0.9.9/watson/tpfplotterSub/tpfplotter_py2.py`

 * *Files identical despite different names*

### Comparing `dearwatson-0.9.7/watson/watson.py` & `dearwatson-0.9.9/watson/watson.py`

 * *Files identical despite different names*

