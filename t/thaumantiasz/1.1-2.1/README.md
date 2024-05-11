# Comparing `tmp/thaumantiasz-1.1.tar.gz` & `tmp/thaumantiasz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thaumantiasz-1.1.tar", last modified: Thu May  9 01:01:47 2024, max compression
+gzip compressed data, was "thaumantiasz-2.1.tar", last modified: Sat May 11 18:45:06 2024, max compression
```

## Comparing `thaumantiasz-1.1.tar` & `thaumantiasz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:01:47.778183 thaumantiasz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 01:01:47.778183 thaumantiasz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 01:01:41.946075 thaumantiasz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 01:01:43.014095 thaumantiasz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:01:47.778183 thaumantiasz-1.1/thaumantiasz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:01:41.946075 thaumantiasz-1.1/thaumantiasz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:01:42.354083 thaumantiasz-1.1/thaumantiasz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:45:05.939073 thaumantiasz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 01:01:41.000000 thaumantiasz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 18:45:05.939073 thaumantiasz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 01:01:41.000000 thaumantiasz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 18:45:05.939073 thaumantiasz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 18:44:52.000000 thaumantiasz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:45:05.919072 thaumantiasz-2.1/thaumantiasz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:01:41.000000 thaumantiasz-2.1/thaumantiasz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:01:42.000000 thaumantiasz-2.1/thaumantiasz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:45:05.939073 thaumantiasz-2.1/thaumantiasz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 18:45:04.000000 thaumantiasz-2.1/thaumantiasz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 18:45:04.000000 thaumantiasz-2.1/thaumantiasz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 18:45:04.000000 thaumantiasz-2.1/thaumantiasz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 18:45:04.000000 thaumantiasz-2.1/thaumantiasz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 18:45:04.000000 thaumantiasz-2.1/thaumantiasz.egg-info/top_level.txt
```

### Comparing `thaumantiasz-1.1/setup.py` & `thaumantiasz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'thaumantiasz',
     packages = ['thaumantiasz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'thaumantiasz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/thaumantiasz',
```

