# Comparing `tmp/multiovulatez-1.1.tar.gz` & `tmp/multiovulatez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiovulatez-1.1.tar", last modified: Wed May  8 22:45:20 2024, max compression
+gzip compressed data, was "multiovulatez-2.1.tar", last modified: Sat May 11 05:11:42 2024, max compression
```

## Comparing `multiovulatez-1.1.tar` & `multiovulatez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 22:45:20.007238 multiovulatez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-08 22:45:20.007238 multiovulatez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 22:45:20.007238 multiovulatez-1.1/multiovulatez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 22:45:16.883181 multiovulatez-1.1/multiovulatez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 22:45:17.027183 multiovulatez-1.1/multiovulatez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 22:45:16.883181 multiovulatez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-08 22:45:17.287188 multiovulatez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:11:42.960137 multiovulatez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 22:45:16.000000 multiovulatez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 05:11:42.960137 multiovulatez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 22:45:16.000000 multiovulatez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:11:42.960137 multiovulatez-2.1/multiovulatez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 22:45:16.000000 multiovulatez-2.1/multiovulatez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 22:45:17.000000 multiovulatez-2.1/multiovulatez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:11:42.960137 multiovulatez-2.1/multiovulatez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 05:11:42.000000 multiovulatez-2.1/multiovulatez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 05:11:42.000000 multiovulatez-2.1/multiovulatez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 05:11:42.000000 multiovulatez-2.1/multiovulatez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 05:11:42.000000 multiovulatez-2.1/multiovulatez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 05:11:42.000000 multiovulatez-2.1/multiovulatez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 05:11:42.960137 multiovulatez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 05:11:42.000000 multiovulatez-2.1/setup.py
```

### Comparing `multiovulatez-1.1/setup.py` & `multiovulatez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'multiovulatez',
     packages = ['multiovulatez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'multiovulatez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/multiovulatez',
```

