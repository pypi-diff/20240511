# Comparing `tmp/spiremz-1.1.tar.gz` & `tmp/spiremz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiremz-1.1.tar", last modified: Thu May  9 02:50:26 2024, max compression
+gzip compressed data, was "spiremz-2.1.tar", last modified: Sat May 11 15:49:17 2024, max compression
```

## Comparing `spiremz-1.1.tar` & `spiremz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:50:25.925598 spiremz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1644 2024-05-09 02:50:25.925598 spiremz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 02:50:18.193457 spiremz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-09 02:50:19.613483 spiremz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:50:25.925598 spiremz-1.1/spiremz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:50:18.193457 spiremz-1.1/spiremz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:50:18.597465 spiremz-1.1/spiremz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:49:17.856190 spiremz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 02:50:18.000000 spiremz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-11 15:49:17.856190 spiremz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 02:50:18.000000 spiremz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 15:49:17.856190 spiremz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-11 15:49:11.000000 spiremz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:49:17.852190 spiremz-2.1/spiremz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:50:18.000000 spiremz-2.1/spiremz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:50:18.000000 spiremz-2.1/spiremz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:49:17.856190 spiremz-2.1/spiremz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-11 15:49:17.000000 spiremz-2.1/spiremz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      226 2024-05-11 15:49:17.000000 spiremz-2.1/spiremz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 15:49:17.000000 spiremz-2.1/spiremz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 15:49:17.000000 spiremz-2.1/spiremz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-11 15:49:17.000000 spiremz-2.1/spiremz.egg-info/top_level.txt
```

### Comparing `spiremz-1.1/setup.py` & `spiremz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'spiremz',
     packages = ['spiremz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'spiremz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/spiremz',
```

