# Comparing `tmp/pysparkler-0.9.dev1715453058.tar.gz` & `tmp/pysparkler-0.9.dev1715454332.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.9.dev1715453058.tar", max compression
+gzip compressed data, was "pysparkler-0.9.dev1715454332.tar", max compression
```

## Comparing `pysparkler-0.9.dev1715453058.tar` & `pysparkler-0.9.dev1715454332.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    13414 2024-05-11 18:44:12.880597 pysparkler-0.9.dev1715453058/README.md
--rw-r--r--   0        0        0     1344 2024-05-11 18:44:19.220601 pysparkler-0.9.dev1715453058/pyproject.toml
--rw-r--r--   0        0        0      807 2024-05-11 18:44:12.880597 pysparkler-0.9.dev1715453058/pysparkler/__init__.py
--rw-r--r--   0        0        0     5398 2024-05-11 18:44:12.880597 pysparkler-0.9.dev1715453058/pysparkler/api.py
--rw-r--r--   0        0        0     7372 2024-05-11 18:44:12.880597 pysparkler-0.9.dev1715453058/pysparkler/base.py
--rw-r--r--   0        0        0     7749 2024-05-11 18:44:12.880597 pysparkler-0.9.dev1715453058/pysparkler/cli.py
--rw-r--r--   0        0        0     6077 2024-05-11 18:44:12.880597 pysparkler-0.9.dev1715453058/pysparkler/pyspark_22_to_23.py
--rw-r--r--   0        0        0     4650 2024-05-11 18:44:12.880597 pysparkler-0.9.dev1715453058/pysparkler/pyspark_23_to_24.py
--rw-r--r--   0        0        0    10561 2024-05-11 18:44:12.880597 pysparkler-0.9.dev1715453058/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3969 2024-05-11 18:44:12.880597 pysparkler-0.9.dev1715453058/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     3895 2024-05-11 18:44:12.880597 pysparkler-0.9.dev1715453058/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0     6404 2024-05-11 18:44:12.880597 pysparkler-0.9.dev1715453058/pysparkler/sql_21_to_33.py
--rw-r--r--   0        0        0    14450 1970-01-01 00:00:00.000000 pysparkler-0.9.dev1715453058/PKG-INFO
+-rw-r--r--   0        0        0    13414 2024-05-11 19:05:25.999816 pysparkler-0.9.dev1715454332/README.md
+-rw-r--r--   0        0        0     1344 2024-05-11 19:05:32.331878 pysparkler-0.9.dev1715454332/pyproject.toml
+-rw-r--r--   0        0        0      807 2024-05-11 19:05:25.999816 pysparkler-0.9.dev1715454332/pysparkler/__init__.py
+-rw-r--r--   0        0        0     5398 2024-05-11 19:05:25.999816 pysparkler-0.9.dev1715454332/pysparkler/api.py
+-rw-r--r--   0        0        0     7372 2024-05-11 19:05:25.999816 pysparkler-0.9.dev1715454332/pysparkler/base.py
+-rw-r--r--   0        0        0     7749 2024-05-11 19:05:25.999816 pysparkler-0.9.dev1715454332/pysparkler/cli.py
+-rw-r--r--   0        0        0     6077 2024-05-11 19:05:25.999816 pysparkler-0.9.dev1715454332/pysparkler/pyspark_22_to_23.py
+-rw-r--r--   0        0        0     4650 2024-05-11 19:05:25.999816 pysparkler-0.9.dev1715454332/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10561 2024-05-11 19:05:25.999816 pysparkler-0.9.dev1715454332/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3969 2024-05-11 19:05:25.999816 pysparkler-0.9.dev1715454332/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     3895 2024-05-11 19:05:25.999816 pysparkler-0.9.dev1715454332/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0     6404 2024-05-11 19:05:25.999816 pysparkler-0.9.dev1715454332/pysparkler/sql_21_to_33.py
+-rw-r--r--   0        0        0    14450 1970-01-01 00:00:00.000000 pysparkler-0.9.dev1715454332/PKG-INFO
```

### Comparing `pysparkler-0.9.dev1715453058/README.md` & `pysparkler-0.9.dev1715454332/README.md`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1715453058/pyproject.toml` & `pysparkler-0.9.dev1715454332/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.9.dev1715453058"
+version = "0.9.dev1715454332"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.9.dev1715453058/pysparkler/__init__.py` & `pysparkler-0.9.dev1715454332/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1715453058/pysparkler/api.py` & `pysparkler-0.9.dev1715454332/pysparkler/api.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1715453058/pysparkler/base.py` & `pysparkler-0.9.dev1715454332/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1715453058/pysparkler/cli.py` & `pysparkler-0.9.dev1715454332/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1715453058/pysparkler/pyspark_22_to_23.py` & `pysparkler-0.9.dev1715454332/pysparkler/pyspark_22_to_23.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1715453058/pysparkler/pyspark_23_to_24.py` & `pysparkler-0.9.dev1715454332/pysparkler/pyspark_23_to_24.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1715453058/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.9.dev1715454332/pysparkler/pyspark_24_to_30.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1715453058/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.9.dev1715454332/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1715453058/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.9.dev1715454332/pysparkler/pyspark_32_to_33.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1715453058/pysparkler/sql_21_to_33.py` & `pysparkler-0.9.dev1715454332/pysparkler/sql_21_to_33.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.9.dev1715453058/PKG-INFO` & `pysparkler-0.9.dev1715454332/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.9.dev1715453058
+Version: 0.9.dev1715454332
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
```

