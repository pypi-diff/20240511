# Comparing `tmp/dingodb-0.0.8.tar.gz` & `tmp/dingodb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingodb-0.0.8.tar", last modified: Tue Sep 26 03:58:39 2023, max compression
+gzip compressed data, was "dingodb-0.0.9.tar", last modified: Wed Sep 27 11:06:50 2023, max compression
```

## Comparing `dingodb-0.0.8.tar` & `dingodb-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-09-26 03:58:39.656370 dingodb-0.0.8/
--rw-rw-r--   0 gary      (1000) gary      (1000)    11357 2023-08-01 03:44:49.000000 dingodb-0.0.8/LICENSE
--rw-rw-r--   0 gary      (1000) gary      (1000)       72 2023-07-20 09:31:54.000000 dingodb-0.0.8/MANIFEST.in
--rw-rw-r--   0 gary      (1000) gary      (1000)     5960 2023-09-26 03:58:39.656370 dingodb-0.0.8/PKG-INFO
--rw-rw-r--   0 gary      (1000) gary      (1000)     4584 2023-09-08 06:07:06.000000 dingodb-0.0.8/README.md
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-09-26 03:58:39.652370 dingodb-0.0.8/dingodb/
--rw-rw-r--   0 gary      (1000) gary      (1000)       60 2023-07-20 09:31:54.000000 dingodb-0.0.8/dingodb/__init__.py
--rw-rw-r--   0 gary      (1000) gary      (1000)        6 2023-09-22 05:40:16.000000 dingodb-0.0.8/dingodb/__version__
--rw-rw-r--   0 gary      (1000) gary      (1000)     1636 2023-08-01 03:23:27.000000 dingodb-0.0.8/dingodb/config.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    14293 2023-09-26 02:56:19.000000 dingodb-0.0.8/dingodb/db.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     9348 2023-09-08 06:07:06.000000 dingodb-0.0.8/dingodb/dingo_param.py
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-09-26 03:58:39.656370 dingodb-0.0.8/dingodb/grpc/
--rw-rw-r--   0 gary      (1000) gary      (1000)       78 2023-08-16 02:03:36.000000 dingodb-0.0.8/dingodb/grpc/__init__.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     1890 2023-08-10 17:42:10.000000 dingodb-0.0.8/dingodb/grpc/grpc_config.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    18641 2023-09-22 06:00:24.000000 dingodb-0.0.8/dingodb/grpc/grpc_db.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     9300 2023-09-25 10:38:40.000000 dingodb-0.0.8/dingodb/grpc/grpc_dingo_param.py
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-09-26 03:58:39.656370 dingodb-0.0.8/dingodb/protos/
--rw-rw-r--   0 gary      (1000) gary      (1000)       63 2023-08-08 10:21:42.000000 dingodb-0.0.8/dingodb/protos/__init__.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    13469 2023-09-22 06:28:51.000000 dingodb-0.0.8/dingodb/protos/proxy_common_pb2.py
--rw-rw-r--   0 gary      (1000) gary      (1000)      159 2023-09-22 06:28:51.000000 dingodb-0.0.8/dingodb/protos/proxy_common_pb2_grpc.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     8403 2023-09-22 06:28:51.000000 dingodb-0.0.8/dingodb/protos/proxy_index_pb2.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    14046 2023-09-22 06:28:51.000000 dingodb-0.0.8/dingodb/protos/proxy_index_pb2_grpc.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     7022 2023-09-22 06:28:51.000000 dingodb-0.0.8/dingodb/protos/proxy_meta_pb2.py
--rw-rw-r--   0 gary      (1000) gary      (1000)    13724 2023-09-22 06:28:51.000000 dingodb-0.0.8/dingodb/protos/proxy_meta_pb2_grpc.py
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-09-26 03:58:39.652370 dingodb-0.0.8/dingodb.egg-info/
--rw-rw-r--   0 gary      (1000) gary      (1000)     5960 2023-09-26 03:58:39.000000 dingodb-0.0.8/dingodb.egg-info/PKG-INFO
--rw-rw-r--   0 gary      (1000) gary      (1000)      675 2023-09-26 03:58:39.000000 dingodb-0.0.8/dingodb.egg-info/SOURCES.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-09-26 03:58:39.000000 dingodb-0.0.8/dingodb.egg-info/dependency_links.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)      187 2023-09-26 03:58:39.000000 dingodb-0.0.8/dingodb.egg-info/requires.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        8 2023-09-26 03:58:39.000000 dingodb-0.0.8/dingodb.egg-info/top_level.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        0 2023-07-13 06:19:14.000000 dingodb-0.0.8/pyproject.toml
--rw-rw-r--   0 gary      (1000) gary      (1000)      195 2023-09-22 06:29:13.000000 dingodb-0.0.8/requirements.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       38 2023-09-26 03:58:39.656370 dingodb-0.0.8/setup.cfg
--rw-rw-r--   0 gary      (1000) gary      (1000)     1957 2023-08-31 08:57:42.000000 dingodb-0.0.8/setup.py
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-09-27 11:06:50.335643 dingodb-0.0.9/
+-rw-rw-r--   0 gary      (1000) gary      (1000)    11357 2023-08-01 03:44:49.000000 dingodb-0.0.9/LICENSE
+-rw-rw-r--   0 gary      (1000) gary      (1000)       72 2023-07-20 09:31:54.000000 dingodb-0.0.9/MANIFEST.in
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5960 2023-09-27 11:06:50.335643 dingodb-0.0.9/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)     4584 2023-09-08 06:07:06.000000 dingodb-0.0.9/README.md
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-09-27 11:06:50.335643 dingodb-0.0.9/dingodb/
+-rw-rw-r--   0 gary      (1000) gary      (1000)       60 2023-07-20 09:31:54.000000 dingodb-0.0.9/dingodb/__init__.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)        6 2023-09-27 10:57:34.000000 dingodb-0.0.9/dingodb/__version__
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1636 2023-08-01 03:23:27.000000 dingodb-0.0.9/dingodb/config.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    14529 2023-09-27 10:57:34.000000 dingodb-0.0.9/dingodb/db.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     9348 2023-09-08 06:07:06.000000 dingodb-0.0.9/dingodb/dingo_param.py
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-09-27 11:06:50.335643 dingodb-0.0.9/dingodb/grpc/
+-rw-rw-r--   0 gary      (1000) gary      (1000)       78 2023-08-16 02:03:36.000000 dingodb-0.0.9/dingodb/grpc/__init__.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1890 2023-08-10 17:42:10.000000 dingodb-0.0.9/dingodb/grpc/grpc_config.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    20187 2023-09-27 10:57:34.000000 dingodb-0.0.9/dingodb/grpc/grpc_db.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     9174 2023-09-27 10:57:34.000000 dingodb-0.0.9/dingodb/grpc/grpc_dingo_param.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    35664 2023-09-27 10:57:34.000000 dingodb-0.0.9/dingodb/grpc/json_format.py
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-09-27 11:06:50.335643 dingodb-0.0.9/dingodb/protos/
+-rw-rw-r--   0 gary      (1000) gary      (1000)       63 2023-08-08 10:21:42.000000 dingodb-0.0.9/dingodb/protos/__init__.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    14417 2023-09-27 10:57:34.000000 dingodb-0.0.9/dingodb/protos/proxy_common_pb2.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)      159 2023-09-27 10:03:02.000000 dingodb-0.0.9/dingodb/protos/proxy_common_pb2_grpc.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1453 2023-09-27 10:57:34.000000 dingodb-0.0.9/dingodb/protos/proxy_error_pb2.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)      159 2023-09-27 10:57:34.000000 dingodb-0.0.9/dingodb/protos/proxy_error_pb2_grpc.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     7853 2023-09-27 10:57:34.000000 dingodb-0.0.9/dingodb/protos/proxy_index_pb2.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    13955 2023-09-27 10:57:34.000000 dingodb-0.0.9/dingodb/protos/proxy_index_pb2_grpc.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     7691 2023-09-27 10:57:34.000000 dingodb-0.0.9/dingodb/protos/proxy_meta_pb2.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    13724 2023-09-27 10:03:02.000000 dingodb-0.0.9/dingodb/protos/proxy_meta_pb2_grpc.py
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-09-27 11:06:50.335643 dingodb-0.0.9/dingodb.egg-info/
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5960 2023-09-27 11:06:50.000000 dingodb-0.0.9/dingodb.egg-info/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)      776 2023-09-27 11:06:50.000000 dingodb-0.0.9/dingodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-09-27 11:06:50.000000 dingodb-0.0.9/dingodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)      187 2023-09-27 11:06:50.000000 dingodb-0.0.9/dingodb.egg-info/requires.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        8 2023-09-27 11:06:50.000000 dingodb-0.0.9/dingodb.egg-info/top_level.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        0 2023-07-13 06:19:14.000000 dingodb-0.0.9/pyproject.toml
+-rw-rw-r--   0 gary      (1000) gary      (1000)      195 2023-09-22 06:29:13.000000 dingodb-0.0.9/requirements.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       38 2023-09-27 11:06:50.339643 dingodb-0.0.9/setup.cfg
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1957 2023-08-31 08:57:42.000000 dingodb-0.0.9/setup.py
```

### Comparing `dingodb-0.0.8/LICENSE` & `dingodb-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dingodb-0.0.8/PKG-INFO` & `dingodb-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingodb
-Version: 0.0.8
+Version: 0.0.9
 Summary: dingodb is dingodb sdk
 Home-page: https://www.dingodb.com/
 Author: DingoDB
 Author-email: dingodb@zetyun.com
 License: Proprietary License
 Project-URL: Homepage, https://www.dingodb.com/
 Project-URL: Documentation, https://dingodb.readthedocs.io/en/latest/
```

### Comparing `dingodb-0.0.8/README.md` & `dingodb-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dingodb-0.0.8/dingodb/config.py` & `dingodb-0.0.9/dingodb/config.py`

 * *Files identical despite different names*

### Comparing `dingodb-0.0.8/dingodb/db.py` & `dingodb-0.0.9/dingodb/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,14 @@
 
     def close(self):
         self.session.close()
 
     def make_response(self, res, deal="default"):
         res_json = res.json()
         if res_json.get("status") == 200:
-            if deal == "vector_count":
-                res_data = res_json.get("data")
-                return res_data.get("currentCount") - res_data.get("deletedCount")
             return res_json.get("data")
         else:
             raise RuntimeError(res_json)
 
     def describe_index_info(self, index_name: str) -> dict:
         """
         describe_index_info index info
@@ -242,19 +239,36 @@
         Args:
             index_name (str): the name of in index
 
         Returns:
             int: count num
         """
         res = self.session.get(
+            f"{self.requestProto}{self.host[0]}{self.vectorApi}{index_name}/count",
+            headers=self.headers,
+        )
+
+        return self.make_response(res)
+
+    def vector_metrics(self, index_name: str):
+        """
+        vector_metrics metrics in index
+
+        Args:
+            index_name (str): the name of in index
+
+        Returns:
+            dict: metrics info
+        """
+        res = self.session.get(
             f"{self.requestProto}{self.host[0]}{self.vectorApi}{index_name}",
             headers=self.headers,
         )
 
-        return self.make_response(res, deal="vector_count")
+        return self.make_response(res)
 
     def vector_scan(
         self,
         index_name: str,
         start_id: int,
         max_count: int = 1000,
         is_reverse: bool = False,
```

### Comparing `dingodb-0.0.8/dingodb/dingo_param.py` & `dingodb-0.0.9/dingodb/dingo_param.py`

 * *Files identical despite different names*

### Comparing `dingodb-0.0.8/dingodb/grpc/grpc_config.py` & `dingodb-0.0.9/dingodb/grpc/grpc_config.py`

 * *Files identical despite different names*

### Comparing `dingodb-0.0.8/dingodb/grpc/grpc_db.py` & `dingodb-0.0.9/dingodb/grpc/grpc_db.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from dingodb.protos.proxy_common_pb2 import *
 from dingodb.protos.proxy_index_pb2 import *
 from dingodb.protos.proxy_index_pb2_grpc import *
 from dingodb.protos.proxy_meta_pb2 import *
 from dingodb.protos.proxy_meta_pb2_grpc import *
-from google.protobuf.json_format import MessageToDict, ParseDict
 
 import grpc
 from grpc._cython import cygrpc
 
 from .grpc_dingo_param import (
     CheckClintParam,
     CheckCreateIndexParam,
     CheckVectorAddParam,
     CheckVectorDeleteParam,
     CheckVectorGetParam,
     CheckVectorScanParam,
     CheckVectorSearchParam,
 )
 
+from .json_format import MessageToDict, MessageToJson, ParseDict
+
 
 class GrpcDingoDB:
     def __init__(self, host: list, timeout: int = 55000) -> None:
         CheckClintParam(host=host, timeout=timeout)
         self._get_channel(host, timeout)
         self.index_stub = IndexServiceStub(self._channel)
         self.meta_stub = MetaServiceStub(self._channel)
@@ -59,21 +60,22 @@
 
         describe_index_request = GetIndexRequest(
             schema_name="dingo", index_name=index_name
         )
 
         describe_index_response = self.meta_stub.GetIndex.future(describe_index_request)
 
-        describe_info = MessageToDict(
-            describe_index_response.result().definition,
-            including_default_value_fields=True,
-        )
-        describe_info.update({"autoIncrement": int(describe_info["autoIncrement"])})
-
-        return describe_info
+        if describe_index_response.result().error.errcode == 0:
+            describe_info = MessageToDict(
+                describe_index_response.result().definition,
+                including_default_value_fields=True,
+            )
+            return describe_info
+        else:
+            raise RuntimeError(describe_index_response.result().error.errmsg)
 
     def describe_index_info_all(self) -> dict:
         """
         describe_index_info index info
 
         Raises:
             RuntimeError: return error
@@ -83,27 +85,21 @@
         """
 
         describe_indexes_request = GetIndexesRequest(schema_name="dingo")
 
         describe_indexes_response = self.meta_stub.GetIndexes.future(
             describe_indexes_request
         )
-        return list(
-            map(
-                lambda definition: {
-                    **MessageToDict(definition, including_default_value_fields=True),
-                    "autoIncrement": int(
-                        MessageToDict(definition, including_default_value_fields=True)[
-                            "autoIncrement"
-                        ]
-                    ),
-                },
-                describe_indexes_response.result().definitions,
-            )
-        )
+        if describe_indexes_response.result().error.errcode == 0:
+            return [
+                MessageToDict(definition, including_default_value_fields=True)
+                for definition in describe_indexes_response.result().definitions
+            ]
+        else:
+            raise RuntimeError(describe_indexes_response.result().error.errmsg)
 
     def create_index(
         self,
         index_name: str,
         dimension: int,
         index_type: str = "hnsw",
         metric_type: str = "cosine",
@@ -174,15 +170,18 @@
                         params.index_config, VectorIndexParameter()
                     ),
                 ),
             ),
         )
         vec_create_response = self.meta_stub.CreateIndex.future(vec_create_request)
 
