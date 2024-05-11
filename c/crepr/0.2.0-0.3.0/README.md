# Comparing `tmp/crepr-0.2.0.tar.gz` & `tmp/crepr-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crepr-0.2.0.tar", last modified: Mon Dec 11 19:34:20 2023, max compression
+gzip compressed data, was "crepr-0.3.0.tar", last modified: Sat May 11 12:14:30 2024, max compression
```

## Comparing `crepr-0.2.0.tar` & `crepr-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 19:34:20.756573 crepr-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-11 19:34:09.000000 crepr-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2023-12-11 19:34:20.756573 crepr-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2023-12-11 19:34:09.000000 crepr-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 19:34:20.752573 crepr-0.2.0/crepr/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-12-11 19:34:09.000000 crepr-0.2.0/crepr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-11 19:34:09.000000 crepr-0.2.0/crepr/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2023-12-11 19:34:09.000000 crepr-0.2.0/crepr/crepr.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 19:34:09.000000 crepr-0.2.0/crepr/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 19:34:20.752573 crepr-0.2.0/crepr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2023-12-11 19:34:20.000000 crepr-0.2.0/crepr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-12-11 19:34:20.000000 crepr-0.2.0/crepr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 19:34:20.000000 crepr-0.2.0/crepr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-11 19:34:20.000000 crepr-0.2.0/crepr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      434 2023-12-11 19:34:20.000000 crepr-0.2.0/crepr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-11 19:34:20.000000 crepr-0.2.0/crepr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2023-12-11 19:34:09.000000 crepr-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 19:34:20.756573 crepr-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:14:30.583850 crepr-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-11 12:14:22.000000 crepr-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-11 12:14:30.583850 crepr-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-11 12:14:22.000000 crepr-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:14:30.579850 crepr-0.3.0/crepr/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-11 12:14:22.000000 crepr-0.3.0/crepr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-11 12:14:22.000000 crepr-0.3.0/crepr/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-05-11 12:14:22.000000 crepr-0.3.0/crepr/crepr.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:14:22.000000 crepr-0.3.0/crepr/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:14:30.579850 crepr-0.3.0/crepr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-11 12:14:30.000000 crepr-0.3.0/crepr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-11 12:14:30.000000 crepr-0.3.0/crepr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:14:30.000000 crepr-0.3.0/crepr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-11 12:14:30.000000 crepr-0.3.0/crepr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-11 12:14:30.000000 crepr-0.3.0/crepr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 12:14:30.000000 crepr-0.3.0/crepr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-11 12:14:22.000000 crepr-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:14:30.583850 crepr-0.3.0/setup.cfg
```

### Comparing `crepr-0.2.0/LICENSE` & `crepr-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crepr-0.2.0/PKG-INFO` & `crepr-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepr
-Version: 0.2.0
+Version: 0.3.0
 Summary: Create a __repr__ for your python classes from the definition found in __init__
 Author-email: Christian Ledermann <christian.ledermann@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/cleder/crepr/
 Keywords: __repr__,cli,code generator,introspection
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -85,28 +85,68 @@
 ```bash
 pip install crepr
 ```
 
 ## Usage
 
 ```bash
-❯ crepr --help
-Usage: crepr [OPTIONS] FILE_PATH
-
-  Create a __repr__ method for each class of a python file.
-
-Arguments:
-  FILE_PATH  [required]
+❯ crepr  --help
+Usage: crepr [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --install-completion [bash|zsh|fish|powershell|pwsh]
                                   Install completion for the specified shell.
   --show-completion [bash|zsh|fish|powershell|pwsh]
                                   Show completion for the specified shell, to
-                                  copy it or customize
+                                  copy it or customize the installation.
+  --help                          Show this message and exit.
+
+Commands:
+  add     Add __repr__ to all classes in the source code.
+  remove  Remove the __repr__ method from all classes in the source code.
+```
+
+### Add
+
+The command `crepr add ...`  adds a `__repr__` method to all classes in this file, that
+have a `__init__` method with no positional only arguments.
+
+```bash
+❯ crepr add  --help
+Usage: crepr add [OPTIONS] FILES...
+
+  Add __repr__ to all classes in the source code.
+
+Arguments:
+  FILES...  The python source file(s)  [required]
+
+Options:
+  --kwarg-splat TEXT  The **kwarg splat  [default: ...]
+  --diff / --inline   Display the diff / Apply changes to the file(s)
+  --help              Show this message and exit.
+```
+
+### Remove
+
+The command `crepr remove ...` removes the `__repr__` methods from all classes that have
+an `__init__` method with no positional only arguments.
+
+
+```bash
+❯ crepr remove  --help
+Usage: crepr remove [OPTIONS] FILES...
+
+  Remove the __repr__ method from all classes in the source code.
+
+Arguments:
+  FILES...  The python source file(s)  [required]
+
+Options:
+  --diff / --inline  Display the diff / Apply changes to the file(s)
+  --help             Show this message and exit.
 ```
 
 ## Example
 
 Given the file `tests/classes/kw_only_test.py` with the contents:
 
 ```python
@@ -115,15 +155,15 @@
         self.name = name
         self.age = age
 ```
 
 The command:
 
 ```bash
-❯ crepr tests/kw_only_test.py
+❯ crepr add tests/classes/kw_only_test.py
 ```
 
 produces
 
 ```python
 class KwOnly:
     def __init__(self, name: str, *, age: int) -> None:
@@ -143,10 +183,16 @@
 ```python
 >>> from tests.classes.kw_only_test import KwOnly
 >>> kwo = KwOnly('Christian', age=25)
 >>> kwo
 tests.classes.kw_only_test.KwOnly(name='Christian', age=25, )
 ```
 
+Apply the changes to the file with:
+
+```bash
+❯ crepr add tests/classes/kw_only_test.py --inline
+```
+
 Give your representations some love.
 
 ❤️`.__repr__(self) -> str:`
```

