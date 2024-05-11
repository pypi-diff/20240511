# Comparing `tmp/polygamistsz-1.1.tar.gz` & `tmp/polygamistsz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygamistsz-1.1.tar", last modified: Thu May  9 05:45:22 2024, max compression
+gzip compressed data, was "polygamistsz-2.1.tar", last modified: Sat May 11 09:56:19 2024, max compression
```

## Comparing `polygamistsz-1.1.tar` & `polygamistsz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:45:22.458768 polygamistsz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 05:45:22.458768 polygamistsz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:45:22.458768 polygamistsz-1.1/polygamistsz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:45:21.670753 polygamistsz-1.1/polygamistsz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:45:21.678753 polygamistsz-1.1/polygamistsz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 05:45:21.670753 polygamistsz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 05:45:21.686753 polygamistsz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:56:19.990119 polygamistsz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 05:45:21.000000 polygamistsz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 09:56:19.990119 polygamistsz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 05:45:21.000000 polygamistsz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:56:19.986118 polygamistsz-2.1/polygamistsz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:45:21.000000 polygamistsz-2.1/polygamistsz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:45:21.000000 polygamistsz-2.1/polygamistsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:56:19.990119 polygamistsz-2.1/polygamistsz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 09:56:19.000000 polygamistsz-2.1/polygamistsz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 09:56:19.000000 polygamistsz-2.1/polygamistsz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 09:56:19.000000 polygamistsz-2.1/polygamistsz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 09:56:19.000000 polygamistsz-2.1/polygamistsz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 09:56:19.000000 polygamistsz-2.1/polygamistsz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 09:56:19.990119 polygamistsz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 09:56:19.000000 polygamistsz-2.1/setup.py
```

### Comparing `polygamistsz-1.1/setup.py` & `polygamistsz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'polygamistsz',
     packages = ['polygamistsz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'polygamistsz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/polygamistsz',
```

