# Comparing `tmp/pyproject_fmt-2.0.1.tar.gz` & `tmp/pyproject_fmt-2.0.2.tar.gz`

## Comparing `pyproject_fmt-2.0.1.tar` & `pyproject_fmt-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/tox.ini
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/src/pyproject_fmt/__init__.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/src/pyproject_fmt/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/src/pyproject_fmt/_version.py
--rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/src/pyproject_fmt/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/src/pyproject_fmt/py.typed
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/tests/test_cli.py
--rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/tests/test_main.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/tests/test_pyproject_toml_fmt.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/README.md
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/tox.ini
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/src/pyproject_fmt/__init__.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/src/pyproject_fmt/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/src/pyproject_fmt/_version.py
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/src/pyproject_fmt/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/src/pyproject_fmt/py.typed
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/tests/test_cli.py
+-rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/tests/test_main.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/tests/test_pyproject_toml_fmt.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/README.md
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.2/PKG-INFO
```

### Comparing `pyproject_fmt-2.0.1/tox.ini` & `pyproject_fmt-2.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.1/src/pyproject_fmt/__main__.py` & `pyproject_fmt-2.0.2/src/pyproject_fmt/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,22 +31,15 @@
         elif line.startswith("-"):
             yield f"{RED}{line}{RESET}"
         else:
             yield line
 
 
 def _handle_one(config: Config) -> bool:
-    formatted = format_toml(
-        config.toml,
-        column_width=config.column_width,
-        indent=config.indent,
-        keep_full_version=config.keep_full_version,
-        max_supported_python=config.max_supported_python,
-        min_supported_python=config.min_supported_python,
-    )
+    formatted = format_toml(config.toml, config.settings)
     before = config.toml
     changed = before != formatted
     if config.stdout:  # stdout just prints new format to stdout
         print(formatted, end="")  # noqa: T201
         return changed
 
     if before != formatted and not config.check:
```

### Comparing `pyproject_fmt-2.0.1/src/pyproject_fmt/cli.py` & `pyproject_fmt-2.0.2/src/pyproject_fmt/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     Namespace,
 )
 from dataclasses import dataclass
 from importlib.metadata import version
 from pathlib import Path
 from typing import Sequence
 
+from pyproject_fmt_rust import Settings
+
 if sys.version_info >= (3, 11):  # pragma: >=3.11 cover
     import tomllib
 else:  # pragma: <3.11 cover
     import tomli as tomllib
 
 
 class PyProjectFmtNamespace(Namespace):
@@ -38,20 +40,15 @@
 @dataclass(frozen=True)
 class Config:
     """Configuration flags for the formatting."""
 
     pyproject_toml: Path
     stdout: bool  # push to standard out
     check: bool  # check only
-
-    column_width: int  #: maximum column width
-    indent: int  #: indentation to apply
-    keep_full_version: bool  #: whether to keep full dependency versions
-    max_supported_python: tuple[int, int]  #: the maximum supported Python version
-    min_supported_python: tuple[int, int]  #: the minimum supported Python version
+    settings: Settings
 
     @property
     def toml(self) -> str:
         """:return: the toml files content"""
         return self.pyproject_toml.read_text(encoding="utf-8")
 
 
