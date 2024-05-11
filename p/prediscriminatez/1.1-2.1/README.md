# Comparing `tmp/prediscriminatez-1.1.tar.gz` & `tmp/prediscriminatez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prediscriminatez-1.1.tar", last modified: Fri May 10 04:13:41 2024, max compression
+gzip compressed data, was "prediscriminatez-2.1.tar", last modified: Sat May 11 10:42:22 2024, max compression
```

## Comparing `prediscriminatez-1.1.tar` & `prediscriminatez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 04:13:41.028001 prediscriminatez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1680 2024-05-10 04:13:41.028001 prediscriminatez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 04:13:41.028001 prediscriminatez-1.1/prediscriminatez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 04:13:40.843998 prediscriminatez-1.1/prediscriminatez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 04:13:40.855998 prediscriminatez-1.1/prediscriminatez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 04:13:40.843998 prediscriminatez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-10 04:13:40.863998 prediscriminatez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:42:22.269207 prediscriminatez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 04:13:40.000000 prediscriminatez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-11 10:42:22.269207 prediscriminatez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 04:13:40.000000 prediscriminatez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:42:22.269207 prediscriminatez-2.1/prediscriminatez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 04:13:40.000000 prediscriminatez-2.1/prediscriminatez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 04:13:40.000000 prediscriminatez-2.1/prediscriminatez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:42:22.269207 prediscriminatez-2.1/prediscriminatez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-11 10:42:21.000000 prediscriminatez-2.1/prediscriminatez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      289 2024-05-11 10:42:21.000000 prediscriminatez-2.1/prediscriminatez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 10:42:21.000000 prediscriminatez-2.1/prediscriminatez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 10:42:21.000000 prediscriminatez-2.1/prediscriminatez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       17 2024-05-11 10:42:21.000000 prediscriminatez-2.1/prediscriminatez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 10:42:22.269207 prediscriminatez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-11 10:42:16.000000 prediscriminatez-2.1/setup.py
```

### Comparing `prediscriminatez-1.1/setup.py` & `prediscriminatez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'prediscriminatez',
     packages = ['prediscriminatez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'prediscriminatez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/prediscriminatez',
```

