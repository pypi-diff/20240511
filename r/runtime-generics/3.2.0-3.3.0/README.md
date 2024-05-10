# Comparing `tmp/runtime_generics-3.2.0.tar.gz` & `tmp/runtime_generics-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtime_generics-3.2.0.tar", max compression
+gzip compressed data, was "runtime_generics-3.3.0.tar", max compression
```

## Comparing `runtime_generics-3.2.0.tar` & `runtime_generics-3.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2024-04-14 00:43:43.672735 runtime_generics-3.2.0/LICENSE
--rw-r--r--   0        0        0     8137 2024-04-14 00:43:43.672735 runtime_generics-3.2.0/README.md
--rw-r--r--   0        0        0     5429 2024-04-14 00:43:43.676735 runtime_generics-3.2.0/pyproject.toml
--rw-r--r--   0        0        0    22205 2024-04-14 00:43:43.676735 runtime_generics-3.2.0/runtime_generics/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 00:43:43.676735 runtime_generics-3.2.0/runtime_generics/py.typed
--rw-r--r--   0        0        0     9195 1970-01-01 00:00:00.000000 runtime_generics-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-10 23:55:59.571493 runtime_generics-3.3.0/LICENSE
+-rw-r--r--   0        0        0     7973 2024-05-10 23:55:59.571493 runtime_generics-3.3.0/README.md
+-rw-r--r--   0        0        0     5675 2024-05-10 23:55:59.571493 runtime_generics-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0    22232 2024-05-10 23:55:59.571493 runtime_generics-3.3.0/runtime_generics/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:55:59.571493 runtime_generics-3.3.0/runtime_generics/py.typed
+-rw-r--r--   0        0        0     9021 1970-01-01 00:00:00.000000 runtime_generics-3.3.0/PKG-INFO
```

### Comparing `runtime_generics-3.2.0/LICENSE` & `runtime_generics-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runtime_generics-3.2.0/README.md` & `runtime_generics-3.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# <div align="center">runtime_generics<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–215–g792492f-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f) [![Supported Python versions](https://img.shields.io/pypi/pyversions/runtime-generics.svg?logo=python&label=Python)](https://pypi.org/project/runtime-generics/) [![Package version](https://img.shields.io/pypi/v/runtime-generics?label=PyPI)](https://pypi.org/project/runtime-generics/)</div>
+# <div align="center">runtime_generics<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–244–g52a2805-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-244-g52a2805) [![Supported Python versions](https://img.shields.io/pypi/pyversions/runtime-generics.svg?logo=python&label=Python)](https://pypi.org/project/runtime-generics/) [![Package version](https://img.shields.io/pypi/v/runtime-generics?label=PyPI)](https://pypi.org/project/runtime-generics/)</div>
 
 [![Tests](https://github.com/bswck/runtime_generics/actions/workflows/test.yml/badge.svg)](https://github.com/bswck/runtime_generics/actions/workflows/test.yml)
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/runtime_generics.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/runtime_generics)
-[![Documentation Status](https://readthedocs.org/projects/runtime-generics/badge/?version=latest)](https://runtime-generics.readthedocs.io/en/latest/?badge=latest)
 [![Lifted?](https://tidelift.com/badges/package/pypi/runtime-generics)](https://tidelift.com/subscription/pkg/pypi-runtime-generics?utm_source=pypi-runtime-generics&utm_medium=readme)
 
 Highly into type-safe Python code?
 
 _runtime_generics_ is a niche Python library that allows you to reuse type arguments explicitly passed at runtime
 to generic classes before instantiation.
 
@@ -135,17 +134,17 @@
 ```
 
 ## For Contributors
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 <!--
-This section was generated from skeleton-ci/skeleton-python@0.0.2rc-215-g792492f.
+This section was generated from skeleton-ci/skeleton-python@0.0.2rc-244-g52a2805.
 Instead of changing this particular file, you might want to alter the template:
-https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f/project/README.md.jinja
+https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-244-g52a2805/project/README.md.jinja
 -->
 > [!Note]
 > If you use Windows, it is highly recommended to complete the installation in the way presented below through [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install).
 1.  Fork the [runtime_generics repository](https://github.com/bswck/runtime_generics) on GitHub.
 
 1.  [Install Poetry](https://python-poetry.org/docs/#installation).<br/>
     Poetry is an amazing tool for managing dependencies & virtual environments, building packages and publishing them.
```

### Comparing `runtime_generics-3.2.0/pyproject.toml` & `runtime_generics-3.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-# This file was generated from skeleton-ci/skeleton-python@0.0.2rc-215-g792492f.
+# This file was generated from skeleton-ci/skeleton-python@0.0.2rc-244-g52a2805.
 # Instead of changing this particular file, you might want to alter the template:
-# https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f/project/pyproject.toml.jinja
+# https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-244-g52a2805/project/pyproject.toml.jinja
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "runtime_generics"
-version = "3.2.0"
+version = "3.3.0"
 description = "Reuse generic class type arguments at runtime."
 authors = ["bswck <bartoszpiotrslawecki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "runtime_generics/" }]
 homepage = "https://github.com/bswck/runtime_generics"
 
 [tool.poetry.urls]
-Documentation = "https://runtime-generics.readthedocs.io/en/latest/"
+Documentation = "https://bswck.github.io/runtime_generics"
 Issues = "https://github.com/bswck/runtime_generics/issues"
 Distribution = "https://pypi.org/project/runtime-generics/"
 Coverage = "https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/runtime_generics"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 typing-extensions = ">=4.9.0"
 backframe = ">=0.1.2"
 
 [tool.poetry.group.dev.dependencies]
 
 [tool.poetry.group.dev-skeleton.dependencies]
-# This dependency group was generated from skeleton-ci/skeleton-python@0.0.2rc-215-g792492f.
+# This dependency group was generated from skeleton-ci/skeleton-python@0.0.2rc-244-g52a2805.
 # Instead of changing this particular file, you might want to alter the template:
-# https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f/project/pyproject.toml.jinja
+# https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-244-g52a2805/project/pyproject.toml.jinja
 mypy = ">=1.9.0"
 ruff = ">=0.3.4"
 towncrier = ">=23.11.0"
 coverage = ">=7.4.4"
 pytest = ">=8.1.1"
 pytest-doctestplus = ">=1.2.1"
 pytest-sugar = ">=1.0.0"
@@ -41,27 +45,26 @@
 pre-commit = "<3.6.0"
 smokeshow = ">=0.4.0"
 keyring = ">=25.0.0"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 
-
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 markdown-exec = ">=1.3.0"
 mkdocs-material = ">=8.2,<10.0.0"
 mkdocstrings = { version = ">=0.19.0", extras = ["python"] }
 
 [tool.poe.tasks]
 test = "pytest -v"
 lint = "ruff check ."
-skeleton = "scripts/skeleton.0.0.2rc-215-g792492f.bash"
+skeleton = "scripts/skeleton.0.0.2rc-244-g52a2805.bash"
 check = [
     { ref="test" },
     { ref="lint" },
 ]
 release.script = "scripts.release:main"
 
 [tool.poe.tasks.added]
@@ -118,14 +121,22 @@
     # Description: Multi-line docstring summary should start at the second line
     # Rationale: Remove the warning -- D213 (multi-line-summary-second-line) preferred.
     "D212",
 
     # Description: Line contains TODO, consider resolving the issue
     # Rationale: Not appropriate for the project.
     "FIX002",
+
+    # Description: Implicitly concatenated string literals on one line
+    # Rationale: Allegedly conflicts with the formatter.
+    "ISC001",
+
+    # Description: Trailing comma missing
+    # Rationale: Allegedly conflicts with the formatter.
+    "COM812",
 ]
 
 [tool.ruff.lint.isort]
 required-imports = ["from __future__ import annotations"]
 
 [tool.mypy]
 strict = true
@@ -172,11 +183,7 @@
 [tool.coverage.run]
 plugins = ["covdefaults"]
 source = ["runtime_generics/"]
 relative_files = true
 
 [tool.coverage.report]
 fail_under = 90
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
```

### Comparing `runtime_generics-3.2.0/runtime_generics/__init__.py` & `runtime_generics-3.3.0/runtime_generics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: MIT
 # (C) 2024-present Bartosz Sławecki (bswck)
 """
-`runtime_generics`.
+Reuse generic class type arguments at runtime.
 
 This library provides a decorator that allows you to mark a class as
 a 'runtime generic': after instantiation, the class will have a `__args__` attribute
 that contains the type arguments of the instance.
 
 Examples
 --------
```

### Comparing `runtime_generics-3.2.0/PKG-INFO` & `runtime_generics-3.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtime_generics
-Version: 3.2.0
+Version: 3.3.0
 Summary: Reuse generic class type arguments at runtime.
 Home-page: https://github.com/bswck/runtime_generics
 License: MIT
 Author: bswck
 Author-email: bartoszpiotrslawecki@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -13,24 +13,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: backframe (>=0.1.2)
 Requires-Dist: typing-extensions (>=4.9.0)
 Project-URL: Coverage, https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/runtime_generics
-Project-URL: Documentation, https://runtime-generics.readthedocs.io/en/latest/
+Project-URL: Documentation, https://bswck.github.io/runtime_generics
 Project-URL: Distribution, https://pypi.org/project/runtime-generics/
 Project-URL: Issues, https://github.com/bswck/runtime_generics/issues
 Description-Content-Type: text/markdown
 
-# <div align="center">runtime_generics<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–215–g792492f-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f) [![Supported Python versions](https://img.shields.io/pypi/pyversions/runtime-generics.svg?logo=python&label=Python)](https://pypi.org/project/runtime-generics/) [![Package version](https://img.shields.io/pypi/v/runtime-generics?label=PyPI)](https://pypi.org/project/runtime-generics/)</div>
+# <div align="center">runtime_generics<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–244–g52a2805-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-244-g52a2805) [![Supported Python versions](https://img.shields.io/pypi/pyversions/runtime-generics.svg?logo=python&label=Python)](https://pypi.org/project/runtime-generics/) [![Package version](https://img.shields.io/pypi/v/runtime-generics?label=PyPI)](https://pypi.org/project/runtime-generics/)</div>
 
 [![Tests](https://github.com/bswck/runtime_generics/actions/workflows/test.yml/badge.svg)](https://github.com/bswck/runtime_generics/actions/workflows/test.yml)
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/runtime_generics.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/runtime_generics)
-[![Documentation Status](https://readthedocs.org/projects/runtime-generics/badge/?version=latest)](https://runtime-generics.readthedocs.io/en/latest/?badge=latest)
 [![Lifted?](https://tidelift.com/badges/package/pypi/runtime-generics)](https://tidelift.com/subscription/pkg/pypi-runtime-generics?utm_source=pypi-runtime-generics&utm_medium=readme)
 
 Highly into type-safe Python code?
 
 _runtime_generics_ is a niche Python library that allows you to reuse type arguments explicitly passed at runtime
 to generic classes before instantiation.
 
@@ -159,17 +158,17 @@
 ```
 
 ## For Contributors
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 <!--
-This section was generated from skeleton-ci/skeleton-python@0.0.2rc-215-g792492f.
+This section was generated from skeleton-ci/skeleton-python@0.0.2rc-244-g52a2805.
 Instead of changing this particular file, you might want to alter the template:
-https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f/project/README.md.jinja
+https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-244-g52a2805/project/README.md.jinja
 -->
 > [!Note]
 > If you use Windows, it is highly recommended to complete the installation in the way presented below through [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install).
 1.  Fork the [runtime_generics repository](https://github.com/bswck/runtime_generics) on GitHub.
 
 1.  [Install Poetry](https://python-poetry.org/docs/#installation).<br/>
     Poetry is an amazing tool for managing dependencies & virtual environments, building packages and publishing them.
```

