# Comparing `tmp/prefatorialz-1.1.tar.gz` & `tmp/prefatorialz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefatorialz-1.1.tar", last modified: Fri May 10 03:41:14 2024, max compression
+gzip compressed data, was "prefatorialz-2.1.tar", last modified: Sat May 11 10:52:59 2024, max compression
```

## Comparing `prefatorialz-1.1.tar` & `prefatorialz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 03:41:14.403962 prefatorialz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-10 03:41:14.403962 prefatorialz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 03:41:14.403962 prefatorialz-1.1/prefatorialz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 03:41:14.195958 prefatorialz-1.1/prefatorialz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 03:41:14.203959 prefatorialz-1.1/prefatorialz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 03:41:14.195958 prefatorialz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-10 03:41:14.215959 prefatorialz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:52:59.752961 prefatorialz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 03:41:14.000000 prefatorialz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 10:52:59.752961 prefatorialz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 03:41:14.000000 prefatorialz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:52:59.716961 prefatorialz-2.1/prefatorialz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 03:41:14.000000 prefatorialz-2.1/prefatorialz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 03:41:14.000000 prefatorialz-2.1/prefatorialz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:52:59.752961 prefatorialz-2.1/prefatorialz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 10:52:59.000000 prefatorialz-2.1/prefatorialz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 10:52:59.000000 prefatorialz-2.1/prefatorialz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 10:52:59.000000 prefatorialz-2.1/prefatorialz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 10:52:59.000000 prefatorialz-2.1/prefatorialz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 10:52:59.000000 prefatorialz-2.1/prefatorialz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 10:52:59.752961 prefatorialz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 10:52:53.000000 prefatorialz-2.1/setup.py
```

### Comparing `prefatorialz-1.1/setup.py` & `prefatorialz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'prefatorialz',
     packages = ['prefatorialz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'prefatorialz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/prefatorialz',
```

