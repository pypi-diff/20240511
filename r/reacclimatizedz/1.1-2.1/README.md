# Comparing `tmp/reacclimatizedz-1.1.tar.gz` & `tmp/reacclimatizedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reacclimatizedz-1.1.tar", last modified: Thu May  9 12:14:42 2024, max compression
+gzip compressed data, was "reacclimatizedz-2.1.tar", last modified: Sat May 11 12:52:30 2024, max compression
```

## Comparing `reacclimatizedz-1.1.tar` & `reacclimatizedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 12:14:42.477018 reacclimatizedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1676 2024-05-09 12:14:42.477018 reacclimatizedz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 12:14:42.477018 reacclimatizedz-1.1/reacclimatizedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 12:14:39.268958 reacclimatizedz-1.1/reacclimatizedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 12:14:39.512962 reacclimatizedz-1.1/reacclimatizedz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 12:14:39.268958 reacclimatizedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-09 12:14:39.744967 reacclimatizedz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 12:52:30.800928 reacclimatizedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 12:14:39.000000 reacclimatizedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 12:52:30.800928 reacclimatizedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 12:14:39.000000 reacclimatizedz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 12:52:30.800928 reacclimatizedz-2.1/reacclimatizedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 12:14:39.000000 reacclimatizedz-2.1/reacclimatizedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 12:14:39.000000 reacclimatizedz-2.1/reacclimatizedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 12:52:30.800928 reacclimatizedz-2.1/reacclimatizedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 12:52:30.000000 reacclimatizedz-2.1/reacclimatizedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      282 2024-05-11 12:52:30.000000 reacclimatizedz-2.1/reacclimatizedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 12:52:30.000000 reacclimatizedz-2.1/reacclimatizedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 12:52:30.000000 reacclimatizedz-2.1/reacclimatizedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       16 2024-05-11 12:52:30.000000 reacclimatizedz-2.1/reacclimatizedz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 12:52:30.800928 reacclimatizedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-11 12:52:30.000000 reacclimatizedz-2.1/setup.py
```

### Comparing `reacclimatizedz-1.1/setup.py` & `reacclimatizedz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'reacclimatizedz',
     packages = ['reacclimatizedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'reacclimatizedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/reacclimatizedz',
```

