# Comparing `tmp/overaccentuationz-1.1.tar.gz` & `tmp/overaccentuationz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overaccentuationz-1.1.tar", last modified: Thu May  9 08:59:14 2024, max compression
+gzip compressed data, was "overaccentuationz-2.1.tar", last modified: Sat May 11 07:31:28 2024, max compression
```

## Comparing `overaccentuationz-1.1.tar` & `overaccentuationz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 08:59:14.264865 overaccentuationz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1684 2024-05-09 08:59:14.264865 overaccentuationz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 08:59:14.264865 overaccentuationz-1.1/overaccentuationz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 08:59:14.060862 overaccentuationz-1.1/overaccentuationz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 08:59:14.076862 overaccentuationz-1.1/overaccentuationz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 08:59:14.060862 overaccentuationz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-09 08:59:14.084862 overaccentuationz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:31:28.866410 overaccentuationz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 08:59:14.000000 overaccentuationz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 07:31:28.866410 overaccentuationz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 08:59:14.000000 overaccentuationz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:31:28.866410 overaccentuationz-2.1/overaccentuationz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 08:59:14.000000 overaccentuationz-2.1/overaccentuationz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 08:59:14.000000 overaccentuationz-2.1/overaccentuationz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:31:28.866410 overaccentuationz-2.1/overaccentuationz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 07:31:28.000000 overaccentuationz-2.1/overaccentuationz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      296 2024-05-11 07:31:28.000000 overaccentuationz-2.1/overaccentuationz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 07:31:28.000000 overaccentuationz-2.1/overaccentuationz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 07:31:28.000000 overaccentuationz-2.1/overaccentuationz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       18 2024-05-11 07:31:28.000000 overaccentuationz-2.1/overaccentuationz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 07:31:28.866410 overaccentuationz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-11 07:31:28.000000 overaccentuationz-2.1/setup.py
```

### Comparing `overaccentuationz-1.1/setup.py` & `overaccentuationz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'overaccentuationz',
     packages = ['overaccentuationz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'overaccentuationz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/overaccentuationz',
```

