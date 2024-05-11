# Comparing `tmp/spinozistz-1.1.tar.gz` & `tmp/spinozistz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinozistz-1.1.tar", last modified: Thu May  9 10:58:16 2024, max compression
+gzip compressed data, was "spinozistz-2.1.tar", last modified: Sat May 11 15:44:03 2024, max compression
```

## Comparing `spinozistz-1.1.tar` & `spinozistz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 10:58:16.504375 spinozistz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 10:58:16.504375 spinozistz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 10:58:16.312372 spinozistz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 10:58:16.332372 spinozistz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 10:58:16.504375 spinozistz-1.1/spinozistz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 10:58:16.312372 spinozistz-1.1/spinozistz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 10:58:16.320372 spinozistz-1.1/spinozistz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:44:03.774396 spinozistz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 10:58:16.000000 spinozistz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 15:44:03.770396 spinozistz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 10:58:16.000000 spinozistz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 15:44:03.774396 spinozistz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 15:43:58.000000 spinozistz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:44:03.742396 spinozistz-2.1/spinozistz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 10:58:16.000000 spinozistz-2.1/spinozistz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 10:58:16.000000 spinozistz-2.1/spinozistz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:44:03.770396 spinozistz-2.1/spinozistz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 15:44:03.000000 spinozistz-2.1/spinozistz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 15:44:03.000000 spinozistz-2.1/spinozistz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 15:44:03.000000 spinozistz-2.1/spinozistz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 15:44:03.000000 spinozistz-2.1/spinozistz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 15:44:03.000000 spinozistz-2.1/spinozistz.egg-info/top_level.txt
```

### Comparing `spinozistz-1.1/setup.py` & `spinozistz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'spinozistz',
     packages = ['spinozistz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'spinozistz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/spinozistz',
```

