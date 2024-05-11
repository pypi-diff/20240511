# Comparing `tmp/roughhousingz-1.1.tar.gz` & `tmp/roughhousingz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roughhousingz-1.1.tar", last modified: Thu May  9 03:44:40 2024, max compression
+gzip compressed data, was "roughhousingz-2.1.tar", last modified: Sat May 11 14:10:16 2024, max compression
```

## Comparing `roughhousingz-1.1.tar` & `roughhousingz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 03:44:40.873491 roughhousingz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-09 03:44:40.873491 roughhousingz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 03:44:40.873491 roughhousingz-1.1/roughhousingz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 03:44:39.925474 roughhousingz-1.1/roughhousingz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 03:44:40.089477 roughhousingz-1.1/roughhousingz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 03:44:39.921474 roughhousingz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-09 03:44:40.321481 roughhousingz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:10:16.466267 roughhousingz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 03:44:39.000000 roughhousingz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 14:10:16.466267 roughhousingz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 03:44:39.000000 roughhousingz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:10:16.466267 roughhousingz-2.1/roughhousingz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 03:44:39.000000 roughhousingz-2.1/roughhousingz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 03:44:40.000000 roughhousingz-2.1/roughhousingz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:10:16.466267 roughhousingz-2.1/roughhousingz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 14:10:16.000000 roughhousingz-2.1/roughhousingz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 14:10:16.000000 roughhousingz-2.1/roughhousingz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 14:10:16.000000 roughhousingz-2.1/roughhousingz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 14:10:16.000000 roughhousingz-2.1/roughhousingz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 14:10:16.000000 roughhousingz-2.1/roughhousingz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 14:10:16.466267 roughhousingz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 14:10:15.000000 roughhousingz-2.1/setup.py
```

### Comparing `roughhousingz-1.1/setup.py` & `roughhousingz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'roughhousingz',
     packages = ['roughhousingz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'roughhousingz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/roughhousingz',
```

