# Comparing `tmp/pytest-discord-0.1.6.tar.gz` & `tmp/pytest_discord-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-discord-0.1.6.tar", last modified: Wed Oct 18 13:25:59 2023, max compression
+gzip compressed data, was "pytest_discord-0.2.0.tar", last modified: Sat May 11 14:39:06 2024, max compression
```

## Comparing `pytest-discord-0.1.6.tar` & `pytest_discord-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,44 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-10-18 13:25:59.218060 pytest-discord-0.1.6/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:14:09.000000 pytest-discord-0.1.6/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      185 2021-03-20 04:14:09.000000 pytest-discord-0.1.6/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     7664 2023-10-18 13:25:59.218060 pytest-discord-0.1.6/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     5833 2023-10-18 13:18:04.000000 pytest-discord-0.1.6/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)     1236 2023-10-18 13:10:30.000000 pytest-discord-0.1.6/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-10-18 13:25:59.208060 pytest-discord-0.1.6/pytest_discord/
--rw-r--r--   0 toor      (1000) toor      (1000)       88 2021-03-20 04:14:09.000000 pytest-discord-0.1.6/pytest_discord/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-10-18 13:18:35.000000 pytest-discord-0.1.6/pytest_discord/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1913 2023-05-27 13:01:00.000000 pytest-discord-0.1.6/pytest_discord/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3120 2023-07-15 14:52:47.000000 pytest-discord-0.1.6/pytest_discord/_opt_retriever.py
--rw-r--r--   0 toor      (1000) toor      (1000)    13797 2023-10-18 11:53:46.000000 pytest-discord-0.1.6/pytest_discord/plugin.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-10-18 13:25:59.208060 pytest-discord-0.1.6/pytest_discord.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     7664 2023-10-18 13:25:59.000000 pytest-discord-0.1.6/pytest_discord.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      573 2023-10-18 13:25:59.000000 pytest-discord-0.1.6/pytest_discord.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-10-18 13:25:59.000000 pytest-discord-0.1.6/pytest_discord.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       50 2023-10-18 13:25:59.000000 pytest-discord-0.1.6/pytest_discord.egg-info/entry_points.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-10-18 13:25:39.000000 pytest-discord-0.1.6/pytest_discord.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)      142 2023-10-18 13:25:59.000000 pytest-discord-0.1.6/pytest_discord.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       15 2023-10-18 13:25:59.000000 pytest-discord-0.1.6/pytest_discord.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-10-18 13:25:59.218060 pytest-discord-0.1.6/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)      159 2023-10-18 09:32:01.000000 pytest-discord-0.1.6/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        5 2021-03-20 04:14:09.000000 pytest-discord-0.1.6/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-10-18 13:25:59.218060 pytest-discord-0.1.6/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2857 2023-10-18 13:09:38.000000 pytest-discord-0.1.6/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-10-18 13:25:59.218060 pytest-discord-0.1.6/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)       30 2021-03-20 04:14:09.000000 pytest-discord-0.1.6/tests/conftest.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4423 2023-02-05 14:10:17.000000 pytest-discord-0.1.6/tests/test_plugin.py
--rw-r--r--   0 toor      (1000) toor      (1000)      923 2023-10-18 13:09:25.000000 pytest-discord-0.1.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:39:06.429591 pytest_discord-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:39:06.421591 pytest_discord-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:39:06.421591 pytest_discord-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-05-11 14:39:06.425591 pytest_discord-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:39:06.421591 pytest_discord-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/examples/test_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/examples/test_skipped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/examples/test_xfailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/examples/test_xpassed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:39:06.425591 pytest_discord-0.2.0/pytest_discord/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/pytest_discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/pytest_discord/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/pytest_discord/_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/pytest_discord/_opt_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14177 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/pytest_discord/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:39:06.425591 pytest_discord-0.2.0/pytest_discord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-05-11 14:39:06.000000 pytest_discord-0.2.0/pytest_discord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-11 14:39:06.000000 pytest_discord-0.2.0/pytest_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:39:06.000000 pytest_discord-0.2.0/pytest_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-11 14:39:06.000000 pytest_discord-0.2.0/pytest_discord.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:38:51.000000 pytest_discord-0.2.0/pytest_discord.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-11 14:39:06.000000 pytest_discord-0.2.0/pytest_discord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 14:39:06.000000 pytest_discord-0.2.0/pytest_discord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:39:06.425591 pytest_discord-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/requirements/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 14:39:06.429591 pytest_discord-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:39:06.425591 pytest_discord-0.2.0/ss/
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/ss/pytest-discord.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25658 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/ss/pytest-discord_verbose.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:39:06.425591 pytest_discord-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-11 14:38:35.000000 pytest_discord-0.2.0/tox.ini
```

### Comparing `pytest-discord-0.1.6/LICENSE` & `pytest_discord-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-discord-0.1.6/PKG-INFO` & `pytest_discord-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,77 +1,82 @@
 Metadata-Version: 2.1
 Name: pytest-discord
