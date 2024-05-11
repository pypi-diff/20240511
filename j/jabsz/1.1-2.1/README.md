# Comparing `tmp/jabsz-1.1.tar.gz` & `tmp/jabsz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jabsz-1.1.tar", last modified: Thu May  9 07:53:57 2024, max compression
+gzip compressed data, was "jabsz-2.1.tar", last modified: Sat May 11 00:56:57 2024, max compression
```

## Comparing `jabsz-1.1.tar` & `jabsz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 07:53:57.620655 jabsz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1636 2024-05-09 07:53:57.620655 jabsz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 07:53:57.620655 jabsz-1.1/jabsz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 07:53:55.068609 jabsz-1.1/jabsz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 07:53:55.296613 jabsz-1.1/jabsz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 07:53:55.068609 jabsz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1558 2024-05-09 07:53:55.572618 jabsz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:56:57.535167 jabsz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 07:53:55.000000 jabsz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1898 2024-05-11 00:56:57.535167 jabsz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 07:53:55.000000 jabsz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:56:57.531166 jabsz-2.1/jabsz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 07:53:55.000000 jabsz-2.1/jabsz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 07:53:55.000000 jabsz-2.1/jabsz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:56:57.531166 jabsz-2.1/jabsz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1898 2024-05-11 00:56:56.000000 jabsz-2.1/jabsz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      212 2024-05-11 00:56:56.000000 jabsz-2.1/jabsz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 00:56:56.000000 jabsz-2.1/jabsz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 00:56:56.000000 jabsz-2.1/jabsz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        6 2024-05-11 00:56:56.000000 jabsz-2.1/jabsz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 00:56:57.535167 jabsz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1558 2024-05-11 00:56:51.000000 jabsz-2.1/setup.py
```

### Comparing `jabsz-1.1/setup.py` & `jabsz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'jabsz',
     packages = ['jabsz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'jabsz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/jabsz',
```

