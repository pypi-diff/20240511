# Comparing `tmp/devon_agent-0.1.1.tar.gz` & `tmp/devon_agent-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devon_agent-0.1.1.tar", max compression
+gzip compressed data, was "devon_agent-0.1.2.tar", max compression
```

## Comparing `devon_agent-0.1.1.tar` & `devon_agent-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,24 @@
--rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.1.1/LICENSE
--rw-r--r--   0        0        0     1463 2024-04-08 19:20:30.592278 devon_agent-0.1.1/README.md
--rw-r--r--   0        0        0      129 2024-05-10 17:13:36.831768 devon_agent-0.1.1/devon_agent/TODO
--rw-r--r--   0        0        0      794 2024-05-10 17:13:36.832076 devon_agent-0.1.1/devon_agent/__main__.py
--rw-r--r--   0        0        0     9751 2024-05-10 17:13:36.832377 devon_agent-0.1.1/devon_agent/agent.py
--rw-r--r--   0        0        0     2512 2024-05-10 17:13:36.832634 devon_agent-0.1.1/devon_agent/environment.py
--rw-r--r--   0        0        0     2195 2024-05-10 17:13:36.832781 devon_agent-0.1.1/devon_agent/model.py
--rw-r--r--   0        0        0    19947 2024-05-10 17:13:36.833052 devon_agent-0.1.1/devon_agent/prompt.py
--rw-r--r--   0        0        0     6312 2024-05-11 00:03:38.899715 devon_agent-0.1.1/devon_agent/server.py
--rw-r--r--   0        0        0    14732 2024-05-11 00:03:38.900376 devon_agent-0.1.1/devon_agent/session.py
--rw-r--r--   0        0        0     4607 2024-05-11 00:03:38.900486 devon_agent-0.1.1/devon_agent/telemetry.py
--rw-r--r--   0        0        0      898 2024-05-10 17:13:36.833911 devon_agent-0.1.1/devon_agent/test/test_tools.py
--rw-r--r--   0        0        0    42575 2024-05-11 00:03:38.900960 devon_agent-0.1.1/devon_agent/tools.py
--rw-r--r--   0        0        0    29381 2024-05-10 23:28:51.716909 devon_agent-0.1.1/devon_agent/udiff.py
--rw-r--r--   0        0        0      727 2024-05-10 17:13:36.835159 devon_agent-0.1.1/devon_agent/utils.py
--rw-r--r--   0        0        0     1509 2024-05-10 17:13:36.835377 devon_agent-0.1.1/devon_agent/vgit.py
--rw-r--r--   0        0        0     1127 2024-05-11 00:26:40.396257 devon_agent-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 devon_agent-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-17 15:42:25.856965 devon_agent-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1463 2024-04-08 19:20:30.592278 devon_agent-0.1.2/README.md
+-rw-r--r--   0        0        0      129 2024-05-10 17:13:36.831768 devon_agent-0.1.2/devon_agent/TODO
+-rw-r--r--   0        0        0      794 2024-05-10 17:13:36.832076 devon_agent-0.1.2/devon_agent/__main__.py
+-rw-r--r--   0        0        0     9751 2024-05-10 17:13:36.832377 devon_agent-0.1.2/devon_agent/agent.py
+-rw-r--r--   0        0        0     2512 2024-05-10 17:13:36.832634 devon_agent-0.1.2/devon_agent/environment.py
+-rw-r--r--   0        0        0     2195 2024-05-10 17:13:36.832781 devon_agent-0.1.2/devon_agent/model.py
+-rw-r--r--   0        0        0    19947 2024-05-10 17:13:36.833052 devon_agent-0.1.2/devon_agent/prompt.py
+-rw-r--r--   0        0        0     6334 2024-05-11 00:35:58.935374 devon_agent-0.1.2/devon_agent/retrieval/ast_extractor.py
+-rw-r--r--   0        0        0      561 2024-05-11 00:35:58.937331 devon_agent-0.1.2/devon_agent/retrieval/ast_parser.py
+-rw-r--r--   0        0        0     5222 2024-05-11 00:35:58.939359 devon_agent-0.1.2/devon_agent/retrieval/codebase_graph.py
+-rw-r--r--   0        0        0      849 2024-05-11 00:35:58.941356 devon_agent-0.1.2/devon_agent/retrieval/file_discovery.py
+-rw-r--r--   0        0        0     3660 2024-05-11 00:35:58.941798 devon_agent-0.1.2/devon_agent/retrieval/graph_visualization.py
+-rw-r--r--   0        0        0     9127 2024-05-11 00:35:58.942173 devon_agent-0.1.2/devon_agent/retrieval/main.py
+-rw-r--r--   0        0        0     6312 2024-05-11 00:03:38.899715 devon_agent-0.1.2/devon_agent/server.py
+-rw-r--r--   0        0        0    14732 2024-05-11 00:03:38.900376 devon_agent-0.1.2/devon_agent/session.py
+-rw-r--r--   0        0        0     4607 2024-05-11 00:03:38.900486 devon_agent-0.1.2/devon_agent/telemetry.py
+-rw-r--r--   0        0        0      898 2024-05-10 17:13:36.833911 devon_agent-0.1.2/devon_agent/test/test_tools.py
+-rw-r--r--   0        0        0    42558 2024-05-11 00:36:32.388456 devon_agent-0.1.2/devon_agent/tools.py
+-rw-r--r--   0        0        0    29381 2024-05-10 23:28:51.716909 devon_agent-0.1.2/devon_agent/udiff.py
+-rw-r--r--   0        0        0      727 2024-05-10 17:13:36.835159 devon_agent-0.1.2/devon_agent/utils.py
+-rw-r--r--   0        0        0     1509 2024-05-10 17:13:36.835377 devon_agent-0.1.2/devon_agent/vgit.py
+-rw-r--r--   0        0        0     1133 2024-05-11 00:37:33.365404 devon_agent-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 devon_agent-0.1.2/PKG-INFO
```

### Comparing `devon_agent-0.1.1/LICENSE` & `devon_agent-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/README.md` & `devon_agent-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/devon_agent/__main__.py` & `devon_agent-0.1.2/devon_agent/__main__.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/devon_agent/agent.py` & `devon_agent-0.1.2/devon_agent/agent.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/devon_agent/environment.py` & `devon_agent-0.1.2/devon_agent/environment.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/devon_agent/model.py` & `devon_agent-0.1.2/devon_agent/model.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/devon_agent/prompt.py` & `devon_agent-0.1.2/devon_agent/prompt.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/devon_agent/server.py` & `devon_agent-0.1.2/devon_agent/server.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/devon_agent/session.py` & `devon_agent-0.1.2/devon_agent/session.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/devon_agent/telemetry.py` & `devon_agent-0.1.2/devon_agent/telemetry.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/devon_agent/test/test_tools.py` & `devon_agent-0.1.2/devon_agent/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/devon_agent/tools.py` & `devon_agent-0.1.2/devon_agent/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import re
 import tarfile
 import tempfile
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Protocol, TypedDict
 from devon_agent.utils import DotDict
 
