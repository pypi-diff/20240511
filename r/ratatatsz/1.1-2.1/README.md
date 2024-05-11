# Comparing `tmp/ratatatsz-1.1.tar.gz` & `tmp/ratatatsz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratatatsz-1.1.tar", last modified: Thu May  9 17:42:43 2024, max compression
+gzip compressed data, was "ratatatsz-2.1.tar", last modified: Sat May 11 12:47:26 2024, max compression
```

## Comparing `ratatatsz-1.1.tar` & `ratatatsz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 17:42:43.307232 ratatatsz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-09 17:42:43.307232 ratatatsz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 17:42:43.307232 ratatatsz-1.1/ratatatsz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 17:42:40.363178 ratatatsz-1.1/ratatatsz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 17:42:40.531181 ratatatsz-1.1/ratatatsz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 17:42:40.363178 ratatatsz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-09 17:42:40.703185 ratatatsz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 12:47:26.267304 ratatatsz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 17:42:40.000000 ratatatsz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 12:47:26.267304 ratatatsz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 17:42:40.000000 ratatatsz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 12:47:26.267304 ratatatsz-2.1/ratatatsz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 17:42:40.000000 ratatatsz-2.1/ratatatsz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 17:42:40.000000 ratatatsz-2.1/ratatatsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 12:47:26.267304 ratatatsz-2.1/ratatatsz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 12:47:26.000000 ratatatsz-2.1/ratatatsz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-11 12:47:26.000000 ratatatsz-2.1/ratatatsz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 12:47:26.000000 ratatatsz-2.1/ratatatsz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 12:47:26.000000 ratatatsz-2.1/ratatatsz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-11 12:47:26.000000 ratatatsz-2.1/ratatatsz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 12:47:26.267304 ratatatsz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-11 12:47:25.000000 ratatatsz-2.1/setup.py
```

### Comparing `ratatatsz-1.1/setup.py` & `ratatatsz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'ratatatsz',
     packages = ['ratatatsz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'ratatatsz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/ratatatsz',
```

