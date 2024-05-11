# Comparing `tmp/taskwarrior_flow-0.3.2.tar.gz` & `tmp/taskwarrior_flow-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskwarrior_flow-0.3.2.tar", max compression
+gzip compressed data, was "taskwarrior_flow-0.4.0.tar", max compression
```

## Comparing `taskwarrior_flow-0.3.2.tar` & `taskwarrior_flow-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-05-08 07:52:16.381068 taskwarrior_flow-0.3.2/LICENSE
--rw-r--r--   0        0        0     1452 2024-05-08 07:52:16.381068 taskwarrior_flow-0.3.2/README.md
--rw-r--r--   0        0        0     1035 2024-05-08 07:52:16.381068 taskwarrior_flow-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1351 2024-05-08 07:52:16.381068 taskwarrior_flow-0.3.2/tools/__init__.py
--rw-r--r--   0        0        0     3376 2024-05-08 07:52:16.381068 taskwarrior_flow-0.3.2/tools/main.py
--rw-r--r--   0        0        0    20383 2024-05-08 07:52:16.381068 taskwarrior_flow-0.3.2/tools/utils.py
--rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 taskwarrior_flow-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-10 12:15:24.374409 taskwarrior_flow-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1452 2024-05-10 12:15:24.374409 taskwarrior_flow-0.4.0/README.md
+-rw-r--r--   0        0        0     1035 2024-05-10 12:15:24.374409 taskwarrior_flow-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2261 2024-05-10 12:15:24.374409 taskwarrior_flow-0.4.0/tools/__init__.py
+-rw-r--r--   0        0        0     3376 2024-05-10 12:15:24.374409 taskwarrior_flow-0.4.0/tools/main.py
+-rw-r--r--   0        0        0    24555 2024-05-10 12:15:24.374409 taskwarrior_flow-0.4.0/tools/utils.py
+-rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 taskwarrior_flow-0.4.0/PKG-INFO
```

### Comparing `taskwarrior_flow-0.3.2/LICENSE` & `taskwarrior_flow-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.3.2/README.md` & `taskwarrior_flow-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.3.2/pyproject.toml` & `taskwarrior_flow-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskwarrior_flow"
-version = "0.3.2"
+version = "0.4.0"
 description = "Set of helpers for improving Taskwarrior workflow"
 authors = ["Ben Trinh <huantrinh1802@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "tools" }]
 
 [tool.poetry.scripts]
 twf = 'tools.main:app'
```

### Comparing `taskwarrior_flow-0.3.2/tools/__init__.py` & `taskwarrior_flow-0.4.0/tools/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,29 +2,49 @@
 import os
 
 config_file = os.environ.get("TW_CONFIG", f'{os.path.expanduser("~")}/.local/share/nvim/m_taskwarrior_d.json')
 if os.path.isfile(config_file):
     with open(config_file, "r") as f:
         tw_config = json.load(f)
 else:
-    if config_file == '/tmp/m_taskwarrior_d.json':
+    if config_file == "/tmp/m_taskwarrior_d.json":
         with open(config_file, "w") as f:
             tw_config = {
                 "use_mtwd": False,
-                "flow_config": {"task": {"data": "~/.task", "config": "~/.taskrc"}},
-
-                "saved_queries": {"name_max_length": 0, "data": [{"query": "project:Test", "name": "Test"}]},
+                "flow_config": {
+                    "task": {"data": "~/.task", "config": "~/.taskrc"},
+                    "work": {"data": "~/.task_work", "config": "~/.taskrc"},
+                    "test": {"data": "~/.task_test", "config": "~/.taskrc"},
+                },
+                "add_templates": {
+                    "date_fields": ["due", "scheduled"],
+                    "data": [
+                        {
+                            "name": "Bills",
+                            "command": "add %s +TDBillsS +bill +home +todoist +utility wait:due-1day",
+                            "fields": {
+                                "description": {"template": "'%s'", "type": "text"},
+                                "project": {"template": "project:%s", "type": "text"},
+                                "due": {"template": "due:%s", "type": "date"},
+                            },
+                        },
+                    ],
+                },
+                "saved_queries": {
+                    "name_max_length": 14,
+                    "data": [{"query": "project:Test", "name": "Test project"}],
+                },
             }
             f.write(json.dumps(tw_config))
     else:
         with open(config_file, "w") as f:
             tw_config = {
                 "use_mtwd": False,
                 "flow_config": {"task": {"data": "~/.task", "config": "~/.taskrc"}},
-                "add_templates": {"date_fields": ["due", "scheduled"], "data": []},
+                "add_templates": {"data": []},
                 "saved_queries": {"name_max_length": 0, "data": []},
             }
             f.write(json.dumps(tw_config))
 group_mappings = {key: f'TASKDATA={value["data"]}' for key, value in tw_config["flow_config"].items()}
 
 
 def group_mappings_completion():
```

### Comparing `taskwarrior_flow-0.3.2/tools/main.py` & `taskwarrior_flow-0.4.0/tools/main.py`

 * *Files identical despite different names*

### Comparing `taskwarrior_flow-0.3.2/tools/utils.py` & `taskwarrior_flow-0.4.0/tools/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 import re
 import shutil
 import subprocess
+from datetime import datetime
 from typing import Annotated, Callable, TypedDict
 
 import dateparser
 import questionary
 import typer
 from prompt_toolkit.shortcuts import CompleteStyle
 from rich import print as rprint
@@ -24,31 +25,86 @@
         ("selected", "fg:white"),  # style for a selected item of a checkbox
         ("separator", "fg:#008888"),  # separator in lists
         ("instruction", "fg:#858585"),  # user instructions for select, rawselect, checkbox
         ("text", ""),  # plain text
         ("disabled", "fg:#858585 italic"),  # disabled choices for select and checkbox prompts
     ]
 )
