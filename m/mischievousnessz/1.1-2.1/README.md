# Comparing `tmp/mischievousnessz-1.1.tar.gz` & `tmp/mischievousnessz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mischievousnessz-1.1.tar", last modified: Thu May  9 07:42:38 2024, max compression
+gzip compressed data, was "mischievousnessz-2.1.tar", last modified: Sat May 11 04:41:05 2024, max compression
```

## Comparing `mischievousnessz-1.1.tar` & `mischievousnessz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 07:42:38.300176 mischievousnessz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1680 2024-05-09 07:42:38.300176 mischievousnessz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 07:42:38.300176 mischievousnessz-1.1/mischievousnessz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 07:42:34.908113 mischievousnessz-1.1/mischievousnessz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 07:42:35.156118 mischievousnessz-1.1/mischievousnessz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 07:42:34.908113 mischievousnessz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-09 07:42:35.484124 mischievousnessz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:41:05.494179 mischievousnessz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 07:42:34.000000 mischievousnessz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-11 04:41:05.494179 mischievousnessz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 07:42:34.000000 mischievousnessz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:41:05.494179 mischievousnessz-2.1/mischievousnessz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 07:42:34.000000 mischievousnessz-2.1/mischievousnessz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 07:42:35.000000 mischievousnessz-2.1/mischievousnessz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 04:41:05.494179 mischievousnessz-2.1/mischievousnessz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1975 2024-05-11 04:41:05.000000 mischievousnessz-2.1/mischievousnessz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      289 2024-05-11 04:41:05.000000 mischievousnessz-2.1/mischievousnessz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 04:41:05.000000 mischievousnessz-2.1/mischievousnessz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 04:41:05.000000 mischievousnessz-2.1/mischievousnessz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       17 2024-05-11 04:41:05.000000 mischievousnessz-2.1/mischievousnessz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 04:41:05.494179 mischievousnessz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1646 2024-05-11 04:41:04.000000 mischievousnessz-2.1/setup.py
```

### Comparing `mischievousnessz-1.1/setup.py` & `mischievousnessz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'mischievousnessz',
     packages = ['mischievousnessz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'mischievousnessz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/mischievousnessz',
```

