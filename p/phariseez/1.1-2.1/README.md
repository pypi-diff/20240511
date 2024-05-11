# Comparing `tmp/phariseez-1.1.tar.gz` & `tmp/phariseez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phariseez-1.1.tar", last modified: Fri May 10 03:46:51 2024, max compression
+gzip compressed data, was "phariseez-2.1.tar", last modified: Sat May 11 09:09:42 2024, max compression
```

## Comparing `phariseez-1.1.tar` & `phariseez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 03:46:51.082136 phariseez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-10 03:46:51.082136 phariseez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 03:46:51.082136 phariseez-1.1/phariseez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 03:46:47.374067 phariseez-1.1/phariseez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 03:46:47.570071 phariseez-1.1/phariseez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 03:46:47.374067 phariseez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-10 03:46:48.062080 phariseez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:09:42.054646 phariseez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 03:46:47.000000 phariseez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 09:09:42.054646 phariseez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 03:46:47.000000 phariseez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:09:42.050645 phariseez-2.1/phariseez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 03:46:47.000000 phariseez-2.1/phariseez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 03:46:47.000000 phariseez-2.1/phariseez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 09:09:42.054646 phariseez-2.1/phariseez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 09:09:41.000000 phariseez-2.1/phariseez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-11 09:09:41.000000 phariseez-2.1/phariseez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 09:09:41.000000 phariseez-2.1/phariseez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 09:09:41.000000 phariseez-2.1/phariseez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-11 09:09:41.000000 phariseez-2.1/phariseez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 09:09:42.054646 phariseez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-11 09:09:41.000000 phariseez-2.1/setup.py
```

### Comparing `phariseez-1.1/setup.py` & `phariseez-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'phariseez',
     packages = ['phariseez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'phariseez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/phariseez',
```

