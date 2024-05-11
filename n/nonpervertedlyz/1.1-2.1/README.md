# Comparing `tmp/nonpervertedlyz-1.1.tar.gz` & `tmp/nonpervertedlyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonpervertedlyz-1.1.tar", last modified: Wed May  8 21:52:06 2024, max compression
+gzip compressed data, was "nonpervertedlyz-2.1.tar", last modified: Sat May 11 06:18:14 2024, max compression
```

## Comparing `nonpervertedlyz-1.1.tar` & `nonpervertedlyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 21:52:06.304561 nonpervertedlyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1676 2024-05-08 21:52:06.304561 nonpervertedlyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 21:52:06.304561 nonpervertedlyz-1.1/nonpervertedlyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 21:52:06.112557 nonpervertedlyz-1.1/nonpervertedlyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 21:52:06.120557 nonpervertedlyz-1.1/nonpervertedlyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 21:52:06.112557 nonpervertedlyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-08 21:52:06.124557 nonpervertedlyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:18:14.397548 nonpervertedlyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 21:52:06.000000 nonpervertedlyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 06:18:14.397548 nonpervertedlyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 21:52:06.000000 nonpervertedlyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:18:14.397548 nonpervertedlyz-2.1/nonpervertedlyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 21:52:06.000000 nonpervertedlyz-2.1/nonpervertedlyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 21:52:06.000000 nonpervertedlyz-2.1/nonpervertedlyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:18:14.397548 nonpervertedlyz-2.1/nonpervertedlyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 06:18:14.000000 nonpervertedlyz-2.1/nonpervertedlyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      282 2024-05-11 06:18:14.000000 nonpervertedlyz-2.1/nonpervertedlyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 06:18:14.000000 nonpervertedlyz-2.1/nonpervertedlyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 06:18:14.000000 nonpervertedlyz-2.1/nonpervertedlyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       16 2024-05-11 06:18:14.000000 nonpervertedlyz-2.1/nonpervertedlyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 06:18:14.401548 nonpervertedlyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-11 06:18:09.000000 nonpervertedlyz-2.1/setup.py
```

### Comparing `nonpervertedlyz-1.1/setup.py` & `nonpervertedlyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'nonpervertedlyz',
     packages = ['nonpervertedlyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'nonpervertedlyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/nonpervertedlyz',
```

