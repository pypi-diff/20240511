# Comparing `tmp/mastodonsz-1.1.tar.gz` & `tmp/mastodonsz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mastodonsz-1.1.tar", last modified: Thu May  9 06:35:38 2024, max compression
+gzip compressed data, was "mastodonsz-2.1.tar", last modified: Sat May 11 03:48:43 2024, max compression
```

## Comparing `mastodonsz-1.1.tar` & `mastodonsz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 06:35:38.250359 mastodonsz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 06:35:38.250359 mastodonsz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 06:35:38.250359 mastodonsz-1.1/mastodonsz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 06:35:38.050355 mastodonsz-1.1/mastodonsz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 06:35:38.066355 mastodonsz-1.1/mastodonsz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 06:35:38.050355 mastodonsz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 06:35:38.078355 mastodonsz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:48:43.092690 mastodonsz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 06:35:38.000000 mastodonsz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 03:48:43.092690 mastodonsz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 06:35:38.000000 mastodonsz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:48:43.068690 mastodonsz-2.1/mastodonsz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 06:35:38.000000 mastodonsz-2.1/mastodonsz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 06:35:38.000000 mastodonsz-2.1/mastodonsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:48:43.092690 mastodonsz-2.1/mastodonsz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 03:48:42.000000 mastodonsz-2.1/mastodonsz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 03:48:42.000000 mastodonsz-2.1/mastodonsz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 03:48:42.000000 mastodonsz-2.1/mastodonsz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 03:48:42.000000 mastodonsz-2.1/mastodonsz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 03:48:42.000000 mastodonsz-2.1/mastodonsz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 03:48:43.092690 mastodonsz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 03:48:37.000000 mastodonsz-2.1/setup.py
```

### Comparing `mastodonsz-1.1/setup.py` & `mastodonsz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'mastodonsz',
     packages = ['mastodonsz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'mastodonsz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/mastodonsz',
```

