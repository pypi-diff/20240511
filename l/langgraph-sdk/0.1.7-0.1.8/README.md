# Comparing `tmp/langgraph_sdk-0.1.7.tar.gz` & `tmp/langgraph_sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph_sdk-0.1.7.tar", max compression
+gzip compressed data, was "langgraph_sdk-0.1.8.tar", max compression
```

## Comparing `langgraph_sdk-0.1.7.tar` & `langgraph_sdk-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       12 2024-05-02 00:35:49.778092 langgraph_sdk-0.1.7/README.md
--rw-r--r--   0        0        0       70 2024-05-02 17:41:01.189167 langgraph_sdk-0.1.7/langgraph_sdk/__init__.py
--rw-r--r--   0        0        0    11514 2024-05-09 22:54:49.457337 langgraph_sdk-0.1.7/langgraph_sdk/client.py
--rw-r--r--   0        0        0     3212 2024-05-03 18:21:58.272136 langgraph_sdk-0.1.7/langgraph_sdk/schema.py
--rw-r--r--   0        0        0     1004 2024-05-09 22:57:57.764341 langgraph_sdk-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 langgraph_sdk-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-05-02 00:35:49.778092 langgraph_sdk-0.1.8/README.md
+-rw-r--r--   0        0        0       70 2024-05-02 17:41:01.189167 langgraph_sdk-0.1.8/langgraph_sdk/__init__.py
+-rw-r--r--   0        0        0    11521 2024-05-10 23:22:35.925150 langgraph_sdk-0.1.8/langgraph_sdk/client.py
+-rw-r--r--   0        0        0     3212 2024-05-03 18:21:58.272136 langgraph_sdk-0.1.8/langgraph_sdk/schema.py
+-rw-r--r--   0        0        0     1004 2024-05-11 00:20:29.377803 langgraph_sdk-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 langgraph_sdk-0.1.8/PKG-INFO
```

### Comparing `langgraph_sdk-0.1.7/langgraph_sdk/client.py` & `langgraph_sdk-0.1.8/langgraph_sdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         """Get a thread by ID."""
         return await self.http.get(f"/threads/{thread_id}")
 
     async def create(self, *, metadata: Metadata = None) -> Thread:
         """Create a new thread."""
         return await self.http.post("/threads", json={"metadata": metadata})
 
-    async def upsert(self, thread_id: str, *, metadata: Metadata) -> Thread:
+    async def upsert(self, thread_id: str, *, metadata: Metadata = None) -> Thread:
         """Create or update a thread."""
         return await self.http.put(f"/threads/{thread_id}", json={"metadata": metadata})
 
     async def delete(self, thread_id: str) -> None:
         """Delete a thread."""
         await self.http.delete(f"/threads/{thread_id}")
```

### Comparing `langgraph_sdk-0.1.7/langgraph_sdk/schema.py` & `langgraph_sdk-0.1.8/langgraph_sdk/schema.py`

 * *Files identical despite different names*

### Comparing `langgraph_sdk-0.1.7/pyproject.toml` & `langgraph_sdk-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langgraph-sdk"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Nuno Campos <nuno@langchain.dev>"]
 readme = "README.md"
 packages = [{include = "langgraph_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.9.0,<4.0"
```

### Comparing `langgraph_sdk-0.1.7/PKG-INFO` & `langgraph_sdk-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langgraph-sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Nuno Campos
 Author-email: nuno@langchain.dev
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

