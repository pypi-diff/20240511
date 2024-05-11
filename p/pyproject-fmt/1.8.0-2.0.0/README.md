# Comparing `tmp/pyproject_fmt-1.8.0.tar.gz` & `tmp/pyproject_fmt-2.0.0.tar.gz`

## Comparing `pyproject_fmt-1.8.0.tar` & `pyproject_fmt-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,14 @@
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tox.ini
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/__init__.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/_version.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/py.typed
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/__init__.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/build_system.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/config.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/pep508.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/project.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/tools.py
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/src/pyproject_fmt/formatter/util.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/__init__.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/test_cli.py
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/test_main.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/test_pyproject_toml_fmt.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/formatter/conftest.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/formatter/test_build_system.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/formatter/test_pep508.py
--rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/formatter/test_project.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/tests/formatter/test_tools.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/LICENSE.txt
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/README.md
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pyproject_fmt-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/tox.ini
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/src/pyproject_fmt/__init__.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/src/pyproject_fmt/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/src/pyproject_fmt/_version.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/src/pyproject_fmt/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/src/pyproject_fmt/py.typed
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/tests/test_cli.py
+-rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/tests/test_main.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/tests/test_pyproject_toml_fmt.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/README.md
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 pyproject_fmt-2.0.0/PKG-INFO
```

### Comparing `pyproject_fmt-1.8.0/tox.ini` & `pyproject_fmt-2.0.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -31,35 +31,35 @@
       --cov-report html:{envtmpdir}{/}htmlcov --cov-report xml:{toxworkdir}{/}coverage.{envname}.xml \
       tests}
 
 [testenv:fix]
 description = run static analysis and style check using flake8
 skip_install = true
 deps =
-    pre-commit>=3.5
+    pre-commit>=3.7
 commands =
     pre-commit run --all-files --show-diff-on-failure
     python -c 'print("hint: run {envdir}/bin/pre-commit install to add checks as pre-commit hook")'
 
 [testenv:type]
 description = run type check on code base
 deps =
-    mypy==1.7.1
+    mypy==1.10
 set_env =
     {tty:MYPY_FORCE_COLOR = 1}
 commands =
     mypy src
     mypy tests
 
 [testenv:readme]
 description = check that the long description is valid
 skip_install = true
 deps =
