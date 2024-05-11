# Comparing `tmp/tamerlanismz-1.1.tar.gz` & `tmp/tamerlanismz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamerlanismz-1.1.tar", last modified: Fri May 10 02:18:53 2024, max compression
+gzip compressed data, was "tamerlanismz-2.1.tar", last modified: Sat May 11 18:08:57 2024, max compression
```

## Comparing `tamerlanismz-1.1.tar` & `tamerlanismz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 02:18:53.308954 tamerlanismz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-10 02:18:53.308954 tamerlanismz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 02:18:53.076950 tamerlanismz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-10 02:18:53.100951 tamerlanismz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 02:18:53.308954 tamerlanismz-1.1/tamerlanismz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 02:18:53.076950 tamerlanismz-1.1/tamerlanismz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 02:18:53.088950 tamerlanismz-1.1/tamerlanismz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:08:57.819141 tamerlanismz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 02:18:53.000000 tamerlanismz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 18:08:57.819141 tamerlanismz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 02:18:53.000000 tamerlanismz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 18:08:57.819141 tamerlanismz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 18:08:57.000000 tamerlanismz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:08:57.819141 tamerlanismz-2.1/tamerlanismz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 02:18:53.000000 tamerlanismz-2.1/tamerlanismz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 02:18:53.000000 tamerlanismz-2.1/tamerlanismz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:08:57.819141 tamerlanismz-2.1/tamerlanismz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 18:08:57.000000 tamerlanismz-2.1/tamerlanismz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 18:08:57.000000 tamerlanismz-2.1/tamerlanismz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 18:08:57.000000 tamerlanismz-2.1/tamerlanismz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 18:08:57.000000 tamerlanismz-2.1/tamerlanismz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 18:08:57.000000 tamerlanismz-2.1/tamerlanismz.egg-info/top_level.txt
```

### Comparing `tamerlanismz-1.1/setup.py` & `tamerlanismz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'tamerlanismz',
     packages = ['tamerlanismz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'tamerlanismz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/tamerlanismz',
```

