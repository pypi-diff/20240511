# Comparing `tmp/nonproduciblez-1.1.tar.gz` & `tmp/nonproduciblez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonproduciblez-1.1.tar", last modified: Fri May 10 03:30:22 2024, max compression
+gzip compressed data, was "nonproduciblez-2.1.tar", last modified: Sat May 11 06:23:26 2024, max compression
```

## Comparing `nonproduciblez-1.1.tar` & `nonproduciblez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 03:30:22.920085 nonproduciblez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1672 2024-05-10 03:30:22.920085 nonproduciblez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 03:30:22.920085 nonproduciblez-1.1/nonproduciblez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 03:30:17.455986 nonproduciblez-1.1/nonproduciblez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 03:30:18.047996 nonproduciblez-1.1/nonproduciblez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 03:30:17.455986 nonproduciblez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-10 03:30:18.744009 nonproduciblez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:23:26.219166 nonproduciblez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 03:30:17.000000 nonproduciblez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 06:23:26.219166 nonproduciblez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 03:30:17.000000 nonproduciblez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:23:26.219166 nonproduciblez-2.1/nonproduciblez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 03:30:17.000000 nonproduciblez-2.1/nonproduciblez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 03:30:18.000000 nonproduciblez-2.1/nonproduciblez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:23:26.219166 nonproduciblez-2.1/nonproduciblez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 06:23:25.000000 nonproduciblez-2.1/nonproduciblez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      275 2024-05-11 06:23:25.000000 nonproduciblez-2.1/nonproduciblez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 06:23:25.000000 nonproduciblez-2.1/nonproduciblez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 06:23:25.000000 nonproduciblez-2.1/nonproduciblez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       15 2024-05-11 06:23:25.000000 nonproduciblez-2.1/nonproduciblez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 06:23:26.219166 nonproduciblez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-11 06:23:19.000000 nonproduciblez-2.1/setup.py
```

### Comparing `nonproduciblez-1.1/setup.py` & `nonproduciblez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'nonproduciblez',
     packages = ['nonproduciblez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'nonproduciblez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/nonproduciblez',
```

