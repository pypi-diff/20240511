# Comparing `tmp/refoldingz-1.1.tar.gz` & `tmp/refoldingz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refoldingz-1.1.tar", last modified: Wed May  8 18:57:07 2024, max compression
+gzip compressed data, was "refoldingz-2.1.tar", last modified: Sat May 11 13:23:14 2024, max compression
```

## Comparing `refoldingz-1.1.tar` & `refoldingz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 18:57:07.171322 refoldingz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 18:57:07.171322 refoldingz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 18:57:07.171322 refoldingz-1.1/refoldingz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 18:57:06.999319 refoldingz-1.1/refoldingz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 18:57:07.007320 refoldingz-1.1/refoldingz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 18:57:06.999319 refoldingz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 18:57:07.015320 refoldingz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 13:23:14.830462 refoldingz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 18:57:06.000000 refoldingz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 13:23:14.830462 refoldingz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 18:57:06.000000 refoldingz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 13:23:14.830462 refoldingz-2.1/refoldingz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 18:57:06.000000 refoldingz-2.1/refoldingz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 18:57:07.000000 refoldingz-2.1/refoldingz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 13:23:14.830462 refoldingz-2.1/refoldingz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 13:23:14.000000 refoldingz-2.1/refoldingz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 13:23:14.000000 refoldingz-2.1/refoldingz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 13:23:14.000000 refoldingz-2.1/refoldingz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 13:23:14.000000 refoldingz-2.1/refoldingz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 13:23:14.000000 refoldingz-2.1/refoldingz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 13:23:14.830462 refoldingz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 13:23:09.000000 refoldingz-2.1/setup.py
```

### Comparing `refoldingz-1.1/setup.py` & `refoldingz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'refoldingz',
     packages = ['refoldingz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'refoldingz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/refoldingz',
```

