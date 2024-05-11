# Comparing `tmp/pypomes_db-0.6.9.tar.gz` & `tmp/pypomes_db-0.7.0.tar.gz`

## Comparing `pypomes_db-0.6.9.tar` & `pypomes_db-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    38230 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    15238 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    25271 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    24853 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    29148 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    15850 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    15400 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    13760 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.7.0/PKG-INFO
```

### Comparing `pypomes_db-0.6.9/src/pypomes_db/__init__.py` & `pypomes_db-0.7.0/src/pypomes_db/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from .db_pomes import (
     db_setup, db_get_engines, db_get_params,
     db_assert_connection, db_connect, db_exists,
-    db_select_one, db_select_all, db_update,
-    db_delete, db_insert, db_bulk_insert, db_bulk_migrate,
-    db_update_lob, db_execute,
+    db_select_one, db_select_all, db_update, db_delete,
+    db_insert, db_bulk_insert, db_update_lob, db_execute,
     db_call_function, db_call_procedure,
 )
 from .migration_pomes import (
     db_migrate_data, db_migrate_lobs,
 )
 
 __all__ = [
     # db_pomes
     "db_setup", "db_get_engines", "db_get_params",
     "db_assert_connection", "db_connect", "db_exists",
-    "db_select_one", "db_select_all", "db_update",
-    "db_delete", "db_insert", "db_bulk_insert", "db_bulk_migrate",
-    "db_update_lob", "db_execute",
+    "db_select_one", "db_select_all", "db_update", "db_delete",
+    "db_insert", "db_bulk_insert", "db_update_lob", "db_execute",
     "db_call_function", "db_call_procedure",
     # migration_pomes
     "db_migrate_data", "db_migrate_lobs",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_db")
```

### Comparing `pypomes_db-0.6.9/src/pypomes_db/db_common.py` & `pypomes_db-0.7.0/src/pypomes_db/db_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-import uuid
 from logging import DEBUG, Logger
-from tempfile import gettempdir
-from pathlib import Path
 from pypomes_core import (
     APP_PREFIX,
     env_get_int, env_get_str, str_sanitize, str_get_positional
 )
 
 # the preferred way to specify database connection parameters is dynamically with 'db_setup_params'
 # specifying database connection parameters with environment variables can be done in two ways:
@@ -127,26 +124,14 @@
                                             engine=engine,
                                             bind_vals=where_vals)
             errors.append(f"{count} tuples returned, at least {require_min} expected, for '{msg}'")
 
     return result
 
 
