# Comparing `tmp/synoviaz-1.1.tar.gz` & `tmp/synoviaz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synoviaz-1.1.tar", last modified: Thu May  9 04:27:50 2024, max compression
+gzip compressed data, was "synoviaz-2.1.tar", last modified: Sat May 11 17:58:33 2024, max compression
```

## Comparing `synoviaz-1.1.tar` & `synoviaz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 04:27:50.877282 synoviaz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-09 04:27:50.877282 synoviaz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 04:27:50.657278 synoviaz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-09 04:27:50.677278 synoviaz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 04:27:50.877282 synoviaz-1.1/synoviaz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 04:27:50.657278 synoviaz-1.1/synoviaz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 04:27:50.665278 synoviaz-1.1/synoviaz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:58:33.303627 synoviaz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 04:27:50.000000 synoviaz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 17:58:33.303627 synoviaz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 04:27:50.000000 synoviaz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 17:58:33.303627 synoviaz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-11 17:58:32.000000 synoviaz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:58:33.299627 synoviaz-2.1/synoviaz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 04:27:50.000000 synoviaz-2.1/synoviaz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 04:27:50.000000 synoviaz-2.1/synoviaz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:58:33.303627 synoviaz-2.1/synoviaz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 17:58:33.000000 synoviaz-2.1/synoviaz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-11 17:58:33.000000 synoviaz-2.1/synoviaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 17:58:33.000000 synoviaz-2.1/synoviaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 17:58:33.000000 synoviaz-2.1/synoviaz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-11 17:58:33.000000 synoviaz-2.1/synoviaz.egg-info/top_level.txt
```

### Comparing `synoviaz-1.1/setup.py` & `synoviaz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'synoviaz',
     packages = ['synoviaz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'synoviaz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/synoviaz',
```

