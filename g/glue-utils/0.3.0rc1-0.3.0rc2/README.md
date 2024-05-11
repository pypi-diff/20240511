# Comparing `tmp/glue_utils-0.3.0rc1.tar.gz` & `tmp/glue_utils-0.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_utils-0.3.0rc1.tar", max compression
+gzip compressed data, was "glue_utils-0.3.0rc2.tar", max compression
```

## Comparing `glue_utils-0.3.0rc1.tar` & `glue_utils-0.3.0rc2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.3.0rc1/LICENSE
--rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.3.0rc1/README.md
--rw-r--r--   0        0        0     3828 2024-05-10 13:50:37.609619 glue_utils-0.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0       92 2024-05-10 13:50:37.609951 glue_utils-0.3.0rc1/src/glue_utils/__init__.py
--rw-r--r--   0        0        0     1050 2024-05-10 09:44:26.756369 glue_utils-0.3.0rc1/src/glue_utils/options.py
--rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.3.0rc1/src/glue_utils/py.typed
--rw-r--r--   0        0        0      577 2024-05-10 13:36:16.852414 glue_utils-0.3.0rc1/src/glue_utils/pyspark/__init__.py
--rw-r--r--   0        0        0      674 2024-05-10 12:17:39.961510 glue_utils-0.3.0rc1/src/glue_utils/pyspark/context.py
--rw-r--r--   0        0        0     2652 2024-05-10 12:17:39.961783 glue_utils-0.3.0rc1/src/glue_utils/pyspark/job.py
--rw-r--r--   0        0        0      466 2024-05-10 13:35:53.859751 glue_utils-0.3.0rc1/src/glue_utils/pyspark/mixins/__init__.py
--rw-r--r--   0        0        0      849 2024-05-10 12:17:39.962157 glue_utils-0.3.0rc1/src/glue_utils/pyspark/mixins/connection_types.py
--rw-r--r--   0        0        0    10430 2024-05-10 13:45:45.636681 glue_utils-0.3.0rc1/src/glue_utils/pyspark/mixins/jdbc.py
--rw-r--r--   0        0        0    17339 2024-05-10 13:35:37.065435 glue_utils-0.3.0rc1/src/glue_utils/pyspark/mixins/s3.py
--rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 glue_utils-0.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.3.0rc2/LICENSE
+-rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.3.0rc2/README.md
+-rw-r--r--   0        0        0     3828 2024-05-11 15:43:48.344519 glue_utils-0.3.0rc2/pyproject.toml
+-rw-r--r--   0        0        0       92 2024-05-11 15:43:48.344882 glue_utils-0.3.0rc2/src/glue_utils/__init__.py
+-rw-r--r--   0        0        0     1050 2024-05-10 09:44:26.756369 glue_utils-0.3.0rc2/src/glue_utils/options.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.3.0rc2/src/glue_utils/py.typed
+-rw-r--r--   0        0        0      577 2024-05-10 13:36:16.852414 glue_utils-0.3.0rc2/src/glue_utils/pyspark/__init__.py
+-rw-r--r--   0        0        0      674 2024-05-10 12:17:39.961510 glue_utils-0.3.0rc2/src/glue_utils/pyspark/context.py
+-rw-r--r--   0        0        0     2652 2024-05-10 12:17:39.961783 glue_utils-0.3.0rc2/src/glue_utils/pyspark/job.py
+-rw-r--r--   0        0        0      466 2024-05-10 13:35:53.859751 glue_utils-0.3.0rc2/src/glue_utils/pyspark/mixins/__init__.py
+-rw-r--r--   0        0        0      849 2024-05-10 12:17:39.962157 glue_utils-0.3.0rc2/src/glue_utils/pyspark/mixins/connection_types.py
+-rw-r--r--   0        0        0     8981 2024-05-11 14:16:33.769298 glue_utils-0.3.0rc2/src/glue_utils/pyspark/mixins/jdbc.py
+-rw-r--r--   0        0        0    13057 2024-05-11 15:31:40.196489 glue_utils-0.3.0rc2/src/glue_utils/pyspark/mixins/s3.py
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 glue_utils-0.3.0rc2/PKG-INFO
```

### Comparing `glue_utils-0.3.0rc1/LICENSE` & `glue_utils-0.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.0rc1/README.md` & `glue_utils-0.3.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.0rc1/pyproject.toml` & `glue_utils-0.3.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-utils"
-version = "0.3.0rc1"
+version = "0.3.0rc2"
 package-mode = true
 description = "Reusable utilities for working with Glue PySpark jobs"
 authors = ["Noel Llevares <dashmug@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dashmug/glue-utils"
 repository = "https://github.com/dashmug/glue-utils/issues"
@@ -126,15 +126,15 @@
     "if TYPE_CHECKING:",
     "class .*\\bProtocol\\):",
     "@(abc\\.)?abstractmethod",
     "@overload",
 ]
 
 [tool.bumpver]
