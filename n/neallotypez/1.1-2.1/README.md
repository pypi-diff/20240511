# Comparing `tmp/neallotypez-1.1.tar.gz` & `tmp/neallotypez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neallotypez-1.1.tar", last modified: Wed May  8 15:46:12 2024, max compression
+gzip compressed data, was "neallotypez-2.1.tar", last modified: Sat May 11 05:37:22 2024, max compression
```

## Comparing `neallotypez-1.1.tar` & `neallotypez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 15:46:11.984082 neallotypez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-08 15:46:11.984082 neallotypez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 15:46:11.984082 neallotypez-1.1/neallotypez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 15:46:08.612019 neallotypez-1.1/neallotypez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 15:46:08.872024 neallotypez-1.1/neallotypez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 15:46:08.612019 neallotypez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-08 15:46:09.208031 neallotypez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:37:22.068619 neallotypez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 15:46:08.000000 neallotypez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 05:37:22.068619 neallotypez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 15:46:08.000000 neallotypez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:37:22.064619 neallotypez-2.1/neallotypez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 15:46:08.000000 neallotypez-2.1/neallotypez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 15:46:08.000000 neallotypez-2.1/neallotypez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:37:22.068619 neallotypez-2.1/neallotypez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 05:37:21.000000 neallotypez-2.1/neallotypez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-11 05:37:21.000000 neallotypez-2.1/neallotypez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 05:37:21.000000 neallotypez-2.1/neallotypez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 05:37:21.000000 neallotypez-2.1/neallotypez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-11 05:37:21.000000 neallotypez-2.1/neallotypez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 05:37:22.068619 neallotypez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-11 05:37:20.000000 neallotypez-2.1/setup.py
```

### Comparing `neallotypez-1.1/setup.py` & `neallotypez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'neallotypez',
     packages = ['neallotypez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'neallotypez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/neallotypez',
```

