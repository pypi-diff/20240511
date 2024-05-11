# Comparing `tmp/dbmg-0.1.0.tar.gz` & `tmp/dbmg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbmg-0.1.0.tar", max compression
+gzip compressed data, was "dbmg-0.2.0.tar", max compression
```

## Comparing `dbmg-0.1.0.tar` & `dbmg-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1068 2024-05-04 13:39:30.020296 dbmg-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0       73 2024-05-11 17:44:04.340245 dbmg-0.1.0/README.md
--rw-r--r--   0        0        0      853 2024-05-11 18:02:35.559924 dbmg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2478 2024-05-11 17:56:00.410032 dbmg-0.1.0/src/dbmg.py
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 dbmg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-04 13:39:30.020296 dbmg-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0       73 2024-05-11 17:44:04.340245 dbmg-0.2.0/README.md
+-rw-r--r--   0        0        0      853 2024-05-11 18:03:33.519912 dbmg-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2468 2024-05-11 18:03:33.539912 dbmg-0.2.0/src/dbmg.py
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 dbmg-0.2.0/PKG-INFO
```

### Comparing `dbmg-0.1.0/LICENSE.txt` & `dbmg-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbmg-0.1.0/pyproject.toml` & `dbmg-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbmg"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Karl Rittner <k.rittner@hotmail.de>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dbmg-0.1.0/src/dbmg.py` & `dbmg-0.2.0/src/dbmg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from sqlalchemy import create_engine, Table, MetaData, text, insert, values, table, column, Integer
 import pandas as pd
 
 
-class DatabaseManagerPandas:
+class DataManager:
     def __init__(self, database_conf: dict):
         # conn = SqlAlchemyConnector.load("scrappy-sql-connector")
         # self.engine = create_engine('postgresql://scrappy_user:idaho777@localhost:5435/spy')
         # TODO need to check if it works the same way for bigquery and mysql
         self.engine = create_engine(
             f"{database_conf.get('database_type')}://{database_conf.get('user')}:{database_conf.get('password')}@{database_conf.get('host')}:{database_conf.get('port')}/{database_conf.get('database')}")
         self.conn = self.engine.connect()
```

### Comparing `dbmg-0.1.0/PKG-INFO` & `dbmg-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbmg
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Karl Rittner
 Author-email: k.rittner@hotmail.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

