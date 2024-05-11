# Comparing `tmp/fissure-engine-1.0.5.tar.gz` & `tmp/fissure_engine-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fissure-engine-1.0.5.tar", last modified: Fri Apr 12 19:12:48 2024, max compression
+gzip compressed data, was "fissure_engine-1.0.6.tar", last modified: Sat May 11 13:14:52 2024, max compression
```

## Comparing `fissure-engine-1.0.5.tar` & `fissure_engine-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 19:12:48.040608 fissure-engine-1.0.5/
--rw-rw-rw-   0        0        0      485 2024-04-12 19:12:48.039609 fissure-engine-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 19:12:48.033623 fissure-engine-1.0.5/fissure_engine/
--rw-rw-rw-   0        0        0        0 2024-04-05 16:22:54.000000 fissure-engine-1.0.5/fissure_engine/__init__.py
--rw-rw-rw-   0        0        0    75962 2024-03-27 20:54:24.000000 fissure-engine-1.0.5/fissure_engine/common.py
--rw-rw-rw-   0        0        0    17886 2024-04-12 19:12:33.000000 fissure-engine-1.0.5/fissure_engine/fissure_engine.py
-drwxrwxrwx   0        0        0        0 2024-04-12 19:12:48.038608 fissure-engine-1.0.5/fissure_engine.egg-info/
--rw-rw-rw-   0        0        0      485 2024-04-12 19:12:47.000000 fissure-engine-1.0.5/fissure_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-04-12 19:12:47.000000 fissure-engine-1.0.5/fissure_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 19:12:47.000000 fissure-engine-1.0.5/fissure_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-12 19:12:47.000000 fissure-engine-1.0.5/fissure_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-12 19:12:47.000000 fissure-engine-1.0.5/fissure_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 19:12:48.040608 fissure-engine-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      749 2024-04-12 19:12:40.000000 fissure-engine-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 13:14:52.447024 fissure_engine-1.0.6/
+-rw-rw-rw-   0        0        0      485 2024-05-11 13:14:52.446026 fissure_engine-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 13:14:52.442301 fissure_engine-1.0.6/fissure_engine/
+-rw-rw-rw-   0        0        0        0 2024-05-11 13:06:59.000000 fissure_engine-1.0.6/fissure_engine/__init__.py
+-rw-rw-rw-   0        0        0    76001 2024-05-11 13:12:36.000000 fissure_engine-1.0.6/fissure_engine/common.py
+-rw-rw-rw-   0        0        0    18046 2024-05-11 13:12:00.000000 fissure_engine-1.0.6/fissure_engine/fissure_engine.py
+drwxrwxrwx   0        0        0        0 2024-05-11 13:14:52.446026 fissure_engine-1.0.6/fissure_engine.egg-info/
+-rw-rw-rw-   0        0        0      485 2024-05-11 13:14:52.000000 fissure_engine-1.0.6/fissure_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-11 13:14:52.000000 fissure_engine-1.0.6/fissure_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 13:14:52.000000 fissure_engine-1.0.6/fissure_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-11 13:14:52.000000 fissure_engine-1.0.6/fissure_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-11 13:14:52.000000 fissure_engine-1.0.6/fissure_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 13:14:52.447024 fissure_engine-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      749 2024-05-11 13:14:44.000000 fissure_engine-1.0.6/setup.py
```

### Comparing `fissure-engine-1.0.5/fissure_engine/common.py` & `fissure_engine-1.0.6/fissure_engine/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -3271,14 +3271,15 @@
         "Volatile": 2,
         "Core Sabotage": 1,
         "Machine Sabotage": 1,
         "Ship Sabotage": 2,
         "Gas City Sabotage": 4,
         "Orokin Sabotage": 4,
         "Injector Sabotage": 4,
+        "Steel Path Void Cascade": 3,
         "Void Cascade": 5,
         "Void Flood": 5,
         "Alchemy": 5
     }
 }
 
 SORT_ORDER = {'Lith': 0,
```

### Comparing `fissure-engine-1.0.5/fissure_engine/fissure_engine.py` & `fissure_engine-1.0.6/fissure_engine/fissure_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,19 @@
             tileset = node['tileset']
 
         return mission, node['node'], node['planet'], tileset, node['enemy']
 
     @staticmethod
     def get_fissure_data(fissure, fissure_type, mission):
         era = fissure_parser['era'][fissure[fissure_parser["era_key"][fissure_type]]]
-        tier = fissure_parser['tier'][mission]
+
+        if f"{fissure_type} {mission}" in fissure_parser['tier']:
+            tier = fissure_parser['tier'][f"{fissure_type} {mission}"]
+        else:
+            tier = fissure_parser['tier'][mission]
 
         return era, tier
 
     def classify_fissure_type(self, fissure):
         if 'ActiveMissionTier' in fissure:
             return self.FISSURE_TYPE_VOID_STORMS
         elif 'Hard' in fissure:
```

### Comparing `fissure-engine-1.0.5/setup.py` & `fissure_engine-1.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 DESCRIPTION = 'Engine for getting fissure information in Warframe.'
 LONG_DESCRIPTION = 'Engine for getting the current fissures for Warframe in a dictionary object.'
 
 
 setup(
     name='fissure-engine',
     version=VERSION,
```

