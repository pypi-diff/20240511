# Comparing `tmp/GazooResearchUtils-1.3.5.tar.gz` & `tmp/GazooResearchUtils-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.3.5.tar", last modified: Fri May 10 23:24:51 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.3.6.tar", last modified: Fri May 10 23:30:07 2024, max compression
```

## Comparing `GazooResearchUtils-1.3.5.tar` & `GazooResearchUtils-1.3.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:24:51.549108 GazooResearchUtils-1.3.5/
--rw-r--r--   0 andrewlim   (501) staff       (20)      242 2024-05-10 23:24:51.548740 GazooResearchUtils-1.3.5/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:24:51.547074 GazooResearchUtils-1.3.5/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:24:51.547508 GazooResearchUtils-1.3.5/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)       70 2024-05-10 21:31:29.000000 GazooResearchUtils-1.3.5/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:24:51.548460 GazooResearchUtils-1.3.5/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)     4490 2024-05-10 23:22:24.000000 GazooResearchUtils-1.3.5/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.3.5/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:24:51.548133 GazooResearchUtils-1.3.5/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      242 2024-05-10 23:24:51.000000 GazooResearchUtils-1.3.5/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      305 2024-05-10 23:24:51.000000 GazooResearchUtils-1.3.5/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-10 23:24:51.000000 GazooResearchUtils-1.3.5/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-10 23:24:51.000000 GazooResearchUtils-1.3.5/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-10 23:24:51.549178 GazooResearchUtils-1.3.5/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      461 2024-05-10 23:24:49.000000 GazooResearchUtils-1.3.5/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:30:07.063851 GazooResearchUtils-1.3.6/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      275 2024-05-10 23:30:07.063526 GazooResearchUtils-1.3.6/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:30:07.061176 GazooResearchUtils-1.3.6/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:30:07.061615 GazooResearchUtils-1.3.6/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)       70 2024-05-10 21:31:29.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:30:07.062980 GazooResearchUtils-1.3.6/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     4490 2024-05-10 23:22:24.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:30:07.062505 GazooResearchUtils-1.3.6/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      275 2024-05-10 23:30:07.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-10 23:30:07.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-10 23:30:07.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-10 23:30:07.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-10 23:30:07.000000 GazooResearchUtils-1.3.6/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-10 23:30:07.063928 GazooResearchUtils-1.3.6/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      422 2024-05-10 23:30:06.000000 GazooResearchUtils-1.3.6/setup.py
```

### Comparing `GazooResearchUtils-1.3.5/app/GazooResearchUtils/src/Analysis.py` & `GazooResearchUtils-1.3.6/app/GazooResearchUtils/src/Analysis.py`

 * *Files identical despite different names*