### Comparing `crepr-0.2.0/README.md` & `crepr-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -29,28 +29,68 @@
 ```bash
 pip install crepr
 ```
 
 ## Usage
 
 ```bash
-❯ crepr --help
-Usage: crepr [OPTIONS] FILE_PATH
-
-  Create a __repr__ method for each class of a python file.
-
-Arguments:
-  FILE_PATH  [required]
+❯ crepr  --help
+Usage: crepr [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --install-completion [bash|zsh|fish|powershell|pwsh]
                                   Install completion for the specified shell.
   --show-completion [bash|zsh|fish|powershell|pwsh]
                                   Show completion for the specified shell, to
-                                  copy it or customize
+                                  copy it or customize the installation.
+  --help                          Show this message and exit.
+
+Commands:
+  add     Add __repr__ to all classes in the source code.
+  remove  Remove the __repr__ method from all classes in the source code.
+```
+
+### Add
+
+The command `crepr add ...`  adds a `__repr__` method to all classes in this file, that
+have a `__init__` method with no positional only arguments.
+
+```bash
+❯ crepr add  --help
+Usage: crepr add [OPTIONS] FILES...
+
+  Add __repr__ to all classes in the source code.
+
+Arguments:
+  FILES...  The python source file(s)  [required]
+
+Options:
+  --kwarg-splat TEXT  The **kwarg splat  [default: ...]
+  --diff / --inline   Display the diff / Apply changes to the file(s)
+  --help              Show this message and exit.
+```
+
+### Remove
+
+The command `crepr remove ...` removes the `__repr__` methods from all classes that have
+an `__init__` method with no positional only arguments.
+
+
+```bash
+❯ crepr remove  --help
+Usage: crepr remove [OPTIONS] FILES...
+
+  Remove the __repr__ method from all classes in the source code.
+
+Arguments:
+  FILES...  The python source file(s)  [required]
+
+Options:
+  --diff / --inline  Display the diff / Apply changes to the file(s)
+  --help             Show this message and exit.
 ```
 
 ## Example
 
 Given the file `tests/classes/kw_only_test.py` with the contents:
 
 ```python
@@ -59,15 +99,15 @@
         self.name = name
         self.age = age
 ```
 
 The command:
 
 ```bash
-❯ crepr tests/kw_only_test.py
+❯ crepr add tests/classes/kw_only_test.py
 ```
 
 produces
 
 ```python
 class KwOnly:
     def __init__(self, name: str, *, age: int) -> None:
@@ -87,10 +127,16 @@
 ```python
 >>> from tests.classes.kw_only_test import KwOnly
 >>> kwo = KwOnly('Christian', age=25)
 >>> kwo
 tests.classes.kw_only_test.KwOnly(name='Christian', age=25, )
 ```
 
+Apply the changes to the file with:
+
+```bash
+❯ crepr add tests/classes/kw_only_test.py --inline
+```
+
 Give your representations some love.
 
 ❤️`.__repr__(self) -> str:`
```

