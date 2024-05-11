# Comparing `tmp/unquarteredz-1.1.tar.gz` & `tmp/unquarteredz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unquarteredz-1.1.tar", last modified: Thu May  9 20:21:22 2024, max compression
+gzip compressed data, was "unquarteredz-2.1.tar", last modified: Sat May 11 21:26:45 2024, max compression
```

## Comparing `unquarteredz-1.1.tar` & `unquarteredz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 20:21:22.818318 unquarteredz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 20:21:22.818318 unquarteredz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 20:21:22.630315 unquarteredz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 20:21:22.646315 unquarteredz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 20:21:22.818318 unquarteredz-1.1/unquarteredz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 20:21:22.630315 unquarteredz-1.1/unquarteredz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 20:21:22.638315 unquarteredz-1.1/unquarteredz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:26:45.285692 unquarteredz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 20:21:22.000000 unquarteredz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 21:26:45.285692 unquarteredz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 20:21:22.000000 unquarteredz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 21:26:45.285692 unquarteredz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 21:26:44.000000 unquarteredz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:26:45.285692 unquarteredz-2.1/unquarteredz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 20:21:22.000000 unquarteredz-2.1/unquarteredz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 20:21:22.000000 unquarteredz-2.1/unquarteredz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:26:45.285692 unquarteredz-2.1/unquarteredz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 21:26:45.000000 unquarteredz-2.1/unquarteredz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 21:26:45.000000 unquarteredz-2.1/unquarteredz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 21:26:45.000000 unquarteredz-2.1/unquarteredz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 21:26:45.000000 unquarteredz-2.1/unquarteredz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 21:26:45.000000 unquarteredz-2.1/unquarteredz.egg-info/top_level.txt
```

### Comparing `unquarteredz-1.1/setup.py` & `unquarteredz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'unquarteredz',
     packages = ['unquarteredz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'unquarteredz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/unquarteredz',
```

