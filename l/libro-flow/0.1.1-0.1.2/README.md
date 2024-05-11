# Comparing `tmp/libro_flow-0.1.1.tar.gz` & `tmp/libro_flow-0.1.2.tar.gz`

## Comparing `libro_flow-0.1.1.tar` & `libro_flow-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libro_flow-0.1.1/.python-version
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 libro_flow-0.1.1/src/libro_flow/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libro_flow-0.1.1/src/libro_flow/_version.py
--rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 libro_flow-0.1.1/src/libro_flow/libro_client.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 libro_flow-0.1.1/src/libro_flow/libro_execution.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 libro_flow-0.1.1/src/libro_flow/libro_schema_form_widget.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 libro_flow-0.1.1/.gitignore
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 libro_flow-0.1.1/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 libro_flow-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 libro_flow-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libro_flow-0.1.2/.python-version
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 libro_flow-0.1.2/src/libro_flow/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 libro_flow-0.1.2/src/libro_flow/_version.py
+-rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 libro_flow-0.1.2/src/libro_flow/libro_client.py
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 libro_flow-0.1.2/src/libro_flow/libro_execution.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 libro_flow-0.1.2/src/libro_flow/libro_schema_form_widget.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 libro_flow-0.1.2/.gitignore
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 libro_flow-0.1.2/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 libro_flow-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 libro_flow-0.1.2/PKG-INFO
```

### Comparing `libro_flow-0.1.1/src/libro_flow/libro_client.py` & `libro_flow-0.1.2/src/libro_flow/libro_client.py`

 * *Files identical despite different names*

### Comparing `libro_flow-0.1.1/src/libro_flow/libro_execution.py` & `libro_flow-0.1.2/src/libro_flow/libro_execution.py`

 * *Files 19% similar despite different names*

```diff
@@ -112,7 +112,34 @@
         execute_record_path=execute_record_path,
         **kwargs,
     )
     client.update_execution()
     asyncio.create_task(client.async_execute())
     display(client.execute_result_path)
     return client
+
+
+def execute_notebook_sync(
+    notebook: Any,
+    args=None,
+    execute_result_path: str | None = None,
+    execute_record_path: str | None = None,
+    notebook_parser: Callable | None = None,
+    km: Union[KernelManager, None] = None,
+    **kwargs: Any,
+):
+    if notebook_parser is not None:
+        nb = notebook_parser(notebook)
+    else:
+        nb = load_notebook_node(notebook)
+    client = LibroNotebookClient(
+        nb=nb,
+        km=km,
+        args=args,
+        execute_result_path=execute_result_path,
+        execute_record_path=execute_record_path,
+        **kwargs,
+    )
+    client.update_execution()
+    client.execute()
+    display(client.execute_result_path)
+    return client
```

### Comparing `libro_flow-0.1.1/src/libro_flow/libro_schema_form_widget.py` & `libro_flow-0.1.2/src/libro_flow/libro_schema_form_widget.py`

 * *Files identical despite different names*

### Comparing `libro_flow-0.1.1/pyproject.toml` & `libro_flow-0.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "libro-flow"
-version = "0.1.1"
+version = "0.1.2"
 description = "libro flow"
 authors = [
     { name = "brokun", email = "brokun0128@gmail.com" },
     { name = "sunshinesmilelk", email= "1176136681@qq.com"},
     { name = "zhanba", email = "c5e1856@gmail.com" }
 ]
 dependencies = [
```

