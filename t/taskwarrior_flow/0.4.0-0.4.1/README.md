# Comparing `tmp/taskwarrior_flow-0.4.0.tar.gz` & `tmp/taskwarrior_flow-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskwarrior_flow-0.4.0.tar", max compression
+gzip compressed data, was "taskwarrior_flow-0.4.1.tar", max compression
```

## Comparing `taskwarrior_flow-0.4.0.tar` & `taskwarrior_flow-0.4.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-05-10 12:15:24.374409 taskwarrior_flow-0.4.0/LICENSE
--rw-r--r--   0        0        0     1452 2024-05-10 12:15:24.374409 taskwarrior_flow-0.4.0/README.md
--rw-r--r--   0        0        0     1035 2024-05-10 12:15:24.374409 taskwarrior_flow-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2261 2024-05-10 12:15:24.374409 taskwarrior_flow-0.4.0/tools/__init__.py
--rw-r--r--   0        0        0     3376 2024-05-10 12:15:24.374409 taskwarrior_flow-0.4.0/tools/main.py
--rw-r--r--   0        0        0    24555 2024-05-10 12:15:24.374409 taskwarrior_flow-0.4.0/tools/utils.py
--rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 taskwarrior_flow-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-11 03:29:07.279468 taskwarrior_flow-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1452 2024-05-11 03:29:07.279468 taskwarrior_flow-0.4.1/README.md
+-rw-r--r--   0        0        0     1035 2024-05-11 03:29:07.279468 taskwarrior_flow-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2261 2024-05-11 03:29:07.279468 taskwarrior_flow-0.4.1/tools/__init__.py
+-rw-r--r--   0        0        0     3376 2024-05-11 03:29:07.279468 taskwarrior_flow-0.4.1/tools/main.py
+-rw-r--r--   0        0        0    25307 2024-05-11 03:29:07.283468 taskwarrior_flow-0.4.1/tools/utils.py
+-rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 taskwarrior_flow-0.4.1/PKG-INFO
```

### Comparing `taskwarrior_flow-0.4.0/LICENSE` & `taskwarrior_flow-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.4.0/README.md` & `taskwarrior_flow-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.4.0/pyproject.toml` & `taskwarrior_flow-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskwarrior_flow"
-version = "0.4.0"
+version = "0.4.1"
 description = "Set of helpers for improving Taskwarrior workflow"
 authors = ["Ben Trinh <huantrinh1802@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "tools" }]
 
 [tool.poetry.scripts]
 twf = 'tools.main:app'
```

### Comparing `taskwarrior_flow-0.4.0/tools/__init__.py` & `taskwarrior_flow-0.4.1/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.4.0/tools/main.py` & `taskwarrior_flow-0.4.1/tools/main.py`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.4.0/tools/utils.py` & `taskwarrior_flow-0.4.1/tools/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,36 +236,55 @@
             elif field["type"] == "list":
                 parts += " " + " ".join(
                     field["template"].replace("%s", item) if item != "" else "" for item in answers[name]
                 )
             else:
                 parts += " " + field["template"].replace("%s", value)
     command = tw_config["add_templates"]["data"][chosen_template]["command"].replace("%s", parts)
-    confirm = safe_ask(questionary.confirm("Add task?", instruction=f"\n{command}\n", style=question_style))
-    if confirm:
-        uuid_compiled = re.compile(r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}")
-        result = subprocess.run(
-            f"{group_mappings[group]} task rc.verbose=new-uuid add {command}",
-            capture_output=True,
-            text=True,
-            shell=True,
+    confirm = "edit"
+    while confirm == "edit":
+        confirm = safe_ask(
+            questionary.rawselect(
+                "Add task?",
+                choices=["yes", "edit", "no"],
+                default="yes",
+                instruction=f"\n{command}\n",
+                style=question_style,
+            )
         )
-        if result.stderr:
-            print(result.stderr)
-        uuid_match = uuid_compiled.search(result.stdout)
-        if uuid_match:
-            uuid = uuid_match.group()
-            if annotations:
-                for annotate in annotations:
-                    result = subprocess.run(
-                        f"{group_mappings[group]} task {uuid} annotate {annotate}",
-                        capture_output=True,
-                        text=True,
-                        shell=True,
-                    )
+        match confirm:
+            case "yes":
+                uuid_compiled = re.compile(r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}")
+                result = subprocess.run(
+                    f"{group_mappings[group]} task rc.verbose=new-uuid add {command}",
+                    capture_output=True,
+                    text=True,
+                    shell=True,
+                )
+                if result.stderr:
+                    print(result.stderr)
+                uuid_match = uuid_compiled.search(result.stdout)
+                if uuid_match:
+                    uuid = uuid_match.group()
+                    if annotations:
+                        for annotate in annotations:
+                            result = subprocess.run(
+                                f"{group_mappings[group]} task {uuid} annotate {annotate}",
+                                capture_output=True,
+                                text=True,
+                                shell=True,
+                            )
+            case "edit":
+                if isinstance(command, str):
+                    command = safe_ask(questionary.text("Edit command", style=question_style, default=command))
+                else:
+                    print("Cannot edit command")
+            case "no":
+                print("Cancelled by user")
+                return
 
 
 def create_group(*_):
     result = safe_ask(
         questionary.form(
             name=questionary.text("Enter name", style=question_style),
             data=questionary.text("Enter data location", style=question_style),
```

### Comparing `taskwarrior_flow-0.4.0/PKG-INFO` & `taskwarrior_flow-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskwarrior_flow
-Version: 0.4.0
+Version: 0.4.1
 Summary: Set of helpers for improving Taskwarrior workflow
 Author: Ben Trinh
 Author-email: huantrinh1802@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

