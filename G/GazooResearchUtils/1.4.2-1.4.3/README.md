# Comparing `tmp/GazooResearchUtils-1.4.2.tar.gz` & `tmp/GazooResearchUtils-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.4.2.tar", last modified: Sat May 11 02:39:42 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.4.3.tar", last modified: Sat May 11 02:43:00 2024, max compression
```

## Comparing `GazooResearchUtils-1.4.2.tar` & `GazooResearchUtils-1.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:39:42.271333 GazooResearchUtils-1.4.2/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:39:42.271042 GazooResearchUtils-1.4.2/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:39:42.268932 GazooResearchUtils-1.4.2/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:39:42.269385 GazooResearchUtils-1.4.2/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)       96 2024-05-11 02:39:34.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:39:42.270701 GazooResearchUtils-1.4.2/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)     5518 2024-05-11 02:35:01.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:39:42.270282 GazooResearchUtils-1.4.2/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:39:42.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-11 02:39:42.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-11 02:39:42.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-11 02:39:42.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils.egg-info/requires.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-11 02:39:42.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-11 02:39:42.271389 GazooResearchUtils-1.4.2/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-11 02:39:41.000000 GazooResearchUtils-1.4.2/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:43:00.222396 GazooResearchUtils-1.4.3/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:43:00.222089 GazooResearchUtils-1.4.3/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:43:00.220198 GazooResearchUtils-1.4.3/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:43:00.220636 GazooResearchUtils-1.4.3/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)       96 2024-05-11 02:39:34.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:43:00.221741 GazooResearchUtils-1.4.3/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     5523 2024-05-11 02:42:42.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:43:00.221368 GazooResearchUtils-1.4.3/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:43:00.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-11 02:43:00.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-11 02:43:00.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-11 02:43:00.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-11 02:43:00.000000 GazooResearchUtils-1.4.3/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-11 02:43:00.222451 GazooResearchUtils-1.4.3/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-11 02:42:50.000000 GazooResearchUtils-1.4.3/setup.py
```

### Comparing `GazooResearchUtils-1.4.2/app/GazooResearchUtils/src/Analysis.py` & `GazooResearchUtils-1.4.3/app/GazooResearchUtils/src/Analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
       # 
       if len(test.index) >= 1: valid.append(True)
       else: valid.append(False)
 
     #print(valid)
     # Append mrn to list if all filters apply
     if all(valid):
-      mrn_list.append(mrn) 
+      mrn_list.append(str(mrn)) 
 
   return mrn_list
 
 def plot_km_curves(time_list, event_list):
     """
     Creates a Kaplan-Meier plot.
```

