# Comparing `tmp/moldersz-1.1.tar.gz` & `tmp/moldersz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moldersz-1.1.tar", last modified: Wed May  8 18:08:20 2024, max compression
+gzip compressed data, was "moldersz-2.1.tar", last modified: Sat May 11 04:56:30 2024, max compression
```

## Comparing `moldersz-1.1.tar` & `moldersz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 18:08:20.577536 moldersz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-08 18:08:20.577536 moldersz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 18:08:20.577536 moldersz-1.1/moldersz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 18:08:17.473479 moldersz-1.1/moldersz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 18:08:17.653482 moldersz-1.1/moldersz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 18:08:17.473479 moldersz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-08 18:08:17.957487 moldersz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:56:30.599099 moldersz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 18:08:17.000000 moldersz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 04:56:30.599099 moldersz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 18:08:17.000000 moldersz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:56:30.599099 moldersz-2.1/moldersz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 18:08:17.000000 moldersz-2.1/moldersz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 18:08:17.000000 moldersz-2.1/moldersz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:56:30.599099 moldersz-2.1/moldersz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 04:56:30.000000 moldersz-2.1/moldersz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-11 04:56:30.000000 moldersz-2.1/moldersz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 04:56:30.000000 moldersz-2.1/moldersz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 04:56:30.000000 moldersz-2.1/moldersz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-11 04:56:30.000000 moldersz-2.1/moldersz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 04:56:30.599099 moldersz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-11 04:56:30.000000 moldersz-2.1/setup.py
```

### Comparing `moldersz-1.1/setup.py` & `moldersz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'moldersz',
     packages = ['moldersz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'moldersz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/moldersz',
```

