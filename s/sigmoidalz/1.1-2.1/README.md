# Comparing `tmp/sigmoidalz-1.1.tar.gz` & `tmp/sigmoidalz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmoidalz-1.1.tar", last modified: Wed May  8 21:20:06 2024, max compression
+gzip compressed data, was "sigmoidalz-2.1.tar", last modified: Sat May 11 15:07:27 2024, max compression
```

## Comparing `sigmoidalz-1.1.tar` & `sigmoidalz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 21:20:06.017219 sigmoidalz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 21:20:06.017219 sigmoidalz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 21:20:02.369151 sigmoidalz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 21:20:02.785159 sigmoidalz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 21:20:06.017219 sigmoidalz-1.1/sigmoidalz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 21:20:02.369151 sigmoidalz-1.1/sigmoidalz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 21:20:02.505154 sigmoidalz-1.1/sigmoidalz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:07:27.357891 sigmoidalz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 21:20:02.000000 sigmoidalz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 15:07:27.357891 sigmoidalz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 21:20:02.000000 sigmoidalz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 15:07:27.357891 sigmoidalz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 15:07:26.000000 sigmoidalz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:07:27.357891 sigmoidalz-2.1/sigmoidalz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 21:20:02.000000 sigmoidalz-2.1/sigmoidalz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 21:20:02.000000 sigmoidalz-2.1/sigmoidalz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:07:27.357891 sigmoidalz-2.1/sigmoidalz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 15:07:27.000000 sigmoidalz-2.1/sigmoidalz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 15:07:27.000000 sigmoidalz-2.1/sigmoidalz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 15:07:27.000000 sigmoidalz-2.1/sigmoidalz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 15:07:27.000000 sigmoidalz-2.1/sigmoidalz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 15:07:27.000000 sigmoidalz-2.1/sigmoidalz.egg-info/top_level.txt
```

### Comparing `sigmoidalz-1.1/setup.py` & `sigmoidalz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'sigmoidalz',
     packages = ['sigmoidalz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'sigmoidalz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/sigmoidalz',
```

