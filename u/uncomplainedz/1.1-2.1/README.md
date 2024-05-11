# Comparing `tmp/uncomplainedz-1.1.tar.gz` & `tmp/uncomplainedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uncomplainedz-1.1.tar", last modified: Wed May  8 19:18:52 2024, max compression
+gzip compressed data, was "uncomplainedz-2.1.tar", last modified: Sat May 11 20:29:04 2024, max compression
```

## Comparing `uncomplainedz-1.1.tar` & `uncomplainedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 19:18:52.071375 uncomplainedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-08 19:18:52.071375 uncomplainedz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 19:18:51.887371 uncomplainedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-08 19:18:51.903371 uncomplainedz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 19:18:52.071375 uncomplainedz-1.1/uncomplainedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 19:18:51.887371 uncomplainedz-1.1/uncomplainedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 19:18:51.895371 uncomplainedz-1.1/uncomplainedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:29:04.057970 uncomplainedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 19:18:51.000000 uncomplainedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 20:29:04.057970 uncomplainedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 19:18:51.000000 uncomplainedz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 20:29:04.057970 uncomplainedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 20:28:58.000000 uncomplainedz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:29:04.057970 uncomplainedz-2.1/uncomplainedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 19:18:51.000000 uncomplainedz-2.1/uncomplainedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 19:18:51.000000 uncomplainedz-2.1/uncomplainedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:29:04.057970 uncomplainedz-2.1/uncomplainedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 20:29:03.000000 uncomplainedz-2.1/uncomplainedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 20:29:03.000000 uncomplainedz-2.1/uncomplainedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 20:29:03.000000 uncomplainedz-2.1/uncomplainedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 20:29:03.000000 uncomplainedz-2.1/uncomplainedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 20:29:03.000000 uncomplainedz-2.1/uncomplainedz.egg-info/top_level.txt
```

### Comparing `uncomplainedz-1.1/setup.py` & `uncomplainedz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'uncomplainedz',
     packages = ['uncomplainedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'uncomplainedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/uncomplainedz',
```

