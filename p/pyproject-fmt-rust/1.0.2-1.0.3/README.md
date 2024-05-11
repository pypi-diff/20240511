# Comparing `tmp/pyproject_fmt_rust-1.0.2.tar.gz` & `tmp/pyproject_fmt_rust-1.0.3.tar.gz`

## Comparing `pyproject_fmt_rust-1.0.2.tar` & `pyproject_fmt_rust-1.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.2/Cargo.toml
--rw-r--r--   0     1001      127       36 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/.github/FUNDING.yml
--rw-r--r--   0     1001      127      365 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/.github/SECURITY.md
--rw-r--r--   0     1001      127      117 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/.github/dependabot.yml
--rw-r--r--   0     1001      127       76 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/.github/release.yml
--rw-r--r--   0     1001      127     2248 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/.github/workflows/check.yml
--rw-r--r--   0     1001      127     3801 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/.github/workflows/release.yml
--rw-r--r--   0     1001      127      158 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/.gitignore
--rw-r--r--   0     1001      127      973 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      240 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/.pre-commit-hooks.yaml
--rw-r--r--   0     1001      127       16 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/.rustfmt.toml
--rw-r--r--   0     1001      127     3256 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      127     1023 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/LICENSE.txt
--rw-r--r--   0     1001      127     1147 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/README.md
--rw-r--r--   0     1001      127     3370 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/rust/src/build_system.rs
--rw-r--r--   0     1001      127     3454 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/rust/src/global.rs
--rw-r--r--   0     1001      127     8964 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/rust/src/helpers/array.rs
--rw-r--r--   0     1001      127     4529 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/rust/src/helpers/create.rs
--rw-r--r--   0     1001      127       78 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/rust/src/helpers/mod.rs
--rw-r--r--   0     1001      127     4056 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/rust/src/helpers/pep508.rs
--rw-r--r--   0     1001      127     1605 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/rust/src/helpers/string.rs
--rw-r--r--   0     1001      127     9237 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/rust/src/helpers/table.rs
--rw-r--r--   0     1001      127     5188 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/rust/src/main.rs
--rw-r--r--   0     1001      127    29493 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/rust/src/project.rs
--rw-r--r--   0     1001      127       29 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/rust-toolchain.toml
--rw-r--r--   0     1001      127      161 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/src/pyproject_fmt_rust/__init__.py
--rw-r--r--   0     1001      127      638 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/src/pyproject_fmt_rust/_lib.pyi
--rw-r--r--   0     1001      127        0 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/src/pyproject_fmt_rust/py.typed
--rw-r--r--   0     1001      127      991 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/tests/test_main.py
--rw-r--r--   0     1001      127     2076 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/tox.ini
--rw-r--r--   0     1001      127    26464 2024-05-11 05:23:08.000000 pyproject_fmt_rust-1.0.2/Cargo.lock
--rw-r--r--   0     1001      127     3317 2024-05-11 05:22:56.000000 pyproject_fmt_rust-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2387 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.3/Cargo.toml
+-rw-r--r--   0     1001      127       36 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/.github/FUNDING.yml
+-rw-r--r--   0     1001      127      365 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/.github/SECURITY.md
+-rw-r--r--   0     1001      127      117 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/.github/dependabot.yml
+-rw-r--r--   0     1001      127       76 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/.github/release.yml
+-rw-r--r--   0     1001      127     2248 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/.github/workflows/check.yml
+-rw-r--r--   0     1001      127     3801 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/.github/workflows/release.yml
+-rw-r--r--   0     1001      127      158 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/.gitignore
+-rw-r--r--   0     1001      127      973 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      240 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/.pre-commit-hooks.yaml
+-rw-r--r--   0     1001      127       16 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/.rustfmt.toml
+-rw-r--r--   0     1001      127     3256 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      127     1023 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/LICENSE.txt
+-rw-r--r--   0     1001      127      861 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/README.md
+-rw-r--r--   0     1001      127     3370 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/rust/src/build_system.rs
+-rw-r--r--   0     1001      127     3454 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/rust/src/global.rs
+-rw-r--r--   0     1001      127     8964 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/rust/src/helpers/array.rs
+-rw-r--r--   0     1001      127     4529 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/rust/src/helpers/create.rs
+-rw-r--r--   0     1001      127       78 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/rust/src/helpers/mod.rs
+-rw-r--r--   0     1001      127     4056 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/rust/src/helpers/pep508.rs
+-rw-r--r--   0     1001      127     1605 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/rust/src/helpers/string.rs
+-rw-r--r--   0     1001      127     9237 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/rust/src/helpers/table.rs
+-rw-r--r--   0     1001      127     5188 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/rust/src/main.rs
+-rw-r--r--   0     1001      127    29493 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/rust/src/project.rs
+-rw-r--r--   0     1001      127       29 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/rust-toolchain.toml
+-rw-r--r--   0     1001      127      161 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/src/pyproject_fmt_rust/__init__.py
+-rw-r--r--   0     1001      127      638 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/src/pyproject_fmt_rust/_lib.pyi
+-rw-r--r--   0     1001      127        0 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/src/pyproject_fmt_rust/py.typed
+-rw-r--r--   0     1001      127      991 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/tests/test_main.py
+-rw-r--r--   0     1001      127     2076 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/tox.ini
+-rw-r--r--   0     1001      127    26464 2024-05-11 05:31:15.000000 pyproject_fmt_rust-1.0.3/Cargo.lock
+-rw-r--r--   0     1001      127     3312 2024-05-11 05:30:58.000000 pyproject_fmt_rust-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 pyproject_fmt_rust-1.0.3/PKG-INFO
```

### Comparing `pyproject_fmt_rust-1.0.2/Cargo.toml` & `pyproject_fmt_rust-1.0.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyproject-fmt-rust"
-version = "1.0.2"
+version = "1.0.3"
 description = "Format pyproject.toml files"
 repository = "https://github.com/tox-dev/pyproject-fmt"
 readme = "README.md"
 license = "MIT"
 edition = "2021"
 
 [lib]
