# Comparing `tmp/hatch_gradle_version-0.9.6.tar.gz` & `tmp/hatch_gradle_version-0.9.7.tar.gz`

## Comparing `hatch_gradle_version-0.9.6.tar` & `hatch_gradle_version-0.9.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/__init__.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/_hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/cd.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/codegen.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/decorators.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/gradle.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/model.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/path.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/__init__.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_scheme.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/__init__.py
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/base.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/gradle_properties.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/test_gradle_properties.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/test_version_catalog.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/version_catalog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/__init__.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/base.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/gradle_properties.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/json.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/test_gradle_properties.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/test_json.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/LICENSE
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/README.md
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/pyproject.toml
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/__init__.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/_hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/common/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/common/cd.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/common/codegen.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/common/decorators.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/common/gradle.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/common/model.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/common/path.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/__init__.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/version_scheme.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/metadata_hook/__init__.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/metadata_hook/base.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/metadata_hook/gradle_properties.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/metadata_hook/test_gradle_properties.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/metadata_hook/test_version_catalog.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/metadata_hook/version_catalog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/version_source/__init__.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/version_source/base.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/version_source/gradle_properties.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/version_source/json.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/version_source/test_gradle_properties.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/version_source/test_json.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/LICENSE
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/README.md
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 hatch_gradle_version-0.9.7/PKG-INFO
```

### Comparing `hatch_gradle_version-0.9.6/.github/workflows/publish.yaml` & `hatch_gradle_version-0.9.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/.vscode/settings.json` & `hatch_gradle_version-0.9.7/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/_hooks.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/_hooks.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/gradle.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/common/gradle.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/common/model.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/common/model.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_scheme.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/version_scheme.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/base.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/metadata_hook/base.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/gradle_properties.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/metadata_hook/gradle_properties.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/test_gradle_properties.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/metadata_hook/test_gradle_properties.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/test_version_catalog.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/metadata_hook/test_version_catalog.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/metadata_hook/version_catalog.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/metadata_hook/version_catalog.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/base.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/version_source/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import re
 from abc import ABC, abstractmethod
 from typing import Any, TypedDict
 
 from casefy import casefy
 from hatchling.version.core import DEFAULT_PATTERN
 from hatchling.version.source.plugin.interface import VersionSourceInterface
+from pydantic import AliasChoices, Field
 
 from hatch_gradle_version.common.codegen import write_code
 from hatch_gradle_version.common.gradle import GradleVersion
-from hatch_gradle_version.common.model import HookModel, ProjectPath
+from hatch_gradle_version.common.model import HookModel, KebabModel, ProjectPath
 
 PY_VERSION_REGEX = re.compile(
     r'(?i)^(PY_VERSION) *= *([\'"])v?(?P<version>.+?)\2',
     flags=re.MULTILINE,
 )
 
 DEFAULT_REGEX = re.compile(DEFAULT_PATTERN, flags=re.MULTILINE)
@@ -22,38 +23,43 @@
     version: str
     gradle_version: str
     py_version: str
     extra_versions: dict[str, str]
     full_gradle_version: GradleVersion
 
 
+class GradleVersionRegex(KebabModel):
+    pattern: re.Pattern[str] = Field(
+        validation_alias=AliasChoices("pattern", "pat", "regex"),
+    )
+    replacement: str = Field(
+        r"\1",
+        validation_alias=AliasChoices("replacement", "repl"),
+    )
+
+
 class BaseVersionSource(HookModel, VersionSourceInterface, ABC):
     source: str
     py_path: ProjectPath
     scheme: str | None = None
-    gradle_version_regex: re.Pattern[str] | None = None
-    """Should contain exactly one match group, representing the part of the raw Gradle
-    version to keep."""
+    gradle_version_regex: re.Pattern[str] | GradleVersionRegex | None = None
+    """If this is a standalone regex, it should contain exactly one match group,
+    representing the part of the raw Gradle version to keep."""
 
     @abstractmethod
-    def get_gradle_version(self) -> GradleVersion:
-        ...
+    def get_gradle_version(self) -> GradleVersion: ...
 
     def fmt_raw_gradle_version(self, raw: str) -> str:
