# Comparing `tmp/qamomile-0.1.0rc10.tar.gz` & `tmp/qamomile-0.1.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qamomile-0.1.0rc10.tar", max compression
+gzip compressed data, was "qamomile-0.1.0rc9.tar", max compression
```

## Comparing `qamomile-0.1.0rc10.tar` & `qamomile-0.1.0rc9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1678 2024-05-11 12:04:36.696434 qamomile-0.1.0rc10/README.md
--rw-r--r--   0        0        0     1153 2024-05-11 12:05:18.924677 qamomile-0.1.0rc10/pyproject.toml
--rw-r--r--   0        0        0      293 2024-05-11 12:04:36.704434 qamomile-0.1.0rc10/qamomile/core/__init__.py
--rw-r--r--   0        0        0      147 2024-05-11 12:04:36.704434 qamomile-0.1.0rc10/qamomile/core/ising_qubo/__init__.py
--rw-r--r--   0        0        0     2474 2024-05-11 12:04:36.704434 qamomile-0.1.0rc10/qamomile/core/ising_qubo/ising_qubo.py
--rw-r--r--   0        0        0      282 2024-05-11 12:04:36.704434 qamomile-0.1.0rc10/qamomile/core/qrac/__init__.py
--rw-r--r--   0        0        0     3918 2024-05-11 12:04:36.704434 qamomile-0.1.0rc10/qamomile/core/qrac/graph_coloring.py
--rw-r--r--   0        0        0      566 2024-05-11 12:04:36.704434 qamomile-0.1.0rc10/qamomile/qiskit/__init__.py
--rw-r--r--   0        0        0      244 2024-05-11 12:04:36.704434 qamomile-0.1.0rc10/qamomile/qiskit/minimal_encoding/__init__.py
--rw-r--r--   0        0        0     2813 2024-05-11 12:04:36.704434 qamomile-0.1.0rc10/qamomile/qiskit/minimal_encoding/cost_function.py
--rw-r--r--   0        0        0     8327 2024-05-11 12:04:36.704434 qamomile-0.1.0rc10/qamomile/qiskit/minimal_encoding/to_minimal_encoding.py
--rw-r--r--   0        0        0      175 2024-05-11 12:04:36.704434 qamomile-0.1.0rc10/qamomile/qiskit/qaoa/__init__.py
--rw-r--r--   0        0        0     1731 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/qiskit/qaoa/ising_hamiltonian.py
--rw-r--r--   0        0        0     6140 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/qiskit/qaoa/to_qaoa.py
--rw-r--r--   0        0        0      568 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/qiskit/qrao/__init__.py
--rw-r--r--   0        0        0     1786 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/qiskit/qrao/qrao21.py
--rw-r--r--   0        0        0     3158 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/qiskit/qrao/qrao31.py
--rw-r--r--   0        0        0     4347 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/qiskit/qrao/qrao32.py
--rw-r--r--   0        0        0     2449 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/qiskit/qrao/qrao_space_efficient.py
--rw-r--r--   0        0        0    11281 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/qiskit/qrao/to_qrac.py
--rw-r--r--   0        0        0      353 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/quri_parts/__init__.py
--rw-r--r--   0        0        0       86 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/quri_parts/qaoa/__init__.py
--rw-r--r--   0        0        0     7468 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/quri_parts/qaoa/to_qaoa.py
--rw-r--r--   0        0        0      504 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/quri_parts/qrao/__init__.py
--rw-r--r--   0        0        0     2171 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/quri_parts/qrao/qrao21.py
--rw-r--r--   0        0        0     3624 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/quri_parts/qrao/qrao31.py
--rw-r--r--   0        0        0     5320 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/quri_parts/qrao/qrao32.py
--rw-r--r--   0        0        0     8771 2024-05-11 12:04:36.708433 qamomile-0.1.0rc10/qamomile/quri_parts/qrao/to_qrac.py
--rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 qamomile-0.1.0rc10/PKG-INFO
+-rw-r--r--   0        0        0     1678 2024-05-11 11:52:00.262736 qamomile-0.1.0rc9/README.md
+-rw-r--r--   0        0        0     1157 2024-05-11 12:01:34.632696 qamomile-0.1.0rc9/pyproject.toml
+-rw-r--r--   0        0        0      293 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/core/__init__.py
+-rw-r--r--   0        0        0      147 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/core/ising_qubo/__init__.py
+-rw-r--r--   0        0        0     2474 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/core/ising_qubo/ising_qubo.py
+-rw-r--r--   0        0        0      282 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/core/qrac/__init__.py
+-rw-r--r--   0        0        0     3918 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/core/qrac/graph_coloring.py
+-rw-r--r--   0        0        0      566 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/qiskit/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/qiskit/minimal_encoding/__init__.py
+-rw-r--r--   0        0        0     2813 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/qiskit/minimal_encoding/cost_function.py
+-rw-r--r--   0        0        0     8327 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/qiskit/minimal_encoding/to_minimal_encoding.py
+-rw-r--r--   0        0        0      175 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/qiskit/qaoa/__init__.py
+-rw-r--r--   0        0        0     1731 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/qiskit/qaoa/ising_hamiltonian.py
+-rw-r--r--   0        0        0     6140 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/qiskit/qaoa/to_qaoa.py
+-rw-r--r--   0        0        0      568 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/qiskit/qrao/__init__.py
+-rw-r--r--   0        0        0     1786 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/qiskit/qrao/qrao21.py
+-rw-r--r--   0        0        0     3158 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/qiskit/qrao/qrao31.py
+-rw-r--r--   0        0        0     4347 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/qiskit/qrao/qrao32.py
+-rw-r--r--   0        0        0     2449 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/qiskit/qrao/qrao_space_efficient.py
+-rw-r--r--   0        0        0    11281 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/qiskit/qrao/to_qrac.py
+-rw-r--r--   0        0        0      353 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/quri_parts/__init__.py
+-rw-r--r--   0        0        0       86 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/quri_parts/qaoa/__init__.py
+-rw-r--r--   0        0        0     7468 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/quri_parts/qaoa/to_qaoa.py
+-rw-r--r--   0        0        0      504 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/quri_parts/qrao/__init__.py
+-rw-r--r--   0        0        0     2171 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/quri_parts/qrao/qrao21.py
+-rw-r--r--   0        0        0     3624 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/quri_parts/qrao/qrao31.py
+-rw-r--r--   0        0        0     5320 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/quri_parts/qrao/qrao32.py
+-rw-r--r--   0        0        0     8771 2024-05-11 11:37:15.402754 qamomile-0.1.0rc9/qamomile/quri_parts/qrao/to_qrac.py
+-rw-r--r--   0        0        0     2232 1970-01-01 00:00:00.000000 qamomile-0.1.0rc9/PKG-INFO
```

### Comparing `qamomile-0.1.0rc10/README.md` & `qamomile-0.1.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/pyproject.toml` & `qamomile-0.1.0rc9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["poetry-core>=1.5.2", "poetry-dynamic-versioning>=0.21.4"]
 build-backend = "poetry_dynamic_versioning.backend"
 
