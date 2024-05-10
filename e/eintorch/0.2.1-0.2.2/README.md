# Comparing `tmp/eintorch-0.2.1.tar.gz` & `tmp/eintorch-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eintorch-0.2.1.tar", max compression
+gzip compressed data, was "eintorch-0.2.2.tar", max compression
```

## Comparing `eintorch-0.2.1.tar` & `eintorch-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1515 2024-02-04 11:41:26.968966 eintorch-0.2.1/LICENSE
--rw-r--r--   0        0        0       63 2024-05-06 21:43:46.710723 eintorch-0.2.1/README.md
--rw-r--r--   0        0        0      678 2024-05-08 16:00:57.377873 eintorch-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-05-06 21:46:30.204115 eintorch-0.2.1/src/eintorch/.DS_Store
--rw-r--r--   0        0        0       99 2024-05-02 15:12:31.395026 eintorch-0.2.1/src/eintorch/__init__.py
--rw-r--r--   0        0        0     4347 2024-05-07 12:38:20.849516 eintorch-0.2.1/src/eintorch/_core.py
--rw-r--r--   0        0        0     1369 2024-05-06 23:31:40.470828 eintorch-0.2.1/src/eintorch/_functions.py
--rw-r--r--   0        0        0     2412 2024-05-06 21:10:54.810858 eintorch-0.2.1/src/eintorch/_preprocessing.py
--rw-r--r--   0        0        0     1017 2024-05-06 21:29:42.595030 eintorch-0.2.1/src/eintorch/_utils.py
--rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 eintorch-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1515 2024-02-04 11:41:26.968966 eintorch-0.2.2/LICENSE
+-rw-r--r--   0        0        0       63 2024-05-06 21:43:46.710723 eintorch-0.2.2/README.md
+-rw-r--r--   0        0        0      678 2024-05-10 23:16:37.913294 eintorch-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-06 21:46:30.204115 eintorch-0.2.2/src/eintorch/.DS_Store
+-rw-r--r--   0        0        0       99 2024-05-02 15:12:31.395026 eintorch-0.2.2/src/eintorch/__init__.py
+-rw-r--r--   0        0        0     4347 2024-05-07 12:38:20.849516 eintorch-0.2.2/src/eintorch/_core.py
+-rw-r--r--   0        0        0     1369 2024-05-06 23:31:40.470828 eintorch-0.2.2/src/eintorch/_functions.py
+-rw-r--r--   0        0        0     2412 2024-05-06 21:10:54.810858 eintorch-0.2.2/src/eintorch/_preprocessing.py
+-rw-r--r--   0        0        0      878 2024-05-10 23:16:17.627187 eintorch-0.2.2/src/eintorch/_utils.py
+-rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 eintorch-0.2.2/PKG-INFO
```

### Comparing `eintorch-0.2.1/LICENSE` & `eintorch-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eintorch-0.2.1/pyproject.toml` & `eintorch-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eintorch"
-version = "0.2.1"
+version = "0.2.2"
 description = "An alternative interface for torchdim"
 authors = ["Jakub Bachurski <kbachurski@gmail.com>", "Euan Ong <euan.l.y.ong@gmail.com>"]
 readme = "README.md"
 packages = [{include = "eintorch", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `eintorch-0.2.1/src/eintorch/.DS_Store` & `eintorch-0.2.2/src/eintorch/.DS_Store`

 * *Files identical despite different names*

### Comparing `eintorch-0.2.1/src/eintorch/_core.py` & `eintorch-0.2.2/src/eintorch/_core.py`

 * *Files identical despite different names*

### Comparing `eintorch-0.2.1/src/eintorch/_functions.py` & `eintorch-0.2.2/src/eintorch/_functions.py`

 * *Files identical despite different names*

### Comparing `eintorch-0.2.1/src/eintorch/_preprocessing.py` & `eintorch-0.2.2/src/eintorch/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `eintorch-0.2.1/src/eintorch/_utils.py` & `eintorch-0.2.2/src/eintorch/_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,13 @@
 from __future__ import annotations
 
-import hashlib
 import inspect
-import io
-import pickle
 from inspect import signature
 from typing import Any, Callable
 
-import dill
-import torch
-from functorch.dim import Dim
-from functorch.dim import Tensor as DTensor
-
 SINGLE_POSITIONALS = frozenset(
     (inspect.Parameter.POSITIONAL_ONLY, inspect.Parameter.POSITIONAL_OR_KEYWORD)
 )
 try:
     from IPython import get_ipython
 
     ipy = get_ipython()
```

### Comparing `eintorch-0.2.1/PKG-INFO` & `eintorch-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eintorch
-Version: 0.2.1
+Version: 0.2.2
 Summary: An alternative interface for torchdim
 Author: Jakub Bachurski
 Author-email: kbachurski@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

