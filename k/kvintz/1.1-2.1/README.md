# Comparing `tmp/kvintz-1.1.tar.gz` & `tmp/kvintz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvintz-1.1.tar", last modified: Thu May  9 05:29:02 2024, max compression
+gzip compressed data, was "kvintz-2.1.tar", last modified: Sat May 11 01:38:38 2024, max compression
```

## Comparing `kvintz-1.1.tar` & `kvintz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:29:02.784760 kvintz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1640 2024-05-09 05:29:02.784760 kvintz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 05:29:02.784760 kvintz-1.1/kvintz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:28:59.988709 kvintz-1.1/kvintz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:29:00.084710 kvintz-1.1/kvintz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 05:28:59.988709 kvintz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1566 2024-05-09 05:29:00.376716 kvintz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:38:37.981158 kvintz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 05:28:59.000000 kvintz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1905 2024-05-11 01:38:37.981158 kvintz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 05:28:59.000000 kvintz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:38:37.981158 kvintz-2.1/kvintz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 05:28:59.000000 kvintz-2.1/kvintz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 05:29:00.000000 kvintz-2.1/kvintz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 01:38:37.981158 kvintz-2.1/kvintz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1905 2024-05-11 01:38:37.000000 kvintz-2.1/kvintz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      219 2024-05-11 01:38:37.000000 kvintz-2.1/kvintz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 01:38:37.000000 kvintz-2.1/kvintz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 01:38:37.000000 kvintz-2.1/kvintz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        7 2024-05-11 01:38:37.000000 kvintz-2.1/kvintz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 01:38:37.981158 kvintz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1566 2024-05-11 01:38:32.000000 kvintz-2.1/setup.py
```

### Comparing `kvintz-1.1/setup.py` & `kvintz-2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'kvintz',
     packages = ['kvintz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'kvintz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/kvintz',
```

