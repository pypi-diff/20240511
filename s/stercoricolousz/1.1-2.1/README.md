# Comparing `tmp/stercoricolousz-1.1.tar.gz` & `tmp/stercoricolousz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stercoricolousz-1.1.tar", last modified: Thu May  9 19:20:04 2024, max compression
+gzip compressed data, was "stercoricolousz-2.1.tar", last modified: Sat May 11 16:25:13 2024, max compression
```

## Comparing `stercoricolousz-1.1.tar` & `stercoricolousz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 19:20:04.859171 stercoricolousz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1676 2024-05-09 19:20:04.859171 stercoricolousz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 19:20:01.507109 stercoricolousz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-09 19:20:01.975118 stercoricolousz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 19:20:04.859171 stercoricolousz-1.1/stercoricolousz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 19:20:01.507109 stercoricolousz-1.1/stercoricolousz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 19:20:01.675112 stercoricolousz-1.1/stercoricolousz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:25:13.372599 stercoricolousz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 19:20:01.000000 stercoricolousz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 16:25:13.372599 stercoricolousz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 19:20:01.000000 stercoricolousz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 16:25:13.372599 stercoricolousz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-11 16:25:12.000000 stercoricolousz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:25:13.368599 stercoricolousz-2.1/stercoricolousz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 19:20:01.000000 stercoricolousz-2.1/stercoricolousz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 19:20:01.000000 stercoricolousz-2.1/stercoricolousz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 16:25:13.372599 stercoricolousz-2.1/stercoricolousz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 16:25:13.000000 stercoricolousz-2.1/stercoricolousz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      282 2024-05-11 16:25:13.000000 stercoricolousz-2.1/stercoricolousz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 16:25:13.000000 stercoricolousz-2.1/stercoricolousz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 16:25:13.000000 stercoricolousz-2.1/stercoricolousz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       16 2024-05-11 16:25:13.000000 stercoricolousz-2.1/stercoricolousz.egg-info/top_level.txt
```

### Comparing `stercoricolousz-1.1/setup.py` & `stercoricolousz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'stercoricolousz',
     packages = ['stercoricolousz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'stercoricolousz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/stercoricolousz',
```

