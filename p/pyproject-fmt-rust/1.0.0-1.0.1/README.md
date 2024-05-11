# Comparing `tmp/pyproject_fmt_rust-1.0.0.tar.gz` & `tmp/pyproject_fmt_rust-1.0.1.tar.gz`

## Comparing `pyproject_fmt_rust-1.0.0.tar` & `pyproject_fmt_rust-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.0/Cargo.toml
--rw-r--r--   0     1001      127       36 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/.github/FUNDING.yml
--rw-r--r--   0     1001      127      365 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/.github/SECURITY.md
--rw-r--r--   0     1001      127      117 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/.github/dependabot.yml
--rw-r--r--   0     1001      127       76 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/.github/release.yml
--rw-r--r--   0     1001      127     2248 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/.github/workflows/check.yml
--rw-r--r--   0     1001      127     3508 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/.github/workflows/release.yml
--rw-r--r--   0     1001      127      158 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/.gitignore
--rw-r--r--   0     1001      127     1022 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      240 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/.pre-commit-hooks.yaml
--rw-r--r--   0     1001      127       16 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/.rustfmt.toml
--rw-r--r--   0     1001      127     3256 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      127     1023 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/LICENSE.txt
--rw-r--r--   0     1001      127     1147 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/README.md
--rw-r--r--   0     1001      127     3370 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/rust/src/build_system.rs
--rw-r--r--   0     1001      127     3454 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/rust/src/global.rs
--rw-r--r--   0     1001      127     8964 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/rust/src/helpers/array.rs
--rw-r--r--   0     1001      127     4529 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/rust/src/helpers/create.rs
--rw-r--r--   0     1001      127       78 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/rust/src/helpers/mod.rs
--rw-r--r--   0     1001      127     4056 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/rust/src/helpers/pep508.rs
--rw-r--r--   0     1001      127     1605 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/rust/src/helpers/string.rs
--rw-r--r--   0     1001      127     9237 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/rust/src/helpers/table.rs
--rw-r--r--   0     1001      127     4311 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/rust/src/main.rs
--rw-r--r--   0     1001      127    29493 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/rust/src/project.rs
--rw-r--r--   0     1001      127       29 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/rust-toolchain.toml
--rw-r--r--   0     1001      127      135 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/src/pyproject_fmt_rust/__init__.py
--rw-r--r--   0     1001      127      228 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/src/pyproject_fmt_rust/_lib.pyi
--rw-r--r--   0     1001      127        0 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/src/pyproject_fmt_rust/py.typed
--rw-r--r--   0     1001      127      955 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/tests/test_main.py
--rw-r--r--   0     1001      127     2076 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/tox.ini
--rw-r--r--   0     1001      127    26464 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/Cargo.lock
--rw-r--r--   0     1001      127     3375 2024-05-10 20:46:06.000000 pyproject_fmt_rust-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2387 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.1/Cargo.toml
+-rw-r--r--   0     1001      127       36 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/.github/FUNDING.yml
+-rw-r--r--   0     1001      127      365 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/.github/SECURITY.md
+-rw-r--r--   0     1001      127      117 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/.github/dependabot.yml
+-rw-r--r--   0     1001      127       76 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/.github/release.yml
+-rw-r--r--   0     1001      127     2248 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/.github/workflows/check.yml
+-rw-r--r--   0     1001      127     3508 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      158 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/.gitignore
+-rw-r--r--   0     1001      127      973 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      240 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/.pre-commit-hooks.yaml
+-rw-r--r--   0     1001      127       16 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/.rustfmt.toml
+-rw-r--r--   0     1001      127     3256 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127     1023 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/LICENSE.txt
+-rw-r--r--   0     1001      127     1147 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/README.md
+-rw-r--r--   0     1001      127     3370 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/rust/src/build_system.rs
+-rw-r--r--   0     1001      127     3454 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/rust/src/global.rs
+-rw-r--r--   0     1001      127     8964 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/rust/src/helpers/array.rs
+-rw-r--r--   0     1001      127     4529 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/rust/src/helpers/create.rs
+-rw-r--r--   0     1001      127       78 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/rust/src/helpers/mod.rs
+-rw-r--r--   0     1001      127     4056 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/rust/src/helpers/pep508.rs
+-rw-r--r--   0     1001      127     1605 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/rust/src/helpers/string.rs
+-rw-r--r--   0     1001      127     9237 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/rust/src/helpers/table.rs
+-rw-r--r--   0     1001      127     5188 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/rust/src/main.rs
+-rw-r--r--   0     1001      127    29493 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/rust/src/project.rs
+-rw-r--r--   0     1001      127       29 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/rust-toolchain.toml
+-rw-r--r--   0     1001      127      161 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/src/pyproject_fmt_rust/__init__.py
+-rw-r--r--   0     1001      127      638 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/src/pyproject_fmt_rust/_lib.pyi
+-rw-r--r--   0     1001      127        0 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/src/pyproject_fmt_rust/py.typed
+-rw-r--r--   0     1001      127      991 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/tests/test_main.py
+-rw-r--r--   0     1001      127     2076 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/tox.ini
+-rw-r--r--   0     1001      127    26464 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/Cargo.lock
+-rw-r--r--   0     1001      127     3335 2024-05-11 04:18:21.000000 pyproject_fmt_rust-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2387 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.1/PKG-INFO
```

### Comparing `pyproject_fmt_rust-1.0.0/Cargo.toml` & `pyproject_fmt_rust-1.0.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyproject-fmt-rust"
-version = "1.0.0"
+version = "1.0.1"
 description = "Format pyproject.toml files"
 repository = "https://github.com/tox-dev/pyproject-fmt"
 readme = "README.md"
 license = "MIT"
 edition = "2021"
 
 [lib]
