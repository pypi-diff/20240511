# Comparing `tmp/pseudomoralz-1.1.tar.gz` & `tmp/pseudomoralz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pseudomoralz-1.1.tar", last modified: Thu May  9 22:44:33 2024, max compression
+gzip compressed data, was "pseudomoralz-2.1.tar", last modified: Sat May 11 11:55:55 2024, max compression
```

## Comparing `pseudomoralz-1.1.tar` & `pseudomoralz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 22:44:33.488330 pseudomoralz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 22:44:33.488330 pseudomoralz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 22:44:33.488330 pseudomoralz-1.1/pseudomoralz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 22:44:33.296326 pseudomoralz-1.1/pseudomoralz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 22:44:33.304326 pseudomoralz-1.1/pseudomoralz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 22:44:33.296326 pseudomoralz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 22:44:33.312326 pseudomoralz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:55:55.906090 pseudomoralz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 22:44:33.000000 pseudomoralz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 11:55:55.906090 pseudomoralz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 22:44:33.000000 pseudomoralz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:55:55.906090 pseudomoralz-2.1/pseudomoralz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 22:44:33.000000 pseudomoralz-2.1/pseudomoralz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 22:44:33.000000 pseudomoralz-2.1/pseudomoralz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:55:55.906090 pseudomoralz-2.1/pseudomoralz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 11:55:55.000000 pseudomoralz-2.1/pseudomoralz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 11:55:55.000000 pseudomoralz-2.1/pseudomoralz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 11:55:55.000000 pseudomoralz-2.1/pseudomoralz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 11:55:55.000000 pseudomoralz-2.1/pseudomoralz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 11:55:55.000000 pseudomoralz-2.1/pseudomoralz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 11:55:55.910090 pseudomoralz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 11:55:48.000000 pseudomoralz-2.1/setup.py
```

### Comparing `pseudomoralz-1.1/setup.py` & `pseudomoralz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'pseudomoralz',
     packages = ['pseudomoralz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'pseudomoralz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/pseudomoralz',
```

