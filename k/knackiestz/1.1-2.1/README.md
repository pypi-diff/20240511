# Comparing `tmp/knackiestz-1.1.tar.gz` & `tmp/knackiestz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knackiestz-1.1.tar", last modified: Thu May  9 00:39:21 2024, max compression
+gzip compressed data, was "knackiestz-2.1.tar", last modified: Sat May 11 01:28:23 2024, max compression
```

## Comparing `knackiestz-1.1.tar` & `knackiestz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 00:39:21.521069 knackiestz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 00:39:21.521069 knackiestz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 00:39:21.521069 knackiestz-1.1/knackiestz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 00:39:18.057005 knackiestz-1.1/knackiestz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 00:39:18.185008 knackiestz-1.1/knackiestz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 00:39:18.053005 knackiestz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 00:39:18.657016 knackiestz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:28:23.749846 knackiestz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 00:39:18.000000 knackiestz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 01:28:23.749846 knackiestz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 00:39:18.000000 knackiestz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:28:23.721845 knackiestz-2.1/knackiestz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 00:39:18.000000 knackiestz-2.1/knackiestz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 00:39:18.000000 knackiestz-2.1/knackiestz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:28:23.749846 knackiestz-2.1/knackiestz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 01:28:23.000000 knackiestz-2.1/knackiestz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 01:28:23.000000 knackiestz-2.1/knackiestz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 01:28:23.000000 knackiestz-2.1/knackiestz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 01:28:23.000000 knackiestz-2.1/knackiestz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 01:28:23.000000 knackiestz-2.1/knackiestz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 01:28:23.749846 knackiestz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 01:28:23.000000 knackiestz-2.1/setup.py
```

### Comparing `knackiestz-1.1/setup.py` & `knackiestz-2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'knackiestz',
     packages = ['knackiestz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'knackiestz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/knackiestz',
```

