# Comparing `tmp/stoundedz-1.1.tar.gz` & `tmp/stoundedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stoundedz-1.1.tar", last modified: Thu May  9 21:52:04 2024, max compression
+gzip compressed data, was "stoundedz-2.1.tar", last modified: Sat May 11 16:35:43 2024, max compression
```

## Comparing `stoundedz-1.1.tar` & `stoundedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 21:52:04.702449 stoundedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-09 21:52:04.702449 stoundedz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 21:51:56.498298 stoundedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-09 21:51:57.634319 stoundedz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 21:52:04.702449 stoundedz-1.1/stoundedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 21:51:56.498298 stoundedz-1.1/stoundedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 21:51:56.890305 stoundedz-1.1/stoundedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:35:43.431967 stoundedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 21:51:56.000000 stoundedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 16:35:43.431967 stoundedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 21:51:56.000000 stoundedz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 16:35:43.431967 stoundedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-11 16:35:36.000000 stoundedz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:35:43.407967 stoundedz-2.1/stoundedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 21:51:56.000000 stoundedz-2.1/stoundedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 21:51:56.000000 stoundedz-2.1/stoundedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:35:43.431967 stoundedz-2.1/stoundedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 16:35:42.000000 stoundedz-2.1/stoundedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-11 16:35:42.000000 stoundedz-2.1/stoundedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 16:35:42.000000 stoundedz-2.1/stoundedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 16:35:42.000000 stoundedz-2.1/stoundedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-11 16:35:42.000000 stoundedz-2.1/stoundedz.egg-info/top_level.txt
```

### Comparing `stoundedz-1.1/setup.py` & `stoundedz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'stoundedz',
     packages = ['stoundedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'stoundedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/stoundedz',
```

