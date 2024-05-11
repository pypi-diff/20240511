# Comparing `tmp/taxpayersz-1.1.tar.gz` & `tmp/taxpayersz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taxpayersz-1.1.tar", last modified: Thu May  9 11:30:18 2024, max compression
+gzip compressed data, was "taxpayersz-2.1.tar", last modified: Sat May 11 18:24:25 2024, max compression
```

## Comparing `taxpayersz-1.1.tar` & `taxpayersz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 11:30:18.099738 taxpayersz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-09 11:30:18.099738 taxpayersz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 11:30:15.247686 taxpayersz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-09 11:30:15.707694 taxpayersz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 11:30:18.099738 taxpayersz-1.1/taxpayersz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 11:30:15.247686 taxpayersz-1.1/taxpayersz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 11:30:15.567692 taxpayersz-1.1/taxpayersz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:24:25.624210 taxpayersz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 11:30:15.000000 taxpayersz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 18:24:25.624210 taxpayersz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 11:30:15.000000 taxpayersz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 18:24:25.628210 taxpayersz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 18:24:18.000000 taxpayersz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:24:25.600209 taxpayersz-2.1/taxpayersz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 11:30:15.000000 taxpayersz-2.1/taxpayersz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 11:30:15.000000 taxpayersz-2.1/taxpayersz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:24:25.624210 taxpayersz-2.1/taxpayersz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 18:24:24.000000 taxpayersz-2.1/taxpayersz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 18:24:24.000000 taxpayersz-2.1/taxpayersz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 18:24:24.000000 taxpayersz-2.1/taxpayersz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 18:24:24.000000 taxpayersz-2.1/taxpayersz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 18:24:24.000000 taxpayersz-2.1/taxpayersz.egg-info/top_level.txt
```

### Comparing `taxpayersz-1.1/setup.py` & `taxpayersz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'taxpayersz',
     packages = ['taxpayersz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'taxpayersz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/taxpayersz',
```

