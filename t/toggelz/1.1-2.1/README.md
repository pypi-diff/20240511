# Comparing `tmp/toggelz-1.1.tar.gz` & `tmp/toggelz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toggelz-1.1.tar", last modified: Thu May  9 17:58:33 2024, max compression
+gzip compressed data, was "toggelz-2.1.tar", last modified: Sat May 11 19:32:03 2024, max compression
```

## Comparing `toggelz-1.1.tar` & `toggelz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 17:58:33.984585 toggelz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1644 2024-05-09 17:58:33.984585 toggelz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 17:58:33.756581 toggelz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-09 17:58:33.768581 toggelz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 17:58:33.984585 toggelz-1.1/toggelz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 17:58:33.756581 toggelz-1.1/toggelz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 17:58:33.764581 toggelz-1.1/toggelz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:32:03.979028 toggelz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 17:58:33.000000 toggelz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-11 19:32:03.979028 toggelz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 17:58:33.000000 toggelz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 19:32:03.979028 toggelz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-11 19:32:02.000000 toggelz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:32:03.975028 toggelz-2.1/toggelz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 17:58:33.000000 toggelz-2.1/toggelz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 17:58:33.000000 toggelz-2.1/toggelz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:32:03.979028 toggelz-2.1/toggelz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-11 19:32:02.000000 toggelz-2.1/toggelz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      226 2024-05-11 19:32:03.000000 toggelz-2.1/toggelz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 19:32:02.000000 toggelz-2.1/toggelz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 19:32:02.000000 toggelz-2.1/toggelz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-11 19:32:02.000000 toggelz-2.1/toggelz.egg-info/top_level.txt
```

### Comparing `toggelz-1.1/setup.py` & `toggelz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'toggelz',
     packages = ['toggelz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'toggelz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/toggelz',
```

