# Comparing `tmp/pypomes_db-0.6.6.tar.gz` & `tmp/pypomes_db-0.6.7.tar.gz`

## Comparing `pypomes_db-0.6.6.tar` & `pypomes_db-0.6.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypomes_db-0.6.6/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 pypomes_db-0.6.6/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.6/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.6/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    25271 2020-02-02 00:00:00.000000 pypomes_db-0.6.6/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    24910 2020-02-02 00:00:00.000000 pypomes_db-0.6.6/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 pypomes_db-0.6.6/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.6/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    14492 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    25271 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    24910 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/PKG-INFO
```

### Comparing `pypomes_db-0.6.6/src/pypomes_db/db_pomes.py` & `pypomes_db-0.6.7/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.6/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.6.7/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.6/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.6.7/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.6/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.6.7/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.6/LICENSE` & `pypomes_db-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.6/pyproject.toml` & `pypomes_db-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.6.6"
+version = "0.6.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -20,15 +20,15 @@
 ]
 dependencies = [
     "pip>=24.0",
 #   "mysql-connector-python>=8.4.0",
 #   "oracledb>=2.2.0",
 #   "psycopg2-binary>=2.9.9",
 #   "pyodbc>=5.1.0",
-    "pypomes_core>=0.9.7",
+    "pypomes_core>=0.9.9",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

### Comparing `pypomes_db-0.6.6/PKG-INFO` & `pypomes_db-0.6.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.6.6
+Version: 0.6.7
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.9.7
+Requires-Dist: pypomes-core>=0.9.9
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

