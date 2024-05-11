# Comparing `tmp/lwoz-1.1.tar.gz` & `tmp/lwoz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lwoz-1.1.tar", last modified: Thu May  9 18:25:14 2024, max compression
+gzip compressed data, was "lwoz-2.1.tar", last modified: Sat May 11 03:12:29 2024, max compression
```

## Comparing `lwoz-1.1.tar` & `lwoz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 18:25:14.502114 lwoz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1632 2024-05-09 18:25:14.502114 lwoz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 18:25:14.502114 lwoz-1.1/lwoz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 18:25:12.250072 lwoz-1.1/lwoz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 18:25:12.462076 lwoz-1.1/lwoz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 18:25:12.250072 lwoz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1550 2024-05-09 18:25:12.802082 lwoz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:12:28.996547 lwoz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 18:25:12.000000 lwoz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1891 2024-05-11 03:12:28.996547 lwoz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 18:25:12.000000 lwoz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:12:28.996547 lwoz-2.1/lwoz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 18:25:12.000000 lwoz-2.1/lwoz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 18:25:12.000000 lwoz-2.1/lwoz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:12:28.996547 lwoz-2.1/lwoz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1891 2024-05-11 03:12:28.000000 lwoz-2.1/lwoz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      205 2024-05-11 03:12:28.000000 lwoz-2.1/lwoz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 03:12:28.000000 lwoz-2.1/lwoz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 03:12:28.000000 lwoz-2.1/lwoz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        5 2024-05-11 03:12:28.000000 lwoz-2.1/lwoz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 03:12:28.996547 lwoz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1550 2024-05-11 03:12:28.000000 lwoz-2.1/setup.py
```

### Comparing `lwoz-1.1/setup.py` & `lwoz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'lwoz',
     packages = ['lwoz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'lwoz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/lwoz',
```

