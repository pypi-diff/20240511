# Comparing `tmp/subjugatingz-1.1.tar.gz` & `tmp/subjugatingz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subjugatingz-1.1.tar", last modified: Thu May  9 18:08:58 2024, max compression
+gzip compressed data, was "subjugatingz-2.1.tar", last modified: Sat May 11 17:06:26 2024, max compression
```

## Comparing `subjugatingz-1.1.tar` & `subjugatingz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 18:08:58.864035 subjugatingz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1664 2024-05-09 18:08:58.864035 subjugatingz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 18:08:58.676032 subjugatingz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-09 18:08:58.696032 subjugatingz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 18:08:58.864035 subjugatingz-1.1/subjugatingz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 18:08:58.676032 subjugatingz-1.1/subjugatingz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 18:08:58.684032 subjugatingz-1.1/subjugatingz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:06:26.197910 subjugatingz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 18:08:58.000000 subjugatingz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 17:06:26.197910 subjugatingz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 18:08:58.000000 subjugatingz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 17:06:26.197910 subjugatingz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1614 2024-05-11 17:06:25.000000 subjugatingz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:06:26.193910 subjugatingz-2.1/subjugatingz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 18:08:58.000000 subjugatingz-2.1/subjugatingz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 18:08:58.000000 subjugatingz-2.1/subjugatingz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:06:26.197910 subjugatingz-2.1/subjugatingz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2024-05-11 17:06:26.000000 subjugatingz-2.1/subjugatingz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-11 17:06:26.000000 subjugatingz-2.1/subjugatingz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 17:06:26.000000 subjugatingz-2.1/subjugatingz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 17:06:26.000000 subjugatingz-2.1/subjugatingz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       13 2024-05-11 17:06:26.000000 subjugatingz-2.1/subjugatingz.egg-info/top_level.txt
```

### Comparing `subjugatingz-1.1/setup.py` & `subjugatingz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'subjugatingz',
     packages = ['subjugatingz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'subjugatingz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/subjugatingz',
```

