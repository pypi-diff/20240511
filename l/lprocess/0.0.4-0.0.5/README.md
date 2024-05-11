# Comparing `tmp/lprocess-0.0.4.tar.gz` & `tmp/lprocess-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lprocess-0.0.4.tar", last modified: Sat May 11 01:46:59 2024, max compression
+gzip compressed data, was "lprocess-0.0.5.tar", last modified: Sat May 11 11:33:45 2024, max compression
```

## Comparing `lprocess-0.0.4.tar` & `lprocess-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-11 01:46:59.540552 lprocess-0.0.4/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-11 01:46:59.540552 lprocess-0.0.4/PKG-INFO
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-11 01:46:59.540552 lprocess-0.0.4/lprocess/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       27 2024-05-10 15:02:52.000000 lprocess-0.0.4/lprocess/__init__.py
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       47 2024-05-11 01:33:25.000000 lprocess-0.0.4/lprocess/hello.py
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-11 01:46:59.540552 lprocess-0.0.4/lprocess.egg-info/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-11 01:46:59.000000 lprocess-0.0.4/lprocess.egg-info/PKG-INFO
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      206 2024-05-11 01:46:59.000000 lprocess-0.0.4/lprocess.egg-info/SOURCES.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        1 2024-05-11 01:46:59.000000 lprocess-0.0.4/lprocess.egg-info/dependency_links.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       24 2024-05-11 01:46:59.000000 lprocess-0.0.4/lprocess.egg-info/requires.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        9 2024-05-11 01:46:59.000000 lprocess-0.0.4/lprocess.egg-info/top_level.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       38 2024-05-11 01:46:59.540552 lprocess-0.0.4/setup.cfg
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      703 2024-05-11 01:46:53.000000 lprocess-0.0.4/setup.py
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-11 11:33:45.366538 lprocess-0.0.5/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-11 11:33:45.366538 lprocess-0.0.5/PKG-INFO
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-11 11:33:45.366538 lprocess-0.0.5/lprocess/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      810 2024-05-11 11:28:18.000000 lprocess-0.0.5/lprocess/EDA.py
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       25 2024-05-11 11:28:37.000000 lprocess-0.0.5/lprocess/__init__.py
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-11 11:33:45.366538 lprocess-0.0.5/lprocess.egg-info/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-11 11:33:45.000000 lprocess-0.0.5/lprocess.egg-info/PKG-INFO
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      204 2024-05-11 11:33:45.000000 lprocess-0.0.5/lprocess.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        1 2024-05-11 11:33:45.000000 lprocess-0.0.5/lprocess.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       24 2024-05-11 11:33:45.000000 lprocess-0.0.5/lprocess.egg-info/requires.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        9 2024-05-11 11:33:45.000000 lprocess-0.0.5/lprocess.egg-info/top_level.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       38 2024-05-11 11:33:45.366538 lprocess-0.0.5/setup.cfg
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      703 2024-05-11 11:28:40.000000 lprocess-0.0.5/setup.py
```

### Comparing `lprocess-0.0.4/setup.py` & `lprocess-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Data Preprocessing library'
 
 
 # Setting up
 setup(
     name="lprocess",
     version=VERSION,
```

