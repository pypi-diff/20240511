# Comparing `tmp/pypomes_db-0.6.8.tar.gz` & `tmp/pypomes_db-0.6.9.tar.gz`

## Comparing `pypomes_db-0.6.8.tar` & `pypomes_db-0.6.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    15306 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    25271 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    24910 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    15238 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    25271 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    24853 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/PKG-INFO
```

### Comparing `pypomes_db-0.6.8/src/pypomes_db/__init__.py` & `pypomes_db-0.6.9/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.8/src/pypomes_db/db_common.py` & `pypomes_db-0.6.9/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.8/src/pypomes_db/db_pomes.py` & `pypomes_db-0.6.9/src/pypomes_db/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.8/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.6.9/src/pypomes_db/migration_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,16 +299,15 @@
                 match target_engine:
                     case "mysql":
                         pass
                     case "oracle":
                         target_cursor.execute(statement=update_stmt,
                                               parameters=(lob_data, *pk_vals))
                     case "postgres":
-                        target_cursor.execute(statement=update_stmt,
-                                              parameters=(PgBinary(lob_data), *pk_vals))
+                        target_cursor.execute(update_stmt, (PgBinary(lob_data), *pk_vals))
                     case "sqlserver":
                         target_cursor.execute(sql=update_stmt,
                                               params=(SqlsBinary(lob_data), *pk_vals))
                 # read the next chunk
                 lob_data = lob.read(chunk_size)
 
                 # increment the LOB migration counter
```

### Comparing `pypomes_db-0.6.8/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.6.9/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.8/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.6.9/src/pypomes_db/postgres_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -501,16 +501,15 @@
         with curr_conn.cursor() as cursor:
 
             # retrieve the lob data from file in chunks and write to the file
             lob_data : bytes
             with data_file.open("rb") as file:
                 lob_data = file.read(chunk_size)
                 while lob_data:
-                    cursor.execute(statement=update_stmt,
-                                   parameters=(Binary(lob_data), *pk_vals))
+                    cursor.execute(update_stmt, (Binary(lob_data), *pk_vals))
                     lob_data = file.read(chunk_size)
 
         # commit the transaction
         curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
```

### Comparing `pypomes_db-0.6.8/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.6.9/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.8/LICENSE` & `pypomes_db-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.8/pyproject.toml` & `pypomes_db-0.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.6.8"
+version = "0.6.9"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.6.8/PKG-INFO` & `pypomes_db-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.6.8
+Version: 0.6.9
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

