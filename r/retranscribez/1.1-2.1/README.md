# Comparing `tmp/retranscribez-1.1.tar.gz` & `tmp/retranscribez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retranscribez-1.1.tar", last modified: Thu May  9 17:37:00 2024, max compression
+gzip compressed data, was "retranscribez-2.1.tar", last modified: Sat May 11 13:44:25 2024, max compression
```

## Comparing `retranscribez-1.1.tar` & `retranscribez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 17:37:00.428922 retranscribez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-09 17:37:00.428922 retranscribez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 17:37:00.428922 retranscribez-1.1/retranscribez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 17:36:57.668871 retranscribez-1.1/retranscribez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 17:36:57.820874 retranscribez-1.1/retranscribez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 17:36:57.664871 retranscribez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-09 17:36:58.196881 retranscribez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 13:44:25.673722 retranscribez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 17:36:57.000000 retranscribez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 13:44:25.673722 retranscribez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 17:36:57.000000 retranscribez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 13:44:25.673722 retranscribez-2.1/retranscribez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 17:36:57.000000 retranscribez-2.1/retranscribez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 17:36:57.000000 retranscribez-2.1/retranscribez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 13:44:25.673722 retranscribez-2.1/retranscribez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 13:44:25.000000 retranscribez-2.1/retranscribez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 13:44:25.000000 retranscribez-2.1/retranscribez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 13:44:25.000000 retranscribez-2.1/retranscribez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 13:44:25.000000 retranscribez-2.1/retranscribez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 13:44:25.000000 retranscribez-2.1/retranscribez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 13:44:25.677722 retranscribez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 13:44:21.000000 retranscribez-2.1/setup.py
```

### Comparing `retranscribez-1.1/setup.py` & `retranscribez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'retranscribez',
     packages = ['retranscribez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'retranscribez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/retranscribez',
```

