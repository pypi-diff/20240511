# Comparing `tmp/stac_fastapi_core-2.4.1.tar.gz` & `tmp/stac_fastapi_core-3.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_core-2.4.1.tar", last modified: Mon May  6 16:10:14 2024, max compression
+gzip compressed data, was "stac_fastapi_core-3.0.0a0.tar", last modified: Sat May 11 10:58:49 2024, max compression
```

## Comparing `stac_fastapi_core-2.4.1.tar` & `stac_fastapi_core-3.0.0a0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:14.103391 stac_fastapi_core-2.4.1/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1217 2024-05-06 16:10:14.103011 stac_fastapi_core-2.4.1/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)       69 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/README.md
--rw-r--r--   0 primeradiant   (501) staff       (20)      104 2024-05-06 16:10:14.106200 stac_fastapi_core-2.4.1/setup.cfg
--rw-r--r--   0 primeradiant   (501) staff       (20)     1385 2024-05-04 09:54:48.000000 stac_fastapi_core-2.4.1/setup.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:13.985082 stac_fastapi_core-2.4.1/stac_fastapi/
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:14.053169 stac_fastapi_core-2.4.1/stac_fastapi/core/
--rw-r--r--   0 primeradiant   (501) staff       (20)       20 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     1608 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/base_database_logic.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      239 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/base_settings.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     3826 2024-05-02 09:57:35.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/basic_auth.py
--rw-r--r--   0 primeradiant   (501) staff       (20)    35886 2024-05-06 15:51:07.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/core.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      384 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/datetime_utils.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:14.064436 stac_fastapi_core-2.4.1/stac_fastapi/core/extensions/
--rw-r--r--   0 primeradiant   (501) staff       (20)      167 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/extensions/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     7464 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/extensions/filter.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     1892 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/extensions/query.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:14.083999 stac_fastapi_core-2.4.1/stac_fastapi/core/models/
--rw-r--r--   0 primeradiant   (501) staff       (20)       48 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/models/__init__.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     4470 2024-03-19 04:19:17.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/models/links.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       27 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/models/search.py
--rw-r--r--   0 primeradiant   (501) staff       (20)     5892 2024-03-19 04:19:17.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/serializers.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      473 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/session.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:14.092935 stac_fastapi_core-2.4.1/stac_fastapi/core/types/
--rw-r--r--   0 primeradiant   (501) staff       (20)     9155 2024-04-24 05:29:38.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/types/core.py
--rw-r--r--   0 primeradiant   (501) staff       (20)      933 2024-02-08 06:37:21.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/utilities.py
--rw-r--r--   0 primeradiant   (501) staff       (20)       45 2024-05-06 15:56:07.000000 stac_fastapi_core-2.4.1/stac_fastapi/core/version.py
-drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-06 16:10:14.101586 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/
--rw-r--r--   0 primeradiant   (501) staff       (20)     1217 2024-05-06 16:10:13.000000 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/PKG-INFO
--rw-r--r--   0 primeradiant   (501) staff       (20)      850 2024-05-06 16:10:13.000000 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/SOURCES.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-06 16:10:13.000000 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/dependency_links.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-01-31 08:38:37.000000 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/not-zip-safe
--rw-r--r--   0 primeradiant   (501) staff       (20)      250 2024-05-06 16:10:13.000000 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/requires.txt
--rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-06 16:10:13.000000 stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/top_level.txt
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.960157 stac_fastapi_core-3.0.0a0/
+-rw-r--r--   0 primeradiant   (501) staff       (20)    14638 2024-05-11 10:58:49.959358 stac_fastapi_core-3.0.0a0/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)    13479 2024-05-11 10:42:06.000000 stac_fastapi_core-3.0.0a0/README.md
+-rw-r--r--   0 primeradiant   (501) staff       (20)      104 2024-05-11 10:58:49.963905 stac_fastapi_core-3.0.0a0/setup.cfg
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1401 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a0/setup.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.892128 stac_fastapi_core-3.0.0a0/stac_fastapi/
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.934731 stac_fastapi_core-3.0.0a0/stac_fastapi/core/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       20 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1608 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/base_database_logic.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      239 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/base_settings.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     3826 2024-05-02 09:57:35.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/basic_auth.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)    37146 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/core.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1481 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/datetime_utils.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.941841 stac_fastapi_core-3.0.0a0/stac_fastapi/core/extensions/
+-rw-r--r--   0 primeradiant   (501) staff       (20)      167 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/extensions/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     6095 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/extensions/filter.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     1921 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/extensions/query.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.949977 stac_fastapi_core-3.0.0a0/stac_fastapi/core/models/
+-rw-r--r--   0 primeradiant   (501) staff       (20)       48 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/models/__init__.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     4470 2024-03-19 04:19:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/models/links.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       27 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/models/search.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)     5892 2024-03-19 04:19:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/serializers.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      473 2024-02-08 06:37:21.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/session.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.952508 stac_fastapi_core-3.0.0a0/stac_fastapi/core/types/
+-rw-r--r--   0 primeradiant   (501) staff       (20)     8120 2024-05-11 10:41:17.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/types/core.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)      952 2024-05-11 10:42:06.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/utilities.py
+-rw-r--r--   0 primeradiant   (501) staff       (20)       47 2024-05-11 10:41:59.000000 stac_fastapi_core-3.0.0a0/stac_fastapi/core/version.py
+drwxr-xr-x   0 primeradiant   (501) staff       (20)        0 2024-05-11 10:58:49.957363 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/
+-rw-r--r--   0 primeradiant   (501) staff       (20)    14638 2024-05-11 10:58:49.000000 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/PKG-INFO
+-rw-r--r--   0 primeradiant   (501) staff       (20)      850 2024-05-11 10:58:49.000000 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/SOURCES.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-05-11 10:58:49.000000 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/dependency_links.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)        1 2024-01-31 08:38:37.000000 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/not-zip-safe
+-rw-r--r--   0 primeradiant   (501) staff       (20)      223 2024-05-11 10:58:49.000000 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/requires.txt
+-rw-r--r--   0 primeradiant   (501) staff       (20)       18 2024-05-11 10:58:49.000000 stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/top_level.txt
```

### Comparing `stac_fastapi_core-2.4.1/setup.py` & `stac_fastapi_core-3.0.0a0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "fastapi",
-    "attrs",
-    "pydantic[dotenv]<2",
-    "stac_pydantic==2.0.*",
-    "stac-fastapi.types==2.5.5.post1",
-    "stac-fastapi.api==2.5.5.post1",
-    "stac-fastapi.extensions==2.5.5.post1",
-    "pystac[validation]",
+    "fastapi-slim",
+    "attrs>=23.2.0",
+    "pydantic[dotenv]",
+    "stac_pydantic>=3",
+    "stac-fastapi.types==3.0.0a",
+    "stac-fastapi.api==3.0.0a",
+    "stac-fastapi.extensions==3.0.0a",
     "orjson",
     "overrides",
     "geojson-pydantic",
     "pygeofilter==0.2.1",
