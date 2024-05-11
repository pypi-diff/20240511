# Comparing `tmp/oordz-1.1.tar.gz` & `tmp/oordz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oordz-1.1.tar", last modified: Thu May  9 12:09:10 2024, max compression
+gzip compressed data, was "oordz-2.1.tar", last modified: Sat May 11 07:05:27 2024, max compression
```

## Comparing `oordz-1.1.tar` & `oordz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 12:09:10.494804 oordz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1636 2024-05-09 12:09:10.494804 oordz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 12:09:10.494804 oordz-1.1/oordz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 12:09:06.346726 oordz-1.1/oordz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 12:09:06.650731 oordz-1.1/oordz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 12:09:06.346726 oordz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1558 2024-05-09 12:09:07.134741 oordz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:05:27.413748 oordz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 12:09:06.000000 oordz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1898 2024-05-11 07:05:27.413748 oordz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 12:09:06.000000 oordz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:05:27.413748 oordz-2.1/oordz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 12:09:06.000000 oordz-2.1/oordz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 12:09:06.000000 oordz-2.1/oordz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:05:27.413748 oordz-2.1/oordz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1898 2024-05-11 07:05:27.000000 oordz-2.1/oordz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      212 2024-05-11 07:05:27.000000 oordz-2.1/oordz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 07:05:27.000000 oordz-2.1/oordz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 07:05:27.000000 oordz-2.1/oordz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        6 2024-05-11 07:05:27.000000 oordz-2.1/oordz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 07:05:27.413748 oordz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1558 2024-05-11 07:05:26.000000 oordz-2.1/setup.py
```

### Comparing `oordz-1.1/setup.py` & `oordz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'oordz',
     packages = ['oordz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'oordz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/oordz',
```

