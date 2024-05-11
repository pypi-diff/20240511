# Comparing `tmp/stac_fastapi_opensearch-2.4.1.tar.gz` & `tmp/stac_fastapi_opensearch-3.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_opensearch-2.4.1.tar", last modified: Mon May  6 16:32:55 2024, max compression
+gzip compressed data, was "stac_fastapi_opensearch-3.0.0a0.tar", last modified: Sat May 11 12:06:43 2024, max compression
```

## Comparing `stac_fastapi_opensearch-2.4.1.tar` & `stac_fastapi_opensearch-3.0.0a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:32:55.127369 stac_fastapi_opensearch-2.4.1/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1462 2024-05-06 16:32:55.126990 stac_fastapi_opensearch-2.4.1/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)       92 2024-03-19 04:19:17.000000 stac_fastapi_opensearch-2.4.1/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)      110 2024-05-06 16:32:55.137972 stac_fastapi_opensearch-2.4.1/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1541 2024-05-06 15:55:42.000000 stac_fastapi_opensearch-2.4.1/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:32:55.068071 stac_fastapi_opensearch-2.4.1/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:32:55.119995 stac_fastapi_opensearch-2.4.1/stac_fastapi/opensearch/
--rw-r--r--   0 primeradiant   (501) staff       (20)       28 2024-02-08 06:37:21.000000 stac_fastapi_opensearch-2.4.1/stac_fastapi/opensearch/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     3272 2024-05-02 09:57:35.000000 stac_fastapi_opensearch-2.4.1/stac_fastapi/opensearch/app.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2366 2024-04-09 14:42:19.000000 stac_fastapi_opensearch-2.4.1/stac_fastapi/opensearch/config.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    34073 2024-03-19 04:19:17.000000 stac_fastapi_opensearch-2.4.1/stac_fastapi/opensearch/database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-05-06 16:32:29.000000 stac_fastapi_opensearch-2.4.1/stac_fastapi/opensearch/version.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:32:55.120922 stac_fastapi_opensearch-2.4.1/stac_fastapi.opensearch.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1462 2024-05-06 16:32:55.000000 stac_fastapi_opensearch-2.4.1/stac_fastapi.opensearch.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      536 2024-05-06 16:32:55.000000 stac_fastapi_opensearch-2.4.1/stac_fastapi.opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-06 16:32:55.000000 stac_fastapi_opensearch-2.4.1/stac_fastapi.opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       76 2024-05-06 16:32:55.000000 stac_fastapi_opensearch-2.4.1/stac_fastapi.opensearch.egg-info/entry_points.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-04 04:08:14.000000 stac_fastapi_opensearch-2.4.1/stac_fastapi.opensearch.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      240 2024-05-06 16:32:55.000000 stac_fastapi_opensearch-2.4.1/stac_fastapi.opensearch.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-06 16:32:55.000000 stac_fastapi_opensearch-2.4.1/stac_fastapi.opensearch.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:06:43.661950 stac_fastapi_opensearch-3.0.0a0/
+-rw-r--r--   0 primeradiant   (501) staff       (20)    14904 2024-05-11 12:06:43.661594 stac_fastapi_opensearch-3.0.0a0/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)    13479 2024-05-11 10:42:06.000000 stac_fastapi_opensearch-3.0.0a0/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)      110 2024-05-11 12:06:43.693953 stac_fastapi_opensearch-3.0.0a0/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1593 2024-05-11 10:41:59.000000 stac_fastapi_opensearch-3.0.0a0/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:06:43.489185 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:06:43.652075 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       28 2024-02-08 06:37:21.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3272 2024-05-02 09:57:35.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/app.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2366 2024-04-09 14:42:19.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/config.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    35204 2024-05-11 10:43:40.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       47 2024-05-11 10:41:59.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/version.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:06:43.652884 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)    14904 2024-05-11 12:06:43.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      536 2024-05-11 12:06:43.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-11 12:06:43.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       76 2024-05-11 12:06:43.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/entry_points.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-04 04:08:14.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      242 2024-05-11 12:06:43.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-11 12:06:43.000000 stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/top_level.txt
```

### Comparing `stac_fastapi_opensearch-2.4.1/setup.py` & `stac_fastapi_opensearch-3.0.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "stac-fastapi.core==2.4.1",
+    "stac-fastapi.core==3.0.0a0",
     "opensearch-py==2.4.2",
     "opensearch-py[async]==2.4.2",
     "uvicorn",
     "starlette",
 ]
 
 extra_reqs = {
@@ -37,14 +37,15 @@
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ],
     url="https://github.com/stac-utils/stac-fastapi-elasticsearch-opensearch",
     license="MIT",
     packages=find_namespace_packages(),
     zip_safe=False,
     install_requires=install_requires,
```

### Comparing `stac_fastapi_opensearch-2.4.1/stac_fastapi/opensearch/app.py` & `stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/app.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_opensearch-2.4.1/stac_fastapi/opensearch/config.py` & `stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_opensearch-2.4.1/stac_fastapi/opensearch/database_logic.py` & `stac_fastapi_opensearch-3.0.0a0/stac_fastapi/opensearch/database_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from opensearchpy import exceptions, helpers
 from opensearchpy.exceptions import TransportError
 from opensearchpy.helpers.query import Q
 from opensearchpy.helpers.search import Search
 
 from stac_fastapi.core import serializers
 from stac_fastapi.core.extensions import filter
