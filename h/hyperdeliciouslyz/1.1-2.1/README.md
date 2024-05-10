# Comparing `tmp/hyperdeliciouslyz-1.1.tar.gz` & `tmp/hyperdeliciouslyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdeliciouslyz-1.1.tar", last modified: Wed May  8 22:08:21 2024, max compression
+gzip compressed data, was "hyperdeliciouslyz-2.1.tar", last modified: Fri May 10 23:07:21 2024, max compression
```

## Comparing `hyperdeliciouslyz-1.1.tar` & `hyperdeliciouslyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 22:08:21.850468 hyperdeliciouslyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1684 2024-05-08 22:08:21.850468 hyperdeliciouslyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 22:08:21.850468 hyperdeliciouslyz-1.1/hyperdeliciouslyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 22:08:21.658465 hyperdeliciouslyz-1.1/hyperdeliciouslyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 22:08:21.670465 hyperdeliciouslyz-1.1/hyperdeliciouslyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 22:08:21.658465 hyperdeliciouslyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-08 22:08:21.678465 hyperdeliciouslyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 23:07:21.681179 hyperdeliciouslyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 22:08:21.000000 hyperdeliciouslyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-10 23:07:21.681179 hyperdeliciouslyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 22:08:21.000000 hyperdeliciouslyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 23:07:21.681179 hyperdeliciouslyz-2.1/hyperdeliciouslyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 22:08:21.000000 hyperdeliciouslyz-2.1/hyperdeliciouslyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 22:08:21.000000 hyperdeliciouslyz-2.1/hyperdeliciouslyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 23:07:21.681179 hyperdeliciouslyz-2.1/hyperdeliciouslyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-10 23:07:19.000000 hyperdeliciouslyz-2.1/hyperdeliciouslyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      296 2024-05-10 23:07:19.000000 hyperdeliciouslyz-2.1/hyperdeliciouslyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 23:07:19.000000 hyperdeliciouslyz-2.1/hyperdeliciouslyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 23:07:19.000000 hyperdeliciouslyz-2.1/hyperdeliciouslyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       18 2024-05-10 23:07:19.000000 hyperdeliciouslyz-2.1/hyperdeliciouslyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 23:07:21.681179 hyperdeliciouslyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-10 23:07:12.000000 hyperdeliciouslyz-2.1/setup.py
```

### Comparing `hyperdeliciouslyz-1.1/setup.py` & `hyperdeliciouslyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'hyperdeliciouslyz',
     packages = ['hyperdeliciouslyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'hyperdeliciouslyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/hyperdeliciouslyz',
```

