# Comparing `tmp/uninvigorativelyz-1.1.tar.gz` & `tmp/uninvigorativelyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uninvigorativelyz-1.1.tar", last modified: Thu May  9 08:26:39 2024, max compression
+gzip compressed data, was "uninvigorativelyz-2.1.tar", last modified: Sat May 11 21:11:15 2024, max compression
```

## Comparing `uninvigorativelyz-1.1.tar` & `uninvigorativelyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 08:26:39.400859 uninvigorativelyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1684 2024-05-09 08:26:39.400859 uninvigorativelyz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 08:26:39.212856 uninvigorativelyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-09 08:26:39.224856 uninvigorativelyz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 08:26:39.400859 uninvigorativelyz-1.1/uninvigorativelyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 08:26:39.212856 uninvigorativelyz-1.1/uninvigorativelyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 08:26:39.220856 uninvigorativelyz-1.1/uninvigorativelyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:11:15.364568 uninvigorativelyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 08:26:39.000000 uninvigorativelyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 21:11:15.364568 uninvigorativelyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 08:26:39.000000 uninvigorativelyz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 21:11:15.364568 uninvigorativelyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-11 21:11:14.000000 uninvigorativelyz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:11:15.364568 uninvigorativelyz-2.1/uninvigorativelyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 08:26:39.000000 uninvigorativelyz-2.1/uninvigorativelyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 08:26:39.000000 uninvigorativelyz-2.1/uninvigorativelyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:11:15.364568 uninvigorativelyz-2.1/uninvigorativelyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 21:11:15.000000 uninvigorativelyz-2.1/uninvigorativelyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      296 2024-05-11 21:11:15.000000 uninvigorativelyz-2.1/uninvigorativelyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 21:11:15.000000 uninvigorativelyz-2.1/uninvigorativelyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 21:11:15.000000 uninvigorativelyz-2.1/uninvigorativelyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       18 2024-05-11 21:11:15.000000 uninvigorativelyz-2.1/uninvigorativelyz.egg-info/top_level.txt
```

### Comparing `uninvigorativelyz-1.1/setup.py` & `uninvigorativelyz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'uninvigorativelyz',
     packages = ['uninvigorativelyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'uninvigorativelyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/uninvigorativelyz',
```

