# Comparing `tmp/lamebrainedz-1.1.tar.gz` & `tmp/lamebrainedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamebrainedz-1.1.tar", last modified: Thu May  9 19:03:31 2024, max compression
+gzip compressed data, was "lamebrainedz-2.1.tar", last modified: Sat May 11 01:43:47 2024, max compression
```

## Comparing `lamebrainedz-1.1.tar` & `lamebrainedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 19:03:30.968754 lamebrainedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 19:03:30.968754 lamebrainedz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 19:03:30.968754 lamebrainedz-1.1/lamebrainedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 19:03:22.868603 lamebrainedz-1.1/lamebrainedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 19:03:23.308611 lamebrainedz-1.1/lamebrainedz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 19:03:22.868603 lamebrainedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 19:03:24.204628 lamebrainedz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:43:47.282824 lamebrainedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 19:03:22.000000 lamebrainedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 01:43:47.282824 lamebrainedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 19:03:22.000000 lamebrainedz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:43:47.278824 lamebrainedz-2.1/lamebrainedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 19:03:22.000000 lamebrainedz-2.1/lamebrainedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 19:03:23.000000 lamebrainedz-2.1/lamebrainedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:43:47.282824 lamebrainedz-2.1/lamebrainedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 01:43:47.000000 lamebrainedz-2.1/lamebrainedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 01:43:47.000000 lamebrainedz-2.1/lamebrainedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 01:43:47.000000 lamebrainedz-2.1/lamebrainedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 01:43:47.000000 lamebrainedz-2.1/lamebrainedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 01:43:47.000000 lamebrainedz-2.1/lamebrainedz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 01:43:47.282824 lamebrainedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 01:43:46.000000 lamebrainedz-2.1/setup.py
```

### Comparing `lamebrainedz-1.1/setup.py` & `lamebrainedz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'lamebrainedz',
     packages = ['lamebrainedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'lamebrainedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/lamebrainedz',
```

