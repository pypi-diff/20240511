# Comparing `tmp/stac_fastapi_elasticsearch-2.4.1.tar.gz` & `tmp/stac_fastapi_elasticsearch-3.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_elasticsearch-2.4.1.tar", last modified: Mon May  6 16:29:51 2024, max compression
+gzip compressed data, was "stac_fastapi_elasticsearch-3.0.0a0.tar", last modified: Sat May 11 12:04:26 2024, max compression
```

## Comparing `stac_fastapi_elasticsearch-2.4.1.tar` & `stac_fastapi_elasticsearch-3.0.0a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:29:51.142038 stac_fastapi_elasticsearch-2.4.1/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1547 2024-05-06 16:29:51.141800 stac_fastapi_elasticsearch-2.4.1/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      101 2024-03-19 04:19:17.000000 stac_fastapi_elasticsearch-2.4.1/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)      113 2024-05-06 16:29:51.144104 stac_fastapi_elasticsearch-2.4.1/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1725 2024-05-06 15:55:57.000000 stac_fastapi_elasticsearch-2.4.1/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:29:51.042477 stac_fastapi_elasticsearch-2.4.1/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:29:51.138014 stac_fastapi_elasticsearch-2.4.1/stac_fastapi/elasticsearch/
--rw-r--r--   0 primeradiant   (501) staff       (20)       31 2024-01-31 03:57:09.000000 stac_fastapi_elasticsearch-2.4.1/stac_fastapi/elasticsearch/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     3293 2024-05-02 09:57:35.000000 stac_fastapi_elasticsearch-2.4.1/stac_fastapi/elasticsearch/app.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     2405 2024-04-09 14:42:19.000000 stac_fastapi_elasticsearch-2.4.1/stac_fastapi/elasticsearch/config.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    33316 2024-03-19 04:19:17.000000 stac_fastapi_elasticsearch-2.4.1/stac_fastapi/elasticsearch/database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-05-06 15:55:50.000000 stac_fastapi_elasticsearch-2.4.1/stac_fastapi/elasticsearch/version.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:29:51.139052 stac_fastapi_elasticsearch-2.4.1/stac_fastapi.elasticsearch.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1547 2024-05-06 16:29:51.000000 stac_fastapi_elasticsearch-2.4.1/stac_fastapi.elasticsearch.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      572 2024-05-06 16:29:51.000000 stac_fastapi_elasticsearch-2.4.1/stac_fastapi.elasticsearch.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-06 16:29:51.000000 stac_fastapi_elasticsearch-2.4.1/stac_fastapi.elasticsearch.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       82 2024-05-06 16:29:51.000000 stac_fastapi_elasticsearch-2.4.1/stac_fastapi.elasticsearch.egg-info/entry_points.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-03 03:16:23.000000 stac_fastapi_elasticsearch-2.4.1/stac_fastapi.elasticsearch.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      246 2024-05-06 16:29:51.000000 stac_fastapi_elasticsearch-2.4.1/stac_fastapi.elasticsearch.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-06 16:29:51.000000 stac_fastapi_elasticsearch-2.4.1/stac_fastapi.elasticsearch.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:04:26.977320 stac_fastapi_elasticsearch-3.0.0a0/
+-rw-r--r--   0 primeradiant   (501) staff       (20)    14981 2024-05-11 12:04:26.976882 stac_fastapi_elasticsearch-3.0.0a0/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)    13479 2024-05-11 10:42:06.000000 stac_fastapi_elasticsearch-3.0.0a0/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)      113 2024-05-11 12:04:26.979784 stac_fastapi_elasticsearch-3.0.0a0/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1777 2024-05-11 10:41:59.000000 stac_fastapi_elasticsearch-3.0.0a0/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:04:26.696045 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:04:26.935650 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       31 2024-01-31 03:57:09.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3293 2024-05-02 09:57:35.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/app.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     2405 2024-04-09 14:42:19.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/config.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    34398 2024-05-11 10:43:13.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       47 2024-05-11 10:41:59.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/version.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 12:04:26.938938 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)    14981 2024-05-11 12:04:25.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      572 2024-05-11 12:04:26.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-11 12:04:25.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       82 2024-05-11 12:04:25.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/entry_points.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-02-03 03:16:23.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      248 2024-05-11 12:04:25.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-11 12:04:25.000000 stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/top_level.txt
```

### Comparing `stac_fastapi_elasticsearch-2.4.1/setup.py` & `stac_fastapi_elasticsearch-3.0.0a0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "stac-fastapi.core==2.4.1",
+    "stac-fastapi.core==3.0.0a0",
     "elasticsearch[async]==8.11.0",
     "elasticsearch-dsl==8.11.0",
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
     packages=find_namespace_packages(exclude=["alembic", "tests", "scripts"]),
     zip_safe=False,
     install_requires=install_requires,
