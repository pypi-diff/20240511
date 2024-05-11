# Comparing `tmp/GazooResearchUtils-1.4.3.tar.gz` & `tmp/GazooResearchUtils-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.4.3.tar", last modified: Sat May 11 02:43:00 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.4.4.tar", last modified: Sat May 11 02:51:47 2024, max compression
```

## Comparing `GazooResearchUtils-1.4.3.tar` & `GazooResearchUtils-1.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:43:00.222396 GazooResearchUtils-1.4.3/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:43:00.222089 GazooResearchUtils-1.4.3/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:43:00.220198 GazooResearchUtils-1.4.3/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:43:00.220636 GazooResearchUtils-1.4.3/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)       96 2024-05-11 02:39:34.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:43:00.221741 GazooResearchUtils-1.4.3/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)     5523 2024-05-11 02:42:42.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:43:00.221368 GazooResearchUtils-1.4.3/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:43:00.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-11 02:43:00.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-11 02:43:00.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-11 02:43:00.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils.egg-info/requires.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-11 02:43:00.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-11 02:43:00.222451 GazooResearchUtils-1.4.3/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-11 02:42:50.000000 GazooResearchUtils-1.4.3/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:51:47.485192 GazooResearchUtils-1.4.4/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:51:47.484910 GazooResearchUtils-1.4.4/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:51:47.482786 GazooResearchUtils-1.4.4/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:51:47.483211 GazooResearchUtils-1.4.4/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)       96 2024-05-11 02:39:34.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:51:47.484537 GazooResearchUtils-1.4.4/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     6131 2024-05-11 02:51:33.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:51:47.484122 GazooResearchUtils-1.4.4/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:51:47.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-11 02:51:47.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-11 02:51:47.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-11 02:51:47.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-11 02:51:47.000000 GazooResearchUtils-1.4.4/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-11 02:51:47.485247 GazooResearchUtils-1.4.4/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-11 02:51:43.000000 GazooResearchUtils-1.4.4/setup.py
```

### Comparing `GazooResearchUtils-1.4.3/app/GazooResearchUtils/src/Analysis.py` & `GazooResearchUtils-1.4.4/app/GazooResearchUtils/src/Analysis.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,30 +24,44 @@
     # Select mrn specific Information
     pt = data.loc[(data['mrn'] == mrn)]
 
     # Loop Through Conditions
     #print(filters)
     valid = []
     for filter in filters:
-      test = pt.loc[(pt['icd10'] == filter['icd10']) 
-        & (pt['tag'] == filter['tag'])
-        & (pt['field'] == filter['field'])
-        & (pt['value'].isin(filter['value']))]
 
-      # 
+      if "value" in filter and "field" in filter and "tag" in filter and "icd10" in filter:
+        test = pt.loc[(pt['icd10'] == filter['icd10']) 
+          & (pt['tag'] == filter['tag'])
+          & (pt['field'] == filter['field'])
+          & (pt['value'].isin(filter['value']))]
+      elif "field" in filter and "tag" in filter and "icd10" in filter:
+        test = pt.loc[(pt['icd10'] == filter['icd10']) 
+          & (pt['tag'] == filter['tag'])
+          & (pt['field'] == filter['field'])]
+      elif "tag" in filter and "icd10" in filter:
+        test = pt.loc[(pt['icd10'] == filter['icd10']) 
+          & (pt['tag'] == filter['tag'])]
+      elif "icd10" in filter:
+        test = pt.loc[(pt['icd10'] == filter['icd10'])]
+      else:
+        test = pd.DataFrame()
+
+      # Is filter apply
       if len(test.index) >= 1: valid.append(True)
       else: valid.append(False)
 
     #print(valid)
     # Append mrn to list if all filters apply
     if all(valid):
       mrn_list.append(str(mrn)) 
 
   return mrn_list
 
+
 def plot_km_curves(time_list, event_list):
     """
     Creates a Kaplan-Meier plot.
 
     Parameters:
     time_list (list of int): time in months until censoring of data
     event_list (list of int): 1 or 0 to specify if event occurred
```