+preset_questions = ["project", "tags"]
 
 
+def date_parser(date_str):
+    result = subprocess.run(f"task calc {date_str}", capture_output=True, text=True, shell=True)
+    if (
+        result.stderr
+        or result.stdout.replace("\n", "") == ""
+        or result.stdout.replace("\n", "") == date_str
+        or "P" in result.stdout
+    ):
+        parsed = dateparser.parse(date_str)
+        if parsed:
+            return parsed
+        else:
+            return None
+    else:
+        return datetime.fromisoformat(result.stdout.strip("\n"))
+
+
+def get_preset_questions(group, field):
+    projects = (
+        subprocess.run(f"{group_mappings[group]} task _projects", shell=True, capture_output=True)
+        .stdout.decode()
+        .split("\n")
+    )
+    tags = (
+        subprocess.run(f"{group_mappings[group]} task _tags", shell=True, capture_output=True)
+        .stdout.decode()
+        .split("\n")
+    )
+    match field:
+        case "project":
+            return questionary.autocomplete(
+                "Enter project",
+                choices=projects,
+                style=question_style,
+                complete_style=CompleteStyle.MULTI_COLUMN,
+            )
+        case "tags":
+            return questionary.autocomplete(
+                "Enter tags",
+                choices=tags,
+                style=question_style,
+                complete_style=CompleteStyle.MULTI_COLUMN,
+            )
+    return None
+
 
 class FunctionsGroup(TypedDict):
     func: Callable
     help: str
 
 
 class DateValidator(questionary.Validator):
-    def validate(self, document):
-        if dateparser.parse(document.text) or len(document.text) == 0:
-            return True
+    def validate(self, document):  # type: ignore
+        result = subprocess.run(f"task calc {document.text}", capture_output=True, text=True, shell=True)
+        if (
+            result.stderr
+            or result.stdout == ""
+            or result.stdout.replace("\n", "") == document.text
+            or "P" in result.stdout
+        ):
+            if dateparser.parse(document.text) or len(document.text) == 0:
+                return True
+            else:
+                raise questionary.ValidationError(
+                    message="Invalid date",
+                    cursor_position=len(document.text),
+                )
         else:
-            raise questionary.ValidationError(
-                message="Invalid date",
-                cursor_position=len(document.text),
-            )
+            return True
 
 
 def safe_ask(question):
     try:
         response = question.unsafe_ask()
         return response
     except KeyboardInterrupt:
@@ -89,18 +145,29 @@
     print("<---------Fields--------->")
     field_name = "placeholder"
     while field_name != "":
         field_name = safe_ask(questionary.text("Enter field name", style=question_style))
         if field_name is None:
             return
         if field_name != "":
-            field_template = safe_ask(questionary.text("Enter field template", style=question_style))
-            if field_template is None:
+            field_form = safe_ask(
+                questionary.form(
+                    template=questionary.text("Enter field template", style=question_style),
+                    type=questionary.rawselect(
+                        "Select type of the field",
+                        choices=["text", "list", "date"],
+                        default="text",
+                        use_jk_keys=True,
+                        style=question_style,
+                    ),
+                )
+            )
+            if field_form is None:
                 return
-            template["fields"][field_name] = field_template
+            template["fields"][field_name] = {"template": field_form["template"], "type": field_form["type"]}
             print("To end enter nothing")
     with open(config_file, "w") as f:
         tw_config["add_templates"]["data"].append(template)
         f.write(json.dumps(tw_config))
 
 
 def create_task(group):
@@ -109,53 +176,85 @@
         for index, template in enumerate(tw_config["add_templates"]["data"])
     ]
     chosen_template = safe_ask(
         questionary.rawselect("Select template", choices=templates, use_jk_keys=True, style=question_style)
     )
     if chosen_template is None:
         return
