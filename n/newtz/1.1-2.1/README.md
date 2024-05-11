# Comparing `tmp/newtz-1.1.tar.gz` & `tmp/newtz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newtz-1.1.tar", last modified: Thu May  9 21:09:25 2024, max compression
+gzip compressed data, was "newtz-2.1.tar", last modified: Sat May 11 05:47:32 2024, max compression
```

## Comparing `newtz-1.1.tar` & `newtz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 21:09:25.274935 newtz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1636 2024-05-09 21:09:25.274935 newtz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 21:09:25.274935 newtz-1.1/newtz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 21:09:25.054931 newtz-1.1/newtz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 21:09:25.058931 newtz-1.1/newtz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 21:09:25.054931 newtz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1558 2024-05-09 21:09:25.066931 newtz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:47:32.475917 newtz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 21:09:25.000000 newtz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1898 2024-05-11 05:47:32.475917 newtz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 21:09:25.000000 newtz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:47:32.475917 newtz-2.1/newtz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 21:09:25.000000 newtz-2.1/newtz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 21:09:25.000000 newtz-2.1/newtz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:47:32.475917 newtz-2.1/newtz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1898 2024-05-11 05:47:32.000000 newtz-2.1/newtz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      212 2024-05-11 05:47:32.000000 newtz-2.1/newtz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 05:47:32.000000 newtz-2.1/newtz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 05:47:32.000000 newtz-2.1/newtz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        6 2024-05-11 05:47:32.000000 newtz-2.1/newtz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 05:47:32.475917 newtz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1558 2024-05-11 05:47:31.000000 newtz-2.1/setup.py
```

### Comparing `newtz-1.1/setup.py` & `newtz-2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'newtz',
     packages = ['newtz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'newtz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/newtz',
```

