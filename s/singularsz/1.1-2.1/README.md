# Comparing `tmp/singularsz-1.1.tar.gz` & `tmp/singularsz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singularsz-1.1.tar", last modified: Wed May  8 22:18:43 2024, max compression
+gzip compressed data, was "singularsz-2.1.tar", last modified: Sat May 11 15:23:15 2024, max compression
```

## Comparing `singularsz-1.1.tar` & `singularsz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 22:18:43.357887 singularsz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 22:18:43.357887 singularsz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 22:18:43.145883 singularsz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 22:18:43.165883 singularsz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 22:18:43.357887 singularsz-1.1/singularsz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 22:18:43.145883 singularsz-1.1/singularsz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 22:18:43.157883 singularsz-1.1/singularsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:23:15.667376 singularsz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 22:18:43.000000 singularsz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 15:23:15.667376 singularsz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 22:18:43.000000 singularsz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 15:23:15.671376 singularsz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 15:23:08.000000 singularsz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:23:15.667376 singularsz-2.1/singularsz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 22:18:43.000000 singularsz-2.1/singularsz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 22:18:43.000000 singularsz-2.1/singularsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:23:15.667376 singularsz-2.1/singularsz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 15:23:14.000000 singularsz-2.1/singularsz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 15:23:14.000000 singularsz-2.1/singularsz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 15:23:14.000000 singularsz-2.1/singularsz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 15:23:14.000000 singularsz-2.1/singularsz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 15:23:14.000000 singularsz-2.1/singularsz.egg-info/top_level.txt
```

### Comparing `singularsz-1.1/setup.py` & `singularsz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'singularsz',
     packages = ['singularsz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'singularsz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/singularsz',
```

