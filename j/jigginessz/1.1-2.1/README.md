# Comparing `tmp/jigginessz-1.1.tar.gz` & `tmp/jigginessz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jigginessz-1.1.tar", last modified: Wed May  8 16:30:34 2024, max compression
+gzip compressed data, was "jigginessz-2.1.tar", last modified: Sat May 11 01:02:03 2024, max compression
```

## Comparing `jigginessz-1.1.tar` & `jigginessz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:30:34.425335 jigginessz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 16:30:34.425335 jigginessz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 16:30:34.425335 jigginessz-1.1/jigginessz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:30:31.005271 jigginessz-1.1/jigginessz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:30:31.185275 jigginessz-1.1/jigginessz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 16:30:31.005271 jigginessz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 16:30:31.433279 jigginessz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:02:03.324817 jigginessz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 16:30:31.000000 jigginessz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 01:02:03.324817 jigginessz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 16:30:31.000000 jigginessz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:02:03.320817 jigginessz-2.1/jigginessz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 16:30:31.000000 jigginessz-2.1/jigginessz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 16:30:31.000000 jigginessz-2.1/jigginessz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:02:03.324817 jigginessz-2.1/jigginessz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 01:02:03.000000 jigginessz-2.1/jigginessz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 01:02:03.000000 jigginessz-2.1/jigginessz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 01:02:03.000000 jigginessz-2.1/jigginessz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 01:02:03.000000 jigginessz-2.1/jigginessz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 01:02:03.000000 jigginessz-2.1/jigginessz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 01:02:03.324817 jigginessz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 01:02:02.000000 jigginessz-2.1/setup.py
```

### Comparing `jigginessz-1.1/setup.py` & `jigginessz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'jigginessz',
     packages = ['jigginessz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'jigginessz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/jigginessz',
```

