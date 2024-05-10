# Comparing `tmp/hematospermatocelez-1.1.tar.gz` & `tmp/hematospermatocelez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hematospermatocelez-1.1.tar", last modified: Wed May  8 21:25:45 2024, max compression
+gzip compressed data, was "hematospermatocelez-2.1.tar", last modified: Fri May 10 22:25:51 2024, max compression
```

## Comparing `hematospermatocelez-1.1.tar` & `hematospermatocelez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 21:25:45.355478 hematospermatocelez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1692 2024-05-08 21:25:45.355478 hematospermatocelez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 21:25:45.355478 hematospermatocelez-1.1/hematospermatocelez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 21:25:42.675429 hematospermatocelez-1.1/hematospermatocelez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 21:25:42.779431 hematospermatocelez-1.1/hematospermatocelez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 21:25:42.675429 hematospermatocelez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1670 2024-05-08 21:25:43.159438 hematospermatocelez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 22:25:51.543499 hematospermatocelez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 21:25:42.000000 hematospermatocelez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1996 2024-05-10 22:25:51.543499 hematospermatocelez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 21:25:42.000000 hematospermatocelez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 22:25:51.499498 hematospermatocelez-2.1/hematospermatocelez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 21:25:42.000000 hematospermatocelez-2.1/hematospermatocelez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 21:25:42.000000 hematospermatocelez-2.1/hematospermatocelez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 22:25:51.543499 hematospermatocelez-2.1/hematospermatocelez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1996 2024-05-10 22:25:50.000000 hematospermatocelez-2.1/hematospermatocelez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      310 2024-05-10 22:25:50.000000 hematospermatocelez-2.1/hematospermatocelez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-10 22:25:50.000000 hematospermatocelez-2.1/hematospermatocelez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-10 22:25:50.000000 hematospermatocelez-2.1/hematospermatocelez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       20 2024-05-10 22:25:50.000000 hematospermatocelez-2.1/hematospermatocelez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-10 22:25:51.543499 hematospermatocelez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1670 2024-05-10 22:25:45.000000 hematospermatocelez-2.1/setup.py
```

### Comparing `hematospermatocelez-1.1/setup.py` & `hematospermatocelez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'hematospermatocelez',
     packages = ['hematospermatocelez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'hematospermatocelez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/hematospermatocelez',
```

