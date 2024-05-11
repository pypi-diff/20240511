# Comparing `tmp/pressurizesz-1.1.tar.gz` & `tmp/pressurizesz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pressurizesz-1.1.tar", last modified: Thu May  9 12:20:09 2024, max compression
+gzip compressed data, was "pressurizesz-2.1.tar", last modified: Sat May 11 11:24:21 2024, max compression
```

## Comparing `pressurizesz-1.1.tar` & `pressurizesz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 12:20:09.375099 pressurizesz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 12:20:09.375099 pressurizesz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 12:20:09.375099 pressurizesz-1.1/pressurizesz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 12:20:06.175039 pressurizesz-1.1/pressurizesz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 12:20:06.335042 pressurizesz-1.1/pressurizesz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 12:20:06.175039 pressurizesz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 12:20:06.767050 pressurizesz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:24:21.459423 pressurizesz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 12:20:06.000000 pressurizesz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 11:24:21.459423 pressurizesz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 12:20:06.000000 pressurizesz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:24:21.455423 pressurizesz-2.1/pressurizesz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 12:20:06.000000 pressurizesz-2.1/pressurizesz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 12:20:06.000000 pressurizesz-2.1/pressurizesz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:24:21.459423 pressurizesz-2.1/pressurizesz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 11:24:21.000000 pressurizesz-2.1/pressurizesz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 11:24:21.000000 pressurizesz-2.1/pressurizesz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 11:24:21.000000 pressurizesz-2.1/pressurizesz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 11:24:21.000000 pressurizesz-2.1/pressurizesz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 11:24:21.000000 pressurizesz-2.1/pressurizesz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 11:24:21.459423 pressurizesz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 11:24:20.000000 pressurizesz-2.1/setup.py
```

### Comparing `pressurizesz-1.1/setup.py` & `pressurizesz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'pressurizesz',
     packages = ['pressurizesz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'pressurizesz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/pressurizesz',
```

