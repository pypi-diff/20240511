# Comparing `tmp/poetry_plugin_export-1.7.1.tar.gz` & `tmp/poetry_plugin_export-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_export-1.7.1.tar", max compression
+gzip compressed data, was "poetry_plugin_export-1.8.0.tar", max compression
```

## Comparing `poetry_plugin_export-1.7.1.tar` & `poetry_plugin_export-1.8.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1062 2024-03-19 20:07:41.714429 poetry_plugin_export-1.7.1/LICENSE
--rw-r--r--   0        0        0     1976 2024-03-19 20:07:41.714429 poetry_plugin_export-1.7.1/README.md
--rw-r--r--   0        0        0     2680 2024-03-19 20:07:41.714429 poetry_plugin_export-1.7.1/pyproject.toml
--rw-r--r--   0        0        0      168 2024-03-19 20:07:41.714429 poetry_plugin_export-1.7.1/src/poetry_plugin_export/__init__.py
--rw-r--r--   0        0        0     4366 2024-03-19 20:07:41.714429 poetry_plugin_export-1.7.1/src/poetry_plugin_export/command.py
--rw-r--r--   0        0        0     7327 2024-03-19 20:07:41.714429 poetry_plugin_export-1.7.1/src/poetry_plugin_export/exporter.py
--rw-r--r--   0        0        0      957 2024-03-19 20:07:41.714429 poetry_plugin_export-1.7.1/src/poetry_plugin_export/plugins.py
--rw-r--r--   0        0        0     9933 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/src/poetry_plugin_export/walker.py
--rw-r--r--   0        0        0        0 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/command/__init__.py
--rw-r--r--   0        0        0     2549 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/command/conftest.py
--rw-r--r--   0        0        0     8410 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/command/test_command_export.py
--rw-r--r--   0        0        0     5673 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/conftest.py
--rw-r--r--   0        0        0     1116 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0      961 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/distributions/demo-0.1.0.tar.gz
--rw-r--r--   0        0        0      264 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/project_with_nested_local/bar/pyproject.toml
--rw-r--r--   0        0        0      262 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/project_with_nested_local/foo/pyproject.toml
--rw-r--r--   0        0        0      324 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/project_with_nested_local/pyproject.toml
--rw-r--r--   0        0        0      221 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/project_with_nested_local/quix/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/project_with_setup/my_package/__init__.py
--rw-r--r--   0        0        0      239 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/PKG-INFO
--rw-r--r--   0        0        0      201 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        0 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       38 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/requires.txt
--rw-r--r--   0        0        0       11 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/project_with_setup/project_with_setup.egg-info/top_level.txt
--rw-r--r--   0        0        0      416 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/project_with_setup/setup.py
--rw-r--r--   0        0        0       22 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/sample_project/README.rst
--rw-r--r--   0        0        0     1495 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/sample_project/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/simple_project/README.rst
--rw-r--r--   0        0        0     1106 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/simple_project/dist/simple-project-1.2.3.tar.gz
--rw-r--r--   0        0        0     1320 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
--rw-r--r--   0        0        0      771 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/simple_project/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/fixtures/simple_project/simple_project/__init__.py
--rw-r--r--   0        0        0     3174 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/helpers.py
--rw-r--r--   0        0        0     1262 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/markers.py
--rw-r--r--   0        0        0    91758 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/test_exporter.py
--rw-r--r--   0        0        0      995 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/test_walker.py
--rw-r--r--   0        0        0      978 2024-03-19 20:07:41.718428 poetry_plugin_export-1.7.1/tests/types.py
--rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 poetry_plugin_export-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-11 16:11:17.857624 poetry_plugin_export-1.8.0/LICENSE
+-rw-r--r--   0        0        0     1976 2024-05-11 16:11:17.857624 poetry_plugin_export-1.8.0/README.md
+-rw-r--r--   0        0        0     2696 2024-05-11 16:11:17.857624 poetry_plugin_export-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2024-05-11 16:11:17.857624 poetry_plugin_export-1.8.0/src/poetry_plugin_export/__init__.py
+-rw-r--r--   0        0        0     4366 2024-05-11 16:11:17.857624 poetry_plugin_export-1.8.0/src/poetry_plugin_export/command.py
+-rw-r--r--   0        0        0     7369 2024-05-11 16:11:17.857624 poetry_plugin_export-1.8.0/src/poetry_plugin_export/exporter.py
+-rw-r--r--   0        0        0      957 2024-05-11 16:11:17.857624 poetry_plugin_export-1.8.0/src/poetry_plugin_export/plugins.py
+-rw-r--r--   0        0        0     9933 2024-05-11 16:11:17.857624 poetry_plugin_export-1.8.0/src/poetry_plugin_export/walker.py
+-rw-r--r--   0        0        0        0 2024-05-11 16:11:17.857624 poetry_plugin_export-1.8.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-11 16:11:17.857624 poetry_plugin_export-1.8.0/tests/command/__init__.py
+-rw-r--r--   0        0        0     2549 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/command/conftest.py
+-rw-r--r--   0        0        0     8410 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/command/test_command_export.py
+-rw-r--r--   0        0        0     5673 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     1116 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0      961 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/distributions/demo-0.1.0.tar.gz
+-rw-r--r--   0        0        0      264 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/project_with_nested_local/bar/pyproject.toml
+-rw-r--r--   0        0        0      262 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/project_with_nested_local/foo/pyproject.toml
+-rw-r--r--   0        0        0      324 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/project_with_nested_local/pyproject.toml
+-rw-r--r--   0        0        0      221 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/project_with_nested_local/quix/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/project_with_setup/my_package/__init__.py
+-rw-r--r--   0        0        0      239 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      201 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        0 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       38 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/requires.txt
+-rw-r--r--   0        0        0       11 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/project_with_setup/project_with_setup.egg-info/top_level.txt
+-rw-r--r--   0        0        0      416 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/project_with_setup/setup.py
+-rw-r--r--   0        0        0       22 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/sample_project/README.rst
+-rw-r--r--   0        0        0     1495 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/sample_project/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/simple_project/README.rst
+-rw-r--r--   0        0        0     1106 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/simple_project/dist/simple-project-1.2.3.tar.gz
+-rw-r--r--   0        0        0     1320 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
+-rw-r--r--   0        0        0      771 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/simple_project/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/fixtures/simple_project/simple_project/__init__.py
+-rw-r--r--   0        0        0     3174 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/helpers.py
+-rw-r--r--   0        0        0     1262 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/markers.py
+-rw-r--r--   0        0        0    93318 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/test_exporter.py
+-rw-r--r--   0        0        0      995 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/test_walker.py
+-rw-r--r--   0        0        0      978 2024-05-11 16:11:17.861624 poetry_plugin_export-1.8.0/tests/types.py
+-rw-r--r--   0        0        0     2806 1970-01-01 00:00:00.000000 poetry_plugin_export-1.8.0/PKG-INFO
```

### Comparing `poetry_plugin_export-1.7.1/LICENSE` & `poetry_plugin_export-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/README.md` & `poetry_plugin_export-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/pyproject.toml` & `poetry_plugin_export-1.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-export"
-version = "1.7.1"
+version = "1.8.0"
 description = "Poetry plugin to export the dependencies to various formats"
 authors = ["Sébastien Eustace <sebastien@eustace.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://python-poetry.org/"
 repository = "https://github.com/python-poetry/poetry-plugin-export"
 
@@ -14,16 +14,16 @@
 
 include = [
     { path = "tests", format = "sdist" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-poetry = "^1.8.0"
-poetry-core = "^1.7.0"
+poetry = ">=1.8.0,<3.0.0"
+poetry-core = ">=1.7.0,<3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=2.18"
 pytest = "^8.0"
 pytest-cov = "^4.0"
 pytest-mock = "^3.9"
 pytest-randomly = "^3.12"
```

### Comparing `poetry_plugin_export-1.7.1/src/poetry_plugin_export/command.py` & `poetry_plugin_export-1.8.0/src/poetry_plugin_export/command.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/src/poetry_plugin_export/exporter.py` & `poetry_plugin_export-1.8.0/src/poetry_plugin_export/exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,36 +104,37 @@
 
             if not with_extras:
                 dependency_package = dependency_package.without_features()
 
             dependency = dependency_package.dependency
             package = dependency_package.package
 
-            if package.develop:
-                if not allow_editable:
-                    self._io.write_error_line(
-                        f"<warning>Warning: {package.pretty_name} is locked in develop"
-                        " (editable) mode, which is incompatible with the"
-                        " constraints.txt format.</warning>"
-                    )
-                    continue
-                line += "-e "
+            if package.develop and not allow_editable:
+                self._io.write_error_line(
+                    f"<warning>Warning: {package.pretty_name} is locked in develop"
+                    " (editable) mode, which is incompatible with the"
+                    " constraints.txt format.</warning>"
+                )
+                continue
 
             requirement = dependency.to_pep_508(with_extras=False, resolved=True)
             is_direct_local_reference = (
                 dependency.is_file() or dependency.is_directory()
             )
             is_direct_remote_reference = dependency.is_vcs() or dependency.is_url()
 
             if is_direct_remote_reference:
                 line = requirement
             elif is_direct_local_reference:
                 assert dependency.source_url is not None
                 dependency_uri = path_to_url(dependency.source_url)
-                line = f"{package.complete_name} @ {dependency_uri}"
+                if package.develop:
+                    line = f"-e {dependency_uri}"
+                else:
+                    line = f"{package.complete_name} @ {dependency_uri}"
             else:
                 line = f"{package.complete_name}=={package.version}"
 
             if not is_direct_remote_reference and ";" in requirement:
                 markers = requirement.split(";", 1)[1].strip()
                 if markers:
                     line += f" ; {markers}"
```

### Comparing `poetry_plugin_export-1.7.1/src/poetry_plugin_export/plugins.py` & `poetry_plugin_export-1.8.0/src/poetry_plugin_export/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/src/poetry_plugin_export/walker.py` & `poetry_plugin_export-1.8.0/src/poetry_plugin_export/walker.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/tests/command/conftest.py` & `poetry_plugin_export-1.8.0/tests/command/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/tests/command/test_command_export.py` & `poetry_plugin_export-1.8.0/tests/command/test_command_export.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/tests/conftest.py` & `poetry_plugin_export-1.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl` & `poetry_plugin_export-1.8.0/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/tests/fixtures/distributions/demo-0.1.0.tar.gz` & `poetry_plugin_export-1.8.0/tests/fixtures/distributions/demo-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/tests/fixtures/sample_project/pyproject.toml` & `poetry_plugin_export-1.8.0/tests/fixtures/sample_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/tests/fixtures/simple_project/dist/simple-project-1.2.3.tar.gz` & `poetry_plugin_export-1.8.0/tests/fixtures/simple_project/dist/simple-project-1.2.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl` & `poetry_plugin_export-1.8.0/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/tests/fixtures/simple_project/pyproject.toml` & `poetry_plugin_export-1.8.0/tests/fixtures/simple_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/tests/helpers.py` & `poetry_plugin_export-1.8.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/tests/markers.py` & `poetry_plugin_export-1.8.0/tests/markers.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/tests/test_exporter.py` & `poetry_plugin_export-1.8.0/tests/test_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,25 +78,30 @@
     p = Factory().create_poetry(fixture_root / "sample_project")
     p._locker = locker
 
     return p
 
 
 def set_package_requires(
-    poetry: Poetry, skip: set[str] | None = None, dev: set[str] | None = None
+    poetry: Poetry,
+    skip: set[str] | None = None,
+    dev: set[str] | None = None,
+    markers: dict[str, str] | None = None,
 ) -> None:
     skip = skip or set()
     dev = dev or set()
     packages = poetry.locker.locked_repository().packages
     package = poetry.package.with_dependency_groups([], only=True)
     for pkg in packages:
         if pkg.name not in skip:
             dep = pkg.to_dependency()
             if pkg.name in dev:
                 dep._groups = frozenset(["dev"])
+            if markers and pkg.name in markers:
+                dep._marker = parse_marker(markers[pkg.name])
             package.add_dependency(dep)
 
     poetry._package = package
 
 
 def test_exporter_can_export_requirements_txt_with_standard_packages(
     tmp_path: Path, poetry: Poetry
@@ -147,39 +152,41 @@
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
                     "optional": False,
                     "python-versions": "*",
-                    "marker": "python_version < '3.7'",
                 },
                 {
                     "name": "bar",
                     "version": "4.5.6",
                     "optional": False,
                     "python-versions": "*",
-                    "marker": "extra =='foo'",
                 },
                 {
                     "name": "baz",
                     "version": "7.8.9",
                     "optional": False,
                     "python-versions": "*",
-                    "marker": "sys_platform == 'win32'",
                 },
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
                 "files": {"foo": [], "bar": [], "baz": []},
             },
         }
     )
