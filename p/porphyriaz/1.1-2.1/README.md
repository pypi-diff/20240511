# Comparing `tmp/porphyriaz-1.1.tar.gz` & `tmp/porphyriaz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "porphyriaz-1.1.tar", last modified: Fri May 10 05:26:08 2024, max compression
+gzip compressed data, was "porphyriaz-2.1.tar", last modified: Sat May 11 10:06:28 2024, max compression
```

## Comparing `porphyriaz-1.1.tar` & `porphyriaz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 05:26:08.836185 porphyriaz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-10 05:26:08.836185 porphyriaz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 05:26:08.836185 porphyriaz-1.1/porphyriaz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 05:26:05.636126 porphyriaz-1.1/porphyriaz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 05:26:05.940132 porphyriaz-1.1/porphyriaz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 05:26:05.636126 porphyriaz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 05:26:06.200136 porphyriaz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:06:28.585306 porphyriaz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 05:26:05.000000 porphyriaz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 10:06:28.585306 porphyriaz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 05:26:05.000000 porphyriaz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:06:28.581306 porphyriaz-2.1/porphyriaz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 05:26:05.000000 porphyriaz-2.1/porphyriaz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 05:26:05.000000 porphyriaz-2.1/porphyriaz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 10:06:28.585306 porphyriaz-2.1/porphyriaz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 10:06:28.000000 porphyriaz-2.1/porphyriaz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 10:06:28.000000 porphyriaz-2.1/porphyriaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 10:06:28.000000 porphyriaz-2.1/porphyriaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 10:06:28.000000 porphyriaz-2.1/porphyriaz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 10:06:28.000000 porphyriaz-2.1/porphyriaz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 10:06:28.585306 porphyriaz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 10:06:28.000000 porphyriaz-2.1/setup.py
```

### Comparing `porphyriaz-1.1/setup.py` & `porphyriaz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'porphyriaz',
     packages = ['porphyriaz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'porphyriaz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/porphyriaz',
```
