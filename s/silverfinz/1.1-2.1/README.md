# Comparing `tmp/silverfinz-1.1.tar.gz` & `tmp/silverfinz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverfinz-1.1.tar", last modified: Wed May  8 23:18:13 2024, max compression
+gzip compressed data, was "silverfinz-2.1.tar", last modified: Sat May 11 15:12:43 2024, max compression
```

## Comparing `silverfinz-1.1.tar` & `silverfinz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 23:18:13.355560 silverfinz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 23:18:13.355560 silverfinz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 23:18:10.415506 silverfinz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 23:18:10.887515 silverfinz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 23:18:13.355560 silverfinz-1.1/silverfinz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 23:18:10.415506 silverfinz-1.1/silverfinz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 23:18:10.651511 silverfinz-1.1/silverfinz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:12:43.199713 silverfinz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 23:18:10.000000 silverfinz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 15:12:43.199713 silverfinz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 23:18:10.000000 silverfinz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 15:12:43.199713 silverfinz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 15:12:33.000000 silverfinz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:12:43.139712 silverfinz-2.1/silverfinz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 23:18:10.000000 silverfinz-2.1/silverfinz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 23:18:10.000000 silverfinz-2.1/silverfinz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:12:43.199713 silverfinz-2.1/silverfinz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 15:12:41.000000 silverfinz-2.1/silverfinz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 15:12:41.000000 silverfinz-2.1/silverfinz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 15:12:41.000000 silverfinz-2.1/silverfinz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 15:12:41.000000 silverfinz-2.1/silverfinz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 15:12:41.000000 silverfinz-2.1/silverfinz.egg-info/top_level.txt
```

### Comparing `silverfinz-1.1/setup.py` & `silverfinz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'silverfinz',
     packages = ['silverfinz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'silverfinz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/silverfinz',
```

