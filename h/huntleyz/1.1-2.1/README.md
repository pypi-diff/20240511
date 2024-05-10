# Comparing `tmp/huntleyz-1.1.tar.gz` & `tmp/huntleyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huntleyz-1.1.tar", last modified: Thu May  9 10:47:30 2024, max compression
+gzip compressed data, was "huntleyz-2.1.tar", last modified: Fri May 10 22:56:59 2024, max compression
```

## Comparing `huntleyz-1.1.tar` & `huntleyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 10:47:30.028478 huntleyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-09 10:47:30.028478 huntleyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 10:47:30.028478 huntleyz-1.1/huntleyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 10:47:29.832474 huntleyz-1.1/huntleyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 10:47:29.844474 huntleyz-1.1/huntleyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 10:47:29.832474 huntleyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-09 10:47:29.860475 huntleyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 22:56:59.593758 huntleyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 10:47:29.000000 huntleyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 22:56:59.593758 huntleyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 10:47:29.000000 huntleyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 22:56:59.593758 huntleyz-2.1/huntleyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 10:47:29.000000 huntleyz-2.1/huntleyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 10:47:29.000000 huntleyz-2.1/huntleyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 22:56:59.593758 huntleyz-2.1/huntleyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 22:56:59.000000 huntleyz-2.1/huntleyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-10 22:56:59.000000 huntleyz-2.1/huntleyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 22:56:59.000000 huntleyz-2.1/huntleyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 22:56:59.000000 huntleyz-2.1/huntleyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-10 22:56:59.000000 huntleyz-2.1/huntleyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 22:56:59.593758 huntleyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 22:56:53.000000 huntleyz-2.1/setup.py
```

### Comparing `huntleyz-1.1/setup.py` & `huntleyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'huntleyz',
     packages = ['huntleyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'huntleyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/huntleyz',
```

