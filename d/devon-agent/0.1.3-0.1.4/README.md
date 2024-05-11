# Comparing `tmp/devon_agent-0.1.3.tar.gz` & `tmp/devon_agent-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devon_agent-0.1.3.tar", max compression
+gzip compressed data, was "devon_agent-0.1.4.tar", max compression
```

## Comparing `devon_agent-0.1.3.tar` & `devon_agent-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.1.3/LICENSE
--rw-r--r--   0        0        0     1463 2024-04-08 19:20:30.592278 devon_agent-0.1.3/README.md
--rw-r--r--   0        0        0      129 2024-05-10 17:13:36.831768 devon_agent-0.1.3/devon_agent/TODO
--rw-r--r--   0        0        0      794 2024-05-10 17:13:36.832076 devon_agent-0.1.3/devon_agent/__main__.py
--rw-r--r--   0        0        0     9751 2024-05-10 17:13:36.832377 devon_agent-0.1.3/devon_agent/agent.py
--rw-r--r--   0        0        0     2512 2024-05-10 17:13:36.832634 devon_agent-0.1.3/devon_agent/environment.py
--rw-r--r--   0        0        0     2195 2024-05-10 17:13:36.832781 devon_agent-0.1.3/devon_agent/model.py
--rw-r--r--   0        0        0    19947 2024-05-10 17:13:36.833052 devon_agent-0.1.3/devon_agent/prompt.py
--rw-r--r--   0        0        0     6334 2024-05-11 00:35:58.935374 devon_agent-0.1.3/devon_agent/retrieval/ast_extractor.py
--rw-r--r--   0        0        0      561 2024-05-11 00:35:58.937331 devon_agent-0.1.3/devon_agent/retrieval/ast_parser.py
--rw-r--r--   0        0        0     5222 2024-05-11 00:35:58.939359 devon_agent-0.1.3/devon_agent/retrieval/codebase_graph.py
--rw-r--r--   0        0        0      849 2024-05-11 00:35:58.941356 devon_agent-0.1.3/devon_agent/retrieval/file_discovery.py
--rw-r--r--   0        0        0     3660 2024-05-11 00:35:58.941798 devon_agent-0.1.3/devon_agent/retrieval/graph_visualization.py
--rw-r--r--   0        0        0     9127 2024-05-11 00:35:58.942173 devon_agent-0.1.3/devon_agent/retrieval/main.py
--rw-r--r--   0        0        0     6312 2024-05-11 00:03:38.899715 devon_agent-0.1.3/devon_agent/server.py
--rw-r--r--   0        0        0    14732 2024-05-11 00:03:38.900376 devon_agent-0.1.3/devon_agent/session.py
--rw-r--r--   0        0        0     4607 2024-05-11 00:03:38.900486 devon_agent-0.1.3/devon_agent/telemetry.py
--rw-r--r--   0        0        0      898 2024-05-10 17:13:36.833911 devon_agent-0.1.3/devon_agent/test/test_tools.py
--rw-r--r--   0        0        0    42558 2024-05-11 00:36:32.388456 devon_agent-0.1.3/devon_agent/tools.py
--rw-r--r--   0        0        0    29381 2024-05-10 23:28:51.716909 devon_agent-0.1.3/devon_agent/udiff.py
--rw-r--r--   0        0        0      727 2024-05-10 17:13:36.835159 devon_agent-0.1.3/devon_agent/utils.py
--rw-r--r--   0        0        0     1509 2024-05-10 17:13:36.835377 devon_agent-0.1.3/devon_agent/vgit.py
--rw-r--r--   0        0        0     1131 2024-05-11 01:11:49.959967 devon_agent-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 devon_agent-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1463 2024-04-08 19:20:30.592278 devon_agent-0.1.4/README.md
+-rw-r--r--   0        0        0      129 2024-05-10 17:13:36.831768 devon_agent-0.1.4/devon_agent/TODO
+-rw-r--r--   0        0        0      794 2024-05-10 17:13:36.832076 devon_agent-0.1.4/devon_agent/__main__.py
+-rw-r--r--   0        0        0     9751 2024-05-10 17:13:36.832377 devon_agent-0.1.4/devon_agent/agent.py
+-rw-r--r--   0        0        0     2512 2024-05-10 17:13:36.832634 devon_agent-0.1.4/devon_agent/environment.py
+-rw-r--r--   0        0        0     2195 2024-05-10 17:13:36.832781 devon_agent-0.1.4/devon_agent/model.py
+-rw-r--r--   0        0        0    19947 2024-05-10 17:13:36.833052 devon_agent-0.1.4/devon_agent/prompt.py
+-rw-r--r--   0        0        0     6317 2024-05-11 01:42:20.814775 devon_agent-0.1.4/devon_agent/retrieval/ast_extractor.py
+-rw-r--r--   0        0        0      561 2024-05-11 00:35:58.937331 devon_agent-0.1.4/devon_agent/retrieval/ast_parser.py
+-rw-r--r--   0        0        0     5222 2024-05-11 00:35:58.939359 devon_agent-0.1.4/devon_agent/retrieval/codebase_graph.py
+-rw-r--r--   0        0        0      849 2024-05-11 00:35:58.941356 devon_agent-0.1.4/devon_agent/retrieval/file_discovery.py
+-rw-r--r--   0        0        0     3660 2024-05-11 00:35:58.941798 devon_agent-0.1.4/devon_agent/retrieval/graph_visualization.py
+-rw-r--r--   0        0        0     9059 2024-05-11 01:41:30.027339 devon_agent-0.1.4/devon_agent/retrieval/main.py
+-rw-r--r--   0        0        0     6312 2024-05-11 00:03:38.899715 devon_agent-0.1.4/devon_agent/server.py
+-rw-r--r--   0        0        0    14732 2024-05-11 00:03:38.900376 devon_agent-0.1.4/devon_agent/session.py
+-rw-r--r--   0        0        0     4607 2024-05-11 00:03:38.900486 devon_agent-0.1.4/devon_agent/telemetry.py
+-rw-r--r--   0        0        0      811 2024-05-11 01:43:13.118702 devon_agent-0.1.4/devon_agent/test/test_tools.py
+-rw-r--r--   0        0        0    42558 2024-05-11 00:36:32.388456 devon_agent-0.1.4/devon_agent/tools.py
+-rw-r--r--   0        0        0    29381 2024-05-10 23:28:51.716909 devon_agent-0.1.4/devon_agent/udiff.py
+-rw-r--r--   0        0        0      727 2024-05-10 17:13:36.835159 devon_agent-0.1.4/devon_agent/utils.py
+-rw-r--r--   0        0        0     1509 2024-05-10 17:13:36.835377 devon_agent-0.1.4/devon_agent/vgit.py
+-rw-r--r--   0        0        0     1131 2024-05-11 01:43:40.992093 devon_agent-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 devon_agent-0.1.4/PKG-INFO
```

### Comparing `devon_agent-0.1.3/LICENSE` & `devon_agent-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/README.md` & `devon_agent-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/__main__.py` & `devon_agent-0.1.4/devon_agent/__main__.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/agent.py` & `devon_agent-0.1.4/devon_agent/agent.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/environment.py` & `devon_agent-0.1.4/devon_agent/environment.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/model.py` & `devon_agent-0.1.4/devon_agent/model.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/prompt.py` & `devon_agent-0.1.4/devon_agent/prompt.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/retrieval/ast_extractor.py` & `devon_agent-0.1.4/devon_agent/retrieval/ast_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ast_extractor.py
 
 import ast
