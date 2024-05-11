# Comparing `tmp/oklahomanz-1.1.tar.gz` & `tmp/oklahomanz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oklahomanz-1.1.tar", last modified: Thu May  9 13:02:53 2024, max compression
+gzip compressed data, was "oklahomanz-2.1.tar", last modified: Sat May 11 06:49:38 2024, max compression
```

## Comparing `oklahomanz-1.1.tar` & `oklahomanz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 13:02:53.174514 oklahomanz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 13:02:53.174514 oklahomanz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 13:02:53.174514 oklahomanz-1.1/oklahomanz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 13:02:52.998511 oklahomanz-1.1/oklahomanz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 13:02:53.006511 oklahomanz-1.1/oklahomanz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 13:02:52.998511 oklahomanz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 13:02:53.014511 oklahomanz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:49:37.960063 oklahomanz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 13:02:52.000000 oklahomanz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 06:49:37.960063 oklahomanz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 13:02:52.000000 oklahomanz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:49:37.960063 oklahomanz-2.1/oklahomanz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 13:02:52.000000 oklahomanz-2.1/oklahomanz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 13:02:53.000000 oklahomanz-2.1/oklahomanz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:49:37.960063 oklahomanz-2.1/oklahomanz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 06:49:37.000000 oklahomanz-2.1/oklahomanz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 06:49:37.000000 oklahomanz-2.1/oklahomanz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 06:49:37.000000 oklahomanz-2.1/oklahomanz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 06:49:37.000000 oklahomanz-2.1/oklahomanz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 06:49:37.000000 oklahomanz-2.1/oklahomanz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 06:49:37.960063 oklahomanz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 06:49:32.000000 oklahomanz-2.1/setup.py
```

### Comparing `oklahomanz-1.1/setup.py` & `oklahomanz-2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'oklahomanz',
     packages = ['oklahomanz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'oklahomanz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/oklahomanz',
```

