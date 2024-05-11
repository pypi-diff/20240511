# Comparing `tmp/suckerfishesz-1.1.tar.gz` & `tmp/suckerfishesz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suckerfishesz-1.1.tar", last modified: Thu May  9 09:37:05 2024, max compression
+gzip compressed data, was "suckerfishesz-2.1.tar", last modified: Sat May 11 17:21:54 2024, max compression
```

## Comparing `suckerfishesz-1.1.tar` & `suckerfishesz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 09:37:05.782722 suckerfishesz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-09 09:37:05.782722 suckerfishesz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 09:37:05.602719 suckerfishesz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-09 09:37:05.618719 suckerfishesz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 09:37:05.782722 suckerfishesz-1.1/suckerfishesz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 09:37:05.606719 suckerfishesz-1.1/suckerfishesz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 09:37:05.610719 suckerfishesz-1.1/suckerfishesz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:21:54.203057 suckerfishesz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 09:37:05.000000 suckerfishesz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 17:21:54.203057 suckerfishesz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 09:37:05.000000 suckerfishesz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 17:21:54.203057 suckerfishesz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 17:21:48.000000 suckerfishesz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:21:54.203057 suckerfishesz-2.1/suckerfishesz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 09:37:05.000000 suckerfishesz-2.1/suckerfishesz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 09:37:05.000000 suckerfishesz-2.1/suckerfishesz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:21:54.203057 suckerfishesz-2.1/suckerfishesz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 17:21:53.000000 suckerfishesz-2.1/suckerfishesz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 17:21:53.000000 suckerfishesz-2.1/suckerfishesz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 17:21:53.000000 suckerfishesz-2.1/suckerfishesz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 17:21:53.000000 suckerfishesz-2.1/suckerfishesz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 17:21:53.000000 suckerfishesz-2.1/suckerfishesz.egg-info/top_level.txt
```

### Comparing `suckerfishesz-1.1/setup.py` & `suckerfishesz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'suckerfishesz',
     packages = ['suckerfishesz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'suckerfishesz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/suckerfishesz',
```

