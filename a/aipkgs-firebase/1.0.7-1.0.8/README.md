# Comparing `tmp/aipkgs_firebase-1.0.7.tar.gz` & `tmp/aipkgs_firebase-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_firebase-1.0.7.tar", max compression
+gzip compressed data, was "aipkgs_firebase-1.0.8.tar", max compression
```

## Comparing `aipkgs_firebase-1.0.7.tar` & `aipkgs_firebase-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1058 2024-05-09 12:25:47.460445 aipkgs_firebase-1.0.7/LICENSE.md
--rw-r--r--   0        0        0       13 2022-03-08 13:06:48.929037 aipkgs_firebase-1.0.7/README.rst
--rw-r--r--   0        0        0       88 2022-03-08 13:06:48.928222 aipkgs_firebase-1.0.7/aipkgs_firebase/__init__.py
--rw-r--r--   0        0        0     1737 2024-05-11 14:14:48.035567 aipkgs_firebase-1.0.7/aipkgs_firebase/actions/core.py
--rw-r--r--   0        0        0     2302 2023-11-26 13:02:33.501317 aipkgs_firebase-1.0.7/aipkgs_firebase/helpers.py
--rw-r--r--   0        0        0     5948 2024-05-10 18:18:59.859448 aipkgs_firebase-1.0.7/aipkgs_firebase/messaging/core.py
--rw-r--r--   0        0        0      132 2024-05-10 18:17:53.723527 aipkgs_firebase-1.0.7/aipkgs_firebase/messaging/enums.py
--rw-r--r--   0        0        0     3079 2024-05-10 18:46:13.123781 aipkgs_firebase-1.0.7/aipkgs_firebase/messaging/helpers.py
--rw-r--r--   0        0        0     6374 2024-05-11 18:36:56.285659 aipkgs_firebase-1.0.7/aipkgs_firebase/storage/core.py
--rw-r--r--   0        0        0     3644 2024-05-11 18:39:27.920304 aipkgs_firebase-1.0.7/aipkgs_firebase/storage/helpers.py
--rw-r--r--   0        0        0     3168 2024-05-11 18:15:23.035976 aipkgs_firebase-1.0.7/aipkgs_firebase/storage/root.py
--rw-r--r--   0        0        0     2314 2024-05-10 18:47:03.096540 aipkgs_firebase-1.0.7/aipkgs_firebase/user/core.py
--rw-r--r--   0        0        0      687 2024-05-11 18:39:41.838822 aipkgs_firebase-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 aipkgs_firebase-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-09 12:25:47.460445 aipkgs_firebase-1.0.8/LICENSE.md
+-rw-r--r--   0        0        0       13 2022-03-08 13:06:48.929037 aipkgs_firebase-1.0.8/README.rst
+-rw-r--r--   0        0        0       88 2022-03-08 13:06:48.928222 aipkgs_firebase-1.0.8/aipkgs_firebase/__init__.py
+-rw-r--r--   0        0        0     1737 2024-05-11 14:14:48.035567 aipkgs_firebase-1.0.8/aipkgs_firebase/actions/core.py
+-rw-r--r--   0        0        0     2302 2023-11-26 13:02:33.501317 aipkgs_firebase-1.0.8/aipkgs_firebase/helpers.py
+-rw-r--r--   0        0        0     5948 2024-05-10 18:18:59.859448 aipkgs_firebase-1.0.8/aipkgs_firebase/messaging/core.py
+-rw-r--r--   0        0        0      132 2024-05-10 18:17:53.723527 aipkgs_firebase-1.0.8/aipkgs_firebase/messaging/enums.py
+-rw-r--r--   0        0        0     3079 2024-05-10 18:46:13.123781 aipkgs_firebase-1.0.8/aipkgs_firebase/messaging/helpers.py
+-rw-r--r--   0        0        0     7029 2024-05-11 19:20:36.361037 aipkgs_firebase-1.0.8/aipkgs_firebase/storage/core.py
+-rw-r--r--   0        0        0     3644 2024-05-11 18:39:27.920304 aipkgs_firebase-1.0.8/aipkgs_firebase/storage/helpers.py
+-rw-r--r--   0        0        0     3168 2024-05-11 18:15:23.035976 aipkgs_firebase-1.0.8/aipkgs_firebase/storage/root.py
+-rw-r--r--   0        0        0     2314 2024-05-10 18:47:03.096540 aipkgs_firebase-1.0.8/aipkgs_firebase/user/core.py
+-rw-r--r--   0        0        0      687 2024-05-11 19:21:22.254652 aipkgs_firebase-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 aipkgs_firebase-1.0.8/PKG-INFO
```

### Comparing `aipkgs_firebase-1.0.7/LICENSE.md` & `aipkgs_firebase-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.7/aipkgs_firebase/actions/core.py` & `aipkgs_firebase-1.0.8/aipkgs_firebase/actions/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.7/aipkgs_firebase/helpers.py` & `aipkgs_firebase-1.0.8/aipkgs_firebase/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.7/aipkgs_firebase/messaging/core.py` & `aipkgs_firebase-1.0.8/aipkgs_firebase/messaging/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.7/aipkgs_firebase/messaging/helpers.py` & `aipkgs_firebase-1.0.8/aipkgs_firebase/messaging/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.7/aipkgs_firebase/storage/core.py` & `aipkgs_firebase-1.0.8/aipkgs_firebase/storage/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # https://firebase.google.com/docs/firestore
 
 from datetime import datetime
 import threading
 from typing import Dict, List
 
 import firebase_admin
