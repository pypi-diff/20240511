# Comparing `tmp/pyaction-0.6.0.tar.gz` & `tmp/pyaction-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaction-0.6.0.tar", last modified: Tue Apr 30 20:30:34 2024, max compression
+gzip compressed data, was "pyaction-0.6.1.tar", last modified: Sat May 11 17:16:23 2024, max compression
```

## Comparing `pyaction-0.6.0.tar` & `pyaction-0.6.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.593747 pyaction-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-30 20:30:30.000000 pyaction-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 20:30:30.000000 pyaction-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-30 20:30:34.593747 pyaction-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-30 20:30:30.000000 pyaction-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.589748 pyaction-0.6.0/pyaction/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.589748 pyaction-0.6.0/pyaction/issues/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/issues/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/issues/rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.589748 pyaction-0.6.0/pyaction/template/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/copier.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.589748 pyaction-0.6.0/pyaction/template/{{action_slug}}/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/Dockerfile.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/README.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/action.yml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.585747 pyaction-0.6.0/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.589748 pyaction-0.6.0/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyaction/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 20:30:34.589748 pyaction-0.6.0/pyaction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-30 20:30:34.000000 pyaction-0.6.0/pyaction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-30 20:30:34.000000 pyaction-0.6.0/pyaction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 20:30:34.000000 pyaction-0.6.0/pyaction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-30 20:30:34.000000 pyaction-0.6.0/pyaction.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-30 20:30:34.000000 pyaction-0.6.0/pyaction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 20:30:34.000000 pyaction-0.6.0/pyaction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-30 20:30:30.000000 pyaction-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 20:30:34.593747 pyaction-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.652339 pyaction-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-11 17:16:19.000000 pyaction-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-11 17:16:19.000000 pyaction-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-11 17:16:23.652339 pyaction-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-11 17:16:19.000000 pyaction-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.648339 pyaction-0.6.1/pyaction/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.652339 pyaction-0.6.1/pyaction/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/issues/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/issues/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.652339 pyaction-0.6.1/pyaction/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/copier.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.652339 pyaction-0.6.1/pyaction/template/{{action_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/Dockerfile.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/README.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/action.yml.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.648339 pyaction-0.6.1/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.652339 pyaction-0.6.1/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/template/{{action_slug}}/{% if include_cicd_testing %}.github{% endif %}/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyaction/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:16:23.652339 pyaction-0.6.1/pyaction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-11 17:16:23.000000 pyaction-0.6.1/pyaction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-11 17:16:23.000000 pyaction-0.6.1/pyaction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 17:16:23.000000 pyaction-0.6.1/pyaction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-11 17:16:23.000000 pyaction-0.6.1/pyaction.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-11 17:16:23.000000 pyaction-0.6.1/pyaction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 17:16:23.000000 pyaction-0.6.1/pyaction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-11 17:16:19.000000 pyaction-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 17:16:23.652339 pyaction-0.6.1/setup.cfg
```

### Comparing `pyaction-0.6.0/LICENSE` & `pyaction-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.0/PKG-INFO` & `pyaction-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.6.0
+Version: 0.6.1
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,14 +54,30 @@
 Requires-Dist: cairosvg; extra == "docs"
 Requires-Dist: pillow; extra == "docs"
 
 ## PyAction ![Version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) ![Python Versions](https://img.shields.io/pypi/pyversions/pyaction?logo=python&logoColor=949DA5&label=Python&labelColor=2A3035) [![codecov](https://codecov.io/gh/lnxpy/pyaction/graph/badge.svg?token=59XAONX5S1)](https://codecov.io/gh/lnxpy/pyaction) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![Docs CI](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
 
 PyAction helps you to develop [GitHub Actions](https://docs.github.com/en/actions) using Python. It's delivered as an installable package with the ability to test the action locally before any deployment.
 
+```python
+from pyaction import PyAction
+
+
+workflow = PyAction.workflow()
+
+
+@workflow.action()
+def greetings_action(name: str, age: int) -> None:
+    workflow.write(
+        {
+            "phrase": f"Hello {name}. You are {age}!"
+        }
+    )
+```
+
 Check out the [official docs](https://pyaction.imsadra.me) for more detailed information. There is also a [Quickstart](https://pyaction.imsadra.me/quickstart) demo tutorial that walks you through a simple hello-world action.
 
 ### Requirements
 - Python >= 3.8
 - pip
 
 ### Installation
```

### Comparing `pyaction-0.6.0/README.md` & `pyaction-0.6.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 ## PyAction ![Version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) ![Python Versions](https://img.shields.io/pypi/pyversions/pyaction?logo=python&logoColor=949DA5&label=Python&labelColor=2A3035) [![codecov](https://codecov.io/gh/lnxpy/pyaction/graph/badge.svg?token=59XAONX5S1)](https://codecov.io/gh/lnxpy/pyaction) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![Docs CI](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
 
 PyAction helps you to develop [GitHub Actions](https://docs.github.com/en/actions) using Python. It's delivered as an installable package with the ability to test the action locally before any deployment.
 
+```python
+from pyaction import PyAction
+
+
+workflow = PyAction.workflow()
+
+
+@workflow.action()
+def greetings_action(name: str, age: int) -> None:
+    workflow.write(
+        {
+            "phrase": f"Hello {name}. You are {age}!"
+        }
+    )
+```
+
 Check out the [official docs](https://pyaction.imsadra.me) for more detailed information. There is also a [Quickstart](https://pyaction.imsadra.me/quickstart) demo tutorial that walks you through a simple hello-world action.
 
 ### Requirements
 - Python >= 3.8
 - pip
 
 ### Installation
```

### Comparing `pyaction-0.6.0/pyaction/cli.py` & `pyaction-0.6.1/pyaction/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 @click.group()
 def cli():
     """Create GitHub Actions Using Python"""
     pass
 
 
 @cli.command("init", help="creates a basic action template (recommended for starting)")
-@click.argument("path", default=".")
-def init(path: str = ".") -> None:
-    run_copy(TEMPLATE_PATH, path)
+def init() -> None:
+    run_copy(TEMPLATE_PATH)
 
 
 @cli.command("run", help="uses .env to run the action locally")
 def run() -> None:
     if not os.path.isfile(".env"):
         raise FileNotFoundError(
             "Make sure you have the `.env` file inside the root path of your action directory."
```

### Comparing `pyaction-0.6.0/pyaction/consts.py` & `pyaction-0.6.1/pyaction/consts.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.0/pyaction/io.py` & `pyaction-0.6.1/pyaction/io.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,26 +5,19 @@
 from io import TextIOWrapper
 
 from pyaction.consts import GITHUB_OUTPUT
 from pyaction.exceptions import WorkflowParameterNotFound
 
 
 def write(context: dict[str, str], stream: str | TextIOWrapper = GITHUB_OUTPUT) -> None:
-    """writes the key(s) (as variables) and value(s) (as values) to the output stream
+    """writes the key(s) (as variables) and value(s) (as values) into the output stream
 
     Args:
         context (dict[str, str]): variables and values
-        stream (str, TextIOWrapper): output stream (set to STDOUT locally and `GITHUB_OUTPUT` on production)
-
-    Examples:
-        In your action, use this function like:
-
-        >>> write({"name": "John", "age": 20, ...})
-
-        `name` and `age` are the variables and `John` and `20` are the values.
+        stream (str, TextIOWrapper): output stream (set to STDOUT locally, but `GITHUB_OUTPUT` on production)
     """
 
     with nullcontext(stream) if isinstance(stream, TextIOWrapper) else open(
         stream, "w+"
     ) as streamline:
         for var, val in context.items():
             streamline.write(f"{var}={val}\r\n")
```

### Comparing `pyaction-0.6.0/pyaction/issues/connector.py` & `pyaction-0.6.1/pyaction/issues/connector.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.0/pyaction/issues/rendering.py` & `pyaction-0.6.1/pyaction/issues/rendering.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
         Args:
             context (str): issue body
         """
         self.context = context
 
     def to_dict(self) -> dict[str, str]:
-        """convering the issue body to dictionary
+        """converting the issue body to dictionary
 
         Returns:
             Dict[str, str]: issue body in form of dictionary
         """
 
         pattern = re.compile("### ([^\n]+)\n\n([^#]+)")
         matches = pattern.findall(self.context)
```

### Comparing `pyaction-0.6.0/pyaction/logger.py` & `pyaction-0.6.1/pyaction/logger.py`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.0/pyaction/template/copier.yml` & `pyaction-0.6.1/pyaction/template/copier.yml`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.0/pyaction/utils.py` & `pyaction-0.6.1/pyaction/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         NotAnnotated: if there is param(s) not annotated
     """
 
     signature = inspect.signature(func)
     for param_name, param in signature.parameters.items():
         if param.default != inspect.Parameter.empty:
             logger.warning(
-                f"Prameter `{param_name}` in the action function `{func.__name__}` has gotten the default value `{param.default}` which has no effect. "
+                f"Parameter `{param_name}` in the action function `{func.__name__}` has gotten the default value `{param.default}` which has no effect. "
                 "Set the default value(s) inside the `action.yml` instead."
             )
 
         if param.annotation == inspect.Parameter.empty:
             raise NotAnnotated(
                 f"Parameter `{param_name}` in the action function `{func.__name__}` is not annotated."
             )
```

### Comparing `pyaction-0.6.0/pyaction/workflow.py` & `pyaction-0.6.1/pyaction/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,50 +4,49 @@
 
 from pyaction import io
 from pyaction.utils import check_parameters
 
 
 class PyAction:
     @staticmethod
-    def action(func: Callable):
+    def action() -> Callable:
         """action decorator
 
-        Args:
-            func (Callable): action function
-
         Examples:
-            In the `main.py` file, use this decorator to define your action like this:
+            use this action decorator in the following way:
 
             >>> workflow = PyAction()
-            >>> @workflow.action
-            >>> def my_action(...): ...
+            >>> @workflow.action()
+            >>> def your_action(): ...
 
-            Define your action input parameters as the annotated action function arguments.
+            you should define your action input parameters as the arguments of your function..
 
-            >>> ...
-            >>> def my_action(name: str, age: int): ...
-        """
+            >>> @workflow.action()
+            >>> def your_action(name: str, age: int, is_student: bool): ...
 
-        check_parameters(func)
+        Returns:
+            Callable: the wrapper action
+        """
 
-        def wrapper():
+        def wrapper(func: Callable):
+            check_parameters(func)
             params = {
                 key: (type_, io.read(key))
                 for key, type_ in get_type_hints(func).items()
                 if key != "return"
             }
 
             retyped_params = {}
 
             for key, item in params.items():
                 retyped_params[key] = TypeAdapter(item[0]).validate_python(item[1])
 
             return func(**retyped_params)
 
-        return wrapper()
+        return wrapper
 
     @staticmethod
     def write(context: Dict[str, str]) -> None:
         """writes the `context` env var(s) into the streamline
 
         Args:
             context (Dict[str, str]): variables and values
```

### Comparing `pyaction-0.6.0/pyaction.egg-info/PKG-INFO` & `pyaction-0.6.1/pyaction.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaction
-Version: 0.6.0
+Version: 0.6.1
 Summary: Create GitHub Actions using Python
 Author-email: Sadra Yahyapour <lnxpylnxpy@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Sadra Yahyapour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,14 +54,30 @@
 Requires-Dist: cairosvg; extra == "docs"
 Requires-Dist: pillow; extra == "docs"
 
 ## PyAction ![Version)](https://img.shields.io/github/v/tag/lnxpy/pyaction?label=Version) ![Python Versions](https://img.shields.io/pypi/pyversions/pyaction?logo=python&logoColor=949DA5&label=Python&labelColor=2A3035) [![codecov](https://codecov.io/gh/lnxpy/pyaction/graph/badge.svg?token=59XAONX5S1)](https://codecov.io/gh/lnxpy/pyaction) [![Package Testing](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml/badge.svg)](https://github.com/lnxpy/pyaction/actions/workflows/testing.yml) [![Docs CI](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/lnxpy/pyaction/actions/workflows/docs.yml)
 
 PyAction helps you to develop [GitHub Actions](https://docs.github.com/en/actions) using Python. It's delivered as an installable package with the ability to test the action locally before any deployment.
 
+```python
+from pyaction import PyAction
+
+
+workflow = PyAction.workflow()
+
+
+@workflow.action()
+def greetings_action(name: str, age: int) -> None:
+    workflow.write(
+        {
+            "phrase": f"Hello {name}. You are {age}!"
+        }
+    )
+```
+
 Check out the [official docs](https://pyaction.imsadra.me) for more detailed information. There is also a [Quickstart](https://pyaction.imsadra.me/quickstart) demo tutorial that walks you through a simple hello-world action.
 
 ### Requirements
 - Python >= 3.8
 - pip
 
 ### Installation
```

### Comparing `pyaction-0.6.0/pyaction.egg-info/SOURCES.txt` & `pyaction-0.6.1/pyaction.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyaction-0.6.0/pyproject.toml` & `pyaction-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyaction"
-version = "0.6.0"
+version = "0.6.1"
 description = "Create GitHub Actions using Python"
 authors = [{ name = "Sadra Yahyapour", email = "lnxpylnxpy@gmail.com" }]
 requires-python = ">=3.8"
 dependencies = [
     "copier >= 9.2",
     "click >= 8.1",
     "pydantic >= 2.7.0",
@@ -39,15 +39,15 @@
 docs = ["mkdocs-material", "cairosvg", "pillow"]
 
 [project.urls]
 Documentation = "https://pyaction.imsadra.me"
 Repository = "https://github.com/lnxpy/pyaction"
 
 [tool.bumpversion]
-current_version = "0.6.0"
+current_version = "0.6.1"
 commit = "true"
 tag = "true"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 
 [[tool.bumpversion.files]]
```

