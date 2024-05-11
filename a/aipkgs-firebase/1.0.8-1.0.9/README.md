# Comparing `tmp/aipkgs_firebase-1.0.8.tar.gz` & `tmp/aipkgs_firebase-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_firebase-1.0.8.tar", max compression
+gzip compressed data, was "aipkgs_firebase-1.0.9.tar", max compression
```

## Comparing `aipkgs_firebase-1.0.8.tar` & `aipkgs_firebase-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1058 2024-05-09 12:25:47.460445 aipkgs_firebase-1.0.8/LICENSE.md
--rw-r--r--   0        0        0       13 2022-03-08 13:06:48.929037 aipkgs_firebase-1.0.8/README.rst
--rw-r--r--   0        0        0       88 2022-03-08 13:06:48.928222 aipkgs_firebase-1.0.8/aipkgs_firebase/__init__.py
--rw-r--r--   0        0        0     1737 2024-05-11 14:14:48.035567 aipkgs_firebase-1.0.8/aipkgs_firebase/actions/core.py
--rw-r--r--   0        0        0     2302 2023-11-26 13:02:33.501317 aipkgs_firebase-1.0.8/aipkgs_firebase/helpers.py
--rw-r--r--   0        0        0     5948 2024-05-10 18:18:59.859448 aipkgs_firebase-1.0.8/aipkgs_firebase/messaging/core.py
--rw-r--r--   0        0        0      132 2024-05-10 18:17:53.723527 aipkgs_firebase-1.0.8/aipkgs_firebase/messaging/enums.py
--rw-r--r--   0        0        0     3079 2024-05-10 18:46:13.123781 aipkgs_firebase-1.0.8/aipkgs_firebase/messaging/helpers.py
--rw-r--r--   0        0        0     7029 2024-05-11 19:20:36.361037 aipkgs_firebase-1.0.8/aipkgs_firebase/storage/core.py
--rw-r--r--   0        0        0     3644 2024-05-11 18:39:27.920304 aipkgs_firebase-1.0.8/aipkgs_firebase/storage/helpers.py
--rw-r--r--   0        0        0     3168 2024-05-11 18:15:23.035976 aipkgs_firebase-1.0.8/aipkgs_firebase/storage/root.py
--rw-r--r--   0        0        0     2314 2024-05-10 18:47:03.096540 aipkgs_firebase-1.0.8/aipkgs_firebase/user/core.py
--rw-r--r--   0        0        0      687 2024-05-11 19:21:22.254652 aipkgs_firebase-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 aipkgs_firebase-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-09 12:25:47.460445 aipkgs_firebase-1.0.9/LICENSE.md
+-rw-r--r--   0        0        0       13 2022-03-08 13:06:48.929037 aipkgs_firebase-1.0.9/README.rst
+-rw-r--r--   0        0        0       88 2022-03-08 13:06:48.928222 aipkgs_firebase-1.0.9/aipkgs_firebase/__init__.py
+-rw-r--r--   0        0        0     1737 2024-05-11 14:14:48.035567 aipkgs_firebase-1.0.9/aipkgs_firebase/actions/core.py
+-rw-r--r--   0        0        0     2302 2023-11-26 13:02:33.501317 aipkgs_firebase-1.0.9/aipkgs_firebase/helpers.py
+-rw-r--r--   0        0        0     5948 2024-05-10 18:18:59.859448 aipkgs_firebase-1.0.9/aipkgs_firebase/messaging/core.py
+-rw-r--r--   0        0        0      132 2024-05-10 18:17:53.723527 aipkgs_firebase-1.0.9/aipkgs_firebase/messaging/enums.py
+-rw-r--r--   0        0        0     3079 2024-05-10 18:46:13.123781 aipkgs_firebase-1.0.9/aipkgs_firebase/messaging/helpers.py
+-rw-r--r--   0        0        0     7029 2024-05-11 20:38:03.783240 aipkgs_firebase-1.0.9/aipkgs_firebase/storage/core.py
+-rw-r--r--   0        0        0     3644 2024-05-11 18:39:27.920304 aipkgs_firebase-1.0.9/aipkgs_firebase/storage/helpers.py
+-rw-r--r--   0        0        0     3442 2024-05-11 20:37:38.404957 aipkgs_firebase-1.0.9/aipkgs_firebase/storage/root.py
+-rw-r--r--   0        0        0     2314 2024-05-10 18:47:03.096540 aipkgs_firebase-1.0.9/aipkgs_firebase/user/core.py
+-rw-r--r--   0        0        0      687 2024-05-11 20:38:15.035177 aipkgs_firebase-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 aipkgs_firebase-1.0.9/PKG-INFO
```

### Comparing `aipkgs_firebase-1.0.8/LICENSE.md` & `aipkgs_firebase-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.8/aipkgs_firebase/actions/core.py` & `aipkgs_firebase-1.0.9/aipkgs_firebase/actions/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.8/aipkgs_firebase/helpers.py` & `aipkgs_firebase-1.0.9/aipkgs_firebase/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.8/aipkgs_firebase/messaging/core.py` & `aipkgs_firebase-1.0.9/aipkgs_firebase/messaging/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.8/aipkgs_firebase/messaging/helpers.py` & `aipkgs_firebase-1.0.9/aipkgs_firebase/messaging/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.8/aipkgs_firebase/storage/core.py` & `aipkgs_firebase-1.0.9/aipkgs_firebase/storage/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,24 +116,24 @@
 
             return True
 
         return False
 
     @staticmethod
     def create_document_from_snapshot(
-            collection_name: str, document: DocumentSnapshot
+            collection_name: str, snapshot: DocumentSnapshot
     ):