-current_version = "0.3.0rc1"
+current_version = "0.3.0rc2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "release: Bump version {old_version} -> {new_version}"
 commit = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
```

### Comparing `glue_utils-0.3.0rc1/src/glue_utils/options.py` & `glue_utils-0.3.0rc2/src/glue_utils/options.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.0rc1/src/glue_utils/pyspark/__init__.py` & `glue_utils-0.3.0rc2/src/glue_utils/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.0rc1/src/glue_utils/pyspark/context.py` & `glue_utils-0.3.0rc2/src/glue_utils/pyspark/context.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.0rc1/src/glue_utils/pyspark/job.py` & `glue_utils-0.3.0rc2/src/glue_utils/pyspark/job.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.0rc1/src/glue_utils/pyspark/mixins/connection_types.py` & `glue_utils-0.3.0rc2/src/glue_utils/pyspark/mixins/connection_types.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.0rc1/src/glue_utils/pyspark/mixins/jdbc.py` & `glue_utils-0.3.0rc2/src/glue_utils/pyspark/mixins/jdbc.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,53 +8,23 @@
     from awsglue.context import GlueContext
     from awsglue.dynamicframe import DynamicFrame
 
 
 class JDBCConnectionOptions(TypedDict, total=False):
     """Connection options for JDBC connections.
 
-    Parameters
-    ----------
-    useConnectionProperties : Literal["true"], optional
-        Whether to use connection properties. Defaults to None.
-    connectionName : str, optional
-        The name of the connection. Defaults to None.
-    url : str, optional
-        The JDBC URL. Defaults to None.
-    dbtable : str, optional
-        The name of the table. Defaults to None.
-    user : str, optional
-        The username for the connection. Defaults to None.
-    password : str, optional
-        The password for the connection. Defaults to None.
-    customJdbcDriverS3Path : str, optional
-        The S3 path for the custom JDBC driver. Defaults to None.
-    customJdbcDriverClassName : str, optional
-        The class name for the custom JDBC driver. Defaults to None.
-    bulkSize : int, optional
-        The bulk size for the connection. Defaults to None.
-    hashfield : str, optional
-        The hash field for the connection. Defaults to None.
-    hashexpression : str, optional
-        The hash expression for the connection. Defaults to None.
-    hashpartitions : int, optional
-        The number of hash partitions for the connection. Defaults to None.
-    sampleQuery : str, optional
-        The sample query for the connection. Defaults to None.
-    enablePartitioningForSampleQuery : bool, optional
-        Whether to enable partitioning for the sample query. Defaults to None.
-    sampleSize : int, optional
-        The sample size for the connection. Defaults to None.
-
-    Reference: https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-connect-jdbc-home.html
+    Reference
+    ---------
+    - https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-connect-jdbc-home.html
 
     """
 
     useConnectionProperties: Literal["true"]
     connectionName: str
+    databaseName: str
     url: str
     dbtable: str
     user: str
     password: str
     customJdbcDriverS3Path: str
     customJdbcDriverClassName: str
     bulkSize: int
```

### Comparing `glue_utils-0.3.0rc1/PKG-INFO` & `glue_utils-0.3.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-utils
-Version: 0.3.0rc1
+Version: 0.3.0rc2
 Summary: Reusable utilities for working with Glue PySpark jobs
 Home-page: https://github.com/dashmug/glue-utils
 License: MIT
 Keywords: aws,glue,pyspark,spark,etl,data,data-engineering
 Author: Noel Llevares
 Author-email: dashmug@gmail.com
 Requires-Python: >=3.9,<4.0
```

