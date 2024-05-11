# Comparing `tmp/preinstallationz-1.1.tar.gz` & `tmp/preinstallationz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preinstallationz-1.1.tar", last modified: Wed May  8 12:40:54 2024, max compression
+gzip compressed data, was "preinstallationz-2.1.tar", last modified: Sat May 11 10:58:23 2024, max compression
```

## Comparing `preinstallationz-1.1.tar` & `preinstallationz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 12:40:54.103382 preinstallationz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1680 2024-05-08 12:40:54.103382 preinstallationz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 12:40:54.103382 preinstallationz-1.1/preinstallationz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 12:40:49.419295 preinstallationz-1.1/preinstallationz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 12:40:49.763301 preinstallationz-1.1/preinstallationz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 12:40:49.419295 preinstallationz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-08 12:40:49.767301 preinstallationz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:58:23.010921 preinstallationz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 12:40:49.000000 preinstallationz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-11 10:58:23.010921 preinstallationz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 12:40:49.000000 preinstallationz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:58:23.006920 preinstallationz-2.1/preinstallationz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 12:40:49.000000 preinstallationz-2.1/preinstallationz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 12:40:49.000000 preinstallationz-2.1/preinstallationz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:58:23.010921 preinstallationz-2.1/preinstallationz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-11 10:58:22.000000 preinstallationz-2.1/preinstallationz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      289 2024-05-11 10:58:22.000000 preinstallationz-2.1/preinstallationz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 10:58:22.000000 preinstallationz-2.1/preinstallationz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 10:58:22.000000 preinstallationz-2.1/preinstallationz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       17 2024-05-11 10:58:22.000000 preinstallationz-2.1/preinstallationz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 10:58:23.010921 preinstallationz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-11 10:58:16.000000 preinstallationz-2.1/setup.py
```

### Comparing `preinstallationz-1.1/setup.py` & `preinstallationz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'preinstallationz',
     packages = ['preinstallationz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'preinstallationz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/preinstallationz',
```

