# Comparing `tmp/metonymicallyz-1.1.tar.gz` & `tmp/metonymicallyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metonymicallyz-1.1.tar", last modified: Wed May  8 15:03:09 2024, max compression
+gzip compressed data, was "metonymicallyz-2.1.tar", last modified: Sat May 11 04:20:15 2024, max compression
```

## Comparing `metonymicallyz-1.1.tar` & `metonymicallyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 15:03:09.860524 metonymicallyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1672 2024-05-08 15:03:09.860524 metonymicallyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 15:03:09.860524 metonymicallyz-1.1/metonymicallyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 15:03:05.420443 metonymicallyz-1.1/metonymicallyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 15:03:05.748449 metonymicallyz-1.1/metonymicallyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 15:03:05.420443 metonymicallyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-08 15:03:06.072455 metonymicallyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:20:15.511404 metonymicallyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 15:03:05.000000 metonymicallyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 04:20:15.511404 metonymicallyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 15:03:05.000000 metonymicallyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:20:15.511404 metonymicallyz-2.1/metonymicallyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 15:03:05.000000 metonymicallyz-2.1/metonymicallyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 15:03:05.000000 metonymicallyz-2.1/metonymicallyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:20:15.511404 metonymicallyz-2.1/metonymicallyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 04:20:14.000000 metonymicallyz-2.1/metonymicallyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      275 2024-05-11 04:20:14.000000 metonymicallyz-2.1/metonymicallyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 04:20:14.000000 metonymicallyz-2.1/metonymicallyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 04:20:14.000000 metonymicallyz-2.1/metonymicallyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       15 2024-05-11 04:20:14.000000 metonymicallyz-2.1/metonymicallyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 04:20:15.515405 metonymicallyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-11 04:20:01.000000 metonymicallyz-2.1/setup.py
```

### Comparing `metonymicallyz-1.1/setup.py` & `metonymicallyz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'metonymicallyz',
     packages = ['metonymicallyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'metonymicallyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/metonymicallyz',
```

