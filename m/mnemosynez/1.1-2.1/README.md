# Comparing `tmp/mnemosynez-1.1.tar.gz` & `tmp/mnemosynez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnemosynez-1.1.tar", last modified: Thu May  9 10:04:19 2024, max compression
+gzip compressed data, was "mnemosynez-2.1.tar", last modified: Sat May 11 04:51:26 2024, max compression
```

## Comparing `mnemosynez-1.1.tar` & `mnemosynez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 10:04:18.996807 mnemosynez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 10:04:18.996807 mnemosynez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 10:04:18.996807 mnemosynez-1.1/mnemosynez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 10:04:16.684765 mnemosynez-1.1/mnemosynez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 10:04:16.916769 mnemosynez-1.1/mnemosynez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 10:04:16.684765 mnemosynez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 10:04:17.068772 mnemosynez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:51:26.105524 mnemosynez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 10:04:16.000000 mnemosynez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 04:51:26.105524 mnemosynez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 10:04:16.000000 mnemosynez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:51:26.101524 mnemosynez-2.1/mnemosynez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 10:04:16.000000 mnemosynez-2.1/mnemosynez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 10:04:16.000000 mnemosynez-2.1/mnemosynez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:51:26.105524 mnemosynez-2.1/mnemosynez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 04:51:25.000000 mnemosynez-2.1/mnemosynez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 04:51:25.000000 mnemosynez-2.1/mnemosynez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 04:51:25.000000 mnemosynez-2.1/mnemosynez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 04:51:25.000000 mnemosynez-2.1/mnemosynez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 04:51:25.000000 mnemosynez-2.1/mnemosynez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 04:51:26.105524 mnemosynez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 04:51:25.000000 mnemosynez-2.1/setup.py
```

### Comparing `mnemosynez-1.1/setup.py` & `mnemosynez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'mnemosynez',
     packages = ['mnemosynez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'mnemosynez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/mnemosynez',
```

