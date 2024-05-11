# Comparing `tmp/nuancesz-1.1.tar.gz` & `tmp/nuancesz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuancesz-1.1.tar", last modified: Fri May 10 01:41:43 2024, max compression
+gzip compressed data, was "nuancesz-2.1.tar", last modified: Sat May 11 06:34:07 2024, max compression
```

## Comparing `nuancesz-1.1.tar` & `nuancesz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 01:41:43.875948 nuancesz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1648 2024-05-10 01:41:43.875948 nuancesz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 01:41:43.875948 nuancesz-1.1/nuancesz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 01:41:40.951894 nuancesz-1.1/nuancesz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 01:41:41.107897 nuancesz-1.1/nuancesz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 01:41:40.951894 nuancesz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-10 01:41:41.343901 nuancesz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:34:07.738822 nuancesz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 01:41:40.000000 nuancesz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 06:34:07.738822 nuancesz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 01:41:40.000000 nuancesz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:34:07.738822 nuancesz-2.1/nuancesz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 01:41:40.000000 nuancesz-2.1/nuancesz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 01:41:41.000000 nuancesz-2.1/nuancesz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 06:34:07.738822 nuancesz-2.1/nuancesz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1919 2024-05-11 06:34:06.000000 nuancesz-2.1/nuancesz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      233 2024-05-11 06:34:06.000000 nuancesz-2.1/nuancesz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 06:34:06.000000 nuancesz-2.1/nuancesz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 06:34:06.000000 nuancesz-2.1/nuancesz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-11 06:34:06.000000 nuancesz-2.1/nuancesz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 06:34:07.738822 nuancesz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1582 2024-05-11 06:34:00.000000 nuancesz-2.1/setup.py
```

### Comparing `nuancesz-1.1/setup.py` & `nuancesz-2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'nuancesz',
     packages = ['nuancesz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'nuancesz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/nuancesz',
```

