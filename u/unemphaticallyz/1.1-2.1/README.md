# Comparing `tmp/unemphaticallyz-1.1.tar.gz` & `tmp/unemphaticallyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unemphaticallyz-1.1.tar", last modified: Thu May  9 02:07:27 2024, max compression
+gzip compressed data, was "unemphaticallyz-2.1.tar", last modified: Sat May 11 20:50:15 2024, max compression
```

## Comparing `unemphaticallyz-1.1.tar` & `unemphaticallyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:07:27.414929 unemphaticallyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1676 2024-05-09 02:07:27.414929 unemphaticallyz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 02:07:27.210925 unemphaticallyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-09 02:07:27.234926 unemphaticallyz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:07:27.414929 unemphaticallyz-1.1/unemphaticallyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:07:27.210925 unemphaticallyz-1.1/unemphaticallyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:07:27.214925 unemphaticallyz-1.1/unemphaticallyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:50:15.701374 unemphaticallyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 02:07:27.000000 unemphaticallyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 20:50:15.701374 unemphaticallyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 02:07:27.000000 unemphaticallyz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 20:50:15.701374 unemphaticallyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-11 20:50:02.000000 unemphaticallyz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:50:15.657373 unemphaticallyz-2.1/unemphaticallyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:07:27.000000 unemphaticallyz-2.1/unemphaticallyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:07:27.000000 unemphaticallyz-2.1/unemphaticallyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:50:15.701374 unemphaticallyz-2.1/unemphaticallyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 20:50:13.000000 unemphaticallyz-2.1/unemphaticallyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      282 2024-05-11 20:50:13.000000 unemphaticallyz-2.1/unemphaticallyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 20:50:13.000000 unemphaticallyz-2.1/unemphaticallyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 20:50:13.000000 unemphaticallyz-2.1/unemphaticallyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       16 2024-05-11 20:50:13.000000 unemphaticallyz-2.1/unemphaticallyz.egg-info/top_level.txt
```

### Comparing `unemphaticallyz-1.1/setup.py` & `unemphaticallyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'unemphaticallyz',
     packages = ['unemphaticallyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'unemphaticallyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/unemphaticallyz',
```

