# Comparing `tmp/plectridiumz-1.1.tar.gz` & `tmp/plectridiumz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plectridiumz-1.1.tar", last modified: Fri May 10 03:02:29 2024, max compression
+gzip compressed data, was "plectridiumz-2.1.tar", last modified: Sat May 11 09:41:06 2024, max compression
```

## Comparing `plectridiumz-1.1.tar` & `plectridiumz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 03:02:28.753281 plectridiumz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-10 03:02:28.753281 plectridiumz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 03:02:28.753281 plectridiumz-1.1/plectridiumz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 03:02:23.501184 plectridiumz-1.1/plectridiumz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 03:02:23.805189 plectridiumz-1.1/plectridiumz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 03:02:23.501184 plectridiumz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-10 03:02:23.981192 plectridiumz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:41:06.653325 plectridiumz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 03:02:23.000000 plectridiumz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 09:41:06.653325 plectridiumz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 03:02:23.000000 plectridiumz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:41:06.649325 plectridiumz-2.1/plectridiumz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 03:02:23.000000 plectridiumz-2.1/plectridiumz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 03:02:23.000000 plectridiumz-2.1/plectridiumz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:41:06.653325 plectridiumz-2.1/plectridiumz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 09:41:06.000000 plectridiumz-2.1/plectridiumz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 09:41:06.000000 plectridiumz-2.1/plectridiumz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 09:41:06.000000 plectridiumz-2.1/plectridiumz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 09:41:06.000000 plectridiumz-2.1/plectridiumz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 09:41:06.000000 plectridiumz-2.1/plectridiumz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 09:41:06.653325 plectridiumz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 09:40:57.000000 plectridiumz-2.1/setup.py
```

### Comparing `plectridiumz-1.1/setup.py` & `plectridiumz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'plectridiumz',
     packages = ['plectridiumz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'plectridiumz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/plectridiumz',
```

