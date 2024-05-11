# Comparing `tmp/rhadamanthinez-1.1.tar.gz` & `tmp/rhadamanthinez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhadamanthinez-1.1.tar", last modified: Fri May 10 03:52:09 2024, max compression
+gzip compressed data, was "rhadamanthinez-2.1.tar", last modified: Sat May 11 14:00:00 2024, max compression
```

## Comparing `rhadamanthinez-1.1.tar` & `rhadamanthinez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 03:52:09.283979 rhadamanthinez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1672 2024-05-10 03:52:09.283979 rhadamanthinez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 03:52:09.283979 rhadamanthinez-1.1/rhadamanthinez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 03:52:09.083975 rhadamanthinez-1.1/rhadamanthinez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 03:52:09.091975 rhadamanthinez-1.1/rhadamanthinez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 03:52:09.083975 rhadamanthinez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-10 03:52:09.103975 rhadamanthinez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:00:00.902853 rhadamanthinez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 03:52:09.000000 rhadamanthinez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 14:00:00.902853 rhadamanthinez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 03:52:09.000000 rhadamanthinez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:00:00.902853 rhadamanthinez-2.1/rhadamanthinez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 03:52:09.000000 rhadamanthinez-2.1/rhadamanthinez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 03:52:09.000000 rhadamanthinez-2.1/rhadamanthinez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:00:00.902853 rhadamanthinez-2.1/rhadamanthinez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 14:00:00.000000 rhadamanthinez-2.1/rhadamanthinez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      275 2024-05-11 14:00:00.000000 rhadamanthinez-2.1/rhadamanthinez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 14:00:00.000000 rhadamanthinez-2.1/rhadamanthinez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 14:00:00.000000 rhadamanthinez-2.1/rhadamanthinez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       15 2024-05-11 14:00:00.000000 rhadamanthinez-2.1/rhadamanthinez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 14:00:00.902853 rhadamanthinez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-11 14:00:00.000000 rhadamanthinez-2.1/setup.py
```

### Comparing `rhadamanthinez-1.1/setup.py` & `rhadamanthinez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'rhadamanthinez',
     packages = ['rhadamanthinez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'rhadamanthinez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/rhadamanthinez',
```

