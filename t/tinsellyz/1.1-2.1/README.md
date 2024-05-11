# Comparing `tmp/tinsellyz-1.1.tar.gz` & `tmp/tinsellyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinsellyz-1.1.tar", last modified: Wed May  8 14:46:37 2024, max compression
+gzip compressed data, was "tinsellyz-2.1.tar", last modified: Sat May 11 19:11:22 2024, max compression
```

## Comparing `tinsellyz-1.1.tar` & `tinsellyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 14:46:37.666300 tinsellyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1652 2024-05-08 14:46:37.670300 tinsellyz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 14:46:32.210200 tinsellyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-08 14:46:33.034215 tinsellyz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 14:46:37.666300 tinsellyz-1.1/tinsellyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 14:46:32.210200 tinsellyz-1.1/tinsellyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 14:46:32.498205 tinsellyz-1.1/tinsellyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:11:22.324132 tinsellyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 14:46:32.000000 tinsellyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 19:11:22.324132 tinsellyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 14:46:32.000000 tinsellyz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 19:11:22.352132 tinsellyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1590 2024-05-11 19:11:21.000000 tinsellyz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:11:22.312132 tinsellyz-2.1/tinsellyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 14:46:32.000000 tinsellyz-2.1/tinsellyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 14:46:32.000000 tinsellyz-2.1/tinsellyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 19:11:22.324132 tinsellyz-2.1/tinsellyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1926 2024-05-11 19:11:22.000000 tinsellyz-2.1/tinsellyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      240 2024-05-11 19:11:22.000000 tinsellyz-2.1/tinsellyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 19:11:22.000000 tinsellyz-2.1/tinsellyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 19:11:22.000000 tinsellyz-2.1/tinsellyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       10 2024-05-11 19:11:22.000000 tinsellyz-2.1/tinsellyz.egg-info/top_level.txt
```

### Comparing `tinsellyz-1.1/setup.py` & `tinsellyz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'tinsellyz',
     packages = ['tinsellyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'tinsellyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/tinsellyz',
```