-Version: 0.1.6
+Version: 0.2.0
 Summary: A pytest plugin to notify test results to a Discord channel.
 Home-page: https://github.com/thombashi/pytest-discord
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
-Project-URL: Changlog, https://github.com/thombashi/pytest-discord/releases
+Project-URL: Changelog, https://github.com/thombashi/pytest-discord/releases
 Project-URL: Source, https://github.com/thombashi/pytest-discord
 Project-URL: Tracker, https://github.com/thombashi/pytest-discord/issues
 Keywords: discord,plugin,pytest
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: aiohttp<4,>=3.6
-Requires-Dist: discord.py<2,>=1.0.1
+Requires-Dist: discord.py<3,>=2
 Requires-Dist: pathvalidate<4,>=2.5.2
-Requires-Dist: pytest!=6.0.0,<8,>=3.3.2
-Requires-Dist: pytest-md-report<1,>=0.5.0
+Requires-Dist: pytest!=6.0.0,<9,>=3.3.2
+Requires-Dist: pytest-md-report<1,>=0.6.1
 Requires-Dist: typepy<2,>=1.1.4
 Provides-Extra: test
 Requires-Dist: mock; extra == "test"
 
 .. contents:: **pytest-discord**
    :backlinks: top
    :depth: 2
 
 
 Summary
 ============================================
-.. image:: https://badge.fury.io/py/pytest-discord.svg
+|PyPI pkg ver| |Supported Python ver| |Supported Python impl| |CI status| |Test coverage| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/pytest-discord.svg
     :target: https://badge.fury.io/py/pytest-discord
     :alt: PyPI package version
 
-.. image:: https://img.shields.io/pypi/pyversions/pytest-discord.svg
+.. |Supported Python impl| image:: https://img.shields.io/pypi/implementation/pytest-discord.svg
     :target: https://pypi.org/project/pytest-discord
-    :alt: Supported Python versions
+    :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/implementation/pytest-discord.svg
+.. |Supported Python ver| image:: https://img.shields.io/pypi/pyversions/pytest-discord.svg
     :target: https://pypi.org/project/pytest-discord
-    :alt: Supported Python implementations
+    :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/pytest-discord/actions/workflows/ci.yml/badge.svg
+.. |CI status| image:: https://github.com/thombashi/pytest-discord/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/thombashi/pytest-discord/actions/workflows/ci.yml
     :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://coveralls.io/repos/github/thombashi/pytest-discord/badge.svg?branch=master
+.. |Test coverage| image:: https://coveralls.io/repos/github/thombashi/pytest-discord/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/pytest-discord?branch=master
     :alt: Test coverage: coveralls
 
+.. |CodeQL| image:: https://github.com/thombashi/pytest-discord/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/pytest-discord/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
 A pytest plugin to notify test results to a Discord channel.
 
 
 Installation
 ============================================
 ::
 
@@ -187,9 +192,9 @@
         [tool:pytest]
         discord_webhook = https://discordapp.com/api/webhooks/...
         md_report_verbose = 1
 
 
 Dependencies
 ============================================
