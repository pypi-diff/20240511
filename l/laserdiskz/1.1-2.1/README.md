# Comparing `tmp/laserdiskz-1.1.tar.gz` & `tmp/laserdiskz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laserdiskz-1.1.tar", last modified: Wed May  8 16:13:36 2024, max compression
+gzip compressed data, was "laserdiskz-2.1.tar", last modified: Sat May 11 02:14:50 2024, max compression
```

## Comparing `laserdiskz-1.1.tar` & `laserdiskz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:13:35.994457 laserdiskz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 16:13:35.994457 laserdiskz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:13:35.994457 laserdiskz-1.1/laserdiskz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:13:35.794453 laserdiskz-1.1/laserdiskz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:13:35.802453 laserdiskz-1.1/laserdiskz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 16:13:35.794453 laserdiskz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 16:13:35.810453 laserdiskz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 02:14:50.669111 laserdiskz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 16:13:35.000000 laserdiskz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 02:14:50.669111 laserdiskz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 16:13:35.000000 laserdiskz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 02:14:50.665111 laserdiskz-2.1/laserdiskz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:13:35.000000 laserdiskz-2.1/laserdiskz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:13:35.000000 laserdiskz-2.1/laserdiskz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 02:14:50.669111 laserdiskz-2.1/laserdiskz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 02:14:50.000000 laserdiskz-2.1/laserdiskz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 02:14:50.000000 laserdiskz-2.1/laserdiskz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 02:14:50.000000 laserdiskz-2.1/laserdiskz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 02:14:50.000000 laserdiskz-2.1/laserdiskz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 02:14:50.000000 laserdiskz-2.1/laserdiskz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 02:14:50.669111 laserdiskz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 02:14:50.000000 laserdiskz-2.1/setup.py
```

### Comparing `laserdiskz-1.1/setup.py` & `laserdiskz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'laserdiskz',
     packages = ['laserdiskz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'laserdiskz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/laserdiskz',
```
