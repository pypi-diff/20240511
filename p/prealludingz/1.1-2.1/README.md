# Comparing `tmp/prealludingz-1.1.tar.gz` & `tmp/prealludingz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prealludingz-1.1.tar", last modified: Thu May  9 03:02:06 2024, max compression
+gzip compressed data, was "prealludingz-2.1.tar", last modified: Sat May 11 10:21:40 2024, max compression
```

## Comparing `prealludingz-1.1.tar` & `prealludingz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 03:02:06.254486 prealludingz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 03:02:06.254486 prealludingz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 03:02:06.254486 prealludingz-1.1/prealludingz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 03:02:03.778440 prealludingz-1.1/prealludingz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 03:02:03.966444 prealludingz-1.1/prealludingz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 03:02:03.778440 prealludingz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 03:02:04.230449 prealludingz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:21:40.182266 prealludingz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 03:02:03.000000 prealludingz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 10:21:40.182266 prealludingz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 03:02:03.000000 prealludingz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:21:40.182266 prealludingz-2.1/prealludingz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 03:02:03.000000 prealludingz-2.1/prealludingz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 03:02:03.000000 prealludingz-2.1/prealludingz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:21:40.182266 prealludingz-2.1/prealludingz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 10:21:40.000000 prealludingz-2.1/prealludingz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 10:21:40.000000 prealludingz-2.1/prealludingz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 10:21:40.000000 prealludingz-2.1/prealludingz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 10:21:40.000000 prealludingz-2.1/prealludingz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 10:21:40.000000 prealludingz-2.1/prealludingz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 10:21:40.182266 prealludingz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 10:21:39.000000 prealludingz-2.1/setup.py
```

### Comparing `prealludingz-1.1/setup.py` & `prealludingz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'prealludingz',
     packages = ['prealludingz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'prealludingz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/prealludingz',
```

