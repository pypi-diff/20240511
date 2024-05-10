# Comparing `tmp/altscore_workflow_builder-0.0.8.tar.gz` & `tmp/altscore_workflow_builder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altscore_workflow_builder-0.0.8.tar", last modified: Fri May 10 20:20:16 2024, max compression
+gzip compressed data, was "altscore_workflow_builder-0.0.9.tar", last modified: Fri May 10 20:37:20 2024, max compression
```

## Comparing `altscore_workflow_builder-0.0.8.tar` & `altscore_workflow_builder-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:16.266027 altscore_workflow_builder-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 20:20:16.266027 altscore_workflow_builder-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:20:16.266027 altscore_workflow_builder-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:16.262027 altscore_workflow_builder-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:16.262027 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/Home.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/launch_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:16.266027 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Borrowers.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Packages.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Workflow_Inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Workflow_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-10 20:20:12.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:20:16.266027 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 20:20:16.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-10 20:20:16.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:20:16.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-10 20:20:16.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 20:20:16.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 20:20:16.000000 altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:37:20.630730 altscore_workflow_builder-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 20:37:20.630730 altscore_workflow_builder-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:37:20.630730 altscore_workflow_builder-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:37:20.626730 altscore_workflow_builder-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:37:20.626730 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/Home.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/launch_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:37:20.630730 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/pages/Borrowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/pages/Evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/pages/Packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/pages/Rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/pages/Workflow_Inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/pages/Workflow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-10 20:37:15.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:37:20.630730 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-10 20:37:20.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-10 20:37:20.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:37:20.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-10 20:37:20.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 20:37:20.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 20:37:20.000000 altscore_workflow_builder-0.0.9/src/altscore_workflow_builder.egg-info/top_level.txt
```

### Comparing `altscore_workflow_builder-0.0.8/LICENSE` & `altscore_workflow_builder-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.8/PKG-INFO` & `altscore_workflow_builder-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altscore-workflow-builder
-Version: 0.0.8
+Version: 0.0.9
 Summary: Streamlit-based workflow builder for AltScore
 Home-page: https://github.com/altscore/altscore-python
 Author: AltScore
 Author-email: developers@altscore.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `altscore_workflow_builder-0.0.8/setup.py` & `altscore_workflow_builder-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 long_description = "Streamlit-based workflow builder for AltScore"
 
 setup(
     name="altscore-workflow-builder",
-    version="0.0.8",
+    version="0.0.9",
     description="Streamlit-based workflow builder for AltScore",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/altscore/altscore-python",
     author="AltScore",
```

### Comparing `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/launch_app.py` & `altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/launch_app.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Borrowers.py` & `altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/pages/Borrowers.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Evaluators.py` & `altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/pages/Evaluators.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Packages.py` & `altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/pages/Packages.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Workflow_Inspector.py` & `altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/pages/Workflow_Inspector.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/pages/Workflow_builder.py` & `altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/pages/Workflow_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,11 +93,13 @@
         try:
             task_details['inputs'] = json.loads(input_json)
             task_details['outputs'] = json.loads(output_json)
             task_info['input_override'] = json.loads(input_override)
             task_info['input_conversion'] = json.loads(input_conversion)
             save_workflow_definition(workflow['alias'], workflow['version'], flow_definition)
             save_task_definitions(task_definitions)
+            if new_edges != current_edges:
+                task_nodes[selected_task]["to"] = new_edges
             st.sidebar.success("Changes saved successfully!")
-            st.experimental_rerun()
+            st.rerun()
         except json.JSONDecodeError:
             st.sidebar.error("Invalid JSON format. Please check your input.")
```

### Comparing `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/utils.py` & `altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,27 +46,25 @@
                  os.path.isdir(Path(config("PROJECT_ROOT")) / "app" / "workflows" / f)]
     return [
         {"alias": workflow.split("_")[0], "version": workflow.split("_")[-1], "label": workflow} for workflow in
         workflows
     ]
 
 
-def calculate_task_levels(task_nodes):
+def calculate_task_levels(task_nodes, scale=100):
     levels = {}
     queue = []
 
-    # Start with tasks that have no incoming edges (sources)
     sources = [task for task, details in task_nodes.items() if
                all(task not in t.get("to", []) for t in task_nodes.values())]
     for source in sources:
         queue.append((source, 0))  # (task_name, level)
 
-    # BFS to assign levels
     while queue:
         current_task, current_level = queue.pop(0)
         if current_task in levels:
             continue
-        levels[current_task] = current_level
+        levels[current_task] = current_level * scale  # Scale horizontal positions
         for next_task in task_nodes[current_task].get("to", []):
             queue.append((next_task, current_level + 1))
 
     return levels
```

### Comparing `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder/workflow.py` & `altscore_workflow_builder-0.0.9/src/altscore_workflow_builder/workflow.py`

 * *Files identical despite different names*

### Comparing `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/PKG-INFO` & `altscore_workflow_builder-0.0.9/src/altscore_workflow_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altscore-workflow-builder
-Version: 0.0.8
+Version: 0.0.9
 Summary: Streamlit-based workflow builder for AltScore
 Home-page: https://github.com/altscore/altscore-python
 Author: AltScore
 Author-email: developers@altscore.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `altscore_workflow_builder-0.0.8/src/altscore_workflow_builder.egg-info/SOURCES.txt` & `altscore_workflow_builder-0.0.9/src/altscore_workflow_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

