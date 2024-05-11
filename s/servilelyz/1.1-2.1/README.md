# Comparing `tmp/servilelyz-1.1.tar.gz` & `tmp/servilelyz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servilelyz-1.1.tar", last modified: Fri May 10 02:56:52 2024, max compression
+gzip compressed data, was "servilelyz-2.1.tar", last modified: Sat May 11 14:51:41 2024, max compression
```

## Comparing `servilelyz-1.1.tar` & `servilelyz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 02:56:52.507048 servilelyz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-10 02:56:52.507048 servilelyz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 02:56:52.507048 servilelyz-1.1/servilelyz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 02:56:49.442991 servilelyz-1.1/servilelyz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 02:56:49.554993 servilelyz-1.1/servilelyz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 02:56:49.442991 servilelyz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 02:56:49.919000 servilelyz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:51:41.044480 servilelyz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 02:56:49.000000 servilelyz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 14:51:41.044480 servilelyz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 02:56:49.000000 servilelyz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:51:41.020479 servilelyz-2.1/servilelyz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 02:56:49.000000 servilelyz-2.1/servilelyz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 02:56:49.000000 servilelyz-2.1/servilelyz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:51:41.044480 servilelyz-2.1/servilelyz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 14:51:40.000000 servilelyz-2.1/servilelyz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 14:51:40.000000 servilelyz-2.1/servilelyz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 14:51:40.000000 servilelyz-2.1/servilelyz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 14:51:40.000000 servilelyz-2.1/servilelyz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 14:51:40.000000 servilelyz-2.1/servilelyz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 14:51:41.044480 servilelyz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 14:51:33.000000 servilelyz-2.1/setup.py
```

### Comparing `servilelyz-1.1/setup.py` & `servilelyz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'servilelyz',
     packages = ['servilelyz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'servilelyz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/servilelyz',
```

