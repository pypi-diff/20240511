# Comparing `tmp/cuallee-0.9.1.tar.gz` & `tmp/cuallee-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuallee-0.9.1.tar", last modified: Fri Mar 22 20:53:31 2024, max compression
+gzip compressed data, was "cuallee-0.9.2.tar", last modified: Sat Mar 23 09:44:51 2024, max compression
```

## Comparing `cuallee-0.9.1.tar` & `cuallee-0.9.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-22 20:53:31.929852 cuallee-0.9.1/
--rw-rw-r--   0 herminio  (1000) herminio  (1000)    11357 2022-09-20 23:24:07.000000 cuallee-0.9.1/LICENSE
--rw-r--r--   0 herminio  (1000) herminio  (1000)    31368 2024-03-22 20:53:31.929852 cuallee-0.9.1/PKG-INFO
--rw-r--r--   0 herminio  (1000) herminio  (1000)    16613 2024-03-22 20:34:11.000000 cuallee-0.9.1/README.md
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-22 20:53:31.929852 cuallee-0.9.1/cuallee/
--rw-r--r--   0 herminio  (1000) herminio  (1000)    27161 2024-03-22 20:17:39.000000 cuallee-0.9.1/cuallee/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    10379 2024-03-17 20:02:28.000000 cuallee-0.9.1/cuallee/bigquery_validation.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-22 20:53:31.929852 cuallee-0.9.1/cuallee/cloud/
--rw-r--r--   0 herminio  (1000) herminio  (1000)     1485 2024-03-17 20:02:28.000000 cuallee-0.9.1/cuallee/cloud/__init__.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-22 20:53:31.929852 cuallee-0.9.1/cuallee/dagster/
--rw-r--r--   0 herminio  (1000) herminio  (1000)      865 2024-02-10 17:13:08.000000 cuallee-0.9.1/cuallee/dagster/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    10147 2024-03-17 20:02:28.000000 cuallee-0.9.1/cuallee/duckdb_validation.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-22 20:53:31.929852 cuallee-0.9.1/cuallee/iso/
--rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2023-06-03 15:46:05.000000 cuallee-0.9.1/cuallee/iso/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)     2298 2024-02-11 20:37:09.000000 cuallee-0.9.1/cuallee/iso/checks.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    13541 2024-03-17 20:02:28.000000 cuallee-0.9.1/cuallee/pandas_validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    18222 2024-03-17 20:02:28.000000 cuallee-0.9.1/cuallee/polars_validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    29188 2024-03-22 20:34:30.000000 cuallee-0.9.1/cuallee/pyspark_validation.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-22 20:53:31.929852 cuallee-0.9.1/cuallee/report/
--rw-r--r--   0 herminio  (1000) herminio  (1000)      714 2024-03-17 20:38:19.000000 cuallee-0.9.1/cuallee/report/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    30292 2024-03-17 20:02:28.000000 cuallee-0.9.1/cuallee/snowpark_validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)     2302 2023-09-16 13:10:27.000000 cuallee-0.9.1/cuallee/utils.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-22 20:53:31.929852 cuallee-0.9.1/cuallee.egg-info/
--rw-r--r--   0 herminio  (1000) herminio  (1000)    31368 2024-03-22 20:53:31.000000 cuallee-0.9.1/cuallee.egg-info/PKG-INFO
--rw-r--r--   0 herminio  (1000) herminio  (1000)      539 2024-03-22 20:53:31.000000 cuallee-0.9.1/cuallee.egg-info/SOURCES.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)        1 2024-03-22 20:53:31.000000 cuallee-0.9.1/cuallee.egg-info/dependency_links.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)      430 2024-03-22 20:53:31.000000 cuallee-0.9.1/cuallee.egg-info/requires.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)        8 2024-03-22 20:53:31.000000 cuallee-0.9.1/cuallee.egg-info/top_level.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)     1400 2024-03-22 20:15:50.000000 cuallee-0.9.1/pyproject.toml
--rw-r--r--   0 herminio  (1000) herminio  (1000)      109 2024-03-22 20:53:31.929852 cuallee-0.9.1/setup.cfg
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-23 09:44:51.740040 cuallee-0.9.2/
+-rw-rw-r--   0 herminio  (1000) herminio  (1000)    11357 2022-09-20 23:24:07.000000 cuallee-0.9.2/LICENSE
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    31369 2024-03-23 09:44:51.740040 cuallee-0.9.2/PKG-INFO
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    16613 2024-03-23 09:13:11.000000 cuallee-0.9.2/README.md
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-23 09:44:51.736707 cuallee-0.9.2/cuallee/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    27161 2024-03-23 09:44:33.000000 cuallee-0.9.2/cuallee/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    10379 2024-03-17 20:02:28.000000 cuallee-0.9.2/cuallee/bigquery_validation.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-23 09:44:51.736707 cuallee-0.9.2/cuallee/cloud/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     1485 2024-03-17 20:02:28.000000 cuallee-0.9.2/cuallee/cloud/__init__.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-23 09:44:51.736707 cuallee-0.9.2/cuallee/dagster/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      865 2024-02-10 17:13:08.000000 cuallee-0.9.2/cuallee/dagster/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    10147 2024-03-17 20:02:28.000000 cuallee-0.9.2/cuallee/duckdb_validation.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-23 09:44:51.736707 cuallee-0.9.2/cuallee/iso/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2023-06-03 15:46:05.000000 cuallee-0.9.2/cuallee/iso/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     2298 2024-02-11 20:37:09.000000 cuallee-0.9.2/cuallee/iso/checks.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    13541 2024-03-17 20:02:28.000000 cuallee-0.9.2/cuallee/pandas_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    18232 2024-03-23 09:16:16.000000 cuallee-0.9.2/cuallee/polars_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    29188 2024-03-23 09:13:11.000000 cuallee-0.9.2/cuallee/pyspark_validation.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-23 09:44:51.736707 cuallee-0.9.2/cuallee/report/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      714 2024-03-17 20:38:19.000000 cuallee-0.9.2/cuallee/report/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    30292 2024-03-17 20:02:28.000000 cuallee-0.9.2/cuallee/snowpark_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     2302 2023-09-16 13:10:27.000000 cuallee-0.9.2/cuallee/utils.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2024-03-23 09:44:51.736707 cuallee-0.9.2/cuallee.egg-info/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    31369 2024-03-23 09:44:51.000000 cuallee-0.9.2/cuallee.egg-info/PKG-INFO
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      539 2024-03-23 09:44:51.000000 cuallee-0.9.2/cuallee.egg-info/SOURCES.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        1 2024-03-23 09:44:51.000000 cuallee-0.9.2/cuallee.egg-info/dependency_links.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      431 2024-03-23 09:44:51.000000 cuallee-0.9.2/cuallee.egg-info/requires.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        8 2024-03-23 09:44:51.000000 cuallee-0.9.2/cuallee.egg-info/top_level.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     1401 2024-03-23 09:44:33.000000 cuallee-0.9.2/pyproject.toml
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      109 2024-03-23 09:44:51.740040 cuallee-0.9.2/setup.cfg
```

### Comparing `cuallee-0.9.1/LICENSE` & `cuallee-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cuallee-0.9.1/PKG-INFO` & `cuallee-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuallee
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame.
 Author-email: Herminio Vazquez <canimus@gmail.com>, Virginie Grosboillot <vestalisvirginis@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -211,16 +211,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toolz>=0.12.0
 Requires-Dist: requests>=2.28
 Provides-Extra: dev
