# Comparing `tmp/overprecisez-1.1.tar.gz` & `tmp/overprecisez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overprecisez-1.1.tar", last modified: Thu May  9 12:52:26 2024, max compression
+gzip compressed data, was "overprecisez-2.1.tar", last modified: Sat May 11 07:41:35 2024, max compression
```

## Comparing `overprecisez-1.1.tar` & `overprecisez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 12:52:26.518935 overprecisez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 12:52:26.518935 overprecisez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 12:52:26.518935 overprecisez-1.1/overprecisez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 12:52:26.338932 overprecisez-1.1/overprecisez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 12:52:26.346932 overprecisez-1.1/overprecisez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 12:52:26.338932 overprecisez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 12:52:26.358932 overprecisez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:41:35.317536 overprecisez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 12:52:26.000000 overprecisez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 07:41:35.317536 overprecisez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 12:52:26.000000 overprecisez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:41:35.313536 overprecisez-2.1/overprecisez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 12:52:26.000000 overprecisez-2.1/overprecisez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 12:52:26.000000 overprecisez-2.1/overprecisez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:41:35.313536 overprecisez-2.1/overprecisez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 07:41:35.000000 overprecisez-2.1/overprecisez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 07:41:35.000000 overprecisez-2.1/overprecisez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 07:41:35.000000 overprecisez-2.1/overprecisez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 07:41:35.000000 overprecisez-2.1/overprecisez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 07:41:35.000000 overprecisez-2.1/overprecisez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 07:41:35.317536 overprecisez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 07:41:34.000000 overprecisez-2.1/setup.py
```

### Comparing `overprecisez-1.1/setup.py` & `overprecisez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'overprecisez',
     packages = ['overprecisez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'overprecisez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/overprecisez',
```

