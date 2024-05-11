# Comparing `tmp/marinesz-1.1.tar.gz` & `tmp/marinesz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marinesz-1.1.tar", last modified: Thu May  9 06:13:28 2024, max compression
+gzip compressed data, was "marinesz-2.1.tar", last modified: Sat May 11 03:38:19 2024, max compression
```

## Comparing `marinesz-1.1.tar` & `marinesz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 06:13:28.865761 marinesz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-09 06:13:28.865761 marinesz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 06:13:28.865761 marinesz-1.1/marinesz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 06:13:28.649757 marinesz-1.1/marinesz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 06:13:28.673758 marinesz-1.1/marinesz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 06:13:28.649757 marinesz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-09 06:13:28.681758 marinesz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:38:19.029193 marinesz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 06:13:28.000000 marinesz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 03:38:19.029193 marinesz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 06:13:28.000000 marinesz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:38:19.029193 marinesz-2.1/marinesz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 06:13:28.000000 marinesz-2.1/marinesz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 06:13:28.000000 marinesz-2.1/marinesz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 03:38:19.029193 marinesz-2.1/marinesz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 03:38:18.000000 marinesz-2.1/marinesz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-11 03:38:18.000000 marinesz-2.1/marinesz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 03:38:18.000000 marinesz-2.1/marinesz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 03:38:18.000000 marinesz-2.1/marinesz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-11 03:38:18.000000 marinesz-2.1/marinesz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 03:38:19.033193 marinesz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-11 03:38:13.000000 marinesz-2.1/setup.py
```

### Comparing `marinesz-1.1/setup.py` & `marinesz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'marinesz',
     packages = ['marinesz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'marinesz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/marinesz',
```

