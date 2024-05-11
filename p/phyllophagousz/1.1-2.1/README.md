# Comparing `tmp/phyllophagousz-1.1.tar.gz` & `tmp/phyllophagousz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phyllophagousz-1.1.tar", last modified: Thu May  9 00:12:38 2024, max compression
+gzip compressed data, was "phyllophagousz-2.1.tar", last modified: Sat May 11 09:20:05 2024, max compression
```

## Comparing `phyllophagousz-1.1.tar` & `phyllophagousz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 00:12:38.507604 phyllophagousz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1672 2024-05-09 00:12:38.507604 phyllophagousz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 00:12:38.507604 phyllophagousz-1.1/phyllophagousz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 00:12:38.323601 phyllophagousz-1.1/phyllophagousz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 00:12:38.331601 phyllophagousz-1.1/phyllophagousz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 00:12:38.323601 phyllophagousz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-09 00:12:38.339601 phyllophagousz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:20:05.618132 phyllophagousz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 00:12:38.000000 phyllophagousz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 09:20:05.618132 phyllophagousz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 00:12:38.000000 phyllophagousz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:20:05.618132 phyllophagousz-2.1/phyllophagousz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 00:12:38.000000 phyllophagousz-2.1/phyllophagousz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 00:12:38.000000 phyllophagousz-2.1/phyllophagousz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:20:05.618132 phyllophagousz-2.1/phyllophagousz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 09:20:05.000000 phyllophagousz-2.1/phyllophagousz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      275 2024-05-11 09:20:05.000000 phyllophagousz-2.1/phyllophagousz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 09:20:05.000000 phyllophagousz-2.1/phyllophagousz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 09:20:05.000000 phyllophagousz-2.1/phyllophagousz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       15 2024-05-11 09:20:05.000000 phyllophagousz-2.1/phyllophagousz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 09:20:05.650133 phyllophagousz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-11 09:20:05.000000 phyllophagousz-2.1/setup.py
```

### Comparing `phyllophagousz-1.1/setup.py` & `phyllophagousz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'phyllophagousz',
     packages = ['phyllophagousz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'phyllophagousz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/phyllophagousz',
```

