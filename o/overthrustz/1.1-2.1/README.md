# Comparing `tmp/overthrustz-1.1.tar.gz` & `tmp/overthrustz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overthrustz-1.1.tar", last modified: Thu May  9 23:50:16 2024, max compression
+gzip compressed data, was "overthrustz-2.1.tar", last modified: Sat May 11 07:46:43 2024, max compression
```

## Comparing `overthrustz-1.1.tar` & `overthrustz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 23:50:16.544837 overthrustz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1660 2024-05-09 23:50:16.544837 overthrustz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 23:50:16.544837 overthrustz-1.1/overthrustz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 23:50:12.320760 overthrustz-1.1/overthrustz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 23:50:12.524764 overthrustz-1.1/overthrustz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 23:50:12.320760 overthrustz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-09 23:50:12.872770 overthrustz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:46:43.115188 overthrustz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 23:50:12.000000 overthrustz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 07:46:43.115188 overthrustz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 23:50:12.000000 overthrustz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:46:43.115188 overthrustz-2.1/overthrustz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 23:50:12.000000 overthrustz-2.1/overthrustz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 23:50:12.000000 overthrustz-2.1/overthrustz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:46:43.115188 overthrustz-2.1/overthrustz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1940 2024-05-11 07:46:42.000000 overthrustz-2.1/overthrustz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      254 2024-05-11 07:46:43.000000 overthrustz-2.1/overthrustz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 07:46:42.000000 overthrustz-2.1/overthrustz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 07:46:42.000000 overthrustz-2.1/overthrustz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       12 2024-05-11 07:46:42.000000 overthrustz-2.1/overthrustz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 07:46:43.115188 overthrustz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1606 2024-05-11 07:46:42.000000 overthrustz-2.1/setup.py
```

### Comparing `overthrustz-1.1/setup.py` & `overthrustz-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'overthrustz',
     packages = ['overthrustz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'overthrustz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/overthrustz',
```

