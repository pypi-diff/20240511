# Comparing `tmp/pg-es-fdw-0.8.0.tar.gz` & `tmp/pg-es-fdw-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg-es-fdw-0.8.0.tar", last modified: Tue Jun  9 20:13:59 2020, max compression
+gzip compressed data, was "pg-es-fdw-0.9.0.tar", last modified: Fri Sep 25 22:01:38 2020, max compression
```

## Comparing `pg-es-fdw-0.8.0.tar` & `pg-es-fdw-0.9.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1115 2015-12-01 22:03:16.399546 pg-es-fdw-0.8.0/LICENSE
--rw-r--r--   0        0        0    11643 2020-06-09 20:13:11.758956 pg-es-fdw-0.8.0/README.md
--rw-r--r--   0        0        0     8628 2020-06-09 20:13:11.758956 pg-es-fdw-0.8.0/pg_es_fdw/__init__.py
--rw-r--r--   0        0        0      863 2020-06-09 20:13:25.358999 pg-es-fdw-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    12698 2020-06-09 20:14:00.008462 pg-es-fdw-0.8.0/setup.py
--rw-r--r--   0        0        0    12696 2020-06-09 20:14:00.009025 pg-es-fdw-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1115 2015-12-01 22:03:16.399546 pg-es-fdw-0.9.0/LICENSE
+-rw-r--r--   0        0        0    13918 2020-09-25 22:00:45.033822 pg-es-fdw-0.9.0/README.md
+-rw-r--r--   0        0        0     8871 2020-09-25 22:00:45.033822 pg-es-fdw-0.9.0/pg_es_fdw/__init__.py
+-rw-r--r--   0        0        0      863 2020-09-25 22:00:59.345875 pg-es-fdw-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    15069 2020-09-25 22:01:38.051532 pg-es-fdw-0.9.0/setup.py
+-rw-r--r--   0        0        0    14971 2020-09-25 22:01:38.052037 pg-es-fdw-0.9.0/PKG-INFO
```

### Comparing `pg-es-fdw-0.8.0/LICENSE` & `pg-es-fdw-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pg-es-fdw-0.8.0/README.md` & `pg-es-fdw-0.9.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -195,14 +195,88 @@
 WHERE
     query = 'body:chess'
 ;
 ```
 
 This uses the [URI Search](https://www.elastic.co/guide/en/elasticsearch/reference/current/search-uri-request.html) from Elastic Search.
 
+#### Using the default sort and sort column
+
+Example: Creating the table
+```
+CREATE FOREIGN TABLE test_index (
+    id TEXT,
+    unit TEXT,
+    name TEXT,
+    last_updated timestamp,
+    address TEXT,
+    ipv4 TEXT,
+    company TEXT,
+    credit_card_number TEXT,
+    credit_card_provider TEXT,
+    credit_card_security TEXT,
+    email TEXT,
+    query TEXT,
+    sort TEXT,
+    score NUMERIC
+ )
+SERVER multicorn_es
+OPTIONS (
+    host 'localhost',
+    port '9200',
+    index 'test-index',
+    type 'doc',
+    rowid_column 'id',
+    query_column 'query',
+    score_column 'score',
+    default_sort 'last_updated:desc',
+    sort_column 'sort',
+    timeout '20'
+ );
+```
+
+Not using the sort column in the where clause, as you see it uses the default setting.
+
+```
+test=# select unit,last_updated,sort from test_index limit 10;
+NOTICE:  Sort: last_updated:desc
+ unit |        last_updated        |       sort        
+------+----------------------------+-------------------
+ 2426 | 2020-09-25 09:47:33.490236 | last_updated:desc
+ 2425 | 2020-09-25 09:47:32.477546 | last_updated:desc
+ 2424 | 2020-09-25 09:47:31.469799 | last_updated:desc
+ 2423 | 2020-09-25 09:47:30.463913 | last_updated:desc
+ 2422 | 2020-09-25 09:47:29.456766 | last_updated:desc
+ 2421 | 2020-09-25 09:47:28.445883 | last_updated:desc
+ 2420 | 2020-09-25 09:47:27.427684 | last_updated:desc
+ 2419 | 2020-09-25 09:47:26.414521 | last_updated:desc
+ 2418 | 2020-09-25 09:47:25.404088 | last_updated:desc
+ 2417 | 2020-09-25 09:47:24.396159 | last_updated:desc
+```
+
+Using the column to sort by other means. can be a comma seperated list
+```
+unit:asc,last_updated:desc
+```
+```
+test=# select unit,last_updated,sort from test_index WHERE sort = 'unit:asc' limit 10;
+ unit |        last_updated        |   sort   
+------+----------------------------+----------
+ 0    | 2020-09-25 09:06:42.353452 | unit:asc
+ 1    | 2020-09-25 09:06:43.367991 | unit:asc
+ 2    | 2020-09-25 09:06:44.379327 | unit:asc
+ 3    | 2020-09-25 09:06:45.389997 | unit:asc
+ 4    | 2020-09-25 09:06:46.403873 | unit:asc
+ 5    | 2020-09-25 09:06:47.41339  | unit:asc
+ 6    | 2020-09-25 09:06:48.421894 | unit:asc
+ 7    | 2020-09-25 09:06:49.433148 | unit:asc
+ 8    | 2020-09-25 09:06:50.445831 | unit:asc
+ 9    | 2020-09-25 09:06:51.457017 | unit:asc
+```
+
 Caveats
 -------
 
 Elastic Search does not support transactions, so the elasticsearch index
 is not guaranteed to be synchronized with the canonical version in PostgreSQL.
 Unfortunately this is the case even for serializable isolation level transactions.
 It would however be possible to check against Elastic Search version field and locking.
```