@@ -172,19 +169,21 @@
                     elif key == "min_supported_python":  # pragma: no branch
                         min_supported_python = _version_argument(entry)
         res.append(
             Config(
                 pyproject_toml=pyproject_toml,
                 stdout=opt.stdout,
                 check=opt.check,
-                column_width=column_width,
-                indent=indent,
-                keep_full_version=keep_full_version,
-                max_supported_python=max_supported_python,
-                min_supported_python=min_supported_python,
+                settings=Settings(
+                    column_width=column_width,
+                    indent=indent,
+                    keep_full_version=keep_full_version,
+                    max_supported_python=max_supported_python,
+                    min_supported_python=min_supported_python,
+                ),
             )
         )
 
     return res
 
 
 __all__ = [
```

### Comparing `pyproject_fmt-2.0.1/tests/test_cli.py` & `pyproject_fmt-2.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.1/tests/test_main.py` & `pyproject_fmt-2.0.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.1/LICENSE.txt` & `pyproject_fmt-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.1/README.md` & `pyproject_fmt-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.1/pyproject.toml` & `pyproject_fmt-2.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 description = "Format your pyproject.toml file"
 readme = "README.md"
 keywords = [
   "format",
   "pyproject",
 ]
 license.file = "LICENSE.txt"
-authors = [{ name = "Bernat Gabor", email = "gaborjbernat@gmail.com" }]
+authors = [
+  { name = "Bernat Gabor", email = "gaborjbernat@gmail.com" },
+]
 requires-python = ">=3.8"
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
@@ -27,15 +29,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "pyproject-fmt-rust==1",
+  "pyproject-fmt-rust==1.0.1",
 ]
 optional-dependencies.docs = [
   "furo>=2024.5.6",
   "sphinx>=7.3.7",
   "sphinx-argparse-cli>=1.15",
   "sphinx-autodoc-typehints>=2.1",
   "sphinx-copybutton>=0.5.2",
@@ -49,57 +51,71 @@
 urls."Bug Tracker" = "https://github.com/tox-dev/pyproject-fmt/issues"
 urls."Changelog" = "https://github.com/tox-dev/pyproject-fmt/releases"
 urls.Documentation = "https://github.com/tox-dev/pyproject-fmt/"
 urls."Source Code" = "https://github.com/tox-dev/pyproject-fmt"
 scripts.pyproject-fmt = "pyproject_fmt.__main__:run"
 
 [tool.hatch]
-build.dev-mode-dirs = ["src"]
+build.dev-mode-dirs = [
+  "src",
+]
 build.hooks.vcs.version-file = "src/pyproject_fmt/_version.py"
-build.targets.sdist.include = ["/src", "/tests","tox.ini"]
+build.targets.sdist.include = [
+  "/src",
+  "/tests",
+  "tox.ini",
+]
 version.source = "vcs"
 
 [tool.ruff]
 line-length = 120
 target-version = "py38"
-lint.isort = { known-first-party = ["pyproject_fmt"], required-imports = ["from __future__ import annotations"] }
-lint.select = ["ALL"]
+lint.isort = { known-first-party = [
+  "pyproject_fmt",
+], required-imports = [
+  "from __future__ import annotations",
+] }
+lint.select = [
+  "ALL",
+]
 lint.ignore = [
-  "ANN101",  # no type annotation for self
-  "ANN401",  # allow Any as type annotation
-  "D203",  # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
-  "D212",  # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
-  "S104",  # Possible binding to all interface
+  "ANN101", # no type annotation for self
+  "ANN401", # allow Any as type annotation
+  "D203",   # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
+  "D212",   # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
+  "S104",   # Possible binding to all interface
   "COM812", # Conflict with formatter
   "ISC001", # Conflict with formatter
   "CPY",    # No copyright statements
 ]
 lint.preview = true
 format.preview = true
 format.docstring-code-format = true
 format.docstring-code-line-length = 100
 [tool.ruff.lint.per-file-ignores]
 "tests/**/*.py" = [
-  "S101",  # asserts allowed in tests...
-  "FBT",  # don"t care about booleans as positional arguments in tests
-  "INP001", # no implicit namespace
-  "D",  # don"t care about documentation in tests
-  "S603",  # `subprocess` call: check for execution of untrusted input
-  "PLR2004",  # Magic value used in comparison, consider replacing with a constant variable
+  "S101",    # asserts allowed in tests...
+  "FBT",     # don"t care about booleans as positional arguments in tests
+  "INP001",  # no implicit namespace
+  "D",       # don"t care about documentation in tests
+  "S603",    # `subprocess` call: check for execution of untrusted input
+  "PLR2004", # Magic value used in comparison, consider replacing with a constant variable
   "PLR0913", # any number of arguments in tests
   "PLR0917", # any number of arguments in tests
   "PLC2701", # private import
 ]
 
 [tool.codespell]
 builtin = "clear,usage,en-GB_to_en-US"
 count = true
 
 [tool.pytest]
-ini_options.testpaths = ["tests"]
+ini_options.testpaths = [
+  "tests",
+]
 
 [tool.coverage]
 html.show_contexts = true
 html.skip_covered = false
 paths.source = [
   "src",
   ".tox/*/.venv/lib/*/site-packages",
@@ -107,12 +123,14 @@
   ".tox/*/lib/*/site-packages",
   ".tox\\*\\Lib\\site-packages",
   "**/src",
   "**\\src",
 ]
 report.fail_under = 100
 run.parallel = true
-run.plugins = ["covdefaults"]
+run.plugins = [
+  "covdefaults",
+]
 
 [tool.mypy]
 show_error_codes = true
 strict = true
```

### Comparing `pyproject_fmt-2.0.1/PKG-INFO` & `pyproject_fmt-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-fmt
-Version: 2.0.1
+Version: 2.0.2
 Summary: Format your pyproject.toml file
 Project-URL: Bug Tracker, https://github.com/tox-dev/pyproject-fmt/issues
 Project-URL: Changelog, https://github.com/tox-dev/pyproject-fmt/releases
 Project-URL: Documentation, https://github.com/tox-dev/pyproject-fmt/
 Project-URL: Source Code, https://github.com/tox-dev/pyproject-fmt
 Author-email: Bernat Gabor <gaborjbernat@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a
@@ -33,15 +33,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: pyproject-fmt-rust==1
+Requires-Dist: pyproject-fmt-rust==1.0.1
 Provides-Extra: docs
 Requires-Dist: furo>=2024.5.6; extra == 'docs'
 Requires-Dist: sphinx-argparse-cli>=1.15; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints>=2.1; extra == 'docs'
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
 Requires-Dist: sphinx>=7.3.7; extra == 'docs'
 Provides-Extra: test
```