```

### Comparing `pyproject_fmt_rust-1.0.0/.github/workflows/check.yml` & `pyproject_fmt_rust-1.0.1/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/.github/workflows/release.yml` & `pyproject_fmt_rust-1.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/.pre-commit-config.yaml` & `pyproject_fmt_rust-1.0.1/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,17 @@
         args: [ "--write-changes" ]
   - repo: https://github.com/tox-dev/tox-ini-fmt
     rev: "1.3.1"
     hooks:
       - id: tox-ini-fmt
         args: [ "-p", "fix" ]
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: "1.8.0"
+    rev: "2.0.1"
     hooks:
       - id: pyproject-fmt
-        additional_dependencies: [ "tox>=4.15" ]
   - repo: https://github.com/astral-sh/ruff-pre-commit
     rev: "v0.4.4"
     hooks:
       - id: ruff-format
       - id: ruff
         args: [ "--fix", "--unsafe-fixes", "--exit-non-zero-on-fix" ]
   - repo: meta
```

### Comparing `pyproject_fmt_rust-1.0.0/CODE_OF_CONDUCT.md` & `pyproject_fmt_rust-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/LICENSE.txt` & `pyproject_fmt_rust-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/README.md` & `pyproject_fmt_rust-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/rust/src/build_system.rs` & `pyproject_fmt_rust-1.0.1/rust/src/build_system.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/rust/src/global.rs` & `pyproject_fmt_rust-1.0.1/rust/src/global.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/rust/src/helpers/array.rs` & `pyproject_fmt_rust-1.0.1/rust/src/helpers/array.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/rust/src/helpers/create.rs` & `pyproject_fmt_rust-1.0.1/rust/src/helpers/create.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/rust/src/helpers/pep508.rs` & `pyproject_fmt_rust-1.0.1/rust/src/helpers/pep508.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/rust/src/helpers/string.rs` & `pyproject_fmt_rust-1.0.1/rust/src/helpers/string.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/rust/src/helpers/table.rs` & `pyproject_fmt_rust-1.0.1/rust/src/helpers/table.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/rust/src/main.rs` & `pyproject_fmt_rust-1.0.1/rust/src/main.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,88 @@
 use std::string::String;
 
 use pyo3::prelude::PyModule;
