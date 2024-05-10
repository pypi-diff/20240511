# Comparing `tmp/pypomes_db-0.6.7.tar.gz` & `tmp/pypomes_db-0.6.8.tar.gz`

## Comparing `pypomes_db-0.6.7.tar` & `pypomes_db-0.6.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    14492 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    25271 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    24910 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    15306 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    25271 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    24910 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/PKG-INFO
```

### Comparing `pypomes_db-0.6.7/src/pypomes_db/__init__.py` & `pypomes_db-0.6.8/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.7/src/pypomes_db/db_common.py` & `pypomes_db-0.6.8/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.7/src/pypomes_db/db_pomes.py` & `pypomes_db-0.6.8/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.7/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.6.8/src/pypomes_db/migration_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,19 @@
                                       start=1,
                                       finish=len(target_columns)+1)
         values: str = f"VALUES({raw_row})"
     cols: str = ", ".join(target_columns)
     insert_stmt = (f"INSERT INTO {target_table} "
                    f"({cols}) {values}")
 
+    _db_log(logger=logger,
+            engine=source_engine,
+            stmt=(f"Started migrating data, "
+                  f"from {source_engine}.{source_table} "
+                  f"to {target_engine}.{target_table}"))
     err_msg: str | None = None
     try:
         source_cursor: Any = curr_source_conn.cursor()
         target_cursor: Any = curr_target_conn.cursor()
         if target_engine == "sqlserver":
             target_cursor.fast_executemany = True
 
@@ -145,14 +150,19 @@
                                            sql=insert_stmt,
                                            argslist=cleaned_rows)
                 case "sqlserver":
                     target_cursor.executemany(insert_stmt, rows)
 
             # increment the tuple migration counter
             result += len(rows)
+            # read the next batch
+            if batch_size:
+                rows = source_cursor.fetchmany(size=batch_size)
+            else:
+                rows = source_cursor.fetchall()
 
         # close the cursors and commit the transactions
         source_cursor.close()
         curr_source_conn.commit()
         target_cursor.close()
         curr_target_conn.commit()
     except Exception as e:
@@ -171,15 +181,17 @@
             curr_target_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine=source_engine,
             err_msg=err_msg,
             errors=errors,
-            stmt=insert_stmt)
+            stmt=(f"{result} tuples migrated, "
+                  f"from {source_engine}.{source_table} "
+                  f"to {target_engine}.{target_table}"))
 
     return result
 
 def db_migrate_lobs(errors: list[str],
                     source_engine: str,
                     source_table: str,
                     source_column: str,
@@ -255,15 +267,19 @@
                                    columns=pk_columns,
                                    concat=" AND ",
                                    start_index=2)
     update_stmt = (f"UPDATE {target_table} "
                    f"SET {set_column} "
                    f"WHERE {where_columns}")
 
-
+    _db_log(logger=logger,
+            engine=source_engine,
+            stmt=(f"Started migrating LOBs, "
+                  f"from {source_engine}.{source_table}.{source_column} "
+                  f"to {target_engine}.{target_table}.{target_column}"))
     err_msg: str | None = None
     try:
         source_cursor: Any = curr_source_conn.cursor()
         target_cursor: Any = curr_target_conn.cursor()
 
         # execute the query
         source_cursor.execute(statement=sel_stmt)
@@ -306,25 +322,25 @@
     except Exception as e:
         # rollback the transactions
         if curr_source_conn:
             curr_source_conn.rollback()
         if curr_target_conn:
             curr_target_conn.rollback()
         err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
+                                 engine=source_engine)
     finally:
         # close the connections, if locally acquired
         if curr_source_conn and not source_conn:
             curr_source_conn.close()
         if curr_target_conn and not target_conn:
             curr_target_conn.close()
 
     # log the results
     _db_log(logger=logger,
             engine=source_engine,
             err_msg=err_msg,
             errors=errors,
             stmt=(f"{result} LOBs migrated, "
-                  f"from {source_engine} at {source_table}.{source_column} "
-                  f"to {target_engine} at {target_table}.{target_column}"))
+                  f"from {source_engine}.{source_table}.{source_column} "
+                  f"to {target_engine}.{target_table}.{target_column}"))
 
     return result
```

### Comparing `pypomes_db-0.6.7/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.6.8/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.7/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.6.8/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.7/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.6.8/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.7/LICENSE` & `pypomes_db-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.7/pyproject.toml` & `pypomes_db-0.6.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.6.7"
+version = "0.6.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.6.7/PKG-INFO` & `pypomes_db-0.6.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.6.7
+Version: 0.6.8
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

