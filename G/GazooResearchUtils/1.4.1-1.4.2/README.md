# Comparing `tmp/GazooResearchUtils-1.4.1.tar.gz` & `tmp/GazooResearchUtils-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GazooResearchUtils-1.4.1.tar", last modified: Sat May 11 02:35:58 2024, max compression
+gzip compressed data, was "GazooResearchUtils-1.4.2.tar", last modified: Sat May 11 02:39:42 2024, max compression
```

## Comparing `GazooResearchUtils-1.4.1.tar` & `GazooResearchUtils-1.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:35:58.574528 GazooResearchUtils-1.4.1/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:35:58.574270 GazooResearchUtils-1.4.1/PKG-INFO
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:35:58.572256 GazooResearchUtils-1.4.1/app/
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:35:58.572710 GazooResearchUtils-1.4.1/app/GazooResearchUtils/
--rw-r--r--   0 andrewlim   (501) staff       (20)       70 2024-05-10 21:31:29.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:35:58.573903 GazooResearchUtils-1.4.1/app/GazooResearchUtils/src/
--rw-r--r--   0 andrewlim   (501) staff       (20)     5518 2024-05-11 02:35:01.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils/src/Analysis.py
--rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils/src/__init__.py
-drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:35:58.573504 GazooResearchUtils-1.4.1/app/GazooResearchUtils.egg-info/
--rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:35:58.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils.egg-info/PKG-INFO
--rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-11 02:35:58.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils.egg-info/SOURCES.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-11 02:35:58.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils.egg-info/dependency_links.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-11 02:35:58.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils.egg-info/requires.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-11 02:35:58.000000 GazooResearchUtils-1.4.1/app/GazooResearchUtils.egg-info/top_level.txt
--rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-11 02:35:58.574582 GazooResearchUtils-1.4.1/setup.cfg
--rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-11 02:35:19.000000 GazooResearchUtils-1.4.1/setup.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:39:42.271333 GazooResearchUtils-1.4.2/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:39:42.271042 GazooResearchUtils-1.4.2/PKG-INFO
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:39:42.268932 GazooResearchUtils-1.4.2/app/
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:39:42.269385 GazooResearchUtils-1.4.2/app/GazooResearchUtils/
+-rw-r--r--   0 andrewlim   (501) staff       (20)       96 2024-05-11 02:39:34.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:39:42.270701 GazooResearchUtils-1.4.2/app/GazooResearchUtils/src/
+-rw-r--r--   0 andrewlim   (501) staff       (20)     5518 2024-05-11 02:35:01.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils/src/Analysis.py
+-rw-r--r--   0 andrewlim   (501) staff       (20)        0 2024-05-10 21:10:14.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils/src/__init__.py
+drwxr-xr-x   0 andrewlim   (501) staff       (20)        0 2024-05-11 02:39:42.270282 GazooResearchUtils-1.4.2/app/GazooResearchUtils.egg-info/
+-rw-r--r--   0 andrewlim   (501) staff       (20)      268 2024-05-11 02:39:42.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils.egg-info/PKG-INFO
+-rw-r--r--   0 andrewlim   (501) staff       (20)      350 2024-05-11 02:39:42.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)        1 2024-05-11 02:39:42.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       18 2024-05-11 02:39:42.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils.egg-info/requires.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       19 2024-05-11 02:39:42.000000 GazooResearchUtils-1.4.2/app/GazooResearchUtils.egg-info/top_level.txt
+-rw-r--r--   0 andrewlim   (501) staff       (20)       38 2024-05-11 02:39:42.271389 GazooResearchUtils-1.4.2/setup.cfg
+-rw-r--r--   0 andrewlim   (501) staff       (20)      415 2024-05-11 02:39:41.000000 GazooResearchUtils-1.4.2/setup.py
```

### Comparing `GazooResearchUtils-1.4.1/app/GazooResearchUtils/src/Analysis.py` & `GazooResearchUtils-1.4.2/app/GazooResearchUtils/src/Analysis.py`

 * *Files identical despite different names*

