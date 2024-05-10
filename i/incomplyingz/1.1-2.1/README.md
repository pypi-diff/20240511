# Comparing `tmp/incomplyingz-1.1.tar.gz` & `tmp/incomplyingz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incomplyingz-1.1.tar", last modified: Thu May  9 14:34:56 2024, max compression
+gzip compressed data, was "incomplyingz-2.1.tar", last modified: Fri May 10 23:54:51 2024, max compression
```

## Comparing `incomplyingz-1.1.tar` & `incomplyingz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 14:34:56.515744 incomplyingz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 14:34:56.515744 incomplyingz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 14:34:56.515744 incomplyingz-1.1/incomplyingz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 14:34:53.231684 incomplyingz-1.1/incomplyingz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 14:34:53.375686 incomplyingz-1.1/incomplyingz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 14:34:53.231684 incomplyingz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 14:34:53.763693 incomplyingz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 23:54:51.298654 incomplyingz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 14:34:53.000000 incomplyingz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 23:54:51.298654 incomplyingz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 14:34:53.000000 incomplyingz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 23:54:51.298654 incomplyingz-2.1/incomplyingz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 14:34:53.000000 incomplyingz-2.1/incomplyingz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 14:34:53.000000 incomplyingz-2.1/incomplyingz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 23:54:51.298654 incomplyingz-2.1/incomplyingz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-10 23:54:51.000000 incomplyingz-2.1/incomplyingz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-10 23:54:51.000000 incomplyingz-2.1/incomplyingz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 23:54:51.000000 incomplyingz-2.1/incomplyingz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 23:54:51.000000 incomplyingz-2.1/incomplyingz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-10 23:54:51.000000 incomplyingz-2.1/incomplyingz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 23:54:51.298654 incomplyingz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-10 23:54:50.000000 incomplyingz-2.1/setup.py
```

### Comparing `incomplyingz-1.1/setup.py` & `incomplyingz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'incomplyingz',
     packages = ['incomplyingz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'incomplyingz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/incomplyingz',
```

