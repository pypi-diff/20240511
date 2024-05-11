# Comparing `tmp/brainchain-0.6.5.tar.gz` & `tmp/brainchain-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.6.5.tar", max compression
+gzip compressed data, was "brainchain-0.6.6.tar", max compression
```

## Comparing `brainchain-0.6.5.tar` & `brainchain-0.6.6.tar`

### file list

```diff
@@ -1,47 +1,46 @@
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.6.5/brainchain/README.md
--rw-r--r--   0        0        0     2982 2024-05-10 17:23:42.151722 brainchain-0.6.5/brainchain/__init__.py
--rw-r--r--   0        0        0    13634 2024-05-07 16:51:46.069513 brainchain-0.6.5/brainchain/assistants
--rw-r--r--   0        0        0    13624 2024-05-07 16:51:46.070229 brainchain-0.6.5/brainchain/assistants.py
--rw-r--r--   0        0        0    11851 2024-05-09 17:42:15.555016 brainchain-0.6.5/brainchain/brainchain.py
--rw-r--r--   0        0        0     5663 2024-05-09 05:35:25.596909 brainchain-0.6.5/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2024-02-14 04:10:52.129450 brainchain-0.6.5/brainchain/coredata.py
--rw-r--r--   0        0        0     2155 2023-09-12 01:13:30.915323 brainchain-0.6.5/brainchain/embeddings.py
--rw-r--r--   0        0        0    17779 2024-05-10 17:26:05.409771 brainchain-0.6.5/brainchain/graph/base.py
--rw-r--r--   0        0        0     7386 2024-05-10 17:23:37.046295 brainchain-0.6.5/brainchain/graph/schema.py
--rw-r--r--   0        0        0     3426 2024-05-07 16:51:46.072116 brainchain-0.6.5/brainchain/logger.py
--rw-r--r--   0        0        0    11959 2024-05-07 16:51:46.072448 brainchain-0.6.5/brainchain/products.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.6.5/brainchain/requirements.txt
--rw-r--r--   0        0        0     6024 2024-05-07 16:20:56.058058 brainchain-0.6.5/brainchain/sales_intel.py
--rw-r--r--   0        0        0     1977 2024-02-29 23:10:12.854747 brainchain-0.6.5/brainchain/search_v2.py
--rw-r--r--   0        0        0      595 2024-04-12 19:05:17.907126 brainchain-0.6.5/brainchain/tools/__init__.py
--rw-r--r--   0        0        0     2118 2024-05-09 17:28:37.403805 brainchain-0.6.5/brainchain/tools/coding.py
--rw-r--r--   0        0        0     3948 2024-05-07 16:51:46.073351 brainchain-0.6.5/brainchain/tools/diffbot.py
--rw-r--r--   0        0        0      632 2024-02-29 23:10:12.855578 brainchain-0.6.5/brainchain/tools/factual.py
--rw-r--r--   0        0        0     5800 2024-04-10 01:04:48.531327 brainchain-0.6.5/brainchain/tools/fts.py
--rw-r--r--   0        0        0     1450 2024-02-29 23:10:12.856798 brainchain-0.6.5/brainchain/tools/graph.py
--rw-r--r--   0        0        0     1029 2024-02-29 23:10:12.857047 brainchain-0.6.5/brainchain/tools/memory.py
--rw-r--r--   0        0        0     2154 2024-02-29 23:10:12.857190 brainchain-0.6.5/brainchain/tools/plan.py
--rw-r--r--   0        0        0     1660 2024-04-15 19:40:33.833814 brainchain-0.6.5/brainchain/tools/tokens.py
--rw-r--r--   0        0        0    21273 2024-05-07 16:51:46.073960 brainchain-0.6.5/brainchain/tools/tools.py
--rw-r--r--   0        0        0    12159 2024-05-07 16:51:46.074887 brainchain-0.6.5/brainchain/tools/web.py
--rw-r--r--   0        0        0      731 2024-04-23 19:21:58.552351 brainchain-0.6.5/brainchain/tools.py
--rw-r--r--   0        0        0      791 2024-05-07 16:51:51.752365 brainchain-0.6.5/brainchain/webapp/__init__.py
--rw-r--r--   0        0        0       82 2024-05-07 16:51:51.752653 brainchain-0.6.5/brainchain/webapp/agents.py
--rw-r--r--   0        0        0      173 2024-05-07 16:51:51.752960 brainchain-0.6.5/brainchain/webapp/base.py
--rw-r--r--   0        0        0      977 2024-05-07 16:51:51.753234 brainchain-0.6.5/brainchain/webapp/business_ideas.py
--rw-r--r--   0        0        0     1282 2024-05-07 16:51:51.753423 brainchain-0.6.5/brainchain/webapp/contents.py
--rw-r--r--   0        0        0      895 2024-05-07 16:51:51.753590 brainchain-0.6.5/brainchain/webapp/conversations.py
--rw-r--r--   0        0        0       91 2024-05-07 16:51:51.753815 brainchain-0.6.5/brainchain/webapp/embedding_models.py
--rw-r--r--   0        0        0     2709 2024-05-07 16:51:51.753990 brainchain-0.6.5/brainchain/webapp/embeddings.py
--rw-r--r--   0        0        0     1138 2024-05-07 16:51:51.754142 brainchain-0.6.5/brainchain/webapp/files.py
--rw-r--r--   0        0        0      218 2024-05-07 16:51:51.754320 brainchain-0.6.5/brainchain/webapp/health.py
--rw-r--r--   0        0        0       90 2024-05-07 16:51:51.754539 brainchain-0.6.5/brainchain/webapp/language_models.py
--rw-r--r--   0        0        0      622 2024-05-07 16:51:51.754700 brainchain-0.6.5/brainchain/webapp/laws.py
--rw-r--r--   0        0        0     1110 2024-05-07 16:51:51.754849 brainchain-0.6.5/brainchain/webapp/messages.py
--rw-r--r--   0        0        0     2220 2024-05-07 16:51:51.755068 brainchain-0.6.5/brainchain/webapp/namespaces.py
--rw-r--r--   0        0        0     1029 2024-05-07 16:51:51.755220 brainchain-0.6.5/brainchain/webapp/programs.py
--rw-r--r--   0        0        0      626 2024-05-07 16:51:51.755369 brainchain-0.6.5/brainchain/webapp/tasks.py
--rw-r--r--   0        0        0      853 2024-05-07 16:51:51.755565 brainchain-0.6.5/brainchain/webapp/tools.py
--rw-r--r--   0        0        0      677 2024-05-07 16:51:51.755730 brainchain-0.6.5/brainchain/webapp/users.py
--rw-r--r--   0        0        0      538 2024-05-10 17:26:18.966160 brainchain-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 brainchain-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.6.6/brainchain/README.md
+-rw-r--r--   0        0        0     2982 2024-05-10 17:23:42.151722 brainchain-0.6.6/brainchain/__init__.py
+-rw-r--r--   0        0        0    13624 2024-05-07 16:51:46.070229 brainchain-0.6.6/brainchain/assistants.py
+-rw-r--r--   0        0        0    11851 2024-05-10 18:23:33.058953 brainchain-0.6.6/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5663 2024-05-09 05:35:25.596909 brainchain-0.6.6/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2024-02-14 04:10:52.129450 brainchain-0.6.6/brainchain/coredata.py
+-rw-r--r--   0        0        0     2155 2023-09-12 01:13:30.915323 brainchain-0.6.6/brainchain/embeddings.py
+-rw-r--r--   0        0        0    17861 2024-05-11 18:01:39.002320 brainchain-0.6.6/brainchain/graph/base.py
+-rw-r--r--   0        0        0     7386 2024-05-10 17:23:37.046295 brainchain-0.6.6/brainchain/graph/schema.py
+-rw-r--r--   0        0        0     3426 2024-05-07 16:51:46.072116 brainchain-0.6.6/brainchain/logger.py
+-rw-r--r--   0        0        0    11959 2024-05-07 16:51:46.072448 brainchain-0.6.6/brainchain/products.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.6.6/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6024 2024-05-07 16:20:56.058058 brainchain-0.6.6/brainchain/sales_intel.py
+-rw-r--r--   0        0        0     1977 2024-02-29 23:10:12.854747 brainchain-0.6.6/brainchain/search_v2.py
+-rw-r--r--   0        0        0      595 2024-04-12 19:05:17.907126 brainchain-0.6.6/brainchain/tools/__init__.py
+-rw-r--r--   0        0        0     2118 2024-05-09 17:28:37.403805 brainchain-0.6.6/brainchain/tools/coding.py
+-rw-r--r--   0        0        0     3948 2024-05-07 16:51:46.073351 brainchain-0.6.6/brainchain/tools/diffbot.py
+-rw-r--r--   0        0        0      632 2024-02-29 23:10:12.855578 brainchain-0.6.6/brainchain/tools/factual.py
+-rw-r--r--   0        0        0     5800 2024-04-10 01:04:48.531327 brainchain-0.6.6/brainchain/tools/fts.py
+-rw-r--r--   0        0        0     1450 2024-02-29 23:10:12.856798 brainchain-0.6.6/brainchain/tools/graph.py
+-rw-r--r--   0        0        0     1029 2024-02-29 23:10:12.857047 brainchain-0.6.6/brainchain/tools/memory.py
+-rw-r--r--   0        0        0     2154 2024-02-29 23:10:12.857190 brainchain-0.6.6/brainchain/tools/plan.py
+-rw-r--r--   0        0        0     1660 2024-04-15 19:40:33.833814 brainchain-0.6.6/brainchain/tools/tokens.py
+-rw-r--r--   0        0        0    21273 2024-05-07 16:51:46.073960 brainchain-0.6.6/brainchain/tools/tools.py
+-rw-r--r--   0        0        0    12159 2024-05-07 16:51:46.074887 brainchain-0.6.6/brainchain/tools/web.py
+-rw-r--r--   0        0        0      731 2024-04-23 19:21:58.552351 brainchain-0.6.6/brainchain/tools.py
+-rw-r--r--   0        0        0      791 2024-05-07 16:51:51.752365 brainchain-0.6.6/brainchain/webapp/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-07 16:51:51.752653 brainchain-0.6.6/brainchain/webapp/agents.py
+-rw-r--r--   0        0        0      173 2024-05-07 16:51:51.752960 brainchain-0.6.6/brainchain/webapp/base.py
+-rw-r--r--   0        0        0      977 2024-05-07 16:51:51.753234 brainchain-0.6.6/brainchain/webapp/business_ideas.py
+-rw-r--r--   0        0        0     1282 2024-05-07 16:51:51.753423 brainchain-0.6.6/brainchain/webapp/contents.py
+-rw-r--r--   0        0        0      895 2024-05-07 16:51:51.753590 brainchain-0.6.6/brainchain/webapp/conversations.py
+-rw-r--r--   0        0        0       91 2024-05-07 16:51:51.753815 brainchain-0.6.6/brainchain/webapp/embedding_models.py
+-rw-r--r--   0        0        0     2709 2024-05-07 16:51:51.753990 brainchain-0.6.6/brainchain/webapp/embeddings.py
+-rw-r--r--   0        0        0     1138 2024-05-07 16:51:51.754142 brainchain-0.6.6/brainchain/webapp/files.py
+-rw-r--r--   0        0        0      218 2024-05-07 16:51:51.754320 brainchain-0.6.6/brainchain/webapp/health.py
+-rw-r--r--   0        0        0       90 2024-05-07 16:51:51.754539 brainchain-0.6.6/brainchain/webapp/language_models.py
+-rw-r--r--   0        0        0      622 2024-05-07 16:51:51.754700 brainchain-0.6.6/brainchain/webapp/laws.py
+-rw-r--r--   0        0        0     1110 2024-05-07 16:51:51.754849 brainchain-0.6.6/brainchain/webapp/messages.py
+-rw-r--r--   0        0        0     2220 2024-05-07 16:51:51.755068 brainchain-0.6.6/brainchain/webapp/namespaces.py
+-rw-r--r--   0        0        0     1029 2024-05-07 16:51:51.755220 brainchain-0.6.6/brainchain/webapp/programs.py
+-rw-r--r--   0        0        0      626 2024-05-07 16:51:51.755369 brainchain-0.6.6/brainchain/webapp/tasks.py
+-rw-r--r--   0        0        0      853 2024-05-07 16:51:51.755565 brainchain-0.6.6/brainchain/webapp/tools.py
+-rw-r--r--   0        0        0      677 2024-05-07 16:51:51.755730 brainchain-0.6.6/brainchain/webapp/users.py
+-rw-r--r--   0        0        0      538 2024-05-11 18:02:06.987486 brainchain-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 brainchain-0.6.6/PKG-INFO
```

### Comparing `brainchain-0.6.5/brainchain/README.md` & `brainchain-0.6.6/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/__init__.py` & `brainchain-0.6.6/brainchain/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/assistants` & `brainchain-0.6.6/brainchain/assistants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import requests
 import json
