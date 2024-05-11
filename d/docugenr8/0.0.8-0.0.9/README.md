# Comparing `tmp/docugenr8-0.0.8.tar.gz` & `tmp/docugenr8-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugenr8-0.0.8.tar", last modified: Sat May 11 14:21:28 2024, max compression
+gzip compressed data, was "docugenr8-0.0.9.tar", last modified: Sat May 11 14:28:46 2024, max compression
```

## Comparing `docugenr8-0.0.8.tar` & `docugenr8-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:21:28.619546 docugenr8-0.0.8/
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)     1062 2024-05-09 18:57:23.000000 docugenr8-0.0.8/LICENSE
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)      861 2024-05-11 14:21:28.616557 docugenr8-0.0.8/PKG-INFO
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)       11 2024-05-09 18:54:52.000000 docugenr8-0.0.8/README.md
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)     1167 2024-05-11 13:55:22.000000 docugenr8-0.0.8/pyproject.toml
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)       38 2024-05-11 14:21:28.619546 docugenr8-0.0.8/setup.cfg
-drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:21:28.572039 docugenr8-0.0.8/src/
-drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:21:28.589991 docugenr8-0.0.8/src/docugenr8/
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-09 18:58:30.000000 docugenr8-0.0.8/src/docugenr8/__init__.py
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)     8220 2024-05-10 20:44:07.000000 docugenr8-0.0.8/src/docugenr8/document.py
-drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:21:28.612567 docugenr8-0.0.8/src/docugenr8.egg-info/
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)      861 2024-05-11 14:21:28.000000 docugenr8-0.0.8/src/docugenr8.egg-info/PKG-INFO
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)      299 2024-05-11 14:21:28.000000 docugenr8-0.0.8/src/docugenr8.egg-info/SOURCES.txt
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        1 2024-05-11 14:21:28.000000 docugenr8-0.0.8/src/docugenr8.egg-info/dependency_links.txt
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)      173 2024-05-11 14:21:28.000000 docugenr8-0.0.8/src/docugenr8.egg-info/requires.txt
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)       10 2024-05-11 14:21:28.000000 docugenr8-0.0.8/src/docugenr8.egg-info/top_level.txt
-drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:21:28.609573 docugenr8-0.0.8/tests/
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)     1864 2024-05-10 19:41:32.000000 docugenr8-0.0.8/tests/test_init.py
--rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        6 2024-05-11 14:16:53.000000 docugenr8-0.0.8/version.txt
+drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:28:46.948045 docugenr8-0.0.9/
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)     1062 2024-05-09 18:57:23.000000 docugenr8-0.0.9/LICENSE
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)      861 2024-05-11 14:28:46.945053 docugenr8-0.0.9/PKG-INFO
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)       11 2024-05-09 18:54:52.000000 docugenr8-0.0.9/README.md
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)     1167 2024-05-11 13:55:22.000000 docugenr8-0.0.9/pyproject.toml
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)       38 2024-05-11 14:28:46.948045 docugenr8-0.0.9/setup.cfg
+drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:28:46.898663 docugenr8-0.0.9/src/
+drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:28:46.915135 docugenr8-0.0.9/src/docugenr8/
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-09 18:58:30.000000 docugenr8-0.0.9/src/docugenr8/__init__.py
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)     8220 2024-05-10 20:44:07.000000 docugenr8-0.0.9/src/docugenr8/document.py
+drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:28:46.939068 docugenr8-0.0.9/src/docugenr8.egg-info/
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)      861 2024-05-11 14:28:46.000000 docugenr8-0.0.9/src/docugenr8.egg-info/PKG-INFO
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)      299 2024-05-11 14:28:46.000000 docugenr8-0.0.9/src/docugenr8.egg-info/SOURCES.txt
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        1 2024-05-11 14:28:46.000000 docugenr8-0.0.9/src/docugenr8.egg-info/dependency_links.txt
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)      173 2024-05-11 14:28:46.000000 docugenr8-0.0.9/src/docugenr8.egg-info/requires.txt
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)       10 2024-05-11 14:28:46.000000 docugenr8-0.0.9/src/docugenr8.egg-info/top_level.txt
+drwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        0 2024-05-11 14:28:46.935079 docugenr8-0.0.9/tests/
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)     1864 2024-05-10 19:41:32.000000 docugenr8-0.0.9/tests/test_init.py
+-rwxrwxrwx   0 vladimirjo  (1000) vladimirjo  (1000)        6 2024-05-11 14:28:37.000000 docugenr8-0.0.9/version.txt
```

### Comparing `docugenr8-0.0.8/LICENSE` & `docugenr8-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.8/PKG-INFO` & `docugenr8-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for document creating
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docugenr8-0.0.8/pyproject.toml` & `docugenr8-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.8/src/docugenr8/document.py` & `docugenr8-0.0.9/src/docugenr8/document.py`

 * *Files identical despite different names*

### Comparing `docugenr8-0.0.8/src/docugenr8.egg-info/PKG-INFO` & `docugenr8-0.0.9/src/docugenr8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for document creating
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `docugenr8-0.0.8/tests/test_init.py` & `docugenr8-0.0.9/tests/test_init.py`

 * *Files identical despite different names*