-    set_package_requires(poetry)
+    markers = {
+        "foo": "python_version < '3.7'",
+        "bar": "extra =='foo'",
+        "baz": "sys_platform == 'win32'",
+    }
+    set_package_requires(poetry, markers=markers)
 
     exporter = Exporter(poetry, NullIO())
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
         content = f.read()
 
@@ -393,31 +400,37 @@
         {
             "package": [
                 {
                     "name": "a",
                     "version": "1.2.3",
                     "optional": False,
                     "python-versions": "*",
-                    "marker": "python_version < '3.7'",
-                    "dependencies": {"b": ">=0.0.0", "c": ">=0.0.0"},
+                    "dependencies": {
+                        "b": {
+                            "version": ">=0.0.0",
+                            "markers": "platform_system == 'Windows'",
+                        },
+                        "c": {
+                            "version": ">=0.0.0",
+                            "markers": "sys_platform == 'win32'",
+                        },
+                    },
                 },
                 {
                     "name": "b",
                     "version": "4.5.6",
                     "optional": False,
                     "python-versions": "*",
-                    "marker": "platform_system == 'Windows'",
                     "dependencies": {"d": ">=0.0.0"},
                 },
                 {
                     "name": "c",
                     "version": "7.8.9",
                     "optional": False,
                     "python-versions": "*",
-                    "marker": "sys_platform == 'win32'",
                     "dependencies": {"d": ">=0.0.0"},
                 },
                 {
                     "name": "d",
                     "version": "0.0.1",
                     "optional": False,
                     "python-versions": "*",
@@ -426,15 +439,17 @@
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
                 "files": {"a": [], "b": [], "c": [], "d": []},
             },
         }
     )
