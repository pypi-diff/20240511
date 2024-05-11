# Comparing `tmp/soundlesslyz-1.1.tar.gz` & `tmp/soundlesslyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundlesslyz-1.1.tar", last modified: Thu May  9 02:56:23 2024, max compression
+gzip compressed data, was "soundlesslyz-2.1.tar", last modified: Sat May 11 15:38:52 2024, max compression
```

## Comparing `soundlesslyz-1.1.tar` & `soundlesslyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:56:23.148111 soundlesslyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 02:56:23.148111 soundlesslyz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 02:56:15.535972 soundlesslyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 02:56:16.683993 soundlesslyz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 02:56:23.148111 soundlesslyz-1.1/soundlesslyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:56:15.535972 soundlesslyz-1.1/soundlesslyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:56:15.991980 soundlesslyz-1.1/soundlesslyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:38:52.816661 soundlesslyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 02:56:15.000000 soundlesslyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 15:38:52.816661 soundlesslyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 02:56:15.000000 soundlesslyz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 15:38:52.816661 soundlesslyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 15:38:52.000000 soundlesslyz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:38:52.812661 soundlesslyz-2.1/soundlesslyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 02:56:15.000000 soundlesslyz-2.1/soundlesslyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 02:56:15.000000 soundlesslyz-2.1/soundlesslyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:38:52.812661 soundlesslyz-2.1/soundlesslyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 15:38:52.000000 soundlesslyz-2.1/soundlesslyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 15:38:52.000000 soundlesslyz-2.1/soundlesslyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 15:38:52.000000 soundlesslyz-2.1/soundlesslyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 15:38:52.000000 soundlesslyz-2.1/soundlesslyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 15:38:52.000000 soundlesslyz-2.1/soundlesslyz.egg-info/top_level.txt
```

### Comparing `soundlesslyz-1.1/setup.py` & `soundlesslyz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'soundlesslyz',
     packages = ['soundlesslyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'soundlesslyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/soundlesslyz',
```

