# Comparing `tmp/maharishiz-1.1.tar.gz` & `tmp/maharishiz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maharishiz-1.1.tar", last modified: Wed May  8 23:34:57 2024, max compression
+gzip compressed data, was "maharishiz-2.1.tar", last modified: Sat May 11 03:28:03 2024, max compression
```

## Comparing `maharishiz-1.1.tar` & `maharishiz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 23:34:57.770036 maharishiz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 23:34:57.770036 maharishiz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 23:34:57.770036 maharishiz-1.1/maharishiz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 23:34:53.289953 maharishiz-1.1/maharishiz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 23:34:53.521957 maharishiz-1.1/maharishiz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 23:34:53.289953 maharishiz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 23:34:53.793963 maharishiz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:28:03.597826 maharishiz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 23:34:53.000000 maharishiz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 03:28:03.597826 maharishiz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 23:34:53.000000 maharishiz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:28:03.597826 maharishiz-2.1/maharishiz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 23:34:53.000000 maharishiz-2.1/maharishiz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 23:34:53.000000 maharishiz-2.1/maharishiz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:28:03.597826 maharishiz-2.1/maharishiz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 03:28:03.000000 maharishiz-2.1/maharishiz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 03:28:03.000000 maharishiz-2.1/maharishiz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 03:28:03.000000 maharishiz-2.1/maharishiz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 03:28:03.000000 maharishiz-2.1/maharishiz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 03:28:03.000000 maharishiz-2.1/maharishiz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 03:28:03.597826 maharishiz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 03:28:03.000000 maharishiz-2.1/setup.py
```

### Comparing `maharishiz-1.1/setup.py` & `maharishiz-2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'maharishiz',
     packages = ['maharishiz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'maharishiz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/maharishiz',
```

