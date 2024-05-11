# Comparing `tmp/unriggedz-1.1.tar.gz` & `tmp/unriggedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unriggedz-1.1.tar", last modified: Thu May  9 17:31:05 2024, max compression
+gzip compressed data, was "unriggedz-2.1.tar", last modified: Sat May 11 21:31:56 2024, max compression
```

## Comparing `unriggedz-1.1.tar` & `unriggedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 17:31:05.058383 unriggedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-09 17:31:05.058383 unriggedz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 17:31:01.986326 unriggedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-09 17:31:02.378333 unriggedz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 17:31:05.058383 unriggedz-1.1/unriggedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 17:31:01.986326 unriggedz-1.1/unriggedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 17:31:02.118328 unriggedz-1.1/unriggedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:31:56.567424 unriggedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 17:31:01.000000 unriggedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 21:31:56.567424 unriggedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 17:31:01.000000 unriggedz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 21:31:56.567424 unriggedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-11 21:31:50.000000 unriggedz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:31:56.567424 unriggedz-2.1/unriggedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 17:31:01.000000 unriggedz-2.1/unriggedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 17:31:02.000000 unriggedz-2.1/unriggedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:31:56.567424 unriggedz-2.1/unriggedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 21:31:55.000000 unriggedz-2.1/unriggedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-11 21:31:55.000000 unriggedz-2.1/unriggedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 21:31:55.000000 unriggedz-2.1/unriggedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 21:31:55.000000 unriggedz-2.1/unriggedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-11 21:31:55.000000 unriggedz-2.1/unriggedz.egg-info/top_level.txt
```

### Comparing `unriggedz-1.1/setup.py` & `unriggedz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'unriggedz',
     packages = ['unriggedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'unriggedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/unriggedz',
```