-use pyo3::{pyfunction, pymodule, wrap_pyfunction, Bound, PyResult};
+use pyo3::{pyclass, pyfunction, pymethods, pymodule, wrap_pyfunction, Bound, PyResult};
 use taplo::formatter::{format_syntax, Options};
 use taplo::parser::parse;
 
 use crate::build_system::fix_build;
 use crate::global::reorder_tables;
 use crate::helpers::table::Tables;
 use crate::project::fix_project_table;
 
 mod build_system;
 mod project;
 
 mod global;
 mod helpers;
 
-/// Format toml file
-#[pyfunction]
-#[must_use]
-pub fn format_toml(
-    content: &str,
+#[pyclass(frozen, get_all)]
+pub struct Settings {
     column_width: usize,
     indent: usize,
     keep_full_version: bool,
     max_supported_python: (u8, u8),
     min_supported_python: (u8, u8),
-) -> String {
+}
+
+#[pymethods]
+impl Settings {
+    #[new]
+    #[pyo3(signature = (*, column_width, indent, keep_full_version, max_supported_python, min_supported_python ))]
+    const fn new(
+        column_width: usize,
+        indent: usize,
+        keep_full_version: bool,
+        max_supported_python: (u8, u8),
+        min_supported_python: (u8, u8),
+    ) -> Self {
+        Self {
+            column_width,
+            indent,
+            keep_full_version,
+            max_supported_python,
+            min_supported_python,
+        }
+    }
+}
+
+/// Format toml file
+#[must_use]
+#[pyfunction]
+pub fn format_toml(content: &str, opt: &Settings) -> String {
     let root_ast = parse(content).into_syntax().clone_for_update();
     let mut tables = Tables::from_ast(&root_ast);
 
-    fix_build(&mut tables, keep_full_version);
+    fix_build(&mut tables, opt.keep_full_version);
     fix_project_table(
         &mut tables,
-        keep_full_version,
-        max_supported_python,
-        min_supported_python,
+        opt.keep_full_version,
+        opt.max_supported_python,
+        opt.min_supported_python,
     );
     reorder_tables(&root_ast, &mut tables);
 
     let options = Options {
-        align_entries: false,         // do not align by =
-        align_comments: true,         // align inline comments
-        align_single_comments: true,  // align comments after entries
-        array_trailing_comma: true,   // ensure arrays finish with trailing comma
-        array_auto_expand: true,      // arrays go to multi line for easier diffs
-        array_auto_collapse: false,   // do not collapse for easier diffs
-        compact_arrays: false,        // do not compact for easier diffs
-        compact_inline_tables: false, // do not compact for easier diffs
-        compact_entries: false,       // do not compact for easier diffs
-        column_width,                 // always expand arrays per https://github.com/tamasfe/taplo/issues/390
+        align_entries: false,           // do not align by =
+        align_comments: true,           // align inline comments
+        align_single_comments: true,    // align comments after entries
+        array_trailing_comma: true,     // ensure arrays finish with trailing comma
+        array_auto_expand: true,        // arrays go to multi line for easier diffs
+        array_auto_collapse: false,     // do not collapse for easier diffs
+        compact_arrays: false,          // do not compact for easier diffs
+        compact_inline_tables: false,   // do not compact for easier diffs
+        compact_entries: false,         // do not compact for easier diffs
+        column_width: opt.column_width, // always expand arrays per https://github.com/tamasfe/taplo/issues/390
         indent_tables: false,
         indent_entries: false,
         inline_table_expand: true,
         trailing_newline: true,
         allowed_blank_lines: 1, // one blank line to separate
-        indent_string: " ".repeat(indent),
+        indent_string: " ".repeat(opt.indent),
         reorder_keys: false,   // respect custom order
         reorder_arrays: false, // for natural sorting we need to this ourselves
         crlf: false,
     };
     format_syntax(root_ast, options)
 }
 
@@ -67,23 +90,24 @@
 ///
 /// Will return `PyErr` if an error is raised during formatting.
 #[pymodule]
 #[pyo3(name = "_lib")]
 #[cfg(not(tarpaulin_include))]
 pub fn _lib(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(format_toml, m)?)?;
+    m.add_class::<Settings>()?;
     Ok(())
 }
 
 #[cfg(test)]
 mod tests {
     use indoc::indoc;
     use rstest::rstest;
 
-    use crate::format_toml;
+    use crate::{format_toml, Settings};
 
     #[rstest]
     #[case::simple(
         indoc ! {r#"
     # comment
     a= "b"
     [project]
@@ -156,11 +180,20 @@
     fn test_format_toml(
         #[case] start: &str,
         #[case] expected: &str,
         #[case] indent: usize,
         #[case] keep_full_version: bool,
         #[case] max_supported_python: (u8, u8),
     ) {
-        let got = format_toml(start, 1, indent, keep_full_version, max_supported_python, (3, 8));
+        let got = format_toml(
+            start,
+            &Settings {
+                column_width: 1,
+                indent,
+                keep_full_version,
+                max_supported_python,
+                min_supported_python: (3, 8),
+            },
+        );
         assert_eq!(got, expected);
     }
 }
```

### Comparing `pyproject_fmt_rust-1.0.0/rust/src/project.rs` & `pyproject_fmt_rust-1.0.1/rust/src/project.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/tests/test_main.py` & `pyproject_fmt_rust-1.0.1/tests/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from textwrap import dedent
 
-from pyproject_fmt_rust import format_toml
+from pyproject_fmt_rust import Settings, format_toml
 
 
 def test_format_toml() -> None:
     txt = """
     [project]
     keywords = [
       "A",
@@ -18,22 +18,22 @@
       "B",
     ]
     dependencies = [
       "requests>=2.0",
     ]
     """
 
-    res = format_toml(
-        dedent(txt),
+    settings = Settings(
         column_width=120,
         indent=4,
         keep_full_version=True,
         min_supported_python=(3, 7),
         max_supported_python=(3, 8),
     )
+    res = format_toml(dedent(txt), settings)
 
     expected = """\
     [project]
     keywords = [
         "A",
     ]
     classifiers = [
```

### Comparing `pyproject_fmt_rust-1.0.0/tox.ini` & `pyproject_fmt_rust-1.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.0/Cargo.lock` & `pyproject_fmt_rust-1.0.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -516,15 +516,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyproject-fmt-rust"
-version = "1.0.0"
+version = "1.0.1"
 dependencies = [
  "indoc",
  "lexical-sort",
  "pep508_rs",
  "pyo3",
  "regex",
  "rstest",
```

### Comparing `pyproject_fmt_rust-1.0.0/pyproject.toml` & `pyproject_fmt_rust-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 build-backend = "maturin"
 requires = [
   "maturin>=1.5.1",
 ]
 
 [project]
 name = "pyproject-fmt-rust"
-version = "1.0.0"
+version = "1.0.1"
 description = "Format your pyproject.toml file"
 readme = "README.md"
 keywords = [
   "format",
   "pyproject",
 ]
 license.file = "LICENSE.txt"
 authors = [
-    { name = "Bernat Gabor", email = "gaborjbernat@gmail.com" },
+  { name = "Bernat Gabor", email = "gaborjbernat@gmail.com" },
 ]
 requires-python = ">=3.8"
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
@@ -47,85 +47,85 @@
 [tool.maturin]
 bindings = "pyo3"
 manifest-path = "Cargo.toml"
 module-name = "pyproject_fmt_rust._lib"
 python-source = "src"
 strip = true
 include = [
-    "rust-toolchain.toml",
+  "rust-toolchain.toml",
 ]
 
 [tool.cibuildwheel]
 skip = [
-    "pp*",
-    "*musl*",
+  "pp*",
+  "*musl*",
 ]
 
 [tool.ruff]
 line-length = 120
 target-version = "py38"
 lint.isort = { known-first-party = [
-    "pyproject_fmt_rust",
+  "pyproject_fmt_rust",
 ], required-imports = [
-    "from __future__ import annotations",
+  "from __future__ import annotations",
 ] }
 lint.select = [
-    "ALL",
+  "ALL",
 ]
 lint.ignore = [
-    "ANN101", # no type annotation for self
-    "ANN401", # allow Any as type annotation
-    "COM812", # Conflict with formatter
-    "CPY", # No copyright statements
-    "D203", # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
-    "D212", # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
-    "ISC001", # Conflict with formatter
-    "S104", # Possible binding to all interface
+  "ANN101", # no type annotation for self
+  "ANN401", # allow Any as type annotation
+  "COM812", # Conflict with formatter
+  "CPY",    # No copyright statements
+  "D203",   # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
+  "D212",   # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
+  "ISC001", # Conflict with formatter
+  "S104",   # Possible binding to all interface
 ]
 lint.preview = true
 format.preview = true
 format.docstring-code-format = true
 format.docstring-code-line-length = 100
 
 [tool.ruff.lint.per-file-ignores]
 "tests/**/*.py" = [
-    "D", # don"t care about documentation in tests
-    "FBT", # don"t care about booleans as positional arguments in tests
-    "INP001", # no implicit namespace
-    "PLC2701", # private import
-    "PLR0913", # any number of arguments in tests
-    "PLR0917", # any number of arguments in tests
-    "PLR2004", # Magic value used in comparison, consider replacing with a constant variable
-    "S101", # asserts allowed in tests...
-    "S603", # `subprocess` call: check for execution of untrusted input
+  "D",       # don"t care about documentation in tests
+  "FBT",     # don"t care about booleans as positional arguments in tests
+  "INP001",  # no implicit namespace
+  "PLC2701", # private import
+  "PLR0913", # any number of arguments in tests
+  "PLR0917", # any number of arguments in tests
+  "PLR2004", # Magic value used in comparison, consider replacing with a constant variable
+  "S101",    # asserts allowed in tests...
+  "S603",    # `subprocess` call: check for execution of untrusted input
 ]
 
 [tool.codespell]
 builtin = "clear,usage,en-GB_to_en-US"
 count = true
 
 [tool.pytest]
 ini_options.testpaths = [
-    "tests",
+  "tests",
 ]
 
 [tool.coverage]
 html.show_contexts = true
 html.skip_covered = false
 paths.source = [
-    "src",
-    ".tox/*/.venv/lib/*/site-packages",
-    ".tox\\*\\.venv\\Lib\\site-packages",
-    ".tox/*/lib/*/site-packages",
-    ".tox\\*\\Lib\\site-packages",
-    "**/src",
-    "**\\src",
+  "src",
+  ".tox/*/.venv/lib/*/site-packages",
+  ".tox\\*\\.venv\\Lib\\site-packages",
+  ".tox/*/lib/*/site-packages",
+  ".tox\\*\\Lib\\site-packages",
+  "**/src",
+  "**\\src",
 ]
 report.fail_under = 100
 run.parallel = true
 run.plugins = [
-    "covdefaults",
+  "covdefaults",
 ]
 
 [tool.mypy]
 show_error_codes = true
 strict = true
```

### Comparing `pyproject_fmt_rust-1.0.0/PKG-INFO` & `pyproject_fmt_rust-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-fmt-rust
-Version: 1.0.0
+Version: 1.0.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

