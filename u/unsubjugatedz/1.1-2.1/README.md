# Comparing `tmp/unsubjugatedz-1.1.tar.gz` & `tmp/unsubjugatedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unsubjugatedz-1.1.tar", last modified: Thu May  9 04:11:53 2024, max compression
+gzip compressed data, was "unsubjugatedz-2.1.tar", last modified: Sat May 11 21:52:40 2024, max compression
```

## Comparing `unsubjugatedz-1.1.tar` & `unsubjugatedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 04:11:53.875579 unsubjugatedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-09 04:11:53.875579 unsubjugatedz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 04:11:53.667575 unsubjugatedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-09 04:11:53.687575 unsubjugatedz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 04:11:53.875579 unsubjugatedz-1.1/unsubjugatedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 04:11:53.667575 unsubjugatedz-1.1/unsubjugatedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 04:11:53.675575 unsubjugatedz-1.1/unsubjugatedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:52:40.082226 unsubjugatedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 04:11:53.000000 unsubjugatedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 21:52:40.082226 unsubjugatedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 04:11:53.000000 unsubjugatedz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 21:52:40.082226 unsubjugatedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 21:52:33.000000 unsubjugatedz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:52:40.038225 unsubjugatedz-2.1/unsubjugatedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 04:11:53.000000 unsubjugatedz-2.1/unsubjugatedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 04:11:53.000000 unsubjugatedz-2.1/unsubjugatedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 21:52:40.082226 unsubjugatedz-2.1/unsubjugatedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 21:52:39.000000 unsubjugatedz-2.1/unsubjugatedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 21:52:39.000000 unsubjugatedz-2.1/unsubjugatedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 21:52:39.000000 unsubjugatedz-2.1/unsubjugatedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 21:52:39.000000 unsubjugatedz-2.1/unsubjugatedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 21:52:39.000000 unsubjugatedz-2.1/unsubjugatedz.egg-info/top_level.txt
```

### Comparing `unsubjugatedz-1.1/setup.py` & `unsubjugatedz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'unsubjugatedz',
     packages = ['unsubjugatedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'unsubjugatedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/unsubjugatedz',
```

