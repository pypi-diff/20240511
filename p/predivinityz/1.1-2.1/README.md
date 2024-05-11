# Comparing `tmp/predivinityz-1.1.tar.gz` & `tmp/predivinityz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predivinityz-1.1.tar", last modified: Wed May  8 17:52:12 2024, max compression
+gzip compressed data, was "predivinityz-2.1.tar", last modified: Sat May 11 10:47:41 2024, max compression
```

## Comparing `predivinityz-1.1.tar` & `predivinityz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 17:52:12.967713 predivinityz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-08 17:52:12.971713 predivinityz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 17:52:12.967713 predivinityz-1.1/predivinityz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 17:52:12.787710 predivinityz-1.1/predivinityz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 17:52:12.799710 predivinityz-1.1/predivinityz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 17:52:12.787710 predivinityz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-08 17:52:12.803710 predivinityz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:47:41.323090 predivinityz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 17:52:12.000000 predivinityz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 10:47:41.323090 predivinityz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 17:52:12.000000 predivinityz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:47:41.315090 predivinityz-2.1/predivinityz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 17:52:12.000000 predivinityz-2.1/predivinityz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 17:52:12.000000 predivinityz-2.1/predivinityz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:47:41.323090 predivinityz-2.1/predivinityz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 10:47:40.000000 predivinityz-2.1/predivinityz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 10:47:40.000000 predivinityz-2.1/predivinityz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 10:47:40.000000 predivinityz-2.1/predivinityz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 10:47:40.000000 predivinityz-2.1/predivinityz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 10:47:40.000000 predivinityz-2.1/predivinityz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 10:47:41.323090 predivinityz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 10:47:35.000000 predivinityz-2.1/setup.py
```

### Comparing `predivinityz-1.1/setup.py` & `predivinityz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'predivinityz',
     packages = ['predivinityz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'predivinityz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/predivinityz',
```

