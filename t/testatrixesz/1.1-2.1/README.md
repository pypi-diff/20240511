# Comparing `tmp/testatrixesz-1.1.tar.gz` & `tmp/testatrixesz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testatrixesz-1.1.tar", last modified: Thu May  9 12:25:38 2024, max compression
+gzip compressed data, was "testatrixesz-2.1.tar", last modified: Sat May 11 18:34:40 2024, max compression
```

## Comparing `testatrixesz-1.1.tar` & `testatrixesz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 12:25:38.241197 testatrixesz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 12:25:38.241197 testatrixesz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 12:25:35.001137 testatrixesz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 12:25:35.493146 testatrixesz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 12:25:38.241197 testatrixesz-1.1/testatrixesz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 12:25:35.001137 testatrixesz-1.1/testatrixesz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 12:25:35.297142 testatrixesz-1.1/testatrixesz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:34:40.659548 testatrixesz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 12:25:35.000000 testatrixesz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 18:34:40.659548 testatrixesz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 12:25:35.000000 testatrixesz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 18:34:40.659548 testatrixesz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 18:34:40.000000 testatrixesz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:34:40.659548 testatrixesz-2.1/testatrixesz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 12:25:35.000000 testatrixesz-2.1/testatrixesz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 12:25:35.000000 testatrixesz-2.1/testatrixesz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:34:40.659548 testatrixesz-2.1/testatrixesz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 18:34:40.000000 testatrixesz-2.1/testatrixesz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 18:34:40.000000 testatrixesz-2.1/testatrixesz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 18:34:40.000000 testatrixesz-2.1/testatrixesz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 18:34:40.000000 testatrixesz-2.1/testatrixesz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 18:34:40.000000 testatrixesz-2.1/testatrixesz.egg-info/top_level.txt
```

### Comparing `testatrixesz-1.1/setup.py` & `testatrixesz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'testatrixesz',
     packages = ['testatrixesz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'testatrixesz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/testatrixesz',
```

