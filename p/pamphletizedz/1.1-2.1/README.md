# Comparing `tmp/pamphletizedz-1.1.tar.gz` & `tmp/pamphletizedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pamphletizedz-1.1.tar", last modified: Fri May 10 00:34:40 2024, max compression
+gzip compressed data, was "pamphletizedz-2.1.tar", last modified: Sat May 11 07:57:23 2024, max compression
```

## Comparing `pamphletizedz-1.1.tar` & `pamphletizedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 00:34:40.417739 pamphletizedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-10 00:34:40.417739 pamphletizedz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 00:34:40.417739 pamphletizedz-1.1/pamphletizedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 00:34:37.753690 pamphletizedz-1.1/pamphletizedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 00:34:38.013695 pamphletizedz-1.1/pamphletizedz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 00:34:37.753690 pamphletizedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-10 00:34:38.257699 pamphletizedz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:57:23.818963 pamphletizedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 00:34:37.000000 pamphletizedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 07:57:23.818963 pamphletizedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 00:34:37.000000 pamphletizedz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:57:23.818963 pamphletizedz-2.1/pamphletizedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 00:34:37.000000 pamphletizedz-2.1/pamphletizedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 00:34:38.000000 pamphletizedz-2.1/pamphletizedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:57:23.818963 pamphletizedz-2.1/pamphletizedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 07:57:23.000000 pamphletizedz-2.1/pamphletizedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 07:57:23.000000 pamphletizedz-2.1/pamphletizedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 07:57:23.000000 pamphletizedz-2.1/pamphletizedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 07:57:23.000000 pamphletizedz-2.1/pamphletizedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 07:57:23.000000 pamphletizedz-2.1/pamphletizedz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 07:57:23.818963 pamphletizedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 07:57:18.000000 pamphletizedz-2.1/setup.py
```

### Comparing `pamphletizedz-1.1/setup.py` & `pamphletizedz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'pamphletizedz',
     packages = ['pamphletizedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'pamphletizedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/pamphletizedz',
```