-Requires-Dist: black==24.2.0; extra == "dev"
-Requires-Dist: ruff==0.3.2; extra == "dev"
+Requires-Dist: black==24.3.0; extra == "dev"
+Requires-Dist: ruff==0.3.3; extra == "dev"
 Provides-Extra: pyspark
 Requires-Dist: pyspark>=3.4.0; extra == "pyspark"
 Provides-Extra: pyspark-connect
 Requires-Dist: pyspark[connect]; extra == "pyspark-connect"
 Provides-Extra: snowpark
 Requires-Dist: snowflake-snowpark-python==1.11.1; extra == "snowpark"
 Requires-Dist: pyarrow>=14.0.2; extra == "snowpark"
@@ -234,15 +234,15 @@
 Provides-Extra: polars
 Requires-Dist: polars>=0.19.6; extra == "polars"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pendulum>=2.1.2; extra == "test"
 Provides-Extra: dagster
-Requires-Dist: dagster==1.6.9; extra == "dagster"
+Requires-Dist: dagster==1.6.11; extra == "dagster"
 Provides-Extra: cloud
 Requires-Dist: msgpack==1.0.8; extra == "cloud"
 Provides-Extra: pdf
 Requires-Dist: fpdf2==2.7.8; extra == "pdf"
 
 # cuallee
```

### Comparing `cuallee-0.9.1/README.md` & `cuallee-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `cuallee-0.9.1/cuallee/__init__.py` & `cuallee-0.9.2/cuallee/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import datetime, timedelta, timezone
 from types import ModuleType
 from typing import Any, Dict, List, Literal, Optional, Protocol, Tuple, Union
 from toolz import compose, valfilter  # type: ignore
 from toolz.curried import map as map_curried
 
 logger = logging.getLogger("cuallee")
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 # Verify Libraries Available
 # ==========================
 try:
     from pandas import DataFrame as pandas_dataframe  # type: ignore
 except (ModuleNotFoundError, ImportError):
     logger.debug("KO: Pandas")
```