-- Python 3.7+
+- Python 3.8+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytest-discord/network/dependencies>`__
```

### Comparing `pytest-discord-0.1.6/README.rst` & `pytest_discord-0.2.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 .. contents:: **pytest-discord**
    :backlinks: top
    :depth: 2
 
 
 Summary
 ============================================
-.. image:: https://badge.fury.io/py/pytest-discord.svg
+|PyPI pkg ver| |Supported Python ver| |Supported Python impl| |CI status| |Test coverage| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/pytest-discord.svg
     :target: https://badge.fury.io/py/pytest-discord
     :alt: PyPI package version
 
-.. image:: https://img.shields.io/pypi/pyversions/pytest-discord.svg
+.. |Supported Python impl| image:: https://img.shields.io/pypi/implementation/pytest-discord.svg
     :target: https://pypi.org/project/pytest-discord
-    :alt: Supported Python versions
+    :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/implementation/pytest-discord.svg
+.. |Supported Python ver| image:: https://img.shields.io/pypi/pyversions/pytest-discord.svg
     :target: https://pypi.org/project/pytest-discord
-    :alt: Supported Python implementations
+    :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/pytest-discord/actions/workflows/ci.yml/badge.svg
+.. |CI status| image:: https://github.com/thombashi/pytest-discord/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/thombashi/pytest-discord/actions/workflows/ci.yml
     :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://coveralls.io/repos/github/thombashi/pytest-discord/badge.svg?branch=master
+.. |Test coverage| image:: https://coveralls.io/repos/github/thombashi/pytest-discord/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/pytest-discord?branch=master
     :alt: Test coverage: coveralls
 
+.. |CodeQL| image:: https://github.com/thombashi/pytest-discord/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/pytest-discord/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
 A pytest plugin to notify test results to a Discord channel.
 
 
 Installation
 ============================================
 ::
 
@@ -144,9 +150,9 @@
         [tool:pytest]
         discord_webhook = https://discordapp.com/api/webhooks/...
         md_report_verbose = 1
 
 
 Dependencies
 ============================================
-- Python 3.7+
+- Python 3.8+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytest-discord/network/dependencies>`__
```

### Comparing `pytest-discord-0.1.6/pyproject.toml` & `pytest_discord-0.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["setuptools>=61.0"]
+requires = [
+  "setuptools>=64",
+  "setuptools_scm>=8",
+]
 
-[tool.black]
-exclude = '''
-/(
-      \.eggs
-    | \.git
-    | \.mypy_cache
-    | \.tox
-    | \.venv
-    | \.pytype
-    | _build
-    | buck-out
-    | build
-    | dist
-)/
-| docs/conf.py
-'''
-line-length = 100
-target-version = ['py37', 'py38', 'py39', 'py310', 'py311', 'py312']
+[tool.setuptools_scm]
+version_scheme = "guess-next-dev"
+local_scheme = "no-local-version"
 
 [tool.coverage.run]
 branch = true
 source = ['pytest_discord']
 
 [tool.coverage.report]
 exclude_lines = [
   'except ImportError',
   'raise NotImplementedError',
   'pass',
   'ABCmeta',
   'abstractmethod',
-  'abstractproperty',
-  'abstractclassmethod',
   'warnings.warn',
 ]
 precision = 1
 show_missing = true
 
 [tool.isort]
 include_trailing_comma = true
@@ -51,15 +37,15 @@
   '*/.eggs/*',
   '*/.pytype/*',
   '*/.tox/*',
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
-python_version = 3.7
+python_version = 3.8
 
 pretty = true
 
 check_untyped_defs = true
 no_implicit_optional = true
 show_error_codes = true
 show_error_context = true
@@ -70,7 +56,31 @@
 
 [tool.pytest.ini_options]
 testpaths = [
   "tests",
 ]
 
 discord_verbose = 1
