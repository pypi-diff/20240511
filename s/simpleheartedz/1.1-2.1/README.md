# Comparing `tmp/simpleheartedz-1.1.tar.gz` & `tmp/simpleheartedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleheartedz-1.1.tar", last modified: Thu May  9 18:41:19 2024, max compression
+gzip compressed data, was "simpleheartedz-2.1.tar", last modified: Sat May 11 15:18:01 2024, max compression
```

## Comparing `simpleheartedz-1.1.tar` & `simpleheartedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 18:41:19.208032 simpleheartedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1672 2024-05-09 18:41:19.208032 simpleheartedz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 18:41:19.020029 simpleheartedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-09 18:41:19.040029 simpleheartedz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 18:41:19.208032 simpleheartedz-1.1/simpleheartedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 18:41:19.020029 simpleheartedz-1.1/simpleheartedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 18:41:19.028029 simpleheartedz-1.1/simpleheartedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:18:01.169576 simpleheartedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 18:41:19.000000 simpleheartedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 15:18:01.169576 simpleheartedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 18:41:19.000000 simpleheartedz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 15:18:01.173576 simpleheartedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-11 15:18:00.000000 simpleheartedz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:18:01.169576 simpleheartedz-2.1/simpleheartedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 18:41:19.000000 simpleheartedz-2.1/simpleheartedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 18:41:19.000000 simpleheartedz-2.1/simpleheartedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 15:18:01.169576 simpleheartedz-2.1/simpleheartedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 15:18:01.000000 simpleheartedz-2.1/simpleheartedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      275 2024-05-11 15:18:01.000000 simpleheartedz-2.1/simpleheartedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 15:18:01.000000 simpleheartedz-2.1/simpleheartedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 15:18:01.000000 simpleheartedz-2.1/simpleheartedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       15 2024-05-11 15:18:01.000000 simpleheartedz-2.1/simpleheartedz.egg-info/top_level.txt
```

### Comparing `simpleheartedz-1.1/setup.py` & `simpleheartedz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'simpleheartedz',
     packages = ['simpleheartedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'simpleheartedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/simpleheartedz',
```

