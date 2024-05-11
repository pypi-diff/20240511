# Comparing `tmp/otiorhynchidaez-1.1.tar.gz` & `tmp/otiorhynchidaez-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otiorhynchidaez-1.1.tar", last modified: Thu May  9 00:01:50 2024, max compression
+gzip compressed data, was "otiorhynchidaez-2.1.tar", last modified: Sat May 11 07:15:52 2024, max compression
```

## Comparing `otiorhynchidaez-1.1.tar` & `otiorhynchidaez-2.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 00:01:50.791701 otiorhynchidaez-1.1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1676 2024-05-09 00:01:50.791701 otiorhynchidaez-1.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-09 00:01:50.791701 otiorhynchidaez-1.1/otiorhynchidaez/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 00:01:50.591697 otiorhynchidaez-1.1/otiorhynchidaez/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 00:01:50.599697 otiorhynchidaez-1.1/otiorhynchidaez/main.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       61 2024-05-09 00:01:50.591697 otiorhynchidaez-1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-09 00:01:50.603697 otiorhynchidaez-1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:15:52.089267 otiorhynchidaez-2.1/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1069 2024-05-09 00:01:50.000000 otiorhynchidaez-2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 07:15:52.089267 otiorhynchidaez-2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      767 2024-05-09 00:01:50.000000 otiorhynchidaez-2.1/README.md
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:15:52.089267 otiorhynchidaez-2.1/otiorhynchidaez/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       31 2024-05-09 00:01:50.000000 otiorhynchidaez-2.1/otiorhynchidaez/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       37 2024-05-09 00:01:50.000000 otiorhynchidaez-2.1/otiorhynchidaez/main.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-11 07:15:52.089267 otiorhynchidaez-2.1/otiorhynchidaez.egg-info/
+-rw-r--r--   0 ubuntu    (1001) ubuntu    (1001)     1968 2024-05-11 07:15:50.000000 otiorhynchidaez-2.1/otiorhynchidaez.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      282 2024-05-11 07:15:50.000000 otiorhynchidaez-2.1/otiorhynchidaez.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-11 07:15:50.000000 otiorhynchidaez-2.1/otiorhynchidaez.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       52 2024-05-11 07:15:50.000000 otiorhynchidaez-2.1/otiorhynchidaez.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       16 2024-05-11 07:15:50.000000 otiorhynchidaez-2.1/otiorhynchidaez.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       79 2024-05-11 07:15:52.089267 otiorhynchidaez-2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1638 2024-05-11 07:15:38.000000 otiorhynchidaez-2.1/setup.py
```

### Comparing `otiorhynchidaez-1.1/setup.py` & `otiorhynchidaez-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name = 'otiorhynchidaez',
     packages = ['otiorhynchidaez'],
-    version = '1.1',
+    version = '2.1',
     license='MIT',
     description = 'otiorhynchidaez',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = 'Mirukutea',
     author_email = 'tea@masrizky.com',
     url = 'https://github.com/mirukutea/otiorhynchidaez',
```

