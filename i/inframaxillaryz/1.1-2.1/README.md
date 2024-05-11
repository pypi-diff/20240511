# Comparing `tmp/inframaxillaryz-1.1.tar.gz` & `tmp/inframaxillaryz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inframaxillaryz-1.1.tar", last modified: Wed May  8 21:46:50 2024, max compression
+gzip compressed data, was "inframaxillaryz-2.1.tar", last modified: Sat May 11 00:10:20 2024, max compression
```

## Comparing `inframaxillaryz-1.1.tar` & `inframaxillaryz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 21:46:50.266754 inframaxillaryz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1676 2024-05-08 21:46:50.266754 inframaxillaryz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 21:46:50.266754 inframaxillaryz-1.1/inframaxillaryz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 21:46:47.338701 inframaxillaryz-1.1/inframaxillaryz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 21:46:47.510704 inframaxillaryz-1.1/inframaxillaryz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 21:46:47.338701 inframaxillaryz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-08 21:46:47.706707 inframaxillaryz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:10:20.599569 inframaxillaryz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 21:46:47.000000 inframaxillaryz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 00:10:20.599569 inframaxillaryz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 21:46:47.000000 inframaxillaryz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:10:20.599569 inframaxillaryz-2.1/inframaxillaryz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 21:46:47.000000 inframaxillaryz-2.1/inframaxillaryz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 21:46:47.000000 inframaxillaryz-2.1/inframaxillaryz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:10:20.599569 inframaxillaryz-2.1/inframaxillaryz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 00:10:19.000000 inframaxillaryz-2.1/inframaxillaryz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      282 2024-05-11 00:10:19.000000 inframaxillaryz-2.1/inframaxillaryz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 00:10:19.000000 inframaxillaryz-2.1/inframaxillaryz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 00:10:19.000000 inframaxillaryz-2.1/inframaxillaryz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       16 2024-05-11 00:10:19.000000 inframaxillaryz-2.1/inframaxillaryz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 00:10:20.599569 inframaxillaryz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-11 00:10:13.000000 inframaxillaryz-2.1/setup.py
```

### Comparing `inframaxillaryz-1.1/setup.py` & `inframaxillaryz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'inframaxillaryz',
     packages = ['inframaxillaryz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'inframaxillaryz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/inframaxillaryz',
```

