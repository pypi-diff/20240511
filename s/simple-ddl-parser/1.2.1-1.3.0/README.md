# Comparing `tmp/simple_ddl_parser-1.2.1.tar.gz` & `tmp/simple_ddl_parser-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_ddl_parser-1.2.1.tar", max compression
+gzip compressed data, was "simple_ddl_parser-1.3.0.tar", max compression
```

## Comparing `simple_ddl_parser-1.2.1.tar` & `simple_ddl_parser-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1093 2024-04-21 13:06:45.341924 simple_ddl_parser-1.2.1/LICENSE
--rw-r--r--   0        0        0    34808 2024-05-09 12:44:52.521015 simple_ddl_parser-1.2.1/docs/README.rst
--rw-r--r--   0        0        0     1597 2024-05-09 12:38:29.503259 simple_ddl_parser-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      268 2024-04-21 13:06:45.342548 simple_ddl_parser-1.2.1/simple_ddl_parser/__init__.py
--rw-r--r--   0        0        0     2326 2024-04-21 13:06:45.342619 simple_ddl_parser-1.2.1/simple_ddl_parser/cli.py
--rwxr-xr-x   0        0        0     8860 2024-05-09 12:29:34.312314 simple_ddl_parser-1.2.1/simple_ddl_parser/ddl_parser.py
--rw-r--r--   0        0        0      755 2024-04-21 13:06:45.342889 simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/__init__.py
--rw-r--r--   0        0        0      702 2024-04-21 13:06:45.342962 simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/bigquery.py
--rw-r--r--   0        0        0     5326 2024-04-21 18:02:06.063289 simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/hql.py
--rw-r--r--   0        0        0      260 2024-04-21 13:06:45.343230 simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/ibm.py
--rw-r--r--   0        0        0     2608 2024-04-21 13:06:45.343300 simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/mssql.py
--rw-r--r--   0        0        0      510 2024-05-09 11:52:40.501830 simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/mysql.py
--rw-r--r--   0        0        0     2145 2024-05-09 12:29:34.312658 simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/oracle.py
--rw-r--r--   0        0        0      426 2024-04-21 13:06:45.343551 simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/psql.py
--rw-r--r--   0        0        0      928 2024-04-21 13:06:45.343627 simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/redshift.py
--rw-r--r--   0        0        0     7278 2024-04-21 18:13:32.614147 simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/snowflake.py
--rw-r--r--   0        0        0      305 2024-04-21 13:06:45.344047 simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/spark_sql.py
--rw-r--r--   0        0        0    57779 2024-05-09 12:29:34.313079 simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/sql.py
--rw-r--r--   0        0        0    13207 2024-04-21 13:06:45.344438 simple_ddl_parser-1.2.1/simple_ddl_parser/output/base_data.py
--rw-r--r--   0        0        0     5306 2024-04-21 13:06:45.344678 simple_ddl_parser-1.2.1/simple_ddl_parser/output/core.py
--rw-r--r--   0        0        0     9553 2024-05-09 12:29:34.313465 simple_ddl_parser-1.2.1/simple_ddl_parser/output/dialects.py
--rw-r--r--   0        0        0     2840 2024-04-21 13:06:45.345129 simple_ddl_parser-1.2.1/simple_ddl_parser/output/table_data.py
--rwxr-xr-x   0        0        0    13223 2024-05-09 11:53:06.889442 simple_ddl_parser-1.2.1/simple_ddl_parser/parser.py
--rw-r--r--   0        0        0   275364 2024-05-09 12:30:17.435558 simple_ddl_parser-1.2.1/simple_ddl_parser/parsetab.py
--rw-r--r--   0        0        0      247 2024-05-09 12:19:31.247646 simple_ddl_parser-1.2.1/simple_ddl_parser/test.py
--rw-r--r--   0        0        0     3133 2024-05-09 12:29:34.315259 simple_ddl_parser-1.2.1/simple_ddl_parser/tokens.py
--rw-r--r--   0        0        0     1391 2024-04-21 13:06:45.346777 simple_ddl_parser-1.2.1/simple_ddl_parser/utils.py
--rw-r--r--   0        0        0    36287 1970-01-01 00:00:00.000000 simple_ddl_parser-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-04-21 13:06:45.341924 simple_ddl_parser-1.3.0/LICENSE
+-rw-r--r--   0        0        0    35559 2024-05-11 16:48:17.709811 simple_ddl_parser-1.3.0/docs/README.rst
+-rw-r--r--   0        0        0     1597 2024-05-11 15:54:23.475914 simple_ddl_parser-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      268 2024-04-21 13:06:45.342548 simple_ddl_parser-1.3.0/simple_ddl_parser/__init__.py
+-rw-r--r--   0        0        0     2326 2024-04-21 13:06:45.342619 simple_ddl_parser-1.3.0/simple_ddl_parser/cli.py
+-rwxr-xr-x   0        0        0     8860 2024-05-11 15:54:06.836621 simple_ddl_parser-1.3.0/simple_ddl_parser/ddl_parser.py
+-rw-r--r--   0        0        0      755 2024-04-21 13:06:45.342889 simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/__init__.py
+-rw-r--r--   0        0        0      702 2024-04-21 13:06:45.342962 simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/bigquery.py
+-rw-r--r--   0        0        0     5326 2024-04-21 18:02:06.063289 simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/hql.py
+-rw-r--r--   0        0        0      260 2024-04-21 13:06:45.343230 simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/ibm.py
+-rw-r--r--   0        0        0     2608 2024-04-21 13:06:45.343300 simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/mssql.py
+-rw-r--r--   0        0        0      510 2024-05-09 11:52:40.501830 simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/mysql.py
+-rw-r--r--   0        0        0     2145 2024-05-09 12:49:40.928963 simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/oracle.py
+-rw-r--r--   0        0        0      711 2024-05-11 16:32:31.477467 simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/psql.py
+-rw-r--r--   0        0        0      928 2024-04-21 13:06:45.343627 simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/redshift.py
+-rw-r--r--   0        0        0     7278 2024-04-21 18:13:32.614147 simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/snowflake.py
+-rw-r--r--   0        0        0      305 2024-04-21 13:06:45.344047 simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/spark_sql.py
+-rw-r--r--   0        0        0    59004 2024-05-11 16:45:20.555170 simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/sql.py
+-rw-r--r--   0        0        0    13207 2024-04-21 13:06:45.344438 simple_ddl_parser-1.3.0/simple_ddl_parser/output/base_data.py
+-rw-r--r--   0        0        0     5306 2024-04-21 13:06:45.344678 simple_ddl_parser-1.3.0/simple_ddl_parser/output/core.py
+-rw-r--r--   0        0        0     9553 2024-05-09 12:49:40.930396 simple_ddl_parser-1.3.0/simple_ddl_parser/output/dialects.py
+-rw-r--r--   0        0        0     2840 2024-04-21 13:06:45.345129 simple_ddl_parser-1.3.0/simple_ddl_parser/output/table_data.py
+-rwxr-xr-x   0        0        0    13223 2024-05-09 11:53:06.889442 simple_ddl_parser-1.3.0/simple_ddl_parser/parser.py
+-rw-r--r--   0        0        0   969067 2024-05-11 16:42:28.393010 simple_ddl_parser-1.3.0/simple_ddl_parser/parsetab.py
+-rw-r--r--   0        0        0      253 2024-05-11 16:31:33.742597 simple_ddl_parser-1.3.0/simple_ddl_parser/test.py
+-rw-r--r--   0        0        0     3148 2024-05-11 15:47:21.631201 simple_ddl_parser-1.3.0/simple_ddl_parser/tokens.py
+-rw-r--r--   0        0        0     1391 2024-04-21 13:06:45.346777 simple_ddl_parser-1.3.0/simple_ddl_parser/utils.py
+-rw-r--r--   0        0        0    37038 1970-01-01 00:00:00.000000 simple_ddl_parser-1.3.0/PKG-INFO
```

### Comparing `simple_ddl_parser-1.2.1/LICENSE` & `simple_ddl_parser-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/docs/README.rst` & `simple_ddl_parser-1.3.0/docs/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -545,14 +545,41 @@
 
 * https://github.com/ankitdata ,
 * https://github.com/kalyan939
 
 Changelog
 ---------
 