+
+[tool.pyright]
+exclude = [
+    "**/node_modules",
+    "**/__pycache__",
+    ".tox",
+    ".venv",
+    "_build",
+    "_sandbox",
+    "build",
+    "dist"
+]
+pythonVersion = "3.8"
+
+[tool.ruff]
+line-length = 100
+target-version = "py38"
+exclude = [
+    ".eggs/",
+    ".tox/",
+    "_sandbox/*",
+    "build/",
+    "docs/conf.py",
+]
```

### Comparing `pytest-discord-0.1.6/pytest_discord/_const.py` & `pytest_discord-0.2.0/pytest_discord/_const.py`

 * *Files identical despite different names*

### Comparing `pytest-discord-0.1.6/pytest_discord/_opt_retriever.py` & `pytest_discord-0.2.0/pytest_discord/_opt_retriever.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,30 +72,43 @@
 
         if value is None:
             value = config.getini(discord_opt.inioption_str)
 
         if value is None:
             return False
 
-        return value
+        try:
+            return Bool(value, strict_level=StrictLevel.MIN).convert()
+        except TypeConversionError:
+            pass
+
+        return False
 
     def __retrieve_discord_opt(self, discord_opt: Option) -> Optional[str]:
         config = self.__config
         value = None
 
         if hasattr(config.option, discord_opt.inioption_str):
             value = getattr(config.option, discord_opt.inioption_str)
 
         if not value:
             value = os.environ.get(discord_opt.envvar_str)
 
         if not value:
             value = config.getini(discord_opt.inioption_str)
 
-        return value
+        if value is None:
+            return None
+
+        if isinstance(value, str):
+            return value
+
+        raise RuntimeError(
+            f"unexpected value type: expected=Option[str], actual={type(value)}, value={value}"
+        )
 
     @staticmethod
     def _to_int(value: Any) -> Optional[int]:
         try:
             return Integer(value, strict_level=StrictLevel.MIN).convert()
         except TypeConversionError:
             return None
```

### Comparing `pytest-discord-0.1.6/pytest_discord/plugin.py` & `pytest_discord-0.2.0/pytest_discord/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from typing import Dict, List, Mapping, Optional, Sequence, Tuple
 
 import aiohttp
 import pytest
 from _pytest.config import Config
 from _pytest.config.argparsing import Parser
 from _pytest.terminal import TerminalReporter
-from discord import AsyncWebhookAdapter, Colour, Embed, File, Webhook
-from discord.errors import Forbidden, HTTPException, InvalidArgument, NotFound
+from discord import Colour, Embed, File, Webhook
+from discord.errors import Forbidden, HTTPException, NotFound
+from discord.utils import MISSING
 from pytablewriter.writer.text import MarkdownFlavor
 from pytest_md_report.plugin import extract_pytest_stats
 
 from ._const import HelpMsg, Option, TestResultType
 from ._opt_retriever import DiscordOptRetriever
 
 
@@ -188,14 +189,15 @@
             embed = Embed(
                 description="# {}: #{}\n{}".format(
                     stat_key, i + 1, _decorate_code_block(lang="py", text="\n".join(lines))
                 ),
                 colour=colour,
             )
 
+            assert embed.description is not None
             if (total_embed_len + len(embed.description)) > (MAX_EMBEDS_LEN - 128):
                 embeds.append(
                     Embed(description=f"and other {len(values) - i} failed", colour=colour)
                 )
                 exceeds_embeds_limit = True
                 break
 
@@ -212,33 +214,34 @@
     CI = os.environ.get("CI")
     if not CI:
         return False
 
     return CI.strip().lower() == "true"
 
 
-def _make_md_report(config: Config) -> str:
+def _make_md_report(config: Config, reporter: TerminalReporter) -> str:
     from pytest_md_report import ColorPolicy, ZerosRender, make_md_report, retrieve_stat_count_map
 
     opt_retriever = DiscordOptRetriever(config)
     verbosity_level = opt_retriever.retrieve_verbosity_level()