-    build[virtualenv]>=1.0.3
-    twine>=4.0.2
+    build[virtualenv]>=1.2.1
+    twine>=5
 commands =
     python -m build --sdist --wheel -o {envtmpdir} .
     twine check {envtmpdir}/*
 
 [testenv:docs]
 description = build documentation
 extras =
@@ -73,7 +73,8 @@
 package = editable
 extras =
     docs
     test
 commands =
     python -m pip list --format=columns
     python -c 'import sys; print(sys.executable)'
+uv_seed = true
```

### Comparing `pyproject_fmt-1.8.0/src/pyproject_fmt/__main__.py` & `pyproject_fmt-2.0.0/src/pyproject_fmt/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from __future__ import annotations
 
 import difflib
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterable, Sequence
 
-from pyproject_fmt.cli import PyProjectFmtNamespace, cli_args
-from pyproject_fmt.formatter import format_pyproject
+from pyproject_fmt_rust import format_toml
+
+from pyproject_fmt.cli import cli_args
 
 if TYPE_CHECKING:
-    from pyproject_fmt import Config
+    from pyproject_fmt.cli import Config
 
 GREEN = "\u001b[32m"
 RED = "\u001b[31m"
 RESET = "\u001b[0m"
 
 
 def color_diff(diff: Iterable[str]) -> Iterable[str]:
@@ -29,23 +30,30 @@
             yield f"{GREEN}{line}{RESET}"
         elif line.startswith("-"):
             yield f"{RED}{line}{RESET}"
         else:
             yield line
 
 
-def _handle_one(config: Config, opts: PyProjectFmtNamespace) -> bool:
-    formatted = format_pyproject(config)
+def _handle_one(config: Config) -> bool:
+    formatted = format_toml(
+        config.toml,
+        column_width=config.column_width,
+        indent=config.indent,
+        keep_full_version=config.keep_full_version,
+        max_supported_python=(config.max_supported_python.major, config.max_supported_python.minor),
+        min_supported_python=(config.min_supported_python.major, config.min_supported_python.minor),
+    )
     before = config.toml
     changed = before != formatted
-    if opts.stdout:  # stdout just prints new format to stdout
+    if config.stdout:  # stdout just prints new format to stdout
         print(formatted, end="")  # noqa: T201
         return changed
 
-    if before != formatted and not opts.check:
+    if before != formatted and not config.check:
         config.pyproject_toml.write_text(formatted, encoding="utf-8")
     try:
         name = str(config.pyproject_toml.relative_to(Path.cwd()))
     except ValueError:
         name = str(config.pyproject_toml)
     diff: Iterable[str] = []
     if changed:
@@ -62,14 +70,14 @@
 def run(args: Sequence[str] | None = None) -> int:
     """
     Run the formatter.
 
     :param args: CLI arguments
     :return: exit code
     """
-    opts = cli_args(sys.argv[1:] if args is None else args)
-    results = [_handle_one(config, opts) for config in opts.configs]
+    configs = cli_args(sys.argv[1:] if args is None else args)
+    results = [_handle_one(config) for config in configs]
     return 1 if any(results) else 0  # exit with non success on change
 
 
 if __name__ == "__main__":
     raise SystemExit(run())
```

### Comparing `pyproject_fmt-1.8.0/src/pyproject_fmt/cli.py` & `pyproject_fmt-2.0.0/src/pyproject_fmt/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,65 @@
 """CLI interface parser."""
 
 from __future__ import annotations
 
+import sys
+from dataclasses import dataclass
+
+if sys.version_info >= (3, 11):  # pragma: >=3.11 cover
+    import tomllib
+else:  # pragma: <3.11 cover
+    import tomli as tomllib
+
 import os
 from argparse import (
     ArgumentDefaultsHelpFormatter,
     ArgumentParser,
     ArgumentTypeError,
     Namespace,
 )
+from importlib.metadata import version
 from pathlib import Path
 from typing import Sequence
 
 from packaging.version import Version
 
-from ._version import __version__
-from .formatter.config import DEFAULT_INDENT, DEFAULT_MAX_SUPPORTED_PYTHON, Config
-
 
 class PyProjectFmtNamespace(Namespace):
     """Options for pyproject-fmt tool."""
 
     inputs: list[Path]
     stdout: bool
-    indent: int
     check: bool
+
+    column_width: int
+    indent: int
     keep_full_version: bool
     max_supported_python: Version
+    min_supported_python: Version
+
+
+@dataclass(frozen=True)
+class Config:
+    """Configuration flags for the formatting."""
+
+    pyproject_toml: Path
+    stdout: bool  # push to standard out
+    check: bool  # check only
+
+    column_width: int  #: maximum column width
+    indent: int  #: indentation to apply
+    keep_full_version: bool  #: whether to keep full dependency versions
+    max_supported_python: Version  #: the maximum supported Python version
+    min_supported_python: Version  #: the minimum supported Python version
 
     @property
-    def configs(self) -> list[Config]:
-        """:return: configurations"""
-        return [
-            Config(
-                pyproject_toml=toml,
-                toml=toml.read_text(encoding="utf-8"),
-                indent=self.indent,
-                keep_full_version=self.keep_full_version,
-                max_supported_python=self.max_supported_python,
-            )
-            for toml in self.inputs
-        ]
+    def toml(self) -> str:
+        """:return: the toml files content"""
+        return self.pyproject_toml.read_text(encoding="utf-8")
 
 
 def pyproject_toml_path_creator(argument: str) -> Path:
     """
     Validate that pyproject.toml can be formatted.
 
     :param argument: the string argument passed in
@@ -74,50 +89,97 @@
         prog="pyproject-fmt",
     )
     parser.add_argument(
         "-V",
         "--version",
         action="version",
         help="print package version of pyproject_fmt",
-        version=f"%(prog)s ({__version__})",
+        version=f"%(prog)s ({version('pyproject-fmt')})",
     )
     group = parser.add_mutually_exclusive_group()
     msg = "print the formatted text to the stdout (instead of update in-place)"
     group.add_argument("-s", "--stdout", action="store_true", help=msg)
     msg = "check and fail if any input would be formatted, printing any diffs"
     group.add_argument("--check", action="store_true", help=msg)
     msg = "keep full dependency versions. For example do not change version 1.0.0 to 1"
     parser.add_argument("--keep-full-version", action="store_true", help=msg)
     parser.add_argument(
+        "--column-width",
+        type=int,
+        default=1,
+        help="max column width in the file",
+    )
+    parser.add_argument(
         "--indent",
         type=int,
-        default=DEFAULT_INDENT,
+        default=2,
         help="number of spaces to indent",
     )
     parser.add_argument(
+        "--min-supported-python",
+        type=Version,
+        default="3.8",
+        help="latest Python version the project supports (e.g. 3.8)",
+    )
+    parser.add_argument(
         "--max-supported-python",
         type=Version,
-        default=DEFAULT_MAX_SUPPORTED_PYTHON,
+        default="3.12",
         help="latest Python version the project supports (e.g. 3.13)",
     )
     msg = "pyproject.toml file(s) to format"
     parser.add_argument("inputs", nargs="+", type=pyproject_toml_path_creator, help=msg)
     return parser
 
 
-def cli_args(args: Sequence[str]) -> PyProjectFmtNamespace:
+def cli_args(args: Sequence[str]) -> list[Config]:
     """
     Load the tools options.
 
     :param args: CLI arguments
     :return: the parsed options
     """
     parser = _build_cli()
-    result = PyProjectFmtNamespace()
-    parser.parse_args(namespace=result, args=args)
-    return result
+    opt = PyProjectFmtNamespace()
+    parser.parse_args(namespace=opt, args=args)
+    res = []
+    for pyproject_toml in opt.inputs:
+        column_width = opt.column_width
+        indent = opt.indent
+        keep_full_version = opt.keep_full_version
+        max_supported_python = opt.max_supported_python
+        min_supported_python = opt.min_supported_python
+        with pyproject_toml.open("rb") as file_handler:
+            config = tomllib.load(file_handler)
+            if "tool" in config and "pyproject-fmt" in config["tool"]:
+                for key, entry in config["tool"]["pyproject-fmt"].items():
+                    if key == "column_width":
+                        column_width = int(entry)
+                    elif key == "indent":
+                        indent = int(entry)
+                    elif key == "keep_full_version":
+                        keep_full_version = bool(entry)
+                    elif key == "max_supported_python":
+                        max_supported_python = Version(entry)
+                    elif key == "min_supported_python":  # pragma: no branch
+                        min_supported_python = Version(entry)
+        res.append(
+            Config(
+                pyproject_toml=pyproject_toml,
+                stdout=opt.stdout,
+                check=opt.check,
+                column_width=column_width,
+                indent=indent,
+                keep_full_version=keep_full_version,
+                max_supported_python=max_supported_python,
+                min_supported_python=min_supported_python,
+            )
+        )
+
+    return res
 
 
 __all__ = [
+    "Config",
     "PyProjectFmtNamespace",
     "cli_args",
 ]
```

### Comparing `pyproject_fmt-1.8.0/tests/test_cli.py` & `pyproject_fmt-2.0.0/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 from __future__ import annotations
 
 import os
 import sys
+from importlib.metadata import version
 from stat import S_IREAD, S_IWRITE
 from typing import TYPE_CHECKING
 
 import pytest
 
-from pyproject_fmt._version import __version__
 from pyproject_fmt.cli import cli_args
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 
 def test_cli_version(capsys: pytest.CaptureFixture[str]) -> None:
     with pytest.raises(SystemExit) as context:
         cli_args(["--version"])
     assert context.value.code == 0
     out, _err = capsys.readouterr()
-    assert out == f"pyproject-fmt ({__version__})\n"
+    assert out == f"pyproject-fmt ({version('pyproject-fmt')})\n"
 
 
 def test_cli_pyproject_toml_ok(tmp_path: Path) -> None:
     path = tmp_path / "tox.ini"
     path.write_text("")
     result = cli_args([str(path)])
-    assert result.inputs == [path]
+    assert len(result) == 1
+    assert result[0]
 
 
 def test_cli_inputs_ok(tmp_path: Path) -> None:
     paths = []
     for filename in ("tox.ini", "tox2.ini", "tox3.ini"):
         path = tmp_path / filename
         path.write_text("")
         paths.append(path)
     result = cli_args([*map(str, paths)])
-    assert result.inputs == paths
+    assert len(result) == 3
 
 
 def test_cli_pyproject_toml_not_exists(
     tmp_path: Path,
     capsys: pytest.CaptureFixture[str],
 ) -> None:
     with pytest.raises(SystemExit) as context:
@@ -94,13 +95,13 @@
     tmp_path: Path,
     monkeypatch: pytest.MonkeyPatch,
 ) -> None:
     monkeypatch.chdir(tmp_path)
     path = tmp_path / "tox.ini"
     path.write_text("")
     result = cli_args(["tox.ini"])
-    assert result.inputs == [path]
+    assert len(result) == 1
 
 
 def test_pyproject_toml_dir(tmp_path: Path) -> None:
     (tmp_path / "pyproject.toml").write_text("")
     cli_args([str(tmp_path)])
```

### Comparing `pyproject_fmt-1.8.0/tests/test_main.py` & `pyproject_fmt-2.0.0/tests/test_main.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 
 import difflib
 from textwrap import dedent
 from typing import TYPE_CHECKING, Any
 
 import pytest
 
-import pyproject_fmt.__main__
+from pyproject_fmt import __version__
 from pyproject_fmt.__main__ import GREEN, RED, RESET, color_diff, run
 
 if TYPE_CHECKING:
     from pathlib import Path
 
+    from pytest_mock import MockerFixture
+
+
+def test_version() -> None:
+    assert isinstance(__version__, str)
+
 
 def test_color_diff() -> None:
     # Arrange
     before = """
     abc
     def
     ghi
@@ -93,18 +99,19 @@
     tmp_path: Path,
     capsys: pytest.CaptureFixture[str],
     in_place: bool,
     start: str,
     outcome: str,
     output: str,
     monkeypatch: pytest.MonkeyPatch,
+    mocker: MockerFixture,
     cwd: bool,
     check: bool,
 ) -> None:
-    monkeypatch.setattr(pyproject_fmt.__main__, "color_diff", no_color)
+    mocker.patch("pyproject_fmt.__main__.color_diff", no_color)
     if cwd:
         monkeypatch.chdir(tmp_path)
     pyproject_toml = tmp_path / "pyproject.toml"
     pyproject_toml.write_text(start)
     args = [str(pyproject_toml)]
     if not in_place:
         args.append("--stdout")
@@ -143,40 +150,103 @@
         "A",
     ]
     """
 
     expected = f"""\
     [build-system]
     requires = [
-    {" " * indent}"A",
+    {" " * indent}"a",
     ]
     """
     pyproject_toml = tmp_path / "pyproject.toml"
     pyproject_toml.write_text(dedent(start))
     args = [str(pyproject_toml), "--indent", str(indent)]
     run(args)
     output = pyproject_toml.read_text()
     assert output == dedent(expected)
 
 
 def test_keep_full_version_cli(tmp_path: Path) -> None:
     start = """\
     [build-system]
     requires = [
-      "A==1.0.0",
+      "a==1.0.0",
     ]
 
     [project]
+    classifiers = [
+      "Programming Language :: Python :: 3 :: Only",
+      "Programming Language :: Python :: 3.8",
+    ]
     dependencies = [
-      "A==1.0.0",
+      "a==1.0.0",
     ]
-    [project.optional-dependencies]
-    docs = [
-      "B==2.0.0",
+    optional-dependencies.docs = [
+      "b==2.0.0",
     ]
     """
     pyproject_toml = tmp_path / "pyproject.toml"
     pyproject_toml.write_text(dedent(start))
-    args = [str(pyproject_toml), "--keep-full-version"]
+    args = [str(pyproject_toml), "--keep-full-version", "--max-supported-python", "3.8"]
     run(args)
     output = pyproject_toml.read_text()
     assert output == dedent(start)
+
+
+def test_pyproject_toml_config(tmp_path: Path, capsys: pytest.CaptureFixture[str]) -> None:
+    txt = """
+    [project]
+    keywords = [
+      "A",
+    ]
+    classifiers = [
+      "Programming Language :: Python :: 3 :: Only",
+    ]
+    dynamic = [
+      "B",
+    ]
+    dependencies = [
+      "requests>=2.0",
+    ]
+
+    [tool.pyproject-fmt]
+    column_width = 20
+    indent = 4
+    keep_full_version = true
+    min_supported_python = "3.7"
+    max_supported_python = "3.10"
+    """
+    filename = tmp_path / "pyproject.toml"
+    filename.write_text(dedent(txt))
+    run([str(filename)])
+
+    expected = """\
+    [project]
+    keywords = [
+        "A",
+    ]
+    classifiers = [
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+    ]
+    dynamic = [
+        "B",
+    ]
+    dependencies = [
+        "requests>=2.0",
+    ]
+
+    [tool.pyproject-fmt]
+    column_width = 20
+    indent = 4
+    keep_full_version = true
+    min_supported_python = "3.7"
+    max_supported_python = "3.10"
+    """
+    got = filename.read_text()
+    assert got == dedent(expected)
+    out, err = capsys.readouterr()
+    assert out
+    assert not err
```

### Comparing `pyproject_fmt-1.8.0/LICENSE.txt` & `pyproject_fmt-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-1.8.0/README.md` & `pyproject_fmt-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-1.8.0/pyproject.toml` & `pyproject_fmt-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs>=0.4",
-  "hatchling>=1.18",
+  "hatchling>=1.24.2",
 ]
 
 [project]
 name = "pyproject-fmt"
 description = "Format your pyproject.toml file"
 readme = "README.md"
 keywords = [
@@ -27,30 +27,28 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "natsort>=8.4",
-  "packaging>=23.2",
-  "tomlkit>=0.12.3",
+  "pyproject-fmt-rust==1",
 ]
 optional-dependencies.docs = [
-  "furo>=2023.9.10",
-  "sphinx>=7.2.6",
-  "sphinx-argparse-cli>=1.11.1",
-  "sphinx-autodoc-typehints>=1.25.2",
+  "furo>=2024.5.6",
+  "sphinx>=7.3.7",
+  "sphinx-argparse-cli>=1.15",
+  "sphinx-autodoc-typehints>=2.1",
   "sphinx-copybutton>=0.5.2",
 ]
 optional-dependencies.test = [
   "covdefaults>=2.3",
-  "pytest>=7.4.3",
-  "pytest-cov>=4.1",
-  "pytest-mock>=3.12",
+  "pytest>=8.2",
+  "pytest-cov>=5",
+  "pytest-mock>=3.14",
 ]
 urls."Bug Tracker" = "https://github.com/tox-dev/pyproject-fmt/issues"
 urls."Changelog" = "https://github.com/tox-dev/pyproject-fmt/releases"
 urls.Documentation = "https://github.com/tox-dev/pyproject-fmt/"
 urls."Source Code" = "https://github.com/tox-dev/pyproject-fmt"
 scripts.pyproject-fmt = "pyproject_fmt.__main__:run"
 
@@ -98,15 +96,23 @@
 
 [tool.pytest]
 ini_options.testpaths = ["tests"]
 
 [tool.coverage]
 html.show_contexts = true
 html.skip_covered = false
-paths.source = ["src", ".tox/*/lib/python*/site-packages", "*/src"]
-report.fail_under = 88
+paths.source = [
+  "src",
+  ".tox/*/.venv/lib/*/site-packages",
+  ".tox\\*\\.venv\\Lib\\site-packages",
+  ".tox/*/lib/*/site-packages",
+  ".tox\\*\\Lib\\site-packages",
+  "**/src",
+  "**\\src",
+]
+report.fail_under = 100
 run.parallel = true
 run.plugins = ["covdefaults"]
 
 [tool.mypy]
 show_error_codes = true
 strict = true