```

### Comparing `pyproject_fmt_rust-1.0.2/.github/workflows/check.yml` & `pyproject_fmt_rust-1.0.3/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/.github/workflows/release.yml` & `pyproject_fmt_rust-1.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/.pre-commit-config.yaml` & `pyproject_fmt_rust-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/CODE_OF_CONDUCT.md` & `pyproject_fmt_rust-1.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/LICENSE.txt` & `pyproject_fmt_rust-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/README.md` & `pyproject_fmt_rust-1.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,7 @@
 
 [![PyPI](https://img.shields.io/pypi/v/pyproject-fmt-rust?style=flat-square)](https://pypi.org/project/pyproject-fmt-rust)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/pyproject-fmt-rust?style=flat-square)](https://pypi.org/project/pyproject-fmt-rust)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyproject-fmt-rust?style=flat-square)](https://pypi.org/project/pyproject-fmt-rust)
 [![Downloads](https://static.pepy.tech/badge/pyproject-fmt-rust/month)](https://pepy.tech/project/pyproject-fmt-rust)
 [![PyPI - License](https://img.shields.io/pypi/l/pyproject-fmt-rust?style=flat-square)](https://opensource.org/licenses/MIT)
 [![check](https://github.com/tox-dev/pyproject-fmt-rust/actions/workflows/check.yml/badge.svg)](https://github.com/tox-dev/pyproject-fmt-rust/actions/workflows/check.yml)
-
-Apply a consistent format to `pyproject.toml` files.
-[Read the full documentation here](https://pyproject-fmt-rust.readthedocs.io/en/latest/).
-
-## add to pre-commit
-
-```yaml
-- repo: https://github.com/tox-dev/pyproject-fmt-rust
-  rev: "1.7.0"
-  hooks:
-    - id: pyproject-fmt-rust
-```
```

### Comparing `pyproject_fmt_rust-1.0.2/rust/src/build_system.rs` & `pyproject_fmt_rust-1.0.3/rust/src/build_system.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/rust/src/global.rs` & `pyproject_fmt_rust-1.0.3/rust/src/global.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/rust/src/helpers/array.rs` & `pyproject_fmt_rust-1.0.3/rust/src/helpers/array.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/rust/src/helpers/create.rs` & `pyproject_fmt_rust-1.0.3/rust/src/helpers/create.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/rust/src/helpers/pep508.rs` & `pyproject_fmt_rust-1.0.3/rust/src/helpers/pep508.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/rust/src/helpers/string.rs` & `pyproject_fmt_rust-1.0.3/rust/src/helpers/string.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/rust/src/helpers/table.rs` & `pyproject_fmt_rust-1.0.3/rust/src/helpers/table.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/rust/src/main.rs` & `pyproject_fmt_rust-1.0.3/rust/src/main.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/rust/src/project.rs` & `pyproject_fmt_rust-1.0.3/rust/src/project.rs`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/src/pyproject_fmt_rust/_lib.pyi` & `pyproject_fmt_rust-1.0.3/src/pyproject_fmt_rust/_lib.pyi`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/tests/test_main.py` & `pyproject_fmt_rust-1.0.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/tox.ini` & `pyproject_fmt_rust-1.0.3/tox.ini`

 * *Files identical despite different names*

### Comparing `pyproject_fmt_rust-1.0.2/Cargo.lock` & `pyproject_fmt_rust-1.0.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -516,15 +516,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyproject-fmt-rust"
-version = "1.0.2"
+version = "1.0.3"
 dependencies = [
  "indoc",
  "lexical-sort",
  "pep508_rs",
  "pyo3",
  "regex",
  "rstest",
```

### Comparing `pyproject_fmt_rust-1.0.2/pyproject.toml` & `pyproject_fmt_rust-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 dependencies = [
 ]
 optional-dependencies.test = [
   "covdefaults>=2.3",
   "pytest>=8.2",
   "pytest-cov>=5",
 ]
-urls."Bug Tracker" = "https://github.com/tox-dev/pyproject-fmt-rust-rust/issues"
+urls."Bug Tracker" = "https://github.com/tox-dev/pyproject-fmt-rust/issues"
 urls."Changelog" = "https://github.com/tox-dev/pyproject-fmt-rust/releases"
 urls.Documentation = "https://github.com/tox-dev/pyproject-fmt-rust/"
 urls."Source Code" = "https://github.com/tox-dev/pyproject-fmt-rust"
 
 [tool.maturin]
 bindings = "pyo3"
 manifest-path = "Cargo.toml"
```

### Comparing `pyproject_fmt_rust-1.0.2/PKG-INFO` & `pyproject_fmt_rust-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyproject-fmt-rust
-Version: 1.0.2
+Version: 1.0.3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,33 +17,21 @@
 License-File: LICENSE.txt
 Summary: Format your pyproject.toml file
 Keywords: format,pyproject
 Author-email: Bernat Gabor <gaborjbernat@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Bug Tracker, https://github.com/tox-dev/pyproject-fmt-rust-rust/issues
+Project-URL: Bug Tracker, https://github.com/tox-dev/pyproject-fmt-rust/issues
 Project-URL: Changelog, https://github.com/tox-dev/pyproject-fmt-rust/releases
 Project-URL: Documentation, https://github.com/tox-dev/pyproject-fmt-rust/
 Project-URL: Source Code, https://github.com/tox-dev/pyproject-fmt-rust
 
 # pyproject-fmt-rust
 
 [![PyPI](https://img.shields.io/pypi/v/pyproject-fmt-rust?style=flat-square)](https://pypi.org/project/pyproject-fmt-rust)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/pyproject-fmt-rust?style=flat-square)](https://pypi.org/project/pyproject-fmt-rust)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyproject-fmt-rust?style=flat-square)](https://pypi.org/project/pyproject-fmt-rust)
 [![Downloads](https://static.pepy.tech/badge/pyproject-fmt-rust/month)](https://pepy.tech/project/pyproject-fmt-rust)
 [![PyPI - License](https://img.shields.io/pypi/l/pyproject-fmt-rust?style=flat-square)](https://opensource.org/licenses/MIT)
 [![check](https://github.com/tox-dev/pyproject-fmt-rust/actions/workflows/check.yml/badge.svg)](https://github.com/tox-dev/pyproject-fmt-rust/actions/workflows/check.yml)
 
-Apply a consistent format to `pyproject.toml` files.
-[Read the full documentation here](https://pyproject-fmt-rust.readthedocs.io/en/latest/).
-
-## add to pre-commit
-
-```yaml
-- repo: https://github.com/tox-dev/pyproject-fmt-rust
-  rev: "1.7.0"
-  hooks:
-    - id: pyproject-fmt-rust
-```
-
```

