# Comparing `tmp/lirellinez-1.1.tar.gz` & `tmp/lirellinez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lirellinez-1.1.tar", last modified: Thu May  9 19:08:50 2024, max compression
+gzip compressed data, was "lirellinez-2.1.tar", last modified: Sat May 11 02:41:08 2024, max compression
```

## Comparing `lirellinez-1.1.tar` & `lirellinez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 19:08:50.862693 lirellinez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 19:08:50.862693 lirellinez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 19:08:50.862693 lirellinez-1.1/lirellinez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 19:08:50.682690 lirellinez-1.1/lirellinez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 19:08:50.690690 lirellinez-1.1/lirellinez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 19:08:50.682690 lirellinez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 19:08:50.698690 lirellinez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 02:41:08.258168 lirellinez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 19:08:50.000000 lirellinez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 02:41:08.258168 lirellinez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 19:08:50.000000 lirellinez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 02:41:08.254168 lirellinez-2.1/lirellinez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 19:08:50.000000 lirellinez-2.1/lirellinez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 19:08:50.000000 lirellinez-2.1/lirellinez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 02:41:08.254168 lirellinez-2.1/lirellinez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 02:41:08.000000 lirellinez-2.1/lirellinez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 02:41:08.000000 lirellinez-2.1/lirellinez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 02:41:08.000000 lirellinez-2.1/lirellinez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 02:41:08.000000 lirellinez-2.1/lirellinez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 02:41:08.000000 lirellinez-2.1/lirellinez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 02:41:08.258168 lirellinez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 02:41:07.000000 lirellinez-2.1/setup.py
```

### Comparing `lirellinez-1.1/setup.py` & `lirellinez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'lirellinez',
     packages = ['lirellinez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'lirellinez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/lirellinez',
```

