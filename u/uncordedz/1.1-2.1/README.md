# Comparing `tmp/uncordedz-1.1.tar.gz` & `tmp/uncordedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uncordedz-1.1.tar", last modified: Mon May  6 15:18:57 2024, max compression
+gzip compressed data, was "uncordedz-2.1.tar", last modified: Sat May 11 20:34:13 2024, max compression
```

## Comparing `uncordedz-1.1.tar` & `uncordedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-06 15:18:57.369289 uncordedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-06 15:18:57.369289 uncordedz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-06 15:18:57.233287 uncordedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-06 15:18:57.245287 uncordedz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-06 15:18:57.369289 uncordedz-1.1/uncordedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-06 15:18:57.237287 uncordedz-1.1/uncordedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-06 15:18:57.241287 uncordedz-1.1/uncordedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:34:13.379660 uncordedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-06 15:18:57.000000 uncordedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 20:34:13.379660 uncordedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-06 15:18:57.000000 uncordedz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 20:34:13.379660 uncordedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-11 20:34:12.000000 uncordedz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:34:13.379660 uncordedz-2.1/uncordedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-06 15:18:57.000000 uncordedz-2.1/uncordedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-06 15:18:57.000000 uncordedz-2.1/uncordedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:34:13.379660 uncordedz-2.1/uncordedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 20:34:13.000000 uncordedz-2.1/uncordedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-11 20:34:13.000000 uncordedz-2.1/uncordedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 20:34:13.000000 uncordedz-2.1/uncordedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 20:34:13.000000 uncordedz-2.1/uncordedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-11 20:34:13.000000 uncordedz-2.1/uncordedz.egg-info/top_level.txt
```

### Comparing `uncordedz-1.1/setup.py` & `uncordedz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'uncordedz',
     packages = ['uncordedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'uncordedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/uncordedz',
```
