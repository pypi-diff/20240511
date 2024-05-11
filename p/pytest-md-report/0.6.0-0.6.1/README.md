# Comparing `tmp/pytest_md_report-0.6.0.tar.gz` & `tmp/pytest_md_report-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_md_report-0.6.0.tar", last modified: Fri May  3 16:05:19 2024, max compression
+gzip compressed data, was "pytest_md_report-0.6.1.tar", last modified: Sat May 11 12:15:11 2024, max compression
```

## Comparing `pytest_md_report-0.6.0.tar` & `pytest_md_report-0.6.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.709804 pytest_md_report-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.713804 pytest_md_report-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    18499 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16664 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.713804 pytest_md_report-0.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/gfm_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/report.md
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/test_failed.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/test_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/test_skipped.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/test_xfailed.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/examples/test_xpassed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.713804 pytest_md_report-0.6.0/pytest_md_report/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pytest_md_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pytest_md_report/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pytest_md_report/_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pytest_md_report/_style_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18684 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pytest_md_report/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/pytest_md_report/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/pytest_md_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18499 2024-05-03 16:05:19.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-03 16:05:19.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:05:19.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 16:05:19.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:05:08.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-03 16:05:19.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 16:05:19.000000 pytest_md_report-0.6.0/pytest_md_report.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/requirements/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/ss/
--rw-r--r--   0 runner    (1001) docker     (127)    75738 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/ss/md-report_exclude_outcomes_verbose_output.png
--rw-r--r--   0 runner    (1001) docker     (127)    61742 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/ss/md-report_gha.png
--rw-r--r--   0 runner    (1001) docker     (127)    21449 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/ss/pytest_md_report_example.png
--rw-r--r--   0 runner    (1001) docker     (127)    41954 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/ss/pytest_md_report_example_verbose.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:05:19.717804 pytest_md_report-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/tests/test_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-03 16:04:55.000000 pytest_md_report-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.659749 pytest_md_report-0.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.659749 pytest_md_report-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    18499 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16664 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.659749 pytest_md_report-0.6.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/gfm_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/test_failed.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/test_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/test_skipped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/test_xfailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/examples/test_xpassed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.659749 pytest_md_report-0.6.1/pytest_md_report/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pytest_md_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pytest_md_report/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pytest_md_report/_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pytest_md_report/_style_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18557 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pytest_md_report/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/pytest_md_report/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/pytest_md_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18499 2024-05-11 12:15:11.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-11 12:15:11.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:15:11.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-11 12:15:11.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:14:59.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-11 12:15:11.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-11 12:15:11.000000 pytest_md_report-0.6.1/pytest_md_report.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/requirements/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/ss/
+-rw-r--r--   0 runner    (1001) docker     (127)    75738 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/ss/md-report_exclude_outcomes_verbose_output.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61742 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/ss/md-report_gha.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21449 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/ss/pytest_md_report_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41954 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/ss/pytest_md_report_example_verbose.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:15:11.663749 pytest_md_report-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/tests/test_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-11 12:14:42.000000 pytest_md_report-0.6.1/tox.ini
```

### Comparing `pytest_md_report-0.6.0/.github/workflows/ci.yml` & `pytest_md_report-0.6.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/.github/workflows/release.yml` & `pytest_md_report-0.6.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/.gitignore` & `pytest_md_report-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/LICENSE` & `pytest_md_report-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/Makefile` & `pytest_md_report-0.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/PKG-INFO` & `pytest_md_report-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-md-report
-Version: 0.6.0
+Version: 0.6.1
 Summary: A pytest plugin to generate test outcomes reports with markdown table format.
 Home-page: https://github.com/thombashi/pytest-md-report
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Changlog, https://github.com/thombashi/pytest-md-report/releases
 Project-URL: Source, https://github.com/thombashi/pytest-md-report
```

### Comparing `pytest_md_report-0.6.0/README.rst` & `pytest_md_report-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/examples/gfm_report.md` & `pytest_md_report-0.6.1/examples/gfm_report.md`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/examples/report.md` & `pytest_md_report-0.6.1/examples/report.md`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/pyproject.toml` & `pytest_md_report-0.6.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -6,33 +6,14 @@
   "setuptools_scm>=8; python_version>='3.8'",
 ]
 
 [tool.setuptools_scm]
 version_scheme = "guess-next-dev"
 local_scheme = "no-local-version"
 
-[tool.black]
-line-length = 100
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
-target-version = ['py37', 'py38', 'py39', 'py310', 'py311', 'py312']
-
 [tool.isort]
 known_third_party = [
     "mock",
 ]
 include_trailing_comma = true
 line_length = 100
 lines_after_imports = 2
