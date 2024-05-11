# Comparing `tmp/pyproject_fmt-2.0.0.tar.gz` & `tmp/pyproject_fmt-2.0.1.tar.gz`

## Comparing `pyproject_fmt-2.0.0.tar` & `pyproject_fmt-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/tox.ini
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/src/pyproject_fmt/__init__.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/src/pyproject_fmt/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/src/pyproject_fmt/_version.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/src/pyproject_fmt/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/src/pyproject_fmt/py.typed
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/tests/test_main.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/tests/test_pyproject_toml_fmt.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/README.md
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/tox.ini
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/src/pyproject_fmt/__init__.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/src/pyproject_fmt/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/src/pyproject_fmt/_version.py
+-rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/src/pyproject_fmt/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/src/pyproject_fmt/py.typed
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/tests/test_cli.py
+-rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/tests/test_main.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/tests/test_pyproject_toml_fmt.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/README.md
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.1/PKG-INFO
```

### Comparing `pyproject_fmt-2.0.0/tox.ini` & `pyproject_fmt-2.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.0/src/pyproject_fmt/__main__.py` & `pyproject_fmt-2.0.1/src/pyproject_fmt/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 
 def _handle_one(config: Config) -> bool:
     formatted = format_toml(
         config.toml,
         column_width=config.column_width,
         indent=config.indent,
         keep_full_version=config.keep_full_version,
-        max_supported_python=(config.max_supported_python.major, config.max_supported_python.minor),
-        min_supported_python=(config.min_supported_python.major, config.min_supported_python.minor),
+        max_supported_python=config.max_supported_python,
+        min_supported_python=config.min_supported_python,
     )
     before = config.toml
     changed = before != formatted
     if config.stdout:  # stdout just prints new format to stdout
         print(formatted, end="")  # noqa: T201
         return changed
```

### Comparing `pyproject_fmt-2.0.0/src/pyproject_fmt/cli.py` & `pyproject_fmt-2.0.1/src/pyproject_fmt/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 """CLI interface parser."""
 
 from __future__ import annotations
 
-import sys
-from dataclasses import dataclass
-
-if sys.version_info >= (3, 11):  # pragma: >=3.11 cover
-    import tomllib
-else:  # pragma: <3.11 cover
-    import tomli as tomllib
-
 import os
+import sys
 from argparse import (
     ArgumentDefaultsHelpFormatter,
     ArgumentParser,
     ArgumentTypeError,
     Namespace,
 )
+from dataclasses import dataclass
 from importlib.metadata import version
 from pathlib import Path
 from typing import Sequence
 
-from packaging.version import Version
+if sys.version_info >= (3, 11):  # pragma: >=3.11 cover
+    import tomllib
+else:  # pragma: <3.11 cover
+    import tomli as tomllib
 
 
 class PyProjectFmtNamespace(Namespace):
     """Options for pyproject-fmt tool."""
 
     inputs: list[Path]
     stdout: bool
     check: bool
 
     column_width: int
     indent: int
     keep_full_version: bool
-    max_supported_python: Version
-    min_supported_python: Version
+    max_supported_python: tuple[int, int]
+    min_supported_python: tuple[int, int]
 
 
 @dataclass(frozen=True)
 class Config:
     """Configuration flags for the formatting."""
 
     pyproject_toml: Path
     stdout: bool  # push to standard out
     check: bool  # check only
 
     column_width: int  #: maximum column width
     indent: int  #: indentation to apply
     keep_full_version: bool  #: whether to keep full dependency versions
-    max_supported_python: Version  #: the maximum supported Python version
-    min_supported_python: Version  #: the minimum supported Python version
+    max_supported_python: tuple[int, int]  #: the maximum supported Python version
+    min_supported_python: tuple[int, int]  #: the minimum supported Python version
 
     @property
     def toml(self) -> str:
         """:return: the toml files content"""
         return self.pyproject_toml.read_text(encoding="utf-8")
 
 
@@ -79,14 +76,26 @@
         raise ArgumentTypeError(msg)
     if not os.access(path, os.W_OK):
         msg = "cannot write path"
         raise ArgumentTypeError(msg)
     return path
 
 