-    questions = {}
-    preset_questions = get_preset_questions(group)
+    answers = {}
     for name, field in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
-        if name in preset_questions:
-            questions[name] = preset_questions[name]
-        elif name in tw_config["add_templates"]["date_fields"]:
-            questions[name] = questionary.text(f"Enter {name}", style=question_style, validate=DateValidator)
+        if field["type"] == "list":
+            answer = "placeholder"
+            answers[name] = []
+            while answer != "" and answer is not None:
+                if name in preset_questions:
+                    answer = safe_ask(get_preset_questions(group, name))
+                else:
+                    answer = safe_ask(
+                        questionary.text(f"Enter {name}", style=question_style, instruction="Leave blank to stop\n")
+                    )
+                if answer is not None:
+                    if answer != "":
+                        answers[name].append(answer)
+                        questionary.print("Leave blank to stop", style="fg:#858585")
+                else:
+                    return
+        elif field["type"] == "date":
+            answer = safe_ask(questionary.text(f"Enter {name}", style=question_style, validate=DateValidator))
+            if answer is None:
+                return
+            answers[name] = answer
         else:
-            questions[name] = questionary.text(f"Enter {name}", instruction="Use ';' for list\n", style=question_style)
-    answers = safe_ask(questionary.form(**questions))
-    if answers is None:
+            if name in preset_questions:
+                answer = safe_ask(get_preset_questions(group, name))
+                if answer is None:
+                    return
+                answers[name] = answer
+            else:
+                answer = safe_ask(
+                    questionary.text(f"Enter {name}", style=question_style, instruction="Leave blank to stop\n")
+                )
+                if answer is None:
+                    return
+                answers[name] = answer
+    if len(answers) == 0:
         return
     parts = ""
     annotations: None | list[str] = None
     for name, field in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
         value = answers.get(name, "")
-        if len(value) != 0 or answers[name] != " ":
+        if len(value) != 0 or value != " ":
             if name in "annotations":
-                annotations = [annotation for annotation in answers[name].split(";")]
-            elif name in tw_config["add_templates"]["date_fields"]:
-                date_str = dateparser.parse(answers[name])
-                if date_str is not None:
-                    date_str = date_str.strftime("%Y-%m-%dT%H:%M:%S")
-                    parts += " " + field.replace("%s", date_str)
-            else:
+                annotations = [annotation for annotation in answers[name]]
+            elif field["type"] == "date":
+                date_value = date_parser(answers[name])
+                if date_value is not None:
+                    date_str = date_value.strftime("%Y-%m-%dT%H:%M:%S")
+                    parts += " " + field["template"].replace("%s", date_str)
+                else:
+                    print('Cannot parse date "%s"' % answers[name])
+                    return
+            elif field["type"] == "list":
                 parts += " " + " ".join(
-                    field.replace("%s", item) if item != "" else "" for item in answers[name].split(";")
+                    field["template"].replace("%s", item) if item != "" else "" for item in answers[name]
                 )
+            else:
+                parts += " " + field["template"].replace("%s", value)
     command = tw_config["add_templates"]["data"][chosen_template]["command"].replace("%s", parts)
     confirm = safe_ask(questionary.confirm("Add task?", instruction=f"\n{command}\n", style=question_style))
     if confirm:
         uuid_compiled = re.compile(r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}")
         result = subprocess.run(
-            f"{group_mappings[group]} task rc.verbose=new-uuid {command}",
+            f"{group_mappings[group]} task rc.verbose=new-uuid add {command}",
             capture_output=True,
             text=True,
             shell=True,
         )
-        print(result.stdout)
+        if result.stderr:
+            print(result.stderr)
         uuid_match = uuid_compiled.search(result.stdout)
         if uuid_match:
             uuid = uuid_match.group()
             if annotations:
                 for annotate in annotations:
                     result = subprocess.run(
                         f"{group_mappings[group]} task {uuid} annotate {annotate}",
@@ -196,16 +295,27 @@
     return auto_completions
 
 
 @utils_commands.command("add", help="Add task, query, and template")
 def task_create(
     name: Annotated[str, typer.Argument(autocompletion=create_group_completion)] = "task",
     group: Annotated[str, typer.Option("--group", "-g", autocompletion=group_mappings_completion)] = "task",
+    repeat: Annotated[bool, typer.Option("--repeat", "-r")] = False,
 ):
-    create_groups[name]["func"](group)
+    repeating = True
+    while repeating:
+        create_groups[name]["func"](group)
+        if repeat:
+            confirm = safe_ask(questionary.confirm("Add more task?", style=question_style))
+            if confirm:
+                repeating = True
+            else:
+                repeating = False
+        else:
+            repeating = False
 
 
 def edit_template():
     templates = [
         questionary.Choice(title=template["name"], value=index, shortcut_key=str(index + 1))
         for index, template in enumerate(tw_config["add_templates"]["data"])
     ]
@@ -225,34 +335,52 @@
                 default=tw_config["add_templates"]["data"][chosen_template]["command"],
             ),
         )
     )
     if response is None:
         return
     template = {"name": response["name"], "command": response["command"], "fields": {}}
