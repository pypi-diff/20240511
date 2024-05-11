# Comparing `tmp/lvz-1.1.tar.gz` & `tmp/lvz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lvz-1.1.tar", last modified: Wed May  8 12:48:01 2024, max compression
+gzip compressed data, was "lvz-2.1.tar", last modified: Sat May 11 03:07:24 2024, max compression
```

## Comparing `lvz-1.1.tar` & `lvz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 12:48:01.735230 lvz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1628 2024-05-08 12:48:01.735230 lvz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 12:48:01.735230 lvz-1.1/lvz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 12:47:58.803177 lvz-1.1/lvz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 12:47:59.015181 lvz-1.1/lvz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 12:47:58.803177 lvz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1542 2024-05-08 12:47:59.231185 lvz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:07:24.806967 lvz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 12:47:58.000000 lvz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1884 2024-05-11 03:07:24.806967 lvz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 12:47:58.000000 lvz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:07:24.806967 lvz-2.1/lvz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 12:47:58.000000 lvz-2.1/lvz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 12:47:59.000000 lvz-2.1/lvz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:07:24.806967 lvz-2.1/lvz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1884 2024-05-11 03:07:24.000000 lvz-2.1/lvz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      198 2024-05-11 03:07:24.000000 lvz-2.1/lvz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 03:07:24.000000 lvz-2.1/lvz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 03:07:24.000000 lvz-2.1/lvz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        4 2024-05-11 03:07:24.000000 lvz-2.1/lvz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 03:07:24.806967 lvz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1542 2024-05-11 03:07:24.000000 lvz-2.1/setup.py
```

### Comparing `lvz-1.1/setup.py` & `lvz-2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'lvz',
     packages = ['lvz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'lvz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/lvz',
```