-from stac_fastapi.core.utilities import bbox2polygon
+from stac_fastapi.core.utilities import MAX_LIMIT, bbox2polygon
 from stac_fastapi.opensearch.config import (
     AsyncOpensearchSettings as AsyncSearchSettings,
 )
 from stac_fastapi.opensearch.config import OpensearchSettings as SyncSearchSettings
 from stac_fastapi.types.errors import ConflictError, NotFoundError
 from stac_fastapi.types.stac import Collection, Item
 
@@ -531,17 +531,36 @@
         else:
             search = search.filter("term", **{field: value})
 
         return search
 
     @staticmethod
     def apply_cql2_filter(search: Search, _filter: Optional[Dict[str, Any]]):
-        """Database logic to perform query for search endpoint."""
+        """
+        Apply a CQL2 filter to an Opensearch Search object.
+
+        This method transforms a dictionary representing a CQL2 filter into an Opensearch query
+        and applies it to the provided Search object. If the filter is None, the original Search
+        object is returned unmodified.
+
+        Args:
+            search (Search): The Opensearch Search object to which the filter will be applied.
+            _filter (Optional[Dict[str, Any]]): The filter in dictionary form that needs to be applied
+                                                to the search. The dictionary should follow the structure
+                                                required by the `to_es` function which converts it
+                                                to an Opensearch query.
+
+        Returns:
+            Search: The modified Search object with the filter applied if a filter is provided,
+                    otherwise the original Search object.
+        """
         if _filter is not None:
-            search = search.filter(filter.Clause.parse_obj(_filter).to_es())
+            es_query = filter.to_es(_filter)
+            search = search.filter(es_query)
+
         return search
 
     @staticmethod
     def populate_sort(sortby: List) -> Optional[Dict[str, Dict[str, str]]]:
         """Database logic to sort search instance."""
         if sortby:
             return {s.field: {"order": s.direction} for s in sortby}
@@ -578,27 +597,36 @@
         Raises:
             NotFoundError: If the collections specified in `collection_ids` do not exist.
         """
         search_body: Dict[str, Any] = {}
         query = search.query.to_dict() if search.query else None
         if query:
             search_body["query"] = query
+
+        search_after = None
+
         if token:
             search_after = urlsafe_b64decode(token.encode()).decode().split(",")
+        if search_after:
             search_body["search_after"] = search_after
+
         search_body["sort"] = sort if sort else DEFAULT_SORT
 
         index_param = indices(collection_ids)
 
+        max_result_window = MAX_LIMIT
+
+        size_limit = min(limit + 1, max_result_window)
+
         search_task = asyncio.create_task(
             self.client.search(
                 index=index_param,
                 ignore_unavailable=ignore_unavailable,
                 body=search_body,
-                size=limit,
+                size=size_limit,
             )
         )
 
         count_task = asyncio.create_task(
             self.client.count(
                 index=index_param,
                 ignore_unavailable=ignore_unavailable,
@@ -608,32 +636,35 @@
 
         try:
             es_response = await search_task
         except exceptions.NotFoundError:
             raise NotFoundError(f"Collections '{collection_ids}' do not exist")
 
         hits = es_response["hits"]["hits"]
-        items = (hit["_source"] for hit in hits)
+        items = (hit["_source"] for hit in hits[:limit])
 
         next_token = None
-        if hits and (sort_array := hits[-1].get("sort")):
-            next_token = urlsafe_b64encode(
-                ",".join([str(x) for x in sort_array]).encode()
-            ).decode()
-
-        # (1) count should not block returning results, so don't wait for it to be done
-        # (2) don't cancel the task so that it will populate the ES cache for subsequent counts
-        maybe_count = None
+        if len(hits) > limit and limit < max_result_window:
+            if hits and (sort_array := hits[limit - 1].get("sort")):
+                next_token = urlsafe_b64encode(
+                    ",".join([str(x) for x in sort_array]).encode()
+                ).decode()
+
+        matched = (
+            es_response["hits"]["total"]["value"]
+            if es_response["hits"]["total"]["relation"] == "eq"
+            else None
+        )
         if count_task.done():
             try:
-                maybe_count = count_task.result().get("count")
+                matched = count_task.result().get("count")
             except Exception as e:
                 logger.error(f"Count task failed: {e}")
 
-        return items, maybe_count, next_token
+        return items, matched, next_token
 
     """ TRANSACTION LOGIC """
 
     async def check_collection_exists(self, collection_id: str):
         """Database logic to check if a collection exists."""
         if not await self.client.exists(index=COLLECTIONS_INDEX, id=collection_id):
             raise NotFoundError(f"Collection {collection_id} does not exist")
```

### Comparing `stac_fastapi_opensearch-2.4.1/stac_fastapi.opensearch.egg-info/SOURCES.txt` & `stac_fastapi_opensearch-3.0.0a0/stac_fastapi.opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

