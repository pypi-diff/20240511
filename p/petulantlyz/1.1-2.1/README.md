# Comparing `tmp/petulantlyz-1.1.tar.gz` & `tmp/petulantlyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petulantlyz-1.1.tar", last modified: Thu May  9 09:15:07 2024, max compression
+gzip compressed data, was "petulantlyz-2.1.tar", last modified: Sat May 11 08:59:33 2024, max compression
```

## Comparing `petulantlyz-1.1.tar` & `petulantlyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 09:15:07.578423 petulantlyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-09 09:15:07.578423 petulantlyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 09:15:07.578423 petulantlyz-1.1/petulantlyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 09:15:02.362327 petulantlyz-1.1/petulantlyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 09:15:02.774335 petulantlyz-1.1/petulantlyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 09:15:02.358327 petulantlyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-09 09:15:03.102341 petulantlyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 08:59:33.315391 petulantlyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 09:15:02.000000 petulantlyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 08:59:33.315391 petulantlyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 09:15:02.000000 petulantlyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 08:59:33.315391 petulantlyz-2.1/petulantlyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 09:15:02.000000 petulantlyz-2.1/petulantlyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 09:15:02.000000 petulantlyz-2.1/petulantlyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 08:59:33.315391 petulantlyz-2.1/petulantlyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 08:59:33.000000 petulantlyz-2.1/petulantlyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-11 08:59:33.000000 petulantlyz-2.1/petulantlyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 08:59:33.000000 petulantlyz-2.1/petulantlyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 08:59:33.000000 petulantlyz-2.1/petulantlyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-11 08:59:33.000000 petulantlyz-2.1/petulantlyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 08:59:33.315391 petulantlyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-11 08:59:32.000000 petulantlyz-2.1/setup.py
```

### Comparing `petulantlyz-1.1/setup.py` & `petulantlyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'petulantlyz',
     packages = ['petulantlyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'petulantlyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/petulantlyz',
```

