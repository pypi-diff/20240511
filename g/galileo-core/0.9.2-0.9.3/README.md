# Comparing `tmp/galileo_core-0.9.2.tar.gz` & `tmp/galileo_core-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_core-0.9.2.tar", max compression
+gzip compressed data, was "galileo_core-0.9.3.tar", max compression
```

## Comparing `galileo_core-0.9.2.tar` & `galileo_core-0.9.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0    10946 2024-04-08 04:56:54.314595 galileo_core-0.9.2/LICENSE
--rw-r--r--   0        0        0       80 2024-04-08 04:56:54.314595 galileo_core-0.9.2/README.md
--rw-r--r--   0        0        0     2323 2024-04-08 04:56:55.426591 galileo_core-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-08 04:56:55.430592 galileo_core-0.9.2/src/galileo_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 04:56:54.314595 galileo_core-0.9.2/src/galileo_core/constants/__init__.py
--rw-r--r--   0        0        0      573 2024-04-08 04:56:54.314595 galileo_core-0.9.2/src/galileo_core/constants/http_headers.py
--rw-r--r--   0        0        0      362 2024-04-08 04:56:54.314595 galileo_core-0.9.2/src/galileo_core/constants/routes.py
--rw-r--r--   0        0        0        0 2024-04-08 04:56:54.314595 galileo_core-0.9.2/src/galileo_core/helpers/__init__.py
--rw-r--r--   0        0        0     1543 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/helpers/api_client.py
--rw-r--r--   0        0        0     6123 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/helpers/config.py
--rw-r--r--   0        0        0       60 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/helpers/logger.py
--rw-r--r--   0        0        0        0 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/schemas/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/schemas/protect/__init__.py
--rw-r--r--   0        0        0     1382 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/schemas/protect/action.py
--rw-r--r--   0        0        0      890 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/schemas/protect/metric.py
--rw-r--r--   0        0        0      902 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/schemas/protect/payload.py
--rw-r--r--   0        0        0     3905 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/schemas/protect/request.py
--rw-r--r--   0        0        0     1934 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/schemas/protect/rule.py
--rw-r--r--   0        0        0      831 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/schemas/protect/ruleset.py
--rw-r--r--   0        0        0     1124 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/schemas/protect/stage.py
--rw-r--r--   0        0        0        0 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/schemas/shared/__init__.py
--rw-r--r--   0        0        0      149 2024-04-08 04:56:54.318595 galileo_core-0.9.2/src/galileo_core/schemas/shared/metric.py
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 galileo_core-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-04-08 05:10:36.721013 galileo_core-0.9.3/LICENSE
+-rw-r--r--   0        0        0       80 2024-04-08 05:10:36.721013 galileo_core-0.9.3/README.md
+-rw-r--r--   0        0        0     2323 2024-04-08 05:10:38.125014 galileo_core-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-08 05:10:38.129014 galileo_core-0.9.3/src/galileo_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/constants/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/constants/http_headers.py
+-rw-r--r--   0        0        0      362 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/helpers/__init__.py
+-rw-r--r--   0        0        0     1543 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/helpers/api_client.py
+-rw-r--r--   0        0        0     6123 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/helpers/config.py
+-rw-r--r--   0        0        0       60 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/helpers/logger.py
+-rw-r--r--   0        0        0        0 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/py.typed
+-rw-r--r--   0        0        0        0 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/__init__.py
+-rw-r--r--   0        0        0     1382 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/action.py
+-rw-r--r--   0        0        0      890 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/metric.py
+-rw-r--r--   0        0        0      902 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/payload.py
+-rw-r--r--   0        0        0     3905 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/request.py
+-rw-r--r--   0        0        0     1934 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/rule.py
+-rw-r--r--   0        0        0      831 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/ruleset.py
+-rw-r--r--   0        0        0     1124 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/stage.py
+-rw-r--r--   0        0        0        0 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/shared/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/shared/metric.py
+-rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 galileo_core-0.9.3/PKG-INFO
```

### Comparing `galileo_core-0.9.2/LICENSE` & `galileo_core-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.2/pyproject.toml` & `galileo_core-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "galileo-core"
-version = "0.9.2"
+version = "0.9.3"
 description = "Shared schemas and configuration for Galileo's Python packages."
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_core", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
```

### Comparing `galileo_core-0.9.2/src/galileo_core/constants/http_headers.py` & `galileo_core-0.9.3/src/galileo_core/constants/http_headers.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.2/src/galileo_core/helpers/api_client.py` & `galileo_core-0.9.3/src/galileo_core/helpers/api_client.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.2/src/galileo_core/helpers/config.py` & `galileo_core-0.9.3/src/galileo_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.2/src/galileo_core/schemas/protect/action.py` & `galileo_core-0.9.3/src/galileo_core/schemas/protect/action.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.2/src/galileo_core/schemas/protect/metric.py` & `galileo_core-0.9.3/src/galileo_core/schemas/protect/metric.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.2/src/galileo_core/schemas/protect/payload.py` & `galileo_core-0.9.3/src/galileo_core/schemas/protect/payload.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.2/src/galileo_core/schemas/protect/request.py` & `galileo_core-0.9.3/src/galileo_core/schemas/protect/request.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.2/src/galileo_core/schemas/protect/rule.py` & `galileo_core-0.9.3/src/galileo_core/schemas/protect/rule.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.2/src/galileo_core/schemas/protect/ruleset.py` & `galileo_core-0.9.3/src/galileo_core/schemas/protect/ruleset.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.2/src/galileo_core/schemas/protect/stage.py` & `galileo_core-0.9.3/src/galileo_core/schemas/protect/stage.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.2/PKG-INFO` & `galileo_core-0.9.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galileo-core
-Version: 0.9.2
+Version: 0.9.3
 Summary: Shared schemas and configuration for Galileo's Python packages.
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