-        return vec_create_response.result().state
+        if vec_create_response.result().error.errcode == 0:
+            return vec_create_response.result().state
+        else:
+            raise RuntimeError(vec_create_response.result().error.errmsg)
 
     def update_index_max_element(self, index_name: str, max_element: int) -> bool:
         """
         update_index_max_element change index max element
 
         only for hnsw
 
@@ -200,16 +199,18 @@
         update_index_max_element_request = UpdateMaxElementsRequest(
             schema_name="dingo", index_name=index_name, max_elements=max_element
         )
 
         update_index_max_element_response = self.meta_stub.UpdateMaxElements.future(
             update_index_max_element_request
         )
-
-        return update_index_max_element_response.result().state
+        if update_index_max_element_response.result().error.errcode == 0:
+            return update_index_max_element_response.result().state
+        else:
+            raise RuntimeError(update_index_max_element_response.result().error.errmsg)
 
     def update_index(self, index_name: str, definition: dict) -> bool:
         """
         update_index_max_element change index max element
 
         only for hnsw
 
@@ -226,15 +227,18 @@
         # "name", "version", "index_partition", "replica", "index_parameter", "with_auto_increment", "auto_increment"
         update_index_request = UpdateIndexRequest(
             schema_name="dingo", definition=ParseDict(definition, IndexDefinition())
         )
 
         update_index_response = self.meta_stub.UpdateIndex.future(update_index_request)
 
-        return update_index_response.result().state
+        if update_index_response.result().error.errcode == 0:
+            return update_index_response.result().state
+        else:
+            raise RuntimeError(update_index_response.result().error.errmsg)
 
     def delete_index(self, index_name: str) -> bool:
         """
         delete_index del/drop index
 
         Args:
             index_name (str): the name of index
@@ -246,21 +250,22 @@
             bool: True/False
         """
         del_index_request = DeleteIndexRequest(
             schema_name="dingo", index_name=index_name
         )
 
         del_index_response = self.meta_stub.DeleteIndex.future(del_index_request)
-        return del_index_response.result().state
+        if del_index_response.result().error.errcode == 0:
+            return del_index_response.result().state
+        else:
+            raise RuntimeError(del_index_response.result().error.errmsg)
 
     def convert_message_to_dict(self, vec):
         message_dict = MessageToDict(vec, including_default_value_fields=True)
-        if message_dict and int(message_dict["id"]) != 0:
-            message_dict["id"] = int(message_dict["id"])
-            message_dict["scalarData"] = message_dict["scalarData"]["scalarData"]
+        if message_dict and message_dict["id"] != 0:
             return message_dict
         else:
             return None
 
     def vector_add(
         self, index_name: str, datas: list, vectors: list, ids: list = None
     ) -> list:
@@ -284,56 +289,80 @@
         )
 
         vec_add_request = VectorAddRequest(
             schema_name="dingo", index_name=params.index_name
         )
         for i, v in enumerate(params.vectors):
             vec_grpc = VectorWithId()
-            scalar_data_grpc = VectorScalarData()
             for key, value in params.datas[i].items():
-                entry = scalar_data_grpc.scalar_data[key]
+                entry = vec_grpc.scalar_data[key]
                 entry.field_type = STRING
                 field = entry.fields.add()
                 field.string_data = value
 
             vec_grpc.vector.CopyFrom(
                 Vector(dimension=len(v), float_values=v, value_type=FLOAT)
             )
-            vec_grpc.scalar_data.CopyFrom(scalar_data_grpc)
             if ids is not None:
                 vec_grpc.id = params.ids[i]
             vec_add_request.vectors.append(vec_grpc)
 
         vec_add_response = self.index_stub.VectorAdd.future(vec_add_request)
 
-        add_res = list(
-            self.convert_message_to_dict(vec)
-            for vec in vec_add_response.result().vectors
-        )
-        return add_res
+        if vec_add_response.result().error.errcode == 0:
+            add_res = list(
+                self.convert_message_to_dict(vec)
+                for vec in vec_add_response.result().vectors
+            )
+            return add_res
+        else:
+            raise RuntimeError(vec_add_response.result().error.errmsg)
 
     def vector_count(self, index_name: str):
         """
         vector_count count in index
 
         Args:
             index_name (str): the name of in index
 
         Returns:
             int: count num
         """
