# Comparing `tmp/aipkgs_firebase-1.0.3.tar.gz` & `tmp/aipkgs_firebase-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_firebase-1.0.3.tar", max compression
+gzip compressed data, was "aipkgs_firebase-1.0.5.tar", max compression
```

## Comparing `aipkgs_firebase-1.0.3.tar` & `aipkgs_firebase-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1058 2024-05-09 12:25:47.460445 aipkgs_firebase-1.0.3/LICENSE.md
--rw-r--r--   0        0        0       13 2022-03-08 13:06:48.929037 aipkgs_firebase-1.0.3/README.rst
--rw-r--r--   0        0        0       88 2022-03-08 13:06:48.928222 aipkgs_firebase-1.0.3/aipkgs_firebase/__init__.py
--rw-r--r--   0        0        0     1737 2024-05-11 14:14:48.035567 aipkgs_firebase-1.0.3/aipkgs_firebase/actions/core.py
--rw-r--r--   0        0        0     2302 2023-11-26 13:02:33.501317 aipkgs_firebase-1.0.3/aipkgs_firebase/helpers.py
--rw-r--r--   0        0        0     5948 2024-05-10 18:18:59.859448 aipkgs_firebase-1.0.3/aipkgs_firebase/messaging/core.py
--rw-r--r--   0        0        0      132 2024-05-10 18:17:53.723527 aipkgs_firebase-1.0.3/aipkgs_firebase/messaging/enums.py
--rw-r--r--   0        0        0     3079 2024-05-10 18:46:13.123781 aipkgs_firebase-1.0.3/aipkgs_firebase/messaging/helpers.py
--rw-r--r--   0        0        0     5510 2024-05-10 16:47:09.357450 aipkgs_firebase-1.0.3/aipkgs_firebase/storage/core.py
--rw-r--r--   0        0        0     3599 2024-05-10 16:48:36.758619 aipkgs_firebase-1.0.3/aipkgs_firebase/storage/helpers.py
--rw-r--r--   0        0        0     3393 2024-05-10 17:20:12.608367 aipkgs_firebase-1.0.3/aipkgs_firebase/storage/root.py
--rw-r--r--   0        0        0     2314 2024-05-10 18:47:03.096540 aipkgs_firebase-1.0.3/aipkgs_firebase/user/core.py
--rw-r--r--   0        0        0      687 2024-05-11 14:16:12.436012 aipkgs_firebase-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 aipkgs_firebase-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-09 12:25:47.460445 aipkgs_firebase-1.0.5/LICENSE.md
+-rw-r--r--   0        0        0       13 2022-03-08 13:06:48.929037 aipkgs_firebase-1.0.5/README.rst
+-rw-r--r--   0        0        0       88 2022-03-08 13:06:48.928222 aipkgs_firebase-1.0.5/aipkgs_firebase/__init__.py
+-rw-r--r--   0        0        0     1737 2024-05-11 14:14:48.035567 aipkgs_firebase-1.0.5/aipkgs_firebase/actions/core.py
+-rw-r--r--   0        0        0     2302 2023-11-26 13:02:33.501317 aipkgs_firebase-1.0.5/aipkgs_firebase/helpers.py
+-rw-r--r--   0        0        0     5948 2024-05-10 18:18:59.859448 aipkgs_firebase-1.0.5/aipkgs_firebase/messaging/core.py
+-rw-r--r--   0        0        0      132 2024-05-10 18:17:53.723527 aipkgs_firebase-1.0.5/aipkgs_firebase/messaging/enums.py
+-rw-r--r--   0        0        0     3079 2024-05-10 18:46:13.123781 aipkgs_firebase-1.0.5/aipkgs_firebase/messaging/helpers.py
+-rw-r--r--   0        0        0     5510 2024-05-10 16:47:09.357450 aipkgs_firebase-1.0.5/aipkgs_firebase/storage/core.py
+-rw-r--r--   0        0        0     3599 2024-05-10 16:48:36.758619 aipkgs_firebase-1.0.5/aipkgs_firebase/storage/helpers.py
+-rw-r--r--   0        0        0     3375 2024-05-11 15:47:58.271869 aipkgs_firebase-1.0.5/aipkgs_firebase/storage/root.py
+-rw-r--r--   0        0        0     2314 2024-05-10 18:47:03.096540 aipkgs_firebase-1.0.5/aipkgs_firebase/user/core.py
+-rw-r--r--   0        0        0      687 2024-05-11 16:01:30.681927 aipkgs_firebase-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 aipkgs_firebase-1.0.5/PKG-INFO
```

### Comparing `aipkgs_firebase-1.0.3/LICENSE.md` & `aipkgs_firebase-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.3/aipkgs_firebase/actions/core.py` & `aipkgs_firebase-1.0.5/aipkgs_firebase/actions/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.3/aipkgs_firebase/helpers.py` & `aipkgs_firebase-1.0.5/aipkgs_firebase/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.3/aipkgs_firebase/messaging/core.py` & `aipkgs_firebase-1.0.5/aipkgs_firebase/messaging/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.3/aipkgs_firebase/messaging/helpers.py` & `aipkgs_firebase-1.0.5/aipkgs_firebase/messaging/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.3/aipkgs_firebase/storage/core.py` & `aipkgs_firebase-1.0.5/aipkgs_firebase/storage/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.3/aipkgs_firebase/storage/helpers.py` & `aipkgs_firebase-1.0.5/aipkgs_firebase/storage/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.3/aipkgs_firebase/storage/root.py` & `aipkgs_firebase-1.0.5/aipkgs_firebase/storage/root.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from aipkgs_firebase.storage.core import FirebaseStorageCore
 from aipkgs_firebase.storage.helpers import FirebaseStorageHelper
 
 
 class FirebaseRootModel:
     collection_name = ""
 
-    @staticmethod
     def __init__(self, collection_name: str = None) -> None:
         self.collection_name = collection_name
 
     @staticmethod
     def exists(self, document_id: str) -> bool:
         return FirebaseStorageCore.document_exists(
             collection_name=self.collection_name, document_id=document_id
```

### Comparing `aipkgs_firebase-1.0.3/aipkgs_firebase/user/core.py` & `aipkgs_firebase-1.0.5/aipkgs_firebase/user/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.3/pyproject.toml` & `aipkgs_firebase-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["poetry-core>=1.0.3"]
+requires = ["poetry-core>=1.0.5"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aipkgs-firebase"
-version = "1.0.3"
+version = "1.0.5"
 description = "A utility package for interacting with Firebase, specifically Firestore, in a more streamlined and efficient manner."
 authors = ["Alexy <alexy.ib@outlook.com>"]
 # New attributes
 license = "MIT"
 readme = "README.rst"
 homepage = "https://gitlab.com/aipy/public/packages.git"
 repository = "https://gitlab.com/aipy/public/packages.git"
```

### Comparing `aipkgs_firebase-1.0.3/PKG-INFO` & `aipkgs_firebase-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipkgs-firebase
-Version: 1.0.3
+Version: 1.0.5
 Summary: A utility package for interacting with Firebase, specifically Firestore, in a more streamlined and efficient manner.
 Home-page: https://gitlab.com/aipy/public/packages.git
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
 Requires-Python: >=3.11.3,<4.0.0
```

