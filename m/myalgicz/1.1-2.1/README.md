# Comparing `tmp/myalgicz-1.1.tar.gz` & `tmp/myalgicz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myalgicz-1.1.tar", last modified: Fri May 10 00:45:53 2024, max compression
+gzip compressed data, was "myalgicz-2.1.tar", last modified: Sat May 11 05:21:51 2024, max compression
```

## Comparing `myalgicz-1.1.tar` & `myalgicz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 00:45:53.078222 myalgicz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-10 00:45:53.078222 myalgicz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 00:45:53.078222 myalgicz-1.1/myalgicz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 00:45:49.954164 myalgicz-1.1/myalgicz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 00:45:50.250169 myalgicz-1.1/myalgicz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 00:45:49.954164 myalgicz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 00:45:50.606176 myalgicz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:21:51.071426 myalgicz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 00:45:49.000000 myalgicz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 05:21:51.071426 myalgicz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 00:45:49.000000 myalgicz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:21:51.071426 myalgicz-2.1/myalgicz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 00:45:49.000000 myalgicz-2.1/myalgicz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 00:45:50.000000 myalgicz-2.1/myalgicz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 05:21:51.071426 myalgicz-2.1/myalgicz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 05:21:50.000000 myalgicz-2.1/myalgicz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-11 05:21:50.000000 myalgicz-2.1/myalgicz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 05:21:50.000000 myalgicz-2.1/myalgicz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 05:21:50.000000 myalgicz-2.1/myalgicz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-11 05:21:50.000000 myalgicz-2.1/myalgicz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 05:21:51.071426 myalgicz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-11 05:21:50.000000 myalgicz-2.1/setup.py
```

### Comparing `myalgicz-1.1/setup.py` & `myalgicz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'myalgicz',
     packages = ['myalgicz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'myalgicz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/myalgicz',
```

