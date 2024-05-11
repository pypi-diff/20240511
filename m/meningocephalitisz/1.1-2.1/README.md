# Comparing `tmp/meningocephalitisz-1.1.tar.gz` & `tmp/meningocephalitisz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meningocephalitisz-1.1.tar", last modified: Wed May  8 20:52:55 2024, max compression
+gzip compressed data, was "meningocephalitisz-2.1.tar", last modified: Sat May 11 04:04:24 2024, max compression
```

## Comparing `meningocephalitisz-1.1.tar` & `meningocephalitisz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 20:52:55.527329 meningocephalitisz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1688 2024-05-08 20:52:55.527329 meningocephalitisz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 20:52:55.527329 meningocephalitisz-1.1/meningocephalitisz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 20:52:52.423272 meningocephalitisz-1.1/meningocephalitisz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 20:52:52.579275 meningocephalitisz-1.1/meningocephalitisz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 20:52:52.423272 meningocephalitisz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1662 2024-05-08 20:52:52.815279 meningocephalitisz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:04:24.893954 meningocephalitisz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 20:52:52.000000 meningocephalitisz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1989 2024-05-11 04:04:24.893954 meningocephalitisz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 20:52:52.000000 meningocephalitisz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:04:24.893954 meningocephalitisz-2.1/meningocephalitisz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 20:52:52.000000 meningocephalitisz-2.1/meningocephalitisz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 20:52:52.000000 meningocephalitisz-2.1/meningocephalitisz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:04:24.893954 meningocephalitisz-2.1/meningocephalitisz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1989 2024-05-11 04:04:24.000000 meningocephalitisz-2.1/meningocephalitisz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      303 2024-05-11 04:04:24.000000 meningocephalitisz-2.1/meningocephalitisz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 04:04:24.000000 meningocephalitisz-2.1/meningocephalitisz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 04:04:24.000000 meningocephalitisz-2.1/meningocephalitisz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       19 2024-05-11 04:04:24.000000 meningocephalitisz-2.1/meningocephalitisz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 04:04:24.893954 meningocephalitisz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1662 2024-05-11 04:04:24.000000 meningocephalitisz-2.1/setup.py
```

### Comparing `meningocephalitisz-1.1/setup.py` & `meningocephalitisz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'meningocephalitisz',
     packages = ['meningocephalitisz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'meningocephalitisz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/meningocephalitisz',
```

