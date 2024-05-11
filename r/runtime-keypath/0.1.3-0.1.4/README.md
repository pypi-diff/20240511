# Comparing `tmp/runtime-keypath-0.1.3.tar.gz` & `tmp/runtime_keypath-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtime-keypath-0.1.3.tar", last modified: Wed Dec  6 03:49:56 2023, max compression
+gzip compressed data, was "runtime_keypath-0.1.4.tar", last modified: Sat May 11 08:33:59 2024, max compression
```

## Comparing `runtime-keypath-0.1.3.tar` & `runtime_keypath-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 03:49:56.171181 runtime-keypath-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-12-06 03:49:47.000000 runtime-keypath-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-12-06 03:49:56.171181 runtime-keypath-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-12-06 03:49:47.000000 runtime-keypath-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      735 2023-12-06 03:49:47.000000 runtime-keypath-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 03:49:56.171181 runtime-keypath-0.1.3/runtime_keypath/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-06 03:49:47.000000 runtime-keypath-0.1.3/runtime_keypath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9125 2023-12-06 03:49:47.000000 runtime-keypath-0.1.3/runtime_keypath/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2023-12-06 03:49:47.000000 runtime-keypath-0.1.3/runtime_keypath/_core_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 03:49:56.171181 runtime-keypath-0.1.3/runtime_keypath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-12-06 03:49:56.000000 runtime-keypath-0.1.3/runtime_keypath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-06 03:49:56.000000 runtime-keypath-0.1.3/runtime_keypath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 03:49:56.000000 runtime-keypath-0.1.3/runtime_keypath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-06 03:49:56.000000 runtime-keypath-0.1.3/runtime_keypath.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 03:49:56.171181 runtime-keypath-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-06 03:49:47.000000 runtime-keypath-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:33:59.572469 runtime_keypath-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-11 08:33:55.000000 runtime_keypath-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-11 08:33:59.572469 runtime_keypath-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-11 08:33:55.000000 runtime_keypath-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-11 08:33:55.000000 runtime_keypath-0.1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:33:59.568469 runtime_keypath-0.1.4/runtime_keypath/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 08:33:55.000000 runtime_keypath-0.1.4/runtime_keypath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9125 2024-05-11 08:33:55.000000 runtime_keypath-0.1.4/runtime_keypath/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-11 08:33:55.000000 runtime_keypath-0.1.4/runtime_keypath/_core_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 08:33:55.000000 runtime_keypath-0.1.4/runtime_keypath/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:33:59.572469 runtime_keypath-0.1.4/runtime_keypath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-11 08:33:59.000000 runtime_keypath-0.1.4/runtime_keypath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-11 08:33:59.000000 runtime_keypath-0.1.4/runtime_keypath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 08:33:59.000000 runtime_keypath-0.1.4/runtime_keypath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 08:33:59.000000 runtime_keypath-0.1.4/runtime_keypath.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 08:33:59.572469 runtime_keypath-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-11 08:33:55.000000 runtime_keypath-0.1.4/setup.py
```

### Comparing `runtime-keypath-0.1.3/LICENSE` & `runtime_keypath-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `runtime-keypath-0.1.3/PKG-INFO` & `runtime_keypath-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtime-keypath
-Version: 0.1.3
+Version: 0.1.4
 Summary: Supports runtime key-path recording/accessing for Python.
 Author-email: Chris Fu <17433201@qq.com>
 License: MIT License
         
         Copyright (c) 2022 傅立业（Chris Fu）
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `runtime-keypath-0.1.3/README.md` & `runtime_keypath-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `runtime-keypath-0.1.3/pyproject.toml` & `runtime_keypath-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "runtime-keypath"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{ name = "Chris Fu", email = "17433201@qq.com" }]
 description = "Supports runtime key-path recording/accessing for Python."
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
```

### Comparing `runtime-keypath-0.1.3/runtime_keypath/_core.py` & `runtime_keypath-0.1.4/runtime_keypath/_core.py`

 * *Files identical despite different names*

### Comparing `runtime-keypath-0.1.3/runtime_keypath/_core_test.py` & `runtime_keypath-0.1.4/runtime_keypath/_core_test.py`

 * *Files identical despite different names*

### Comparing `runtime-keypath-0.1.3/runtime_keypath.egg-info/PKG-INFO` & `runtime_keypath-0.1.4/runtime_keypath.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtime-keypath
-Version: 0.1.3
+Version: 0.1.4
 Summary: Supports runtime key-path recording/accessing for Python.
 Author-email: Chris Fu <17433201@qq.com>
 License: MIT License
         
         Copyright (c) 2022 傅立业（Chris Fu）
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

