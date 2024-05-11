# Comparing `tmp/prerefinez-1.1.tar.gz` & `tmp/prerefinez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prerefinez-1.1.tar", last modified: Wed May  8 23:51:28 2024, max compression
+gzip compressed data, was "prerefinez-2.1.tar", last modified: Sat May 11 11:14:06 2024, max compression
```

## Comparing `prerefinez-1.1.tar` & `prerefinez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 23:51:28.980265 prerefinez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 23:51:28.980265 prerefinez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 23:51:28.980265 prerefinez-1.1/prerefinez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 23:51:27.196233 prerefinez-1.1/prerefinez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 23:51:27.376236 prerefinez-1.1/prerefinez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 23:51:27.196233 prerefinez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 23:51:27.584240 prerefinez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:14:06.456312 prerefinez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 23:51:27.000000 prerefinez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 11:14:06.456312 prerefinez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 23:51:27.000000 prerefinez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:14:06.456312 prerefinez-2.1/prerefinez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 23:51:27.000000 prerefinez-2.1/prerefinez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 23:51:27.000000 prerefinez-2.1/prerefinez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:14:06.456312 prerefinez-2.1/prerefinez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 11:14:06.000000 prerefinez-2.1/prerefinez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 11:14:06.000000 prerefinez-2.1/prerefinez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 11:14:06.000000 prerefinez-2.1/prerefinez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 11:14:06.000000 prerefinez-2.1/prerefinez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 11:14:06.000000 prerefinez-2.1/prerefinez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 11:14:06.460312 prerefinez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 11:14:05.000000 prerefinez-2.1/setup.py
```

### Comparing `prerefinez-1.1/setup.py` & `prerefinez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'prerefinez',
     packages = ['prerefinez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'prerefinez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/prerefinez',
```