-    "typing_extensions==4.4.0",
+    "typing_extensions==4.8.0",
 ]
 
 setup(
     name="stac-fastapi.core",
     description="Core library for the Elasticsearch and Opensearch stac-fastapi backends.",
     long_description=desc,
     long_description_content_type="text/markdown",
@@ -31,14 +30,15 @@
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

### Comparing `stac_fastapi_core-2.4.1/stac_fastapi/core/base_database_logic.py` & `stac_fastapi_core-3.0.0a0/stac_fastapi/core/base_database_logic.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.4.1/stac_fastapi/core/basic_auth.py` & `stac_fastapi_core-3.0.0a0/stac_fastapi/core/basic_auth.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.4.1/stac_fastapi/core/core.py` & `stac_fastapi_core-3.0.0a0/stac_fastapi/core/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 """Core client."""
 import logging
 import re
 from datetime import datetime as datetime_type
 from datetime import timezone
+from enum import Enum
 from typing import Any, Dict, List, Optional, Set, Type, Union
 from urllib.parse import unquote_plus, urljoin
 
 import attr
 import orjson
 import stac_pydantic
 from fastapi import HTTPException, Request
 from overrides import overrides
 from pydantic import ValidationError
 from pygeofilter.backends.cql2_json import to_cql2
 from pygeofilter.parsers.cql2_text import parse as parse_cql2_text
+from stac_pydantic import Collection, Item, ItemCollection
 from stac_pydantic.links import Relations
 from stac_pydantic.shared import BBox, MimeTypes
 from stac_pydantic.version import STAC_VERSION
 
 from stac_fastapi.core.base_database_logic import BaseDatabaseLogic
 from stac_fastapi.core.base_settings import ApiBaseSettings
 from stac_fastapi.core.models.links import PagingLinks
 from stac_fastapi.core.serializers import CollectionSerializer, ItemSerializer
 from stac_fastapi.core.session import Session
 from stac_fastapi.core.types.core import (
     AsyncBaseCoreClient,
-    AsyncBaseFiltersClient,
     AsyncBaseTransactionsClient,
 )
 from stac_fastapi.extensions.third_party.bulk_transactions import (
     BaseBulkTransactionsClient,
     BulkTransactionMethod,
     Items,
 )
 from stac_fastapi.types import stac as stac_types
 from stac_fastapi.types.config import Settings
 from stac_fastapi.types.conformance import BASE_CONFORMANCE_CLASSES
+from stac_fastapi.types.core import AsyncBaseFiltersClient
 from stac_fastapi.types.extension import ApiExtension
 from stac_fastapi.types.requests import get_base_url
 from stac_fastapi.types.rfc3339 import DateTimeType
 from stac_fastapi.types.search import BaseSearchPostRequest
-from stac_fastapi.types.stac import Collection, Collections, Item, ItemCollection
 
 logger = logging.getLogger(__name__)
 
 NumType = Union[float, int]
 
 
 @attr.s
@@ -185,15 +186,15 @@
                     str(request.base_url), request.app.docs_url.lstrip("/")
                 ),
             }
         )
 
         return landing_page
 
