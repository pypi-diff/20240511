# Comparing `tmp/postlueticz-1.1.tar.gz` & `tmp/postlueticz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postlueticz-1.1.tar", last modified: Thu May  9 11:19:37 2024, max compression
+gzip compressed data, was "postlueticz-2.1.tar", last modified: Sat May 11 10:16:36 2024, max compression
```

## Comparing `postlueticz-1.1.tar` & `postlueticz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 11:19:37.131942 postlueticz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-09 11:19:37.131942 postlueticz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 11:19:37.131942 postlueticz-1.1/postlueticz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 11:19:36.931938 postlueticz-1.1/postlueticz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 11:19:36.939938 postlueticz-1.1/postlueticz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 11:19:36.931938 postlueticz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-09 11:19:36.947938 postlueticz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:16:36.804633 postlueticz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 11:19:36.000000 postlueticz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 10:16:36.804633 postlueticz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 11:19:36.000000 postlueticz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:16:36.804633 postlueticz-2.1/postlueticz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 11:19:36.000000 postlueticz-2.1/postlueticz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 11:19:36.000000 postlueticz-2.1/postlueticz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:16:36.804633 postlueticz-2.1/postlueticz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 10:16:36.000000 postlueticz-2.1/postlueticz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-11 10:16:36.000000 postlueticz-2.1/postlueticz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 10:16:36.000000 postlueticz-2.1/postlueticz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 10:16:36.000000 postlueticz-2.1/postlueticz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-11 10:16:36.000000 postlueticz-2.1/postlueticz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 10:16:36.808634 postlueticz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-11 10:16:36.000000 postlueticz-2.1/setup.py
```

### Comparing `postlueticz-1.1/setup.py` & `postlueticz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'postlueticz',
     packages = ['postlueticz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'postlueticz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/postlueticz',
```

