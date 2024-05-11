# Comparing `tmp/model_checker-0.2.8.tar.gz` & `tmp/model_checker-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.2.8.tar", last modified: Mon May  6 22:12:19 2024, max compression
+gzip compressed data, was "model_checker-0.2.9.tar", last modified: Mon May  6 22:32:57 2024, max compression
```

## Comparing `model_checker-0.2.8.tar` & `model_checker-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 22:12:19.275984 model_checker-0.2.8/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-04-26 19:58:45.000000 model_checker-0.2.8/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     1372 2024-05-06 22:12:19.275984 model_checker-0.2.8/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      683 2024-05-06 19:44:36.000000 model_checker-0.2.8/README.md
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 22:12:19.275984 model_checker-0.2.8/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     1372 2024-05-06 22:12:19.000000 model_checker-0.2.8/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      396 2024-05-06 22:12:19.000000 model_checker-0.2.8/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-06 22:12:19.000000 model_checker-0.2.8/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       61 2024-05-06 22:12:19.000000 model_checker-0.2.8/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-06 22:12:19.000000 model_checker-0.2.8/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        8 2024-05-06 22:12:19.000000 model_checker-0.2.8/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 22:12:19.275984 model_checker-0.2.8/package/
--rw-r--r--   0 benjamin  (1000) users      (100)        0 2024-05-06 21:38:54.000000 model_checker-0.2.8/package/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    16026 2024-05-06 22:03:56.000000 model_checker-0.2.8/package/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    34588 2024-05-06 22:03:56.000000 model_checker-0.2.8/package/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    19659 2024-05-06 22:03:56.000000 model_checker-0.2.8/package/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7265 2024-05-06 21:11:53.000000 model_checker-0.2.8/package/syntax.py
--rw-r--r--   0 benjamin  (1000) users      (100)     5838 2024-05-06 22:08:39.000000 model_checker-0.2.8/package/test_complete.py
--rw-r--r--   0 benjamin  (1000) users      (100)      901 2024-05-06 22:11:52.000000 model_checker-0.2.8/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-06 22:12:19.275984 model_checker-0.2.8/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 22:32:57.401485 model_checker-0.2.9/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-04-26 19:58:45.000000 model_checker-0.2.9/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     1372 2024-05-06 22:32:57.401485 model_checker-0.2.9/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      683 2024-05-06 19:44:36.000000 model_checker-0.2.9/README.md
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 22:32:57.401485 model_checker-0.2.9/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1372 2024-05-06 22:32:57.000000 model_checker-0.2.9/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      456 2024-05-06 22:32:57.000000 model_checker-0.2.9/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-06 22:32:57.000000 model_checker-0.2.9/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       67 2024-05-06 22:32:57.000000 model_checker-0.2.9/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-06 22:32:57.000000 model_checker-0.2.9/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        4 2024-05-06 22:32:57.000000 model_checker-0.2.9/model_checker.egg-info/top_level.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)      907 2024-05-06 22:32:22.000000 model_checker-0.2.9/pyproject.toml
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 22:32:57.400485 model_checker-0.2.9/scr/
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-06 22:32:57.401485 model_checker-0.2.9/scr/model_checker/
+-rw-r--r--   0 benjamin  (1000) users      (100)        0 2024-05-06 21:38:54.000000 model_checker-0.2.9/scr/model_checker/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    16026 2024-05-06 22:19:35.000000 model_checker-0.2.9/scr/model_checker/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    34588 2024-05-06 22:19:35.000000 model_checker-0.2.9/scr/model_checker/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    19659 2024-05-06 22:19:35.000000 model_checker-0.2.9/scr/model_checker/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7265 2024-05-06 21:11:53.000000 model_checker-0.2.9/scr/model_checker/syntax.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     5838 2024-05-06 22:32:06.000000 model_checker-0.2.9/scr/model_checker/test_complete.py
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-06 22:32:57.401485 model_checker-0.2.9/setup.cfg
```

### Comparing `model_checker-0.2.8/LICENCE` & `model_checker-0.2.9/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.8/PKG-INFO` & `model_checker-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.2.8
+Version: 0.2.9
 Summary: A hyperintensional model checker for counterfactual conditionals
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.2.8/README.md` & `model_checker-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.8/model_checker.egg-info/PKG-INFO` & `model_checker-0.2.9/model_checker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.2.8
+Version: 0.2.9
 Summary: A hyperintensional model checker for counterfactual conditionals
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,counterfactuals,model checker,theorem prover
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.2.8/package/model_definitions.py` & `model_checker-0.2.9/scr/model_checker/model_definitions.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.8/package/model_structure.py` & `model_checker-0.2.9/scr/model_checker/model_structure.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.8/package/semantics.py` & `model_checker-0.2.9/scr/model_checker/semantics.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.8/package/syntax.py` & `model_checker-0.2.9/scr/model_checker/syntax.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.8/package/test_complete.py` & `model_checker-0.2.9/scr/model_checker/test_complete.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.2.8/pyproject.toml` & `model_checker-0.2.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.2.8"
+version = "0.2.9"
 description = "A hyperintensional model checker for counterfactual conditionals"
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
@@ -23,8 +23,8 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/benbrastmckie/ModelChecker"
 Issues = "https://github.com/benbrastmckie/ModelChecker/issues"
 
 [project.scripts]
-model-checker = "package.test_complete:main"
+model-checker = "model_checker.test_complete:main"
```