+def _version_argument(got: str) -> tuple[int, int]:
+    parts = got.split(".")
+    if len(parts) != 2:  # noqa: PLR2004
+        msg = f"invalid version: {got}, must be e.g. 3.12"
+        raise ArgumentTypeError(msg)
+    try:
+        return int(parts[0]), int(parts[1])
+    except ValueError as exc:
+        msg = f"invalid version: {got} due {exc!r}, must be e.g. 3.12"
+        raise ArgumentTypeError(msg) from exc
+
+
 def _build_cli() -> ArgumentParser:
     parser = ArgumentParser(
         formatter_class=ArgumentDefaultsHelpFormatter,
         prog="pyproject-fmt",
     )
     parser.add_argument(
         "-V",
@@ -112,22 +121,22 @@
         "--indent",
         type=int,
         default=2,
         help="number of spaces to indent",
     )
     parser.add_argument(
         "--min-supported-python",
-        type=Version,
-        default="3.8",
+        type=_version_argument,
+        default=(3, 8),
         help="latest Python version the project supports (e.g. 3.8)",
     )
     parser.add_argument(
         "--max-supported-python",
-        type=Version,
-        default="3.12",
+        type=_version_argument,
+        default=(3, 12),
         help="latest Python version the project supports (e.g. 3.13)",
     )
     msg = "pyproject.toml file(s) to format"
     parser.add_argument("inputs", nargs="+", type=pyproject_toml_path_creator, help=msg)
     return parser
 
 
@@ -155,17 +164,17 @@
                     if key == "column_width":
                         column_width = int(entry)
                     elif key == "indent":
                         indent = int(entry)
                     elif key == "keep_full_version":
                         keep_full_version = bool(entry)
                     elif key == "max_supported_python":
-                        max_supported_python = Version(entry)
+                        max_supported_python = _version_argument(entry)
                     elif key == "min_supported_python":  # pragma: no branch
-                        min_supported_python = Version(entry)
+                        min_supported_python = _version_argument(entry)
         res.append(
             Config(
                 pyproject_toml=pyproject_toml,
                 stdout=opt.stdout,
                 check=opt.check,
                 column_width=column_width,
                 indent=indent,
```

### Comparing `pyproject_fmt-2.0.0/tests/test_cli.py` & `pyproject_fmt-2.0.1/tests/test_cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,39 @@
     with pytest.raises(SystemExit) as context:
         cli_args(["--version"])
     assert context.value.code == 0
     out, _err = capsys.readouterr()
     assert out == f"pyproject-fmt ({version('pyproject-fmt')})\n"
 
 
+def test_cli_invalid_version(capsys: pytest.CaptureFixture[str], tmp_path: Path) -> None:
+    path = tmp_path / "pyproject.toml"
+    path.write_text("")
+    with pytest.raises(SystemExit) as context:
+        cli_args([str(path), "--max-supported-python", "3"])
+    assert context.value.code == 2
+    out, err = capsys.readouterr()
+    assert not out
+    assert "error: argument --max-supported-python: invalid version: 3, must be e.g. 3.12\n" in err
+
+
+def test_cli_invalid_version_value(capsys: pytest.CaptureFixture[str], tmp_path: Path) -> None:
+    path = tmp_path / "pyproject.toml"
+    path.write_text("")
+    with pytest.raises(SystemExit) as context:
+        cli_args([str(path), "--max-supported-python", "a.1"])
+    assert context.value.code == 2
+    out, err = capsys.readouterr()
+    assert not out
+    assert (
+        "error: argument --max-supported-python: invalid version: a.1 due "
+        'ValueError("invalid literal for int() with base 10:'
+    ) in err
+
+
 def test_cli_pyproject_toml_ok(tmp_path: Path) -> None:
     path = tmp_path / "tox.ini"
     path.write_text("")
     result = cli_args([str(path)])
     assert len(result) == 1
     assert result[0]
```

### Comparing `pyproject_fmt-2.0.0/tests/test_main.py` & `pyproject_fmt-2.0.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.0/LICENSE.txt` & `pyproject_fmt-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.0/README.md` & `pyproject_fmt-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.0/pyproject.toml` & `pyproject_fmt-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-2.0.0/PKG-INFO` & `pyproject_fmt-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-fmt
-Version: 2.0.0
+Version: 2.0.1
 Summary: Format your pyproject.toml file
 Project-URL: Bug Tracker, https://github.com/tox-dev/pyproject-fmt/issues
 Project-URL: Changelog, https://github.com/tox-dev/pyproject-fmt/releases
 Project-URL: Documentation, https://github.com/tox-dev/pyproject-fmt/
 Project-URL: Source Code, https://github.com/tox-dev/pyproject-fmt
 Author-email: Bernat Gabor <gaborjbernat@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a
```

