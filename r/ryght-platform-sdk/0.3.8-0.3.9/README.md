# Comparing `tmp/ryght_platform_sdk-0.3.8.tar.gz` & `tmp/ryght_platform_sdk-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryght_platform_sdk-0.3.8.tar", max compression
+gzip compressed data, was "ryght_platform_sdk-0.3.9.tar", max compression
```

## Comparing `ryght_platform_sdk-0.3.8.tar` & `ryght_platform_sdk-0.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       16 2024-02-02 11:03:05.872282 ryght_platform_sdk-0.3.8/README.md
--rw-r--r--   0        0        0      645 2024-03-28 19:16:30.588596 ryght_platform_sdk-0.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-13 18:28:11.113560 ryght_platform_sdk-0.3.8/src/ryght/__init__.py
--rw-r--r--   0        0        0       58 2024-03-13 05:48:02.731588 ryght_platform_sdk-0.3.8/src/ryght/clients/__init__.py
--rw-r--r--   0        0        0    12961 2024-03-28 19:14:24.776974 ryght_platform_sdk-0.3.8/src/ryght/clients/api.py
--rw-r--r--   0        0        0     4655 2024-03-26 22:13:47.025119 ryght_platform_sdk-0.3.8/src/ryght/clients/user.py
--rw-r--r--   0        0        0     2011 2024-03-21 11:17:01.513468 ryght_platform_sdk-0.3.8/src/ryght/configs/__init__.py
--rw-r--r--   0        0        0     8357 2024-03-28 15:13:48.761560 ryght_platform_sdk-0.3.8/src/ryght/configs/api_config.py
--rw-r--r--   0        0        0     3182 2024-03-25 16:52:52.483525 ryght_platform_sdk-0.3.8/src/ryght/configs/api_endpoints.yaml
--rw-r--r--   0        0        0       61 2024-03-13 05:43:00.067020 ryght_platform_sdk-0.3.8/src/ryght/interface/__init__.py
--rw-r--r--   0        0        0     5340 2024-03-20 17:55:57.727098 ryght_platform_sdk-0.3.8/src/ryght/interface/api.py
--rw-r--r--   0        0        0     6379 2024-03-26 22:21:53.881553 ryght_platform_sdk-0.3.8/src/ryght/interface/client.py
--rw-r--r--   0        0        0       77 2024-02-13 18:28:11.115970 ryght_platform_sdk-0.3.8/src/ryght/managers/__init__.py
--rw-r--r--   0        0        0     1656 2024-03-26 22:18:22.520369 ryght_platform_sdk-0.3.8/src/ryght/managers/collections.py
--rw-r--r--   0        0        0     8368 2024-03-20 11:19:15.859848 ryght_platform_sdk-0.3.8/src/ryght/managers/tokens.py
--rw-r--r--   0        0        0      297 2024-03-09 12:48:07.301267 ryght_platform_sdk-0.3.8/src/ryght/models/__init__.py
--rw-r--r--   0        0        0     8970 2024-03-25 17:48:34.446053 ryght_platform_sdk-0.3.8/src/ryght/models/data_models.py
--rw-r--r--   0        0        0       49 2024-02-13 18:28:11.117875 ryght_platform_sdk-0.3.8/src/ryght/requests/__init__.py
--rw-r--r--   0        0        0     3101 2024-03-14 14:41:30.204889 ryght_platform_sdk-0.3.8/src/ryght/requests/http_requestor.py
--rw-r--r--   0        0        0     3845 2024-02-19 11:54:44.707024 ryght_platform_sdk-0.3.8/src/ryght/utils/__init__.py
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 ryght_platform_sdk-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-02-02 11:03:05.872282 ryght_platform_sdk-0.3.9/README.md
+-rw-r--r--   0        0        0      645 2024-04-16 13:29:47.840381 ryght_platform_sdk-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-13 18:28:11.113560 ryght_platform_sdk-0.3.9/src/ryght/__init__.py
+-rw-r--r--   0        0        0       58 2024-03-13 05:48:02.731588 ryght_platform_sdk-0.3.9/src/ryght/clients/__init__.py
+-rw-r--r--   0        0        0    13731 2024-04-11 12:45:53.149466 ryght_platform_sdk-0.3.9/src/ryght/clients/api.py
+-rw-r--r--   0        0        0     4655 2024-03-26 22:13:47.025119 ryght_platform_sdk-0.3.9/src/ryght/clients/user.py
+-rw-r--r--   0        0        0     2011 2024-03-21 11:17:01.513468 ryght_platform_sdk-0.3.9/src/ryght/configs/__init__.py
+-rw-r--r--   0        0        0     8445 2024-04-11 11:55:48.842899 ryght_platform_sdk-0.3.9/src/ryght/configs/api_config.py
+-rw-r--r--   0        0        0     3371 2024-04-11 11:10:56.796829 ryght_platform_sdk-0.3.9/src/ryght/configs/api_endpoints.yaml
+-rw-r--r--   0        0        0       88 2024-04-11 11:51:25.612490 ryght_platform_sdk-0.3.9/src/ryght/interface/__init__.py
+-rw-r--r--   0        0        0    11692 2024-04-11 17:05:43.131179 ryght_platform_sdk-0.3.9/src/ryght/interface/api.py
+-rw-r--r--   0        0        0     6562 2024-04-12 10:14:53.527141 ryght_platform_sdk-0.3.9/src/ryght/interface/client.py
+-rw-r--r--   0        0        0       77 2024-02-13 18:28:11.115970 ryght_platform_sdk-0.3.9/src/ryght/managers/__init__.py
+-rw-r--r--   0        0        0     1656 2024-03-26 22:18:22.520369 ryght_platform_sdk-0.3.9/src/ryght/managers/collections.py
+-rw-r--r--   0        0        0     8368 2024-03-20 11:19:15.859848 ryght_platform_sdk-0.3.9/src/ryght/managers/tokens.py
+-rw-r--r--   0        0        0      358 2024-04-11 16:37:01.105926 ryght_platform_sdk-0.3.9/src/ryght/models/__init__.py
+-rw-r--r--   0        0        0    13601 2024-04-11 16:39:20.898144 ryght_platform_sdk-0.3.9/src/ryght/models/data_models.py
+-rw-r--r--   0        0        0       49 2024-02-13 18:28:11.117875 ryght_platform_sdk-0.3.9/src/ryght/requests/__init__.py
+-rw-r--r--   0        0        0     3101 2024-03-14 14:41:30.204889 ryght_platform_sdk-0.3.9/src/ryght/requests/http_requestor.py
+-rw-r--r--   0        0        0     4059 2024-04-11 16:51:40.492742 ryght_platform_sdk-0.3.9/src/ryght/utils/__init__.py
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 ryght_platform_sdk-0.3.9/PKG-INFO
```

### Comparing `ryght_platform_sdk-0.3.8/pyproject.toml` & `ryght_platform_sdk-0.3.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ryght-platform-sdk"
-version = "0.3.8"
+version = "0.3.9"
 description = "A SDk to use the Ryght Platform features"
 authors = ["sudo-ai"]
 readme = "README.md"
 packages = [{include="ryght", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11.7"
```

### Comparing `ryght_platform_sdk-0.3.8/src/ryght/clients/api.py` & `ryght_platform_sdk-0.3.9/src/ryght/clients/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,23 @@
 # -------------------------------------------------------------------------------------------------------------------- #
 # <---| * Import section |--->
 # -------------------------------------------------------------------------------------------------------------------- #
 import json
 import logging
 import os.path
 from urllib.parse import urljoin
+from urllib.parse import urlencode
 
-from ryght.interface import ApiInterface
 from ryght.utils import RequestMethods, FlowTypes, ModelOperation
+
+from ryght.interface import (
+    ApiInterface,
+    Conversations
+)
+
 from ryght.models import (
     Collection,
     AIModels,
     Documents,
     TraceStatus,
     JsonDocument,
     CompletionsResponse,
@@ -36,17 +42,17 @@
 # -------------------------------------------------------------------------------------------------------------------- #
 logger = logging.getLogger(__name__)
 
 
 # -------------------------------------------------------------------------------------------------------------------- #
 # <---| * Class Definition |--->
 # -------------------------------------------------------------------------------------------------------------------- #
-class ApiClient(ApiInterface):
-    def get_headers(self):
-        return {'Authorization': self.token_manager.token.authorization_param}
+class ApiClient(
+    Conversations
+):
 
     # Document Collections
     def get_collection_page_by_page(self, param: dict = None):
         raise NotImplementedError(f'Get collections page by page not implemented !')
 
     # Document Collection
 
@@ -68,22 +74,32 @@
                 'name': collection_name,
                 'metadata': metadata,
                 'tagIds': tag_ids if tag_ids else []
             })
         )
         return result.get('id')
 
