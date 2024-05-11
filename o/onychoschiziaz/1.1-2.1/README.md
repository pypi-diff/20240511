# Comparing `tmp/onychoschiziaz-1.1.tar.gz` & `tmp/onychoschiziaz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onychoschiziaz-1.1.tar", last modified: Fri May 10 00:57:10 2024, max compression
+gzip compressed data, was "onychoschiziaz-2.1.tar", last modified: Sat May 11 07:00:12 2024, max compression
```

## Comparing `onychoschiziaz-1.1.tar` & `onychoschiziaz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 00:57:10.578725 onychoschiziaz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1672 2024-05-10 00:57:10.578725 onychoschiziaz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 00:57:10.578725 onychoschiziaz-1.1/onychoschiziaz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 00:57:08.182680 onychoschiziaz-1.1/onychoschiziaz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 00:57:08.322683 onychoschiziaz-1.1/onychoschiziaz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 00:57:08.182680 onychoschiziaz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-10 00:57:08.506686 onychoschiziaz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:00:12.307917 onychoschiziaz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 00:57:08.000000 onychoschiziaz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 07:00:12.307917 onychoschiziaz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 00:57:08.000000 onychoschiziaz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:00:12.223916 onychoschiziaz-2.1/onychoschiziaz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 00:57:08.000000 onychoschiziaz-2.1/onychoschiziaz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 00:57:08.000000 onychoschiziaz-2.1/onychoschiziaz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:00:12.307917 onychoschiziaz-2.1/onychoschiziaz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 07:00:10.000000 onychoschiziaz-2.1/onychoschiziaz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      275 2024-05-11 07:00:10.000000 onychoschiziaz-2.1/onychoschiziaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 07:00:10.000000 onychoschiziaz-2.1/onychoschiziaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 07:00:10.000000 onychoschiziaz-2.1/onychoschiziaz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       15 2024-05-11 07:00:10.000000 onychoschiziaz-2.1/onychoschiziaz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 07:00:12.307917 onychoschiziaz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-11 06:59:57.000000 onychoschiziaz-2.1/setup.py
```

### Comparing `onychoschiziaz-1.1/setup.py` & `onychoschiziaz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'onychoschiziaz',
     packages = ['onychoschiziaz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'onychoschiziaz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/onychoschiziaz',
```

