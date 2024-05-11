# Comparing `tmp/protestantlyz-1.1.tar.gz` & `tmp/protestantlyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protestantlyz-1.1.tar", last modified: Fri May 10 02:29:14 2024, max compression
+gzip compressed data, was "protestantlyz-2.1.tar", last modified: Sat May 11 11:45:18 2024, max compression
```

## Comparing `protestantlyz-1.1.tar` & `protestantlyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 02:29:14.452435 protestantlyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-10 02:29:14.452435 protestantlyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 02:29:14.452435 protestantlyz-1.1/protestantlyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 02:29:14.260431 protestantlyz-1.1/protestantlyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 02:29:14.268432 protestantlyz-1.1/protestantlyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 02:29:14.260431 protestantlyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-10 02:29:14.276432 protestantlyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:45:18.974340 protestantlyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 02:29:14.000000 protestantlyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 11:45:18.974340 protestantlyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 02:29:14.000000 protestantlyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:45:18.970340 protestantlyz-2.1/protestantlyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 02:29:14.000000 protestantlyz-2.1/protestantlyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 02:29:14.000000 protestantlyz-2.1/protestantlyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:45:18.974340 protestantlyz-2.1/protestantlyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 11:45:18.000000 protestantlyz-2.1/protestantlyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 11:45:18.000000 protestantlyz-2.1/protestantlyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 11:45:18.000000 protestantlyz-2.1/protestantlyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 11:45:18.000000 protestantlyz-2.1/protestantlyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 11:45:18.000000 protestantlyz-2.1/protestantlyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 11:45:18.974340 protestantlyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 11:45:12.000000 protestantlyz-2.1/setup.py
```

### Comparing `protestantlyz-1.1/setup.py` & `protestantlyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'protestantlyz',
     packages = ['protestantlyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'protestantlyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/protestantlyz',
```

