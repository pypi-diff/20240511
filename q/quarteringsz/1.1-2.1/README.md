# Comparing `tmp/quarteringsz-1.1.tar.gz` & `tmp/quarteringsz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quarteringsz-1.1.tar", last modified: Thu May  9 02:44:48 2024, max compression
+gzip compressed data, was "quarteringsz-2.1.tar", last modified: Sat May 11 12:32:02 2024, max compression
```

## Comparing `quarteringsz-1.1.tar` & `quarteringsz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:44:48.911467 quarteringsz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 02:44:48.911467 quarteringsz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:44:48.911467 quarteringsz-1.1/quarteringsz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:44:46.295420 quarteringsz-1.1/quarteringsz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:44:46.467423 quarteringsz-1.1/quarteringsz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 02:44:46.291420 quarteringsz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 02:44:46.807429 quarteringsz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 12:32:02.370163 quarteringsz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 02:44:46.000000 quarteringsz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 12:32:02.370163 quarteringsz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 02:44:46.000000 quarteringsz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 12:32:02.370163 quarteringsz-2.1/quarteringsz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:44:46.000000 quarteringsz-2.1/quarteringsz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:44:46.000000 quarteringsz-2.1/quarteringsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 12:32:02.370163 quarteringsz-2.1/quarteringsz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 12:32:01.000000 quarteringsz-2.1/quarteringsz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 12:32:01.000000 quarteringsz-2.1/quarteringsz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 12:32:01.000000 quarteringsz-2.1/quarteringsz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 12:32:01.000000 quarteringsz-2.1/quarteringsz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 12:32:01.000000 quarteringsz-2.1/quarteringsz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 12:32:02.370163 quarteringsz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 12:31:56.000000 quarteringsz-2.1/setup.py
```

### Comparing `quarteringsz-1.1/setup.py` & `quarteringsz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'quarteringsz',
     packages = ['quarteringsz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'quarteringsz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/quarteringsz',
```

