# Comparing `tmp/outkillz-1.1.tar.gz` & `tmp/outkillz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outkillz-1.1.tar", last modified: Fri May 10 00:40:10 2024, max compression
+gzip compressed data, was "outkillz-2.1.tar", last modified: Sat May 11 07:21:04 2024, max compression
```

## Comparing `outkillz-1.1.tar` & `outkillz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 00:40:09.979867 outkillz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-10 00:40:09.979867 outkillz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 00:40:09.979867 outkillz-1.1/outkillz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 00:40:05.883791 outkillz-1.1/outkillz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 00:40:05.903792 outkillz-1.1/outkillz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 00:40:05.883791 outkillz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 00:40:06.131796 outkillz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:21:04.074981 outkillz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 00:40:05.000000 outkillz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 07:21:04.074981 outkillz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 00:40:05.000000 outkillz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:21:04.070981 outkillz-2.1/outkillz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 00:40:05.000000 outkillz-2.1/outkillz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 00:40:05.000000 outkillz-2.1/outkillz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:21:04.074981 outkillz-2.1/outkillz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 07:21:03.000000 outkillz-2.1/outkillz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-11 07:21:03.000000 outkillz-2.1/outkillz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 07:21:03.000000 outkillz-2.1/outkillz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 07:21:03.000000 outkillz-2.1/outkillz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-11 07:21:03.000000 outkillz-2.1/outkillz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 07:21:04.074981 outkillz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-11 07:21:03.000000 outkillz-2.1/setup.py
```

### Comparing `outkillz-1.1/setup.py` & `outkillz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'outkillz',
     packages = ['outkillz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'outkillz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/outkillz',
```