-    reporter = config.pluginmanager.get_plugin("terminalreporter")
     stat_count_map = retrieve_stat_count_map(reporter)
 
     stash_md_report_color = (
         config.option.md_report_color if hasattr(config.option, "md_report_color") else None
     )
     stash_md_report_zeros = (
         config.option.md_report_zeros if hasattr(config.option, "md_report_zeros") else None
     )
 
     if not hasattr(config.option, "md_report_verbose"):
         config.option.md_report_verbose = max(0, verbosity_level - 1)
     if not hasattr(config.option, "md_report_margin"):
         config.option.md_report_margin = 1
+    if not hasattr(config.option, "md_report_exclude_outcomes"):
+        config.option.md_report_exclude_outcomes = []
 
     try:
         config.option.md_report_color = ColorPolicy.NEVER
         config.option.md_report_zeros = ZerosRender.EMPTY
 
         return make_md_report(
             config,
@@ -319,15 +322,18 @@
     opt_retriever = DiscordOptRetriever(config)
     url = opt_retriever.retrieve_webhook_url()
     if not url:
         return
 
     verbosity_level = opt_retriever.retrieve_verbosity_level()
     reporter = config.pluginmanager.get_plugin("terminalreporter")
-    md_report = _make_md_report(config)
+    if reporter is None:
+        return
+
+    md_report = _make_md_report(config, reporter)
 
     try:
         duration = time.time() - reporter._sessionstarttime
     except AttributeError:
         return
 
     message, stat_count_map = _make_results_message(reporter)
@@ -348,15 +354,17 @@
     embeds: List[Embed] = []
     embeds_len_ct = 0
     exceeds_embeds_limit = False
 
     embed_summary = Embed(description=f"{message} in {duration:.1f} seconds", colour=colour)
     embed_summary.set_footer(text=_make_summary_footer(reporter, verbosity_level))
     embeds.append(embed_summary)
-    embeds_len_ct += len(embed_summary.description) + len(embed_summary.footer)
+    assert embed_summary.description is not None
+    assert embed_summary.footer.text is not None
+    embeds_len_ct += len(embed_summary.description) + len(embed_summary.footer.text)
 
     if verbosity_level >= 1:
         pytest_stats = extract_pytest_stats(
             reporter=reporter,
             outcomes=["passed", "failed", "error", "skipped", "xfailed", "xpassed"],
             verbosity_level=max(0, verbosity_level - 1),
         )
@@ -372,14 +380,15 @@
 
         for result_type, result_lines in result_lines_map.items():
             embed = Embed(
                 description="\n".join(result_lines)[:MAX_EMBED_LEN],
                 colour=_result_type_to_colour[result_type],
             )
             embeds.append(embed)
+            assert embed.description is not None
             embeds_len_ct += len(embed.description)
 
         _embeds, exceeds_embeds_limit = _extract_longrepr_embeds(
             reporter, embeds_len_ct, colour=colour
         )
         embeds.extend(_embeds)
 
@@ -411,28 +420,33 @@
     )
 
 
 async def _send_message(
     reporter: TerminalReporter,
     url: str,
     header: str,
-    username: Optional[str],
+    username: str,
     avatar_url: Optional[str],
     embeds: Sequence[Embed],
     attach_file: Optional[File] = None,
 ) -> None:
+    if attach_file:
+        afile = attach_file
+    else:
+        afile = MISSING
+
     async with aiohttp.ClientSession() as session:
         try:
-            webhook = Webhook.from_url(url, adapter=AsyncWebhookAdapter(session))
-        except (InvalidArgument, HTTPException, NotFound, Forbidden) as e:
+            webhook = Webhook.from_url(url, session=session)
+        except (TypeError, ValueError, HTTPException, NotFound, Forbidden) as e:
             reporter.write_line(f"pytest-discord error: {str(e)}")
             return
 
         await webhook.send(
-            header, username=username, avatar_url=avatar_url, embeds=embeds, file=attach_file
+            header, username=username, avatar_url=avatar_url, embeds=embeds, file=afile
         )
 
 
 @pytest.hookimpl()
 def pytest_report_teststatus(report):
     if report.longreprtext:
         _logs.append(report.longreprtext)
