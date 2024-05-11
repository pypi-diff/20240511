# Comparing `tmp/nn_parts-2024.0.0.tar.gz` & `tmp/nn_parts-2024.0.1.tar.gz`

## Comparing `nn_parts-2024.0.0.tar` & `nn_parts-2024.0.1.tar`

### file list

```diff
@@ -1,22 +1,13 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/src/nn_parts/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/src/nn_parts/activation_relu.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/src/nn_parts/activation_sigmoid.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/src/nn_parts/activation_softmax.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/src/nn_parts/cost_cross_entropy.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/src/nn_parts/cost_quadratic.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/src/nn_parts/denselayer.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/src/nn_parts/metric_accuracy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/tests/__init__.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/tests/test_accuracy.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/tests/test_cross_entropy.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/tests/test_denselayer.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/tests/test_quadratic.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/tests/test_relu.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/tests/test_sigmoid.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/tests/test_softmax.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/tests/data/dense_layer.json
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/LICENSE.txt
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/README.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/pyproject.toml
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nn_parts-2024.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nn_parts-2024.0.1/src/nn_parts/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 nn_parts-2024.0.1/src/nn_parts/activation_relu.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 nn_parts-2024.0.1/src/nn_parts/activation_sigmoid.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 nn_parts-2024.0.1/src/nn_parts/activation_softmax.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 nn_parts-2024.0.1/src/nn_parts/cost_cross_entropy.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 nn_parts-2024.0.1/src/nn_parts/cost_quadratic.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 nn_parts-2024.0.1/src/nn_parts/denselayer.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 nn_parts-2024.0.1/src/nn_parts/metric_accuracy.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nn_parts-2024.0.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nn_parts-2024.0.1/LICENSE.txt
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 nn_parts-2024.0.1/README.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 nn_parts-2024.0.1/pyproject.toml
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nn_parts-2024.0.1/PKG-INFO
```

### Comparing `nn_parts-2024.0.0/src/nn_parts/cost_cross_entropy.py` & `nn_parts-2024.0.1/src/nn_parts/cost_cross_entropy.py`

 * *Files identical despite different names*

### Comparing `nn_parts-2024.0.0/src/nn_parts/denselayer.py` & `nn_parts-2024.0.1/src/nn_parts/denselayer.py`

 * *Files identical despite different names*

### Comparing `nn_parts-2024.0.0/pyproject.toml` & `nn_parts-2024.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nn_parts"
-version = "2024.0.0"
+version = "2024.0.1"
 dependencies = [
     "numpy"
 ]
 requires-python = ">=3.8"
 authors = [
     { name = "Pankaj Singh", email = "pankajpriscilla@gmail.com" }
 ]
@@ -26,7 +26,15 @@
 ]
 
 [project.urls]
 Homepage = "https://example.com"
 Documentation = "https://readthedocs.org"
 Repository = "https://github.com/me/spam.git"
 Changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
+
+[tool.hatch.build]
+exclude = [
+    "/.*",
+    "/docs",
+    "/tests",
+    "/dist"
+]
```

### Comparing `nn_parts-2024.0.0/PKG-INFO` & `nn_parts-2024.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nn_parts
-Version: 2024.0.0
+Version: 2024.0.1
 Summary: Diagnois and Triage Neural Network
 Project-URL: Homepage, https://example.com
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/me/spam.git
 Project-URL: Changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
 Author-email: Pankaj Singh <pankajpriscilla@gmail.com>
 Maintainer-email: Pankaj Singh <pankajpriscilla@gmail.com>
```

