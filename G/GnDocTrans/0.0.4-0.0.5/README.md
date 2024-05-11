# Comparing `tmp/GnDocTrans-0.0.4.tar.gz` & `tmp/GnDocTrans-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GnDocTrans-0.0.4.tar", last modified: Fri May 10 03:01:27 2024, max compression
+gzip compressed data, was "GnDocTrans-0.0.5.tar", last modified: Sat May 11 06:57:40 2024, max compression
```

## Comparing `GnDocTrans-0.0.4.tar` & `GnDocTrans-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-10 03:01:27.825815 GnDocTrans-0.0.4/
-drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-10 03:01:27.825815 GnDocTrans-0.0.4/GnDocTrans/
--rw-rw-r--   0 fusen     (1000) fusen     (1000)       30 2024-05-07 06:57:19.000000 GnDocTrans-0.0.4/GnDocTrans/__init__.py
--rw-rw-r--   0 fusen     (1000) fusen     (1000)    23925 2024-05-10 03:00:34.000000 GnDocTrans-0.0.4/GnDocTrans/tri_derive_tile.py
-drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-10 03:01:27.825815 GnDocTrans-0.0.4/GnDocTrans.egg-info/
--rw-rw-r--   0 fusen     (1000) fusen     (1000)      354 2024-05-10 03:01:27.000000 GnDocTrans-0.0.4/GnDocTrans.egg-info/PKG-INFO
--rw-rw-r--   0 fusen     (1000) fusen     (1000)      230 2024-05-10 03:01:27.000000 GnDocTrans-0.0.4/GnDocTrans.egg-info/SOURCES.txt
--rw-rw-r--   0 fusen     (1000) fusen     (1000)        1 2024-05-10 03:01:27.000000 GnDocTrans-0.0.4/GnDocTrans.egg-info/dependency_links.txt
--rw-rw-r--   0 fusen     (1000) fusen     (1000)       20 2024-05-10 03:01:27.000000 GnDocTrans-0.0.4/GnDocTrans.egg-info/requires.txt
--rw-rw-r--   0 fusen     (1000) fusen     (1000)       11 2024-05-10 03:01:27.000000 GnDocTrans-0.0.4/GnDocTrans.egg-info/top_level.txt
--rw-rw-r--   0 fusen     (1000) fusen     (1000)      354 2024-05-10 03:01:27.825815 GnDocTrans-0.0.4/PKG-INFO
--rw-rw-r--   0 fusen     (1000) fusen     (1000)       38 2024-05-10 03:01:27.825815 GnDocTrans-0.0.4/setup.cfg
--rw-rw-r--   0 fusen     (1000) fusen     (1000)      501 2024-05-10 03:00:49.000000 GnDocTrans-0.0.4/setup.py
+drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-11 06:57:40.008150 GnDocTrans-0.0.5/
+drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-11 06:57:40.008150 GnDocTrans-0.0.5/GnDocTrans/
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)       59 2024-05-11 06:54:36.000000 GnDocTrans-0.0.5/GnDocTrans/__init__.py
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)     7916 2024-05-11 06:54:00.000000 GnDocTrans-0.0.5/GnDocTrans/trace_profile.py
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)    23925 2024-05-10 03:00:34.000000 GnDocTrans-0.0.5/GnDocTrans/tri_derive_tile.py
+drwxrwxr-x   0 fusen     (1000) fusen     (1000)        0 2024-05-11 06:57:40.008150 GnDocTrans-0.0.5/GnDocTrans.egg-info/
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)      354 2024-05-11 06:57:40.000000 GnDocTrans-0.0.5/GnDocTrans.egg-info/PKG-INFO
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)      258 2024-05-11 06:57:40.000000 GnDocTrans-0.0.5/GnDocTrans.egg-info/SOURCES.txt
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)        1 2024-05-11 06:57:40.000000 GnDocTrans-0.0.5/GnDocTrans.egg-info/dependency_links.txt
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)       20 2024-05-11 06:57:40.000000 GnDocTrans-0.0.5/GnDocTrans.egg-info/requires.txt
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)       11 2024-05-11 06:57:40.000000 GnDocTrans-0.0.5/GnDocTrans.egg-info/top_level.txt
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)      354 2024-05-11 06:57:40.008150 GnDocTrans-0.0.5/PKG-INFO
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)       38 2024-05-11 06:57:40.008150 GnDocTrans-0.0.5/setup.cfg
+-rw-rw-r--   0 fusen     (1000) fusen     (1000)      501 2024-05-11 06:56:17.000000 GnDocTrans-0.0.5/setup.py
```

### Comparing `GnDocTrans-0.0.4/GnDocTrans/tri_derive_tile.py` & `GnDocTrans-0.0.5/GnDocTrans/tri_derive_tile.py`

 * *Files identical despite different names*

