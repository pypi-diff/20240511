# Comparing `tmp/stegocephalousz-1.1.tar.gz` & `tmp/stegocephalousz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stegocephalousz-1.1.tar", last modified: Wed May  8 16:36:00 2024, max compression
+gzip compressed data, was "stegocephalousz-2.1.tar", last modified: Sat May 11 16:20:06 2024, max compression
```

## Comparing `stegocephalousz-1.1.tar` & `stegocephalousz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:36:00.079351 stegocephalousz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1676 2024-05-08 16:36:00.079351 stegocephalousz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 16:35:59.883347 stegocephalousz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-08 16:35:59.899348 stegocephalousz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:36:00.079351 stegocephalousz-1.1/stegocephalousz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:35:59.883347 stegocephalousz-1.1/stegocephalousz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:35:59.891348 stegocephalousz-1.1/stegocephalousz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:20:06.858926 stegocephalousz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 16:35:59.000000 stegocephalousz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 16:20:06.858926 stegocephalousz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 16:35:59.000000 stegocephalousz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 16:20:06.858926 stegocephalousz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-11 16:20:06.000000 stegocephalousz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:20:06.858926 stegocephalousz-2.1/stegocephalousz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:35:59.000000 stegocephalousz-2.1/stegocephalousz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:35:59.000000 stegocephalousz-2.1/stegocephalousz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:20:06.858926 stegocephalousz-2.1/stegocephalousz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 16:20:06.000000 stegocephalousz-2.1/stegocephalousz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      282 2024-05-11 16:20:06.000000 stegocephalousz-2.1/stegocephalousz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 16:20:06.000000 stegocephalousz-2.1/stegocephalousz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 16:20:06.000000 stegocephalousz-2.1/stegocephalousz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       16 2024-05-11 16:20:06.000000 stegocephalousz-2.1/stegocephalousz.egg-info/top_level.txt
```

### Comparing `stegocephalousz-1.1/setup.py` & `stegocephalousz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'stegocephalousz',
     packages = ['stegocephalousz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'stegocephalousz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/stegocephalousz',
```