```

### Comparing `pyproject_fmt-1.8.0/PKG-INFO` & `pyproject_fmt-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-fmt
-Version: 1.8.0
+Version: 2.0.0
 Summary: Format your pyproject.toml file
 Project-URL: Bug Tracker, https://github.com/tox-dev/pyproject-fmt/issues
 Project-URL: Changelog, https://github.com/tox-dev/pyproject-fmt/releases
 Project-URL: Documentation, https://github.com/tox-dev/pyproject-fmt/
 Project-URL: Source Code, https://github.com/tox-dev/pyproject-fmt
 Author-email: Bernat Gabor <gaborjbernat@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a
@@ -33,28 +33,26 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: natsort>=8.4
-Requires-Dist: packaging>=23.2
-Requires-Dist: tomlkit>=0.12.3
+Requires-Dist: pyproject-fmt-rust==1
 Provides-Extra: docs
-Requires-Dist: furo>=2023.9.10; extra == 'docs'
-Requires-Dist: sphinx-argparse-cli>=1.11.1; extra == 'docs'
-Requires-Dist: sphinx-autodoc-typehints>=1.25.2; extra == 'docs'
+Requires-Dist: furo>=2024.5.6; extra == 'docs'
+Requires-Dist: sphinx-argparse-cli>=1.15; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints>=2.1; extra == 'docs'
 Requires-Dist: sphinx-copybutton>=0.5.2; extra == 'docs'
-Requires-Dist: sphinx>=7.2.6; extra == 'docs'
+Requires-Dist: sphinx>=7.3.7; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: covdefaults>=2.3; extra == 'test'
-Requires-Dist: pytest-cov>=4.1; extra == 'test'
-Requires-Dist: pytest-mock>=3.12; extra == 'test'
-Requires-Dist: pytest>=7.4.3; extra == 'test'
+Requires-Dist: pytest-cov>=5; extra == 'test'
+Requires-Dist: pytest-mock>=3.14; extra == 'test'
+Requires-Dist: pytest>=8.2; extra == 'test'
 Description-Content-Type: text/markdown
 
 # pyproject-fmt
 
 [![PyPI](https://img.shields.io/pypi/v/pyproject-fmt?style=flat-square)](https://pypi.org/project/pyproject-fmt)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/pyproject-fmt?style=flat-square)](https://pypi.org/project/pyproject-fmt)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyproject-fmt?style=flat-square)](https://pypi.org/project/pyproject-fmt)
```

