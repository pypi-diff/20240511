# Comparing `tmp/uncoachablez-1.1.tar.gz` & `tmp/uncoachablez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uncoachablez-1.1.tar", last modified: Thu May  9 11:41:26 2024, max compression
+gzip compressed data, was "uncoachablez-2.1.tar", last modified: Sat May 11 20:23:48 2024, max compression
```

## Comparing `uncoachablez-1.1.tar` & `uncoachablez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 11:41:25.948017 uncoachablez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 11:41:25.948017 uncoachablez-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 11:41:21.867942 uncoachablez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 11:41:22.607956 uncoachablez-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 11:41:25.948017 uncoachablez-1.1/uncoachablez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 11:41:21.867942 uncoachablez-1.1/uncoachablez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 11:41:22.187948 uncoachablez-1.1/uncoachablez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:23:48.068164 uncoachablez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 11:41:21.000000 uncoachablez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 20:23:48.068164 uncoachablez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 11:41:21.000000 uncoachablez-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 20:23:48.068164 uncoachablez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 20:23:40.000000 uncoachablez-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:23:48.068164 uncoachablez-2.1/uncoachablez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 11:41:21.000000 uncoachablez-2.1/uncoachablez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 11:41:22.000000 uncoachablez-2.1/uncoachablez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:23:48.068164 uncoachablez-2.1/uncoachablez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 20:23:47.000000 uncoachablez-2.1/uncoachablez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 20:23:47.000000 uncoachablez-2.1/uncoachablez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 20:23:47.000000 uncoachablez-2.1/uncoachablez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 20:23:47.000000 uncoachablez-2.1/uncoachablez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 20:23:47.000000 uncoachablez-2.1/uncoachablez.egg-info/top_level.txt
```

### Comparing `uncoachablez-1.1/setup.py` & `uncoachablez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'uncoachablez',
     packages = ['uncoachablez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'uncoachablez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/uncoachablez',
```

