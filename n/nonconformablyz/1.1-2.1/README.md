# Comparing `tmp/nonconformablyz-1.1.tar.gz` & `tmp/nonconformablyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonconformablyz-1.1.tar", last modified: Thu May  9 21:20:18 2024, max compression
+gzip compressed data, was "nonconformablyz-2.1.tar", last modified: Sat May 11 05:57:51 2024, max compression
```

## Comparing `nonconformablyz-1.1.tar` & `nonconformablyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 21:20:18.607243 nonconformablyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1676 2024-05-09 21:20:18.611243 nonconformablyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 21:20:18.607243 nonconformablyz-1.1/nonconformablyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 21:20:15.771190 nonconformablyz-1.1/nonconformablyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 21:20:15.979194 nonconformablyz-1.1/nonconformablyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 21:20:15.771190 nonconformablyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-09 21:20:16.291200 nonconformablyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:57:51.155338 nonconformablyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 21:20:15.000000 nonconformablyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 05:57:51.155338 nonconformablyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 21:20:15.000000 nonconformablyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:57:51.111337 nonconformablyz-2.1/nonconformablyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 21:20:15.000000 nonconformablyz-2.1/nonconformablyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 21:20:15.000000 nonconformablyz-2.1/nonconformablyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:57:51.155338 nonconformablyz-2.1/nonconformablyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 05:57:50.000000 nonconformablyz-2.1/nonconformablyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      282 2024-05-11 05:57:50.000000 nonconformablyz-2.1/nonconformablyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 05:57:50.000000 nonconformablyz-2.1/nonconformablyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 05:57:50.000000 nonconformablyz-2.1/nonconformablyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       16 2024-05-11 05:57:50.000000 nonconformablyz-2.1/nonconformablyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 05:57:51.155338 nonconformablyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-11 05:57:44.000000 nonconformablyz-2.1/setup.py
```

### Comparing `nonconformablyz-1.1/setup.py` & `nonconformablyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'nonconformablyz',
     packages = ['nonconformablyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'nonconformablyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/nonconformablyz',
```

