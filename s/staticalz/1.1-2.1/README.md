# Comparing `tmp/staticalz-1.1.tar.gz` & `tmp/staticalz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staticalz-1.1.tar", last modified: Wed May  8 17:25:04 2024, max compression
+gzip compressed data, was "staticalz-2.1.tar", last modified: Sat May 11 16:15:00 2024, max compression
```

## Comparing `staticalz-1.1.tar` & `staticalz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 17:25:04.281784 staticalz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-08 17:25:04.281784 staticalz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 17:25:04.109781 staticalz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-08 17:25:04.125781 staticalz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 17:25:04.281784 staticalz-1.1/staticalz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 17:25:04.109781 staticalz-1.1/staticalz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 17:25:04.117781 staticalz-1.1/staticalz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:15:00.317222 staticalz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 17:25:04.000000 staticalz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 16:15:00.317222 staticalz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 17:25:04.000000 staticalz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 16:15:00.321222 staticalz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-11 16:14:59.000000 staticalz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:15:00.317222 staticalz-2.1/staticalz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 17:25:04.000000 staticalz-2.1/staticalz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 17:25:04.000000 staticalz-2.1/staticalz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:15:00.317222 staticalz-2.1/staticalz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 16:15:00.000000 staticalz-2.1/staticalz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-11 16:15:00.000000 staticalz-2.1/staticalz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 16:15:00.000000 staticalz-2.1/staticalz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 16:15:00.000000 staticalz-2.1/staticalz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-11 16:15:00.000000 staticalz-2.1/staticalz.egg-info/top_level.txt
```

### Comparing `staticalz-1.1/setup.py` & `staticalz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'staticalz',
     packages = ['staticalz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'staticalz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/staticalz',
```

