# Comparing `tmp/GazooResearchUtils-1.3.1.tar.gz` & `tmp/GazooResearchUtils-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.3.1.tar", last modified: Fri May 10 21:39:04 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.3.2.tar", last modified: Fri May 10 23:11:41 2024, max compression
```

## Comparing `GazooResearchUtils-1.3.1.tar` & `GazooResearchUtils-1.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:39:04.627778 GazooResearchUtils-1.3.1/
--rw-r--r--   0 andrewlim   (501) staff       (20)      333 2024-05-10 21:39:04.627520 GazooResearchUtils-1.3.1/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:39:04.625613 GazooResearchUtils-1.3.1/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:39:04.626066 GazooResearchUtils-1.3.1/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)       70 2024-05-10 21:31:29.000000 GazooResearchUtils-1.3.1/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:39:04.627186 GazooResearchUtils-1.3.1/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)     4367 2024-05-10 21:37:41.000000 GazooResearchUtils-1.3.1/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.3.1/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:39:04.626808 GazooResearchUtils-1.3.1/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      333 2024-05-10 21:39:04.000000 GazooResearchUtils-1.3.1/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-10 21:39:04.000000 GazooResearchUtils-1.3.1/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-10 21:39:04.000000 GazooResearchUtils-1.3.1/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       46 2024-05-10 21:39:04.000000 GazooResearchUtils-1.3.1/app/GazooResearchUtils.egg-info/requires.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-10 21:39:04.000000 GazooResearchUtils-1.3.1/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-10 21:39:04.627833 GazooResearchUtils-1.3.1/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      460 2024-05-10 21:38:38.000000 GazooResearchUtils-1.3.1/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:11:41.005640 GazooResearchUtils-1.3.2/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      333 2024-05-10 23:11:41.005378 GazooResearchUtils-1.3.2/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:11:41.003408 GazooResearchUtils-1.3.2/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:11:41.003896 GazooResearchUtils-1.3.2/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)       70 2024-05-10 21:31:29.000000 GazooResearchUtils-1.3.2/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:11:41.005025 GazooResearchUtils-1.3.2/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     4367 2024-05-10 21:37:41.000000 GazooResearchUtils-1.3.2/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.3.2/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-10 23:11:41.004641 GazooResearchUtils-1.3.2/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      333 2024-05-10 23:11:40.000000 GazooResearchUtils-1.3.2/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-10 23:11:40.000000 GazooResearchUtils-1.3.2/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-10 23:11:40.000000 GazooResearchUtils-1.3.2/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       46 2024-05-10 23:11:40.000000 GazooResearchUtils-1.3.2/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-10 23:11:40.000000 GazooResearchUtils-1.3.2/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-10 23:11:41.005693 GazooResearchUtils-1.3.2/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      460 2024-05-10 23:11:27.000000 GazooResearchUtils-1.3.2/setup.py
```

### Comparing `GazooResearchUtils-1.3.1/app/GazooResearchUtils/src/Analysis.py` & `GazooResearchUtils-1.3.2/app/GazooResearchUtils/src/Analysis.py`

 * *Files identical despite different names*

