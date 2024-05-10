# Comparing `tmp/inappellablez-1.1.tar.gz` & `tmp/inappellablez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inappellablez-1.1.tar", last modified: Thu May  9 10:09:53 2024, max compression
+gzip compressed data, was "inappellablez-2.1.tar", last modified: Fri May 10 23:44:43 2024, max compression
```

## Comparing `inappellablez-1.1.tar` & `inappellablez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 10:09:53.662972 inappellablez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-09 10:09:53.662972 inappellablez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 10:09:53.662972 inappellablez-1.1/inappellablez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 10:09:46.594842 inappellablez-1.1/inappellablez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 10:09:47.006850 inappellablez-1.1/inappellablez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 10:09:46.594842 inappellablez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-09 10:09:47.642861 inappellablez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 23:44:43.295332 inappellablez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 10:09:46.000000 inappellablez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-10 23:44:43.295332 inappellablez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 10:09:46.000000 inappellablez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 23:44:43.291332 inappellablez-2.1/inappellablez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 10:09:46.000000 inappellablez-2.1/inappellablez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 10:09:47.000000 inappellablez-2.1/inappellablez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 23:44:43.291332 inappellablez-2.1/inappellablez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-10 23:44:43.000000 inappellablez-2.1/inappellablez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-10 23:44:43.000000 inappellablez-2.1/inappellablez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 23:44:43.000000 inappellablez-2.1/inappellablez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 23:44:43.000000 inappellablez-2.1/inappellablez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-10 23:44:43.000000 inappellablez-2.1/inappellablez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 23:44:43.295332 inappellablez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-10 23:44:42.000000 inappellablez-2.1/setup.py
```

### Comparing `inappellablez-1.1/setup.py` & `inappellablez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'inappellablez',
     packages = ['inappellablez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'inappellablez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/inappellablez',
```

