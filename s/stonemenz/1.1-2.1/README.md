# Comparing `tmp/stonemenz-1.1.tar.gz` & `tmp/stonemenz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stonemenz-1.1.tar", last modified: Wed May  8 13:09:40 2024, max compression
+gzip compressed data, was "stonemenz-2.1.tar", last modified: Sat May 11 16:30:28 2024, max compression
```

## Comparing `stonemenz-1.1.tar` & `stonemenz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:09:40.963093 stonemenz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-08 13:09:40.963093 stonemenz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 13:09:40.755089 stonemenz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-08 13:09:40.771090 stonemenz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:09:40.963093 stonemenz-1.1/stonemenz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:09:40.755089 stonemenz-1.1/stonemenz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:09:40.763090 stonemenz-1.1/stonemenz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:30:28.290240 stonemenz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 13:09:40.000000 stonemenz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 16:30:28.290240 stonemenz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 13:09:40.000000 stonemenz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 16:30:28.290240 stonemenz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-11 16:30:21.000000 stonemenz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:30:28.290240 stonemenz-2.1/stonemenz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:09:40.000000 stonemenz-2.1/stonemenz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:09:40.000000 stonemenz-2.1/stonemenz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:30:28.290240 stonemenz-2.1/stonemenz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 16:30:27.000000 stonemenz-2.1/stonemenz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-11 16:30:27.000000 stonemenz-2.1/stonemenz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 16:30:27.000000 stonemenz-2.1/stonemenz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 16:30:27.000000 stonemenz-2.1/stonemenz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-11 16:30:27.000000 stonemenz-2.1/stonemenz.egg-info/top_level.txt
```

### Comparing `stonemenz-1.1/setup.py` & `stonemenz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'stonemenz',
     packages = ['stonemenz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'stonemenz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/stonemenz',
```

