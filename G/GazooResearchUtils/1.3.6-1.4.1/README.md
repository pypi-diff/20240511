# Comparing `tmp/GazooResearchUtils-1.3.6.tar.gz` & `tmp/GazooResearchUtils-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.3.6.tar", last modified: Fri May 10 23:30:07 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.4.1.tar", last modified: Sat May 11 02:35:58 2024, max compression
```

## Comparing `GazooResearchUtils-1.3.6.tar` & `GazooResearchUtils-1.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:30:07.063851 GazooResearchUtils-1.3.6/
--rw-r--r--   0 andrewlim   (501) staff       (20)      275 2024-05-10 23:30:07.063526 GazooResearchUtils-1.3.6/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:30:07.061176 GazooResearchUtils-1.3.6/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:30:07.061615 GazooResearchUtils-1.3.6/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)       70 2024-05-10 21:31:29.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:30:07.062980 GazooResearchUtils-1.3.6/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)     4490 2024-05-10 23:22:24.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:30:07.062505 GazooResearchUtils-1.3.6/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      275 2024-05-10 23:30:07.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-10 23:30:07.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-10 23:30:07.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-10 23:30:07.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils.egg-info/requires.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-10 23:30:07.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-10 23:30:07.063928 GazooResearchUtils-1.3.6/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      422 2024-05-10 23:30:06.000000 GazooResearchUtils-1.3.6/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:35:58.574528 GazooResearchUtils-1.4.1/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:35:58.574270 GazooResearchUtils-1.4.1/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:35:58.572256 GazooResearchUtils-1.4.1/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:35:58.572710 GazooResearchUtils-1.4.1/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)       70 2024-05-10 21:31:29.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:35:58.573903 GazooResearchUtils-1.4.1/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     5518 2024-05-11 02:35:01.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:35:58.573504 GazooResearchUtils-1.4.1/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:35:58.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-11 02:35:58.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-11 02:35:58.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-11 02:35:58.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-11 02:35:58.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-11 02:35:58.574582 GazooResearchUtils-1.4.1/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-11 02:35:19.000000 GazooResearchUtils-1.4.1/setup.py
```

### Comparing `GazooResearchUtils-1.3.6/app/GazooResearchUtils/src/Analysis.py` & `GazooResearchUtils-1.4.1/app/GazooResearchUtils/src/Analysis.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,53 @@
 import pandas as pd
 from datetime import datetime
 from lifelines import KaplanMeierFitter
 import matplotlib.pyplot as plt
 
+def get_mrns_where_filters(data, filters):
+  """
+  Obtains mrns where filters applies.
+
+  Parameters:
+    data (DataFrame): dataframe with csv data
+    event_tag_list (list of dicts): list of possible filters. Structure of filter {'icd10':str, 'tag': str, 'field': str, 'value': [str, str,...]}
+
+    Returns:
+    mrn_list (list of str): mrns
+    
+  """
+  
+  mrn_list = []
+
+  # Loop Through MRNs
+  for mrn in data.mrn.unique(): 
+    #print("mrn",mrn)
+    # Select mrn specific Information
+    pt = data.loc[(data['mrn'] == mrn)]
+
+    # Loop Through Conditions
+    #print(filters)
+    valid = []
+    for filter in filters:
+      test = pt.loc[(pt['icd10'] == filter['icd10']) 
+        & (pt['tag'] == filter['tag'])
+        & (pt['field'] == filter['field'])
+        & (pt['value'].isin(filter['value']))]
+
+      # 
+      if len(test.index) >= 1: valid.append(True)
+      else: valid.append(False)
+
+    #print(valid)
+    # Append mrn to list if all filters apply
+    if all(valid):
+      mrn_list.append(mrn) 
+
+  return mrn_list
+
 def plot_km_curves(time_list, event_list):
     """
     Creates a Kaplan-Meier plot.
 
     Parameters:
     time_list (list of int): time in months until censoring of data
     event_list (list of int): 1 or 0 to specify if event occurred
```