-from google.cloud.firestore_v1 import FieldFilter, CollectionReference, DocumentReference
+from google.cloud.firestore_v1 import FieldFilter, CollectionReference, DocumentReference, DocumentSnapshot
 
 from aipkgs_firebase import helpers
 
 
 class FirebaseStorageCore:
     @staticmethod
     def collection_ref(
@@ -37,15 +37,15 @@
             return True
 
         return False
 
     @staticmethod
     def get_document(
             collection_name: str, document_id: str
-    ) -> firebase_admin.firestore.firestore.DocumentSnapshot:
+    ) -> DocumentSnapshot:
         doc_ref = FirebaseStorageCore.document_ref(
             collection_name=collection_name, document_id=document_id)
         doc = doc_ref.get()
 
         return doc
 
     @staticmethod
@@ -65,81 +65,103 @@
         doc_watch = doc_ref.on_snapshot(on_snapshot)
 
         return doc_watch
 
     @staticmethod
     def get_documents(
             collection_name: str, filters: Dict[str, any] = None
-    ) -> List[firebase_admin.firestore.firestore.DocumentSnapshot]:
+    ) -> List[DocumentSnapshot]:
         col_ref = FirebaseStorageCore.collection_ref(collection_name=collection_name)
         if filters:
             for key, value in filters.items():
                 col_ref = col_ref.where(filter=FieldFilter(field_path=f"{key}", op_string="==", value=value))
 
         docs = col_ref.get()
 
         return docs
 
-    # @staticmethod
-    # def create_document_from_data(
-    #         dictionary_data: dict, collection_name: str, document_id: str = None
-    # ) -> bool:
-    #     data = dictionary_data
-    #
-    #     now = datetime.now()
-    #     timestamp = now.strftime("%d-%m-%Y %I:%M:%S %p")
-    #     data["timestamp"] = firebase_admin.firestore.SERVER_TIMESTAMP
-    #     data["created_at"] = timestamp
-    #
-    #     # current_time = time.time()
-    #     if document_id is not None:
-    #         # If the document ID is provided, use it to create or update the document
-    #         if not FirebaseStorageCore.document_exists(
-    #                 collection_name=collection_name, document_id=document_id
-    #         ):
-    #             doc_ref = FirebaseStorageCore.document_ref(
-    #                 collection_name=collection_name, document_id=document_id
-    #             )
-    #             data["document_id"] = document_id  # Add document_id to data
-    #             doc_ref.set(data, merge=True)
-    #             return True
-    #     else:
-    #         # If no document ID is provided, let Firestore generate one
-    #         doc_ref = FirebaseStorageCore.collection_ref(
-    #             collection_name=collection_name
-    #         ).document()
-    #
-    #         document_id = doc_ref.id  # Get the auto-generated document ID
-    #         data["document_id"] = document_id  # Update data with the generated document ID
-    #         doc_ref.set(data, merge=False)
-    #
-    #         # doc_ref.set(data, merge=True)  # Resave the data with the document ID included
-    #
-    #         return True
-    #
-    #     return False
-
     @staticmethod
-    def create_collection_in_collection(
-            root_collection_name: str, sub_collection_name:str, dictionary_data: dict, document_id: str = None):
+    def create_document_from_data(
+            dictionary_data: dict, collection_name: str, document_id: str = None
+    ) -> bool:
         data = dictionary_data
 
         now = datetime.now()
         timestamp = now.strftime("%d-%m-%Y %I:%M:%S %p")
         data["timestamp"] = firebase_admin.firestore.SERVER_TIMESTAMP
         data["created_at"] = timestamp
 
