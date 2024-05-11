# Comparing `tmp/scolopendridz-1.1.tar.gz` & `tmp/scolopendridz-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scolopendridz-1.1.tar", last modified: Fri May 10 05:31:25 2024, max compression
+gzip compressed data, was "scolopendridz-2.1.tar", last modified: Sat May 11 14:36:00 2024, max compression
```

## Comparing `scolopendridz-1.1.tar` & `scolopendridz-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 05:31:25.986034 scolopendridz-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1668 2024-05-10 05:31:25.986034 scolopendridz-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-10 05:31:25.986034 scolopendridz-1.1/scolopendridz/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 05:31:25.802030 scolopendridz-1.1/scolopendridz/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 05:31:25.810031 scolopendridz-1.1/scolopendridz/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-10 05:31:25.802030 scolopendridz-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-10 05:31:25.818031 scolopendridz-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:36:00.415209 scolopendridz-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-10 05:31:25.000000 scolopendridz-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 14:36:00.415209 scolopendridz-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-10 05:31:25.000000 scolopendridz-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:36:00.415209 scolopendridz-2.1/scolopendridz/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-10 05:31:25.000000 scolopendridz-2.1/scolopendridz/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-10 05:31:25.000000 scolopendridz-2.1/scolopendridz/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 14:36:00.415209 scolopendridz-2.1/scolopendridz.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1954 2024-05-11 14:36:00.000000 scolopendridz-2.1/scolopendridz.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      268 2024-05-11 14:36:00.000000 scolopendridz-2.1/scolopendridz.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 14:36:00.000000 scolopendridz-2.1/scolopendridz.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 14:36:00.000000 scolopendridz-2.1/scolopendridz.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       14 2024-05-11 14:36:00.000000 scolopendridz-2.1/scolopendridz.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 14:36:00.415209 scolopendridz-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1622 2024-05-11 14:35:59.000000 scolopendridz-2.1/setup.py
```

### Comparing `scolopendridz-1.1/setup.py` & `scolopendridz-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'scolopendridz',
     packages = ['scolopendridz'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'scolopendridz',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/scolopendridz',
```

