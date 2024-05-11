# Comparing `tmp/subdichotomouslyz-1.1.tar.gz` & `tmp/subdichotomouslyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subdichotomouslyz-1.1.tar", last modified: Thu May  9 07:48:11 2024, max compression
+gzip compressed data, was "subdichotomouslyz-2.1.tar", last modified: Sat May 11 16:50:58 2024, max compression
```

## Comparing `subdichotomouslyz-1.1.tar` & `subdichotomouslyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 07:48:11.746301 subdichotomouslyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1684 2024-05-09 07:48:11.746301 subdichotomouslyz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 07:48:05.034178 subdichotomouslyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-09 07:48:06.166199 subdichotomouslyz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 07:48:11.746301 subdichotomouslyz-1.1/subdichotomouslyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 07:48:05.034178 subdichotomouslyz-1.1/subdichotomouslyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 07:48:05.358184 subdichotomouslyz-1.1/subdichotomouslyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:50:58.820785 subdichotomouslyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 07:48:05.000000 subdichotomouslyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 16:50:58.820785 subdichotomouslyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 07:48:05.000000 subdichotomouslyz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 16:50:58.820785 subdichotomouslyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-11 16:50:58.000000 subdichotomouslyz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:50:58.820785 subdichotomouslyz-2.1/subdichotomouslyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 07:48:05.000000 subdichotomouslyz-2.1/subdichotomouslyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 07:48:05.000000 subdichotomouslyz-2.1/subdichotomouslyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:50:58.820785 subdichotomouslyz-2.1/subdichotomouslyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 16:50:58.000000 subdichotomouslyz-2.1/subdichotomouslyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      296 2024-05-11 16:50:58.000000 subdichotomouslyz-2.1/subdichotomouslyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 16:50:58.000000 subdichotomouslyz-2.1/subdichotomouslyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 16:50:58.000000 subdichotomouslyz-2.1/subdichotomouslyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       18 2024-05-11 16:50:58.000000 subdichotomouslyz-2.1/subdichotomouslyz.egg-info/top_level.txt
```

### Comparing `subdichotomouslyz-1.1/setup.py` & `subdichotomouslyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'subdichotomouslyz',
     packages = ['subdichotomouslyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'subdichotomouslyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/subdichotomouslyz',
```

