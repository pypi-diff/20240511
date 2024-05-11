# Comparing `tmp/docugenr8-0.0.7.tar.gz` & `tmp/docugenr8-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugenr8-0.0.7.tar", last modified: Fri May 10 20:48:04 2024, max compression
+gzip compressed data, was "docugenr8-0.0.8.tar", last modified: Sat May 11 14:21:28 2024, max compression
```

## Comparing `docugenr8-0.0.7.tar` & `docugenr8-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:48:04.775699 docugenr8-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-10 20:47:33.000000 docugenr8-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 20:48:04.775699 docugenr8-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 20:47:33.000000 docugenr8-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-10 20:47:33.000000 docugenr8-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:48:04.775699 docugenr8-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:48:04.771699 docugenr8-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:48:04.771699 docugenr8-0.0.7/src/docugenr8/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:47:33.000000 docugenr8-0.0.7/src/docugenr8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-05-10 20:47:33.000000 docugenr8-0.0.7/src/docugenr8/document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:48:04.775699 docugenr8-0.0.7/src/docugenr8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 20:48:04.000000 docugenr8-0.0.7/src/docugenr8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-10 20:48:04.000000 docugenr8-0.0.7/src/docugenr8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:48:04.000000 docugenr8-0.0.7/src/docugenr8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-10 20:48:04.000000 docugenr8-0.0.7/src/docugenr8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 20:48:04.000000 docugenr8-0.0.7/src/docugenr8.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:48:04.775699 docugenr8-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-10 20:47:33.000000 docugenr8-0.0.7/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 20:47:33.000000 docugenr8-0.0.7/version.txt
+drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:21:28.619546 docugenr8-0.0.8/
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)     1062 2024-05-09 18:57:23.000000 docugenr8-0.0.8/LICENSE
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)      861 2024-05-11 14:21:28.616557 docugenr8-0.0.8/PKG-INFO
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)       11 2024-05-09 18:54:52.000000 docugenr8-0.0.8/README.md
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)     1167 2024-05-11 13:55:22.000000 docugenr8-0.0.8/pyproject.toml
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)       38 2024-05-11 14:21:28.619546 docugenr8-0.0.8/setup.cfg
+drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:21:28.572039 docugenr8-0.0.8/src/
+drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:21:28.589991 docugenr8-0.0.8/src/docugenr8/
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-09 18:58:30.000000 docugenr8-0.0.8/src/docugenr8/__init__.py
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)     8220 2024-05-10 20:44:07.000000 docugenr8-0.0.8/src/docugenr8/document.py
+drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:21:28.612567 docugenr8-0.0.8/src/docugenr8.egg-info/
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)      861 2024-05-11 14:21:28.000000 docugenr8-0.0.8/src/docugenr8.egg-info/PKG-INFO
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)      299 2024-05-11 14:21:28.000000 docugenr8-0.0.8/src/docugenr8.egg-info/SOURCES.txt
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        1 2024-05-11 14:21:28.000000 docugenr8-0.0.8/src/docugenr8.egg-info/dependency_links.txt
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)      173 2024-05-11 14:21:28.000000 docugenr8-0.0.8/src/docugenr8.egg-info/requires.txt
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)       10 2024-05-11 14:21:28.000000 docugenr8-0.0.8/src/docugenr8.egg-info/top_level.txt
+drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:21:28.609573 docugenr8-0.0.8/tests/
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)     1864 2024-05-10 19:41:32.000000 docugenr8-0.0.8/tests/test_init.py
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        6 2024-05-11 14:16:53.000000 docugenr8-0.0.8/version.txt
```

### Comparing `docugenr8-0.0.7/LICENSE` & `docugenr8-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.7/PKG-INFO` & `docugenr8-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library for document creating
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docugenr8-0.0.7/pyproject.toml` & `docugenr8-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.7/src/docugenr8/document.py` & `docugenr8-0.0.8/src/docugenr8/document.py`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.7/src/docugenr8.egg-info/PKG-INFO` & `docugenr8-0.0.8/src/docugenr8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library for document creating
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docugenr8-0.0.7/tests/test_init.py` & `docugenr8-0.0.8/tests/test_init.py`

 * *Files identical despite different names*