-        data = document.to_dict()
+        data = snapshot.to_dict()
 
         now = datetime.now()
         timestamp = now.strftime("%d-%m-%Y %I:%M:%S %p")
         data["timestamp"] = firebase_admin.firestore.SERVER_TIMESTAMP
         data["created_at"] = timestamp
 
-        document_id = document.id
+        document_id = snapshot.id
 
         if not FirebaseStorageCore.document_exists(
                 collection_name=collection_name, document_id=document_id
         ):
             doc_ref = FirebaseStorageCore.document_ref(
                 collection_name=collection_name, document_id=document_id
             )
```

### Comparing `aipkgs_firebase-1.0.8/aipkgs_firebase/storage/helpers.py` & `aipkgs_firebase-1.0.9/aipkgs_firebase/storage/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.8/aipkgs_firebase/storage/root.py` & `aipkgs_firebase-1.0.9/aipkgs_firebase/storage/root.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Dict, List, Optional
 
+from google.cloud.firestore_v1 import DocumentSnapshot
+
 from aipkgs_firebase.storage.core import FirebaseStorageCore
 from aipkgs_firebase.storage.helpers import FirebaseStorageHelper
 
 
 class FirebaseRootModel:
     collection_name = ""
 
@@ -62,14 +64,19 @@
     def create_document(self, dictionary: dict, document_id: str = None) -> bool:
         return FirebaseStorageCore.create_document_from_data(
             dictionary_data=dictionary,
             collection_name=self.collection_name,
             document_id=document_id,
         )
 
+    def create_document_from_snapshot(self, snapshot: DocumentSnapshot):
+        return FirebaseStorageCore.create_document_from_snapshot(
+            collection_name=self.collection_name, snapshot=snapshot
+        )
+
     def update(self, dictionary: dict, document_id: str):
         FirebaseStorageCore.update_document_with_data(
             dictionary_data=dictionary,
             collection_name=self.collection_name,
             document_id=document_id,
         )
```

### Comparing `aipkgs_firebase-1.0.8/aipkgs_firebase/user/core.py` & `aipkgs_firebase-1.0.9/aipkgs_firebase/user/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.8/pyproject.toml` & `aipkgs_firebase-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["poetry-core>=1.0.8"]
+requires = ["poetry-core>=1.0.9"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aipkgs-firebase"
-version = "1.0.8"
+version = "1.0.9"
 description = "A utility package for interacting with Firebase, specifically Firestore, in a more streamlined and efficient manner."
 authors = ["Alexy <alexy.ib@outlook.com>"]
 # New attributes
 license = "MIT"
 readme = "README.rst"
 homepage = "https://gitlab.com/aipy/public/packages.git"
 repository = "https://gitlab.com/aipy/public/packages.git"
```

### Comparing `aipkgs_firebase-1.0.8/PKG-INFO` & `aipkgs_firebase-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipkgs-firebase
-Version: 1.0.8
+Version: 1.0.9
 Summary: A utility package for interacting with Firebase, specifically Firestore, in a more streamlined and efficient manner.
 Home-page: https://gitlab.com/aipy/public/packages.git
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
 Requires-Python: >=3.11.3,<4.0.0
```

