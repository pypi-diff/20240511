# Comparing `tmp/sulkierz-1.1.tar.gz` & `tmp/sulkierz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sulkierz-1.1.tar", last modified: Thu May  9 01:28:57 2024, max compression
+gzip compressed data, was "sulkierz-2.1.tar", last modified: Sat May 11 17:32:08 2024, max compression
```

## Comparing `sulkierz-1.1.tar` & `sulkierz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:28:57.044283 sulkierz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-09 01:28:57.044283 sulkierz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 01:28:54.520236 sulkierz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-09 01:28:54.936244 sulkierz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:28:57.044283 sulkierz-1.1/sulkierz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:28:54.520236 sulkierz-1.1/sulkierz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:28:54.664239 sulkierz-1.1/sulkierz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:32:08.874414 sulkierz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 01:28:54.000000 sulkierz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 17:32:08.874414 sulkierz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 01:28:54.000000 sulkierz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 17:32:08.874414 sulkierz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-11 17:32:08.000000 sulkierz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:32:08.870414 sulkierz-2.1/sulkierz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:28:54.000000 sulkierz-2.1/sulkierz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:28:54.000000 sulkierz-2.1/sulkierz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:32:08.874414 sulkierz-2.1/sulkierz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 17:32:08.000000 sulkierz-2.1/sulkierz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-11 17:32:08.000000 sulkierz-2.1/sulkierz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 17:32:08.000000 sulkierz-2.1/sulkierz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 17:32:08.000000 sulkierz-2.1/sulkierz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-11 17:32:08.000000 sulkierz-2.1/sulkierz.egg-info/top_level.txt
```

### Comparing `sulkierz-1.1/setup.py` & `sulkierz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'sulkierz',
     packages = ['sulkierz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'sulkierz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/sulkierz',
```

