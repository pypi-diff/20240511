# Comparing `tmp/pessulusz-1.1.tar.gz` & `tmp/pessulusz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pessulusz-1.1.tar", last modified: Wed May  8 15:40:46 2024, max compression
+gzip compressed data, was "pessulusz-2.1.tar", last modified: Sat May 11 08:49:25 2024, max compression
```

## Comparing `pessulusz-1.1.tar` & `pessulusz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 15:40:46.554066 pessulusz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-08 15:40:46.554066 pessulusz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 15:40:46.554066 pessulusz-1.1/pessulusz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 15:40:43.402007 pessulusz-1.1/pessulusz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 15:40:43.590011 pessulusz-1.1/pessulusz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 15:40:43.402007 pessulusz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-08 15:40:43.762014 pessulusz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 08:49:25.008231 pessulusz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 15:40:43.000000 pessulusz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 08:49:25.008231 pessulusz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 15:40:43.000000 pessulusz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 08:49:25.008231 pessulusz-2.1/pessulusz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 15:40:43.000000 pessulusz-2.1/pessulusz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 15:40:43.000000 pessulusz-2.1/pessulusz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 08:49:25.008231 pessulusz-2.1/pessulusz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 08:49:24.000000 pessulusz-2.1/pessulusz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-11 08:49:24.000000 pessulusz-2.1/pessulusz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 08:49:24.000000 pessulusz-2.1/pessulusz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 08:49:24.000000 pessulusz-2.1/pessulusz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-11 08:49:24.000000 pessulusz-2.1/pessulusz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 08:49:25.008231 pessulusz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-11 08:49:22.000000 pessulusz-2.1/setup.py
```

### Comparing `pessulusz-1.1/setup.py` & `pessulusz-2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'pessulusz',
     packages = ['pessulusz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'pessulusz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/pessulusz',
```

