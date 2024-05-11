# Comparing `tmp/scarcerz-1.1.tar.gz` & `tmp/scarcerz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scarcerz-1.1.tar", last modified: Thu May  9 15:46:06 2024, max compression
+gzip compressed data, was "scarcerz-2.1.tar", last modified: Sat May 11 14:30:46 2024, max compression
```

## Comparing `scarcerz-1.1.tar` & `scarcerz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 15:46:06.570454 scarcerz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-09 15:46:06.570454 scarcerz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 15:46:06.570454 scarcerz-1.1/scarcerz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 15:46:03.354395 scarcerz-1.1/scarcerz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 15:46:03.550398 scarcerz-1.1/scarcerz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 15:46:03.354395 scarcerz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-09 15:46:04.054407 scarcerz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:30:46.877396 scarcerz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 15:46:03.000000 scarcerz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 14:30:46.877396 scarcerz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 15:46:03.000000 scarcerz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:30:46.877396 scarcerz-2.1/scarcerz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 15:46:03.000000 scarcerz-2.1/scarcerz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 15:46:03.000000 scarcerz-2.1/scarcerz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:30:46.877396 scarcerz-2.1/scarcerz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 14:30:45.000000 scarcerz-2.1/scarcerz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-11 14:30:45.000000 scarcerz-2.1/scarcerz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 14:30:45.000000 scarcerz-2.1/scarcerz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 14:30:45.000000 scarcerz-2.1/scarcerz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-11 14:30:45.000000 scarcerz-2.1/scarcerz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 14:30:46.877396 scarcerz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-11 14:30:39.000000 scarcerz-2.1/setup.py
```

### Comparing `scarcerz-1.1/setup.py` & `scarcerz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'scarcerz',
     packages = ['scarcerz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'scarcerz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/scarcerz',
```