-[tool.poetry-dynamic-versioning]
-enable = false
-style = "pep440"
+# [tool.poetry-dynamic-versioning]
+# enable = true
+# style = "pep440"
 
 [tool.poetry]
 name = "qamomile"
-version = "0.1.0rc10" # using poetry-dynamic-versioning
+version = "0.1.0rc9" # using poetry-dynamic-versioning
 description = ""
 authors = ["Jij Inc. <info@j-ij.com>"]
 readme = "README.md"
 packages = [
     {include = "qamomile"},
 ]
```

### Comparing `qamomile-0.1.0rc10/qamomile/core/ising_qubo/ising_qubo.py` & `qamomile-0.1.0rc9/qamomile/core/ising_qubo/ising_qubo.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/core/qrac/graph_coloring.py` & `qamomile-0.1.0rc9/qamomile/core/qrac/graph_coloring.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/qiskit/__init__.py` & `qamomile-0.1.0rc9/qamomile/qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/qiskit/minimal_encoding/cost_function.py` & `qamomile-0.1.0rc9/qamomile/qiskit/minimal_encoding/cost_function.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/qiskit/minimal_encoding/to_minimal_encoding.py` & `qamomile-0.1.0rc9/qamomile/qiskit/minimal_encoding/to_minimal_encoding.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/qiskit/qaoa/ising_hamiltonian.py` & `qamomile-0.1.0rc9/qamomile/qiskit/qaoa/ising_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/qiskit/qaoa/to_qaoa.py` & `qamomile-0.1.0rc9/qamomile/qiskit/qaoa/to_qaoa.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/qiskit/qrao/__init__.py` & `qamomile-0.1.0rc9/qamomile/qiskit/qrao/__init__.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/qiskit/qrao/qrao21.py` & `qamomile-0.1.0rc9/qamomile/qiskit/qrao/qrao21.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/qiskit/qrao/qrao31.py` & `qamomile-0.1.0rc9/qamomile/qiskit/qrao/qrao31.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/qiskit/qrao/qrao32.py` & `qamomile-0.1.0rc9/qamomile/qiskit/qrao/qrao32.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/qiskit/qrao/qrao_space_efficient.py` & `qamomile-0.1.0rc9/qamomile/qiskit/qrao/qrao_space_efficient.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/qiskit/qrao/to_qrac.py` & `qamomile-0.1.0rc9/qamomile/qiskit/qrao/to_qrac.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/quri_parts/qaoa/to_qaoa.py` & `qamomile-0.1.0rc9/qamomile/quri_parts/qaoa/to_qaoa.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/quri_parts/qrao/qrao21.py` & `qamomile-0.1.0rc9/qamomile/quri_parts/qrao/qrao21.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/quri_parts/qrao/qrao31.py` & `qamomile-0.1.0rc9/qamomile/quri_parts/qrao/qrao31.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/quri_parts/qrao/qrao32.py` & `qamomile-0.1.0rc9/qamomile/quri_parts/qrao/qrao32.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/qamomile/quri_parts/qrao/to_qrac.py` & `qamomile-0.1.0rc9/qamomile/quri_parts/qrao/to_qrac.py`

 * *Files identical despite different names*

### Comparing `qamomile-0.1.0rc10/PKG-INFO` & `qamomile-0.1.0rc9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qamomile
-Version: 0.1.0rc10
+Version: 0.1.0rc9
 Summary: 
 Author: Jij Inc.
 Author-email: info@j-ij.com
 Requires-Python: >=3.9.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: qiskit
```

