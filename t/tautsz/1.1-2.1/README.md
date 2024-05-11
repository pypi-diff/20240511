# Comparing `tmp/tautsz-1.1.tar.gz` & `tmp/tautsz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tautsz-1.1.tar", last modified: Wed May  8 23:01:29 2024, max compression
+gzip compressed data, was "tautsz-2.1.tar", last modified: Sat May 11 18:19:08 2024, max compression
```

## Comparing `tautsz-1.1.tar` & `tautsz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 23:01:29.349068 tautsz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1640 2024-05-08 23:01:29.349068 tautsz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 23:01:29.145064 tautsz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1566 2024-05-08 23:01:29.169064 tautsz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 23:01:29.349068 tautsz-1.1/tautsz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 23:01:29.145064 tautsz-1.1/tautsz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 23:01:29.157064 tautsz-1.1/tautsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:19:08.058360 tautsz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 23:01:29.000000 tautsz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1905 2024-05-11 18:19:08.058360 tautsz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 23:01:29.000000 tautsz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 18:19:08.058360 tautsz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1566 2024-05-11 18:19:07.000000 tautsz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:19:08.058360 tautsz-2.1/tautsz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 23:01:29.000000 tautsz-2.1/tautsz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 23:01:29.000000 tautsz-2.1/tautsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:19:08.058360 tautsz-2.1/tautsz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1905 2024-05-11 18:19:07.000000 tautsz-2.1/tautsz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      219 2024-05-11 18:19:07.000000 tautsz-2.1/tautsz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 18:19:07.000000 tautsz-2.1/tautsz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 18:19:07.000000 tautsz-2.1/tautsz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        7 2024-05-11 18:19:07.000000 tautsz-2.1/tautsz.egg-info/top_level.txt
```

### Comparing `tautsz-1.1/setup.py` & `tautsz-2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'tautsz',
     packages = ['tautsz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'tautsz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/tautsz',
```

