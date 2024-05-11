# Comparing `tmp/symptomatologiesz-1.1.tar.gz` & `tmp/symptomatologiesz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symptomatologiesz-1.1.tar", last modified: Thu May  9 12:57:43 2024, max compression
+gzip compressed data, was "symptomatologiesz-2.1.tar", last modified: Sat May 11 17:53:28 2024, max compression
```

## Comparing `symptomatologiesz-1.1.tar` & `symptomatologiesz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 12:57:43.168786 symptomatologiesz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1684 2024-05-09 12:57:43.168786 symptomatologiesz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 12:57:42.992783 symptomatologiesz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-09 12:57:43.004783 symptomatologiesz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 12:57:43.168786 symptomatologiesz-1.1/symptomatologiesz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 12:57:42.992783 symptomatologiesz-1.1/symptomatologiesz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 12:57:43.000783 symptomatologiesz-1.1/symptomatologiesz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:53:28.414000 symptomatologiesz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 12:57:42.000000 symptomatologiesz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 17:53:28.414000 symptomatologiesz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 12:57:42.000000 symptomatologiesz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 17:53:28.414000 symptomatologiesz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1654 2024-05-11 17:53:27.000000 symptomatologiesz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:53:28.414000 symptomatologiesz-2.1/symptomatologiesz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 12:57:42.000000 symptomatologiesz-2.1/symptomatologiesz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 12:57:43.000000 symptomatologiesz-2.1/symptomatologiesz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 17:53:28.414000 symptomatologiesz-2.1/symptomatologiesz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1982 2024-05-11 17:53:28.000000 symptomatologiesz-2.1/symptomatologiesz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      296 2024-05-11 17:53:28.000000 symptomatologiesz-2.1/symptomatologiesz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 17:53:28.000000 symptomatologiesz-2.1/symptomatologiesz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 17:53:28.000000 symptomatologiesz-2.1/symptomatologiesz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       18 2024-05-11 17:53:28.000000 symptomatologiesz-2.1/symptomatologiesz.egg-info/top_level.txt
```

### Comparing `symptomatologiesz-1.1/setup.py` & `symptomatologiesz-2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'symptomatologiesz',
     packages = ['symptomatologiesz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'symptomatologiesz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/symptomatologiesz',
```

