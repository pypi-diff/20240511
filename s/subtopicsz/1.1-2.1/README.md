# Comparing `tmp/subtopicsz-1.1.tar.gz` & `tmp/subtopicsz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subtopicsz-1.1.tar", last modified: Thu May  9 00:17:48 2024, max compression
+gzip compressed data, was "subtopicsz-2.1.tar", last modified: Sat May 11 17:16:43 2024, max compression
```

## Comparing `subtopicsz-1.1.tar` & `subtopicsz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 00:17:48.029292 subtopicsz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 00:17:48.029292 subtopicsz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 00:17:47.845288 subtopicsz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 00:17:47.861289 subtopicsz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 00:17:48.029292 subtopicsz-1.1/subtopicsz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 00:17:47.845288 subtopicsz-1.1/subtopicsz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 00:17:47.853289 subtopicsz-1.1/subtopicsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:16:43.317313 subtopicsz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 00:17:47.000000 subtopicsz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 17:16:43.317313 subtopicsz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 00:17:47.000000 subtopicsz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 17:16:43.317313 subtopicsz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 17:16:37.000000 subtopicsz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:16:43.293313 subtopicsz-2.1/subtopicsz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 00:17:47.000000 subtopicsz-2.1/subtopicsz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 00:17:47.000000 subtopicsz-2.1/subtopicsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:16:43.317313 subtopicsz-2.1/subtopicsz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 17:16:43.000000 subtopicsz-2.1/subtopicsz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 17:16:43.000000 subtopicsz-2.1/subtopicsz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 17:16:43.000000 subtopicsz-2.1/subtopicsz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 17:16:43.000000 subtopicsz-2.1/subtopicsz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 17:16:43.000000 subtopicsz-2.1/subtopicsz.egg-info/top_level.txt
```

### Comparing `subtopicsz-1.1/setup.py` & `subtopicsz-2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'subtopicsz',
     packages = ['subtopicsz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'subtopicsz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/subtopicsz',
```

