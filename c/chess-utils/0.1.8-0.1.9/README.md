# Comparing `tmp/chess_utils-0.1.8.tar.gz` & `tmp/chess_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_utils-0.1.8.tar", last modified: Tue Apr 23 08:40:19 2024, max compression
+gzip compressed data, was "chess_utils-0.1.9.tar", last modified: Tue Apr 23 08:48:08 2024, max compression
```

## Comparing `chess_utils-0.1.8.tar` & `chess_utils-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:40:19.750948 chess_utils-0.1.8/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      404 2024-04-23 08:40:19.740948 chess_utils-0.1.8/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      529 2024-04-23 08:40:17.000000 chess_utils-0.1.8/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-23 08:40:19.750948 chess_utils-0.1.8/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:40:19.740948 chess_utils-0.1.8/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:40:19.740948 chess_utils-0.1.8/src/chess_utils/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-23 08:38:49.000000 chess_utils-0.1.8/src/chess_utils/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      157 2024-04-23 08:39:09.000000 chess_utils-0.1.8/src/chess_utils/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      754 2024-04-23 08:37:14.000000 chess_utils-0.1.8/src/chess_utils/boards.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      591 2024-04-23 08:37:05.000000 chess_utils-0.1.8/src/chess_utils/fens.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      226 2024-04-23 08:37:55.000000 chess_utils-0.1.8/src/chess_utils/pgns.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:40:19.740948 chess_utils-0.1.8/src/chess_utils/random/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-04-23 08:35:13.000000 chess_utils-0.1.8/src/chess_utils/random/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1048 2024-04-23 08:34:52.000000 chess_utils-0.1.8/src/chess_utils/random/random.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:40:19.740948 chess_utils-0.1.8/src/chess_utils/test/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      458 2024-03-21 05:50:11.000000 chess_utils-0.1.8/src/chess_utils/test/test_parsing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      254 2024-04-04 18:45:50.000000 chess_utils-0.1.8/src/chess_utils/test.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:40:19.740948 chess_utils-0.1.8/src/chess_utils.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      404 2024-04-23 08:40:19.000000 chess_utils-0.1.8/src/chess_utils.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      468 2024-04-23 08:40:19.000000 chess_utils-0.1.8/src/chess_utils.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-23 08:40:19.000000 chess_utils-0.1.8/src/chess_utils.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-04-23 08:40:19.000000 chess_utils-0.1.8/src/chess_utils.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-04-23 08:40:19.000000 chess_utils-0.1.8/src/chess_utils.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:48:08.655056 chess_utils-0.1.9/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      404 2024-04-23 08:48:08.655056 chess_utils-0.1.9/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      529 2024-04-23 08:48:05.000000 chess_utils-0.1.9/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-23 08:48:08.655056 chess_utils-0.1.9/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:48:08.645056 chess_utils-0.1.9/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:48:08.655056 chess_utils-0.1.9/src/chess_utils/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-23 08:38:49.000000 chess_utils-0.1.9/src/chess_utils/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      286 2024-04-23 08:48:01.000000 chess_utils-0.1.9/src/chess_utils/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      754 2024-04-23 08:37:14.000000 chess_utils-0.1.9/src/chess_utils/boards.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      591 2024-04-23 08:37:05.000000 chess_utils-0.1.9/src/chess_utils/fens.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      226 2024-04-23 08:37:55.000000 chess_utils-0.1.9/src/chess_utils/pgns.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:48:08.655056 chess_utils-0.1.9/src/chess_utils/random/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-04-23 08:35:13.000000 chess_utils-0.1.9/src/chess_utils/random/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1048 2024-04-23 08:34:52.000000 chess_utils-0.1.9/src/chess_utils/random/random.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:48:08.655056 chess_utils-0.1.9/src/chess_utils/test/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      458 2024-03-21 05:50:11.000000 chess_utils-0.1.9/src/chess_utils/test/test_parsing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      254 2024-04-04 18:45:50.000000 chess_utils-0.1.9/src/chess_utils/test.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:48:08.655056 chess_utils-0.1.9/src/chess_utils.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      404 2024-04-23 08:48:08.000000 chess_utils-0.1.9/src/chess_utils.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      468 2024-04-23 08:48:08.000000 chess_utils-0.1.9/src/chess_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-23 08:48:08.000000 chess_utils-0.1.9/src/chess_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-04-23 08:48:08.000000 chess_utils-0.1.9/src/chess_utils.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-04-23 08:48:08.000000 chess_utils-0.1.9/src/chess_utils.egg-info/top_level.txt
```

### Comparing `chess_utils-0.1.8/pyproject.toml` & `chess_utils-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chess-utils"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Higher level utilities over the `chess` library"
 dependencies = [
   "chess", "pydantic", "lazy-loader"
 ]
```

### Comparing `chess_utils-0.1.8/src/chess_utils/boards.py` & `chess_utils-0.1.9/src/chess_utils/boards.py`

 * *Files identical despite different names*

### Comparing `chess_utils-0.1.8/src/chess_utils/fens.py` & `chess_utils-0.1.9/src/chess_utils/fens.py`

 * *Files identical despite different names*

### Comparing `chess_utils-0.1.8/src/chess_utils/random/random.py` & `chess_utils-0.1.9/src/chess_utils/random/random.py`

 * *Files identical despite different names*

