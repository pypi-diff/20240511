# Comparing `tmp/micrologicz-1.1.tar.gz` & `tmp/micrologicz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micrologicz-1.1.tar", last modified: Thu May  9 15:29:07 2024, max compression
+gzip compressed data, was "micrologicz-2.1.tar", last modified: Sat May 11 04:25:27 2024, max compression
```

## Comparing `micrologicz-1.1.tar` & `micrologicz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 15:29:07.823691 micrologicz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-09 15:29:07.823691 micrologicz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 15:29:07.823691 micrologicz-1.1/micrologicz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 15:29:03.815617 micrologicz-1.1/micrologicz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 15:29:04.063621 micrologicz-1.1/micrologicz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 15:29:03.815617 micrologicz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-09 15:29:04.327626 micrologicz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:25:27.569137 micrologicz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 15:29:03.000000 micrologicz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 04:25:27.569137 micrologicz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 15:29:03.000000 micrologicz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:25:27.565137 micrologicz-2.1/micrologicz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 15:29:03.000000 micrologicz-2.1/micrologicz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 15:29:04.000000 micrologicz-2.1/micrologicz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:25:27.569137 micrologicz-2.1/micrologicz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 04:25:27.000000 micrologicz-2.1/micrologicz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-11 04:25:27.000000 micrologicz-2.1/micrologicz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 04:25:27.000000 micrologicz-2.1/micrologicz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 04:25:27.000000 micrologicz-2.1/micrologicz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-11 04:25:27.000000 micrologicz-2.1/micrologicz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 04:25:27.569137 micrologicz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-11 04:25:27.000000 micrologicz-2.1/setup.py
```

### Comparing `micrologicz-1.1/setup.py` & `micrologicz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'micrologicz',
     packages = ['micrologicz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'micrologicz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/micrologicz',
```

