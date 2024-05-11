# Comparing `tmp/perilenticularz-1.1.tar.gz` & `tmp/perilenticularz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perilenticularz-1.1.tar", last modified: Thu May  9 22:55:35 2024, max compression
+gzip compressed data, was "perilenticularz-2.1.tar", last modified: Sat May 11 08:33:31 2024, max compression
```

## Comparing `perilenticularz-1.1.tar` & `perilenticularz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 22:55:35.804596 perilenticularz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1676 2024-05-09 22:55:35.804596 perilenticularz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 22:55:35.804596 perilenticularz-1.1/perilenticularz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 22:55:33.324549 perilenticularz-1.1/perilenticularz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 22:55:33.492552 perilenticularz-1.1/perilenticularz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 22:55:33.324549 perilenticularz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-09 22:55:33.764557 perilenticularz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 08:33:31.706760 perilenticularz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 22:55:33.000000 perilenticularz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 08:33:31.706760 perilenticularz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 22:55:33.000000 perilenticularz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 08:33:31.702760 perilenticularz-2.1/perilenticularz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 22:55:33.000000 perilenticularz-2.1/perilenticularz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 22:55:33.000000 perilenticularz-2.1/perilenticularz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 08:33:31.706760 perilenticularz-2.1/perilenticularz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 08:33:30.000000 perilenticularz-2.1/perilenticularz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      282 2024-05-11 08:33:30.000000 perilenticularz-2.1/perilenticularz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 08:33:30.000000 perilenticularz-2.1/perilenticularz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 08:33:30.000000 perilenticularz-2.1/perilenticularz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       16 2024-05-11 08:33:30.000000 perilenticularz-2.1/perilenticularz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 08:33:31.706760 perilenticularz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-11 08:33:19.000000 perilenticularz-2.1/setup.py
```

### Comparing `perilenticularz-1.1/setup.py` & `perilenticularz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'perilenticularz',
     packages = ['perilenticularz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'perilenticularz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/perilenticularz',
```

