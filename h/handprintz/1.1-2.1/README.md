# Comparing `tmp/handprintz-1.1.tar.gz` & `tmp/handprintz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handprintz-1.1.tar", last modified: Wed May  8 15:19:41 2024, max compression
+gzip compressed data, was "handprintz-2.1.tar", last modified: Fri May 10 22:10:00 2024, max compression
```

## Comparing `handprintz-1.1.tar` & `handprintz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 15:19:41.766750 handprintz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 15:19:41.766750 handprintz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 15:19:41.766750 handprintz-1.1/handprintz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 15:19:41.570746 handprintz-1.1/handprintz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 15:19:41.578746 handprintz-1.1/handprintz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 15:19:41.570746 handprintz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 15:19:41.586747 handprintz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 22:10:00.294180 handprintz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 15:19:41.000000 handprintz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 22:10:00.294180 handprintz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 15:19:41.000000 handprintz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 22:10:00.290179 handprintz-2.1/handprintz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 15:19:41.000000 handprintz-2.1/handprintz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 15:19:41.000000 handprintz-2.1/handprintz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 22:10:00.294180 handprintz-2.1/handprintz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-10 22:09:59.000000 handprintz-2.1/handprintz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-10 22:09:59.000000 handprintz-2.1/handprintz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 22:09:59.000000 handprintz-2.1/handprintz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 22:09:59.000000 handprintz-2.1/handprintz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-10 22:09:59.000000 handprintz-2.1/handprintz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 22:10:00.294180 handprintz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 22:09:53.000000 handprintz-2.1/setup.py
```

### Comparing `handprintz-1.1/setup.py` & `handprintz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'handprintz',
     packages = ['handprintz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'handprintz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/handprintz',
```

