# Comparing `tmp/hoodlumz-1.1.tar.gz` & `tmp/hoodlumz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoodlumz-1.1.tar", last modified: Thu May  9 08:48:51 2024, max compression
+gzip compressed data, was "hoodlumz-2.1.tar", last modified: Fri May 10 22:41:26 2024, max compression
```

## Comparing `hoodlumz-1.1.tar` & `hoodlumz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 08:48:51.573399 hoodlumz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-09 08:48:51.573399 hoodlumz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 08:48:51.573399 hoodlumz-1.1/hoodlumz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 08:48:51.397395 hoodlumz-1.1/hoodlumz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 08:48:51.405396 hoodlumz-1.1/hoodlumz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 08:48:51.397395 hoodlumz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-09 08:48:51.413396 hoodlumz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 22:41:26.240627 hoodlumz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 08:48:51.000000 hoodlumz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 22:41:26.240627 hoodlumz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 08:48:51.000000 hoodlumz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 22:41:26.184626 hoodlumz-2.1/hoodlumz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 08:48:51.000000 hoodlumz-2.1/hoodlumz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 08:48:51.000000 hoodlumz-2.1/hoodlumz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 22:41:26.240627 hoodlumz-2.1/hoodlumz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-10 22:41:24.000000 hoodlumz-2.1/hoodlumz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-10 22:41:24.000000 hoodlumz-2.1/hoodlumz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 22:41:24.000000 hoodlumz-2.1/hoodlumz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 22:41:24.000000 hoodlumz-2.1/hoodlumz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-10 22:41:24.000000 hoodlumz-2.1/hoodlumz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 22:41:26.240627 hoodlumz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 22:41:17.000000 hoodlumz-2.1/setup.py
```

### Comparing `hoodlumz-1.1/setup.py` & `hoodlumz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'hoodlumz',
     packages = ['hoodlumz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'hoodlumz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/hoodlumz',
```