-    set_package_requires(poetry, skip={"b", "c", "d"})
+    set_package_requires(
+        poetry, skip={"b", "c", "d"}, markers={"a": "python_version < '3.7'"}
+    )
 
     exporter = Exporter(poetry, NullIO())
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
         content = f.read()
 
@@ -1192,15 +1207,14 @@
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
                     "optional": False,
                     "python-versions": "*",
-                    "marker": "python_version < '3.7'",
                     "source": {
                         "type": "git",
                         "url": "https://github.com/foo/foo.git",
                         "reference": "123456",
                         "resolved_reference": "abcdef",
                     },
                 }
@@ -1208,15 +1222,15 @@
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
                 "files": {"foo": []},
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, markers={"foo": "python_version < '3.7'"})
 
     exporter = Exporter(poetry, NullIO())
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
         content = f.read()
 
@@ -1263,14 +1277,55 @@
     expected = f"""\
 foo @ {fixture_root_uri}/sample_project ; {MARKER_PY}
 """
 
     assert content == expected
 
 
+def test_exporter_can_export_requirements_txt_with_directory_packages_editable(
+    tmp_path: Path, poetry: Poetry, fixture_root_uri: str
+) -> None:
+    poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
+        {
+            "package": [
+                {
+                    "name": "foo",
+                    "version": "1.2.3",
+                    "optional": False,
+                    "python-versions": "*",
+                    "develop": True,
+                    "source": {
+                        "type": "directory",
+                        "url": "sample_project",
+                        "reference": "",
+                    },
+                }
+            ],
+            "metadata": {
+                "python-versions": "*",
+                "content-hash": "123456789",
+                "files": {"foo": []},
+            },
+        }
+    )
+    set_package_requires(poetry)
+
+    exporter = Exporter(poetry, NullIO())
+    exporter.export("requirements.txt", tmp_path, "requirements.txt")
+
+    with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
+        content = f.read()
+
+    expected = f"""\
+-e {fixture_root_uri}/sample_project ; {MARKER_PY}
+"""
+
+    assert content == expected
+
+
 def test_exporter_can_export_requirements_txt_with_nested_directory_packages(
     tmp_path: Path, poetry: Poetry, fixture_root_uri: str
 ) -> None:
     poetry.locker.mock_lock_data(  # type: ignore[attr-defined]
         {
             "package": [
                 {
@@ -1338,30 +1393,29 @@
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
                     "optional": False,
                     "python-versions": "*",
-                    "marker": "python_version < '3.7'",
                     "source": {
                         "type": "directory",
                         "url": "sample_project",
                         "reference": "",
                     },
                 }
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
                 "files": {"foo": []},
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, markers={"foo": "python_version < '3.7'"})
 
     exporter = Exporter(poetry, NullIO())
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
         content = f.read()
 
@@ -1421,30 +1475,29 @@
         {
             "package": [
                 {
                     "name": "foo",
                     "version": "1.2.3",
                     "optional": False,
                     "python-versions": "*",
-                    "marker": "python_version < '3.7'",
                     "source": {
                         "type": "file",
                         "url": "distributions/demo-0.1.0.tar.gz",
                         "reference": "",
                     },
                 }
             ],
             "metadata": {
                 "python-versions": "*",
                 "content-hash": "123456789",
                 "files": {"foo": []},
             },
         }
     )
-    set_package_requires(poetry)
+    set_package_requires(poetry, markers={"foo": "python_version < '3.7'"})
 
     exporter = Exporter(poetry, NullIO())
     exporter.export("requirements.txt", tmp_path, "requirements.txt")
 
     with (tmp_path / "requirements.txt").open(encoding="utf-8") as f:
         content = f.read()
```

### Comparing `poetry_plugin_export-1.7.1/tests/test_walker.py` & `poetry_plugin_export-1.8.0/tests/test_walker.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/tests/types.py` & `poetry_plugin_export-1.8.0/tests/types.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_export-1.7.1/PKG-INFO` & `poetry_plugin_export-1.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-export
-Version: 1.7.1
+Version: 1.8.0
 Summary: Poetry plugin to export the dependencies to various formats
 Home-page: https://python-poetry.org/
 License: MIT
 Author: Sébastien Eustace
 Author-email: sebastien@eustace.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: poetry (>=1.8.0,<2.0.0)
-Requires-Dist: poetry-core (>=1.7.0,<2.0.0)
+Requires-Dist: poetry (>=1.8.0,<3.0.0)
+Requires-Dist: poetry-core (>=1.7.0,<3.0.0)
 Project-URL: Repository, https://github.com/python-poetry/poetry-plugin-export
 Description-Content-Type: text/markdown
 
 # Poetry Plugin: Export
 
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
```

