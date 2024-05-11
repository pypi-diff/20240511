# Comparing `tmp/pneumologyz-1.1.tar.gz` & `tmp/pneumologyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pneumologyz-1.1.tar", last modified: Thu May  9 13:23:36 2024, max compression
+gzip compressed data, was "pneumologyz-2.1.tar", last modified: Sat May 11 09:51:16 2024, max compression
```

## Comparing `pneumologyz-1.1.tar` & `pneumologyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 13:23:36.465486 pneumologyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-09 13:23:36.465486 pneumologyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 13:23:36.465486 pneumologyz-1.1/pneumologyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 13:23:36.033478 pneumologyz-1.1/pneumologyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 13:23:36.049478 pneumologyz-1.1/pneumologyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 13:23:36.033478 pneumologyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-09 13:23:36.053478 pneumologyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:51:16.256535 pneumologyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 13:23:36.000000 pneumologyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 09:51:16.256535 pneumologyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 13:23:36.000000 pneumologyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:51:16.256535 pneumologyz-2.1/pneumologyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 13:23:36.000000 pneumologyz-2.1/pneumologyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 13:23:36.000000 pneumologyz-2.1/pneumologyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:51:16.256535 pneumologyz-2.1/pneumologyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 09:51:15.000000 pneumologyz-2.1/pneumologyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-11 09:51:15.000000 pneumologyz-2.1/pneumologyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 09:51:15.000000 pneumologyz-2.1/pneumologyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 09:51:15.000000 pneumologyz-2.1/pneumologyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-11 09:51:15.000000 pneumologyz-2.1/pneumologyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 09:51:16.256535 pneumologyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-11 09:51:15.000000 pneumologyz-2.1/setup.py
```

### Comparing `pneumologyz-1.1/setup.py` & `pneumologyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'pneumologyz',
     packages = ['pneumologyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'pneumologyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/pneumologyz',
```

