# Comparing `tmp/prerogativityz-1.1.tar.gz` & `tmp/prerogativityz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prerogativityz-1.1.tar", last modified: Thu May  9 23:17:29 2024, max compression
+gzip compressed data, was "prerogativityz-2.1.tar", last modified: Sat May 11 11:19:17 2024, max compression
```

## Comparing `prerogativityz-1.1.tar` & `prerogativityz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 23:17:29.557016 prerogativityz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1672 2024-05-09 23:17:29.557016 prerogativityz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 23:17:29.557016 prerogativityz-1.1/prerogativityz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 23:17:29.353012 prerogativityz-1.1/prerogativityz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 23:17:29.365012 prerogativityz-1.1/prerogativityz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 23:17:29.353012 prerogativityz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-09 23:17:29.369012 prerogativityz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:19:17.501972 prerogativityz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 23:17:29.000000 prerogativityz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 11:19:17.501972 prerogativityz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 23:17:29.000000 prerogativityz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:19:17.497971 prerogativityz-2.1/prerogativityz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 23:17:29.000000 prerogativityz-2.1/prerogativityz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 23:17:29.000000 prerogativityz-2.1/prerogativityz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 11:19:17.501972 prerogativityz-2.1/prerogativityz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 11:19:17.000000 prerogativityz-2.1/prerogativityz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      275 2024-05-11 11:19:17.000000 prerogativityz-2.1/prerogativityz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 11:19:17.000000 prerogativityz-2.1/prerogativityz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 11:19:17.000000 prerogativityz-2.1/prerogativityz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       15 2024-05-11 11:19:17.000000 prerogativityz-2.1/prerogativityz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 11:19:17.501972 prerogativityz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-11 11:19:15.000000 prerogativityz-2.1/setup.py
```

### Comparing `prerogativityz-1.1/setup.py` & `prerogativityz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'prerogativityz',
     packages = ['prerogativityz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'prerogativityz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/prerogativityz',
```