-    async def all_collections(self, **kwargs) -> Collections:
+    async def all_collections(self, **kwargs) -> stac_types.Collections:
         """Read all collections from the database.
 
         Args:
             **kwargs: Keyword arguments from the request.
 
         Returns:
             A Collections object containing all the collections in the database and links to various resources.
@@ -217,17 +218,19 @@
             },
         ]
 
         if next_token:
             next_link = PagingLinks(next=next_token, request=request).link_next()
             links.append(next_link)
 
-        return Collections(collections=collections, links=links)
+        return stac_types.Collections(collections=collections, links=links)
 
-    async def get_collection(self, collection_id: str, **kwargs) -> Collection:
+    async def get_collection(
+        self, collection_id: str, **kwargs
+    ) -> stac_types.Collection:
         """Get a collection from the database by its id.
 
         Args:
             collection_id (str): The id of the collection to retrieve.
             kwargs: Additional keyword arguments passed to the API call.
 
         Returns:
@@ -246,15 +249,15 @@
         self,
         collection_id: str,
         bbox: Optional[BBox] = None,
         datetime: Optional[DateTimeType] = None,
         limit: int = 10,
         token: str = None,
         **kwargs,
-    ) -> ItemCollection:
+    ) -> stac_types.ItemCollection:
         """Read items from a specific collection in the database.
 
         Args:
             collection_id (str): The identifier of the collection to read items from.
             bbox (Optional[BBox]): The bounding box to filter items by.
             datetime (Optional[DateTimeType]): The datetime range to filter items by.
             limit (int): The maximum number of items to return. The default value is 10.
@@ -316,22 +319,24 @@
                 "limit": limit,
             }
             if maybe_count is not None:
                 context_obj["matched"] = maybe_count
 
         links = await PagingLinks(request=request, next=next_token).get_links()
 
-        return ItemCollection(
+        return stac_types.ItemCollection(
             type="FeatureCollection",
             features=items,
             links=links,
             context=context_obj,
         )
 
-    async def get_item(self, item_id: str, collection_id: str, **kwargs) -> Item:
+    async def get_item(
+        self, item_id: str, collection_id: str, **kwargs
+    ) -> stac_types.Item:
         """Get an item from the database based on its id and collection id.
 
         Args:
             collection_id (str): The ID of the collection the item belongs to.
             item_id (str): The ID of the item to be retrieved.
 
         Returns:
