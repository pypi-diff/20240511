# Comparing `tmp/pseudodemocraticz-1.1.tar.gz` & `tmp/pseudodemocraticz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pseudodemocraticz-1.1.tar", last modified: Thu May  9 18:30:27 2024, max compression
+gzip compressed data, was "pseudodemocraticz-2.1.tar", last modified: Sat May 11 11:50:35 2024, max compression
```

## Comparing `pseudodemocraticz-1.1.tar` & `pseudodemocraticz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 18:30:27.819963 pseudodemocraticz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1684 2024-05-09 18:30:27.819963 pseudodemocraticz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 18:30:27.819963 pseudodemocraticz-1.1/pseudodemocraticz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 18:30:27.647960 pseudodemocraticz-1.1/pseudodemocraticz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 18:30:27.659960 pseudodemocraticz-1.1/pseudodemocraticz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 18:30:27.647960 pseudodemocraticz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-09 18:30:27.671960 pseudodemocraticz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:50:35.052128 pseudodemocraticz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 18:30:27.000000 pseudodemocraticz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 11:50:35.052128 pseudodemocraticz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 18:30:27.000000 pseudodemocraticz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:50:35.048128 pseudodemocraticz-2.1/pseudodemocraticz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 18:30:27.000000 pseudodemocraticz-2.1/pseudodemocraticz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 18:30:27.000000 pseudodemocraticz-2.1/pseudodemocraticz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:50:35.052128 pseudodemocraticz-2.1/pseudodemocraticz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 11:50:34.000000 pseudodemocraticz-2.1/pseudodemocraticz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      296 2024-05-11 11:50:34.000000 pseudodemocraticz-2.1/pseudodemocraticz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 11:50:34.000000 pseudodemocraticz-2.1/pseudodemocraticz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 11:50:34.000000 pseudodemocraticz-2.1/pseudodemocraticz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       18 2024-05-11 11:50:34.000000 pseudodemocraticz-2.1/pseudodemocraticz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 11:50:35.052128 pseudodemocraticz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-11 11:50:28.000000 pseudodemocraticz-2.1/setup.py
```

### Comparing `pseudodemocraticz-1.1/setup.py` & `pseudodemocraticz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'pseudodemocraticz',
     packages = ['pseudodemocraticz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'pseudodemocraticz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/pseudodemocraticz',
```

