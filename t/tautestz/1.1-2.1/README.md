# Comparing `tmp/tautestz-1.1.tar.gz` & `tmp/tautestz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tautestz-1.1.tar", last modified: Wed May  8 14:13:58 2024, max compression
+gzip compressed data, was "tautestz-2.1.tar", last modified: Sat May 11 18:14:02 2024, max compression
```

## Comparing `tautestz-1.1.tar` & `tautestz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 14:13:58.058495 tautestz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-08 14:13:58.058495 tautestz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 14:13:57.882492 tautestz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-08 14:13:57.898492 tautestz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 14:13:58.058495 tautestz-1.1/tautestz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 14:13:57.882492 tautestz-1.1/tautestz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 14:13:57.890492 tautestz-1.1/tautestz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:14:02.384735 tautestz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 14:13:57.000000 tautestz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 18:14:02.384735 tautestz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 14:13:57.000000 tautestz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 18:14:02.384735 tautestz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-11 18:14:01.000000 tautestz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:14:02.380735 tautestz-2.1/tautestz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 14:13:57.000000 tautestz-2.1/tautestz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 14:13:57.000000 tautestz-2.1/tautestz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:14:02.380735 tautestz-2.1/tautestz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 18:14:02.000000 tautestz-2.1/tautestz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-11 18:14:02.000000 tautestz-2.1/tautestz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 18:14:02.000000 tautestz-2.1/tautestz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 18:14:02.000000 tautestz-2.1/tautestz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-11 18:14:02.000000 tautestz-2.1/tautestz.egg-info/top_level.txt
```

### Comparing `tautestz-1.1/setup.py` & `tautestz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'tautestz',
     packages = ['tautestz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'tautestz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/tautestz',
```

