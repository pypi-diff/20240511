# Comparing `tmp/tetanillaz-1.1.tar.gz` & `tmp/tetanillaz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tetanillaz-1.1.tar", last modified: Fri May 10 05:53:20 2024, max compression
+gzip compressed data, was "tetanillaz-2.1.tar", last modified: Sat May 11 18:39:44 2024, max compression
```

## Comparing `tetanillaz-1.1.tar` & `tetanillaz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 05:53:19.950266 tetanillaz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1656 2024-05-10 05:53:19.950266 tetanillaz-1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 05:53:14.294162 tetanillaz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-10 05:53:15.726189 tetanillaz-1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 05:53:19.950266 tetanillaz-1.1/tetanillaz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 05:53:14.294162 tetanillaz-1.1/tetanillaz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 05:53:14.598168 tetanillaz-1.1/tetanillaz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:39:44.509151 tetanillaz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 05:53:14.000000 tetanillaz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 18:39:44.509151 tetanillaz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 05:53:14.000000 tetanillaz-2.1/README.md
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 18:39:44.509151 tetanillaz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1598 2024-05-11 18:39:43.000000 tetanillaz-2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:39:44.505151 tetanillaz-2.1/tetanillaz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 05:53:14.000000 tetanillaz-2.1/tetanillaz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 05:53:14.000000 tetanillaz-2.1/tetanillaz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 18:39:44.509151 tetanillaz-2.1/tetanillaz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1933 2024-05-11 18:39:44.000000 tetanillaz-2.1/tetanillaz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      247 2024-05-11 18:39:44.000000 tetanillaz-2.1/tetanillaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 18:39:44.000000 tetanillaz-2.1/tetanillaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 18:39:44.000000 tetanillaz-2.1/tetanillaz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       11 2024-05-11 18:39:44.000000 tetanillaz-2.1/tetanillaz.egg-info/top_level.txt
```

### Comparing `tetanillaz-1.1/setup.py` & `tetanillaz-2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'tetanillaz',
     packages = ['tetanillaz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'tetanillaz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/tetanillaz',
```

