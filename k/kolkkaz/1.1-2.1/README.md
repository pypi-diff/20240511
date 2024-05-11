# Comparing `tmp/kolkkaz-1.1.tar.gz` & `tmp/kolkkaz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolkkaz-1.1.tar", last modified: Thu May  9 01:56:49 2024, max compression
+gzip compressed data, was "kolkkaz-2.1.tar", last modified: Sat May 11 01:33:27 2024, max compression
```

## Comparing `kolkkaz-1.1.tar` & `kolkkaz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:56:49.107147 kolkkaz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1644 2024-05-09 01:56:49.107147 kolkkaz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 01:56:49.107147 kolkkaz-1.1/kolkkaz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:56:48.915143 kolkkaz-1.1/kolkkaz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:56:48.931144 kolkkaz-1.1/kolkkaz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 01:56:48.915143 kolkkaz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-09 01:56:48.939144 kolkkaz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:33:27.703450 kolkkaz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 01:56:48.000000 kolkkaz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-11 01:33:27.703450 kolkkaz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 01:56:48.000000 kolkkaz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:33:27.703450 kolkkaz-2.1/kolkkaz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 01:56:48.000000 kolkkaz-2.1/kolkkaz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 01:56:48.000000 kolkkaz-2.1/kolkkaz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:33:27.703450 kolkkaz-2.1/kolkkaz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-11 01:33:27.000000 kolkkaz-2.1/kolkkaz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      226 2024-05-11 01:33:27.000000 kolkkaz-2.1/kolkkaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 01:33:27.000000 kolkkaz-2.1/kolkkaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 01:33:27.000000 kolkkaz-2.1/kolkkaz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-11 01:33:27.000000 kolkkaz-2.1/kolkkaz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 01:33:27.703450 kolkkaz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-11 01:33:27.000000 kolkkaz-2.1/setup.py
```

### Comparing `kolkkaz-1.1/setup.py` & `kolkkaz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'kolkkaz',
     packages = ['kolkkaz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'kolkkaz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/kolkkaz',
```

