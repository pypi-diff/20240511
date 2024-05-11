# Comparing `tmp/subgroupz-1.1.tar.gz` & `tmp/subgroupz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subgroupz-1.1.tar", last modified: Thu May  9 00:07:27 2024, max compression
+gzip compressed data, was "subgroupz-2.1.tar", last modified: Sat May 11 17:01:15 2024, max compression
```

## Comparing `subgroupz-1.1.tar` & `subgroupz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 00:07:27.793898 subgroupz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-09 00:07:27.793898 subgroupz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 00:07:23.889826 subgroupz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-09 00:07:24.577839 subgroupz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 00:07:27.793898 subgroupz-1.1/subgroupz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 00:07:23.889826 subgroupz-1.1/subgroupz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 00:07:24.177832 subgroupz-1.1/subgroupz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:01:15.520168 subgroupz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 00:07:23.000000 subgroupz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 17:01:15.520168 subgroupz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 00:07:23.000000 subgroupz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 17:01:15.520168 subgroupz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-11 17:01:09.000000 subgroupz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:01:15.520168 subgroupz-2.1/subgroupz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 00:07:23.000000 subgroupz-2.1/subgroupz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 00:07:24.000000 subgroupz-2.1/subgroupz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:01:15.520168 subgroupz-2.1/subgroupz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 17:01:14.000000 subgroupz-2.1/subgroupz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-11 17:01:14.000000 subgroupz-2.1/subgroupz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 17:01:14.000000 subgroupz-2.1/subgroupz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 17:01:14.000000 subgroupz-2.1/subgroupz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-11 17:01:14.000000 subgroupz-2.1/subgroupz.egg-info/top_level.txt
```

### Comparing `subgroupz-1.1/setup.py` & `subgroupz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'subgroupz',
     packages = ['subgroupz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'subgroupz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/subgroupz',
```

