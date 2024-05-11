# Comparing `tmp/tipisz-1.1.tar.gz` & `tmp/tipisz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tipisz-1.1.tar", last modified: Thu May  9 14:45:33 2024, max compression
+gzip compressed data, was "tipisz-2.1.tar", last modified: Sat May 11 19:16:25 2024, max compression
```

## Comparing `tipisz-1.1.tar` & `tipisz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 14:45:33.303469 tipisz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1640 2024-05-09 14:45:33.303469 tipisz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 14:45:33.115465 tipisz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1566 2024-05-09 14:45:33.147466 tipisz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 14:45:33.303469 tipisz-1.1/tipisz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 14:45:33.115465 tipisz-1.1/tipisz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 14:45:33.123465 tipisz-1.1/tipisz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:16:25.669725 tipisz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 14:45:33.000000 tipisz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1905 2024-05-11 19:16:25.669725 tipisz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 14:45:33.000000 tipisz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 19:16:25.669725 tipisz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1566 2024-05-11 19:16:25.000000 tipisz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:16:25.665725 tipisz-2.1/tipisz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 14:45:33.000000 tipisz-2.1/tipisz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 14:45:33.000000 tipisz-2.1/tipisz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:16:25.665725 tipisz-2.1/tipisz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1905 2024-05-11 19:16:25.000000 tipisz-2.1/tipisz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      219 2024-05-11 19:16:25.000000 tipisz-2.1/tipisz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 19:16:25.000000 tipisz-2.1/tipisz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 19:16:25.000000 tipisz-2.1/tipisz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        7 2024-05-11 19:16:25.000000 tipisz-2.1/tipisz.egg-info/top_level.txt
```

### Comparing `tipisz-1.1/setup.py` & `tipisz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'tipisz',
     packages = ['tipisz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'tipisz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/tipisz',
```

