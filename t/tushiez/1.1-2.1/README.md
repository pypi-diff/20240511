# Comparing `tmp/tushiez-1.1.tar.gz` & `tmp/tushiez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tushiez-1.1.tar", last modified: Fri May 10 05:58:34 2024, max compression
+gzip compressed data, was "tushiez-2.1.tar", last modified: Sat May 11 20:03:03 2024, max compression
```

## Comparing `tushiez-1.1.tar` & `tushiez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 05:58:34.004058 tushiez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1644 2024-05-10 05:58:34.004058 tushiez-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 05:58:33.812055 tushiez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-10 05:58:33.824055 tushiez-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 05:58:34.004058 tushiez-1.1/tushiez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 05:58:33.812055 tushiez-1.1/tushiez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 05:58:33.820055 tushiez-1.1/tushiez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:03:03.361248 tushiez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 05:58:33.000000 tushiez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-11 20:03:03.361248 tushiez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 05:58:33.000000 tushiez-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 20:03:03.361248 tushiez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1574 2024-05-11 20:03:02.000000 tushiez-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:03:03.361248 tushiez-2.1/tushiez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 05:58:33.000000 tushiez-2.1/tushiez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 05:58:33.000000 tushiez-2.1/tushiez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 20:03:03.361248 tushiez-2.1/tushiez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1912 2024-05-11 20:03:03.000000 tushiez-2.1/tushiez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      226 2024-05-11 20:03:03.000000 tushiez-2.1/tushiez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 20:03:03.000000 tushiez-2.1/tushiez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 20:03:03.000000 tushiez-2.1/tushiez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-11 20:03:03.000000 tushiez-2.1/tushiez.egg-info/top_level.txt
```

### Comparing `tushiez-1.1/setup.py` & `tushiez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'tushiez',
     packages = ['tushiez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'tushiez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/tushiez',
```

