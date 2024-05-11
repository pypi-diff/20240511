# Comparing `tmp/lprocess-0.0.2.tar.gz` & `tmp/lprocess-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lprocess-0.0.2.tar", last modified: Fri May 10 15:24:45 2024, max compression
+gzip compressed data, was "lprocess-0.0.3.tar", last modified: Sat May 11 01:38:10 2024, max compression
```

## Comparing `lprocess-0.0.2.tar` & `lprocess-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-10 15:24:45.248006 lprocess-0.0.2/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      553 2024-05-10 15:24:45.248006 lprocess-0.0.2/PKG-INFO
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-10 15:24:45.248006 lprocess-0.0.2/lprocess/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       27 2024-05-10 15:02:52.000000 lprocess-0.0.2/lprocess/__init__.py
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       29 2024-05-10 15:02:08.000000 lprocess-0.0.2/lprocess/lprocess.py
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-10 15:24:45.248006 lprocess-0.0.2/lprocess.egg-info/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      553 2024-05-10 15:24:45.000000 lprocess-0.0.2/lprocess.egg-info/PKG-INFO
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      209 2024-05-10 15:24:45.000000 lprocess-0.0.2/lprocess.egg-info/SOURCES.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        1 2024-05-10 15:24:45.000000 lprocess-0.0.2/lprocess.egg-info/dependency_links.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       24 2024-05-10 15:24:45.000000 lprocess-0.0.2/lprocess.egg-info/requires.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        9 2024-05-10 15:24:45.000000 lprocess-0.0.2/lprocess.egg-info/top_level.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       38 2024-05-10 15:24:45.248006 lprocess-0.0.2/setup.cfg
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      766 2024-05-10 15:24:12.000000 lprocess-0.0.2/setup.py
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-11 01:38:10.304482 lprocess-0.0.3/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-11 01:38:10.304482 lprocess-0.0.3/PKG-INFO
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-11 01:38:10.304482 lprocess-0.0.3/lprocess/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       27 2024-05-10 15:02:52.000000 lprocess-0.0.3/lprocess/__init__.py
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       47 2024-05-11 01:33:25.000000 lprocess-0.0.3/lprocess/lprocess.py
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-11 01:38:10.304482 lprocess-0.0.3/lprocess.egg-info/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-11 01:38:10.000000 lprocess-0.0.3/lprocess.egg-info/PKG-INFO
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      209 2024-05-11 01:38:10.000000 lprocess-0.0.3/lprocess.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        1 2024-05-11 01:38:10.000000 lprocess-0.0.3/lprocess.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       24 2024-05-11 01:38:10.000000 lprocess-0.0.3/lprocess.egg-info/requires.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        9 2024-05-11 01:38:10.000000 lprocess-0.0.3/lprocess.egg-info/top_level.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       38 2024-05-11 01:38:10.304482 lprocess-0.0.3/setup.cfg
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      703 2024-05-11 01:37:58.000000 lprocess-0.0.3/setup.py
```

### Comparing `lprocess-0.0.2/setup.py` & `lprocess-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Data Preprocessing library'
 
 
 # Setting up
 setup(
     name="lprocess",
     version=VERSION,
     author="Chirag Patil",
     author_email="chiragnpatil@gmail.com",
     description=DESCRIPTION,
     packages=find_packages(),
     install_requires=['numpy', 'pandas', 'matplotlib'],
-    keywords=['python', 'video', 'stream', 'video stream', 'camera stream', 'sockets'],
+    keywords=['python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

