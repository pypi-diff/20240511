# Comparing `tmp/pddl_embeddings-0.0.1.dev1.tar.gz` & `tmp/pddl_embeddings-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pddl_embeddings-0.0.1.dev1.tar", last modified: Tue Apr 30 18:37:43 2024, max compression
+gzip compressed data, was "pddl_embeddings-0.0.2.tar", last modified: Sat May 11 11:03:03 2024, max compression
```

## Comparing `pddl_embeddings-0.0.1.dev1.tar` & `pddl_embeddings-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 vicdoja    (501) staff       (20)        0 2024-04-30 18:37:43.942104 pddl_embeddings-0.0.1.dev1/
--rw-r--r--   0 vicdoja    (501) staff       (20)     1077 2024-04-30 18:11:39.000000 pddl_embeddings-0.0.1.dev1/LICENSE.txt
--rw-r--r--   0 vicdoja    (501) staff       (20)     1995 2024-04-30 18:37:43.941904 pddl_embeddings-0.0.1.dev1/PKG-INFO
--rw-r--r--   0 vicdoja    (501) staff       (20)       89 2024-04-30 18:11:39.000000 pddl_embeddings-0.0.1.dev1/README.md
--rw-r--r--   0 vicdoja    (501) staff       (20)      811 2024-04-30 18:34:13.000000 pddl_embeddings-0.0.1.dev1/pyproject.toml
--rw-r--r--   0 vicdoja    (501) staff       (20)       38 2024-04-30 18:37:43.942144 pddl_embeddings-0.0.1.dev1/setup.cfg
-drwxr-xr-x   0 vicdoja    (501) staff       (20)        0 2024-04-30 18:37:43.939998 pddl_embeddings-0.0.1.dev1/src/
-drwxr-xr-x   0 vicdoja    (501) staff       (20)        0 2024-04-30 18:37:43.940627 pddl_embeddings-0.0.1.dev1/src/pddl_embeddings/
--rw-r--r--   0 vicdoja    (501) staff       (20)        0 2024-04-30 18:10:49.000000 pddl_embeddings-0.0.1.dev1/src/pddl_embeddings/__init__.py
--rw-r--r--   0 vicdoja    (501) staff       (20)       45 2024-04-30 18:11:39.000000 pddl_embeddings-0.0.1.dev1/src/pddl_embeddings/hello_world.py
-drwxr-xr-x   0 vicdoja    (501) staff       (20)        0 2024-04-30 18:37:43.941701 pddl_embeddings-0.0.1.dev1/src/pddl_embeddings.egg-info/
--rw-r--r--   0 vicdoja    (501) staff       (20)     1995 2024-04-30 18:37:43.000000 pddl_embeddings-0.0.1.dev1/src/pddl_embeddings.egg-info/PKG-INFO
--rw-r--r--   0 vicdoja    (501) staff       (20)      275 2024-04-30 18:37:43.000000 pddl_embeddings-0.0.1.dev1/src/pddl_embeddings.egg-info/SOURCES.txt
--rw-r--r--   0 vicdoja    (501) staff       (20)        1 2024-04-30 18:37:43.000000 pddl_embeddings-0.0.1.dev1/src/pddl_embeddings.egg-info/dependency_links.txt
--rw-r--r--   0 vicdoja    (501) staff       (20)       16 2024-04-30 18:37:43.000000 pddl_embeddings-0.0.1.dev1/src/pddl_embeddings.egg-info/top_level.txt
+drwxr-xr-x   0 vicdoja    (501) staff       (20)        0 2024-05-11 11:03:03.612878 pddl_embeddings-0.0.2/
+-rw-r--r--   0 vicdoja    (501) staff       (20)     1077 2024-04-30 18:11:39.000000 pddl_embeddings-0.0.2/LICENSE.txt
+-rw-r--r--   0 vicdoja    (501) staff       (20)     2054 2024-05-11 11:03:03.612713 pddl_embeddings-0.0.2/PKG-INFO
+-rw-r--r--   0 vicdoja    (501) staff       (20)       83 2024-04-30 18:38:58.000000 pddl_embeddings-0.0.2/README.md
+-rw-r--r--   0 vicdoja    (501) staff       (20)      852 2024-05-11 11:02:53.000000 pddl_embeddings-0.0.2/pyproject.toml
+-rw-r--r--   0 vicdoja    (501) staff       (20)       38 2024-05-11 11:03:03.612914 pddl_embeddings-0.0.2/setup.cfg
+drwxr-xr-x   0 vicdoja    (501) staff       (20)        0 2024-05-11 11:03:03.611280 pddl_embeddings-0.0.2/src/
+drwxr-xr-x   0 vicdoja    (501) staff       (20)        0 2024-05-11 11:03:03.611836 pddl_embeddings-0.0.2/src/pddl_embeddings/
+-rw-r--r--   0 vicdoja    (501) staff       (20)        0 2024-04-30 18:10:49.000000 pddl_embeddings-0.0.2/src/pddl_embeddings/__init__.py
+-rw-r--r--   0 vicdoja    (501) staff       (20)     1378 2024-05-11 10:55:16.000000 pddl_embeddings-0.0.2/src/pddl_embeddings/feature_extractor.py
+drwxr-xr-x   0 vicdoja    (501) staff       (20)        0 2024-05-11 11:03:03.612552 pddl_embeddings-0.0.2/src/pddl_embeddings.egg-info/
+-rw-r--r--   0 vicdoja    (501) staff       (20)     2054 2024-05-11 11:03:03.000000 pddl_embeddings-0.0.2/src/pddl_embeddings.egg-info/PKG-INFO
+-rw-r--r--   0 vicdoja    (501) staff       (20)      323 2024-05-11 11:03:03.000000 pddl_embeddings-0.0.2/src/pddl_embeddings.egg-info/SOURCES.txt
+-rw-r--r--   0 vicdoja    (501) staff       (20)        1 2024-05-11 11:03:03.000000 pddl_embeddings-0.0.2/src/pddl_embeddings.egg-info/dependency_links.txt
+-rw-r--r--   0 vicdoja    (501) staff       (20)       25 2024-05-11 11:03:03.000000 pddl_embeddings-0.0.2/src/pddl_embeddings.egg-info/requires.txt
+-rw-r--r--   0 vicdoja    (501) staff       (20)       16 2024-05-11 11:03:03.000000 pddl_embeddings-0.0.2/src/pddl_embeddings.egg-info/top_level.txt
```

### Comparing `pddl_embeddings-0.0.1.dev1/LICENSE.txt` & `pddl_embeddings-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pddl_embeddings-0.0.1.dev1/PKG-INFO` & `pddl_embeddings-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pddl-embeddings
-Version: 0.0.1.dev1
+Version: 0.0.2
 Summary: A package to extract feature embeddings out of PPDL state text.
 Author-email: Victor Dorado Javier <vicdoja@upv.edu.es>
 Maintainer-email: Victor Dorado Javier <vicdoja@upv.edu.es>
 License: MIT License
         
         Copyright (c) 2024 Victor Dorado Javier
         