### Comparing `crepr-0.2.0/crepr.egg-info/PKG-INFO` & `crepr-0.3.0/crepr.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepr
-Version: 0.2.0
+Version: 0.3.0
 Summary: Create a __repr__ for your python classes from the definition found in __init__
 Author-email: Christian Ledermann <christian.ledermann@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/cleder/crepr/
 Keywords: __repr__,cli,code generator,introspection
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -85,28 +85,68 @@
 ```bash
 pip install crepr
 ```
 
 ## Usage
 
 ```bash
-❯ crepr --help
-Usage: crepr [OPTIONS] FILE_PATH
-
-  Create a __repr__ method for each class of a python file.
-
-Arguments:
-  FILE_PATH  [required]
+❯ crepr  --help
+Usage: crepr [OPTIONS] COMMAND [ARGS]...
 
 Options:
   --install-completion [bash|zsh|fish|powershell|pwsh]
                                   Install completion for the specified shell.
   --show-completion [bash|zsh|fish|powershell|pwsh]
                                   Show completion for the specified shell, to
-                                  copy it or customize
+                                  copy it or customize the installation.
+  --help                          Show this message and exit.
+
+Commands:
+  add     Add __repr__ to all classes in the source code.
+  remove  Remove the __repr__ method from all classes in the source code.
+```
+
+### Add
+
+The command `crepr add ...`  adds a `__repr__` method to all classes in this file, that
+have a `__init__` method with no positional only arguments.
+
+```bash
+❯ crepr add  --help
+Usage: crepr add [OPTIONS] FILES...
+
+  Add __repr__ to all classes in the source code.
+
+Arguments:
+  FILES...  The python source file(s)  [required]
+
+Options:
+  --kwarg-splat TEXT  The **kwarg splat  [default: ...]
+  --diff / --inline   Display the diff / Apply changes to the file(s)
+  --help              Show this message and exit.
+```
+
+### Remove
+
+The command `crepr remove ...` removes the `__repr__` methods from all classes that have
+an `__init__` method with no positional only arguments.
+
+
+```bash
+❯ crepr remove  --help
+Usage: crepr remove [OPTIONS] FILES...
+
+  Remove the __repr__ method from all classes in the source code.
+
+Arguments:
+  FILES...  The python source file(s)  [required]
+
+Options:
+  --diff / --inline  Display the diff / Apply changes to the file(s)
+  --help             Show this message and exit.
 ```
 
 ## Example
 
 Given the file `tests/classes/kw_only_test.py` with the contents:
 
 ```python
@@ -115,15 +155,15 @@
         self.name = name
         self.age = age
 ```
 
 The command:
 
 ```bash
-❯ crepr tests/kw_only_test.py
+❯ crepr add tests/classes/kw_only_test.py
 ```
 
 produces
 
 ```python
 class KwOnly:
     def __init__(self, name: str, *, age: int) -> None:
@@ -143,10 +183,16 @@
 ```python
 >>> from tests.classes.kw_only_test import KwOnly
 >>> kwo = KwOnly('Christian', age=25)
 >>> kwo
 tests.classes.kw_only_test.KwOnly(name='Christian', age=25, )
 ```
 
+Apply the changes to the file with:
+
+```bash
+❯ crepr add tests/classes/kw_only_test.py --inline
+```
+
 Give your representations some love.
 
 ❤️`.__repr__(self) -> str:`
```

### Comparing `crepr-0.2.0/pyproject.toml` & `crepr-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -98,14 +98,18 @@
 [tool.coverage.report]
 exclude_also = [
     "if __name__ == .__main__.:",
 ]
 
 [tool.coverage.run]
 branch = true
+omit = [
+    "tests/classes/*",
+    "tests/remove/*",
+]
 
 [tool.flake8]
 max_line_length = 88
 
 [tool.isort]
 force_single_line = true
 line_length = 88
@@ -134,14 +138,17 @@
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.ruff]
 fix = true
+target-version = "py312"
+
+[tool.ruff.lint]
 ignore = [
     "D203",
     "D213",
 ]
 select = [
     "A",
     "AIR",
@@ -198,20 +205,19 @@
     "TD",
     "TID",
     "TRY",
     "UP",
     "W",
     "YTT",
 ]
-target-version = "py312"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-single-line = true
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*.py" = [
     "PLR2004",
     "S101",
     "SLF001",
 ]
 
 [tool.setuptools.dynamic.version]
```