```

### Comparing `stac_fastapi_elasticsearch-2.4.1/stac_fastapi/elasticsearch/app.py` & `stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/app.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_elasticsearch-2.4.1/stac_fastapi/elasticsearch/config.py` & `stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_elasticsearch-2.4.1/stac_fastapi/elasticsearch/database_logic.py` & `stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi/elasticsearch/database_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import attr
 from elasticsearch_dsl import Q, Search
 
 from elasticsearch import exceptions, helpers  # type: ignore
 from stac_fastapi.core.extensions import filter
 from stac_fastapi.core.serializers import CollectionSerializer, ItemSerializer
-from stac_fastapi.core.utilities import bbox2polygon
+from stac_fastapi.core.utilities import MAX_LIMIT, bbox2polygon
 from stac_fastapi.elasticsearch.config import AsyncElasticsearchSettings
 from stac_fastapi.elasticsearch.config import (
     ElasticsearchSettings as SyncElasticsearchSettings,
 )
 from stac_fastapi.types.errors import ConflictError, NotFoundError
 from stac_fastapi.types.stac import Collection, Item
 
@@ -495,26 +495,45 @@
             field (str): The field to perform the comparison on.
             value (float): The value to compare the field against.
 
         Returns:
             search (Search): The search object with the specified filter applied.
         """
         if op != "eq":
-            key_filter = {field: {f"{op}": value}}
+            key_filter = {field: {op: value}}
             search = search.filter(Q("range", **key_filter))
         else:
             search = search.filter("term", **{field: value})
 
         return search
 
     @staticmethod
     def apply_cql2_filter(search: Search, _filter: Optional[Dict[str, Any]]):
-        """Database logic to perform query for search endpoint."""
+        """
+        Apply a CQL2 filter to an Elasticsearch Search object.
+
+        This method transforms a dictionary representing a CQL2 filter into an Elasticsearch query
+        and applies it to the provided Search object. If the filter is None, the original Search
+        object is returned unmodified.
+
+        Args:
+            search (Search): The Elasticsearch Search object to which the filter will be applied.
+            _filter (Optional[Dict[str, Any]]): The filter in dictionary form that needs to be applied
+                                                to the search. The dictionary should follow the structure
+                                                required by the `to_es` function which converts it
+                                                to an Elasticsearch query.
+
+        Returns:
+            Search: The modified Search object with the filter applied if a filter is provided,
+                    otherwise the original Search object.
+        """
         if _filter is not None:
-            search = search.filter(filter.Clause.parse_obj(_filter).to_es())
+            es_query = filter.to_es(_filter)
+            search = search.query(es_query)
+
         return search
 
     @staticmethod
     def populate_sort(sortby: List) -> Optional[Dict[str, Dict[str, str]]]:
         """Database logic to sort search instance."""
         if sortby:
             return {s.field: {"order": s.direction} for s in sortby}
@@ -548,29 +567,34 @@
                 computed.
                 - The token to be used to retrieve the next set of results, or None if there are no more results.
 
         Raises:
             NotFoundError: If the collections specified in `collection_ids` do not exist.
         """
         search_after = None
+
         if token:
             search_after = urlsafe_b64decode(token.encode()).decode().split(",")
 
         query = search.query.to_dict() if search.query else None
 
         index_param = indices(collection_ids)
 
+        max_result_window = MAX_LIMIT
+
+        size_limit = min(limit + 1, max_result_window)
+
         search_task = asyncio.create_task(
             self.client.search(
                 index=index_param,
                 ignore_unavailable=ignore_unavailable,
                 query=query,
                 sort=sort or DEFAULT_SORT,
                 search_after=search_after,
-                size=limit,
+                size=size_limit,
             )
         )
 
         count_task = asyncio.create_task(
             self.client.count(
                 index=index_param,
                 ignore_unavailable=ignore_unavailable,
@@ -580,32 +604,35 @@
 
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

### Comparing `stac_fastapi_elasticsearch-2.4.1/stac_fastapi.elasticsearch.egg-info/SOURCES.txt` & `stac_fastapi_elasticsearch-3.0.0a0/stac_fastapi.elasticsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

