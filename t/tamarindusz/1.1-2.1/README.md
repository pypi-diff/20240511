# Comparing `tmp/tamarindusz-1.1.tar.gz` & `tmp/tamarindusz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamarindusz-1.1.tar", last modified: Thu May  9 03:23:18 2024, max compression
+gzip compressed data, was "tamarindusz-2.1.tar", last modified: Sat May 11 18:03:46 2024, max compression
```

## Comparing `tamarindusz-1.1.tar` & `tamarindusz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 03:23:18.253937 tamarindusz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-09 03:23:18.253937 tamarindusz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 03:23:17.933931 tamarindusz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-09 03:23:17.945931 tamarindusz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 03:23:18.253937 tamarindusz-1.1/tamarindusz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 03:23:17.933931 tamarindusz-1.1/tamarindusz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 03:23:17.941931 tamarindusz-1.1/tamarindusz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:03:46.045400 tamarindusz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 03:23:17.000000 tamarindusz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 18:03:46.045400 tamarindusz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 03:23:17.000000 tamarindusz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 18:03:46.045400 tamarindusz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-11 18:03:38.000000 tamarindusz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:03:46.045400 tamarindusz-2.1/tamarindusz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 03:23:17.000000 tamarindusz-2.1/tamarindusz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 03:23:17.000000 tamarindusz-2.1/tamarindusz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:03:46.045400 tamarindusz-2.1/tamarindusz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 18:03:45.000000 tamarindusz-2.1/tamarindusz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-11 18:03:45.000000 tamarindusz-2.1/tamarindusz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 18:03:45.000000 tamarindusz-2.1/tamarindusz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 18:03:45.000000 tamarindusz-2.1/tamarindusz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-11 18:03:45.000000 tamarindusz-2.1/tamarindusz.egg-info/top_level.txt
```

### Comparing `tamarindusz-1.1/setup.py` & `tamarindusz-2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'tamarindusz',
     packages = ['tamarindusz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'tamarindusz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/tamarindusz',
```