-    def search_collections(self, param: dict = None) -> list[Collection]:
+    def get_all_available_collections(self) -> list[Collection]:
+        return self.search_collections(
+            query_params={
+                'size': 100
+            }
+        )
+
+    def search_collections(self, query_params: dict = None) -> list[Collection]:
         logger.debug(f'Getting available collections ...')
         url = urljoin(self.api_endpoints.base_url, self.api_endpoints.document_collection.search)
+        if isinstance(query_params, dict):
+            url = urljoin(url, '?' + urlencode(query_params))
+            print(url)
         result = self.execute_request(
             method=RequestMethods.GET,
             url=url,
             headers=self.get_headers(),
-            params=param
+            timeout=10.0
         )
         collections = []
         if 'content' in result:
             for collection_details in result['content']:
                 collections.append(Collection(**collection_details))
         return collections
 
@@ -95,14 +111,26 @@
             method=RequestMethods.GET,
             url=url,
             headers=self.get_headers()
         )
 
         return Collection(**result)
 
+    def delete_collection_by_id(self, collection_id: str) -> str:
+        logger.debug(f"Request a collection deletion by collection id ...")
+        url = urljoin(self.api_endpoints.base_url, self.api_endpoints.document_collection.by_id)
+        url = url.format(id=collection_id)
+        result: str = self.execute_request(
+            method=RequestMethods.DELETE,
+            url=url,
+            headers=self.get_headers()
+        )
+
+        return result
+
     def upload_chunked_document_collection(self, document_collection: ChunkedDocumentCollection) -> str:
         logger.debug(f'Create/update chunked document collection')
         url = urljoin(self.api_endpoints.base_url, self.api_endpoints.document_collection.pre_chunked)
         headers = self.get_headers()
         headers['Content-Type'] = 'application/json'
         result = self.execute_request(
             method=RequestMethods.POST,
@@ -177,15 +205,15 @@
             self,
             input_str: str,
             collection_ids: str | list[str],
             flow: FlowTypes = FlowTypes.SEARCH,
             search_limit: int = 5,
             completion_model_id: str = None,
             embedding_model_id: str = None,
-            document_ids: list | None = None
+            document_ids: list[str] | None = None
     ) -> CompletionsResponse:
         logger.debug(f'Performing completions ... ')
         url = urljoin(self.api_endpoints.base_url, self.api_endpoints.completions.base)
         payload = {
             "question": input_str,
             "flow": flow.value if isinstance(flow, FlowTypes) else None,
             "collectionIds": collection_ids if isinstance(collection_ids, list) else [collection_ids],
@@ -327,14 +355,16 @@
         result = self.execute_request(
             method=RequestMethods.DELETE,
             url=url,
             headers=self.get_headers()
         )
         return result
 
+    # permission
+
     # Notes
     def search_notes(self, filter_params: dict = None):
         pass
 
     def get_note_by_id(self, note_id: str):
         pass
```

### Comparing `ryght_platform_sdk-0.3.8/src/ryght/clients/user.py` & `ryght_platform_sdk-0.3.9/src/ryght/clients/user.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.8/src/ryght/configs/__init__.py` & `ryght_platform_sdk-0.3.9/src/ryght/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.8/src/ryght/configs/api_config.py` & `ryght_platform_sdk-0.3.9/src/ryght/configs/api_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,19 +152,20 @@
     json_object: str = Field(..., description="")
 
 
 # -------------------------------------------------------------------------------------------------------------------- #
 class PermissionManagementEndpoint(BaseModel):
     model_config = ConfigDict(extra='ignore')
 
-    group: str = Field(..., description="")
-    users: str = Field(..., description="")
+    for_users: str = Field(..., description="")
     resources: str = Field(..., description="")
-    find_groups: str = Field(..., description="")
+    for_members: str = Field(..., description="")
     permissions: str = Field(..., description="")
+    permissions_users_in_org: str = Field(..., description="")
+    permissions_members_of_org: str = Field(..., description="")
 
 
 # -------------------------------------------------------------------------------------------------------------------- #
 class ApiEndpoints(BaseModel):
     model_config = ConfigDict(
         extra='ignore',
         protected_namespaces=()
```

### Comparing `ryght_platform_sdk-0.3.8/src/ryght/configs/api_endpoints.yaml` & `ryght_platform_sdk-0.3.9/src/ryght/configs/api_endpoints.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -81,12 +81,14 @@
 
         document_import:
             status: /document-import/v1/documents/status/{traceId}
             json_object: /document-import/v1/documents/collections/{collectionId}
             pdf_file: /document-import/v1/documents/collections/{collectionId}/files
 
         permission_management:
-            find_groups: /v1/managements/groups
             resources: /v1/managements/resources
-            users: /v1/managements/permissions/users
             permissions: /v1/managements/permissions
-            group: /v1/managements/permissions/{group}/members
+            for_users: /v1/management/permissions/organizations/users
+            for_members: /v1/management/permissions/organizations/members
+            permissions_users_in_org: /v1/management/permissions/organizations/{organizationId}/users
+            permissions_members_of_org: /v1/management/permissions/organizations/{organizationId}/members
+
```

### Comparing `ryght_platform_sdk-0.3.8/src/ryght/interface/client.py` & `ryght_platform_sdk-0.3.9/src/ryght/interface/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
             self.api_client.token_manager.credentials = user_credentials
         elif isinstance(user_credentials, str) and os.path.isfile(user_credentials):
             credentials = Credentials(_env_file=user_credentials)
             self.api_client.token_manager.credentials = credentials
 
         # Document Collection  ------->
 
-    def list_collections(self) -> list[Collection]:
-        return self.api_client.search_collections()
+    def list_collections(self, query_params: dict | None = None) -> list[Collection]:
+        return self.api_client.search_collections(query_params)
 
     def create_new_collection(
             self,
             collection_name: str,
             metadata: dict | None = None,
             tag_ids: list[str] | None = None
     ) -> str:
@@ -83,14 +83,17 @@
             metadata,
             tag_ids
         )
 
     def get_collection_by_id(self, collection_id: str) -> Collection:
         return self.api_client.get_collection_details(collection_id)
 
+    def delete_collection_by_id(self, collection_id: str) -> str:
+        return self.api_client.delete_collection_by_id(collection_id)
+
     # Document import to a collection ----->
     def upload_a_new_doc_to_collection(
             self,
             collection_id: str,
             document: JsonDocument
     ) -> str:
         return self.api_client.upload_doc_as_json_to_a_document_collection(
```

### Comparing `ryght_platform_sdk-0.3.8/src/ryght/managers/collections.py` & `ryght_platform_sdk-0.3.9/src/ryght/managers/collections.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.8/src/ryght/managers/tokens.py` & `ryght_platform_sdk-0.3.9/src/ryght/managers/tokens.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.8/src/ryght/requests/http_requestor.py` & `ryght_platform_sdk-0.3.9/src/ryght/requests/http_requestor.py`

 * *Files identical despite different names*

### Comparing `ryght_platform_sdk-0.3.8/src/ryght/utils/__init__.py` & `ryght_platform_sdk-0.3.9/src/ryght/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,20 @@
     COMPLETION = "COMPLETION"
     TRANSLATION = "TRANSLATION"
     SUMMARIZATION = "SUMMARIZATION"
     TEXT_GENERATION = "TEXT_GENERATION"
 
 
 # -------------------------------------------------------------------------------------------------------------------- #
+class QnARating(enum.StrEnum):
+    THUMBS_UP = "THUMBS_UP"
+    THUMBS_DOWN = "THUMBS_DOWN"
+
+
+# -------------------------------------------------------------------------------------------------------------------- #
 def set_logging_format(new_format):
     for handler in logging.root.handlers:
         handler.setFormatter(logging.Formatter(new_format))
 
 
 # -------------------------------------------------------------------------------------------------------------------- #
```

### Comparing `ryght_platform_sdk-0.3.8/PKG-INFO` & `ryght_platform_sdk-0.3.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryght-platform-sdk
-Version: 0.3.8
+Version: 0.3.9
 Summary: A SDk to use the Ryght Platform features
 Author: sudo-ai
 Requires-Python: >=3.11.7,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
```

