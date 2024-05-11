# Comparing `tmp/polyspermousz-1.1.tar.gz` & `tmp/polyspermousz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyspermousz-1.1.tar", last modified: Wed May  8 19:13:16 2024, max compression
+gzip compressed data, was "polyspermousz-2.1.tar", last modified: Sat May 11 10:01:25 2024, max compression
```

## Comparing `polyspermousz-1.1.tar` & `polyspermousz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 19:13:16.857200 polyspermousz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-08 19:13:16.857200 polyspermousz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 19:13:16.857200 polyspermousz-1.1/polyspermousz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 19:13:15.153169 polyspermousz-1.1/polyspermousz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 19:13:15.165169 polyspermousz-1.1/polyspermousz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 19:13:15.153169 polyspermousz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-08 19:13:15.173169 polyspermousz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:01:25.067727 polyspermousz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 19:13:15.000000 polyspermousz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 10:01:25.067727 polyspermousz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 19:13:15.000000 polyspermousz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:01:25.063727 polyspermousz-2.1/polyspermousz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 19:13:15.000000 polyspermousz-2.1/polyspermousz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 19:13:15.000000 polyspermousz-2.1/polyspermousz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:01:25.067727 polyspermousz-2.1/polyspermousz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 10:01:24.000000 polyspermousz-2.1/polyspermousz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 10:01:24.000000 polyspermousz-2.1/polyspermousz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 10:01:24.000000 polyspermousz-2.1/polyspermousz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 10:01:24.000000 polyspermousz-2.1/polyspermousz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 10:01:24.000000 polyspermousz-2.1/polyspermousz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 10:01:25.067727 polyspermousz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 10:01:24.000000 polyspermousz-2.1/setup.py
```

### Comparing `polyspermousz-1.1/setup.py` & `polyspermousz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'polyspermousz',
     packages = ['polyspermousz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'polyspermousz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/polyspermousz',
```

