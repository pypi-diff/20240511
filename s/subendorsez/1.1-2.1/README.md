# Comparing `tmp/subendorsez-1.1.tar.gz` & `tmp/subendorsez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subendorsez-1.1.tar", last modified: Thu May  9 16:52:27 2024, max compression
+gzip compressed data, was "subendorsez-2.1.tar", last modified: Sat May 11 16:56:03 2024, max compression
```

## Comparing `subendorsez-1.1.tar` & `subendorsez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 16:52:27.143725 subendorsez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-09 16:52:27.143725 subendorsez-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 16:52:23.831664 subendorsez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-09 16:52:24.331673 subendorsez-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 16:52:27.143725 subendorsez-1.1/subendorsez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 16:52:23.831664 subendorsez-1.1/subendorsez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 16:52:24.079668 subendorsez-1.1/subendorsez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:56:03.214400 subendorsez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 16:52:23.000000 subendorsez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 16:56:03.214400 subendorsez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 16:52:23.000000 subendorsez-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 16:56:03.214400 subendorsez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-11 16:56:02.000000 subendorsez-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:56:03.214400 subendorsez-2.1/subendorsez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 16:52:23.000000 subendorsez-2.1/subendorsez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 16:52:24.000000 subendorsez-2.1/subendorsez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:56:03.214400 subendorsez-2.1/subendorsez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 16:56:03.000000 subendorsez-2.1/subendorsez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-11 16:56:03.000000 subendorsez-2.1/subendorsez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 16:56:03.000000 subendorsez-2.1/subendorsez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 16:56:03.000000 subendorsez-2.1/subendorsez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-11 16:56:03.000000 subendorsez-2.1/subendorsez.egg-info/top_level.txt
```

### Comparing `subendorsez-1.1/setup.py` & `subendorsez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'subendorsez',
     packages = ['subendorsez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'subendorsez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/subendorsez',
```