+**v1.3.0**
+
+Fixes
+^^^^^
+
+PostgreSQL:
+
+
+#. Timezone was moved out from type definition to keyword 'with_time_zone' it can be True (if with time zone) or False (if without)
+   BigQuery:
+#. Previously Range in RANGE_BUCKETS was parsed as a columns, now this behaviour is changed and
+   range placed in own keyword - 'range' (can be array or str).
+   Also for all ```*_TRUNC PARTITIONS`` like DATETIME_TRUNC, TIMESTAMP_TRUNC, etc, second argument moved to arg 'trunc_by'
+
+Improvements
+^^^^^^^^^^^^
+
+PostgreSQL:
+
+
+#. Added support for PostgreSQL with / without time zone - https://github.com/xnuinside/simple-ddl-parser/issues/250
+
+BigQuery:
+
+
+#. Added support for GENERATE_ARRAY in RANGE_BUCKETS https://github.com/xnuinside/simple-ddl-parser/issues/183
+
 **v1.2.1**
 
 Fixes
 ^^^^^
 
 MySQL:
```

### Comparing `simple_ddl_parser-1.2.1/pyproject.toml` & `simple_ddl_parser-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simple-ddl-parser"
-version = "1.2.1"
+version = "1.3.0"
 description = "Simple DDL Parser to parse SQL & dialects like HQL, TSQL (MSSQL), Oracle, AWS Redshift, Snowflake, MySQL, PostgreSQL, etc ddl files to json/python dict with full information about columns: types, defaults, primary keys, etc.; sequences, alters, custom types & other entities from ddl."
 authors = ["Iuliia Volkova <xnuinside@gmail.com>"]
 license = "MIT"
 readme = "docs/README.rst"
 homepage = "https://github.com/xnuinside/simple-ddl-parser"
 repository = "https://github.com/xnuinside/simple-ddl-parser"
 classifiers = [
```

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/cli.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/cli.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/ddl_parser.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/ddl_parser.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/__init__.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/bigquery.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/bigquery.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/hql.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/hql.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/mssql.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/mssql.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/oracle.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/oracle.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/redshift.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/redshift.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/snowflake.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/snowflake.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/dialects/sql.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/dialects/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,64 @@
 
 from simple_ddl_parser.utils import check_spec, remove_par
 
 auth = "AUTHORIZATION"
 
 
 class AfterColumns:
+    @staticmethod
+    def _parse_range_bucket(data: List[str]) -> Tuple[List[str], List[str]]:
+        range = None
+
+        if len(data) == 3:
+            columns = data[0]
+            range = data[2]
+        else:
+            columns = []
+            for column in data[0]:
+                if "[" in column:
+                    range = [column.replace("[", "")]
+                elif range:
+                    range.append(column.replace("]", ""))
+                else:
+                    columns.append(column)
+        return columns, range
+
     def p_expression_partition_by(self, p: List) -> None:
         """expr : expr PARTITION BY LP pid RP
         | expr PARTITION BY id LP pid RP
         | expr PARTITION BY pid
-        | expr PARTITION BY id pid"""
+        | expr PARTITION BY id pid
+        | expr PARTITION BY id LP pid COMMA f_call RP
+        """
         p[0] = p[1]
-        p_list = list(p)
-        _type = None
-        if isinstance(p[4], list):
-            columns = p[4]
-        else:
-            columns = p_list[-2]
-        if isinstance(p[4], str) and p[4].lower() != "(":
-            _type = p[4]
+        p_list = remove_par(list(p))
+        _type, range, trunc_by = None, None, None
+
+        if isinstance(p_list[4], list):
+            columns = p_list[4]
+        elif "_TRUNC" in p_list[4]:
+            # bigquery
+            _type = p_list[4]
+            trunc_by = p_list[5][-1]
+            p_list[5].pop(-1)
+            columns = p_list[5]
+        elif p_list[4].upper() == "RANGE_BUCKET":
+            # bigquery RANGE_BUCKET with GENERATE_ARRAY
+            _type = p_list[4]
+            columns, range = self._parse_range_bucket(p_list[5:])
+        else:
+            columns = p_list[-1]
+        if not _type and isinstance(p_list[4], str):
+            _type = p_list[4]
         p[0]["partition_by"] = {"columns": columns, "type": _type}
+        if range:
+            p[0]["partition_by"]["range"] = range
+        if trunc_by:
+            p[0]["partition_by"]["trunc_by"] = trunc_by
 
 
 class Database:
     def p_expression_create_database(self, p: List) -> None:
         """expr : expr database_base"""
         p[0] = p[1]
         p_list = list(p)
@@ -415,14 +450,15 @@
         | defcolumn autoincrement
         | defcolumn option_order_noorder
         | defcolumn option_with_tag
         | defcolumn option_with_masking_policy
         | defcolumn as_virtual
         | defcolumn constraint
         | defcolumn generated_by
+        | defcolumn timezone
         """
         p[0] = p[1]
         p_list = list(p)
 
         pk, default, unique, references, nullable = self.get_column_properties(p_list)
 
         self.set_property(p)
```

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/output/base_data.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/output/base_data.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/output/core.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/output/core.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/output/dialects.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/output/dialects.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/output/table_data.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/output/table_data.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/parser.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/tokens.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/tokens.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     "ENFORCED",
     "ENCODE",
     "GENERATED",
     "COMMENT",
     "POLICY",
     "MASKING",
     "WITH",
+    "WITHOUT",
     "ORDER",
     "NOORDER",
     "VISIBLE",
     "INVISIBLE",
     "AUTOINCREMENT",
     "GENERATED",
     "BY",
```

### Comparing `simple_ddl_parser-1.2.1/simple_ddl_parser/utils.py` & `simple_ddl_parser-1.3.0/simple_ddl_parser/utils.py`

 * *Files identical despite different names*

### Comparing `simple_ddl_parser-1.2.1/PKG-INFO` & `simple_ddl_parser-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-ddl-parser
-Version: 1.2.1
+Version: 1.3.0
 Summary: Simple DDL Parser to parse SQL & dialects like HQL, TSQL (MSSQL), Oracle, AWS Redshift, Snowflake, MySQL, PostgreSQL, etc ddl files to json/python dict with full information about columns: types, defaults, primary keys, etc.; sequences, alters, custom types & other entities from ddl.
 Home-page: https://github.com/xnuinside/simple-ddl-parser
 License: MIT
 Author: Iuliia Volkova
 Author-email: xnuinside@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -574,14 +574,41 @@
 
 * https://github.com/ankitdata ,
 * https://github.com/kalyan939
 
 Changelog
 ---------
 
+**v1.3.0**
+
+Fixes
+^^^^^
+
+PostgreSQL:
+
+
+#. Timezone was moved out from type definition to keyword 'with_time_zone' it can be True (if with time zone) or False (if without)
+   BigQuery:
+#. Previously Range in RANGE_BUCKETS was parsed as a columns, now this behaviour is changed and
+   range placed in own keyword - 'range' (can be array or str).
+   Also for all ```*_TRUNC PARTITIONS`` like DATETIME_TRUNC, TIMESTAMP_TRUNC, etc, second argument moved to arg 'trunc_by'
+
+Improvements
+^^^^^^^^^^^^
+
+PostgreSQL:
+
+
+#. Added support for PostgreSQL with / without time zone - https://github.com/xnuinside/simple-ddl-parser/issues/250
+
+BigQuery:
+
+
+#. Added support for GENERATE_ARRAY in RANGE_BUCKETS https://github.com/xnuinside/simple-ddl-parser/issues/183
+
 **v1.2.1**
 
 Fixes
 ^^^^^
 
 MySQL:
```

