# Comparing `tmp/streaminessz-1.1.tar.gz` & `tmp/streaminessz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaminessz-1.1.tar", last modified: Thu May  9 21:46:39 2024, max compression
+gzip compressed data, was "streaminessz-2.1.tar", last modified: Sat May 11 16:40:49 2024, max compression
```

## Comparing `streaminessz-1.1.tar` & `streaminessz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 21:46:39.664465 streaminessz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 21:46:39.664465 streaminessz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 21:46:39.488462 streaminessz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 21:46:39.504462 streaminessz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 21:46:39.664465 streaminessz-1.1/streaminessz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 21:46:39.488462 streaminessz-1.1/streaminessz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 21:46:39.496462 streaminessz-1.1/streaminessz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:40:49.969580 streaminessz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 21:46:39.000000 streaminessz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 16:40:49.969580 streaminessz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 21:46:39.000000 streaminessz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 16:40:49.969580 streaminessz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 16:40:49.000000 streaminessz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:40:49.969580 streaminessz-2.1/streaminessz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 21:46:39.000000 streaminessz-2.1/streaminessz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 21:46:39.000000 streaminessz-2.1/streaminessz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:40:49.969580 streaminessz-2.1/streaminessz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 16:40:49.000000 streaminessz-2.1/streaminessz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 16:40:49.000000 streaminessz-2.1/streaminessz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 16:40:49.000000 streaminessz-2.1/streaminessz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 16:40:49.000000 streaminessz-2.1/streaminessz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 16:40:49.000000 streaminessz-2.1/streaminessz.egg-info/top_level.txt
```

### Comparing `streaminessz-1.1/setup.py` & `streaminessz-2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'streaminessz',
     packages = ['streaminessz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'streaminessz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/streaminessz',
```

