# Comparing `tmp/archivefile-0.3.0.tar.gz` & `tmp/archivefile-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archivefile-0.3.0.tar", max compression
+gzip compressed data, was "archivefile-0.3.1.tar", max compression
```

## Comparing `archivefile-0.3.0.tar` & `archivefile-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4912 2024-05-05 07:25:35.226997 archivefile-0.3.0/README.md
--rw-r--r--   0        0        0     2309 2024-05-05 07:25:35.226997 archivefile-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      598 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/__init__.py
--rw-r--r--   0        0        0      244 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_compat.py
--rw-r--r--   0        0        0    36784 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_core.py
--rw-r--r--   0        0        0      980 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_enums.py
--rw-r--r--   0        0        0      201 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_exceptions.py
--rw-r--r--   0        0        0     1404 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_models.py
--rw-r--r--   0        0        0     1171 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_types.py
--rw-r--r--   0        0        0     2775 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_utils.py
--rw-r--r--   0        0        0      526 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/_version.py
--rw-r--r--   0        0        0        0 2024-05-05 07:25:35.226997 archivefile-0.3.0/src/archivefile/py.typed
--rw-r--r--   0        0        0     6718 1970-01-01 00:00:00.000000 archivefile-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4912 2024-05-11 19:07:16.106019 archivefile-0.3.1/README.md
+-rw-r--r--   0        0        0     2309 2024-05-11 19:07:16.110019 archivefile-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      598 2024-05-11 19:07:16.110019 archivefile-0.3.1/src/archivefile/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-11 19:07:16.110019 archivefile-0.3.1/src/archivefile/_compat.py
+-rw-r--r--   0        0        0    36784 2024-05-11 19:07:16.110019 archivefile-0.3.1/src/archivefile/_core.py
+-rw-r--r--   0        0        0      980 2024-05-11 19:07:16.110019 archivefile-0.3.1/src/archivefile/_enums.py
+-rw-r--r--   0        0        0      201 2024-05-11 19:07:16.110019 archivefile-0.3.1/src/archivefile/_exceptions.py
+-rw-r--r--   0        0        0     1404 2024-05-11 19:07:16.110019 archivefile-0.3.1/src/archivefile/_models.py
+-rw-r--r--   0        0        0     1184 2024-05-11 19:07:16.110019 archivefile-0.3.1/src/archivefile/_types.py
+-rw-r--r--   0        0        0     2775 2024-05-11 19:07:16.110019 archivefile-0.3.1/src/archivefile/_utils.py
+-rw-r--r--   0        0        0      529 2024-05-11 19:07:16.110019 archivefile-0.3.1/src/archivefile/_version.py
+-rw-r--r--   0        0        0        0 2024-05-11 19:07:16.110019 archivefile-0.3.1/src/archivefile/py.typed
+-rw-r--r--   0        0        0     6718 1970-01-01 00:00:00.000000 archivefile-0.3.1/PKG-INFO
```

### Comparing `archivefile-0.3.0/README.md` & `archivefile-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `archivefile-0.3.0/pyproject.toml` & `archivefile-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archivefile"
-version = "0.3.0"
+version = "0.3.1"
 description = "Unified interface for tar, zip, sevenzip, and rar files"
 authors = ["Raventric <78981416+Ravencentric@users.noreply.github.com>"]
 readme = "README.md"
 license = "Unlicense"
 packages = [{ include = "archivefile", from = "src" }]
 keywords = ["archive", "archivefile", "zipfile", "tarfile", "sevenzip", "rarfile"]
 homepage = "https://ravencentric.github.io/archivefile"
```

### Comparing `archivefile-0.3.0/src/archivefile/__init__.py` & `archivefile-0.3.1/src/archivefile/__init__.py`

 * *Files identical despite different names*

### Comparing `archivefile-0.3.0/src/archivefile/_core.py` & `archivefile-0.3.1/src/archivefile/_core.py`

 * *Files identical despite different names*

### Comparing `archivefile-0.3.0/src/archivefile/_enums.py` & `archivefile-0.3.1/src/archivefile/_enums.py`

 * *Files identical despite different names*

### Comparing `archivefile-0.3.0/src/archivefile/_models.py` & `archivefile-0.3.1/src/archivefile/_models.py`

 * *Files identical despite different names*

### Comparing `archivefile-0.3.0/src/archivefile/_types.py` & `archivefile-0.3.1/src/archivefile/_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from pathlib import Path
 
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import Literal, TypeAlias, Union
 
-StrPath: TypeAlias = str | Path
+StrPath: TypeAlias = Union[str, Path]
 
 OpenArchiveMode: TypeAlias = Literal[
     "r",
     "r:*",
     "r:",
     "r:gz",
     "r:bz2",
```

### Comparing `archivefile-0.3.0/src/archivefile/_utils.py` & `archivefile-0.3.1/src/archivefile/_utils.py`

 * *Files identical despite different names*

### Comparing `archivefile-0.3.0/src/archivefile/_version.py` & `archivefile-0.3.1/src/archivefile/_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,14 @@
     """Minor version number"""
     patch: int
     """Patch version number"""
 
 
 def _get_version() -> str:
     """
-    Get the version of juicenet
+    Get the version of archivefile
     """
     try:
         return metadata.version("archivefile")
 
     except metadata.PackageNotFoundError:
         return "0.0.0"
```

### Comparing `archivefile-0.3.0/PKG-INFO` & `archivefile-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archivefile
-Version: 0.3.0
+Version: 0.3.1
 Summary: Unified interface for tar, zip, sevenzip, and rar files
 Home-page: https://ravencentric.github.io/archivefile
 License: Unlicense
 Keywords: archive,archivefile,zipfile,tarfile,sevenzip,rarfile
 Author: Raventric
 Author-email: 78981416+Ravencentric@users.noreply.github.com
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: archivefile Version: 0.3.0 Summary: Unified
+Metadata-Version: 2.1 Name: archivefile Version: 0.3.1 Summary: Unified
 interface for tar, zip, sevenzip, and rar files Home-page: https://
 ravencentric.github.io/archivefile License: Unlicense Keywords:
 archive,archivefile,zipfile,tarfile,sevenzip,rarfile Author: Raventric Author-
 email: 78981416+Ravencentric@users.noreply.github.com Requires-Python: >=3.9
 Classifier: License :: OSI Approved Classifier: License :: OSI Approved :: The
 Unlicense (Unlicense) Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

