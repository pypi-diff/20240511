# Comparing `tmp/propertyshipz-1.1.tar.gz` & `tmp/propertyshipz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propertyshipz-1.1.tar", last modified: Thu May  9 01:45:36 2024, max compression
+gzip compressed data, was "propertyshipz-2.1.tar", last modified: Sat May 11 11:40:01 2024, max compression
```

## Comparing `propertyshipz-1.1.tar` & `propertyshipz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:45:36.298728 propertyshipz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-09 01:45:36.298728 propertyshipz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:45:36.298728 propertyshipz-1.1/propertyshipz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:45:32.722662 propertyshipz-1.1/propertyshipz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:45:32.930666 propertyshipz-1.1/propertyshipz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 01:45:32.722662 propertyshipz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-09 01:45:33.306673 propertyshipz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:40:01.328528 propertyshipz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 01:45:32.000000 propertyshipz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 11:40:01.328528 propertyshipz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 01:45:32.000000 propertyshipz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:40:01.328528 propertyshipz-2.1/propertyshipz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:45:32.000000 propertyshipz-2.1/propertyshipz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:45:32.000000 propertyshipz-2.1/propertyshipz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:40:01.328528 propertyshipz-2.1/propertyshipz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 11:40:00.000000 propertyshipz-2.1/propertyshipz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 11:40:00.000000 propertyshipz-2.1/propertyshipz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 11:40:00.000000 propertyshipz-2.1/propertyshipz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 11:40:00.000000 propertyshipz-2.1/propertyshipz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 11:40:00.000000 propertyshipz-2.1/propertyshipz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 11:40:01.328528 propertyshipz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 11:39:53.000000 propertyshipz-2.1/setup.py
```

### Comparing `propertyshipz-1.1/setup.py` & `propertyshipz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'propertyshipz',
     packages = ['propertyshipz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'propertyshipz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/propertyshipz',
```

