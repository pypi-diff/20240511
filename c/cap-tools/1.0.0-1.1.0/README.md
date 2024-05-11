# Comparing `tmp/cap_tools-1.0.0.tar.gz` & `tmp/cap_tools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cap_tools-1.0.0.tar", max compression
+gzip compressed data, was "cap_tools-1.1.0.tar", max compression
```

## Comparing `cap_tools-1.0.0.tar` & `cap_tools-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-05-09 12:14:22.868359 cap_tools-1.0.0/LICENSE
--rw-r--r--   0        0        0      681 2024-05-09 12:14:22.868359 cap_tools-1.0.0/README.md
--rw-r--r--   0        0        0     1894 2024-05-09 12:14:22.872359 cap_tools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      530 2024-05-09 12:14:22.872359 cap_tools-1.0.0/src/cap_tools/__init__.py
--rw-r--r--   0        0        0    12918 2024-05-09 12:14:22.872359 cap_tools-1.0.0/src/cap_tools/models.py
--rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 cap_tools-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-11 09:50:54.925494 cap_tools-1.1.0/LICENSE
+-rw-r--r--   0        0        0      681 2024-05-11 09:50:54.925494 cap_tools-1.1.0/README.md
+-rw-r--r--   0        0        0     1894 2024-05-11 09:50:54.925494 cap_tools-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      530 2024-05-11 09:50:54.925494 cap_tools-1.1.0/src/cap_tools/__init__.py
+-rw-r--r--   0        0        0    12848 2024-05-11 09:50:54.925494 cap_tools-1.1.0/src/cap_tools/models.py
+-rw-r--r--   0        0        0     1170 1970-01-01 00:00:00.000000 cap_tools-1.1.0/PKG-INFO
```

### Comparing `cap_tools-1.0.0/LICENSE` & `cap_tools-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cap_tools-1.0.0/README.md` & `cap_tools-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cap_tools-1.0.0/pyproject.toml` & `cap_tools-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 update_changelog_on_bump = true
 
 [tool.coverage.run]
 source = ["src", "tests"]
 
 [tool.poetry]
 name = "cap-tools"
-version = "1.0.0"
+version = "1.1.0"
 description = "Python data bindings for the Common Alerting Protocol Version."
 authors = ["Björn Reetz <git@bjoern-reetz.de>"]
 readme = "README.md"
 packages = [{include = "cap_tools", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `cap_tools-1.0.0/src/cap_tools/__init__.py` & `cap_tools-1.1.0/src/cap_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cap_tools-1.0.0/src/cap_tools/models.py` & `cap_tools-1.1.0/src/cap_tools/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,43 +128,43 @@
     ACTUAL = "Actual"
     EXERCISE = "Exercise"
     SYSTEM = "System"
     TEST = "Test"
     DRAFT = "Draft"
 
 
-@dataclass(slots=True, kw_only=True)
+@dataclass(slots=True)
 class Value:
     class Meta:
         name = "value"
         namespace = "urn:oasis:names:tc:emergency:cap:1.2"
 
     value: str = field(
         default="",
         metadata={
             "required": True,
         },
     )
 
 
-@dataclass(slots=True, kw_only=True)
+@dataclass(slots=True)
 class ValueName:
     class Meta:
         name = "valueName"
         namespace = "urn:oasis:names:tc:emergency:cap:1.2"
 
     value: str = field(
         default="",
         metadata={
             "required": True,
         },
     )
 
 
-@dataclass(slots=True, kw_only=True)
+@dataclass(slots=True)
 class Geocode:
     class Meta:
         global_type = False
 
     value_name: ValueName = field(
         metadata={
             "name": "valueName",
@@ -178,15 +178,15 @@
             "type": "Element",
             "namespace": "urn:oasis:names:tc:emergency:cap:1.2",
             "required": True,
         }
     )
 
 
-@dataclass(slots=True, kw_only=True)
+@dataclass(slots=True)
 class EventCode:
     class Meta:
         global_type = False
 
     value_name: ValueName = field(
         metadata={
             "name": "valueName",
@@ -200,15 +200,15 @@
             "type": "Element",
             "namespace": "urn:oasis:names:tc:emergency:cap:1.2",
             "required": True,
         }
     )
 
 
-@dataclass(slots=True, kw_only=True)
+@dataclass(slots=True)
 class Parameter:
     class Meta:
         global_type = False
 
     value_name: ValueName = field(
         metadata={
             "name": "valueName",
```

### Comparing `cap_tools-1.0.0/PKG-INFO` & `cap_tools-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cap-tools
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python data bindings for the Common Alerting Protocol Version.
 Author: Björn Reetz
 Author-email: git@bjoern-reetz.de
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