-        if self.gradle_version_regex is None:
-            return raw
-
-        match = self.gradle_version_regex.match(raw)
-        if match is None:
-            raise ValueError(f"gradle_version_regex failed to match version: {raw}")
-
-        if len(match.groups()) < 1:
-            raise ValueError("gradle_version_regex must have at least 1 group, got 0")
-
-        return match[1]
+        match self.gradle_version_regex:
+            case re.Pattern() as pattern:
+                return pattern.sub(r"\1", raw)
+            case GradleVersionRegex(pattern=pattern, replacement=replacement):
+                return pattern.sub(replacement, raw)
+            case None:
+                return raw
 
     def get_version_data(self):
         gradle_version = self.get_gradle_version()
         py_version = self.get_py_version()
 
         version = gradle_version.full_version(py_version)
```

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/gradle_properties.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/version_source/gradle_properties.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/json.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/version_source/json.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/test_gradle_properties.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/version_source/test_gradle_properties.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pathlib import Path
 
+import pytest
 from pytest import MonkeyPatch
 
 from hatch_gradle_version.common.gradle import GradleVersion
 
 from .gradle_properties import GradlePropertiesVersionSource
 
 
@@ -60,7 +61,54 @@
     assert gradle_version == GradleVersion(
         raw_version="0.1.0",
         version="0.1.0",
         rc=None,
         build=None,
         extra_versions={"modVersion": "'1.19.2-0.1.0'"},
     )
+
+
+@pytest.mark.parametrize(
+    ["pattern", "replacement", "raw_version", "expected"],
+    [
+        (r"^(.+?)-(.+)", r"\2.\1", "1.19.2-0.1.0", "0.1.0.1.19.2"),
+        (r"^(.+?)\+(.+)", r"\1.\2", "0.1.0+1.19.2", "0.1.0.1.19.2"),
+    ],
+)
+def test_rewrite(
+    tmp_path: Path,
+    monkeypatch: MonkeyPatch,
+    pattern: str,
+    replacement: str,
+    raw_version: str,
+    expected: str,
+):
+    # arrange
+    monkeypatch.setenv("HATCH_GRADLE_DIR", "gradle_dir")
+
+    gradle = tmp_path / "gradle_dir" / "gradle.properties"
+    gradle.parent.mkdir()
+    gradle.write_text(f"modVersion={raw_version}")
+
+    hook = GradlePropertiesVersionSource.from_config(
+        tmp_path.as_posix(),
+        {
+            "source": "json",
+            "py-path": "",
+            "gradle-path": "gradle.properties",
+            "key": "modVersion",
+            "gradle-version-regex": {
+                "pattern": pattern,
+                "replacement": replacement,
+            },
+        },
+    )
+
+    gradle_version = hook.get_gradle_version()
+
+    assert gradle_version == GradleVersion(
+        raw_version=expected,
+        version=expected,
+        rc=None,
+        build=None,
+        extra_versions={"modVersion": f"'{raw_version}'"},
+    )
```

### Comparing `hatch_gradle_version-0.9.6/src/hatch_gradle_version/plugins/version_source/test_json.py` & `hatch_gradle_version-0.9.7/src/hatch_gradle_version/plugins/version_source/test_json.py`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/.gitignore` & `hatch_gradle_version-0.9.7/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/LICENSE` & `hatch_gradle_version-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hatch_gradle_version-0.9.6/pyproject.toml` & `hatch_gradle_version-0.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hatch-gradle-version"
-version = "0.9.6"
+version = "0.9.7"
 authors = [
     { name="object-Object", email="object@objectobject.ca" },
 ]
 readme = "README.md"
 classifiers = [
     "Framework :: Hatch",
 ]
@@ -42,14 +42,17 @@
 [project.entry-points.hatch]
 gradle_version = "hatch_gradle_version._hooks"
 
 # pytest
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
+filterwarnings = [
+    'ignore:Dependency on package .+? will ONLY accept:UserWarning:hatch_gradle_version.common.gradle',
+]
 
 # formatting/linting
 
 [tool.isort]
 profile = "black"
 combine_as_imports = true
```

### Comparing `hatch_gradle_version-0.9.6/PKG-INFO` & `hatch_gradle_version-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hatch-gradle-version
-Version: 0.9.6
+Version: 0.9.7
 Project-URL: Homepage, https://github.com/hexdoc-dev/hatch-gradle-version
 Project-URL: Bug Tracker, https://github.com/hexdoc-dev/hatch-gradle-version/issues
 Author-email: object-Object <object@objectobject.ca>
 License-File: LICENSE
 Classifier: Framework :: Hatch
 Requires-Python: >=3.11
 Requires-Dist: black==23.7.0
```