@@ -395,14 +400,32 @@
             if start:
                 result["gte"] = start.strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] + "Z"
             if end:
                 result["lte"] = end.strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] + "Z"
 
         return result
 
+    def _format_datetime_range(self, date_tuple: DateTimeType) -> str:
+        """
+        Convert a tuple of datetime objects or None into a formatted string for API requests.
+
+        Args:
+            date_tuple (tuple): A tuple containing two elements, each can be a datetime object or None.
+
+        Returns:
+            str: A string formatted as 'YYYY-MM-DDTHH:MM:SS.sssZ/YYYY-MM-DDTHH:MM:SS.sssZ', with '..' used if any element is None.
+        """
+
+        def format_datetime(dt):
+            """Format a single datetime object to the ISO8601 extended format with 'Z'."""
+            return dt.strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] + "Z" if dt else ".."
+
+        start, end = date_tuple
+        return f"{format_datetime(start)}/{format_datetime(end)}"
+
     async def get_search(
         self,
         request: Request,
         collections: Optional[List[str]] = None,
         ids: Optional[List[str]] = None,
         bbox: Optional[BBox] = None,
         datetime: Optional[DateTimeType] = None,
@@ -411,15 +434,15 @@
         token: Optional[str] = None,
         fields: Optional[List[str]] = None,
         sortby: Optional[str] = None,
         intersects: Optional[str] = None,
         filter: Optional[str] = None,
         filter_lang: Optional[str] = None,
         **kwargs,
-    ) -> ItemCollection:
+    ) -> stac_types.ItemCollection:
         """Get search results from the database.
 
         Args:
             collections (Optional[List[str]]): List of collection IDs to search in.
             ids (Optional[List[str]]): List of item IDs to search for.
             bbox (Optional[BBox]): Bounding box to search in.
             datetime (Optional[DateTimeType]): Filter items based on the datetime field.
@@ -451,15 +474,15 @@
         query_params = str(request.query_params)
         if filter_lang is None:
             match = re.search(r"filter-lang=([a-z0-9-]+)", query_params, re.IGNORECASE)
             if match:
                 filter_lang = match.group(1)
 
         if datetime:
-            base_args["datetime"] = datetime
+            base_args["datetime"] = self._format_datetime_range(datetime)
 
         if intersects:
             base_args["intersects"] = orjson.loads(unquote_plus(intersects))
 
         if sortby:
             sort_param = []
             for sort in sortby:
@@ -498,15 +521,15 @@
             raise HTTPException(status_code=400, detail="Invalid parameters provided")
         resp = await self.post_search(search_request=search_request, request=request)
 
         return resp
 
     async def post_search(
         self, search_request: BaseSearchPostRequest, request: Request
-    ) -> ItemCollection:
+    ) -> stac_types.ItemCollection:
         """
         Perform a POST search on the catalog.
 
         Args:
             search_request (BaseSearchPostRequest): Request object that includes the parameters for the search.
             kwargs: Keyword arguments passed to the function.
 
