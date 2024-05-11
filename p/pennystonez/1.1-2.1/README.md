# Comparing `tmp/pennystonez-1.1.tar.gz` & `tmp/pennystonez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pennystonez-1.1.tar", last modified: Thu May  9 07:08:50 2024, max compression
+gzip compressed data, was "pennystonez-2.1.tar", last modified: Sat May 11 08:17:57 2024, max compression
```

## Comparing `pennystonez-1.1.tar` & `pennystonez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 07:08:50.902961 pennystonez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-09 07:08:50.902961 pennystonez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 07:08:50.902961 pennystonez-1.1/pennystonez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 07:08:50.706958 pennystonez-1.1/pennystonez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 07:08:50.714958 pennystonez-1.1/pennystonez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 07:08:50.706958 pennystonez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-09 07:08:50.726958 pennystonez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 08:17:57.093629 pennystonez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 07:08:50.000000 pennystonez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 08:17:57.093629 pennystonez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 07:08:50.000000 pennystonez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 08:17:57.093629 pennystonez-2.1/pennystonez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 07:08:50.000000 pennystonez-2.1/pennystonez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 07:08:50.000000 pennystonez-2.1/pennystonez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 08:17:57.093629 pennystonez-2.1/pennystonez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 08:17:56.000000 pennystonez-2.1/pennystonez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-11 08:17:56.000000 pennystonez-2.1/pennystonez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 08:17:56.000000 pennystonez-2.1/pennystonez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 08:17:56.000000 pennystonez-2.1/pennystonez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-11 08:17:56.000000 pennystonez-2.1/pennystonez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 08:17:57.093629 pennystonez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-11 08:17:56.000000 pennystonez-2.1/setup.py
```

### Comparing `pennystonez-1.1/setup.py` & `pennystonez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'pennystonez',
     packages = ['pennystonez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'pennystonez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/pennystonez',
```