### Comparing `cuallee-0.9.1/cuallee/bigquery_validation.py` & `cuallee-0.9.2/cuallee/bigquery_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.9.1/cuallee/cloud/__init__.py` & `cuallee-0.9.2/cuallee/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.9.1/cuallee/dagster/__init__.py` & `cuallee-0.9.2/cuallee/dagster/__init__.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.9.1/cuallee/duckdb_validation.py` & `cuallee-0.9.2/cuallee/duckdb_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.9.1/cuallee/iso/checks.py` & `cuallee-0.9.2/cuallee/iso/checks.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.9.1/cuallee/pandas_validation.py` & `cuallee-0.9.2/cuallee/pandas_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.9.1/cuallee/polars_validation.py` & `cuallee-0.9.2/cuallee/polars_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,30 +34,30 @@
         )
 
     def are_complete(self, rule: Rule, dataframe: pl.DataFrame) -> Union[bool, int]:
         """Validate absence of null in group of columns"""
         return Compute._result(
             dataframe.select(
                 [pl.col(c).is_not_null().cast(pl.Int8).sum() for c in rule.column]
-            ).sum(axis=1)
+            ).sum_horizontal()
             / len(rule.column)
         )
 
     def is_unique(self, rule: Rule, dataframe: pl.DataFrame) -> Union[bool, int]:
         """Validate absence of duplicates"""
         return Compute._result(
             dataframe.select(pl.col(rule.column).is_unique().cast(pl.Int8)).sum()
         )
 
     def are_unique(self, rule: Rule, dataframe: pl.DataFrame) -> Union[bool, int]:
         """Validate absence of duplicate in group of columns"""
         return Compute._result(
             dataframe.select(
                 [pl.col(c).is_unique().cast(pl.Int8).sum() for c in rule.column]
-            ).sum(axis=1)
+            ).sum_horizontal()
             / len(rule.column)
         )
 
     def is_greater_than(self, rule: Rule, dataframe: pl.DataFrame) -> Union[bool, int]:
         """Validate column values greater than threshold"""
         return Compute._result(
             dataframe.select(
```

### Comparing `cuallee-0.9.1/cuallee/pyspark_validation.py` & `cuallee-0.9.2/cuallee/pyspark_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.9.1/cuallee/report/__init__.py` & `cuallee-0.9.2/cuallee/report/__init__.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.9.1/cuallee/snowpark_validation.py` & `cuallee-0.9.2/cuallee/snowpark_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.9.1/cuallee/utils.py` & `cuallee-0.9.2/cuallee/utils.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.9.1/cuallee.egg-info/PKG-INFO` & `cuallee-0.9.2/cuallee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuallee
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame.
 Author-email: Herminio Vazquez <canimus@gmail.com>, Virginie Grosboillot <vestalisvirginis@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -211,16 +211,16 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toolz>=0.12.0
 Requires-Dist: requests>=2.28
 Provides-Extra: dev
-Requires-Dist: black==24.2.0; extra == "dev"
-Requires-Dist: ruff==0.3.2; extra == "dev"
+Requires-Dist: black==24.3.0; extra == "dev"
+Requires-Dist: ruff==0.3.3; extra == "dev"
 Provides-Extra: pyspark
 Requires-Dist: pyspark>=3.4.0; extra == "pyspark"
 Provides-Extra: pyspark-connect
 Requires-Dist: pyspark[connect]; extra == "pyspark-connect"
 Provides-Extra: snowpark
 Requires-Dist: snowflake-snowpark-python==1.11.1; extra == "snowpark"
 Requires-Dist: pyarrow>=14.0.2; extra == "snowpark"
@@ -234,15 +234,15 @@
 Provides-Extra: polars
 Requires-Dist: polars>=0.19.6; extra == "polars"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pendulum>=2.1.2; extra == "test"
 Provides-Extra: dagster
-Requires-Dist: dagster==1.6.9; extra == "dagster"
+Requires-Dist: dagster==1.6.11; extra == "dagster"
 Provides-Extra: cloud
 Requires-Dist: msgpack==1.0.8; extra == "cloud"
 Provides-Extra: pdf
 Requires-Dist: fpdf2==2.7.8; extra == "pdf"
 
 # cuallee
```

### Comparing `cuallee-0.9.1/cuallee.egg-info/SOURCES.txt` & `cuallee-0.9.2/cuallee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cuallee-0.9.1/pyproject.toml` & `cuallee-0.9.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cuallee"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
   { name="Herminio Vazquez", email="canimus@gmail.com"},
   { name="Virginie Grosboillot", email="vestalisvirginis@gmail.com" }
 ]
 license = {file = "LICENSE"}
 description = "Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame."
 readme = "README.md"
@@ -20,16 +20,16 @@
 dependencies = [
     "toolz >= 0.12.0",
     "requests>=2.28",
 ]
 
 [project.optional-dependencies]
 dev = [
-  "black==24.2.0",
-  "ruff==0.3.2"
+  "black==24.3.0",
+  "ruff==0.3.3"
 ]
 pyspark = [
   "pyspark>=3.4.0"
 ]
 pyspark_connect = [
   "pyspark[connect]"
 ]
@@ -52,15 +52,15 @@
 ]
 test = [
   "pytest",
   "pytest-cov",
   "pendulum >= 2.1.2"
 ]
 dagster = [
-  "dagster == 1.6.9"
+  "dagster == 1.6.11"
 ]
 cloud = [
   "msgpack == 1.0.8",
 ]
 pdf = [
   "fpdf2==2.7.8"
 ]
```

