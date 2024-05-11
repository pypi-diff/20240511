# Comparing `tmp/recentnessz-1.1.tar.gz` & `tmp/recentnessz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recentnessz-1.1.tar", last modified: Thu May  9 10:31:29 2024, max compression
+gzip compressed data, was "recentnessz-2.1.tar", last modified: Sat May 11 13:12:53 2024, max compression
```

## Comparing `recentnessz-1.1.tar` & `recentnessz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 10:31:29.674810 recentnessz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-09 10:31:29.674810 recentnessz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 10:31:29.674810 recentnessz-1.1/recentnessz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 10:31:27.506770 recentnessz-1.1/recentnessz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 10:31:27.718774 recentnessz-1.1/recentnessz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 10:31:27.506770 recentnessz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-09 10:31:28.094781 recentnessz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 13:12:53.847136 recentnessz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 10:31:27.000000 recentnessz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 13:12:53.847136 recentnessz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 10:31:27.000000 recentnessz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 13:12:53.847136 recentnessz-2.1/recentnessz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 10:31:27.000000 recentnessz-2.1/recentnessz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 10:31:27.000000 recentnessz-2.1/recentnessz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 13:12:53.847136 recentnessz-2.1/recentnessz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 13:12:53.000000 recentnessz-2.1/recentnessz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-11 13:12:53.000000 recentnessz-2.1/recentnessz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 13:12:53.000000 recentnessz-2.1/recentnessz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 13:12:53.000000 recentnessz-2.1/recentnessz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-11 13:12:53.000000 recentnessz-2.1/recentnessz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 13:12:53.847136 recentnessz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-11 13:12:49.000000 recentnessz-2.1/setup.py
```

### Comparing `recentnessz-1.1/setup.py` & `recentnessz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'recentnessz',
     packages = ['recentnessz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'recentnessz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/recentnessz',
```

