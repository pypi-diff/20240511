# Comparing `tmp/makejinja-2.5.0.tar.gz` & `tmp/makejinja-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makejinja-2.5.0.tar", max compression
+gzip compressed data, was "makejinja-2.6.0.tar", max compression
```

## Comparing `makejinja-2.5.0.tar` & `makejinja-2.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2024-01-21 21:25:48.849513 makejinja-2.5.0/LICENSE
--rw-r--r--   0        0        0     3437 2024-01-21 21:25:48.849513 makejinja-2.5.0/README.md
--rw-r--r--   0        0        0      412 2024-01-21 21:25:48.849513 makejinja-2.5.0/makejinja/__init__.py
--rw-r--r--   0        0        0       48 2024-01-21 21:25:48.849513 makejinja-2.5.0/makejinja/__main__.py
--rw-r--r--   0        0        0    12716 2024-01-21 21:25:48.849513 makejinja-2.5.0/makejinja/app.py
--rw-r--r--   0        0        0     1449 2024-01-21 21:25:48.849513 makejinja-2.5.0/makejinja/cli.py
--rw-r--r--   0        0        0    15440 2024-01-21 21:25:48.849513 makejinja-2.5.0/makejinja/config.py
--rw-r--r--   0        0        0     1368 2024-01-21 21:25:48.849513 makejinja-2.5.0/makejinja/plugin.py
--rw-r--r--   0        0        0        0 2024-01-21 21:25:48.849513 makejinja-2.5.0/makejinja/py.typed
--rw-r--r--   0        0        0     2082 2024-01-21 21:26:43.276829 makejinja-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     5231 1970-01-01 00:00:00.000000 makejinja-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-11 09:02:42.894189 makejinja-2.6.0/LICENSE
+-rw-r--r--   0        0        0     3437 2024-05-11 09:02:42.894189 makejinja-2.6.0/README.md
+-rw-r--r--   0        0        0      412 2024-05-11 09:02:42.894189 makejinja-2.6.0/makejinja/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-11 09:02:42.894189 makejinja-2.6.0/makejinja/__main__.py
+-rw-r--r--   0        0        0    12818 2024-05-11 09:02:42.894189 makejinja-2.6.0/makejinja/app.py
+-rw-r--r--   0        0        0     1449 2024-05-11 09:02:42.894189 makejinja-2.6.0/makejinja/cli.py
+-rw-r--r--   0        0        0    15517 2024-05-11 09:02:42.894189 makejinja-2.6.0/makejinja/config.py
+-rw-r--r--   0        0        0     1368 2024-05-11 09:02:42.894189 makejinja-2.6.0/makejinja/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-11 09:02:42.894189 makejinja-2.6.0/makejinja/py.typed
+-rw-r--r--   0        0        0     2086 2024-05-11 09:04:00.506493 makejinja-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5231 1970-01-01 00:00:00.000000 makejinja-2.6.0/PKG-INFO
```

### Comparing `makejinja-2.5.0/LICENSE` & `makejinja-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `makejinja-2.5.0/README.md` & `makejinja-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `makejinja-2.5.0/makejinja/app.py` & `makejinja-2.6.0/makejinja/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,16 @@
     plugin_path_filters: abc.Sequence[abc.Callable[[Path], bool]],
 ) -> None:
     input_paths = (
         input_path
         for include_pattern in config.include_patterns
         for input_path in sorted(user_input_path.glob(include_pattern))
     )
+    # If the user provided a Jinja suffix, enforce it
+    enforce_jinja_suffix = bool(config.jinja_suffix)
 
     for input_path in input_paths:
         relative_path = input_path.relative_to(user_input_path)
         output_path = generate_output_path(config, relative_path)
 
         exclude_pattern_match = any(
             input_path.match(x) for x in config.exclude_patterns
@@ -177,15 +179,15 @@
         elif input_path.is_file() and output_path not in rendered_files:
             render_file(
                 input_path,
                 str(relative_path),
                 output_path,
                 config,
                 env,
-                enforce_jinja_suffix=True,
+                enforce_jinja_suffix,
             )
             rendered_files[output_path] = input_path
 
         elif input_path.is_dir() and output_path not in rendered_dirs:
             render_dir(input_path, output_path, config)
             rendered_dirs[output_path] = input_path
```

### Comparing `makejinja-2.5.0/makejinja/cli.py` & `makejinja-2.6.0/makejinja/cli.py`

 * *Files identical despite different names*

### Comparing `makejinja-2.5.0/makejinja/config.py` & `makejinja-2.6.0/makejinja/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,21 +203,22 @@
         click={"param_decls": ("--exclude-pattern", "--exclude", "-E")},
         help="""
             Glob patterns pattern to exclude files matched.
             Applied against files discovered through `include_patterns`.
             Multiple can be provided.
         """,
     )
-    jinja_suffix: str = ts.option(
+    jinja_suffix: str | None = ts.option(
         default=".jinja",
         help="""
             File ending of Jinja template files.
             All files with this suffix in `inputs` matched by `pattern` are passed to the Jinja renderer.
             This suffix is not enforced for individual files passed to `inputs`.
             **Note:** Should be provided *with* the leading dot.
+            If empty, all files are considered to be Jinja templates.
         """,
     )
     keep_jinja_suffix: bool = ts.option(
         default=False,
         click={"param_decls": "--keep-jinja-suffix"},
         help="""
             Decide whether the specified `jinja-suffix` is removed from the file name after rendering.
```

### Comparing `makejinja-2.5.0/makejinja/plugin.py` & `makejinja-2.6.0/makejinja/plugin.py`

 * *Files identical despite different names*

### Comparing `makejinja-2.5.0/pyproject.toml` & `makejinja-2.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makejinja"
-version = "2.5.0"
+version = "2.6.0"
 description = "Generate entire directory structures using Jinja templates with support for external data and custom plugins."
 authors = ["Mirko Lenz <mirko@mirkolenz.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mirkolenz/makejinja"
 homepage = "https://mirkolenz.github.io/makejinja/"
 documentation = "https://mirkolenz.github.io/makejinja/makejinja/cli.html"
@@ -53,16 +53,16 @@
     "attrs",
     "cattrs",
     "click",
 ] }
 immutables = "^0.20"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4"
-pytest-cov = "^4.1"
+pytest = "^8.0.0"
+pytest-cov = "^5.0.0"
 
 [tool.poetry.group.docs.dependencies]
 pdoc = "^14.1"
 
 [tool.pytest.ini_options]
 addopts = "--cov makejinja --cov-report term-missing"
```

### Comparing `makejinja-2.5.0/PKG-INFO` & `makejinja-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makejinja
-Version: 2.5.0
+Version: 2.6.0
 Summary: Generate entire directory structures using Jinja templates with support for external data and custom plugins.
 Home-page: https://mirkolenz.github.io/makejinja/
 License: MIT
 Keywords: jinja2,home-assistant,hassio,dashboard,lovelace,template,generator,cli,tool,library
 Author: Mirko Lenz
 Author-email: mirko@mirkolenz.com
 Requires-Python: >=3.11,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: makejinja Version: 2.5.0 Summary: Generate entire
+Metadata-Version: 2.1 Name: makejinja Version: 2.6.0 Summary: Generate entire
 directory structures using Jinja templates with support for external data and
 custom plugins. Home-page: https://mirkolenz.github.io/makejinja/ License: MIT
 Keywords: jinja2,home-
 assistant,hassio,dashboard,lovelace,template,generator,cli,tool,library Author:
 Mirko Lenz Author-email: mirko@mirkolenz.com Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Framework :: Pytest Classifier: Intended Audience ::
```

