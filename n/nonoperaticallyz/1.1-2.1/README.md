# Comparing `tmp/nonoperaticallyz-1.1.tar.gz` & `tmp/nonoperaticallyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonoperaticallyz-1.1.tar", last modified: Wed May  8 13:52:12 2024, max compression
+gzip compressed data, was "nonoperaticallyz-2.1.tar", last modified: Sat May 11 06:13:03 2024, max compression
```

## Comparing `nonoperaticallyz-1.1.tar` & `nonoperaticallyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:52:12.218182 nonoperaticallyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1680 2024-05-08 13:52:12.218182 nonoperaticallyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 13:52:12.218182 nonoperaticallyz-1.1/nonoperaticallyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:52:12.014178 nonoperaticallyz-1.1/nonoperaticallyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:52:12.022178 nonoperaticallyz-1.1/nonoperaticallyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 13:52:12.014178 nonoperaticallyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-08 13:52:12.034178 nonoperaticallyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:13:03.652016 nonoperaticallyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 13:52:12.000000 nonoperaticallyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-11 06:13:03.652016 nonoperaticallyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 13:52:12.000000 nonoperaticallyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:13:03.636015 nonoperaticallyz-2.1/nonoperaticallyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 13:52:12.000000 nonoperaticallyz-2.1/nonoperaticallyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 13:52:12.000000 nonoperaticallyz-2.1/nonoperaticallyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:13:03.636015 nonoperaticallyz-2.1/nonoperaticallyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-11 06:13:03.000000 nonoperaticallyz-2.1/nonoperaticallyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      289 2024-05-11 06:13:03.000000 nonoperaticallyz-2.1/nonoperaticallyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 06:13:03.000000 nonoperaticallyz-2.1/nonoperaticallyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 06:13:03.000000 nonoperaticallyz-2.1/nonoperaticallyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       17 2024-05-11 06:13:03.000000 nonoperaticallyz-2.1/nonoperaticallyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 06:13:03.652016 nonoperaticallyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-11 06:13:03.000000 nonoperaticallyz-2.1/setup.py
```

### Comparing `nonoperaticallyz-1.1/setup.py` & `nonoperaticallyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'nonoperaticallyz',
     packages = ['nonoperaticallyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'nonoperaticallyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/nonoperaticallyz',
```

