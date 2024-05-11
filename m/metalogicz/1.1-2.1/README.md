# Comparing `tmp/metalogicz-1.1.tar.gz` & `tmp/metalogicz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalogicz-1.1.tar", last modified: Thu May  9 10:20:47 2024, max compression
+gzip compressed data, was "metalogicz-2.1.tar", last modified: Sat May 11 04:14:53 2024, max compression
```

## Comparing `metalogicz-1.1.tar` & `metalogicz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 10:20:47.163010 metalogicz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 10:20:47.163010 metalogicz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 10:20:47.163010 metalogicz-1.1/metalogicz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 10:20:46.995007 metalogicz-1.1/metalogicz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 10:20:47.003007 metalogicz-1.1/metalogicz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 10:20:46.995007 metalogicz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 10:20:47.011007 metalogicz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:14:53.609492 metalogicz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 10:20:46.000000 metalogicz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 04:14:53.609492 metalogicz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 10:20:46.000000 metalogicz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:14:53.609492 metalogicz-2.1/metalogicz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 10:20:46.000000 metalogicz-2.1/metalogicz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 10:20:47.000000 metalogicz-2.1/metalogicz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:14:53.609492 metalogicz-2.1/metalogicz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 04:14:53.000000 metalogicz-2.1/metalogicz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 04:14:53.000000 metalogicz-2.1/metalogicz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 04:14:53.000000 metalogicz-2.1/metalogicz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 04:14:53.000000 metalogicz-2.1/metalogicz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 04:14:53.000000 metalogicz-2.1/metalogicz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 04:14:53.609492 metalogicz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 04:14:53.000000 metalogicz-2.1/setup.py
```

### Comparing `metalogicz-1.1/setup.py` & `metalogicz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'metalogicz',
     packages = ['metalogicz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'metalogicz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/metalogicz',
```

