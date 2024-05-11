# Comparing `tmp/oenochoaez-1.1.tar.gz` & `tmp/oenochoaez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oenochoaez-1.1.tar", last modified: Wed May  8 19:52:31 2024, max compression
+gzip compressed data, was "oenochoaez-2.1.tar", last modified: Sat May 11 06:44:27 2024, max compression
```

## Comparing `oenochoaez-1.1.tar` & `oenochoaez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 19:52:31.368920 oenochoaez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-08 19:52:31.368920 oenochoaez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 19:52:31.368920 oenochoaez-1.1/oenochoaez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 19:52:28.380864 oenochoaez-1.1/oenochoaez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 19:52:28.524867 oenochoaez-1.1/oenochoaez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 19:52:28.380864 oenochoaez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-08 19:52:28.752871 oenochoaez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:44:27.162127 oenochoaez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 19:52:28.000000 oenochoaez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 06:44:27.162127 oenochoaez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 19:52:28.000000 oenochoaez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:44:27.158127 oenochoaez-2.1/oenochoaez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 19:52:28.000000 oenochoaez-2.1/oenochoaez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 19:52:28.000000 oenochoaez-2.1/oenochoaez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:44:27.162127 oenochoaez-2.1/oenochoaez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 06:44:27.000000 oenochoaez-2.1/oenochoaez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 06:44:27.000000 oenochoaez-2.1/oenochoaez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 06:44:27.000000 oenochoaez-2.1/oenochoaez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 06:44:27.000000 oenochoaez-2.1/oenochoaez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 06:44:27.000000 oenochoaez-2.1/oenochoaez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 06:44:27.162127 oenochoaez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 06:44:26.000000 oenochoaez-2.1/setup.py
```

### Comparing `oenochoaez-1.1/setup.py` & `oenochoaez-2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'oenochoaez',
     packages = ['oenochoaez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'oenochoaez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/oenochoaez',
```

