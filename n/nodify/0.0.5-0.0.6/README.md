# Comparing `tmp/nodify-0.0.5.tar.gz` & `tmp/nodify-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodify-0.0.5.tar", last modified: Wed Apr 24 11:45:04 2024, max compression
+gzip compressed data, was "nodify-0.0.6.tar", last modified: Sat May 11 16:11:30 2024, max compression
```

## Comparing `nodify-0.0.5.tar` & `nodify-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:45:04.774322 nodify-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-24 11:44:58.000000 nodify-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-24 11:45:04.774322 nodify-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 11:44:58.000000 nodify-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-24 11:44:58.000000 nodify-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 11:45:04.774322 nodify-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:45:04.766322 nodify-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:45:04.770322 nodify-0.0.5/src/nodify/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/file_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/syntax_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:45:04.770322 nodify-0.0.5/src/nodify/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/tests/test_file_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/tests/test_pythonscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/tests/test_syntax_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37802 2024-04-24 11:44:58.000000 nodify-0.0.5/src/nodify/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:45:04.770322 nodify-0.0.5/src/nodify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-24 11:45:04.000000 nodify-0.0.5/src/nodify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-24 11:45:04.000000 nodify-0.0.5/src/nodify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:45:04.000000 nodify-0.0.5/src/nodify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 11:45:04.000000 nodify-0.0.5/src/nodify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 11:45:04.000000 nodify-0.0.5/src/nodify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.608688 nodify-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-11 16:11:25.000000 nodify-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-11 16:11:30.608688 nodify-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-11 16:11:25.000000 nodify-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-11 16:11:25.000000 nodify-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 16:11:30.608688 nodify-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.596688 nodify-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.600688 nodify-0.0.6/src/nodify/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/file_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.604688 nodify-0.0.6/src/nodify/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.604688 nodify-0.0.6/src/nodify/server/flask_socketio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/flask_socketio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9357 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/flask_socketio/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/flask_socketio/emiters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/flask_socketio/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/flask_socketio/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29946 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/syntax_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.604688 nodify-0.0.6/src/nodify/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_file_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_pythonscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_syntax_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37803 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.608688 nodify-0.0.6/src/nodify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-11 16:11:30.000000 nodify-0.0.6/src/nodify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-11 16:11:30.000000 nodify-0.0.6/src/nodify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 16:11:30.000000 nodify-0.0.6/src/nodify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-11 16:11:30.000000 nodify-0.0.6/src/nodify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 16:11:30.000000 nodify-0.0.6/src/nodify.egg-info/top_level.txt
```

### Comparing `nodify-0.0.5/LICENSE` & `nodify-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/pyproject.toml` & `nodify-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [project]
 requires-python = ">=3.9"
 
 name = "nodify"
 description = "Supercharge your functional application with a powerful node system."
 readme = "README.md"
 license = {file = "LICENSE"}
-version = "0.0.5"
+version = "0.0.6"
 
 dependencies = []
 
 authors = [
     {name = "Pol Febrer", email = "pfebrer96@gmail.com"}
 ]
 maintainers = [{name="Pol Febrer", email = "pfebrer96@gmail.com"}]
@@ -45,14 +45,23 @@
     "pytest-env",
     "pytest-faulthandler",
     "black",
     "isort",
     "watchdog",
 ]
 
+docs = [
+    "sphinx",
+    "sphinx-rtd-theme",
+    "nbsphinx",
+    "pyvis",
+    "networkx",
+    "matplotlib",
+]
+
 
 [tool.pytest.ini_options]
 testpaths = [
     "src"
 ]
 markers = [
     "slow: mark a test as slow",
```

### Comparing `nodify-0.0.5/src/nodify/_env.py` & `nodify-0.0.6/src/nodify/_env.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,18 +24,18 @@
     process : callable, optional
         a callable which will be used to post-process the value when retrieving
         it.
 
     Raises
     ------
     ValueError
-       if `name` does not start with "NODES_"
+       if `name` does not start with "NODIFY_"
     """
-    if not name.startswith("NODES_"):
-        raise ValueError("register_environ_variable: name should start with 'NODES_'")
+    if not name.startswith("NODIFY_"):
+        raise ValueError("register_environ_variable: name should start with 'NODIFY_'")
     if process is None:
 
         def process(arg: Any) -> Any:
             return arg
 
     global NODES_ENV_VARIABLES
```

### Comparing `nodify-0.0.5/src/nodify/context.py` & `nodify-0.0.6/src/nodify/context.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/conversions.py` & `nodify-0.0.6/src/nodify/conversions.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/dispatcher.py` & `nodify-0.0.6/src/nodify/dispatcher.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/errors.py` & `nodify-0.0.6/src/nodify/errors.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/file_nodes.py` & `nodify-0.0.6/src/nodify/file_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/node.py` & `nodify-0.0.6/src/nodify/node.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/operators.py` & `nodify-0.0.6/src/nodify/operators.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/parse.py` & `nodify-0.0.6/src/nodify/parse.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/registry.py` & `nodify-0.0.6/src/nodify/registry.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/syntax_nodes.py` & `nodify-0.0.6/src/nodify/syntax_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/tests/test_context.py` & `nodify-0.0.6/src/nodify/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/tests/test_file_nodes.py` & `nodify-0.0.6/src/nodify/tests/test_file_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/tests/test_node.py` & `nodify-0.0.6/src/nodify/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/tests/test_pythonscript.py` & `nodify-0.0.6/src/nodify/tests/test_pythonscript.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/tests/test_registry.py` & `nodify-0.0.6/src/nodify/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/tests/test_syntax_nodes.py` & `nodify-0.0.6/src/nodify/tests/test_syntax_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/tests/test_utils.py` & `nodify-0.0.6/src/nodify/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/tests/test_workflow.py` & `nodify-0.0.6/src/nodify/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/utils.py` & `nodify-0.0.6/src/nodify/utils.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.5/src/nodify/workflow.py` & `nodify-0.0.6/src/nodify/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ._env import get_env_variable, register_env_variable
 from .context import temporal_context
 from .node import DummyInputValue, Node
 from .parse import nodify_func
 from .utils import traverse_tree_backward, traverse_tree_forward
 
 register_env_variable(
-    "NODES_EXPORT_VIS",
+    "NODIFY_EXPORT_VIS",
     default=False,
     description="Whether the visualizations of the networks in notebooks are meant to be exported.",
 )
 
 
 class WorkflowInput(DummyInputValue):
     pass
```

