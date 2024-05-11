# Comparing `tmp/innuendoedz-1.1.tar.gz` & `tmp/innuendoedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innuendoedz-1.1.tar", last modified: Wed May  8 17:19:47 2024, max compression
+gzip compressed data, was "innuendoedz-2.1.tar", last modified: Sat May 11 00:15:30 2024, max compression
```

## Comparing `innuendoedz-1.1.tar` & `innuendoedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 17:19:46.936005 innuendoedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-08 17:19:46.936005 innuendoedz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-08 17:19:46.936005 innuendoedz-1.1/innuendoedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 17:19:43.695947 innuendoedz-1.1/innuendoedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 17:19:43.835949 innuendoedz-1.1/innuendoedz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-08 17:19:43.695947 innuendoedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-08 17:19:44.363959 innuendoedz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:15:30.481277 innuendoedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-08 17:19:43.000000 innuendoedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 00:15:30.481277 innuendoedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-08 17:19:43.000000 innuendoedz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:15:30.481277 innuendoedz-2.1/innuendoedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-08 17:19:43.000000 innuendoedz-2.1/innuendoedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-08 17:19:43.000000 innuendoedz-2.1/innuendoedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 00:15:30.481277 innuendoedz-2.1/innuendoedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 00:15:30.000000 innuendoedz-2.1/innuendoedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-11 00:15:30.000000 innuendoedz-2.1/innuendoedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 00:15:30.000000 innuendoedz-2.1/innuendoedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 00:15:30.000000 innuendoedz-2.1/innuendoedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-11 00:15:30.000000 innuendoedz-2.1/innuendoedz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 00:15:30.481277 innuendoedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-11 00:15:29.000000 innuendoedz-2.1/setup.py
```

### Comparing `innuendoedz-1.1/setup.py` & `innuendoedz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'innuendoedz',
     packages = ['innuendoedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'innuendoedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/innuendoedz',
```