-    for name, field_template in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
+    for name, field in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
         response = safe_ask(
             questionary.form(
                 name=questionary.text("Enter field name", style=question_style, default=name),
-                template=questionary.text("Enter field template", style=question_style, default=field_template),
+                template=questionary.text("Enter field template", style=question_style, default=field["template"]),
+                type=questionary.rawselect(
+                    "Select type",
+                    choices=["text", "list", "date"],
+                    use_jk_keys=True,
+                    style=question_style,
+                    default=field["type"],
+                ),
             )
         )
         if response is None:
             return
-        template["fields"][response["name"]] = response["template"]
+        template["fields"][response["name"]] = {"template": response["template"], "type": response["type"]}
     field_name = "placeholder"
     while field_name != "":
         field_name = safe_ask(questionary.text("Enter field name", style=question_style))
         if field_name is None:
             return
         if field_name != "":
-            field_template = safe_ask(questionary.text("Enter field template", style=question_style))
-            if field_template is None:
+            field_form = safe_ask(
+                questionary.form(
+                    template=questionary.text("Enter field template", style=question_style),
+                    type=questionary.rawselect(
+                        "Select type of the field",
+                        choices=["text", "list", "date"],
+                        default="text",
+                        use_jk_keys=True,
+                        style=question_style,
+                    ),
+                )
+            )
+            if field_form is None:
                 return
-            template["fields"][field_name] = field_template
+            template["fields"][field_name] = {"template": field_form["template"], "type": field_form["type"]}
             print("To end enter nothing")
     tw_config["add_templates"]["data"][chosen_template] = template
     with open(config_file, "w") as f:
         f.write(json.dumps(tw_config))
 
 
 def edit_query():
@@ -374,22 +502,24 @@
     ]
     chosen_template = safe_ask(
         questionary.rawselect("Select template", choices=templates, use_jk_keys=True, style=question_style)
     )
     if chosen_template is None:
         return
     header = f'[bold]Template:[/bold] {tw_config["add_templates"]["data"][chosen_template]["name"]}'
-    field_header = f'{"-"*10}Fields{"-"*10}'
+    field_header = f'{"-"*24}Fields{"-"*24}'
     rprint(
         f"""{header}
 [bold]Command:[/bold] {tw_config["add_templates"]["data"][chosen_template]["command"]}
 [bold]{field_header}[/bold]"""
     )
-    for name, field_template in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
-        rprint(f"{name.ljust(16)} | {field_template}")
+    rprint(f"{'name'.ljust(16)} | {'template'.ljust(16)} | type")
+    rprint(f"{'-'*16} | {'-'*16} | {'-'*16}")
+    for name, field in tw_config["add_templates"]["data"][chosen_template]["fields"].items():
+        rprint(f"{name.ljust(16)} | {field['template'].ljust(16)} | {field['type']}")
 
 
 view_groups: dict[str, FunctionsGroup] = {
     "task": {"help": "View tasks based on saved queries", "func": view_task},
     "template": {"help": "View the details of the template", "func": view_template},
 }
 
@@ -509,21 +639,7 @@
         auto_completions.append((key, value["help"]))
     return auto_completions
 
 
 @utils_commands.command("delete", help="Delete task, query, template, and group")
 def task_delete(name: Annotated[str, typer.Argument(autocompletion=edit_group_completion)] = "template"):
     delete_groups[name]["func"]()
-
-
-def get_preset_questions(group):
-    projects = subprocess.run("task _projects", shell=True, capture_output=True).stdout.decode().split("\n")
-    tags = subprocess.run("task _tags", shell=True, capture_output=True).stdout.decode().split("\n")
-    return {
-        "project": questionary.autocomplete(
-            "Enter project", choices=projects, style=question_style, complete_style=CompleteStyle.MULTI_COLUMN
-        ),
-        "tags": questionary.autocomplete(
-            "Enter tags", choices=tags, style=question_style, complete_style=CompleteStyle.MULTI_COLUMN
-        ),
-    }
-
```

### Comparing `taskwarrior_flow-0.3.2/PKG-INFO` & `taskwarrior_flow-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskwarrior_flow
-Version: 0.3.2
+Version: 0.4.0
 Summary: Set of helpers for improving Taskwarrior workflow
 Author: Ben Trinh
 Author-email: huantrinh1802@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