-from devon_swe_bench_experimental.retrieval.main import (
+from devon_agent.retrieval.main import (
     get_class_defn,
     get_function_defn,
     initialize_repository,
 )
 from devon_agent.udiff import (
     Hallucination,
     apply_file_context_diffs,
```

### Comparing `devon_agent-0.1.1/devon_agent/udiff.py` & `devon_agent-0.1.2/devon_agent/udiff.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/devon_agent/utils.py` & `devon_agent-0.1.2/devon_agent/utils.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/devon_agent/vgit.py` & `devon_agent-0.1.2/devon_agent/vgit.py`

 * *Files identical despite different names*

### Comparing `devon_agent-0.1.1/pyproject.toml` & `devon_agent-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "devon-agent"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["killind-dev <61808204+killind-dev@users.noreply.github.com>","mihir1003 <mihir1003@gmail.com>"]
 readme = "README.md"
 exclude = [
     "devon_tui",
 ]
 
@@ -40,9 +40,9 @@
 ruff = "^0.3.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-devon = "devon_agent.__main__:main"
+devon_agent = "devon_agent.__main__:main"
```

### Comparing `devon_agent-0.1.1/PKG-INFO` & `devon_agent-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devon-agent
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: killind-dev
 Author-email: 61808204+killind-dev@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

