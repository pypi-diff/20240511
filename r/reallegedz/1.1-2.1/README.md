# Comparing `tmp/reallegedz-1.1.tar.gz` & `tmp/reallegedz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reallegedz-1.1.tar", last modified: Fri May 10 02:03:20 2024, max compression
+gzip compressed data, was "reallegedz-2.1.tar", last modified: Sat May 11 12:57:34 2024, max compression
```

## Comparing `reallegedz-1.1.tar` & `reallegedz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 02:03:20.587781 reallegedz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-10 02:03:20.587781 reallegedz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 02:03:20.587781 reallegedz-1.1/reallegedz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 02:03:20.407778 reallegedz-1.1/reallegedz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 02:03:20.415778 reallegedz-1.1/reallegedz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 02:03:20.407778 reallegedz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 02:03:20.423778 reallegedz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 12:57:34.682536 reallegedz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 02:03:20.000000 reallegedz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 12:57:34.682536 reallegedz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 02:03:20.000000 reallegedz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 12:57:34.682536 reallegedz-2.1/reallegedz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 02:03:20.000000 reallegedz-2.1/reallegedz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 02:03:20.000000 reallegedz-2.1/reallegedz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 12:57:34.682536 reallegedz-2.1/reallegedz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 12:57:34.000000 reallegedz-2.1/reallegedz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 12:57:34.000000 reallegedz-2.1/reallegedz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 12:57:34.000000 reallegedz-2.1/reallegedz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 12:57:34.000000 reallegedz-2.1/reallegedz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 12:57:34.000000 reallegedz-2.1/reallegedz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 12:57:34.682536 reallegedz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 12:57:34.000000 reallegedz-2.1/setup.py
```

### Comparing `reallegedz-1.1/setup.py` & `reallegedz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'reallegedz',
     packages = ['reallegedz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'reallegedz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/reallegedz',
```

