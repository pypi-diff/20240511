# Comparing `tmp/irreclaimabilityz-1.1.tar.gz` & `tmp/irreclaimabilityz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irreclaimabilityz-1.1.tar", last modified: Thu May  9 16:58:13 2024, max compression
+gzip compressed data, was "irreclaimabilityz-2.1.tar", last modified: Sat May 11 00:46:24 2024, max compression
```

## Comparing `irreclaimabilityz-1.1.tar` & `irreclaimabilityz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 16:58:13.910116 irreclaimabilityz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1684 2024-05-09 16:58:13.910116 irreclaimabilityz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 16:58:13.910116 irreclaimabilityz-1.1/irreclaimabilityz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 16:58:12.430089 irreclaimabilityz-1.1/irreclaimabilityz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 16:58:12.578091 irreclaimabilityz-1.1/irreclaimabilityz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 16:58:12.430089 irreclaimabilityz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-09 16:58:12.814096 irreclaimabilityz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:46:24.123466 irreclaimabilityz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 16:58:12.000000 irreclaimabilityz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 00:46:24.123466 irreclaimabilityz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 16:58:12.000000 irreclaimabilityz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:46:24.119466 irreclaimabilityz-2.1/irreclaimabilityz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 16:58:12.000000 irreclaimabilityz-2.1/irreclaimabilityz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 16:58:12.000000 irreclaimabilityz-2.1/irreclaimabilityz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:46:24.119466 irreclaimabilityz-2.1/irreclaimabilityz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 00:46:23.000000 irreclaimabilityz-2.1/irreclaimabilityz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      296 2024-05-11 00:46:23.000000 irreclaimabilityz-2.1/irreclaimabilityz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 00:46:23.000000 irreclaimabilityz-2.1/irreclaimabilityz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 00:46:23.000000 irreclaimabilityz-2.1/irreclaimabilityz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       18 2024-05-11 00:46:23.000000 irreclaimabilityz-2.1/irreclaimabilityz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 00:46:24.123466 irreclaimabilityz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-11 00:46:18.000000 irreclaimabilityz-2.1/setup.py
```

### Comparing `irreclaimabilityz-1.1/setup.py` & `irreclaimabilityz-2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'irreclaimabilityz',
     packages = ['irreclaimabilityz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'irreclaimabilityz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/irreclaimabilityz',
```

