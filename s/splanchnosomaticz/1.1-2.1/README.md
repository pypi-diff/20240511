# Comparing `tmp/splanchnosomaticz-1.1.tar.gz` & `tmp/splanchnosomaticz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splanchnosomaticz-1.1.tar", last modified: Thu May  9 08:37:40 2024, max compression
+gzip compressed data, was "splanchnosomaticz-2.1.tar", last modified: Sat May 11 15:54:36 2024, max compression
```

## Comparing `splanchnosomaticz-1.1.tar` & `splanchnosomaticz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 08:37:40.657040 splanchnosomaticz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1684 2024-05-09 08:37:40.657040 splanchnosomaticz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 08:37:36.928971 splanchnosomaticz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-09 08:37:37.432981 splanchnosomaticz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 08:37:40.657040 splanchnosomaticz-1.1/splanchnosomaticz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 08:37:36.928971 splanchnosomaticz-1.1/splanchnosomaticz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 08:37:37.084974 splanchnosomaticz-1.1/splanchnosomaticz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:54:36.966264 splanchnosomaticz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 08:37:36.000000 splanchnosomaticz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 15:54:36.966264 splanchnosomaticz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 08:37:36.000000 splanchnosomaticz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 15:54:36.966264 splanchnosomaticz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-11 15:54:36.000000 splanchnosomaticz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:54:36.962263 splanchnosomaticz-2.1/splanchnosomaticz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 08:37:36.000000 splanchnosomaticz-2.1/splanchnosomaticz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 08:37:37.000000 splanchnosomaticz-2.1/splanchnosomaticz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:54:36.966264 splanchnosomaticz-2.1/splanchnosomaticz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 15:54:36.000000 splanchnosomaticz-2.1/splanchnosomaticz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      296 2024-05-11 15:54:36.000000 splanchnosomaticz-2.1/splanchnosomaticz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 15:54:36.000000 splanchnosomaticz-2.1/splanchnosomaticz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 15:54:36.000000 splanchnosomaticz-2.1/splanchnosomaticz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       18 2024-05-11 15:54:36.000000 splanchnosomaticz-2.1/splanchnosomaticz.egg-info/top_level.txt
```

### Comparing `splanchnosomaticz-1.1/setup.py` & `splanchnosomaticz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'splanchnosomaticz',
     packages = ['splanchnosomaticz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'splanchnosomaticz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/splanchnosomaticz',
```