```

### Comparing `pytest-discord-0.1.6/pytest_discord.egg-info/PKG-INFO` & `pytest_discord-0.2.0/pytest_discord.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,77 +1,82 @@
 Metadata-Version: 2.1
 Name: pytest-discord
-Version: 0.1.6
+Version: 0.2.0
 Summary: A pytest plugin to notify test results to a Discord channel.
 Home-page: https://github.com/thombashi/pytest-discord
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
-Project-URL: Changlog, https://github.com/thombashi/pytest-discord/releases
+Project-URL: Changelog, https://github.com/thombashi/pytest-discord/releases
 Project-URL: Source, https://github.com/thombashi/pytest-discord
 Project-URL: Tracker, https://github.com/thombashi/pytest-discord/issues
 Keywords: discord,plugin,pytest
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: aiohttp<4,>=3.6
-Requires-Dist: discord.py<2,>=1.0.1
+Requires-Dist: discord.py<3,>=2
 Requires-Dist: pathvalidate<4,>=2.5.2
-Requires-Dist: pytest!=6.0.0,<8,>=3.3.2
-Requires-Dist: pytest-md-report<1,>=0.5.0
+Requires-Dist: pytest!=6.0.0,<9,>=3.3.2
+Requires-Dist: pytest-md-report<1,>=0.6.1
 Requires-Dist: typepy<2,>=1.1.4
 Provides-Extra: test
 Requires-Dist: mock; extra == "test"
 
 .. contents:: **pytest-discord**
    :backlinks: top
    :depth: 2
 
 
 Summary
 ============================================
-.. image:: https://badge.fury.io/py/pytest-discord.svg
+|PyPI pkg ver| |Supported Python ver| |Supported Python impl| |CI status| |Test coverage| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/pytest-discord.svg
     :target: https://badge.fury.io/py/pytest-discord
     :alt: PyPI package version
 
-.. image:: https://img.shields.io/pypi/pyversions/pytest-discord.svg
+.. |Supported Python impl| image:: https://img.shields.io/pypi/implementation/pytest-discord.svg
     :target: https://pypi.org/project/pytest-discord
-    :alt: Supported Python versions
+    :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/implementation/pytest-discord.svg
+.. |Supported Python ver| image:: https://img.shields.io/pypi/pyversions/pytest-discord.svg
     :target: https://pypi.org/project/pytest-discord
-    :alt: Supported Python implementations
+    :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/pytest-discord/actions/workflows/ci.yml/badge.svg
+.. |CI status| image:: https://github.com/thombashi/pytest-discord/actions/workflows/ci.yml/badge.svg
     :target: https://github.com/thombashi/pytest-discord/actions/workflows/ci.yml
     :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://coveralls.io/repos/github/thombashi/pytest-discord/badge.svg?branch=master
+.. |Test coverage| image:: https://coveralls.io/repos/github/thombashi/pytest-discord/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/pytest-discord?branch=master
     :alt: Test coverage: coveralls
 
+.. |CodeQL| image:: https://github.com/thombashi/pytest-discord/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/pytest-discord/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
 A pytest plugin to notify test results to a Discord channel.
 
 
 Installation
 ============================================
 ::
 
@@ -187,9 +192,9 @@
         [tool:pytest]
         discord_webhook = https://discordapp.com/api/webhooks/...
         md_report_verbose = 1
 
 
 Dependencies
 ============================================
-- Python 3.7+
+- Python 3.8+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/pytest-discord/network/dependencies>`__
```

### Comparing `pytest-discord-0.1.6/pytest_discord.egg-info/SOURCES.txt` & `pytest_discord-0.2.0/pytest_discord.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,33 @@
+.gitignore
 LICENSE
 MANIFEST.in
+Makefile
 README.rst
 pyproject.toml
 setup.py
 tox.ini