```

### Comparing `pytest_md_report-0.6.0/pytest_md_report/_const.py` & `pytest_md_report-0.6.1/pytest_md_report/_const.py`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/pytest_md_report/_style_filter.py` & `pytest_md_report-0.6.1/pytest_md_report/_style_filter.py`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/pytest_md_report/plugin.py` & `pytest_md_report-0.6.1/pytest_md_report/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,17 +453,17 @@
 def make_md_report(
     config: Config,
     reporter: TerminalReporter,
     total_stats: Mapping[str, int],
     color_policy: ColorPolicy,
     apply_ansi_escape: bool,
     md_flavor: MarkdownFlavor,
-    exclude_outcomes: List[str],
 ) -> str:
     verbosity_level = retrieve_verbosity_level(config)
+    exclude_outcomes = retrieve_exclude_outcomes(config)
 
     outcomes = ["passed", "failed", "error", "skipped", "xfailed", "xpassed"]
     outcomes = [key for key in outcomes if key not in exclude_outcomes]
     outcomes = [key for key in outcomes if total_stats.get(key, 0) > 0]
 
     if not outcomes:
         return ""
@@ -547,15 +547,14 @@
         return
 
     stat_count_map = retrieve_stat_count_map(reporter)
     is_tee = retrieve_tee(config)
     output_filepath = retrieve_output_filepath(config)
     color_policy = retrieve_color_policy(config)
     md_flavor = retrieve_md_flavor(config)
-    exclude_outcomes = retrieve_exclude_outcomes(config)
 
     is_output_term = is_tee or not output_filepath
     is_output_file = is_not_null_string(output_filepath)
     term_color_policy = color_policy
     file_color_policy = extract_file_color_policy(color_policy, is_output_file, md_flavor)
 
     apply_ansi_escape_to_file = is_apply_ansi_escape_to_file(color_policy, is_output_file)
@@ -565,15 +564,14 @@
         term_report = make_md_report(
             config,
             reporter,
             stat_count_map,
             color_policy=term_color_policy,
             apply_ansi_escape=apply_ansi_escape_to_term,
             md_flavor=md_flavor,
-            exclude_outcomes=exclude_outcomes,
         )
         reporter._tw.write(term_report)
 
     if not is_output_file:
         return
 
     file_report = term_report
@@ -588,14 +586,13 @@
         file_report = make_md_report(
             config,
             reporter,
             stat_count_map,
             color_policy=file_color_policy,
             apply_ansi_escape=apply_ansi_escape_to_file,
             md_flavor=md_flavor,
-            exclude_outcomes=exclude_outcomes,
         )
 
     if file_report:
         assert output_filepath
         with open(output_filepath, "w") as f:
             f.write(file_report)
```

### Comparing `pytest_md_report-0.6.0/pytest_md_report.egg-info/PKG-INFO` & `pytest_md_report-0.6.1/pytest_md_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-md-report
-Version: 0.6.0
+Version: 0.6.1
 Summary: A pytest plugin to generate test outcomes reports with markdown table format.
 Home-page: https://github.com/thombashi/pytest-md-report
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Changlog, https://github.com/thombashi/pytest-md-report/releases
 Project-URL: Source, https://github.com/thombashi/pytest-md-report
```

### Comparing `pytest_md_report-0.6.0/pytest_md_report.egg-info/SOURCES.txt` & `pytest_md_report-0.6.1/pytest_md_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/setup.py` & `pytest_md_report-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/ss/md-report_exclude_outcomes_verbose_output.png` & `pytest_md_report-0.6.1/ss/md-report_exclude_outcomes_verbose_output.png`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/ss/md-report_gha.png` & `pytest_md_report-0.6.1/ss/md-report_gha.png`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/ss/pytest_md_report_example.png` & `pytest_md_report-0.6.1/ss/pytest_md_report_example.png`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/ss/pytest_md_report_example_verbose.png` & `pytest_md_report-0.6.1/ss/pytest_md_report_example_verbose.png`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/tests/test_option.py` & `pytest_md_report-0.6.1/tests/test_option.py`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/tests/test_plugin.py` & `pytest_md_report-0.6.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_md_report-0.6.0/tox.ini` & `pytest_md_report-0.6.1/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -24,25 +24,14 @@
 [testenv:clean]
 skip_install = true
 deps =
     cleanpy>=0.4
 commands =
     cleanpy --all --exclude-envs .
 
-[testenv:fmt-black]
-skip_install = true
-deps =
-    autoflake>=2
-    black>=24.1
-    isort>=5
-commands =
-    autoflake --in-place --recursive --remove-all-unused-imports .
-    isort .
-    black setup.py examples tests pytest_md_report
-
 [testenv:fmt]
 skip_install = true
 deps =
     autoflake>=2
     isort>=5
     ruff>=0.3.5
 commands =
```

