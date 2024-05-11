# Comparing `tmp/organophonicz-1.1.tar.gz` & `tmp/organophonicz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "organophonicz-1.1.tar", last modified: Wed May  8 16:19:18 2024, max compression
+gzip compressed data, was "organophonicz-2.1.tar", last modified: Sat May 11 07:10:31 2024, max compression
```

## Comparing `organophonicz-1.1.tar` & `organophonicz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:19:18.136817 organophonicz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-08 16:19:18.136817 organophonicz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:19:18.136817 organophonicz-1.1/organophonicz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:19:10.404674 organophonicz-1.1/organophonicz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:19:10.748680 organophonicz-1.1/organophonicz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 16:19:10.404674 organophonicz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-08 16:19:11.340691 organophonicz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:10:31.459359 organophonicz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 16:19:10.000000 organophonicz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 07:10:31.459359 organophonicz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 16:19:10.000000 organophonicz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:10:31.459359 organophonicz-2.1/organophonicz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:19:10.000000 organophonicz-2.1/organophonicz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:19:10.000000 organophonicz-2.1/organophonicz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:10:31.459359 organophonicz-2.1/organophonicz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 07:10:31.000000 organophonicz-2.1/organophonicz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 07:10:31.000000 organophonicz-2.1/organophonicz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 07:10:31.000000 organophonicz-2.1/organophonicz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 07:10:31.000000 organophonicz-2.1/organophonicz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 07:10:31.000000 organophonicz-2.1/organophonicz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 07:10:31.459359 organophonicz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 07:10:30.000000 organophonicz-2.1/setup.py
```

### Comparing `organophonicz-1.1/setup.py` & `organophonicz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'organophonicz',
     packages = ['organophonicz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'organophonicz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/organophonicz',
```

