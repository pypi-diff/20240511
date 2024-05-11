# Comparing `tmp/precleansz-1.1.tar.gz` & `tmp/precleansz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precleansz-1.1.tar", last modified: Wed May  8 19:07:54 2024, max compression
+gzip compressed data, was "precleansz-2.1.tar", last modified: Sat May 11 10:26:51 2024, max compression
```

## Comparing `precleansz-1.1.tar` & `precleansz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 19:07:54.751264 precleansz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 19:07:54.751264 precleansz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 19:07:54.751264 precleansz-1.1/precleansz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 19:07:48.987158 precleansz-1.1/precleansz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 19:07:49.291164 precleansz-1.1/precleansz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 19:07:48.987158 precleansz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 19:07:50.123179 precleansz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:26:51.520028 precleansz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 19:07:48.000000 precleansz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 10:26:51.520028 precleansz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 19:07:48.000000 precleansz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:26:51.520028 precleansz-2.1/precleansz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 19:07:48.000000 precleansz-2.1/precleansz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 19:07:49.000000 precleansz-2.1/precleansz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:26:51.520028 precleansz-2.1/precleansz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 10:26:50.000000 precleansz-2.1/precleansz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 10:26:50.000000 precleansz-2.1/precleansz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 10:26:50.000000 precleansz-2.1/precleansz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 10:26:50.000000 precleansz-2.1/precleansz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 10:26:50.000000 precleansz-2.1/precleansz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 10:26:51.520028 precleansz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 10:26:45.000000 precleansz-2.1/setup.py
```

### Comparing `precleansz-1.1/setup.py` & `precleansz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'precleansz',
     packages = ['precleansz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'precleansz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/precleansz',
```

