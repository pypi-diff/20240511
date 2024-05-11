# Comparing `tmp/rotundatez-1.1.tar.gz` & `tmp/rotundatez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotundatez-1.1.tar", last modified: Thu May  9 08:43:17 2024, max compression
+gzip compressed data, was "rotundatez-2.1.tar", last modified: Sat May 11 14:05:10 2024, max compression
```

## Comparing `rotundatez-1.1.tar` & `rotundatez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 08:43:17.663248 rotundatez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 08:43:17.663248 rotundatez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 08:43:17.663248 rotundatez-1.1/rotundatez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 08:43:14.939198 rotundatez-1.1/rotundatez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 08:43:15.119202 rotundatez-1.1/rotundatez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 08:43:14.939198 rotundatez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 08:43:15.435207 rotundatez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:05:10.552525 rotundatez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 08:43:14.000000 rotundatez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 14:05:10.552525 rotundatez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 08:43:14.000000 rotundatez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:05:10.548525 rotundatez-2.1/rotundatez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 08:43:14.000000 rotundatez-2.1/rotundatez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 08:43:15.000000 rotundatez-2.1/rotundatez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:05:10.552525 rotundatez-2.1/rotundatez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 14:05:10.000000 rotundatez-2.1/rotundatez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 14:05:10.000000 rotundatez-2.1/rotundatez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 14:05:10.000000 rotundatez-2.1/rotundatez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 14:05:10.000000 rotundatez-2.1/rotundatez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 14:05:10.000000 rotundatez-2.1/rotundatez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 14:05:10.552525 rotundatez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 14:05:09.000000 rotundatez-2.1/setup.py
```

### Comparing `rotundatez-1.1/setup.py` & `rotundatez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'rotundatez',
     packages = ['rotundatez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'rotundatez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/rotundatez',
```