-def _db_assert_temp_file(temp_file: str | Path) -> Path:
-
-    result: Path
-    if temp_file is None:
-        result = Path(gettempdir(), str(uuid.uuid4()) + ".bin")
-    elif isinstance(temp_file, str):
-        result = Path(temp_file)
-    else:
-        result = temp_file
-
-    return result
-
 def _db_get_params(engine: str) -> tuple:
     """
     Return the current connection parameters being used for *engine*.
 
     The connection parameters are returned as a *tuple*, with the elements
     *name*, *user*, *pwd*, *host*, *port*.
     The meaning of some parameters may vary between different database engines.
```

### Comparing `pypomes_db-0.6.9/src/pypomes_db/db_pomes.py` & `pypomes_db-0.7.0/src/pypomes_db/db_pomes.py`

 * *Files 12% similar despite different names*

```diff
@@ -436,179 +436,14 @@
                                                 insert_vals=insert_vals,
                                                 conn=conn,
                                                 logger=logger)
 
     return result
 
 
-def db_bulk_migrate(errors: list[str] | None,
-                    sel_stmt: str,
-                    insert_stmt: str,
-                    target_engine: str,
-                    batch_size: int = None,
-                    where_vals: tuple = None,
-                    target_conn: Any = None,
-                    engine: str = None,
-                    conn: Any = None,
-                    logger: Logger = None) -> int:
-    """
-    Bulk migrate data from one database to another database.
-
-    The destination database brand must be in the list of databases configured and supported by this package.
-
-    :param errors: incidental error messages
-    :param sel_stmt: SELECT command for the search
-    :param insert_stmt: the insert statement to use for bulk-inserting
-    :param target_engine: the destination database engine type
-    :param batch_size: number of tuples in the batch, or 0 or None for no limit
-    :param where_vals: the values to be associated with the search criteria
-    :param target_conn: the connection to the destination database
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param conn: optional connection to use (obtains a new one, if not specified)
-    :param logger: optional logger
-    :return: number of tuples effectively migrated
-    """
-    # initialize the return variable
-    result: int | None = None
-
-    curr_engine: str = _assert_engine(errors, engine)
-    if curr_engine == "mysql":
-        pass
-    elif curr_engine == "oracle":
-        from . import oracle_pomes
-        result = oracle_pomes.db_bulk_migrate(errors=errors,
-                                              sel_stmt=sel_stmt,
-                                              insert_stmt=insert_stmt,
-                                              batch_size=batch_size,
-                                              target_engine=target_engine,
-                                              where_vals=where_vals,
-                                              target_conn=target_conn,
-                                              conn=conn,
-                                              logger=logger)
-    elif curr_engine == "postgres":
-        from . import postgres_pomes
-        result = postgres_pomes.db_bulk_migrate(errors=errors,
-                                                sel_stmt=sel_stmt,
-                                                insert_stmt=insert_stmt,
-                                                batch_size=batch_size,
-                                                target_engine=target_engine,
-                                                where_vals=where_vals,
-                                                target_conn=target_conn,
-                                                conn=conn,
-                                                logger=logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        result = sqlserver_pomes.db_bulk_migrate(errors=errors,
-                                                 sel_stmt=sel_stmt,
-                                                 insert_stmt=insert_stmt,
-                                                 batch_size=batch_size,
-                                                 target_engine=target_engine,
-                                                 where_vals=where_vals,
-                                                 target_conn=target_conn,
-                                                 conn=conn,
-                                                 logger=logger)
-
-    return result
-
-
-def db_migrate_lobs(errors: list[str],
-                    lob_table: str,
-                    lob_column: str,
-                    pk_columns: list[str],
-                    target_engine: str,
-                    where_clause: tuple = None,
-                    temp_file: str | Path = None,
-                    chunk_size: int = None,
-                    target_table: str = None,
-                    target_column: str = None,
-                    target_conn: Any = None,
-                    engine: str = None,
-                    conn: Any = None,
-                    logger: Logger = None) -> int:
-    """
-    Migrate large binary objects (LOBs) from one database to another database.
-
-    The destination database must be in the list of databases configured and supported by this package.
-    One or more columns making up a primary key, or a unique row identifier, must exist on *lob_table*,
-    and be provided in *pk_columns*. It is assumed that the primary key columns have the same name,
-    and are of equivalent types, in both the origin and the destination database.
-    If *temp_file* is not provided, a plataform-specific temporary file is used.
-
-    :param errors: incidental error messages
-    :param lob_table: the table holding the LOBs
-    :param lob_column: the column holding the LOB
-    :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
-    :param target_engine: the destination database engine type
-    :param where_clause: the criteria for tuple selection
-    :param temp_file: temporary file to use (a file object or a valid file path)
-    :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
-    :param target_table: the table to write the lob to (defaults to the source table)
-    :param target_column: the column to write the lob to (defaults to the source column)
-    :param target_conn: the connection to the destination database
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param conn: optional connection to use (obtains a new one, if not specified)
-    :param logger: optional logger
-    :return: number of LOBs effectively migrated
-    """
-    # initialize the return variable
-    result: int | None = None
-
-    curr_engine: str = _assert_engine(errors, engine)
-    if curr_engine == "mysql":
-        pass
-    elif curr_engine == "oracle":
-        from . import oracle_pomes
-        result = oracle_pomes.db_migrate_lobs(errors=errors,
-                                              lob_table=lob_table,
-                                              lob_column=lob_column,
-                                              pk_columns=pk_columns,
-                                              target_engine=target_engine,
-                                              where_clause=where_clause,
-                                              temp_file=temp_file,
-                                              chunk_size=chunk_size,
-                                              target_table=target_table,
-                                              target_column=target_column,
-                                              target_conn=target_conn,
-                                              conn=conn,
-                                              logger=logger)
-    elif curr_engine == "postgres":
-        from . import postgres_pomes
-        result = postgres_pomes.db_migrate_lobs(errors=errors,
-                                                lob_table=lob_table,
-                                                lob_column=lob_column,
-                                                pk_columns=pk_columns,
-                                                target_engine=target_engine,
-                                                where_clause=where_clause,
-                                                temp_file=temp_file,
-                                                chunk_size=chunk_size,
-                                                target_table=target_table,
-                                                target_column=target_column,
-                                                target_conn=target_conn,
-                                                conn=conn,
-                                                logger=logger)
-    elif curr_engine == "sqlserver":
-        from . import sqlserver_pomes
-        pass
-        result = sqlserver_pomes.db_migrate_lobs(errors=errors,
-                                                 lob_table=lob_table,
-                                                 lob_column=lob_column,
-                                                 pk_columns=pk_columns,
-                                                 target_engine=target_engine,
-                                                 where_clause=where_clause,
-                                                 temp_file=temp_file,
-                                                 chunk_size=chunk_size,
-                                                 target_table=target_table,
-                                                 target_column=target_column,
-                                                 target_conn=target_conn,
-                                                 conn=conn,
-                                                 logger=logger)
-
-    return result
-
-
 def db_update_lob(errors: list[str],
                  lob_table: str,
                  lob_column: str,
                  pk_columns: list[str],
                  pk_vals: tuple,
                  lob_file: str | Path,
                  chunk_size: int,
```

### Comparing `pypomes_db-0.6.9/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.7.0/src/pypomes_db/migration_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,19 +77,22 @@
                                       start=1,
                                       finish=len(target_columns)+1)
         values: str = f"VALUES({raw_row})"
     cols: str = ", ".join(target_columns)
     insert_stmt = (f"INSERT INTO {target_table} "
                    f"({cols}) {values}")
 
+    # log the migration start
     _db_log(logger=logger,
             engine=source_engine,
             stmt=(f"Started migrating data, "
                   f"from {source_engine}.{source_table} "
                   f"to {target_engine}.{target_table}"))
+
+    # migrate the data
     err_msg: str | None = None
     try:
         source_cursor: Any = curr_source_conn.cursor()
         target_cursor: Any = curr_target_conn.cursor()
         if target_engine == "sqlserver":
             target_cursor.fast_executemany = True
 
@@ -112,24 +115,24 @@
                     result += len(rows)
                 case "postgres":
                     try:
                         execute_values(cur=target_cursor,
                                        sql=insert_stmt,
                                        argslist=rows)
                     except ValueError as e:
-                        # is the exception ValueError ?
+                        # is it a 'ValueError' exception on NULLs in strings ?
                         # ("A string literal cannot contain NUL (0x00) characters.")
                         if "contain NUL" in e.args[0]:
                             # yes, log the occurrence, remove the NULLs, and try again
                             _db_log(logger=logger,
                                     engine="postgres",
                                     level=WARNING,
                                     stmt=f"Found NULLs in values for {insert_stmt}")
                             # search for NULLs in input data
-                            cleaned_rows: list = []
+                            cleaned_rows: [tuple] = []
                             for raw_row in rows:
                                 is_cleaned: bool = False
                                 cleaned_row: list = []
                                 for val in raw_row:
                                     # is 'val' a string containing NULLs ?
                                     if isinstance(val, str) and val.count(chr(0)) > 0:
                                         # yes, clean it up and mark the row as cleaned
@@ -176,20 +179,20 @@
     finally:
         # close the connections, if locally acquired
         if curr_source_conn and not source_conn:
             curr_source_conn.close()
         if curr_target_conn and not target_conn:
             curr_target_conn.close()
 
-    # log the results
+    # log the migration finish
     _db_log(logger=logger,
             engine=source_engine,
             err_msg=err_msg,
             errors=errors,
-            stmt=(f"{result} tuples migrated, "
+            stmt=(f"Migrated {result} tuples, "
                   f"from {source_engine}.{source_table} "
                   f"to {target_engine}.{target_table}"))
 
     return result
 
 def db_migrate_lobs(errors: list[str],
                     source_engine: str,
@@ -255,31 +258,40 @@
     pks: str = ", ".join(pk_columns)
     sel_stmt: str = f"SELECT {pks}, {source_column} FROM {source_table}"
     if where_clause:
         sel_stmt += f" WHERE {where_clause}"
     blob_index: int = len(pk_columns)
 
     # build the UPDATE query
-    set_column = _db_bind_columns(engine=target_engine,
-                                  columns=[target_column],
-                                  concat=", ",
-                                  start_index=1)
-    where_columns = _db_bind_columns(engine=target_engine,
-                                   columns=pk_columns,
-                                   concat=" AND ",
-                                   start_index=2)
-    update_stmt = (f"UPDATE {target_table} "
-                   f"SET {set_column} "
-                   f"WHERE {where_columns}")
+    set_column: str = _db_bind_columns(engine=target_engine,
+                                       columns=[target_column],
+                                       concat=", ",
+                                       start_index=1)
+    where_columns: str = _db_bind_columns(engine=target_engine,
+                                          columns=pk_columns,
+                                          concat=" AND ",
+                                          start_index=2)
+    # insert the value
+    update_stmt_1: str = (f"UPDATE {target_table} "
+                          f"SET {set_column} "
+                          f"WHERE {where_columns}")
+    # append the value
+    update_stmt_2: str = (f"UPDATE {target_table} "
+                          f"SET {set_column[:len(target_column)+3]}"
+                          f"{target_column} || {set_column[len(target_column)+3:]} "
+                          f"WHERE {where_columns}")
 
+    # log the migration start
     _db_log(logger=logger,
             engine=source_engine,
             stmt=(f"Started migrating LOBs, "
                   f"from {source_engine}.{source_table}.{source_column} "
                   f"to {target_engine}.{target_table}.{target_column}"))
+
+    # migrate the LOBs
     err_msg: str | None = None
     try:
         source_cursor: Any = curr_source_conn.cursor()
         target_cursor: Any = curr_target_conn.cursor()
 
         # execute the query
         source_cursor.execute(statement=sel_stmt)
@@ -287,35 +299,39 @@
         # fetch rows
         for row in source_cursor:
 
             # retrieve the values of the primary key columns (leave blob column out)
             pk_vals: tuple = tuple([row[inx] for inx in range(blob_index)])
 
             # access the blob in chunks and write it to file
-            size: int = 0
+            offset: int = 1
+            update_stmt: str = update_stmt_1
             lob: Any = row[blob_index]
-            lob_data: bytes = lob.read(chunk_size)
+            lob_data: bytes = lob.read(offset=offset,
+                                       amount=chunk_size)
             while lob_data:
-                size += len(lob_data)
+                offset += len(lob_data)
                 match target_engine:
                     case "mysql":
                         pass
                     case "oracle":
                         target_cursor.execute(statement=update_stmt,
                                               parameters=(lob_data, *pk_vals))
                     case "postgres":
                         target_cursor.execute(update_stmt, (PgBinary(lob_data), *pk_vals))
                     case "sqlserver":
                         target_cursor.execute(sql=update_stmt,
                                               params=(SqlsBinary(lob_data), *pk_vals))
+                update_stmt = update_stmt_2
                 # read the next chunk
-                lob_data = lob.read(chunk_size)
+                lob_data = lob.read(offset=offset,
+                                    amount=chunk_size)
 
-                # increment the LOB migration counter
-                result += 1
+            # increment the LOB migration counter
+            result += 1
 
         # close the cursors and commit the transactions
         source_cursor.close()
         curr_source_conn.commit()
         target_cursor.close()
         curr_target_conn.commit()
     except Exception as e:
@@ -329,17 +345,17 @@
     finally:
         # close the connections, if locally acquired
         if curr_source_conn and not source_conn:
             curr_source_conn.close()
         if curr_target_conn and not target_conn:
             curr_target_conn.close()
 
-    # log the results
+    # log the migration finish
     _db_log(logger=logger,
             engine=source_engine,
             err_msg=err_msg,
             errors=errors,
-            stmt=(f"{result} LOBs migrated, "
+            stmt=(f"Migrated {result} LOBs, "
                   f"from {source_engine}.{source_table}.{source_column} "
                   f"to {target_engine}.{target_table}.{target_column}"))
 
     return result
```

### Comparing `pypomes_db-0.6.9/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.7.0/src/pypomes_db/postgres_pomes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # noinspection DuplicatedCode
 from logging import WARNING, Logger
 from pathlib import Path
 from psycopg2 import Binary, connect
-from psycopg2.extras import DictCursor, execute_values
+from psycopg2.extras import execute_values
 # noinspection PyProtectedMember
 from psycopg2._psycopg import connection
-from typing import Any
 
 from .db_common import (
-    _db_assert_query_quota, _db_assert_temp_file,
-    _db_get_params, _db_log, _db_except_msg
+    _db_assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
-from .db_pomes import db_bulk_insert as db_bulk_insert_to
-from .db_pomes import db_update_lob as db_update_lob_to
 
 
 def db_connect(errors: list[str],
                logger: Logger = None) -> connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
@@ -219,247 +215,14 @@
             err_msg=err_msg,
             errors=errors,
             stmt=insert_stmt)
 
     return result
 
 
-def db_bulk_migrate(errors: list[str],
-                    sel_stmt: str,
-                    insert_stmt: str,
-                    target_engine: str,
-                    batch_size: int,
-                    where_vals: tuple,
-                    target_conn: Any,
-                    conn: connection,
-                    logger: Logger) -> int:
-    """
-    Bulk migrate data from a Postgres database to another database.
-
-    The destination database brand must be in the list of databases configured and supported by this package.
-
-    :param errors: incidental error messages
-    :param sel_stmt: SELECT command for the search
-    :param insert_stmt: the insert statement to use for bulk-inserting
-    :param target_engine: the destination database engine type
-    :param batch_size: number of tuples in the batch, or 0 or None for no limit
-    :param where_vals: the values to be associated with the search criteria
-    :param target_conn: the connection to the destination database
-    :param conn: optional connection to use (obtains a new one, if not specified)
-    :param logger: optional logger
-    :return: number of tuples effectively migrated
-    """
-    # initialize the return variable
-    result: int = 0
-
-    # make sure to have a connection
-    curr_conn: connection = conn or db_connect(errors=errors,
-                                               logger=logger)
-
-    err_msg: str | None = None
-    try:
-        with curr_conn.cursor() as cursor:
-
-            # execute the query
-            cursor.execute(statement=sel_stmt,
-                           parameters=where_vals)
-
-            # fetch rows in batches/all rows
-            op_errors: list[str] = []
-            rows: list[tuple]
-            if batch_size:
-                rows = cursor.fetchmany(batch_size)
-            else:
-                rows = cursor.fetchall()
-            while rows:
-                result += db_bulk_insert_to(errors=op_errors,
-                                            insert_stmt=insert_stmt,
-                                            insert_vals=rows,
-                                            engine=target_engine,
-                                            conn=target_conn,
-                                            logger=logger) or 0
-                # errors ?
-                if op_errors:
-                    # yes, register them and abort the operation
-                    errors.extend(op_errors)
-                    break
-                if not batch_size:
-                    break
-                rows = cursor.fetchmany(batch_size)
-
-        # commit the source and target transactions
-        curr_conn.commit()
-        if target_conn:
-          target_conn.commit()
-    except Exception as e:
-        if curr_conn:
-            curr_conn.rollback()
-        if target_conn:
-            target_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
-    finally:
-        # close the connection, if locally acquired
-        if curr_conn and not conn:
-            curr_conn.close()
-
-    # log the results
-    _db_log(logger=logger,
-            engine="postgres",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=sel_stmt,
-            bind_vals=where_vals)
-    _db_log(logger=logger,
-            engine="postgres",
-            stmt=(f"{result} tuples migrated, "
-                        f"from postgres to {target_engine}"))
-
-    return result
-
-
-def db_migrate_lobs(errors: list[str],
-                    lob_table: str,
-                    lob_column: str,
-                    pk_columns: list[str],
-                    target_engine: str,
-                    where_clause: tuple,
-                    temp_file: str | Path,
-                    chunk_size: int,
-                    target_table: str,
-                    target_column: str,
-                    target_conn: Any,
-                    conn: connection,
-                    logger: Logger) -> int:
-    """
-    Migrate large binary objects (LOBs) from a Postgres database to another database.
-
-    The destination database must be in the list of databases configured and supported by this package.
-    One or more columns making up a primary key, or a unique row identifier, must exist on *lob_table*,
-    and be provided in *pk_columns*. It is assumed that the primary key columns have the same name,
-    and are of equivalent types, in both the origin and the destination database.
-    If *temp_file* is not provided, a plataform-specific temporary file is used.
-
-    :param errors: incidental error messages
-    :param lob_table: the table holding the LOBs
-    :param lob_column: the column holding the LOB
-    :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
-    :param target_engine: the destination database engine type
-    :param where_clause: the criteria for tuple selection
-    :param temp_file: temporary file to use (a file object or a valid file path)
-    :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
-    :param target_table: the table to write the lob to (defaults to the source table)
-    :param target_column: the column to write the lob to (defaults to the source column)
-    :param target_conn: the connection to the destination database
-    :param conn: optional connection to use (obtains a new one, if not specified)
-    :param logger: optional logger
-    :return: number of LOBs effectively migrated
-    """
-    # initialize the return variable
-    result: int = 0
-
-    # make sure to have a connection
-    curr_conn: connection = conn or db_connect(errors=errors,
-                                               logger=logger)
-
-    # make sure to have a target table
-    if not target_table:
-        target_table = lob_table
-
-    # make sure to have a target column
-    if not target_column:
-        target_column = lob_column
-
-    # make sure to have a temporary file
-    lob_file: Path = _db_assert_temp_file(temp_file)
-
-    # normalize the chunk size
-    if not chunk_size:
-        chunk_size = -1
-
-    # buid the query
-    pks: str = ", ".join(pk_columns)
-    sel_stmt: str = f"SELECT {pks}, {lob_column} FROM {lob_table}"
-    if where_clause:
-        sel_stmt += f" WHERE {where_clause}"
-    blob_index: int = len(pk_columns)
-
-    err_msg: str | None = None
-    try:
-        with curr_conn.cursor(cursor_factory=DictCursor) as cursor:
-
-            # execute the query
-            cursor.execute(statement=sel_stmt)
-
-            # fetch rows
-            for row in cursor:
-
-                # retrieve the values of the primary key columns (leave blob column out)
-                pk_vals: tuple = tuple([row[inx] for inx in range(blob_index)])
-
-                # access the blob in chunks and write it to file
-                size: int = 0
-                blob: Any = row[blob_index]
-                with lob_file.open(mode="wb") as file:
-                    blob_data: bytes = blob.read(chunk_size)
-                    while blob_data:
-                        size += len(blob_data)
-                        file.write(blob_data)
-                        blob_data = blob.read(chunk_size)
-
-                # send blob to the destination database
-                op_errors: list[str] = []
-                if size > 0:
-                    db_update_lob_to(errors=op_errors,
-                                     lob_table=target_table,
-                                     lob_column=target_column,
-                                     lob_file=lob_file,
-                                     chunk_size=chunk_size,
-                                     pk_columns=pk_columns,
-                                     pk_vals=pk_vals,
-                                     engine=target_engine,
-                                     conn=target_conn,
-                                     logger=logger)
-                # errors ?
-                if op_errors:
-                    # yes, register them
-                    errors.extend(op_errors)
-                else:
-                    # no, increment the LOB migration counter
-                    result += 1
-
-        # commit the source and target transactions
-        curr_conn.commit()
-        target_conn.commit()
-    except Exception as e:
-        if curr_conn:
-            curr_conn.rollback()
-        if target_conn:
-            target_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
-    finally:
-        # close the connection, if locally acquired
-        if curr_conn and not conn:
-            curr_conn.close()
-        if lob_file and lob_file.exists():
-            lob_file.unlink()
-
-    # log the results
-    _db_log(logger=logger,
-            engine="postgres",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=(f"{result} LOBs migrated, "
-                        f"from postgres at {lob_table}.{lob_column} "
-                        f"to {target_engine} at {target_table}.{target_column}"))
-
-    return result
-
-
 def db_update_lob(errors: list[str],
                   lob_table: str,
                   lob_column: str,
                   pk_columns: list[str],
                   pk_vals: tuple,
                   lob_file: str | Path,
                   chunk_size: int,
```

### Comparing `pypomes_db-0.6.9/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.7.0/src/pypomes_db/sqlserver_pomes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 # noinspection DuplicatedCode
 from logging import Logger
 from pyodbc import Binary, Connection, Row, connect
 from pathlib import Path
-from typing import Any
 
 from .db_common import (
-    _db_assert_query_quota, _db_assert_temp_file,
-    _db_get_params, _db_log, _db_except_msg
+    _db_assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
-from .db_pomes import db_bulk_insert as db_bulk_insert_to
-from .db_pomes import db_update_lob as db_update_lob_to
 
 
 def db_connect(errors: list[str],
                logger: Logger = None) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
@@ -181,247 +177,14 @@
             errors=errors,
             stmt=insert_stmt,
             bind_vals=insert_vals[0])
 
     return result
 
 
-def db_bulk_migrate(errors: list[str],
-                    sel_stmt: str,
-                    insert_stmt: str,
-                    target_engine: str,
-                    batch_size: int,
-                    where_vals: tuple,
-                    target_conn: Any,
-                    conn: Connection,
-                    logger: Logger) -> int:
-    """
-    Bulk migrate data from a SQLServer database to another database.
-
-    The destination database brand must be in the list of databases configured and supported by this package.
-
-    :param errors: incidental error messages
-    :param sel_stmt: SELECT command for the search
-    :param insert_stmt: the insert statement to use for bulk-inserting
-    :param target_engine: the destination database engine type
-    :param batch_size: number of tuples in the batch, or 0 or None for no limit
-    :param where_vals: the values to be associated with the search criteria
-    :param target_conn: the connection to the destination database
-    :param conn: optional connection to use (obtains a new one, if not specified)
-    :param logger: optional logger
-    :return: number of tuples effectively migrated
-    """
-    # initialize the return variable
-    result: int = 0
-
-    # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
-                                               logger=logger)
-
-    err_msg: str | None = None
-    try:
-        with curr_conn.cursor() as cursor:
-
-            # execute the query
-            cursor.execute(sel_stmt, where_vals)
-
-            # fetch rows in batches/all rows
-            op_errors: list[str] = []
-            rows: list[Row]
-            if batch_size:
-                rows = cursor.fetchmany(batch_size)
-            else:
-                rows = cursor.fetchall()
-            while rows:
-                tuples: list[tuple] = [tuple(row) for row in rows]
-                result += db_bulk_insert_to(errors=op_errors,
-                                            insert_stmt=insert_stmt,
-                                            insert_vals=tuples,
-                                            engine=target_engine,
-                                            conn=target_conn,
-                                            logger=logger) or 0
-                # errors ?
-                if op_errors:
-                    # yes, register them and abort the operation
-                    errors.extend(op_errors)
-                    break
-                if not batch_size:
-                    break
-                rows = cursor.fetchmany(batch_size)
-
-        # commit the source and target transactions
-        curr_conn.commit()
-        if target_conn:
-            target_conn.commit()
-    except Exception as e:
-        if curr_conn:
-            curr_conn.rollback()
-        if target_conn:
-            target_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
-    finally:
-        # close the connection, if locally acquired
-        if curr_conn and not conn:
-            curr_conn.close()
-
-    # log the results
-    _db_log(logger=logger,
-            engine="sqlserver",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=sel_stmt,
-            bind_vals=where_vals)
-    _db_log(logger=logger,
-            engine="sqlserver",
-            stmt=(f"{result} tuples migrated, "
-                        f"from sqlserver to {target_engine}"))
-
-    return result
-
-
-def db_migrate_lobs(errors: list[str],
-                    lob_table: str,
-                    lob_column: str,
-                    pk_columns: list[str],
-                    target_engine: str,
-                    where_clause: tuple,
-                    temp_file: str | Path,
-                    chunk_size: int,
-                    target_table: str,
-                    target_column: str,
-                    target_conn: Any,
-                    conn: Connection,
-                    logger: Logger) -> int:
-    """
-    Migrate large binary objects (LOBs) from a SQLServer database to another database.
-
-    The destination database must be in the list of databases configured and supported by this package.
-    One or more columns making up a primary key, or a unique row identifier, must exist on *lob_table*,
-    and be provided in *pk_columns*. It is assumed that the primary key columns have the same name,
-    and are of equivalent types, in both the origin and the destination database.
-    If *temp_file* is not provided, a plataform-specific temporary file is used.
-
-    :param errors: incidental error messages
-    :param lob_table: the table holding the LOBs
-    :param lob_column: the column holding the LOB
-    :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
-    :param target_engine: the destination database engine type
-    :param where_clause: the criteria for tuple selection
-    :param temp_file: temporary file to use (a file object or a valid file path)
-    :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
-    :param target_table: the table to write the lob to (defaults to the source table)
-    :param target_column: the column to write the lob to (defaults to the source column)
-    :param target_conn: the connection to the destination database
-    :param conn: optional connection to use (obtains a new one, if not specified)
-    :param logger: optional logger
-    :return: number of LOBs effectively migrated
-    """
-    # initialize the return variable
-    result: int = 0
-
-    # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
-                                               logger=logger)
-
-    # make sure to have a target table
-    if not target_table:
-        target_table = lob_table
-
-    # make sure to have a target column
-    if not target_column:
-        target_column = lob_column
-
-    # make sure to have a temporary file
-    lob_file: Path = _db_assert_temp_file(temp_file)
-
-    # normalize the chunk size
-    if not chunk_size:
-        chunk_size = -1
-
-    # buid the query
-    pks: str = ", ".join(pk_columns)
-    sel_stmt: str = f"SELECT {pks}, {lob_column} FROM {lob_table}"
-    if where_clause:
-        sel_stmt += f" WHERE {where_clause}"
-    blob_index: int = len(pk_columns)
-
-    err_msg: str | None = None
-    try:
-        with curr_conn.cursor() as cursor:
-
-            # execute the query
-            cursor.execute(sel_stmt)
-
-            # fetch rows
-            for row in cursor:
-
-                # retrieve the values of the primary key columns (leave blob column out)
-                pk_vals: tuple = tuple([row[inx] for inx in range(blob_index)])
-
-                # access the blob in chunks and write it to file
-                size: int = 0
-                blob: Any = row[blob_index]
-                with lob_file.open(mode="wb") as file:
-                    blob_data: bytes = blob.read(chunk_size)
-                    while blob_data:
-                        size += len(blob_data)
-                        file.write(blob_data)
-                        blob_data = blob.read(chunk_size)
-
-                # send blob to the destination database
-                op_errors: list[str] = []
-                if size > 0:
-                    db_update_lob_to(errors=op_errors,
-                                     lob_table=target_table,
-                                     lob_column=target_column,
-                                     lob_file=lob_file,
-                                     chunk_size=chunk_size,
-                                     pk_columns=pk_columns,
-                                     pk_vals=pk_vals,
-                                     engine=target_engine,
-                                     conn=target_conn,
-                                     logger=logger)
-                # errors ?
-                if op_errors:
-                    # yes, register them
-                    errors.extend(op_errors)
-                else:
-                    # no, increment the LOB migration counter
-                    result += 1
-
-        # commit the source and target transactions
-        curr_conn.commit()
-        target_conn.commit()
-    except Exception as e:
-        if curr_conn:
-            curr_conn.rollback()
-        if target_conn:
-            target_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
-    finally:
-        # close the connection, if locally acquired
-        if curr_conn and not conn:
-            curr_conn.close()
-        if lob_file and lob_file.exists():
-            lob_file.unlink()
-
-    # log the results
-    _db_log(logger=logger,
-            engine="sqlserver",
-            err_msg=err_msg,
-            errors=errors,
-            stmt=(f"{result} LOBs migrated, "
-                        f"from sqlserver at {lob_table}.{lob_column} "
-                        f"to {target_engine} at {target_table}.{target_column}"))
-
-    return result
-
-
 def db_update_lob(errors: list[str],
                   lob_table: str,
                   lob_column: str,
                   pk_columns: list[str],
                   pk_vals: tuple,
                   lob_file: str | Path,
                   chunk_size: int,
```

### Comparing `pypomes_db-0.6.9/LICENSE` & `pypomes_db-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.6.9/pyproject.toml` & `pypomes_db-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.6.9"
+version = "0.7.0"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.6.9/PKG-INFO` & `pypomes_db-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.6.9
+Version: 0.7.0
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