@@ -548,16 +571,18 @@
                 search=search, intersects=search_request.intersects
             )
 
         if search_request.query:
             for field_name, expr in search_request.query.items():
                 field = "properties__" + field_name
                 for op, value in expr.items():
+                    # Convert enum to string
+                    operator = op.value if isinstance(op, Enum) else op
                     search = self.database.apply_stacql_filter(
-                        search=search, op=op, field=field, value=value
+                        search=search, op=operator, field=field, value=value
                     )
 
         # only cql2_json is supported here
         if hasattr(search_request, "filter"):
             cql2_filter = getattr(search_request, "filter", None)
             try:
                 search = self.database.apply_cql2_filter(search, cql2_filter)
@@ -615,15 +640,15 @@
                 "limit": limit,
             }
             if maybe_count is not None:
                 context_obj["matched"] = maybe_count
 
         links = await PagingLinks(request=request, next=next_token).get_links()
 
-        return ItemCollection(
+        return stac_types.ItemCollection(
             type="FeatureCollection",
             features=items,
             links=links,
             context=context_obj,
         )
 
 
@@ -633,15 +658,15 @@
 
     database: BaseDatabaseLogic = attr.ib()
     settings: ApiBaseSettings = attr.ib()
     session: Session = attr.ib(default=attr.Factory(Session.create_from_env))
 
     @overrides
     async def create_item(
-        self, collection_id: str, item: stac_types.Item, **kwargs
+        self, collection_id: str, item: Union[Item, ItemCollection], **kwargs
     ) -> Optional[stac_types.Item]:
         """Create an item in the collection.
 
         Args:
             collection_id (str): The id of the collection to add the item to.
             item (stac_types.Item): The item to be added to the collection.
             kwargs: Additional keyword arguments.
@@ -650,14 +675,15 @@
             stac_types.Item: The created item.
 
         Raises:
             NotFound: If the specified collection is not found in the database.
             ConflictError: If the item in the specified collection already exists.
 
         """
+        item = item.model_dump(mode="json")
         base_url = str(kwargs["request"].base_url)
 
         # If a feature collection is posted
         if item["type"] == "FeatureCollection":
             bulk_client = BulkTransactionsClient(
                 database=self.database, settings=self.settings
             )
@@ -673,15 +699,15 @@
         else:
             item = await self.database.prep_create_item(item=item, base_url=base_url)
             await self.database.create_item(item, refresh=kwargs.get("refresh", False))
             return ItemSerializer.db_to_stac(item, base_url)
 
     @overrides
     async def update_item(
-        self, collection_id: str, item_id: str, item: stac_types.Item, **kwargs
+        self, collection_id: str, item_id: str, item: Item, **kwargs
     ) -> stac_types.Item:
         """Update an item in the collection.
 
         Args:
             collection_id (str): The ID of the collection the item belongs to.
             item_id (str): The ID of the item to be updated.
             item (stac_types.Item): The new item data.
@@ -690,21 +716,22 @@
         Returns:
             stac_types.Item: The updated item object.
 
         Raises:
             NotFound: If the specified collection is not found in the database.
 
         """
+        item = item.model_dump(mode="json")
         base_url = str(kwargs["request"].base_url)
         now = datetime_type.now(timezone.utc).isoformat().replace("+00:00", "Z")
         item["properties"]["updated"] = now
 
         await self.database.check_collection_exists(collection_id)
         await self.delete_item(item_id=item_id, collection_id=collection_id)
-        await self.create_item(collection_id=collection_id, item=item, **kwargs)
+        await self.create_item(collection_id=collection_id, item=Item(**item), **kwargs)
 
         return ItemSerializer.db_to_stac(item, base_url)
 
     @overrides
     async def delete_item(
         self, item_id: str, collection_id: str, **kwargs
     ) -> Optional[stac_types.Item]:
@@ -718,39 +745,39 @@
             Optional[stac_types.Item]: The deleted item, or `None` if the item was successfully deleted.
         """
         await self.database.delete_item(item_id=item_id, collection_id=collection_id)
         return None
 
     @overrides
     async def create_collection(
-        self, collection: stac_types.Collection, **kwargs
+        self, collection: Collection, **kwargs
     ) -> stac_types.Collection:
         """Create a new collection in the database.
 
         Args:
             collection (stac_types.Collection): The collection to be created.
             kwargs: Additional keyword arguments.
 
         Returns:
             stac_types.Collection: The created collection object.
 
         Raises:
             ConflictError: If the collection already exists.
         """
+        collection = collection.model_dump(mode="json")
         base_url = str(kwargs["request"].base_url)
         collection = self.database.collection_serializer.stac_to_db(
             collection, base_url
         )
         await self.database.create_collection(collection=collection)
-
         return CollectionSerializer.db_to_stac(collection, base_url)
 
     @overrides
     async def update_collection(
-        self, collection: stac_types.Collection, **kwargs
+        self, collection: Collection, **kwargs
     ) -> stac_types.Collection:
         """
         Update a collection.
 
         This method updates an existing collection in the database by first finding
         the collection by the id given in the keyword argument `collection_id`.
         If no `collection_id` is given the id of the given collection object is used.
@@ -762,14 +789,16 @@
             collection: A STAC collection that needs to be updated.
             kwargs: Additional keyword arguments.
 
         Returns:
             A STAC collection that has been updated in the database.
 
         """
+        collection = collection.model_dump(mode="json")
+
         base_url = str(kwargs["request"].base_url)
 
         collection_id = kwargs["request"].query_params.get(
             "collection_id", collection["id"]
         )
 
         collection = self.database.collection_serializer.stac_to_db(
```

### Comparing `stac_fastapi_core-2.4.1/stac_fastapi/core/extensions/query.py` & `stac_fastapi_core-3.0.0a0/stac_fastapi/core/extensions/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,23 +59,23 @@
 class QueryExtensionPostRequest(BaseModel):
     """Queryable validation.
 
     Add queryables validation to the POST request
     to raise errors for unsupported querys.
     """
 
-    query: Optional[Dict[Queryables, Dict[Operator, Any]]]
+    query: Optional[Dict[str, Dict[Operator, Any]]] = None
 
     @root_validator(pre=True)
     def validate_query_fields(cls, values: Dict) -> Dict:
         """Validate query fields."""
         ...
 
 
 class QueryExtension(QueryExtensionBase):
     """Query Extenson.
 
     Override the POST request model to add validation against
     supported fields
     """
 
-    ...
+    POST = QueryExtensionPostRequest
```

### Comparing `stac_fastapi_core-2.4.1/stac_fastapi/core/models/links.py` & `stac_fastapi_core-3.0.0a0/stac_fastapi/core/models/links.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.4.1/stac_fastapi/core/serializers.py` & `stac_fastapi_core-3.0.0a0/stac_fastapi/core/serializers.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_core-2.4.1/stac_fastapi/core/types/core.py` & `stac_fastapi_core-3.0.0a0/stac_fastapi/core/types/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Base clients. Taken from stac-fastapi.types.core v2.4.9."""
 import abc
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Union
 
 import attr
+from stac_pydantic import Collection, Item, ItemCollection
 from starlette.responses import Response
 
 from stac_fastapi.core.base_database_logic import BaseDatabaseLogic
 from stac_fastapi.types import stac as stac_types
 from stac_fastapi.types.conformance import BASE_CONFORMANCE_CLASSES
 from stac_fastapi.types.extension import ApiExtension
 from stac_fastapi.types.search import BaseSearchPostRequest
@@ -23,15 +24,15 @@
 
     database = attr.ib(default=BaseDatabaseLogic)
 
     @abc.abstractmethod
     async def create_item(
         self,
         collection_id: str,
-        item: Union[stac_types.Item, stac_types.ItemCollection],
+        item: Union[Item, ItemCollection],
         **kwargs,
     ) -> Optional[Union[stac_types.Item, Response, None]]:
         """Create a new item.
 
         Called with `POST /collections/{collection_id}/items`.
 
         Args:
@@ -41,15 +42,15 @@
         Returns:
             The item that was created or None if item collection.
         """
         ...
 
     @abc.abstractmethod
     async def update_item(
-        self, collection_id: str, item_id: str, item: stac_types.Item, **kwargs
+        self, collection_id: str, item_id: str, item: Item, **kwargs
     ) -> Optional[Union[stac_types.Item, Response]]:
         """Perform a complete update on an existing item.
 
         Called with `PUT /collections/{collection_id}/items`. It is expected
         that this item already exists.  The update should do a diff against the
         saved item and perform any necessary updates.  Partial updates are not
         supported by the transactions extension.
@@ -77,15 +78,15 @@
         Returns:
             The deleted item.
         """
         ...
 
     @abc.abstractmethod
     async def create_collection(
-        self, collection: stac_types.Collection, **kwargs
+        self, collection: Collection, **kwargs
     ) -> Optional[Union[stac_types.Collection, Response]]:
         """Create a new collection.
 
         Called with `POST /collections`.
 
         Args:
             collection: the collection
@@ -93,15 +94,15 @@
         Returns:
             The collection that was created.
         """
         ...
 
     @abc.abstractmethod
     async def update_collection(
-        self, collection: stac_types.Collection, **kwargs
+        self, collection: Collection, **kwargs
     ) -> Optional[Union[stac_types.Collection, Response]]:
         """Perform a complete update on an existing collection.
 
         Called with `PUT /collections`. It is expected that this item already
         exists.  The update should do a diff against the saved collection and
         perform any necessary updates.  Partial updates are not supported by the
         transactions extension.
@@ -274,33 +275,7 @@
             limit: number of items to return.
             token: pagination token.
 
         Returns:
             An ItemCollection.
         """
         ...
-
-
-@attr.s
-class AsyncBaseFiltersClient(abc.ABC):
-    """Defines a pattern for implementing the STAC filter extension."""
-
-    async def get_queryables(
-        self, collection_id: Optional[str] = None, **kwargs
-    ) -> Dict[str, Any]:
-        """Get the queryables available for the given collection_id.
-
-        If collection_id is None, returns the intersection of all queryables over all
-        collections.
-
-        This base implementation returns a blank queryable schema. This is not allowed
-        under OGC CQL but it is allowed by the STAC API Filter Extension
-        https://github.com/radiantearth/stac-api-spec/tree/master/fragments/filter#queryables
-        """
-        return {
-            "$schema": "https://json-schema.org/draft/2019-09/schema",
-            "$id": "https://example.org/queryables",
-            "type": "object",
-            "title": "Queryables for Example STAC API",
-            "description": "Queryable names for the example STAC API Item Search filter.",
-            "properties": {},
-        }
```

### Comparing `stac_fastapi_core-2.4.1/stac_fastapi/core/utilities.py` & `stac_fastapi_core-3.0.0a0/stac_fastapi/core/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Module for geospatial processing functions.
 
 This module contains functions for transforming geospatial coordinates,
 such as converting bounding boxes to polygon representations.
 """
 from typing import List
 
+MAX_LIMIT = 10000
+
 
 def bbox2polygon(b0: float, b1: float, b2: float, b3: float) -> List[List[List[float]]]:
     """Transform a bounding box represented by its four coordinates `b0`, `b1`, `b2`, and `b3` into a polygon.
 
     Args:
         b0 (float): The x-coordinate of the lower-left corner of the bounding box.
         b1 (float): The y-coordinate of the lower-left corner of the bounding box.
```

### Comparing `stac_fastapi_core-2.4.1/stac_fastapi.core.egg-info/SOURCES.txt` & `stac_fastapi_core-3.0.0a0/stac_fastapi.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