-        vec_count_request = VectorGetRegionMetricsRequest(
+        vec_count_request = VectorCountRequest(
             schema_name="dingo", index_name=index_name
         )
-        vec_count_response = self.index_stub.VectorGetRegionMetrics.future(
-            vec_count_request
+        vec_count_response = self.index_stub.VectorCount.future(vec_count_request)
+
+        if vec_count_response.result().error.errcode == 0:
+            return vec_count_response.result().count
+        else:
+            raise RuntimeError(vec_count_response.result().error.errmsg)
+
+    def vector_metrics(self, index_name: str):
+        """
+        vector_metrics metrics in index
+
+        Args:
+            index_name (str): the name of in index
+
+        Returns:
+            dict: metrics
+        """
+        vec_metrics_request = VectorGetRegionMetricsRequest(
+            schema_name="dingo", index_name=index_name
+        )
+        vec_metrics_response = self.index_stub.VectorGetRegionMetrics.future(
+            vec_metrics_request
         )
-        records = MessageToDict(vec_count_response.result().metrics)
 
-        return int(records.get("currentCount", 0)) - int(records.get("deletedCount", 0))
+        if vec_metrics_response.result().error.errcode == 0:
+            records = MessageToDict(vec_metrics_response.result().metrics)
+            return records
+        else:
+            raise RuntimeError(vec_metrics_response.result().error.errmsg)
 
     def vector_scan(
         self,
         index_name: str,
         start_id: int,
         max_count: int = 1000,
         is_reverse: bool = False,
@@ -401,16 +430,18 @@
             vec_scan_request.scalar_for_filter.CopyFrom(scalar_data_grpc)
         vec_scan_response = self.index_stub.VectorScanQuery.future(vec_scan_request)
 
         scan_res = list(
             self.convert_message_to_dict(vec)
             for vec in vec_scan_response.result().vectors
         )
-
-        return scan_res
+        if vec_scan_response.result().error.errcode == 0:
+            return scan_res
+        else:
+            raise RuntimeError(vec_scan_response.result().error.errmsg)
 
     def get_index(self):
         """
         get_index get all index
 
         Raises:
             RuntimeError: return error
@@ -420,16 +451,18 @@
         """
 
         get_index_name_request = GetIndexNamesRequest(schema_name="dingo")
 
         get_index_name_response = self.meta_stub.GetIndexNames.future(
             get_index_name_request
         )
-
-        return get_index_name_response.result().names
+        if get_index_name_response.result().error.errcode == 0:
+            return get_index_name_response.result().names
+        else:
+            raise RuntimeError(get_index_name_response.result().error.errmsg)
 
     def get_max_index_row(self, index_name: str, get_min: bool = False):
         """
         get_max_index_row get max id in index
 
         Args:
             index_name (str): the name of in index
@@ -445,16 +478,18 @@
         vec_max_id_request = VectorGetBorderIdRequest(
             schema_name="dingo", index_name=index_name, get_min=get_min
         )
 
         vec_max_id_response = self.index_stub.VectorGetBorderId.future(
             vec_max_id_request
         )
-
-        return vec_max_id_response.result().id
+        if vec_max_id_response.result().error.errcode == 0:
+            return vec_max_id_response.result().id
+        else:
+            raise RuntimeError(vec_max_id_response.result().error.errmsg)
 
     def vector_search(
         self,
         index_name: str,
         xq: list,
         top_k: int = 10,
         search_params: dict = None,
@@ -481,30 +516,21 @@
             xq=xq,
             top_k=top_k,
             pre_filter=pre_filter,
             search_params=search_params,
         )
 
         vec_search_response = self.index_stub.VectorSearch.future(params.search_params)
-        search_res = []
-        for vec in vec_search_response.result().batch_results:
-            res_info = []
-            msg_dict = MessageToDict(vec, including_default_value_fields=True)
-            for vec_info in msg_dict["vectorWithDistances"]:
-                vec_info["vectorWithId"]["id"] = int(vec_info["vectorWithId"]["id"])
-                vec_info["vectorWithId"]["scalarData"] = vec_info["vectorWithId"][
-                    "scalarData"
-                ]["scalarData"]
-                vec_info.update(vec_info["vectorWithId"])
-                vec_info.pop("vectorWithId")
-                res_info.append(vec_info)
-            msg_dict["vectorWithDistances"] = res_info
-            search_res.append(msg_dict)
-
-        return search_res
+        if vec_search_response.result().error.errcode == 0:
+            return [
+                MessageToDict(vec, including_default_value_fields=True)
+                for vec in vec_search_response.result().batch_results
+            ]
+        else:
+            raise RuntimeError(vec_search_response.result().error.errmsg)
 
     def vector_get(
         self, index_name: str, ids: list, scalar: bool = True, vector: bool = True
     ) -> list:
         """
         vector_get query vector
 
@@ -530,20 +556,22 @@
             vector_ids=params.ids,
             without_vector_data=not vector,
             without_scalar_data=not scalar,
         )
 
         vec_get_response = self.index_stub.VectorGet.future(vec_get_request)
 
-        get_res = list(
-            self.convert_message_to_dict(vec)
-            for vec in vec_get_response.result().vectors
-        )
-
-        return get_res
+        if vec_get_response.result().error.errcode == 0:
+            get_res = list(
+                self.convert_message_to_dict(vec)
+                for vec in vec_get_response.result().vectors
+            )
+            return get_res
+        else:
+            raise RuntimeError(vec_get_response.result().error.errmsg)
 
     def vector_delete(self, index_name: str, ids: list):
         """
         vector_delete delete vector with ids
 
         Args:
             index_name (str): the name of the index
@@ -558,8 +586,11 @@
         params = CheckVectorDeleteParam(index_name=index_name, ids=ids)
 
         vec_del_request = VectorDeleteRequest(
             schema_name="dingo", index_name=params.index_name, ids=params.ids
         )
 
         vec_del_response = self.index_stub.VectorDelete.future(vec_del_request)
-        return vec_del_response.result().key_states
+        if vec_del_response.result().error.errcode == 0:
+            return vec_del_response.result().key_states
+        else:
+            raise RuntimeError(vec_del_response.result().error.errmsg)
```

### Comparing `dingodb-0.0.8/dingodb/grpc/grpc_dingo_param.py` & `dingodb-0.0.9/dingodb/grpc/grpc_dingo_param.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,22 +213,20 @@
         parameter.use_scalar_filter = use_scalar_filter
         # scalar_data_map = {}
         for xq in values.get("xq"):
             vec_with_id = VectorWithId(
                 vector=Vector(dimension=len(xq), float_values=xq, value_type=FLOAT)
             )
             if use_scalar_filter:
-                scalar_data_grpc = VectorScalarData()
                 for key, value in search_params["meta_expr"].items():
-                    entry = scalar_data_grpc.scalar_data[key]
+                    entry = vec_with_id.scalar_data[key]
                     entry.field_type = STRING
                     field = entry.fields.add()
                     field.string_data = value
 
-                vec_with_id.scalar_data.CopyFrom(scalar_data_grpc)
             vec_search_request.vectors.append(vec_with_id)
 
         ef_search = 32 if search_params is None else search_params.get("efSearch", 32)
         assert ef_search >= 0, f"efSearch must >= 0, but get {ef_search}"
 
         parameter.hnsw.CopyFrom(SearchHNSWParam(efSearch=ef_search))
         if search_params and "parallelOnQueries" in search_params.keys():
```

### Comparing `dingodb-0.0.8/dingodb/protos/proxy_common_pb2.py` & `dingodb-0.0.9/dingodb/protos/proxy_common_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,91 +9,99 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12proxy_common.proto\x12\x17\x64ingodb.pb.proxy.common\"\xbe\x01\n\x10\x43olumnDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08sql_type\x18\x02 \x01(\t\x12\x14\n\x0c\x65lement_type\x18\x03 \x01(\t\x12\x11\n\tprecision\x18\x04 \x01(\x05\x12\r\n\x05scale\x18\x05 \x01(\x05\x12\x10\n\x08nullable\x18\x06 \x01(\x08\x12\x12\n\nindexOfKey\x18\x07 \x01(\x05\x12\x17\n\x0fhas_default_val\x18\x08 \x01(\x08\x12\x13\n\x0b\x64\x65\x66\x61ult_val\x18\t \x01(\t\"\x80\x01\n\x06Vector\x12\x11\n\tdimension\x18\x01 \x01(\x05\x12\x36\n\nvalue_type\x18\x02 \x01(\x0e\x32\".dingodb.pb.proxy.common.ValueType\x12\x14\n\x0c\x66loat_values\x18\x03 \x03(\x02\x12\x15\n\rbinary_values\x18\x04 \x03(\x0c\"\xbb\x01\n\x10VectorScalarData\x12N\n\x0bscalar_data\x18\x01 \x03(\x0b\x32\x39.dingodb.pb.proxy.common.VectorScalarData.ScalarDataEntry\x1aW\n\x0fScalarDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.dingodb.pb.proxy.common.ScalarValue:\x02\x38\x01\"9\n\x0fVectorTableData\x12\x11\n\ttable_key\x18\x01 \x01(\x0c\x12\x13\n\x0btable_value\x18\x02 \x01(\x0c\"\xc9\x01\n\x0cVectorWithId\x12\n\n\x02id\x18\x01 \x01(\x04\x12/\n\x06vector\x18\x02 \x01(\x0b\x32\x1f.dingodb.pb.proxy.common.Vector\x12>\n\x0bscalar_data\x18\x03 \x01(\x0b\x32).dingodb.pb.proxy.common.VectorScalarData\x12<\n\ntable_data\x18\x04 \x01(\x0b\x32(.dingodb.pb.proxy.common.VectorTableData\"\x9f\x01\n\x12VectorWithDistance\x12=\n\x0evector_with_id\x18\x01 \x01(\x0b\x32%.dingodb.pb.proxy.common.VectorWithId\x12\x10\n\x08\x64istance\x18\x02 \x01(\x02\x12\x38\n\x0bmetric_type\x18\x03 \x01(\x0e\x32#.dingodb.pb.proxy.common.MetricType\"\xe6\x01\n\x0eIndexParameter\x12\x36\n\nindex_type\x18\x01 \x01(\x0e\x32\".dingodb.pb.proxy.common.IndexType\x12M\n\x16vector_index_parameter\x18\x02 \x01(\x0b\x32-.dingodb.pb.proxy.common.VectorIndexParameter\x12M\n\x16scalar_index_parameter\x18\x03 \x01(\x0b\x32-.dingodb.pb.proxy.common.ScalarIndexParameter\"^\n\x0f\x43reateFlatParam\x12\x11\n\tdimension\x18\x01 \x01(\r\x12\x38\n\x0bmetric_type\x18\x02 \x01(\x0e\x32#.dingodb.pb.proxy.common.MetricType\"u\n\x12\x43reateIvfFlatParam\x12\x11\n\tdimension\x18\x01 \x01(\r\x12\x38\n\x0bmetric_type\x18\x02 \x01(\x0e\x32#.dingodb.pb.proxy.common.MetricType\x12\x12\n\nncentroids\x18\x03 \x01(\x05\"\xba\x01\n\x10\x43reateIvfPqParam\x12\x11\n\tdimension\x18\x01 \x01(\r\x12\x38\n\x0bmetric_type\x18\x02 \x01(\x0e\x32#.dingodb.pb.proxy.common.MetricType\x12\x12\n\nncentroids\x18\x03 \x01(\x05\x12\x12\n\nnsubvector\x18\x04 \x01(\x05\x12\x18\n\x10\x62ucket_init_size\x18\x05 \x01(\x05\x12\x17\n\x0f\x62ucket_max_size\x18\x06 \x01(\x05\"\x9c\x01\n\x0f\x43reateHnswParam\x12\x11\n\tdimension\x18\x01 \x01(\r\x12\x38\n\x0bmetric_type\x18\x02 \x01(\x0e\x32#.dingodb.pb.proxy.common.MetricType\x12\x16\n\x0e\x65\x66\x43onstruction\x18\x03 \x01(\r\x12\x14\n\x0cmax_elements\x18\x04 \x01(\r\x12\x0e\n\x06nlinks\x18\x05 \x01(\x05\"\xa0\x01\n\x12\x43reateDiskAnnParam\x12\x11\n\tdimension\x18\x01 \x01(\r\x12\x38\n\x0bmetric_type\x18\x02 \x01(\x0e\x32#.dingodb.pb.proxy.common.MetricType\x12\x11\n\tnum_trees\x18\x03 \x01(\x05\x12\x15\n\rnum_neighbors\x18\x04 \x01(\x05\x12\x13\n\x0bnum_threads\x18\x05 \x01(\x05\"\xd9\x03\n\x14VectorIndexParameter\x12\x43\n\x11vector_index_type\x18\x01 \x01(\x0e\x32(.dingodb.pb.proxy.common.VectorIndexType\x12\x42\n\x0e\x66lat_parameter\x18\x02 \x01(\x0b\x32(.dingodb.pb.proxy.common.CreateFlatParamH\x00\x12I\n\x12ivf_flat_parameter\x18\x03 \x01(\x0b\x32+.dingodb.pb.proxy.common.CreateIvfFlatParamH\x00\x12\x45\n\x10ivf_pq_parameter\x18\x04 \x01(\x0b\x32).dingodb.pb.proxy.common.CreateIvfPqParamH\x00\x12\x42\n\x0ehnsw_parameter\x18\x05 \x01(\x0b\x32(.dingodb.pb.proxy.common.CreateHnswParamH\x00\x12H\n\x11\x64iskann_parameter\x18\x06 \x01(\x0b\x32+.dingodb.pb.proxy.common.CreateDiskAnnParamH\x00\x42\x18\n\x16vector_index_parameter\"\xc8\x01\n\x0cVectorSchema\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.dingodb.pb.proxy.common.VectorSchema.Type\x12\x0e\n\x06is_key\x18\x02 \x01(\x08\x12\x13\n\x0bis_nullable\x18\x03 \x01(\x08\x12\r\n\x05index\x18\x04 \x01(\x05\"J\n\x04Type\x12\x08\n\x04\x42OOL\x10\x00\x12\x0b\n\x07INTEGER\x10\x01\x12\t\n\x05\x46LOAT\x10\x02\x12\x08\n\x04LONG\x10\x03\x12\n\n\x06\x44OUBLE\x10\x04\x12\n\n\x06STRING\x10\x05\"[\n\x14ScalarIndexParameter\x12\x43\n\x11scalar_index_type\x18\x01 \x01(\x0e\x32(.dingodb.pb.proxy.common.ScalarIndexType\".\n\x0fSearchFlatParam\x12\x1b\n\x13parallel_on_queries\x18\x01 \x01(\x05\"A\n\x12SearchIvfFlatParam\x12\x0e\n\x06nprobe\x18\x01 \x01(\x05\x12\x1b\n\x13parallel_on_queries\x18\x02 \x01(\x05\"S\n\x10SearchIvfPqParam\x12\x0e\n\x06nprobe\x18\x01 \x01(\x05\x12\x1b\n\x13parallel_on_queries\x18\x02 \x01(\x05\x12\x12\n\nrecall_num\x18\x03 \x01(\x05\"#\n\x0fSearchHNSWParam\x12\x10\n\x08\x65\x66Search\x18\x01 \x01(\x05\"\x14\n\x12SearchDiskAnnParam\"\xcb\x05\n\x15VectorSearchParameter\x12\r\n\x05top_n\x18\x01 \x01(\r\x12\x1b\n\x13without_vector_data\x18\x02 \x01(\x08\x12\x1b\n\x13without_scalar_data\x18\x03 \x01(\x08\x12\x15\n\rselected_keys\x18\x04 \x03(\t\x12\x1a\n\x12without_table_data\x18\x05 \x01(\x08\x12\x38\n\x04\x66lat\x18\x0b \x01(\x0b\x32(.dingodb.pb.proxy.common.SearchFlatParamH\x00\x12?\n\x08ivf_flat\x18\x0c \x01(\x0b\x32+.dingodb.pb.proxy.common.SearchIvfFlatParamH\x00\x12;\n\x06ivf_pq\x18\r \x01(\x0b\x32).dingodb.pb.proxy.common.SearchIvfPqParamH\x00\x12\x38\n\x04hnsw\x18\x0e \x01(\x0b\x32(.dingodb.pb.proxy.common.SearchHNSWParamH\x00\x12>\n\x07\x64iskann\x18\x0f \x01(\x0b\x32+.dingodb.pb.proxy.common.SearchDiskAnnParamH\x00\x12\x19\n\x11use_scalar_filter\x18\x14 \x01(\x08\x12<\n\rvector_filter\x18\x15 \x01(\x0e\x32%.dingodb.pb.proxy.common.VectorFilter\x12\x45\n\x12vector_filter_type\x18\x16 \x01(\x0e\x32).dingodb.pb.proxy.common.VectorFilterType\x12\x46\n\x12vector_coprocessor\x18\x17 \x01(\x0b\x32*.dingodb.pb.proxy.common.VectorCoprocessor\x12\x12\n\nvector_ids\x18\x18 \x03(\x04\x42\x08\n\x06search\"\xa1\x01\n\x11VectorCoprocessor\x12\x16\n\x0eschema_version\x18\x01 \x01(\x05\x12\x45\n\x0foriginal_schema\x18\x02 \x01(\x0b\x32,.dingodb.pb.proxy.common.VectorSchemaWrapper\x12\x19\n\x11selection_columns\x18\x03 \x03(\x05\x12\x12\n\nexpression\x18\x04 \x01(\x0c\"c\n\x13VectorSchemaWrapper\x12\x39\n\x06schema\x18\x01 \x03(\x0b\x32).dingodb.pb.proxy.common.ColumnDefinition\x12\x11\n\tcommon_id\x18\x02 \x01(\x03\"\xad\x01\n\x0bScalarField\x12\x13\n\tbool_data\x18\x01 \x01(\x08H\x00\x12\x12\n\x08int_data\x18\x02 \x01(\x05H\x00\x12\x13\n\tlong_data\x18\x03 \x01(\x03H\x00\x12\x14\n\nfloat_data\x18\x04 \x01(\x02H\x00\x12\x15\n\x0b\x64ouble_data\x18\x05 \x01(\x01H\x00\x12\x15\n\x0bstring_data\x18\x06 \x01(\tH\x00\x12\x14\n\nbytes_data\x18\x07 \x01(\x0cH\x00\x42\x06\n\x04\x64\x61ta\"\x81\x01\n\x0bScalarValue\x12<\n\nfield_type\x18\x01 \x01(\x0e\x32(.dingodb.pb.proxy.common.ScalarFieldType\x12\x34\n\x06\x66ields\x18\x02 \x03(\x0b\x32$.dingodb.pb.proxy.common.ScalarField\"\xbd\x01\n\x12VectorIndexMetrics\x12\x43\n\x11vector_index_type\x18\x01 \x01(\x0e\x32(.dingodb.pb.proxy.common.VectorIndexType\x12\x15\n\rcurrent_count\x18\x02 \x01(\x03\x12\x15\n\rdeleted_count\x18\x03 \x01(\x03\x12\x0e\n\x06max_id\x18\x04 \x01(\x03\x12\x0e\n\x06min_id\x18\x05 \x01(\x03\x12\x14\n\x0cmemory_bytes\x18\x06 \x01(\x03*!\n\tValueType\x12\t\n\x05\x46LOAT\x10\x00\x12\t\n\x05UINT8\x10\x01*e\n\x0fScalarIndexType\x12\x1a\n\x16SCALAR_INDEX_TYPE_NONE\x10\x00\x12\x19\n\x15SCALAR_INDEX_TYPE_LSM\x10\x01\x12\x1b\n\x17SCALAR_INDEX_TYPE_BTREE\x10\x02*N\n\tIndexType\x12\x13\n\x0fINDEX_TYPE_NONE\x10\x00\x12\x15\n\x11INDEX_TYPE_VECTOR\x10\x01\x12\x15\n\x11INDEX_TYPE_SCALAR\x10\x02*\xc2\x01\n\x0fVectorIndexType\x12\x1a\n\x16VECTOR_INDEX_TYPE_NONE\x10\x00\x12\x1a\n\x16VECTOR_INDEX_TYPE_FLAT\x10\x01\x12\x1e\n\x1aVECTOR_INDEX_TYPE_IVF_FLAT\x10\x02\x12\x1c\n\x18VECTOR_INDEX_TYPE_IVF_PQ\x10\x03\x12\x1a\n\x16VECTOR_INDEX_TYPE_HNSW\x10\x04\x12\x1d\n\x19VECTOR_INDEX_TYPE_DISKANN\x10\x05*m\n\nMetricType\x12\x14\n\x10METRIC_TYPE_NONE\x10\x00\x12\x12\n\x0eMETRIC_TYPE_L2\x10\x01\x12\x1d\n\x19METRIC_TYPE_INNER_PRODUCT\x10\x02\x12\x16\n\x12METRIC_TYPE_COSINE\x10\x03*I\n\x0cVectorFilter\x12\x11\n\rSCALAR_FILTER\x10\x00\x12\x10\n\x0cTABLE_FILTER\x10\x01\x12\x14\n\x10VECTOR_ID_FILTER\x10\n*1\n\x10VectorFilterType\x12\x0e\n\nQUERY_POST\x10\x00\x12\r\n\tQUERY_PRE\x10\x01*\x80\x01\n\x0fScalarFieldType\x12\x08\n\x04NONE\x10\x00\x12\x08\n\x04\x42OOL\x10\x01\x12\x08\n\x04INT8\x10\x02\x12\t\n\x05INT16\x10\x03\x12\t\n\x05INT32\x10\x04\x12\t\n\x05INT64\x10\x05\x12\x0b\n\x07\x46LOAT32\x10\x06\x12\n\n\x06\x44OUBLE\x10\x07\x12\n\n\x06STRING\x10\x08\x12\t\n\x05\x42YTES\x10\tB\x1c\n\x17io.dingodb.proxy.common\x88\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12proxy_common.proto\x12\x17\x64ingodb.pb.proxy.common\"\xbe\x01\n\x10\x43olumnDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08sql_type\x18\x02 \x01(\t\x12\x14\n\x0c\x65lement_type\x18\x03 \x01(\t\x12\x11\n\tprecision\x18\x04 \x01(\x05\x12\r\n\x05scale\x18\x05 \x01(\x05\x12\x10\n\x08nullable\x18\x06 \x01(\x08\x12\x12\n\nindexOfKey\x18\x07 \x01(\x05\x12\x17\n\x0fhas_default_val\x18\x08 \x01(\x08\x12\x13\n\x0b\x64\x65\x66\x61ult_val\x18\t \x01(\t\"\x80\x01\n\x06Vector\x12\x11\n\tdimension\x18\x01 \x01(\x05\x12\x36\n\nvalue_type\x18\x02 \x01(\x0e\x32\".dingodb.pb.proxy.common.ValueType\x12\x14\n\x0c\x66loat_values\x18\x03 \x03(\x02\x12\x15\n\rbinary_values\x18\x04 \x03(\x0c\"\xbb\x01\n\x10VectorScalarData\x12N\n\x0bscalar_data\x18\x01 \x03(\x0b\x32\x39.dingodb.pb.proxy.common.VectorScalarData.ScalarDataEntry\x1aW\n\x0fScalarDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.dingodb.pb.proxy.common.ScalarValue:\x02\x38\x01\"9\n\x0fVectorTableData\x12\x11\n\ttable_key\x18\x01 \x01(\x0c\x12\x13\n\x0btable_value\x18\x02 \x01(\x0c\"\xae\x02\n\x0cVectorWithId\x12\n\n\x02id\x18\x01 \x01(\x04\x12/\n\x06vector\x18\x02 \x01(\x0b\x32\x1f.dingodb.pb.proxy.common.Vector\x12J\n\x0bscalar_data\x18\x03 \x03(\x0b\x32\x35.dingodb.pb.proxy.common.VectorWithId.ScalarDataEntry\x12<\n\ntable_data\x18\x04 \x01(\x0b\x32(.dingodb.pb.proxy.common.VectorTableData\x1aW\n\x0fScalarDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.dingodb.pb.proxy.common.ScalarValue:\x02\x38\x01\"\xc8\x02\n\x12VectorWithDistance\x12\n\n\x02id\x18\x01 \x01(\x04\x12/\n\x06vector\x18\x02 \x01(\x0b\x32\x1f.dingodb.pb.proxy.common.Vector\x12P\n\x0bscalar_data\x18\x03 \x03(\x0b\x32;.dingodb.pb.proxy.common.VectorWithDistance.ScalarDataEntry\x12\x10\n\x08\x64istance\x18\x04 \x01(\x02\x12\x38\n\x0bmetric_type\x18\x05 \x01(\x0e\x32#.dingodb.pb.proxy.common.MetricType\x1aW\n\x0fScalarDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.dingodb.pb.proxy.common.ScalarValue:\x02\x38\x01\"\xe6\x01\n\x0eIndexParameter\x12\x36\n\nindex_type\x18\x01 \x01(\x0e\x32\".dingodb.pb.proxy.common.IndexType\x12M\n\x16vector_index_parameter\x18\x02 \x01(\x0b\x32-.dingodb.pb.proxy.common.VectorIndexParameter\x12M\n\x16scalar_index_parameter\x18\x03 \x01(\x0b\x32-.dingodb.pb.proxy.common.ScalarIndexParameter\"^\n\x0f\x43reateFlatParam\x12\x11\n\tdimension\x18\x01 \x01(\r\x12\x38\n\x0bmetric_type\x18\x02 \x01(\x0e\x32#.dingodb.pb.proxy.common.MetricType\"u\n\x12\x43reateIvfFlatParam\x12\x11\n\tdimension\x18\x01 \x01(\r\x12\x38\n\x0bmetric_type\x18\x02 \x01(\x0e\x32#.dingodb.pb.proxy.common.MetricType\x12\x12\n\nncentroids\x18\x03 \x01(\x05\"\xba\x01\n\x10\x43reateIvfPqParam\x12\x11\n\tdimension\x18\x01 \x01(\r\x12\x38\n\x0bmetric_type\x18\x02 \x01(\x0e\x32#.dingodb.pb.proxy.common.MetricType\x12\x12\n\nncentroids\x18\x03 \x01(\x05\x12\x12\n\nnsubvector\x18\x04 \x01(\x05\x12\x18\n\x10\x62ucket_init_size\x18\x05 \x01(\x05\x12\x17\n\x0f\x62ucket_max_size\x18\x06 \x01(\x05\"\x9c\x01\n\x0f\x43reateHnswParam\x12\x11\n\tdimension\x18\x01 \x01(\r\x12\x38\n\x0bmetric_type\x18\x02 \x01(\x0e\x32#.dingodb.pb.proxy.common.MetricType\x12\x16\n\x0e\x65\x66\x43onstruction\x18\x03 \x01(\r\x12\x14\n\x0cmax_elements\x18\x04 \x01(\r\x12\x0e\n\x06nlinks\x18\x05 \x01(\x05\"\xa0\x01\n\x12\x43reateDiskAnnParam\x12\x11\n\tdimension\x18\x01 \x01(\r\x12\x38\n\x0bmetric_type\x18\x02 \x01(\x0e\x32#.dingodb.pb.proxy.common.MetricType\x12\x11\n\tnum_trees\x18\x03 \x01(\x05\x12\x15\n\rnum_neighbors\x18\x04 \x01(\x05\x12\x13\n\x0bnum_threads\x18\x05 \x01(\x05\"\xd9\x03\n\x14VectorIndexParameter\x12\x43\n\x11vector_index_type\x18\x01 \x01(\x0e\x32(.dingodb.pb.proxy.common.VectorIndexType\x12\x42\n\x0e\x66lat_parameter\x18\x02 \x01(\x0b\x32(.dingodb.pb.proxy.common.CreateFlatParamH\x00\x12I\n\x12ivf_flat_parameter\x18\x03 \x01(\x0b\x32+.dingodb.pb.proxy.common.CreateIvfFlatParamH\x00\x12\x45\n\x10ivf_pq_parameter\x18\x04 \x01(\x0b\x32).dingodb.pb.proxy.common.CreateIvfPqParamH\x00\x12\x42\n\x0ehnsw_parameter\x18\x05 \x01(\x0b\x32(.dingodb.pb.proxy.common.CreateHnswParamH\x00\x12H\n\x11\x64iskann_parameter\x18\x06 \x01(\x0b\x32+.dingodb.pb.proxy.common.CreateDiskAnnParamH\x00\x42\x18\n\x16vector_index_parameter\"\xc8\x01\n\x0cVectorSchema\x12\x38\n\x04type\x18\x01 \x01(\x0e\x32*.dingodb.pb.proxy.common.VectorSchema.Type\x12\x0e\n\x06is_key\x18\x02 \x01(\x08\x12\x13\n\x0bis_nullable\x18\x03 \x01(\x08\x12\r\n\x05index\x18\x04 \x01(\x05\"J\n\x04Type\x12\x08\n\x04\x42OOL\x10\x00\x12\x0b\n\x07INTEGER\x10\x01\x12\t\n\x05\x46LOAT\x10\x02\x12\x08\n\x04LONG\x10\x03\x12\n\n\x06\x44OUBLE\x10\x04\x12\n\n\x06STRING\x10\x05\"[\n\x14ScalarIndexParameter\x12\x43\n\x11scalar_index_type\x18\x01 \x01(\x0e\x32(.dingodb.pb.proxy.common.ScalarIndexType\".\n\x0fSearchFlatParam\x12\x1b\n\x13parallel_on_queries\x18\x01 \x01(\x05\"A\n\x12SearchIvfFlatParam\x12\x0e\n\x06nprobe\x18\x01 \x01(\x05\x12\x1b\n\x13parallel_on_queries\x18\x02 \x01(\x05\"S\n\x10SearchIvfPqParam\x12\x0e\n\x06nprobe\x18\x01 \x01(\x05\x12\x1b\n\x13parallel_on_queries\x18\x02 \x01(\x05\x12\x12\n\nrecall_num\x18\x03 \x01(\x05\"#\n\x0fSearchHNSWParam\x12\x10\n\x08\x65\x66Search\x18\x01 \x01(\x05\"\x14\n\x12SearchDiskAnnParam\"\xcb\x05\n\x15VectorSearchParameter\x12\r\n\x05top_n\x18\x01 \x01(\r\x12\x1b\n\x13without_vector_data\x18\x02 \x01(\x08\x12\x1b\n\x13without_scalar_data\x18\x03 \x01(\x08\x12\x15\n\rselected_keys\x18\x04 \x03(\t\x12\x1a\n\x12without_table_data\x18\x05 \x01(\x08\x12\x38\n\x04\x66lat\x18\x0b \x01(\x0b\x32(.dingodb.pb.proxy.common.SearchFlatParamH\x00\x12?\n\x08ivf_flat\x18\x0c \x01(\x0b\x32+.dingodb.pb.proxy.common.SearchIvfFlatParamH\x00\x12;\n\x06ivf_pq\x18\r \x01(\x0b\x32).dingodb.pb.proxy.common.SearchIvfPqParamH\x00\x12\x38\n\x04hnsw\x18\x0e \x01(\x0b\x32(.dingodb.pb.proxy.common.SearchHNSWParamH\x00\x12>\n\x07\x64iskann\x18\x0f \x01(\x0b\x32+.dingodb.pb.proxy.common.SearchDiskAnnParamH\x00\x12\x19\n\x11use_scalar_filter\x18\x14 \x01(\x08\x12<\n\rvector_filter\x18\x15 \x01(\x0e\x32%.dingodb.pb.proxy.common.VectorFilter\x12\x45\n\x12vector_filter_type\x18\x16 \x01(\x0e\x32).dingodb.pb.proxy.common.VectorFilterType\x12\x46\n\x12vector_coprocessor\x18\x17 \x01(\x0b\x32*.dingodb.pb.proxy.common.VectorCoprocessor\x12\x12\n\nvector_ids\x18\x18 \x03(\x04\x42\x08\n\x06search\"\xa1\x01\n\x11VectorCoprocessor\x12\x16\n\x0eschema_version\x18\x01 \x01(\x05\x12\x45\n\x0foriginal_schema\x18\x02 \x01(\x0b\x32,.dingodb.pb.proxy.common.VectorSchemaWrapper\x12\x19\n\x11selection_columns\x18\x03 \x03(\x05\x12\x12\n\nexpression\x18\x04 \x01(\x0c\"c\n\x13VectorSchemaWrapper\x12\x39\n\x06schema\x18\x01 \x03(\x0b\x32).dingodb.pb.proxy.common.ColumnDefinition\x12\x11\n\tcommon_id\x18\x02 \x01(\x03\"\xad\x01\n\x0bScalarField\x12\x13\n\tbool_data\x18\x01 \x01(\x08H\x00\x12\x12\n\x08int_data\x18\x02 \x01(\x05H\x00\x12\x13\n\tlong_data\x18\x03 \x01(\x03H\x00\x12\x14\n\nfloat_data\x18\x04 \x01(\x02H\x00\x12\x15\n\x0b\x64ouble_data\x18\x05 \x01(\x01H\x00\x12\x15\n\x0bstring_data\x18\x06 \x01(\tH\x00\x12\x14\n\nbytes_data\x18\x07 \x01(\x0cH\x00\x42\x06\n\x04\x64\x61ta\"\x81\x01\n\x0bScalarValue\x12<\n\nfield_type\x18\x01 \x01(\x0e\x32(.dingodb.pb.proxy.common.ScalarFieldType\x12\x34\n\x06\x66ields\x18\x02 \x03(\x0b\x32$.dingodb.pb.proxy.common.ScalarField\"\xbd\x01\n\x12VectorIndexMetrics\x12\x43\n\x11vector_index_type\x18\x01 \x01(\x0e\x32(.dingodb.pb.proxy.common.VectorIndexType\x12\x15\n\rcurrent_count\x18\x02 \x01(\x03\x12\x15\n\rdeleted_count\x18\x03 \x01(\x03\x12\x0e\n\x06max_id\x18\x04 \x01(\x03\x12\x0e\n\x06min_id\x18\x05 \x01(\x03\x12\x14\n\x0cmemory_bytes\x18\x06 \x01(\x03*!\n\tValueType\x12\t\n\x05\x46LOAT\x10\x00\x12\t\n\x05UINT8\x10\x01*e\n\x0fScalarIndexType\x12\x1a\n\x16SCALAR_INDEX_TYPE_NONE\x10\x00\x12\x19\n\x15SCALAR_INDEX_TYPE_LSM\x10\x01\x12\x1b\n\x17SCALAR_INDEX_TYPE_BTREE\x10\x02*N\n\tIndexType\x12\x13\n\x0fINDEX_TYPE_NONE\x10\x00\x12\x15\n\x11INDEX_TYPE_VECTOR\x10\x01\x12\x15\n\x11INDEX_TYPE_SCALAR\x10\x02*\xc2\x01\n\x0fVectorIndexType\x12\x1a\n\x16VECTOR_INDEX_TYPE_NONE\x10\x00\x12\x1a\n\x16VECTOR_INDEX_TYPE_FLAT\x10\x01\x12\x1e\n\x1aVECTOR_INDEX_TYPE_IVF_FLAT\x10\x02\x12\x1c\n\x18VECTOR_INDEX_TYPE_IVF_PQ\x10\x03\x12\x1a\n\x16VECTOR_INDEX_TYPE_HNSW\x10\x04\x12\x1d\n\x19VECTOR_INDEX_TYPE_DISKANN\x10\x05*m\n\nMetricType\x12\x14\n\x10METRIC_TYPE_NONE\x10\x00\x12\x12\n\x0eMETRIC_TYPE_L2\x10\x01\x12\x1d\n\x19METRIC_TYPE_INNER_PRODUCT\x10\x02\x12\x16\n\x12METRIC_TYPE_COSINE\x10\x03*I\n\x0cVectorFilter\x12\x11\n\rSCALAR_FILTER\x10\x00\x12\x10\n\x0cTABLE_FILTER\x10\x01\x12\x14\n\x10VECTOR_ID_FILTER\x10\n*1\n\x10VectorFilterType\x12\x0e\n\nQUERY_POST\x10\x00\x12\r\n\tQUERY_PRE\x10\x01*\x80\x01\n\x0fScalarFieldType\x12\x08\n\x04NONE\x10\x00\x12\x08\n\x04\x42OOL\x10\x01\x12\x08\n\x04INT8\x10\x02\x12\t\n\x05INT16\x10\x03\x12\t\n\x05INT32\x10\x04\x12\t\n\x05INT64\x10\x05\x12\x0b\n\x07\x46LOAT32\x10\x06\x12\n\n\x06\x44OUBLE\x10\x07\x12\n\n\x06STRING\x10\x08\x12\t\n\x05\x42YTES\x10\tB\x1c\n\x17io.dingodb.proxy.common\x88\x01\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proxy_common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\027io.dingodb.proxy.common\210\001\001'
   _VECTORSCALARDATA_SCALARDATAENTRY._options = None
   _VECTORSCALARDATA_SCALARDATAENTRY._serialized_options = b'8\001'
-  _globals['_VALUETYPE']._serialized_start=4459
-  _globals['_VALUETYPE']._serialized_end=4492
-  _globals['_SCALARINDEXTYPE']._serialized_start=4494
-  _globals['_SCALARINDEXTYPE']._serialized_end=4595
-  _globals['_INDEXTYPE']._serialized_start=4597
-  _globals['_INDEXTYPE']._serialized_end=4675
-  _globals['_VECTORINDEXTYPE']._serialized_start=4678
-  _globals['_VECTORINDEXTYPE']._serialized_end=4872
-  _globals['_METRICTYPE']._serialized_start=4874
-  _globals['_METRICTYPE']._serialized_end=4983
-  _globals['_VECTORFILTER']._serialized_start=4985
-  _globals['_VECTORFILTER']._serialized_end=5058
-  _globals['_VECTORFILTERTYPE']._serialized_start=5060
-  _globals['_VECTORFILTERTYPE']._serialized_end=5109
-  _globals['_SCALARFIELDTYPE']._serialized_start=5112
-  _globals['_SCALARFIELDTYPE']._serialized_end=5240
+  _VECTORWITHID_SCALARDATAENTRY._options = None
+  _VECTORWITHID_SCALARDATAENTRY._serialized_options = b'8\001'
+  _VECTORWITHDISTANCE_SCALARDATAENTRY._options = None
+  _VECTORWITHDISTANCE_SCALARDATAENTRY._serialized_options = b'8\001'
+  _globals['_VALUETYPE']._serialized_start=4729
+  _globals['_VALUETYPE']._serialized_end=4762
+  _globals['_SCALARINDEXTYPE']._serialized_start=4764
+  _globals['_SCALARINDEXTYPE']._serialized_end=4865
+  _globals['_INDEXTYPE']._serialized_start=4867
+  _globals['_INDEXTYPE']._serialized_end=4945
+  _globals['_VECTORINDEXTYPE']._serialized_start=4948
+  _globals['_VECTORINDEXTYPE']._serialized_end=5142
+  _globals['_METRICTYPE']._serialized_start=5144
+  _globals['_METRICTYPE']._serialized_end=5253
+  _globals['_VECTORFILTER']._serialized_start=5255
+  _globals['_VECTORFILTER']._serialized_end=5328
+  _globals['_VECTORFILTERTYPE']._serialized_start=5330
+  _globals['_VECTORFILTERTYPE']._serialized_end=5379
+  _globals['_SCALARFIELDTYPE']._serialized_start=5382
+  _globals['_SCALARFIELDTYPE']._serialized_end=5510
   _globals['_COLUMNDEFINITION']._serialized_start=48
   _globals['_COLUMNDEFINITION']._serialized_end=238
   _globals['_VECTOR']._serialized_start=241
   _globals['_VECTOR']._serialized_end=369
   _globals['_VECTORSCALARDATA']._serialized_start=372
   _globals['_VECTORSCALARDATA']._serialized_end=559
   _globals['_VECTORSCALARDATA_SCALARDATAENTRY']._serialized_start=472
   _globals['_VECTORSCALARDATA_SCALARDATAENTRY']._serialized_end=559
   _globals['_VECTORTABLEDATA']._serialized_start=561
   _globals['_VECTORTABLEDATA']._serialized_end=618
   _globals['_VECTORWITHID']._serialized_start=621
-  _globals['_VECTORWITHID']._serialized_end=822
-  _globals['_VECTORWITHDISTANCE']._serialized_start=825
-  _globals['_VECTORWITHDISTANCE']._serialized_end=984
-  _globals['_INDEXPARAMETER']._serialized_start=987
-  _globals['_INDEXPARAMETER']._serialized_end=1217
-  _globals['_CREATEFLATPARAM']._serialized_start=1219
-  _globals['_CREATEFLATPARAM']._serialized_end=1313
-  _globals['_CREATEIVFFLATPARAM']._serialized_start=1315
-  _globals['_CREATEIVFFLATPARAM']._serialized_end=1432
-  _globals['_CREATEIVFPQPARAM']._serialized_start=1435
-  _globals['_CREATEIVFPQPARAM']._serialized_end=1621
-  _globals['_CREATEHNSWPARAM']._serialized_start=1624
-  _globals['_CREATEHNSWPARAM']._serialized_end=1780
-  _globals['_CREATEDISKANNPARAM']._serialized_start=1783
-  _globals['_CREATEDISKANNPARAM']._serialized_end=1943
-  _globals['_VECTORINDEXPARAMETER']._serialized_start=1946
-  _globals['_VECTORINDEXPARAMETER']._serialized_end=2419
-  _globals['_VECTORSCHEMA']._serialized_start=2422
-  _globals['_VECTORSCHEMA']._serialized_end=2622
-  _globals['_VECTORSCHEMA_TYPE']._serialized_start=2548
-  _globals['_VECTORSCHEMA_TYPE']._serialized_end=2622
-  _globals['_SCALARINDEXPARAMETER']._serialized_start=2624
-  _globals['_SCALARINDEXPARAMETER']._serialized_end=2715
-  _globals['_SEARCHFLATPARAM']._serialized_start=2717
-  _globals['_SEARCHFLATPARAM']._serialized_end=2763
-  _globals['_SEARCHIVFFLATPARAM']._serialized_start=2765
-  _globals['_SEARCHIVFFLATPARAM']._serialized_end=2830
-  _globals['_SEARCHIVFPQPARAM']._serialized_start=2832
-  _globals['_SEARCHIVFPQPARAM']._serialized_end=2915
-  _globals['_SEARCHHNSWPARAM']._serialized_start=2917
-  _globals['_SEARCHHNSWPARAM']._serialized_end=2952
-  _globals['_SEARCHDISKANNPARAM']._serialized_start=2954
-  _globals['_SEARCHDISKANNPARAM']._serialized_end=2974
-  _globals['_VECTORSEARCHPARAMETER']._serialized_start=2977
-  _globals['_VECTORSEARCHPARAMETER']._serialized_end=3692
-  _globals['_VECTORCOPROCESSOR']._serialized_start=3695
-  _globals['_VECTORCOPROCESSOR']._serialized_end=3856
-  _globals['_VECTORSCHEMAWRAPPER']._serialized_start=3858
-  _globals['_VECTORSCHEMAWRAPPER']._serialized_end=3957
-  _globals['_SCALARFIELD']._serialized_start=3960
-  _globals['_SCALARFIELD']._serialized_end=4133
-  _globals['_SCALARVALUE']._serialized_start=4136
-  _globals['_SCALARVALUE']._serialized_end=4265
-  _globals['_VECTORINDEXMETRICS']._serialized_start=4268
-  _globals['_VECTORINDEXMETRICS']._serialized_end=4457
+  _globals['_VECTORWITHID']._serialized_end=923
+  _globals['_VECTORWITHID_SCALARDATAENTRY']._serialized_start=472
+  _globals['_VECTORWITHID_SCALARDATAENTRY']._serialized_end=559
+  _globals['_VECTORWITHDISTANCE']._serialized_start=926
+  _globals['_VECTORWITHDISTANCE']._serialized_end=1254
+  _globals['_VECTORWITHDISTANCE_SCALARDATAENTRY']._serialized_start=472
+  _globals['_VECTORWITHDISTANCE_SCALARDATAENTRY']._serialized_end=559
+  _globals['_INDEXPARAMETER']._serialized_start=1257
+  _globals['_INDEXPARAMETER']._serialized_end=1487
+  _globals['_CREATEFLATPARAM']._serialized_start=1489
+  _globals['_CREATEFLATPARAM']._serialized_end=1583
+  _globals['_CREATEIVFFLATPARAM']._serialized_start=1585
+  _globals['_CREATEIVFFLATPARAM']._serialized_end=1702
+  _globals['_CREATEIVFPQPARAM']._serialized_start=1705
+  _globals['_CREATEIVFPQPARAM']._serialized_end=1891
+  _globals['_CREATEHNSWPARAM']._serialized_start=1894
+  _globals['_CREATEHNSWPARAM']._serialized_end=2050
+  _globals['_CREATEDISKANNPARAM']._serialized_start=2053
+  _globals['_CREATEDISKANNPARAM']._serialized_end=2213
+  _globals['_VECTORINDEXPARAMETER']._serialized_start=2216
+  _globals['_VECTORINDEXPARAMETER']._serialized_end=2689
+  _globals['_VECTORSCHEMA']._serialized_start=2692
+  _globals['_VECTORSCHEMA']._serialized_end=2892
+  _globals['_VECTORSCHEMA_TYPE']._serialized_start=2818
+  _globals['_VECTORSCHEMA_TYPE']._serialized_end=2892
+  _globals['_SCALARINDEXPARAMETER']._serialized_start=2894
+  _globals['_SCALARINDEXPARAMETER']._serialized_end=2985
+  _globals['_SEARCHFLATPARAM']._serialized_start=2987
+  _globals['_SEARCHFLATPARAM']._serialized_end=3033
+  _globals['_SEARCHIVFFLATPARAM']._serialized_start=3035
+  _globals['_SEARCHIVFFLATPARAM']._serialized_end=3100
+  _globals['_SEARCHIVFPQPARAM']._serialized_start=3102
+  _globals['_SEARCHIVFPQPARAM']._serialized_end=3185
+  _globals['_SEARCHHNSWPARAM']._serialized_start=3187
+  _globals['_SEARCHHNSWPARAM']._serialized_end=3222
+  _globals['_SEARCHDISKANNPARAM']._serialized_start=3224
+  _globals['_SEARCHDISKANNPARAM']._serialized_end=3244
+  _globals['_VECTORSEARCHPARAMETER']._serialized_start=3247
+  _globals['_VECTORSEARCHPARAMETER']._serialized_end=3962
+  _globals['_VECTORCOPROCESSOR']._serialized_start=3965
+  _globals['_VECTORCOPROCESSOR']._serialized_end=4126
+  _globals['_VECTORSCHEMAWRAPPER']._serialized_start=4128
+  _globals['_VECTORSCHEMAWRAPPER']._serialized_end=4227
+  _globals['_SCALARFIELD']._serialized_start=4230
+  _globals['_SCALARFIELD']._serialized_end=4403
+  _globals['_SCALARVALUE']._serialized_start=4406
+  _globals['_SCALARVALUE']._serialized_end=4535
+  _globals['_VECTORINDEXMETRICS']._serialized_start=4538
+  _globals['_VECTORINDEXMETRICS']._serialized_end=4727
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dingodb-0.0.8/dingodb/protos/proxy_index_pb2.py` & `dingodb-0.0.9/dingodb/protos/proxy_index_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,59 +8,56 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 import proxy_common_pb2 as proxy__common__pb2
+import proxy_error_pb2 as proxy__error__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11proxy_index.proto\x12\x16\x64ingodb.pb.proxy.index\x1a\x12proxy_common.proto\"\x9f\x01\n\x10VectorAddRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x36\n\x07vectors\x18\x03 \x03(\x0b\x32%.dingodb.pb.proxy.common.VectorWithId\x12\x17\n\x0freplace_deleted\x18\x04 \x01(\x08\x12\x11\n\tis_update\x18\x05 \x01(\x08\"K\n\x11VectorAddResponse\x12\x36\n\x07vectors\x18\x01 \x03(\x0b\x32%.dingodb.pb.proxy.common.VectorWithId\"\xbc\x01\n\x10VectorGetRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x12\n\nvector_ids\x18\x03 \x03(\x04\x12\x1b\n\x13without_vector_data\x18\x04 \x01(\x08\x12\x1b\n\x13without_scalar_data\x18\x05 \x01(\x08\x12\x15\n\rselected_keys\x18\x06 \x03(\t\x12\x1a\n\x12without_table_data\x18\x07 \x01(\x08\"K\n\x11VectorGetResponse\x12\x36\n\x07vectors\x18\x01 \x03(\x0b\x32%.dingodb.pb.proxy.common.VectorWithId\"\xb9\x01\n\x13VectorSearchRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x36\n\x07vectors\x18\x03 \x03(\x0b\x32%.dingodb.pb.proxy.common.VectorWithId\x12\x41\n\tparameter\x18\x04 \x01(\x0b\x32..dingodb.pb.proxy.common.VectorSearchParameter\"f\n\x18VectorWithDistanceResult\x12J\n\x15vector_with_distances\x18\x01 \x03(\x0b\x32+.dingodb.pb.proxy.common.VectorWithDistance\"_\n\x14VectorSearchResponse\x12G\n\rbatch_results\x18\x01 \x03(\x0b\x32\x30.dingodb.pb.proxy.index.VectorWithDistanceResult\"K\n\x13VectorDeleteRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\x04\"*\n\x14VectorDeleteResponse\x12\x12\n\nkey_states\x18\x01 \x03(\x08\"T\n\x18VectorGetBorderIdRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x0f\n\x07get_min\x18\x03 \x01(\x08\"\'\n\x19VectorGetBorderIdResponse\x12\n\n\x02id\x18\x01 \x01(\x04\"\xf0\x02\n\x16VectorScanQueryRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x17\n\x0fvector_id_start\x18\x03 \x01(\x04\x12\x17\n\x0fis_reverse_scan\x18\x04 \x01(\x08\x12\x16\n\x0emax_scan_count\x18\x05 \x01(\x04\x12\x15\n\rvector_id_end\x18\x06 \x01(\x04\x12\x1b\n\x13without_vector_data\x18\x0b \x01(\x08\x12\x1b\n\x13without_scalar_data\x18\x0c \x01(\x08\x12\x15\n\rselected_keys\x18\r \x03(\t\x12\x1a\n\x12without_table_data\x18\x0e \x01(\x08\x12\x19\n\x11use_scalar_filter\x18\x14 \x01(\x08\x12\x44\n\x11scalar_for_filter\x18\x15 \x01(\x0b\x32).dingodb.pb.proxy.common.VectorScalarData\"Q\n\x17VectorScanQueryResponse\x12\x36\n\x07vectors\x18\x01 \x03(\x0b\x32%.dingodb.pb.proxy.common.VectorWithId\"H\n\x1dVectorGetRegionMetricsRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"^\n\x1eVectorGetRegionMetricsResponse\x12<\n\x07metrics\x18\x01 \x01(\x0b\x32+.dingodb.pb.proxy.common.VectorIndexMetrics\",\n\x0eVectorDistance\x12\x1a\n\x12internal_distances\x18\x01 \x03(\x02\"\xe2\x02\n\x19VectorCalcDistanceRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x11\n\tvector_id\x18\x03 \x01(\x04\x12=\n\x0e\x61lgorithm_type\x18\x04 \x01(\x0e\x32%.dingodb.pb.proxy.index.AlgorithmType\x12\x38\n\x0bmetric_type\x18\x05 \x01(\x0e\x32#.dingodb.pb.proxy.common.MetricType\x12\x38\n\x0fop_left_vectors\x18\x06 \x03(\x0b\x32\x1f.dingodb.pb.proxy.common.Vector\x12\x39\n\x10op_right_vectors\x18\x07 \x03(\x0b\x32\x1f.dingodb.pb.proxy.common.Vector\x12\x1b\n\x13is_return_normalize\x18\x08 \x01(\x08\"\xf5\x01\n\x1aVectorCalcDistanceResponse\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x38\n\x0fop_left_vectors\x18\x03 \x03(\x0b\x32\x1f.dingodb.pb.proxy.common.Vector\x12\x39\n\x10op_right_vectors\x18\x04 \x03(\x0b\x32\x1f.dingodb.pb.proxy.common.Vector\x12\x39\n\tdistances\x18\x05 \x03(\x0b\x32&.dingodb.pb.proxy.index.VectorDistance*O\n\rAlgorithmType\x12\x12\n\x0e\x41LGORITHM_NONE\x10\x00\x12\x13\n\x0f\x41LGORITHM_FAISS\x10\x01\x12\x15\n\x11\x41LGORITHM_HNSWLIB\x10\x02\x32\x9d\x07\n\x0cIndexService\x12`\n\tVectorAdd\x12(.dingodb.pb.proxy.index.VectorAddRequest\x1a).dingodb.pb.proxy.index.VectorAddResponse\x12`\n\tVectorGet\x12(.dingodb.pb.proxy.index.VectorGetRequest\x1a).dingodb.pb.proxy.index.VectorGetResponse\x12i\n\x0cVectorSearch\x12+.dingodb.pb.proxy.index.VectorSearchRequest\x1a,.dingodb.pb.proxy.index.VectorSearchResponse\x12i\n\x0cVectorDelete\x12+.dingodb.pb.proxy.index.VectorDeleteRequest\x1a,.dingodb.pb.proxy.index.VectorDeleteResponse\x12x\n\x11VectorGetBorderId\x12\x30.dingodb.pb.proxy.index.VectorGetBorderIdRequest\x1a\x31.dingodb.pb.proxy.index.VectorGetBorderIdResponse\x12r\n\x0fVectorScanQuery\x12..dingodb.pb.proxy.index.VectorScanQueryRequest\x1a/.dingodb.pb.proxy.index.VectorScanQueryResponse\x12\x87\x01\n\x16VectorGetRegionMetrics\x12\x35.dingodb.pb.proxy.index.VectorGetRegionMetricsRequest\x1a\x36.dingodb.pb.proxy.index.VectorGetRegionMetricsResponse\x12{\n\x12VectorCalcDistance\x12\x31.dingodb.pb.proxy.index.VectorCalcDistanceRequest\x1a\x32.dingodb.pb.proxy.index.VectorCalcDistanceResponseB\x1b\n\x16io.dingodb.proxy.index\x88\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11proxy_index.proto\x12\x16\x64ingodb.pb.proxy.index\x1a\x12proxy_common.proto\x1a\x11proxy_error.proto\"\x9f\x01\n\x10VectorAddRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x36\n\x07vectors\x18\x03 \x03(\x0b\x32%.dingodb.pb.proxy.common.VectorWithId\x12\x17\n\x0freplace_deleted\x18\x04 \x01(\x08\x12\x11\n\tis_update\x18\x05 \x01(\x08\"y\n\x11VectorAddResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12\x36\n\x07vectors\x18\x02 \x03(\x0b\x32%.dingodb.pb.proxy.common.VectorWithId\"\xbc\x01\n\x10VectorGetRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x12\n\nvector_ids\x18\x03 \x03(\x04\x12\x1b\n\x13without_vector_data\x18\x04 \x01(\x08\x12\x1b\n\x13without_scalar_data\x18\x05 \x01(\x08\x12\x15\n\rselected_keys\x18\x06 \x03(\t\x12\x1a\n\x12without_table_data\x18\x07 \x01(\x08\"y\n\x11VectorGetResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12\x36\n\x07vectors\x18\x02 \x03(\x0b\x32%.dingodb.pb.proxy.common.VectorWithId\"\xb9\x01\n\x13VectorSearchRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x36\n\x07vectors\x18\x03 \x03(\x0b\x32%.dingodb.pb.proxy.common.VectorWithId\x12\x41\n\tparameter\x18\x04 \x01(\x0b\x32..dingodb.pb.proxy.common.VectorSearchParameter\"f\n\x18VectorWithDistanceResult\x12J\n\x15vector_with_distances\x18\x01 \x03(\x0b\x32+.dingodb.pb.proxy.common.VectorWithDistance\"\x8d\x01\n\x14VectorSearchResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12G\n\rbatch_results\x18\x02 \x03(\x0b\x32\x30.dingodb.pb.proxy.index.VectorWithDistanceResult\"K\n\x13VectorDeleteRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x0b\n\x03ids\x18\x03 \x03(\x04\"X\n\x14VectorDeleteResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12\x12\n\nkey_states\x18\x02 \x03(\x08\"T\n\x18VectorGetBorderIdRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x0f\n\x07get_min\x18\x03 \x01(\x08\"U\n\x19VectorGetBorderIdResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12\n\n\x02id\x18\x02 \x01(\x04\"\xf0\x02\n\x16VectorScanQueryRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x17\n\x0fvector_id_start\x18\x03 \x01(\x04\x12\x17\n\x0fis_reverse_scan\x18\x04 \x01(\x08\x12\x16\n\x0emax_scan_count\x18\x05 \x01(\x04\x12\x15\n\rvector_id_end\x18\x06 \x01(\x04\x12\x1b\n\x13without_vector_data\x18\x0b \x01(\x08\x12\x1b\n\x13without_scalar_data\x18\x0c \x01(\x08\x12\x15\n\rselected_keys\x18\r \x03(\t\x12\x1a\n\x12without_table_data\x18\x0e \x01(\x08\x12\x19\n\x11use_scalar_filter\x18\x14 \x01(\x08\x12\x44\n\x11scalar_for_filter\x18\x15 \x01(\x0b\x32).dingodb.pb.proxy.common.VectorScalarData\"\x7f\n\x17VectorScanQueryResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12\x36\n\x07vectors\x18\x02 \x03(\x0b\x32%.dingodb.pb.proxy.common.VectorWithId\"H\n\x1dVectorGetRegionMetricsRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"\x8c\x01\n\x1eVectorGetRegionMetricsResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12<\n\x07metrics\x18\x02 \x01(\x0b\x32+.dingodb.pb.proxy.common.VectorIndexMetrics\"=\n\x12VectorCountRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"R\n\x13VectorCountResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12\r\n\x05\x63ount\x18\x02 \x01(\x04\x32\x88\x07\n\x0cIndexService\x12`\n\tVectorAdd\x12(.dingodb.pb.proxy.index.VectorAddRequest\x1a).dingodb.pb.proxy.index.VectorAddResponse\x12`\n\tVectorGet\x12(.dingodb.pb.proxy.index.VectorGetRequest\x1a).dingodb.pb.proxy.index.VectorGetResponse\x12i\n\x0cVectorSearch\x12+.dingodb.pb.proxy.index.VectorSearchRequest\x1a,.dingodb.pb.proxy.index.VectorSearchResponse\x12i\n\x0cVectorDelete\x12+.dingodb.pb.proxy.index.VectorDeleteRequest\x1a,.dingodb.pb.proxy.index.VectorDeleteResponse\x12x\n\x11VectorGetBorderId\x12\x30.dingodb.pb.proxy.index.VectorGetBorderIdRequest\x1a\x31.dingodb.pb.proxy.index.VectorGetBorderIdResponse\x12r\n\x0fVectorScanQuery\x12..dingodb.pb.proxy.index.VectorScanQueryRequest\x1a/.dingodb.pb.proxy.index.VectorScanQueryResponse\x12\x87\x01\n\x16VectorGetRegionMetrics\x12\x35.dingodb.pb.proxy.index.VectorGetRegionMetricsRequest\x1a\x36.dingodb.pb.proxy.index.VectorGetRegionMetricsResponse\x12\x66\n\x0bVectorCount\x12*.dingodb.pb.proxy.index.VectorCountRequest\x1a+.dingodb.pb.proxy.index.VectorCountResponseB\x1b\n\x16io.dingodb.proxy.index\x88\x01\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proxy_index_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\026io.dingodb.proxy.index\210\001\001'
-  _globals['_ALGORITHMTYPE']._serialized_start=2484
-  _globals['_ALGORITHMTYPE']._serialized_end=2563
-  _globals['_VECTORADDREQUEST']._serialized_start=66
-  _globals['_VECTORADDREQUEST']._serialized_end=225
-  _globals['_VECTORADDRESPONSE']._serialized_start=227
-  _globals['_VECTORADDRESPONSE']._serialized_end=302
-  _globals['_VECTORGETREQUEST']._serialized_start=305
-  _globals['_VECTORGETREQUEST']._serialized_end=493
-  _globals['_VECTORGETRESPONSE']._serialized_start=495
-  _globals['_VECTORGETRESPONSE']._serialized_end=570
-  _globals['_VECTORSEARCHREQUEST']._serialized_start=573
-  _globals['_VECTORSEARCHREQUEST']._serialized_end=758
-  _globals['_VECTORWITHDISTANCERESULT']._serialized_start=760
-  _globals['_VECTORWITHDISTANCERESULT']._serialized_end=862
-  _globals['_VECTORSEARCHRESPONSE']._serialized_start=864
-  _globals['_VECTORSEARCHRESPONSE']._serialized_end=959
-  _globals['_VECTORDELETEREQUEST']._serialized_start=961
-  _globals['_VECTORDELETEREQUEST']._serialized_end=1036
-  _globals['_VECTORDELETERESPONSE']._serialized_start=1038
-  _globals['_VECTORDELETERESPONSE']._serialized_end=1080
-  _globals['_VECTORGETBORDERIDREQUEST']._serialized_start=1082
-  _globals['_VECTORGETBORDERIDREQUEST']._serialized_end=1166
-  _globals['_VECTORGETBORDERIDRESPONSE']._serialized_start=1168
-  _globals['_VECTORGETBORDERIDRESPONSE']._serialized_end=1207
-  _globals['_VECTORSCANQUERYREQUEST']._serialized_start=1210
-  _globals['_VECTORSCANQUERYREQUEST']._serialized_end=1578
-  _globals['_VECTORSCANQUERYRESPONSE']._serialized_start=1580
-  _globals['_VECTORSCANQUERYRESPONSE']._serialized_end=1661
-  _globals['_VECTORGETREGIONMETRICSREQUEST']._serialized_start=1663
-  _globals['_VECTORGETREGIONMETRICSREQUEST']._serialized_end=1735
-  _globals['_VECTORGETREGIONMETRICSRESPONSE']._serialized_start=1737
-  _globals['_VECTORGETREGIONMETRICSRESPONSE']._serialized_end=1831
-  _globals['_VECTORDISTANCE']._serialized_start=1833
-  _globals['_VECTORDISTANCE']._serialized_end=1877
-  _globals['_VECTORCALCDISTANCEREQUEST']._serialized_start=1880
-  _globals['_VECTORCALCDISTANCEREQUEST']._serialized_end=2234
-  _globals['_VECTORCALCDISTANCERESPONSE']._serialized_start=2237
-  _globals['_VECTORCALCDISTANCERESPONSE']._serialized_end=2482
-  _globals['_INDEXSERVICE']._serialized_start=2566
-  _globals['_INDEXSERVICE']._serialized_end=3491
+  _globals['_VECTORADDREQUEST']._serialized_start=85
+  _globals['_VECTORADDREQUEST']._serialized_end=244
+  _globals['_VECTORADDRESPONSE']._serialized_start=246
+  _globals['_VECTORADDRESPONSE']._serialized_end=367
+  _globals['_VECTORGETREQUEST']._serialized_start=370
+  _globals['_VECTORGETREQUEST']._serialized_end=558
+  _globals['_VECTORGETRESPONSE']._serialized_start=560
+  _globals['_VECTORGETRESPONSE']._serialized_end=681
+  _globals['_VECTORSEARCHREQUEST']._serialized_start=684
+  _globals['_VECTORSEARCHREQUEST']._serialized_end=869
+  _globals['_VECTORWITHDISTANCERESULT']._serialized_start=871
+  _globals['_VECTORWITHDISTANCERESULT']._serialized_end=973
+  _globals['_VECTORSEARCHRESPONSE']._serialized_start=976
+  _globals['_VECTORSEARCHRESPONSE']._serialized_end=1117
+  _globals['_VECTORDELETEREQUEST']._serialized_start=1119
+  _globals['_VECTORDELETEREQUEST']._serialized_end=1194
+  _globals['_VECTORDELETERESPONSE']._serialized_start=1196
+  _globals['_VECTORDELETERESPONSE']._serialized_end=1284
+  _globals['_VECTORGETBORDERIDREQUEST']._serialized_start=1286
+  _globals['_VECTORGETBORDERIDREQUEST']._serialized_end=1370
+  _globals['_VECTORGETBORDERIDRESPONSE']._serialized_start=1372
+  _globals['_VECTORGETBORDERIDRESPONSE']._serialized_end=1457
+  _globals['_VECTORSCANQUERYREQUEST']._serialized_start=1460
+  _globals['_VECTORSCANQUERYREQUEST']._serialized_end=1828
+  _globals['_VECTORSCANQUERYRESPONSE']._serialized_start=1830
+  _globals['_VECTORSCANQUERYRESPONSE']._serialized_end=1957
+  _globals['_VECTORGETREGIONMETRICSREQUEST']._serialized_start=1959
+  _globals['_VECTORGETREGIONMETRICSREQUEST']._serialized_end=2031
+  _globals['_VECTORGETREGIONMETRICSRESPONSE']._serialized_start=2034
+  _globals['_VECTORGETREGIONMETRICSRESPONSE']._serialized_end=2174
+  _globals['_VECTORCOUNTREQUEST']._serialized_start=2176
+  _globals['_VECTORCOUNTREQUEST']._serialized_end=2237
+  _globals['_VECTORCOUNTRESPONSE']._serialized_start=2239
+  _globals['_VECTORCOUNTRESPONSE']._serialized_end=2321
+  _globals['_INDEXSERVICE']._serialized_start=2324
+  _globals['_INDEXSERVICE']._serialized_end=3228
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dingodb-0.0.8/dingodb/protos/proxy_index_pb2_grpc.py` & `dingodb-0.0.9/dingodb/protos/proxy_index_pb2_grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,18 +45,18 @@
                 response_deserializer=proxy__index__pb2.VectorScanQueryResponse.FromString,
                 )
         self.VectorGetRegionMetrics = channel.unary_unary(
                 '/dingodb.pb.proxy.index.IndexService/VectorGetRegionMetrics',
                 request_serializer=proxy__index__pb2.VectorGetRegionMetricsRequest.SerializeToString,
                 response_deserializer=proxy__index__pb2.VectorGetRegionMetricsResponse.FromString,
                 )
-        self.VectorCalcDistance = channel.unary_unary(
-                '/dingodb.pb.proxy.index.IndexService/VectorCalcDistance',
-                request_serializer=proxy__index__pb2.VectorCalcDistanceRequest.SerializeToString,
-                response_deserializer=proxy__index__pb2.VectorCalcDistanceResponse.FromString,
+        self.VectorCount = channel.unary_unary(
+                '/dingodb.pb.proxy.index.IndexService/VectorCount',
+                request_serializer=proxy__index__pb2.VectorCountRequest.SerializeToString,
+                response_deserializer=proxy__index__pb2.VectorCountResponse.FromString,
                 )
 
 
 class IndexServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def VectorAdd(self, request, context):
@@ -97,15 +97,15 @@
 
     def VectorGetRegionMetrics(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def VectorCalcDistance(self, request, context):
+    def VectorCount(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_IndexServiceServicer_to_server(servicer, server):
@@ -141,18 +141,18 @@
                     response_serializer=proxy__index__pb2.VectorScanQueryResponse.SerializeToString,
             ),
             'VectorGetRegionMetrics': grpc.unary_unary_rpc_method_handler(
                     servicer.VectorGetRegionMetrics,
                     request_deserializer=proxy__index__pb2.VectorGetRegionMetricsRequest.FromString,
                     response_serializer=proxy__index__pb2.VectorGetRegionMetricsResponse.SerializeToString,
             ),
-            'VectorCalcDistance': grpc.unary_unary_rpc_method_handler(
-                    servicer.VectorCalcDistance,
-                    request_deserializer=proxy__index__pb2.VectorCalcDistanceRequest.FromString,
-                    response_serializer=proxy__index__pb2.VectorCalcDistanceResponse.SerializeToString,
+            'VectorCount': grpc.unary_unary_rpc_method_handler(
+                    servicer.VectorCount,
+                    request_deserializer=proxy__index__pb2.VectorCountRequest.FromString,
+                    response_serializer=proxy__index__pb2.VectorCountResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'dingodb.pb.proxy.index.IndexService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -276,22 +276,22 @@
         return grpc.experimental.unary_unary(request, target, '/dingodb.pb.proxy.index.IndexService/VectorGetRegionMetrics',
             proxy__index__pb2.VectorGetRegionMetricsRequest.SerializeToString,
             proxy__index__pb2.VectorGetRegionMetricsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def VectorCalcDistance(request,
+    def VectorCount(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/dingodb.pb.proxy.index.IndexService/VectorCalcDistance',
-            proxy__index__pb2.VectorCalcDistanceRequest.SerializeToString,
-            proxy__index__pb2.VectorCalcDistanceResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/dingodb.pb.proxy.index.IndexService/VectorCount',
+            proxy__index__pb2.VectorCountRequest.SerializeToString,
+            proxy__index__pb2.VectorCountResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `dingodb-0.0.8/dingodb/protos/proxy_meta_pb2.py` & `dingodb-0.0.9/dingodb/protos/proxy_meta_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,59 +8,60 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 import proxy_common_pb2 as proxy__common__pb2
+import proxy_error_pb2 as proxy__error__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10proxy_meta.proto\x12\x15\x64ingodb.pb.proxy.meta\x1a\x12proxy_common.proto\"Q\n\x19PartitionDetailDefinition\x12\x11\n\tpart_name\x18\x01 \x01(\t\x12\x10\n\x08operator\x18\x02 \x01(\t\x12\x0f\n\x07operand\x18\x03 \x03(\t\"v\n\rPartitionRule\x12\x11\n\tfunc_name\x18\x01 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\x12\x41\n\x07\x64\x65tails\x18\x03 \x03(\x0b\x32\x30.dingodb.pb.proxy.meta.PartitionDetailDefinition\"\xf7\x01\n\x0fIndexDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\r\x12=\n\x0findex_partition\x18\x03 \x01(\x0b\x32$.dingodb.pb.proxy.meta.PartitionRule\x12\x0f\n\x07replica\x18\x04 \x01(\r\x12@\n\x0findex_parameter\x18\x05 \x01(\x0b\x32\'.dingodb.pb.proxy.common.IndexParameter\x12\x1b\n\x13with_auto_increment\x18\x06 \x01(\x08\x12\x16\n\x0e\x61uto_increment\x18\x07 \x01(\x04\"e\n\x12\x43reateIndexRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12:\n\ndefinition\x18\x02 \x01(\x0b\x32&.dingodb.pb.proxy.meta.IndexDefinition\"$\n\x13\x43reateIndexResponse\x12\r\n\x05state\x18\x01 \x01(\x08\"e\n\x12UpdateIndexRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12:\n\ndefinition\x18\x02 \x01(\x0b\x32&.dingodb.pb.proxy.meta.IndexDefinition\"$\n\x13UpdateIndexResponse\x12\r\n\x05state\x18\x01 \x01(\x08\"Y\n\x18UpdateMaxElementsRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x14\n\x0cmax_elements\x18\x03 \x01(\x05\"*\n\x19UpdateMaxElementsResponse\x12\r\n\x05state\x18\x01 \x01(\x08\"=\n\x12\x44\x65leteIndexRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"$\n\x13\x44\x65leteIndexResponse\x12\r\n\x05state\x18\x01 \x01(\x08\":\n\x0fGetIndexRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"N\n\x10GetIndexResponse\x12:\n\ndefinition\x18\x01 \x01(\x0b\x32&.dingodb.pb.proxy.meta.IndexDefinition\"(\n\x11GetIndexesRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\"Q\n\x12GetIndexesResponse\x12;\n\x0b\x64\x65\x66initions\x18\x01 \x03(\x0b\x32&.dingodb.pb.proxy.meta.IndexDefinition\"+\n\x14GetIndexNamesRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\"&\n\x15GetIndexNamesResponse\x12\r\n\x05names\x18\x01 \x03(\t\"A\n\x16GetIndexMetricsRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"\x85\x02\n\x17GetIndexMetricsResponse\x12\x12\n\nrows_count\x18\x01 \x01(\x04\x12\x0f\n\x07min_key\x18\x02 \x01(\x0c\x12\x0f\n\x07max_key\x18\x03 \x01(\x0c\x12\x12\n\npart_count\x18\x04 \x01(\x04\x12<\n\nindex_type\x18\x05 \x01(\x0e\x32(.dingodb.pb.proxy.common.VectorIndexType\x12\x15\n\rcurrent_count\x18\x06 \x01(\x04\x12\x15\n\rdeleted_count\x18\x07 \x01(\x04\x12\x0e\n\x06max_id\x18\x08 \x01(\x04\x12\x0e\n\x06min_id\x18\t \x01(\x04\x12\x14\n\x0cmemory_bytes\x18\n \x01(\x04\x32\xd5\x06\n\x0bMetaService\x12\x64\n\x0b\x43reateIndex\x12).dingodb.pb.proxy.meta.CreateIndexRequest\x1a*.dingodb.pb.proxy.meta.CreateIndexResponse\x12\x64\n\x0bUpdateIndex\x12).dingodb.pb.proxy.meta.UpdateIndexRequest\x1a*.dingodb.pb.proxy.meta.UpdateIndexResponse\x12v\n\x11UpdateMaxElements\x12/.dingodb.pb.proxy.meta.UpdateMaxElementsRequest\x1a\x30.dingodb.pb.proxy.meta.UpdateMaxElementsResponse\x12\x64\n\x0b\x44\x65leteIndex\x12).dingodb.pb.proxy.meta.DeleteIndexRequest\x1a*.dingodb.pb.proxy.meta.DeleteIndexResponse\x12[\n\x08GetIndex\x12&.dingodb.pb.proxy.meta.GetIndexRequest\x1a\'.dingodb.pb.proxy.meta.GetIndexResponse\x12\x61\n\nGetIndexes\x12(.dingodb.pb.proxy.meta.GetIndexesRequest\x1a).dingodb.pb.proxy.meta.GetIndexesResponse\x12j\n\rGetIndexNames\x12+.dingodb.pb.proxy.meta.GetIndexNamesRequest\x1a,.dingodb.pb.proxy.meta.GetIndexNamesResponse\x12p\n\x0fGetIndexMetrics\x12-.dingodb.pb.proxy.meta.GetIndexMetricsRequest\x1a..dingodb.pb.proxy.meta.GetIndexMetricsResponseB\x1a\n\x15io.dingodb.proxy.meta\x88\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10proxy_meta.proto\x12\x15\x64ingodb.pb.proxy.meta\x1a\x12proxy_common.proto\x1a\x11proxy_error.proto\"Q\n\x19PartitionDetailDefinition\x12\x11\n\tpart_name\x18\x01 \x01(\t\x12\x10\n\x08operator\x18\x02 \x01(\t\x12\x0f\n\x07operand\x18\x03 \x03(\t\"v\n\rPartitionRule\x12\x11\n\tfunc_name\x18\x01 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\x12\x41\n\x07\x64\x65tails\x18\x03 \x03(\x0b\x32\x30.dingodb.pb.proxy.meta.PartitionDetailDefinition\"\xf7\x01\n\x0fIndexDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\r\x12=\n\x0findex_partition\x18\x03 \x01(\x0b\x32$.dingodb.pb.proxy.meta.PartitionRule\x12\x0f\n\x07replica\x18\x04 \x01(\r\x12@\n\x0findex_parameter\x18\x05 \x01(\x0b\x32\'.dingodb.pb.proxy.common.IndexParameter\x12\x1b\n\x13with_auto_increment\x18\x06 \x01(\x08\x12\x16\n\x0e\x61uto_increment\x18\x07 \x01(\x04\"e\n\x12\x43reateIndexRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12:\n\ndefinition\x18\x02 \x01(\x0b\x32&.dingodb.pb.proxy.meta.IndexDefinition\"R\n\x13\x43reateIndexResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12\r\n\x05state\x18\x02 \x01(\x08\"e\n\x12UpdateIndexRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12:\n\ndefinition\x18\x02 \x01(\x0b\x32&.dingodb.pb.proxy.meta.IndexDefinition\"R\n\x13UpdateIndexResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12\r\n\x05state\x18\x02 \x01(\x08\"Y\n\x18UpdateMaxElementsRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x14\n\x0cmax_elements\x18\x03 \x01(\x05\"X\n\x19UpdateMaxElementsResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12\r\n\x05state\x18\x02 \x01(\x08\"=\n\x12\x44\x65leteIndexRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"R\n\x13\x44\x65leteIndexResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12\r\n\x05state\x18\x02 \x01(\x08\":\n\x0fGetIndexRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"|\n\x10GetIndexResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12:\n\ndefinition\x18\x02 \x01(\x0b\x32&.dingodb.pb.proxy.meta.IndexDefinition\"(\n\x11GetIndexesRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\"\x7f\n\x12GetIndexesResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12;\n\x0b\x64\x65\x66initions\x18\x02 \x03(\x0b\x32&.dingodb.pb.proxy.meta.IndexDefinition\"+\n\x14GetIndexNamesRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\"T\n\x15GetIndexNamesResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12\r\n\x05names\x18\x02 \x03(\t\"A\n\x16GetIndexMetricsRequest\x12\x13\n\x0bschema_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"\xb3\x02\n\x17GetIndexMetricsResponse\x12,\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x1d.dingodb.pb.proxy.error.Error\x12\x12\n\nrows_count\x18\x02 \x01(\x04\x12\x0f\n\x07min_key\x18\x03 \x01(\x0c\x12\x0f\n\x07max_key\x18\x04 \x01(\x0c\x12\x12\n\npart_count\x18\x05 \x01(\x04\x12<\n\nindex_type\x18\x06 \x01(\x0e\x32(.dingodb.pb.proxy.common.VectorIndexType\x12\x15\n\rcurrent_count\x18\x07 \x01(\x04\x12\x15\n\rdeleted_count\x18\x08 \x01(\x04\x12\x0e\n\x06max_id\x18\t \x01(\x04\x12\x0e\n\x06min_id\x18\n \x01(\x04\x12\x14\n\x0cmemory_bytes\x18\x0b \x01(\x04\x32\xd5\x06\n\x0bMetaService\x12\x64\n\x0b\x43reateIndex\x12).dingodb.pb.proxy.meta.CreateIndexRequest\x1a*.dingodb.pb.proxy.meta.CreateIndexResponse\x12\x64\n\x0bUpdateIndex\x12).dingodb.pb.proxy.meta.UpdateIndexRequest\x1a*.dingodb.pb.proxy.meta.UpdateIndexResponse\x12v\n\x11UpdateMaxElements\x12/.dingodb.pb.proxy.meta.UpdateMaxElementsRequest\x1a\x30.dingodb.pb.proxy.meta.UpdateMaxElementsResponse\x12\x64\n\x0b\x44\x65leteIndex\x12).dingodb.pb.proxy.meta.DeleteIndexRequest\x1a*.dingodb.pb.proxy.meta.DeleteIndexResponse\x12[\n\x08GetIndex\x12&.dingodb.pb.proxy.meta.GetIndexRequest\x1a\'.dingodb.pb.proxy.meta.GetIndexResponse\x12\x61\n\nGetIndexes\x12(.dingodb.pb.proxy.meta.GetIndexesRequest\x1a).dingodb.pb.proxy.meta.GetIndexesResponse\x12j\n\rGetIndexNames\x12+.dingodb.pb.proxy.meta.GetIndexNamesRequest\x1a,.dingodb.pb.proxy.meta.GetIndexNamesResponse\x12p\n\x0fGetIndexMetrics\x12-.dingodb.pb.proxy.meta.GetIndexMetricsRequest\x1a..dingodb.pb.proxy.meta.GetIndexMetricsResponseB\x1a\n\x15io.dingodb.proxy.meta\x88\x01\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proxy_meta_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\025io.dingodb.proxy.meta\210\001\001'
-  _globals['_PARTITIONDETAILDEFINITION']._serialized_start=63
-  _globals['_PARTITIONDETAILDEFINITION']._serialized_end=144
-  _globals['_PARTITIONRULE']._serialized_start=146
-  _globals['_PARTITIONRULE']._serialized_end=264
-  _globals['_INDEXDEFINITION']._serialized_start=267
-  _globals['_INDEXDEFINITION']._serialized_end=514
-  _globals['_CREATEINDEXREQUEST']._serialized_start=516
-  _globals['_CREATEINDEXREQUEST']._serialized_end=617
-  _globals['_CREATEINDEXRESPONSE']._serialized_start=619
-  _globals['_CREATEINDEXRESPONSE']._serialized_end=655
-  _globals['_UPDATEINDEXREQUEST']._serialized_start=657
-  _globals['_UPDATEINDEXREQUEST']._serialized_end=758
-  _globals['_UPDATEINDEXRESPONSE']._serialized_start=760
-  _globals['_UPDATEINDEXRESPONSE']._serialized_end=796
-  _globals['_UPDATEMAXELEMENTSREQUEST']._serialized_start=798
-  _globals['_UPDATEMAXELEMENTSREQUEST']._serialized_end=887
-  _globals['_UPDATEMAXELEMENTSRESPONSE']._serialized_start=889
-  _globals['_UPDATEMAXELEMENTSRESPONSE']._serialized_end=931
-  _globals['_DELETEINDEXREQUEST']._serialized_start=933
-  _globals['_DELETEINDEXREQUEST']._serialized_end=994
-  _globals['_DELETEINDEXRESPONSE']._serialized_start=996
-  _globals['_DELETEINDEXRESPONSE']._serialized_end=1032
-  _globals['_GETINDEXREQUEST']._serialized_start=1034
-  _globals['_GETINDEXREQUEST']._serialized_end=1092
-  _globals['_GETINDEXRESPONSE']._serialized_start=1094
-  _globals['_GETINDEXRESPONSE']._serialized_end=1172
-  _globals['_GETINDEXESREQUEST']._serialized_start=1174
-  _globals['_GETINDEXESREQUEST']._serialized_end=1214
-  _globals['_GETINDEXESRESPONSE']._serialized_start=1216
-  _globals['_GETINDEXESRESPONSE']._serialized_end=1297
-  _globals['_GETINDEXNAMESREQUEST']._serialized_start=1299
-  _globals['_GETINDEXNAMESREQUEST']._serialized_end=1342
-  _globals['_GETINDEXNAMESRESPONSE']._serialized_start=1344
-  _globals['_GETINDEXNAMESRESPONSE']._serialized_end=1382
-  _globals['_GETINDEXMETRICSREQUEST']._serialized_start=1384
-  _globals['_GETINDEXMETRICSREQUEST']._serialized_end=1449
-  _globals['_GETINDEXMETRICSRESPONSE']._serialized_start=1452
-  _globals['_GETINDEXMETRICSRESPONSE']._serialized_end=1713
-  _globals['_METASERVICE']._serialized_start=1716
-  _globals['_METASERVICE']._serialized_end=2569
+  _globals['_PARTITIONDETAILDEFINITION']._serialized_start=82
+  _globals['_PARTITIONDETAILDEFINITION']._serialized_end=163
+  _globals['_PARTITIONRULE']._serialized_start=165
+  _globals['_PARTITIONRULE']._serialized_end=283
+  _globals['_INDEXDEFINITION']._serialized_start=286
+  _globals['_INDEXDEFINITION']._serialized_end=533
+  _globals['_CREATEINDEXREQUEST']._serialized_start=535
+  _globals['_CREATEINDEXREQUEST']._serialized_end=636
+  _globals['_CREATEINDEXRESPONSE']._serialized_start=638
+  _globals['_CREATEINDEXRESPONSE']._serialized_end=720
+  _globals['_UPDATEINDEXREQUEST']._serialized_start=722
+  _globals['_UPDATEINDEXREQUEST']._serialized_end=823
+  _globals['_UPDATEINDEXRESPONSE']._serialized_start=825
+  _globals['_UPDATEINDEXRESPONSE']._serialized_end=907
+  _globals['_UPDATEMAXELEMENTSREQUEST']._serialized_start=909
+  _globals['_UPDATEMAXELEMENTSREQUEST']._serialized_end=998
+  _globals['_UPDATEMAXELEMENTSRESPONSE']._serialized_start=1000
+  _globals['_UPDATEMAXELEMENTSRESPONSE']._serialized_end=1088
+  _globals['_DELETEINDEXREQUEST']._serialized_start=1090
+  _globals['_DELETEINDEXREQUEST']._serialized_end=1151
+  _globals['_DELETEINDEXRESPONSE']._serialized_start=1153
+  _globals['_DELETEINDEXRESPONSE']._serialized_end=1235
+  _globals['_GETINDEXREQUEST']._serialized_start=1237
+  _globals['_GETINDEXREQUEST']._serialized_end=1295
+  _globals['_GETINDEXRESPONSE']._serialized_start=1297
+  _globals['_GETINDEXRESPONSE']._serialized_end=1421
+  _globals['_GETINDEXESREQUEST']._serialized_start=1423
+  _globals['_GETINDEXESREQUEST']._serialized_end=1463
+  _globals['_GETINDEXESRESPONSE']._serialized_start=1465
+  _globals['_GETINDEXESRESPONSE']._serialized_end=1592
+  _globals['_GETINDEXNAMESREQUEST']._serialized_start=1594
+  _globals['_GETINDEXNAMESREQUEST']._serialized_end=1637
+  _globals['_GETINDEXNAMESRESPONSE']._serialized_start=1639
+  _globals['_GETINDEXNAMESRESPONSE']._serialized_end=1723
+  _globals['_GETINDEXMETRICSREQUEST']._serialized_start=1725
+  _globals['_GETINDEXMETRICSREQUEST']._serialized_end=1790
+  _globals['_GETINDEXMETRICSRESPONSE']._serialized_start=1793
+  _globals['_GETINDEXMETRICSRESPONSE']._serialized_end=2100
+  _globals['_METASERVICE']._serialized_start=2103
+  _globals['_METASERVICE']._serialized_end=2956
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dingodb-0.0.8/dingodb/protos/proxy_meta_pb2_grpc.py` & `dingodb-0.0.9/dingodb/protos/proxy_meta_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dingodb-0.0.8/dingodb.egg-info/PKG-INFO` & `dingodb-0.0.9/dingodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingodb
-Version: 0.0.8
+Version: 0.0.9
 Summary: dingodb is dingodb sdk
 Home-page: https://www.dingodb.com/
 Author: DingoDB
 Author-email: dingodb@zetyun.com
 License: Proprietary License
 Project-URL: Homepage, https://www.dingodb.com/
 Project-URL: Documentation, https://dingodb.readthedocs.io/en/latest/
```

### Comparing `dingodb-0.0.8/dingodb.egg-info/SOURCES.txt` & `dingodb-0.0.9/dingodb.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 dingodb.egg-info/dependency_links.txt
 dingodb.egg-info/requires.txt
 dingodb.egg-info/top_level.txt
 dingodb/grpc/__init__.py
 dingodb/grpc/grpc_config.py
 dingodb/grpc/grpc_db.py
 dingodb/grpc/grpc_dingo_param.py
+dingodb/grpc/json_format.py
 dingodb/protos/__init__.py
 dingodb/protos/proxy_common_pb2.py
 dingodb/protos/proxy_common_pb2_grpc.py
+dingodb/protos/proxy_error_pb2.py
+dingodb/protos/proxy_error_pb2_grpc.py
 dingodb/protos/proxy_index_pb2.py
 dingodb/protos/proxy_index_pb2_grpc.py
 dingodb/protos/proxy_meta_pb2.py
 dingodb/protos/proxy_meta_pb2_grpc.py
```

### Comparing `dingodb-0.0.8/setup.py` & `dingodb-0.0.9/setup.py`

 * *Files identical despite different names*

