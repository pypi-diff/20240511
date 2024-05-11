# Comparing `tmp/aipkgs_firebase-0.0.8.tar.gz` & `tmp/aipkgs_firebase-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_firebase-0.0.8.tar", max compression
+gzip compressed data, was "aipkgs_firebase-0.0.9.tar", max compression
```

## Comparing `aipkgs_firebase-0.0.8.tar` & `aipkgs_firebase-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.928787 aipkgs_firebase-0.0.8/LICENSE.md
--rw-r--r--   0        0        0       13 2022-03-08 13:06:48.929037 aipkgs_firebase-0.0.8/README.rst
--rw-r--r--   0        0        0       88 2022-03-08 13:06:48.928222 aipkgs_firebase-0.0.8/aipkgs_firebase/__init__.py
--rw-r--r--   0        0        0     2302 2023-11-26 13:02:33.501317 aipkgs_firebase-0.0.8/aipkgs_firebase/helpers.py
--rw-r--r--   0        0        0      136 2023-11-26 12:53:12.992955 aipkgs_firebase-0.0.8/aipkgs_firebase/messaging/__init__.py
--rw-r--r--   0        0        0     5155 2022-03-08 13:06:48.928493 aipkgs_firebase-0.0.8/aipkgs_firebase/messaging/core.py
--rw-r--r--   0        0        0       74 2022-03-08 13:06:48.928579 aipkgs_firebase-0.0.8/aipkgs_firebase/messaging/enums.py
--rw-r--r--   0        0        0     2474 2022-03-08 13:06:48.928861 aipkgs_firebase-0.0.8/aipkgs_firebase/messaging/helpers.py
--rw-r--r--   0        0        0     4215 2023-11-26 13:02:21.871322 aipkgs_firebase-0.0.8/aipkgs_firebase/storage/core.py
--rw-r--r--   0        0        0     2501 2023-11-26 12:59:30.711356 aipkgs_firebase-0.0.8/aipkgs_firebase/storage/helpers.py
--rw-r--r--   0        0        0     2511 2023-11-26 12:59:11.574625 aipkgs_firebase-0.0.8/aipkgs_firebase/storage/root.py
--rw-r--r--   0        0        0      571 2024-05-08 14:08:14.528442 aipkgs_firebase-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 aipkgs_firebase-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.928787 aipkgs_firebase-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0       13 2022-03-08 13:06:48.929037 aipkgs_firebase-0.0.9/README.rst
+-rw-r--r--   0        0        0       88 2022-03-08 13:06:48.928222 aipkgs_firebase-0.0.9/aipkgs_firebase/__init__.py
+-rw-r--r--   0        0        0     2302 2023-11-26 13:02:33.501317 aipkgs_firebase-0.0.9/aipkgs_firebase/helpers.py
+-rw-r--r--   0        0        0      136 2023-11-26 12:53:12.992955 aipkgs_firebase-0.0.9/aipkgs_firebase/messaging/__init__.py
+-rw-r--r--   0        0        0     5155 2022-03-08 13:06:48.928493 aipkgs_firebase-0.0.9/aipkgs_firebase/messaging/core.py
+-rw-r--r--   0        0        0       74 2022-03-08 13:06:48.928579 aipkgs_firebase-0.0.9/aipkgs_firebase/messaging/enums.py
+-rw-r--r--   0        0        0     2474 2022-03-08 13:06:48.928861 aipkgs_firebase-0.0.9/aipkgs_firebase/messaging/helpers.py
+-rw-r--r--   0        0        0     4215 2023-11-26 13:02:21.871322 aipkgs_firebase-0.0.9/aipkgs_firebase/storage/core.py
+-rw-r--r--   0        0        0     2723 2024-05-09 11:42:43.751124 aipkgs_firebase-0.0.9/aipkgs_firebase/storage/helpers.py
+-rw-r--r--   0        0        0     2689 2024-05-09 11:43:09.034133 aipkgs_firebase-0.0.9/aipkgs_firebase/storage/root.py
+-rw-r--r--   0        0        0      571 2024-05-09 11:44:08.800804 aipkgs_firebase-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 aipkgs_firebase-0.0.9/PKG-INFO
```

### Comparing `aipkgs_firebase-0.0.8/LICENSE.md` & `aipkgs_firebase-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-0.0.8/aipkgs_firebase/helpers.py` & `aipkgs_firebase-0.0.9/aipkgs_firebase/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-0.0.8/aipkgs_firebase/messaging/core.py` & `aipkgs_firebase-0.0.9/aipkgs_firebase/messaging/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-0.0.8/aipkgs_firebase/messaging/helpers.py` & `aipkgs_firebase-0.0.9/aipkgs_firebase/messaging/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-0.0.8/aipkgs_firebase/storage/core.py` & `aipkgs_firebase-0.0.9/aipkgs_firebase/storage/core.py`

 * *Files identical despite different names*

### Comparing `aipkgs_firebase-0.0.8/aipkgs_firebase/storage/helpers.py` & `aipkgs_firebase-0.0.9/aipkgs_firebase/storage/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 from typing import Dict, List, Optional
 
 from aipkgs_firebase.storage import core
 
 
 # Use the application default credentials
 
+def document_exists(collection_name: str, filters: Dict[str, any]) -> bool:
+    docs = core.get_documents(
+        collection_name=collection_name, filters=filters
+    )
+
+    if docs:
+        return True
+
+    return False
 
 def get_document(collection_name: str, document_id: str) -> Optional[dict]:
     doc = core.get_document(
         collection_name=collection_name, document_id=document_id
     )
 
     if doc.exists:
```

### Comparing `aipkgs_firebase-0.0.8/aipkgs_firebase/storage/root.py` & `aipkgs_firebase-0.0.9/aipkgs_firebase/storage/root.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,19 @@
         self.collection_name = collection_name
 
     def exists(self, document_id: str) -> bool:
         return core.document_exists(
             collection_name=self.collection_name, document_id=document_id
         )
 
+    def exists_where(self, filters: Dict[str, any]) -> bool:
+        return helpers.document_exists(
+            collection_name=self.collection_name, filters=filters
+        )
+
     def get_document(self, document_id: str) -> dict:
         return helpers.get_document(
             collection_name=self.collection_name, document_id=document_id
         )
 
     def get_document_realtime(self, document_id: str, callback):
         def temp_callback(document):
```

### Comparing `aipkgs_firebase-0.0.8/pyproject.toml` & `aipkgs_firebase-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aipkgs-firebase"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["Alexy <alexy.ib@outlook.com>"]
 # New attributes
 license = "MIT"
 readme = "README.rst"
 homepage = "https://gitlab.com/aipy/public/packages.git"
 repository = "https://gitlab.com/aipy/public/packages.git"
```

### Comparing `aipkgs_firebase-0.0.8/PKG-INFO` & `aipkgs_firebase-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipkgs-firebase
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Home-page: https://gitlab.com/aipy/public/packages.git
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
 Requires-Python: >=3.11.3,<4.0.0
```

