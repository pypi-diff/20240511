# Comparing `tmp/unirradiatedz-1.1.tar.gz` & `tmp/unirradiatedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unirradiatedz-1.1.tar", last modified: Thu May  9 21:04:14 2024, max compression
+gzip compressed data, was "unirradiatedz-2.1.tar", last modified: Sat May 11 21:16:35 2024, max compression
```

## Comparing `unirradiatedz-1.1.tar` & `unirradiatedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 21:04:14.005246 unirradiatedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-09 21:04:14.005246 unirradiatedz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 21:04:13.829243 unirradiatedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-09 21:04:13.845243 unirradiatedz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 21:04:14.005246 unirradiatedz-1.1/unirradiatedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 21:04:13.829243 unirradiatedz-1.1/unirradiatedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 21:04:13.837243 unirradiatedz-1.1/unirradiatedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:16:35.794469 unirradiatedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 21:04:13.000000 unirradiatedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 21:16:35.794469 unirradiatedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 21:04:13.000000 unirradiatedz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 21:16:35.794469 unirradiatedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 21:16:26.000000 unirradiatedz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:16:35.750468 unirradiatedz-2.1/unirradiatedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 21:04:13.000000 unirradiatedz-2.1/unirradiatedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 21:04:13.000000 unirradiatedz-2.1/unirradiatedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:16:35.794469 unirradiatedz-2.1/unirradiatedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 21:16:34.000000 unirradiatedz-2.1/unirradiatedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 21:16:34.000000 unirradiatedz-2.1/unirradiatedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 21:16:34.000000 unirradiatedz-2.1/unirradiatedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 21:16:34.000000 unirradiatedz-2.1/unirradiatedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 21:16:34.000000 unirradiatedz-2.1/unirradiatedz.egg-info/top_level.txt
```

### Comparing `unirradiatedz-1.1/setup.py` & `unirradiatedz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'unirradiatedz',
     packages = ['unirradiatedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'unirradiatedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/unirradiatedz',
```

