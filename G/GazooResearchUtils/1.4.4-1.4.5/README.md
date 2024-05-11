# Comparing `tmp/GazooResearchUtils-1.4.4.tar.gz` & `tmp/GazooResearchUtils-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.4.4.tar", last modified: Sat May 11 02:51:47 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.4.5.tar", last modified: Sat May 11 03:34:00 2024, max compression
```

## Comparing `GazooResearchUtils-1.4.4.tar` & `GazooResearchUtils-1.4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:51:47.485192 GazooResearchUtils-1.4.4/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:51:47.484910 GazooResearchUtils-1.4.4/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:51:47.482786 GazooResearchUtils-1.4.4/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:51:47.483211 GazooResearchUtils-1.4.4/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)       96 2024-05-11 02:39:34.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:51:47.484537 GazooResearchUtils-1.4.4/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)     6131 2024-05-11 02:51:33.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:51:47.484122 GazooResearchUtils-1.4.4/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:51:47.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-11 02:51:47.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-11 02:51:47.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-11 02:51:47.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils.egg-info/requires.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-11 02:51:47.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-11 02:51:47.485247 GazooResearchUtils-1.4.4/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-11 02:51:43.000000 GazooResearchUtils-1.4.4/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 03:34:00.549818 GazooResearchUtils-1.4.5/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 03:34:00.549415 GazooResearchUtils-1.4.5/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 03:34:00.547309 GazooResearchUtils-1.4.5/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 03:34:00.547757 GazooResearchUtils-1.4.5/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      119 2024-05-11 03:33:46.000000 GazooResearchUtils-1.4.5/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 03:34:00.549020 GazooResearchUtils-1.4.5/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     6575 2024-05-11 03:33:39.000000 GazooResearchUtils-1.4.5/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.4.5/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 03:34:00.548509 GazooResearchUtils-1.4.5/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 03:34:00.000000 GazooResearchUtils-1.4.5/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-11 03:34:00.000000 GazooResearchUtils-1.4.5/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-11 03:34:00.000000 GazooResearchUtils-1.4.5/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-11 03:34:00.000000 GazooResearchUtils-1.4.5/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-11 03:34:00.000000 GazooResearchUtils-1.4.5/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-11 03:34:00.549899 GazooResearchUtils-1.4.5/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-11 03:33:51.000000 GazooResearchUtils-1.4.5/setup.py
```

### Comparing `GazooResearchUtils-1.4.4/app/GazooResearchUtils/src/Analysis.py` & `GazooResearchUtils-1.4.5/app/GazooResearchUtils/src/Analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 import pandas as pd
 from datetime import datetime
 from lifelines import KaplanMeierFitter
 import matplotlib.pyplot as plt
 
+def get_data_dictionary(data):
+  """
+  Returns data dictionary.
+
+  Parameters:
+    data (DataFrame): dataframe with csv data
+
+    Returns:
+    dictionary (DataFrame): dataframe with options
+    
+  """
+  
+  data = data[['icd10', 'tag', 'field', 'data_type']]
+  # Remove Duplicates
+  dictionary = data.drop_duplicates()
+  # Sort
+  dictionary = dictionary.sort_values(['icd10', 'tag', 'field'], ascending=[True, True, True])
+
+  return dictionary
+
 def get_mrns_where_filters(data, filters):
   """
   Obtains mrns where filters applies.
 
   Parameters:
     data (DataFrame): dataframe with csv data
     event_tag_list (list of dicts): list of possible filters. Structure of filter {'icd10':str, 'tag': str, 'field': str, 'value': [str, str,...]}
```

