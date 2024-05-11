# Comparing `tmp/sanctimonyz-1.1.tar.gz` & `tmp/sanctimonyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanctimonyz-1.1.tar", last modified: Wed May  8 12:59:13 2024, max compression
+gzip compressed data, was "sanctimonyz-2.1.tar", last modified: Sat May 11 14:25:33 2024, max compression
```

## Comparing `sanctimonyz-1.1.tar` & `sanctimonyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 12:59:13.619536 sanctimonyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-08 12:59:13.619536 sanctimonyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 12:59:13.619536 sanctimonyz-1.1/sanctimonyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 12:59:11.523498 sanctimonyz-1.1/sanctimonyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 12:59:11.667500 sanctimonyz-1.1/sanctimonyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 12:59:11.523498 sanctimonyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-08 12:59:11.903505 sanctimonyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:25:33.467570 sanctimonyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 12:59:11.000000 sanctimonyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 14:25:33.467570 sanctimonyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 12:59:11.000000 sanctimonyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:25:33.467570 sanctimonyz-2.1/sanctimonyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 12:59:11.000000 sanctimonyz-2.1/sanctimonyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 12:59:11.000000 sanctimonyz-2.1/sanctimonyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:25:33.467570 sanctimonyz-2.1/sanctimonyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 14:25:33.000000 sanctimonyz-2.1/sanctimonyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-11 14:25:33.000000 sanctimonyz-2.1/sanctimonyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 14:25:33.000000 sanctimonyz-2.1/sanctimonyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 14:25:33.000000 sanctimonyz-2.1/sanctimonyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-11 14:25:33.000000 sanctimonyz-2.1/sanctimonyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 14:25:33.467570 sanctimonyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-11 14:25:32.000000 sanctimonyz-2.1/setup.py
```

### Comparing `sanctimonyz-1.1/setup.py` & `sanctimonyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'sanctimonyz',
     packages = ['sanctimonyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'sanctimonyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/sanctimonyz',
```

