# Comparing `tmp/omphalospinousz-1.1.tar.gz` & `tmp/omphalospinousz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omphalospinousz-1.1.tar", last modified: Wed May  8 16:02:40 2024, max compression
+gzip compressed data, was "omphalospinousz-2.1.tar", last modified: Sat May 11 06:54:47 2024, max compression
```

## Comparing `omphalospinousz-1.1.tar` & `omphalospinousz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:02:40.118302 omphalospinousz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1676 2024-05-08 16:02:40.118302 omphalospinousz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:02:40.118302 omphalospinousz-1.1/omphalospinousz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:02:36.802241 omphalospinousz-1.1/omphalospinousz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:02:37.014245 omphalospinousz-1.1/omphalospinousz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 16:02:36.802241 omphalospinousz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-08 16:02:37.374252 omphalospinousz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:54:47.205870 omphalospinousz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 16:02:36.000000 omphalospinousz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 06:54:47.205870 omphalospinousz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 16:02:36.000000 omphalospinousz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:54:47.201870 omphalospinousz-2.1/omphalospinousz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:02:36.000000 omphalospinousz-2.1/omphalospinousz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:02:37.000000 omphalospinousz-2.1/omphalospinousz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:54:47.205870 omphalospinousz-2.1/omphalospinousz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 06:54:47.000000 omphalospinousz-2.1/omphalospinousz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      282 2024-05-11 06:54:47.000000 omphalospinousz-2.1/omphalospinousz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 06:54:47.000000 omphalospinousz-2.1/omphalospinousz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 06:54:47.000000 omphalospinousz-2.1/omphalospinousz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       16 2024-05-11 06:54:47.000000 omphalospinousz-2.1/omphalospinousz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 06:54:47.205870 omphalospinousz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-11 06:54:46.000000 omphalospinousz-2.1/setup.py
```

### Comparing `omphalospinousz-1.1/setup.py` & `omphalospinousz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'omphalospinousz',
     packages = ['omphalospinousz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'omphalospinousz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/omphalospinousz',
```

