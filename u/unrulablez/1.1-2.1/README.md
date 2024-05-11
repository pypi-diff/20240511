# Comparing `tmp/unrulablez-1.1.tar.gz` & `tmp/unrulablez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unrulablez-1.1.tar", last modified: Wed May  8 16:51:53 2024, max compression
+gzip compressed data, was "unrulablez-2.1.tar", last modified: Sat May 11 21:37:07 2024, max compression
```

## Comparing `unrulablez-1.1.tar` & `unrulablez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:51:53.285058 unrulablez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 16:51:53.285058 unrulablez-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 16:51:53.105055 unrulablez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 16:51:53.121055 unrulablez-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:51:53.285058 unrulablez-1.1/unrulablez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:51:53.105055 unrulablez-1.1/unrulablez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:51:53.113055 unrulablez-1.1/unrulablez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:37:07.461108 unrulablez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 16:51:53.000000 unrulablez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 21:37:07.457108 unrulablez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 16:51:53.000000 unrulablez-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 21:37:07.461108 unrulablez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 21:37:06.000000 unrulablez-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:37:07.457108 unrulablez-2.1/unrulablez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:51:53.000000 unrulablez-2.1/unrulablez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:51:53.000000 unrulablez-2.1/unrulablez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:37:07.457108 unrulablez-2.1/unrulablez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 21:37:07.000000 unrulablez-2.1/unrulablez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 21:37:07.000000 unrulablez-2.1/unrulablez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 21:37:07.000000 unrulablez-2.1/unrulablez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 21:37:07.000000 unrulablez-2.1/unrulablez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 21:37:07.000000 unrulablez-2.1/unrulablez.egg-info/top_level.txt
```

### Comparing `unrulablez-1.1/setup.py` & `unrulablez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'unrulablez',
     packages = ['unrulablez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'unrulablez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/unrulablez',
```