@@ -31,11 +31,14 @@
 Classifier: Programming Language :: Python
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: transformers
+Requires-Dist: numpy
+Requires-Dist: torch
 
-# ppdl-state-embeddings
+# ppdl-embeddings
 
 A package to extract feature embeddings out of PPDL state text.
```

### Comparing `pddl_embeddings-0.0.1.dev1/pyproject.toml` & `pddl_embeddings-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pddl-embeddings"
-version = "0.0.1dev1"
+version = "0.0.2"
 dependencies = [
-
+    "transformers",
+    "numpy",
+    "torch",
 ]
 requires-python = ">=3.9"
 authors = [
     {name = "Victor Dorado Javier", email = "vicdoja@upv.edu.es"},
 ]
 maintainers = [
     {name = "Victor Dorado Javier", email = "vicdoja@upv.edu.es"},
```

### Comparing `pddl_embeddings-0.0.1.dev1/src/pddl_embeddings.egg-info/PKG-INFO` & `pddl_embeddings-0.0.2/src/pddl_embeddings.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pddl-embeddings
-Version: 0.0.1.dev1
+Version: 0.0.2
 Summary: A package to extract feature embeddings out of PPDL state text.
 Author-email: Victor Dorado Javier <vicdoja@upv.edu.es>
 Maintainer-email: Victor Dorado Javier <vicdoja@upv.edu.es>
 License: MIT License
         
         Copyright (c) 2024 Victor Dorado Javier
         
@@ -31,11 +31,14 @@
 Classifier: Programming Language :: Python
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: transformers
+Requires-Dist: numpy
+Requires-Dist: torch
 
-# ppdl-state-embeddings
+# ppdl-embeddings
 
 A package to extract feature embeddings out of PPDL state text.
```

