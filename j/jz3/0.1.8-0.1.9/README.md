# Comparing `tmp/jz3-0.1.8.tar.gz` & `tmp/jz3-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jz3-0.1.8.tar", last modified: Mon Apr 29 05:36:08 2024, max compression
+gzip compressed data, was "jz3-0.1.9.tar", last modified: Mon Apr 29 05:37:58 2024, max compression
```

## Comparing `jz3-0.1.8.tar` & `jz3-0.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.363923 jz3-0.1.8/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1096 2024-04-18 04:18:37.000000 jz3-0.1.8/LICENSE-Z3.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     1092 2024-04-18 04:24:33.000000 jz3-0.1.8/LICENSE.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:30:26.000000 jz3-0.1.8/MANIFEST.in
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-29 05:36:08.363510 jz3-0.1.8/PKG-INFO
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2347 2024-04-19 04:33:39.000000 jz3-0.1.8/README.md
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.333994 jz3-0.1.8/jz3/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       76 2024-04-28 23:38:27.000000 jz3-0.1.8/jz3/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.334939 jz3-0.1.8/jz3/analysis/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.8/jz3/analysis/__init__.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.335129 jz3-0.1.8/jz3/analysis/archive/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.8/jz3/analysis/archive/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2859 2024-04-19 01:59:02.000000 jz3-0.1.8/jz3/analysis/archive/export_to_excel.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.336335 jz3-0.1.8/jz3/analysis/scripts/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 04:00:01.000000 jz3-0.1.8/jz3/analysis/scripts/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7204 2024-04-29 03:30:57.000000 jz3-0.1.8/jz3/analysis/scripts/compare_whole_problems.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     7955 2024-04-28 04:25:24.000000 jz3-0.1.8/jz3/analysis/scripts/plot_comparison.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.336737 jz3-0.1.8/jz3/solvers/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.8/jz3/solvers/__init__.py
--rwxr-xr-x   0 jiazhenghao   (501) staff       (20) 20962472 2024-04-18 02:04:14.000000 jz3-0.1.8/jz3/solvers/cvc5-macOS-arm64
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.358243 jz3-0.1.8/jz3/src/
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.360969 jz3-0.1.8/jz3/src/SMTs/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    11530 2024-04-18 02:04:15.000000 jz3-0.1.8/jz3/src/SMTs/SMTs.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.8/jz3/src/SMTs/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.8/jz3/src/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     4545 2024-04-28 23:56:27.000000 jz3-0.1.8/jz3/src/run_solvers.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      282 2024-04-28 04:36:42.000000 jz3-0.1.8/jz3/src/z3_quick_start_guide.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)    11111 2024-04-29 03:24:04.000000 jz3-0.1.8/jz3/src/z3_wrapper.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.361525 jz3-0.1.8/jz3/tests/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:12.000000 jz3-0.1.8/jz3/tests/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:20.000000 jz3-0.1.8/jz3/tests/test_solver.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.362433 jz3-0.1.8/jz3/utils/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 07:53:53.000000 jz3-0.1.8/jz3/utils/__init__.py
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2900 2024-04-28 17:01:30.000000 jz3-0.1.8/jz3/utils/helpers.py
-drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:36:08.334819 jz3-0.1.8/jz3.egg-info/
--rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-29 05:36:08.000000 jz3-0.1.8/jz3.egg-info/PKG-INFO
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      711 2024-04-29 05:36:08.000000 jz3-0.1.8/jz3.egg-info/SOURCES.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        1 2024-04-29 05:36:08.000000 jz3-0.1.8/jz3.egg-info/dependency_links.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       21 2024-04-29 05:36:08.000000 jz3-0.1.8/jz3.egg-info/requires.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)        4 2024-04-29 05:36:08.000000 jz3-0.1.8/jz3.egg-info/top_level.txt
--rw-r--r--   0 jiazhenghao   (501) staff       (20)       38 2024-04-29 05:36:08.364165 jz3-0.1.8/setup.cfg
--rw-r--r--   0 jiazhenghao   (501) staff       (20)      894 2024-04-29 05:36:07.000000 jz3-0.1.8/setup.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:37:58.906118 jz3-0.1.9/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1096 2024-04-18 04:18:37.000000 jz3-0.1.9/LICENSE-Z3.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     1092 2024-04-18 04:24:33.000000 jz3-0.1.9/LICENSE.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 05:30:26.000000 jz3-0.1.9/MANIFEST.in
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-29 05:37:58.905981 jz3-0.1.9/PKG-INFO
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2347 2024-04-19 04:33:39.000000 jz3-0.1.9/README.md
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:37:58.883710 jz3-0.1.9/jz3/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       80 2024-04-29 05:37:40.000000 jz3-0.1.9/jz3/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:37:58.886541 jz3-0.1.9/jz3/analysis/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.9/jz3/analysis/__init__.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:37:58.887040 jz3-0.1.9/jz3/analysis/archive/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:10.000000 jz3-0.1.9/jz3/analysis/archive/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20)     2859 2024-04-19 01:59:02.000000 jz3-0.1.9/jz3/analysis/archive/export_to_excel.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:37:58.887980 jz3-0.1.9/jz3/analysis/scripts/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 04:00:01.000000 jz3-0.1.9/jz3/analysis/scripts/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     7204 2024-04-29 03:30:57.000000 jz3-0.1.9/jz3/analysis/scripts/compare_whole_problems.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     7955 2024-04-28 04:25:24.000000 jz3-0.1.9/jz3/analysis/scripts/plot_comparison.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:37:58.888457 jz3-0.1.9/jz3/solvers/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:04:14.000000 jz3-0.1.9/jz3/solvers/__init__.py
+-rwxr-xr-x   0 jiazhenghao   (501) staff       (20) 20962472 2024-04-18 02:04:14.000000 jz3-0.1.9/jz3/solvers/cvc5-macOS-arm64
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:37:58.904115 jz3-0.1.9/jz3/src/
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:37:58.904738 jz3-0.1.9/jz3/src/SMTs/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    11530 2024-04-18 02:04:15.000000 jz3-0.1.9/jz3/src/SMTs/SMTs.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.9/jz3/src/SMTs/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-19 03:56:15.000000 jz3-0.1.9/jz3/src/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     4545 2024-04-28 23:56:27.000000 jz3-0.1.9/jz3/src/run_solvers.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      282 2024-04-28 04:36:42.000000 jz3-0.1.9/jz3/src/z3_quick_start_guide.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)    11111 2024-04-29 03:24:04.000000 jz3-0.1.9/jz3/src/z3_wrapper.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:37:58.904950 jz3-0.1.9/jz3/tests/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:12.000000 jz3-0.1.9/jz3/tests/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-18 02:08:20.000000 jz3-0.1.9/jz3/tests/test_solver.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:37:58.905145 jz3-0.1.9/jz3/utils/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        0 2024-04-28 07:53:53.000000 jz3-0.1.9/jz3/utils/__init__.py
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2900 2024-04-28 17:01:30.000000 jz3-0.1.9/jz3/utils/helpers.py
+drwxr-xr-x   0 jiazhenghao   (501) staff       (20)        0 2024-04-29 05:37:58.886242 jz3-0.1.9/jz3.egg-info/
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)     2984 2024-04-29 05:37:58.000000 jz3-0.1.9/jz3.egg-info/PKG-INFO
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      711 2024-04-29 05:37:58.000000 jz3-0.1.9/jz3.egg-info/SOURCES.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        1 2024-04-29 05:37:58.000000 jz3-0.1.9/jz3.egg-info/dependency_links.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       21 2024-04-29 05:37:58.000000 jz3-0.1.9/jz3.egg-info/requires.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)        4 2024-04-29 05:37:58.000000 jz3-0.1.9/jz3.egg-info/top_level.txt
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)       38 2024-04-29 05:37:58.906170 jz3-0.1.9/setup.cfg
+-rw-r--r--   0 jiazhenghao   (501) staff       (20)      894 2024-04-29 05:37:56.000000 jz3-0.1.9/setup.py
```

### Comparing `jz3-0.1.8/LICENSE-Z3.txt` & `jz3-0.1.9/LICENSE-Z3.txt`

 * *Files identical despite different names*

### Comparing `jz3-0.1.8/LICENSE.txt` & `jz3-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jz3-0.1.8/PKG-INFO` & `jz3-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jz3
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple wrapper for Z3 solver
 Home-page: https://github.com/Robert-Jia00129/jz3
 Author: Sebastiaan Joosten, Zheng Robert Jia
 Author-email: jia00129@umn.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `jz3-0.1.8/README.md` & `jz3-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jz3-0.1.8/jz3/analysis/archive/export_to_excel.py` & `jz3-0.1.9/jz3/analysis/archive/export_to_excel.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.8/jz3/analysis/scripts/compare_whole_problems.py` & `jz3-0.1.9/jz3/analysis/scripts/compare_whole_problems.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.8/jz3/analysis/scripts/plot_comparison.py` & `jz3-0.1.9/jz3/analysis/scripts/plot_comparison.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.8/jz3/solvers/cvc5-macOS-arm64` & `jz3-0.1.9/jz3/solvers/cvc5-macOS-arm64`

 * *Files identical despite different names*

### Comparing `jz3-0.1.8/jz3/src/SMTs/SMTs.py` & `jz3-0.1.9/jz3/src/SMTs/SMTs.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.8/jz3/src/run_solvers.py` & `jz3-0.1.9/jz3/src/run_solvers.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.8/jz3/src/z3_wrapper.py` & `jz3-0.1.9/jz3/src/z3_wrapper.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.8/jz3/utils/helpers.py` & `jz3-0.1.9/jz3/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `jz3-0.1.8/jz3.egg-info/PKG-INFO` & `jz3-0.1.9/jz3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jz3
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple wrapper for Z3 solver
 Home-page: https://github.com/Robert-Jia00129/jz3
 Author: Sebastiaan Joosten, Zheng Robert Jia
 Author-email: jia00129@umn.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `jz3-0.1.8/jz3.egg-info/SOURCES.txt` & `jz3-0.1.9/jz3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