-from logger import log_function_info
-from tools import *
 import os
+from .logger import log_function_info
+from .tools import *
 import time
-import math
 
 class AssistantClient:
     def __init__(self, assistants_api_host: str = "https://assistants-api.brainchain.cloud", api_host: str = "https://api.brainchain.cloud"):
         self.API_HOST = api_host or os.getenv("ASSISTANTS_API_HOST") 
         self.ASSISTANTS_API_HOST = assistants_api_host or os.getenv("API_HOST")
         print(f"Brainchain API: {self.API_HOST}")
         print(f"Assistants API: {self.ASSISTANTS_API_HOST}")
```

### Comparing `brainchain-0.6.5/brainchain/brainchain.py` & `brainchain-0.6.6/brainchain/brainchain.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/carnivore.py` & `brainchain-0.6.6/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/coredata.py` & `brainchain-0.6.6/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/embeddings.py` & `brainchain-0.6.6/brainchain/embeddings.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/graph/base.py` & `brainchain-0.6.6/brainchain/graph/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from .schema import GraphSchema
 from neo4j import GraphDatabase
 from functools import lru_cache
+import matplotlib.pyplot as plt
+import networkx as nx
+import hashlib
+import neo4j
 
 import os
 import json
 GRAPH_URL = os.getenv("GRAPH_URL", "bolt://n4j.brainchain.cloud")
 GRAPH_USER = os.getenv("GRAPH_USER", "neo4j")
 GRAPH_PASSWORD = os.getenv("GRAPH_PASSWORD")
