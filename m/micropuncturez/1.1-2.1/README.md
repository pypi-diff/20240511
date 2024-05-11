# Comparing `tmp/micropuncturez-1.1.tar.gz` & `tmp/micropuncturez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropuncturez-1.1.tar", last modified: Thu May  9 17:48:01 2024, max compression
+gzip compressed data, was "micropuncturez-2.1.tar", last modified: Sat May 11 04:30:32 2024, max compression
```

## Comparing `micropuncturez-1.1.tar` & `micropuncturez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 17:48:01.853053 micropuncturez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1672 2024-05-09 17:48:01.853053 micropuncturez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 17:48:01.853053 micropuncturez-1.1/micropuncturez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 17:48:01.657049 micropuncturez-1.1/micropuncturez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 17:48:01.665049 micropuncturez-1.1/micropuncturez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 17:48:01.657049 micropuncturez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-09 17:48:01.673049 micropuncturez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:30:32.014670 micropuncturez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 17:48:01.000000 micropuncturez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 04:30:32.014670 micropuncturez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 17:48:01.000000 micropuncturez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:30:32.010671 micropuncturez-2.1/micropuncturez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 17:48:01.000000 micropuncturez-2.1/micropuncturez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 17:48:01.000000 micropuncturez-2.1/micropuncturez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:30:32.014670 micropuncturez-2.1/micropuncturez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1961 2024-05-11 04:30:31.000000 micropuncturez-2.1/micropuncturez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      275 2024-05-11 04:30:31.000000 micropuncturez-2.1/micropuncturez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 04:30:31.000000 micropuncturez-2.1/micropuncturez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 04:30:31.000000 micropuncturez-2.1/micropuncturez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       15 2024-05-11 04:30:31.000000 micropuncturez-2.1/micropuncturez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 04:30:32.014670 micropuncturez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1630 2024-05-11 04:30:31.000000 micropuncturez-2.1/setup.py
```

### Comparing `micropuncturez-1.1/setup.py` & `micropuncturez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'micropuncturez',
     packages = ['micropuncturez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'micropuncturez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/micropuncturez',
```