+        # current_time = time.time()
         if document_id is not None:
+            # If the document ID is provided, use it to create or update the document
             if not FirebaseStorageCore.document_exists(
-                    collection_name=root_collection_name, document_id=document_id
+                    collection_name=collection_name, document_id=document_id
             ):
                 doc_ref = FirebaseStorageCore.document_ref(
-                    collection_name=root_collection_name, document_id=document_id
+                    collection_name=collection_name, document_id=document_id
                 )
-                data["document_id"] = document_id
+                data["document_id"] = document_id  # Add document_id to data
+                doc_ref.set(data, merge=True)
+                return True
+        else:
+            # If no document ID is provided, let Firestore generate one
+            doc_ref = FirebaseStorageCore.collection_ref(
+                collection_name=collection_name
+            ).document()
+
+            document_id = doc_ref.id  # Get the auto-generated document ID
+            data["document_id"] = document_id  # Update data with the generated document ID
+            doc_ref.set(data, merge=False)
+
+            # doc_ref.set(data, merge=True)  # Resave the data with the document ID included
+
+            return True
+
+        return False
+
+    @staticmethod
+    def create_document_from_snapshot(
+            collection_name: str, document: DocumentSnapshot
+    ):
+        data = document.to_dict()
+
+        now = datetime.now()
+        timestamp = now.strftime("%d-%m-%Y %I:%M:%S %p")
+        data["timestamp"] = firebase_admin.firestore.SERVER_TIMESTAMP
+        data["created_at"] = timestamp
+
+        document_id = document.id
+
+        if not FirebaseStorageCore.document_exists(
+                collection_name=collection_name, document_id=document_id
+        ):
+            doc_ref = FirebaseStorageCore.document_ref(
+                collection_name=collection_name, document_id=document_id
+            )
+            data["document_id"] = document_id
+            doc_ref.set(data, merge=True)
+
+    # @staticmethod
+    # def create_collection_in_collection(
+    #         root_collection_name: str, sub_collection_name:str, dictionary_data: dict, document_id: str = None):
+    #     data = dictionary_data
+    #
+    #     now = datetime.now()
+    #     timestamp = now.strftime("%d-%m-%Y %I:%M:%S %p")
+    #     data["timestamp"] = firebase_admin.firestore.SERVER_TIMESTAMP
+    #     data["created_at"] = timestamp
+    #
+    #     if document_id is not None:
+    #         if not FirebaseStorageCore.document_exists(
+    #                 collection_name=root_collection_name, document_id=document_id
+    #         ):
+    #             doc_ref = FirebaseStorageCore.document_ref(
+    #                 collection_name=root_collection_name, document_id=document_id
+    #             )
+    #             data["document_id"] = document_id
 
     @staticmethod
     def update_document_with_data(
             dictionary_data: dict, collection_name: str, document_id: str
     ):
         data = dictionary_data
```

### Comparing `aipkgs_firebase-1.0.7/aipkgs_firebase/storage/helpers.py` & `aipkgs_firebase-1.0.8/aipkgs_firebase/storage/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.7/aipkgs_firebase/storage/root.py` & `aipkgs_firebase-1.0.8/aipkgs_firebase/storage/root.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.7/aipkgs_firebase/user/core.py` & `aipkgs_firebase-1.0.8/aipkgs_firebase/user/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-1.0.7/pyproject.toml` & `aipkgs_firebase-1.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["poetry-core>=1.0.7"]
+requires = ["poetry-core>=1.0.8"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aipkgs-firebase"
-version = "1.0.7"
+version = "1.0.8"
 description = "A utility package for interacting with Firebase, specifically Firestore, in a more streamlined and efficient manner."
 authors = ["Alexy <alexy.ib@outlook.com>"]
 # New attributes
 license = "MIT"
 readme = "README.rst"
 homepage = "https://gitlab.com/aipy/public/packages.git"
 repository = "https://gitlab.com/aipy/public/packages.git"
```

### Comparing `aipkgs_firebase-1.0.7/PKG-INFO` & `aipkgs_firebase-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipkgs-firebase
-Version: 1.0.7
+Version: 1.0.8
 Summary: A utility package for interacting with Firebase, specifically Firestore, in a more streamlined and efficient manner.
 Home-page: https://gitlab.com/aipy/public/packages.git
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
 Requires-Python: >=3.11.3,<4.0.0
```