### Comparing `pg-es-fdw-0.8.0/pg_es_fdw/__init__.py` & `pg-es-fdw-0.9.0/pg_es_fdw/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # pylint: disable=too-many-instance-attributes, import-error, unexpected-keyword-arg, broad-except, line-too-long
 
 import json
 import logging
 
 from elasticsearch import VERSION as ELASTICSEARCH_VERSION
 from elasticsearch import Elasticsearch
-
 from multicorn import ForeignDataWrapper
 from multicorn.utils import log_to_postgres as log2pg
 
 
 class ElasticsearchFDW(ForeignDataWrapper):
     """ Elastic Search Foreign Data Wrapper """
 
@@ -28,14 +27,16 @@
     def __init__(self, options, columns):
         super(ElasticsearchFDW, self).__init__(options, columns)
 
         self.index = options.pop("index", "")
         self.doc_type = options.pop("type", "")
         self.query_column = options.pop("query_column", None)
         self.score_column = options.pop("score_column", None)
+        self.default_sort = options.pop("default_sort", "")
+        self.sort_column = options.pop("sort_column", None)
         self.scroll_size = int(options.pop("scroll_size", "1000"))
         self.scroll_duration = options.pop("scroll_duration", "10m")
         self._rowid_column = options.pop("rowid_column", "id")
         username = options.pop("username", None)
         password = options.pop("password", None)
 
         if ELASTICSEARCH_VERSION[0] >= 7:
@@ -70,15 +71,14 @@
 
     def get_rel_size(self, quals, columns):
         """ Helps the planner by returning costs.
             Returns a tuple of the form (number of rows, average row width) """
 
         try:
             query = self._get_query(quals)
-
             if query:
                 response = self.client.count(q=query, **self.arguments)
             else:
                 response = self.client.count(**self.arguments)
             return (response["count"], len(columns) * 100)
         except Exception as exception:
             log2pg(
@@ -89,33 +89,36 @@
             )
             return (0, 0)
 
     def execute(self, quals, columns):
         """ Execute the query """
 
         try:
+            arguments = dict(self.arguments)
+            arguments['sort'] = self._get_sort(quals)
+            sort = arguments['sort']
             query = self._get_query(quals)
 
             if query:
                 response = self.client.search(
                     size=self.scroll_size,
                     scroll=self.scroll_duration,
                     q=query,
-                    **self.arguments
+                    **arguments
                 )
             else:
                 response = self.client.search(
-                    size=self.scroll_size, scroll=self.scroll_duration, **self.arguments
+                    size=self.scroll_size, scroll=self.scroll_duration, **arguments
                 )
 
             while True:
                 scroll_id = response["_scroll_id"]
 
                 for result in response["hits"]["hits"]:
-                    yield self._convert_response_row(result, columns, query)
+                    yield self._convert_response_row(result, columns, query, sort)
 
                 if len(response["hits"]["hits"]) < self.scroll_size:
                     return
                 response = self.client.scroll(
                     scroll_id=scroll_id, scroll=self.scroll_duration
                 )
         except Exception as exception:
@@ -211,34 +214,39 @@
                 qualifier.value
                 for qualifier in quals
                 if qualifier.field_name == self.query_column
             ),
             None,
         )
 
-    def _convert_response_row(self, row_data, columns, query):
-        if query:
-            # Postgres checks the query after too, so the query column needs to be present
-            return dict(
-                [
-                    (column, self._convert_response_column(column, row_data))
-                    for column in columns
-                    if column in row_data["_source"]
-                    or column == self.rowid_column
-                    or column == self.score_column
-                ]
-                + [(self.query_column, query)]
-            )
-        return {
+    def _get_sort(self, quals):
+        if not self.sort_column:
+            return self.default_sort
+
+        return next(
+            (
+                qualifier.value
+                for qualifier in quals
+                if qualifier.field_name == self.sort_column and qualifier.value
+            ),
+            self.default_sort
+        )
+
+    def _convert_response_row(self, row_data, columns, query, sort):
+        return_dict = {
             column: self._convert_response_column(column, row_data)
             for column in columns
             if column in row_data["_source"]
             or column == self.rowid_column
             or column == self.score_column
         }
+        if query:
+            return_dict[self.query_column] = query
+        return_dict[self.sort_column] = sort
+        return return_dict
 
     def _convert_response_column(self, column, row_data):
         if column == self.rowid_column:
             return row_data["_id"]
         if column == self.score_column:
             return row_data["_score"]
         value = row_data["_source"][column]
```

### Comparing `pg-es-fdw-0.8.0/pyproject.toml` & `pg-es-fdw-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "pg-es-fdw"
-version = "0.8.0"
+version = "0.9.0"
 description = "Connect PostgreSQL and Elastic Search with this Foreign Data Wrapper"
 authors = ["Matthew Franglen <matthew@franglen.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/matthewfranglen/postgres-elasticsearch-fdw"
 repository = "https://github.com/matthewfranglen/postgres-elasticsearch-fdw"
 keywords = ["postgresql", "postgres", "elasticsearch", "es", "fdw"]
 
 [tool.poetry.urls]
-download ="https://github.com/matthewfranglen/postgres-elasticsearch-fdw/archive/0.8.0.zip"
+download ="https://github.com/matthewfranglen/postgres-elasticsearch-fdw/archive/0.9.0.zip"
 
 [tool.poetry.dependencies]
 elasticsearch = "^7.6.0"
 
 [tool.poetry.dev-dependencies]
 black = "^19.10b0"
 pylint = "^2.4.4"
```