+.github/dependabot.yml
+.github/workflows/ci.yml
+.github/workflows/release.yml
+examples/test_pass.py
+examples/test_skipped.py
+examples/test_xfailed.py
+examples/test_xpassed.py
 pytest_discord/__init__.py
 pytest_discord/__version__.py
 pytest_discord/_const.py
 pytest_discord/_opt_retriever.py
 pytest_discord/plugin.py
 pytest_discord.egg-info/PKG-INFO
 pytest_discord.egg-info/SOURCES.txt
 pytest_discord.egg-info/dependency_links.txt
 pytest_discord.egg-info/entry_points.txt
 pytest_discord.egg-info/not-zip-safe
 pytest_discord.egg-info/requires.txt
 pytest_discord.egg-info/top_level.txt
 requirements/requirements.txt
 requirements/test_requirements.txt
+ss/pytest-discord.png
+ss/pytest-discord_verbose.png
 tests/conftest.py
 tests/test_plugin.py
```

### Comparing `pytest-discord-0.1.6/setup.py` & `pytest_discord-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,44 +32,42 @@
 
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
     TESTS_REQUIRES = [line.strip() for line in f if line.strip()]
 
 
 setuptools.setup(
     name=MODULE_NAME,
-    version=pkg_info["__version__"],
     url=REPOSITORY_URL,
     author=pkg_info["__author__"],
     author_email=pkg_info["__email__"],
     description="A pytest plugin to notify test results to a Discord channel.",
     include_package_data=True,
     keywords=["discord", "plugin", "pytest"],
     license=pkg_info["__license__"],
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
     package_data={MODULE_NAME: ["py.typed"]},
     project_urls={
-        "Changlog": f"{REPOSITORY_URL:s}/releases",
+        "Changelog": f"{REPOSITORY_URL:s}/releases",
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=INSTALL_REQUIRES,
     extras_require={"test": TESTS_REQUIRES},
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Plugins",
         "Framework :: Pytest",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `pytest-discord-0.1.6/tests/test_plugin.py` & `pytest_discord-0.2.0/tests/test_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,17 +136,15 @@
     ],
 )
 def test_pytest_discord_avatar_url(testdir, value, expected):
     testdir.makepyfile(
         """
         def test_avatar_url():
             assert {}
-        """.format(
-            value
-        )
+        """.format(value)
     )
 
     with mock.patch("discord.Webhook.send", new_callable=AsyncMock) as mock_send:
         testdir.runpytest(
             "--discord-webhook",
             DUMMY_WEBHOOK_URL,
             "--discord-success-icon",
```

### Comparing `pytest-discord-0.1.6/tox.ini` & `pytest_discord-0.2.0/tox.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py{37,38,39,310,311,312}
+    py{38,39,310,311,312}
     pypy3
     build
     cov
     fmt
     lint
 
 [testenv]
@@ -17,15 +17,15 @@
 [testenv:build]
 deps =
     build>=1
     twine
     wheel
 commands =
     python -m build
-    twine check dist/*.whl dist/*.tar.gz
+    -twine check dist/*.whl dist/*.tar.gz
 
 [testenv:clean]
 skip_install = true
 deps =
     cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
@@ -40,22 +40,33 @@
     coverage run -m pytest {posargs:-vv}
     coverage report -m
 
 [testenv:fmt]
 skip_install = true
 deps =
     autoflake>=2
-    black>=23.1
     isort>=5
+    ruff>=0.3.5
 commands =
-    autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
+    autoflake --in-place --recursive --remove-all-unused-imports .
     isort .
-    black setup.py tests pytest_discord
+    ruff format
 
 [testenv:lint]
-skip_install = true
 deps =
+    codespell>=2
     mypy>=1
-    pylama>=8.4.1
+    releasecmd
+    ruff>=0.3.5
+    pyright>=1.1
 commands =
     mypy pytest_discord setup.py
-    pylama
+    pyright
+    ruff format --check
+    ruff check
+    -codespell . -q2 --check-filenames
+
+[testenv:release]
+deps =
+    releasecmd
+commands =
+    python setup.py release --sign --skip-uploading --verbose
```

