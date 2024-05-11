# Comparing `tmp/thingutz-1.1.tar.gz` & `tmp/thingutz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingutz-1.1.tar", last modified: Wed May  8 15:24:53 2024, max compression
+gzip compressed data, was "thingutz-2.1.tar", last modified: Sat May 11 19:00:43 2024, max compression
```

## Comparing `thingutz-1.1.tar` & `thingutz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 15:24:53.396481 thingutz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-08 15:24:53.396481 thingutz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 15:24:53.224478 thingutz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-08 15:24:53.240478 thingutz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 15:24:53.396481 thingutz-1.1/thingutz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 15:24:53.224478 thingutz-1.1/thingutz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 15:24:53.232478 thingutz-1.1/thingutz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:00:43.708356 thingutz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 15:24:53.000000 thingutz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 19:00:43.708356 thingutz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 15:24:53.000000 thingutz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 19:00:43.712356 thingutz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-11 19:00:43.000000 thingutz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:00:43.708356 thingutz-2.1/thingutz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 15:24:53.000000 thingutz-2.1/thingutz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 15:24:53.000000 thingutz-2.1/thingutz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:00:43.708356 thingutz-2.1/thingutz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 19:00:43.000000 thingutz-2.1/thingutz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-11 19:00:43.000000 thingutz-2.1/thingutz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 19:00:43.000000 thingutz-2.1/thingutz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 19:00:43.000000 thingutz-2.1/thingutz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-11 19:00:43.000000 thingutz-2.1/thingutz.egg-info/top_level.txt
```

### Comparing `thingutz-1.1/setup.py` & `thingutz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'thingutz',
     packages = ['thingutz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'thingutz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/thingutz',
```