```

### Comparing `brainchain-0.6.5/brainchain/graph/schema.py` & `brainchain-0.6.6/brainchain/graph/schema.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/logger.py` & `brainchain-0.6.6/brainchain/logger.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/products.py` & `brainchain-0.6.6/brainchain/products.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/requirements.txt` & `brainchain-0.6.6/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/sales_intel.py` & `brainchain-0.6.6/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/search_v2.py` & `brainchain-0.6.6/brainchain/search_v2.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/tools/__init__.py` & `brainchain-0.6.6/brainchain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/tools/coding.py` & `brainchain-0.6.6/brainchain/tools/coding.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/tools/diffbot.py` & `brainchain-0.6.6/brainchain/tools/diffbot.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/tools/factual.py` & `brainchain-0.6.6/brainchain/tools/factual.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/tools/fts.py` & `brainchain-0.6.6/brainchain/tools/fts.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/tools/graph.py` & `brainchain-0.6.6/brainchain/tools/graph.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/tools/memory.py` & `brainchain-0.6.6/brainchain/tools/memory.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/tools/plan.py` & `brainchain-0.6.6/brainchain/tools/plan.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/tools/tokens.py` & `brainchain-0.6.6/brainchain/tools/tokens.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/tools/tools.py` & `brainchain-0.6.6/brainchain/tools/tools.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/tools/web.py` & `brainchain-0.6.6/brainchain/tools/web.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/tools.py` & `brainchain-0.6.6/brainchain/tools.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/webapp/__init__.py` & `brainchain-0.6.6/brainchain/webapp/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/webapp/business_ideas.py` & `brainchain-0.6.6/brainchain/webapp/business_ideas.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/webapp/contents.py` & `brainchain-0.6.6/brainchain/webapp/contents.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/webapp/conversations.py` & `brainchain-0.6.6/brainchain/webapp/conversations.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/webapp/embeddings.py` & `brainchain-0.6.6/brainchain/webapp/embeddings.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/webapp/files.py` & `brainchain-0.6.6/brainchain/webapp/files.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/webapp/laws.py` & `brainchain-0.6.6/brainchain/webapp/laws.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/webapp/messages.py` & `brainchain-0.6.6/brainchain/webapp/messages.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/webapp/namespaces.py` & `brainchain-0.6.6/brainchain/webapp/namespaces.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/webapp/programs.py` & `brainchain-0.6.6/brainchain/webapp/programs.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/webapp/tasks.py` & `brainchain-0.6.6/brainchain/webapp/tasks.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/webapp/tools.py` & `brainchain-0.6.6/brainchain/webapp/tools.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/brainchain/webapp/users.py` & `brainchain-0.6.6/brainchain/webapp/users.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.5/pyproject.toml` & `brainchain-0.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.6.5"
+version = "0.6.6"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 urllib3 = "2.0.6"
 requests = "2.31.0"
```

### Comparing `brainchain-0.6.5/PKG-INFO` & `brainchain-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.6.5
+Version: 0.6.6
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

