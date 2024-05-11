# Comparing `tmp/ultz-1.1.tar.gz` & `tmp/ultz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultz-1.1.tar", last modified: Thu May  9 09:31:46 2024, max compression
+gzip compressed data, was "ultz-2.1.tar", last modified: Sat May 11 20:13:23 2024, max compression
```

## Comparing `ultz-1.1.tar` & `ultz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 09:31:46.672843 ultz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1632 2024-05-09 09:31:46.672843 ultz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 09:31:43.420783 ultz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1550 2024-05-09 09:31:43.916792 ultz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 09:31:46.672843 ultz-1.1/ultz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 09:31:43.420783 ultz-1.1/ultz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 09:31:43.592786 ultz-1.1/ultz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:13:23.752667 ultz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 09:31:43.000000 ultz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1891 2024-05-11 20:13:23.752667 ultz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 09:31:43.000000 ultz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 20:13:23.752667 ultz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1550 2024-05-11 20:13:23.000000 ultz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:13:23.720666 ultz-2.1/ultz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 09:31:43.000000 ultz-2.1/ultz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 09:31:43.000000 ultz-2.1/ultz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:13:23.720666 ultz-2.1/ultz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1891 2024-05-11 20:13:23.000000 ultz-2.1/ultz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      205 2024-05-11 20:13:23.000000 ultz-2.1/ultz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 20:13:23.000000 ultz-2.1/ultz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 20:13:23.000000 ultz-2.1/ultz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        5 2024-05-11 20:13:23.000000 ultz-2.1/ultz.egg-info/top_level.txt
```

### Comparing `ultz-1.1/setup.py` & `ultz-2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'ultz',
     packages = ['ultz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'ultz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/ultz',
```