-from devon_swe_bench_experimental.retrieval.codebase_graph import add_node, add_edge
+from devon_agent.retrieval.codebase_graph import add_node, add_edge
 import networkx as nx
 import os
 
 def extract_info_from_ast(graph, ast_tree, file_path):
     # Add file node to the graph
 
     def nestedTestFunction():
```

### Comparing `devon_agent-0.1.3/devon_agent/retrieval/ast_parser.py` & `devon_agent-0.1.4/devon_agent/retrieval/ast_parser.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/retrieval/codebase_graph.py` & `devon_agent-0.1.4/devon_agent/retrieval/codebase_graph.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/retrieval/file_discovery.py` & `devon_agent-0.1.4/devon_agent/retrieval/file_discovery.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/retrieval/graph_visualization.py` & `devon_agent-0.1.4/devon_agent/retrieval/graph_visualization.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/retrieval/main.py` & `devon_agent-0.1.4/devon_agent/retrieval/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # main.py
 
 from functools import reduce
 import json
 import os
 import tarfile
 import tempfile
-from devon_swe_bench_experimental.retrieval.file_discovery import discover_python_files
-from devon_swe_bench_experimental.retrieval.ast_parser import parse_python_file
-from devon_swe_bench_experimental.retrieval.ast_extractor import extract_info_from_ast
-from devon_swe_bench_experimental.retrieval.codebase_graph import create_graph
+from devon_agent.retrieval.file_discovery import discover_python_files
+from devon_agent.retrieval.ast_parser import parse_python_file
+from devon_agent.retrieval.ast_extractor import extract_info_from_ast
+from devon_agent.retrieval.codebase_graph import create_graph
 
 
 class FunctionTable:
     
     def __init__(self,temp_dir=None):
         self.function_table = {}
         self.temp_dir = temp_dir if temp_dir is not None else ""
```

### Comparing `devon_agent-0.1.3/devon_agent/server.py` & `devon_agent-0.1.4/devon_agent/server.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/session.py` & `devon_agent-0.1.4/devon_agent/session.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/telemetry.py` & `devon_agent-0.1.4/devon_agent/telemetry.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/test/test_tools.py` & `devon_agent-0.1.4/devon_agent/test/test_tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from pathlib import Path
 
-from devon_swe_bench_experimental.environment.environment import LocalEnvironment
-from devon_swe_bench_experimental.environment.tools import create_file
-from devon_swe_bench_experimental.environment.utils import DotDict
+from devon_agent.environment import LocalEnvironment
+from devon_agent.tools import create_file
+from devon_agent.utils import DotDict
 
 
 def test_create_file():
     # make temp dir
     import tempfile
 
     temp_dir = tempfile.mkdtemp()
```

### Comparing `devon_agent-0.1.3/devon_agent/tools.py` & `devon_agent-0.1.4/devon_agent/tools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/udiff.py` & `devon_agent-0.1.4/devon_agent/udiff.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/utils.py` & `devon_agent-0.1.4/devon_agent/utils.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/devon_agent/vgit.py` & `devon_agent-0.1.4/devon_agent/vgit.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.3/pyproject.toml` & `devon_agent-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "devon-agent"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["killind-dev <61808204+killind-dev@users.noreply.github.com>","mihir1003 <mihir1003@gmail.com>"]
 readme = "README.md"
 exclude = [
     "devon_tui",
 ]
```

### Comparing `devon_agent-0.1.3/PKG-INFO` & `devon_agent-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devon-agent
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: killind-dev
 Author-email: 61808204+killind-dev@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

