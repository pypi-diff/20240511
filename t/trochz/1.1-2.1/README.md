# Comparing `tmp/trochz-1.1.tar.gz` & `tmp/trochz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trochz-1.1.tar", last modified: Thu May  9 21:57:33 2024, max compression
+gzip compressed data, was "trochz-2.1.tar", last modified: Sat May 11 19:47:46 2024, max compression
```

## Comparing `trochz-1.1.tar` & `trochz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 21:57:33.016492 trochz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1640 2024-05-09 21:57:33.016492 trochz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 21:57:32.832489 trochz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1566 2024-05-09 21:57:32.848489 trochz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 21:57:33.016492 trochz-1.1/trochz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 21:57:32.832489 trochz-1.1/trochz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 21:57:32.844489 trochz-1.1/trochz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:47:46.116402 trochz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 21:57:32.000000 trochz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1905 2024-05-11 19:47:46.116402 trochz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 21:57:32.000000 trochz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 19:47:46.120402 trochz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1566 2024-05-11 19:47:45.000000 trochz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:47:46.116402 trochz-2.1/trochz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 21:57:32.000000 trochz-2.1/trochz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 21:57:32.000000 trochz-2.1/trochz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:47:46.116402 trochz-2.1/trochz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1905 2024-05-11 19:47:45.000000 trochz-2.1/trochz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      219 2024-05-11 19:47:46.000000 trochz-2.1/trochz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 19:47:45.000000 trochz-2.1/trochz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 19:47:45.000000 trochz-2.1/trochz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        7 2024-05-11 19:47:45.000000 trochz-2.1/trochz.egg-info/top_level.txt
```

### Comparing `trochz-1.1/setup.py` & `trochz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'trochz',
     packages = ['trochz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'trochz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/trochz',
```

