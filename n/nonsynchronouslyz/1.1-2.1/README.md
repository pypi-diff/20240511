# Comparing `tmp/nonsynchronouslyz-1.1.tar.gz` & `tmp/nonsynchronouslyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonsynchronouslyz-1.1.tar", last modified: Thu May  9 20:26:33 2024, max compression
+gzip compressed data, was "nonsynchronouslyz-2.1.tar", last modified: Sat May 11 06:28:47 2024, max compression
```

## Comparing `nonsynchronouslyz-1.1.tar` & `nonsynchronouslyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 20:26:33.575967 nonsynchronouslyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1684 2024-05-09 20:26:33.575967 nonsynchronouslyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 20:26:33.575967 nonsynchronouslyz-1.1/nonsynchronouslyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 20:26:33.403964 nonsynchronouslyz-1.1/nonsynchronouslyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 20:26:33.411964 nonsynchronouslyz-1.1/nonsynchronouslyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 20:26:33.403964 nonsynchronouslyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-09 20:26:33.419964 nonsynchronouslyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:28:47.252989 nonsynchronouslyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 20:26:33.000000 nonsynchronouslyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 06:28:47.252989 nonsynchronouslyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 20:26:33.000000 nonsynchronouslyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:28:47.252989 nonsynchronouslyz-2.1/nonsynchronouslyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 20:26:33.000000 nonsynchronouslyz-2.1/nonsynchronouslyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 20:26:33.000000 nonsynchronouslyz-2.1/nonsynchronouslyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:28:47.252989 nonsynchronouslyz-2.1/nonsynchronouslyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 06:28:46.000000 nonsynchronouslyz-2.1/nonsynchronouslyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      296 2024-05-11 06:28:46.000000 nonsynchronouslyz-2.1/nonsynchronouslyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 06:28:46.000000 nonsynchronouslyz-2.1/nonsynchronouslyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 06:28:46.000000 nonsynchronouslyz-2.1/nonsynchronouslyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       18 2024-05-11 06:28:46.000000 nonsynchronouslyz-2.1/nonsynchronouslyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 06:28:47.252989 nonsynchronouslyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-11 06:28:34.000000 nonsynchronouslyz-2.1/setup.py
```

### Comparing `nonsynchronouslyz-1.1/setup.py` & `nonsynchronouslyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'nonsynchronouslyz',
     packages = ['nonsynchronouslyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'nonsynchronouslyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/nonsynchronouslyz',
```

