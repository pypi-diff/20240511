# Comparing `tmp/integripalliatez-1.1.tar.gz` & `tmp/integripalliatez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integripalliatez-1.1.tar", last modified: Thu May  9 05:56:39 2024, max compression
+gzip compressed data, was "integripalliatez-2.1.tar", last modified: Sat May 11 00:25:38 2024, max compression
```

## Comparing `integripalliatez-1.1.tar` & `integripalliatez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:56:39.187204 integripalliatez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1680 2024-05-09 05:56:39.187204 integripalliatez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:56:39.187204 integripalliatez-1.1/integripalliatez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:56:35.931144 integripalliatez-1.1/integripalliatez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:56:36.147148 integripalliatez-1.1/integripalliatez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 05:56:35.931144 integripalliatez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-09 05:56:36.543156 integripalliatez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:25:38.700508 integripalliatez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 05:56:35.000000 integripalliatez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-11 00:25:38.700508 integripalliatez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 05:56:35.000000 integripalliatez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:25:38.700508 integripalliatez-2.1/integripalliatez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:56:35.000000 integripalliatez-2.1/integripalliatez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:56:36.000000 integripalliatez-2.1/integripalliatez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:25:38.700508 integripalliatez-2.1/integripalliatez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-11 00:25:38.000000 integripalliatez-2.1/integripalliatez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      289 2024-05-11 00:25:38.000000 integripalliatez-2.1/integripalliatez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 00:25:38.000000 integripalliatez-2.1/integripalliatez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 00:25:38.000000 integripalliatez-2.1/integripalliatez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       17 2024-05-11 00:25:38.000000 integripalliatez-2.1/integripalliatez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 00:25:38.700508 integripalliatez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-11 00:25:38.000000 integripalliatez-2.1/setup.py
```

### Comparing `integripalliatez-1.1/setup.py` & `integripalliatez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'integripalliatez',
     packages = ['integripalliatez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'integripalliatez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/integripalliatez',
```

