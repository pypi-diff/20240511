# Comparing `tmp/pgwarehouse-0.1.3.tar.gz` & `tmp/pgwarehouse-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgwarehouse-0.1.3.tar", max compression
+gzip compressed data, was "pgwarehouse-0.1.4.tar", max compression
```

## Comparing `pgwarehouse-0.1.3.tar` & `pgwarehouse-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1059 2023-03-13 00:25:10.022556 pgwarehouse-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     9466 2023-03-21 00:20:54.251089 pgwarehouse-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-03-04 05:37:05.189039 pgwarehouse-0.1.3/pgwarehouse/__init__.py
--rw-r--r--   0        0        0     1367 2023-03-21 00:20:54.251308 pgwarehouse-0.1.3/pgwarehouse/__main__.py
--rw-r--r--   0        0        0     1314 2023-03-11 01:06:58.627928 pgwarehouse-0.1.3/pgwarehouse/backend.py
--rw-r--r--   0        0        0    11778 2023-03-13 00:43:05.862352 pgwarehouse-0.1.3/pgwarehouse/clickhouse_backend.py
--rw-r--r--   0        0        0     7997 2023-03-21 00:20:54.251534 pgwarehouse-0.1.3/pgwarehouse/duckdb_backend.py
--rw-r--r--   0        0        0    13464 2023-03-21 00:20:54.251828 pgwarehouse-0.1.3/pgwarehouse/pgwarehouse.py
--rw-r--r--   0        0        0    11987 2023-03-13 00:09:31.202009 pgwarehouse-0.1.3/pgwarehouse/snowflake_backend.py
--rw-r--r--   0        0        0        0 2023-03-11 01:06:58.628793 pgwarehouse-0.1.3/pgwarehouse/tests/__init__.py
--rw-r--r--   0        0        0      192 2023-03-13 00:39:41.126083 pgwarehouse-0.1.3/pgwarehouse/tests/data/local_parks.csv
--rw-r--r--   0        0        0    37729 2023-03-11 01:06:58.629308 pgwarehouse-0.1.3/pgwarehouse/tests/data/my_orders.csv
--rw-r--r--   0        0        0    46636 2023-03-11 01:06:58.629660 pgwarehouse-0.1.3/pgwarehouse/tests/data/users10.csv
--rw-r--r--   0        0        0      658 2023-03-13 00:41:51.953146 pgwarehouse-0.1.3/pgwarehouse/tests/pg_setup.sql
--rw-r--r--   0        0        0     7135 2023-03-21 00:20:54.252053 pgwarehouse-0.1.3/pgwarehouse/tests/test_postgres.py
--rw-r--r--   0        0        0      616 2023-03-21 00:21:22.375245 pgwarehouse-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    10797 1970-01-01 00:00:00.000000 pgwarehouse-0.1.3/setup.py
--rw-r--r--   0        0        0    10324 1970-01-01 00:00:00.000000 pgwarehouse-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-03-13 00:25:10.022556 pgwarehouse-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     9771 2024-05-07 19:22:03.022666 pgwarehouse-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-03-04 05:37:05.189039 pgwarehouse-0.1.4/pgwarehouse/__init__.py
+-rw-r--r--   0        0        0     1367 2023-03-21 00:20:54.251308 pgwarehouse-0.1.4/pgwarehouse/__main__.py
+-rw-r--r--   0        0        0     1314 2023-03-11 01:06:58.627928 pgwarehouse-0.1.4/pgwarehouse/backend.py
+-rw-r--r--   0        0        0    12023 2024-05-07 19:17:52.299536 pgwarehouse-0.1.4/pgwarehouse/clickhouse_backend.py
+-rw-r--r--   0        0        0     7997 2023-03-21 00:20:54.251534 pgwarehouse-0.1.4/pgwarehouse/duckdb_backend.py
+-rw-r--r--   0        0        0    14168 2024-05-11 15:18:01.650463 pgwarehouse-0.1.4/pgwarehouse/pgwarehouse.py
+-rw-r--r--   0        0        0    12318 2024-05-11 15:16:04.352534 pgwarehouse-0.1.4/pgwarehouse/snowflake_backend.py
+-rw-r--r--   0        0        0        0 2023-03-11 01:06:58.628793 pgwarehouse-0.1.4/pgwarehouse/tests/__init__.py
+-rw-r--r--   0        0        0      192 2023-03-13 00:39:41.126083 pgwarehouse-0.1.4/pgwarehouse/tests/data/local_parks.csv
+-rw-r--r--   0        0        0    37729 2023-03-11 01:06:58.629308 pgwarehouse-0.1.4/pgwarehouse/tests/data/my_orders.csv
+-rw-r--r--   0        0        0    46636 2023-03-11 01:06:58.629660 pgwarehouse-0.1.4/pgwarehouse/tests/data/users10.csv
+-rw-r--r--   0        0        0      658 2023-03-13 00:41:51.953146 pgwarehouse-0.1.4/pgwarehouse/tests/pg_setup.sql
+-rw-r--r--   0        0        0     7190 2024-05-07 19:17:52.301720 pgwarehouse-0.1.4/pgwarehouse/tests/test_postgres.py
+-rw-r--r--   0        0        0      651 2024-05-11 15:20:06.735383 pgwarehouse-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    11177 1970-01-01 00:00:00.000000 pgwarehouse-0.1.4/setup.py
+-rw-r--r--   0        0        0    10629 1970-01-01 00:00:00.000000 pgwarehouse-0.1.4/PKG-INFO
```

### Comparing `pgwarehouse-0.1.3/LICENSE.txt` & `pgwarehouse-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pgwarehouse-0.1.3/README.md` & `pgwarehouse-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,22 +45,24 @@
 
 Again you can use the environment or the config file. Set these sets of vars in your env:
 
     CLICKHOUSE_HOST
     CLICKHOUSE_DATABASE
     CLICKHOUSE_USER
     CLICKHOUSE_PWD
+    CLICKHOUSE_SECURE
 
 or
 
     SNOWSQL_ACCOUNT
     SNOWSQL_DATABASE
     SNOWSQL_SCHEMA
     SNOWSQL_WAREHOUSE
     SNOWSQL_USER
+    SNOWSQL_ROLE
     SNOWSQL_PWD
 
 or
 
     DUCKDB_PATH (path to the duckdb database file)
 
 (The Snowflake parameters are the same as those for the [SnowSQL](https://docs.snowflake.com/en/user-guide/snowsql-start)
@@ -70,26 +72,32 @@
 
     warehouse:
         backend: (clickhouse|snowflake)
         clickhouse_host: 
         clickhouse_database: 
         clickhouse_user:
         clickhouse_password:
+        clickhouse_secure:
         --or--
         snowsql_account:
         snowsql_database:
         snowsql_schema:
         snowsql_warehouse:
         snowsql_user:
         snowsql_pwd:
         --or--
         duckdb_path:
 
 # Usage
 
+General way for run:
+```
+source .env.local; pgwarehouse --config .local.yaml sync users
+```
+
 Once the credentials are configured you can start syncing data. Start by listing tables from the Postgres database:
 
     pgwarehouse list
 
 And you can see which tables exist so far in the warehouse:
 
     pgwarehouse listwh
@@ -217,14 +225,24 @@
     pgwarehouse load <table>        - loads the data into the warehouse
 
 When the `extract` process runs, its stores data in `./pgw_data/<table name>_data`. As
 files are uploaded they are moved into an `archive` subdirectory. When the **next sync**
 runs then this archive directory will be cleaned up. This allows you to go examine
 the CSV downloaded data in case the upload fails for some reason. 
 
+## Development
+
+Requirements:
+```bash
+sudo apt install libpq-dev postgresql postgresql-contrib
+```
+
+Run tests:
+```poetry run python -m pytest```
+
 ## Limitations
 
 Column type mapping today is [very limited](https://github.com/scottpersinger/pgwarehouse/blob/a20dc316bbdbc78317cfdd796216a847919d8755/pgwarehouse/snowflake_backend.py). More esoteric column types like JSON or ARRAY are simply
 mapped as VARCHAR columns. Some of these types are supported in the warehouse and could be
 implemented more accurately.
 
 Composite primary keys (using multiple columns) have limited support. Today they will only work
```

### Comparing `pgwarehouse-0.1.3/pgwarehouse/__main__.py` & `pgwarehouse-0.1.4/pgwarehouse/__main__.py`

 * *Files identical despite different names*

### Comparing `pgwarehouse-0.1.3/pgwarehouse/backend.py` & `pgwarehouse-0.1.4/pgwarehouse/backend.py`

 * *Files identical despite different names*

### Comparing `pgwarehouse-0.1.3/pgwarehouse/clickhouse_backend.py` & `pgwarehouse-0.1.4/pgwarehouse/clickhouse_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,24 @@
     def setup_clickhouse_env(self):
         for key in ['clickhouse_host', 'clickhouse_user', 'clickhouse_password']:
             val = self.config.get(key, os.environ.get(key.upper()))
             if val is None:
                 raise RuntimeError(f"Missing {key} in config file or environment ({key.upper()})")
             setattr(self, key, val)
         self.clickhouse_database = self.config.get('clickhouse_database', os.environ.get('CLICKHOUSE_DATABASE', 'default'))
+        self.clickhouse_secure = bool(self.config.get('clickhouse_secure', int(os.environ.get('CLICKHOUSE_SECURE', 0))))
+
         if shutil.which("clickhouse-client") is None:
             raise RuntimeError("clickhouse-client not found in PATH")
         self.client: ClickhouseClient = ClickhouseClient(
             host=self.clickhouse_host,
             user=self.clickhouse_user,
             password=self.clickhouse_password,
-            database=self.clickhouse_database
+            database=self.clickhouse_database,
+            secure=self.clickhouse_secure
         )
 
     def list_tables(self):
         print(self.clickclient("SHOW TABLES;", echo=True))
 
     def convert_pg_root_type_clickhouse(self, pgtype: str, for_parse=False):
         if pgtype.endswith("_enum"):
@@ -83,26 +86,27 @@
             return self.convert_pg_root_type_clickhouse(pgtype, for_parse=for_parse)
 
     def clickclient(self, sql, input_file = None, echo=False):
         host = self.clickhouse_host
         user = self.clickhouse_user
         password = self.clickhouse_password
         database = self.clickhouse_database
+        secure = '--secure' if self.clickhouse_secure else ''
         if echo:
             echo = "--echo"
         else:
             echo = ""
 
         if input_file:
-            cat = "gzcat" if input_file.endswith(".gz") else "cat"
+            cat = "zcat" if input_file.endswith(".gz") else "cat"
             logger.debug(f"{cat} {input_file} | clickhouse-client --query {sql}")
-            ret = subprocess.run(f'{cat} {input_file} | clickhouse-client -h {host} -d {database} -u {user} --password "{password}" --query "{sql}"', 
+            ret = subprocess.run(f'{cat} {input_file} | clickhouse-client -h {host} {secure} -d {database} -u {user} --password "{password}" --query "{sql}"', 
                                     shell=True, capture_output=True)            
         else:
-            cmd = f'clickhouse-client {echo} -h {host} -d {database} -u {user} --password "{password}" --query "{sql}"'
+            cmd = f'clickhouse-client {echo} -h {host} {secure} -d {database} -u {user} --password "{password}" --query "{sql}"'
             logger.debug(f"clickhouse-client --query {sql}")
             ret = subprocess.run(cmd, 
                                 shell=True, capture_output=True)
         if ret.returncode != 0:
             logger.error(f"Command failed {ret}: {sql}")
             raise RuntimeError(f"Command failed {ret}: {sql}")
         return ret.stdout.decode('utf-8').strip()
@@ -238,22 +242,22 @@
         else:
             self.load_table(table, schema_file, create_table=False)
 
     def merge_table(self, table:str, schema_file:str):
         # New+updated records have been downloaded to CSV already.
         # Clickhouse doesn't support Upsert, so instead we load the new 
         # records into a temp table, then we join the target table to the temp table
-        # and delete existing records. Finally we Insert all the new records into the
+        # and delete existing records. Finally, we Insert all the new records into the
         # target table and remove the temp table.
 
         opts = self.parent.parse_schema_file(table, schema_file)
         if not opts['primary_key_cols']:
             raise RuntimeError("No primary key for the table found, have to reload")
 
-        temp_table = table + "__changes"
+        temp_table = f"{table}__changes"
         csv_dir = self.parent.csv_dir(table)
 
         self.load_table(temp_table, schema_file, create_table=True, drop_table=True, csv_dir=csv_dir)
         primary_key = opts['primary_key_cols'][0]
 
         logger.debug(f"Deleting dupe records between {temp_table} and {table}")
         self.clickclient(f"""
```

### Comparing `pgwarehouse-0.1.3/pgwarehouse/duckdb_backend.py` & `pgwarehouse-0.1.4/pgwarehouse/duckdb_backend.py`

 * *Files identical despite different names*

### Comparing `pgwarehouse-0.1.3/pgwarehouse/pgwarehouse.py` & `pgwarehouse-0.1.4/pgwarehouse/pgwarehouse.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,31 +70,41 @@
             raise RuntimeError(f"Unknown backend: {self.backend_type}")
 
         def get_table_opts(tablename, last_modified=None):
             for t in self.config.get('tables', []):
                 if t == tablename:
                     return {}
                 elif isinstance(t, dict) and tablename in t:
-                    return t[tablename]
+                    # remove tablename from the dict, leaving only the options
+                    t.pop(tablename)
+                    return t
             return {'last_modified':last_modified} if last_modified else {}
 
         def get_all_tables():
             if 'tables' in self.config:
-                return self.config['tables']
+                tables = self.config['tables']
+                tables_returned = []
+                for table in tables:
+                    # deal with the case where the tables contain options (thus a dict)
+                    if isinstance(table, dict):
+                        tables_returned.append(list(table.keys())[0])
+                    else:
+                        tables_returned.append(table)
+                return tables_returned
             else:
                 return self.all_table_names()
             
         tables:list = []
         if table == 'all':
             print(f"============== {command} ALL TABLES =========== ")
             for table in get_all_tables():
                 table_opts = get_table_opts(table)
                 self.table = table
-                self.schema_file = os.path.join(self.data_dir, table + ".schema")
-                logger.info(f">>>>>>>>> {command} {table}")
+                self.schema_file = os.path.join(self.data_dir, self.table + ".schema")
+                logger.info(f">>>>>>>>> {command} {self.table} {table_opts}")
                 try:
                     getattr(self, command)(self.table, table_opts)
                 except RuntimeError:
                     print(f"ERROR: {command} {table}")
                     traceback.print_exc()
                 logger.info("<<<<<<<<<\n")
             print("============== DONE =========== ")
@@ -119,31 +129,31 @@
 
     def init(self, config_file: str):
         if os.path.exists(config_file):
             print("Config file already exists")
         else:
             print("This will create a pgwarehouse config file in the current directory.")
             backend = None
-            while backend not in ["1", "2"]:
-                backend = input("Choose your warehouse type (Snowflake - 1, Clickhouse - 2): ")
-            backend = ["snowflake", "clickhouse"][int(backend)-1]
+            while backend not in ["1", "2", "3"]:
+                backend = input("Choose your warehouse type (Snowflake - 1, Clickhouse - 2, Duckdb - 3): ")
+            backend = ["snowflake", "clickhouse", "duckdb"][int(backend)-1]
             conf = {
                 "postgres": {
                     'pghost':"",
                     'pgdatabase':"",
                     'pguser':"",
                     'pgpassword':"",
                     'pgschema': 'public'
                 },
                 "warehouse": {
                     "backend": backend
                 }
             }
             if backend == "snowflake":
-                for key in ['snowsql_account',  'snowsql_warehouse', 'snowsql_database', 'snowsql_user', 'snowsql_password']:
+                for key in ['snowsql_account',  'snowsql_warehouse', 'snowsql_database', 'snowsql_user', 'snowsql_pwd']:
                     conf['warehouse'][key] = ""
             elif backend == "clickhouse":
                 for key in ['clickhouse_host', 'clickhouse_database', 'clickhouse_user', 'clickhouse_password']:
                     conf['warehouse'][key] = ""
             with open(config_file, "w") as f:
                 f.write(yaml.dump(conf))
                 f.write("# Add a 'tables' list to specify tables to sync\n")
@@ -193,34 +203,35 @@
             val = conf.get(key, os.environ.get(key.upper()))
             if val is None:
                 raise RuntimeError(f"Missing {key} in config file or environment ({key.upper()})")
             setattr(self, key, val)
             os.environ[key.upper()] = val
         self.pgschema = conf.get('pgschema', os.environ.get('PGSCHEMA', 'public'))
         self.pgport = int(conf.get('pgport', os.environ.get('PGPORT', '5432')))
+        self.pgsslmode = conf.get('pgsslmode', os.environ.get('PGSSLMODE', 'prefer'))
         self.max_pg_records = conf.get('max_records', None)
         self.client = psycopg2.connect(
-            f"host={self.pghost} dbname={self.pgdatabase} user={self.pguser} password={self.pgpassword} port={self.pgport}",
+            f"host={self.pghost} dbname={self.pgdatabase} user={self.pguser} password={self.pgpassword} port={self.pgport} sslmode={self.pgsslmode}",
             connect_timeout=10
         )
         self.cursor: psycopg2.extensions.cursor = self.client.cursor()
 
     def list(self) -> None:
-        sql = """
+        sql = f"""
             SELECT table_schema, table_name, pg_size_pretty(total_bytes) AS total, to_char(row_estimate, 'FM999,999,999,999') as rows
             FROM (
             SELECT *, total_bytes-index_bytes-coalesce(toast_bytes,0) AS table_bytes FROM (
                 SELECT c.oid,nspname AS table_schema, relname AS table_name
                         , c.reltuples AS row_estimate
                         , pg_total_relation_size(c.oid) AS total_bytes
                         , pg_indexes_size(c.oid) AS index_bytes
                         , pg_total_relation_size(reltoastrelid) AS toast_bytes
                     FROM pg_class c
                     LEFT JOIN pg_namespace n ON n.oid = c.relnamespace
-                    WHERE relkind = 'r' and nspname='public'
+                    WHERE relkind = 'r' and nspname='{self.pgschema}'
             ) a order by table_bytes desc
             ) a;
         """
         sql = sql.strip().replace("\n", " ")
         self.cursor.execute(sql)
         rows = self.cursor.fetchall()
         print(tabulate(rows, headers=['schema', 'table', 'size', 'rows']))
@@ -231,15 +242,15 @@
     def all_table_names(self):
         self.cursor.execute(
             f"select table_name from information_schema.tables where table_schema='{self.pgschema}'"
         )
         return sorted([r[0] for r in self.cursor.fetchall()])
 
     def dump_schema(self, table: str, schema_file: str):
-        ret = os.system(f"psql --pset=format=unaligned -c \"\\d {table}\" > {schema_file}")
+        ret = os.system(f"psql --pset=format=unaligned -c \"\\d {self.pgschema}.{table}\" > {schema_file}")
         if ret != 0:
             raise RuntimeError("Error saving schema")
         logger.debug(f"Saved schema to {schema_file}")
 
     def extract(self, table: str, table_opts: dict, filter=""):
         # Returns a tuple of [file count, line count] of downloaded records
         self.dump_schema(table, self.schema_file)
@@ -257,15 +268,15 @@
 
         def next_file():
             fname = os.path.join(out_dir, f"{table}{file_suffix}0.csv.gz")
             logger.info(f"Writing to {fname} total records written: {total_records:,} total bytes: {current_size:,}")
             return gzip.open(fname, "wt")
 
         outfile = next_file()
-        cmd = f'psql -c "\\copy (select * from {table} {filter}) to STDOUT CSV HEADER\"'
+        cmd = f'psql -c "\\copy (select * from {self.pgschema}.{table} {filter}) to STDOUT CSV HEADER\"'
         args = shlex.split(cmd)
         proc = subprocess.Popen(args, stdout=subprocess.PIPE)
         for line in iter(proc.stdout.readline, b''):
             strline = line.decode('utf-8')
             if header is None:
                 header = strline
             else:
```

### Comparing `pgwarehouse-0.1.3/pgwarehouse/snowflake_backend.py` & `pgwarehouse-0.1.4/pgwarehouse/snowflake_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,41 +14,47 @@
     val = subprocess.run(cmd, shell=True, capture_output=True, check=True)
     return val.stdout.decode('utf-8').strip()
 
 class SnowflakeBackend(Backend):
     ###############
     # Snowflake
     ###############
-    RESERVED_COL_NAMES = ['current_date','order','to','from']
+    RESERVED_COL_NAMES = ['current_date','order','to','from','values','start','current']
 
     def __init__(self, config: dict, parent: PGBackend) -> None:
         self.snowsql_account: str
         self.snowsql_database: str
         self.snowsql_schema: str
         self.snowsql_warehouse: str
         self.snowsql_user: str
         self.snowsql_pwd: str
+        self.snowsql_role: str = None
         self.config = config
         self.parent: PGBackend = parent
         self.setup_env()
         
     def setup_env(self):
         for key in ['snowsql_account', 'snowsql_database', 'snowsql_schema','snowsql_warehouse','snowsql_user','snowsql_pwd']:
             val = self.config.get(key, os.environ.get(key.upper()))
             if val is None:
                 raise RuntimeError(f"Missing {key} in config file or environment ({key.upper()})")
             setattr(self, key, val)
 
         # Gets the version
-        ctx = snowflake.connector.connect(
-            user=self.snowsql_user,
-            password=self.snowsql_pwd,
-            account=self.snowsql_account,
-            database=self.snowsql_database
-            )
+        connection_config = {
+            'user': self.snowsql_user,
+            'password': self.snowsql_pwd,
+            'account': self.snowsql_account,
+            'database': self.snowsql_database,
+            'schema': self.snowsql_schema
+        }
+        if self.snowsql_role:
+            connection_config.update({'role': self.snowsql_role})
+
+        ctx = snowflake.connector.connect(**connection_config)
         self.snow_cursor = ctx.cursor()
         self.snow_cursor.execute("use warehouse " + self.snowsql_warehouse + "; ")
 
         sflogger = logging.getLogger('snowflake.connector')
         sflogger.setLevel(logging.WARNING)
         sflogger.addHandler(self.parent.get_log_handler())
 
@@ -105,15 +111,15 @@
     def quote_col(self, colname: str):
         if colname.lower() in SnowflakeBackend.RESERVED_COL_NAMES:
             return f'"{colname}"'
         else:
             return colname
 
     def list_tables(self):
-        for row in self.snow_cursor.execute("SHOW TABLES;"):
+        for row in self.snow_cursor.execute(f"SHOW TABLES IN SCHEMA {self.snowsql_schema};"):
             print(row)                              
 
     def load_table(self, table, schema_file, create_table=True, drop_table=False):
         csv_dir = self.parent.csv_dir(table)
         if not os.path.exists(csv_dir):
             raise RuntimeError("Cannot find data dir: ", csv_dir)
 
@@ -127,31 +133,30 @@
             self.snow_cursor.execute(f"USE DATABASE {self.snowsql_database}")
             self.snow_cursor.execute(f"CREATE TABLE IF NOT EXISTS {self.snowsql_schema}.{table} ({import_structure});")
 
         archive_dir = csv_dir + "/archive"
         if not os.path.exists(archive_dir):
             os.makedirs(archive_dir)
 
-        logger.info(f"Sending to {table} data to Snowflake...")
+        logger.info(f"Sending {table} data to Snowflake...")
 
         for idx, nextfile in self.parent.iterate_csv_files(csv_dir):
             logger.debug(f"Loading file: {nextfile}")
             skip = 1
             if not nextfile.endswith(".gz"):
                 print(return_output(f"gzip -9 {nextfile}"))
                 nextfile += ".gz"
             csv = os.path.basename(nextfile)
             self.snow_cursor.execute(f"USE SCHEMA {self.snowsql_schema}")
             logger.debug("PUTing file")
             self.snow_cursor.execute(f"PUT file://{nextfile} @{self.snowsql_database}.{self.snowsql_schema}.%{table};")
-            logger.info(f"COPY INTO INTO {self.snowsql_database}.{self.snowsql_schema}.{table} FROM @%{table} PATTERN = '{csv}'")
+            logger.info(f"COPY INTO {self.snowsql_database}.{self.snowsql_schema}.{table} FROM @{self.snowsql_database}.{self.snowsql_schema}.%{table}/{csv}")
             for row in self.snow_cursor.execute(f""" 
-                COPY INTO {self.snowsql_database}.{self.snowsql_schema}.{table} FROM @%{table}
+                COPY INTO {self.snowsql_database}.{self.snowsql_schema}.{table} FROM @{self.snowsql_database}.{self.snowsql_schema}.%{table}/{csv}
                     FILE_FORMAT = (type = csv field_optionally_enclosed_by='\\"' SKIP_HEADER={skip}) ON_ERROR=CONTINUE FORCE=TRUE 
-                    PATTERN = '{csv}'
                 PURGE = TRUE
             """):
                 logger.info(row)
             shutil.move(nextfile, archive_dir)
 
     def merge_table(self, table:str, schema_file:str, allow_create=False):
         if not self.table_exists(table):
@@ -186,15 +191,15 @@
             logger.debug("LOADing file into database")
             update_sets = ", ".join([f'{table}.{self.quote_col(col)} = csvsrc.{self.quote_col(col)}' for col in columns])
             values_list = ", ".join([f'csvsrc.{self.quote_col(col)}' for col in columns])
             self.snow_cursor.execute(f"""
                 CREATE OR REPLACE FILE FORMAT pgw_csv_format TYPE = 'csv' SKIP_HEADER = 1 
                 FIELD_OPTIONALLY_ENCLOSED_BY = '0x22' ESCAPE_UNENCLOSED_FIELD = NONE
             """)
-            logger.info(f"MERGE INTO INTO {self.snowsql_database}.{self.snowsql_schema}.{table} PATTERN = '{csv}'")
+            logger.info(f"MERGE INTO {self.snowsql_database}.{self.snowsql_schema}.{table} PATTERN = '{csv}'")
             self.snow_cursor.execute(f""" 
                 MERGE INTO {self.snowsql_database}.{self.snowsql_schema}.{table} USING 
                     (SELECT 
                     {column_list} 
                     FROM @%{table}(FILE_FORMAT => 'pgw_csv_format', PATTERN => '{csv}')
                     ) csvsrc
                     ON csvsrc.{key_col} = {table}.{key_col}
```

### Comparing `pgwarehouse-0.1.3/pgwarehouse/tests/data/my_orders.csv` & `pgwarehouse-0.1.4/pgwarehouse/tests/data/my_orders.csv`

 * *Files identical despite different names*

### Comparing `pgwarehouse-0.1.3/pgwarehouse/tests/data/users10.csv` & `pgwarehouse-0.1.4/pgwarehouse/tests/data/users10.csv`

 * *Files identical despite different names*

### Comparing `pgwarehouse-0.1.3/pgwarehouse/tests/pg_setup.sql` & `pgwarehouse-0.1.4/pgwarehouse/tests/pg_setup.sql`

 * *Files identical despite different names*

### Comparing `pgwarehouse-0.1.3/pgwarehouse/tests/test_postgres.py` & `pgwarehouse-0.1.4/pgwarehouse/tests/test_postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 #BACKEND = 'clickhouse'
 BACKEND = 'duckdb'
 
 def dbsetup(postgresql):
     conn = psycopg2.connect(**postgresql.dsn())
     with conn.cursor() as cursor:
+        cursor.execute("SET datestyle = 'MDY';")
         with open(os.path.join(os.path.dirname(__file__), 'pg_setup.sql')) as f:
             cursor.execute(f.read())
 
         for path in glob.glob(os.path.join(os.path.dirname(__file__), 'data', '*.csv')):
             table = os.path.basename(path).split('.')[0]
             print(f"Loading CSV into table {table}")
             with open(path) as f:
@@ -59,21 +60,21 @@
 
     return client
     #Postgresql.clear_cache()
 
 @pytest.fixture
 def out_dir():
     dir = os.path.join(os.path.dirname(__file__), 'output')
-    shutil.rmtree(dir)
     os.makedirs(dir, exist_ok=True)
+    shutil.rmtree(dir)
     return dir
 
 @pytest.fixture
 def ch_env():
-    assert 'CLICKHOUSE_HOST' in os.environ
+    # assert 'CLICKHOUSE_HOST' in os.environ
     return None
 
 def drop_table(connection, table):
     with connection.cursor() as cursor:
         cursor.execute(f"DROP TABLE IF EXISTS {table}")
 
 def table_size(connection, table) -> int:
@@ -90,20 +91,20 @@
     pgw = PGWarehouse(command='listwh', table=None,
             data_dir=out_dir, backend_type=BACKEND, debug=True)
     
 def test_extract(connection, out_dir, ch_env):
     for table in ['local_parks','my_orders']:
         pgw = PGWarehouse(command='extract', table=table,
                     data_dir=out_dir, backend_type=BACKEND, debug=True)
-        assert os.path.exists(os.path.join(out_dir, table + "_data"))
-        assert len(glob.glob(os.path.join(out_dir, table+"_data", "*"))) > 0
+        assert os.path.exists(os.path.join(out_dir, f"{table}_data"))
+        assert len(glob.glob(os.path.join(out_dir, f"{table}_data", "*"))) > 0
 
 def test_extract_load(connection, out_dir, ch_env):
     for table in ['local_parks','users10','my_orders']:
-        path = os.path.join(os.path.dirname(__file__), 'data', table+".csv")
+        path = os.path.join(os.path.dirname(__file__), 'data', f"{table}.csv")
         pgw = PGWarehouse(command='extract', table=table,
                     data_dir=out_dir, backend_type=BACKEND, debug=True)
         pgw.backend._drop_table(table)
         pgw = PGWarehouse(command='load', table=table,
                     data_dir=out_dir, backend_type=BACKEND, debug=True)
         assert pgw.count_warehouse_table(table) == table_size(connection, table)
```

### Comparing `pgwarehouse-0.1.3/pyproject.toml` & `pgwarehouse-0.1.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pgwarehouse"
-version = "0.1.3"
+version = "0.1.4"
 description = "Easily sync your Postgres database to your data warehouse."
 authors = ["Scott Persinger <scottpersinger@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyyaml = "^6.0"
@@ -21,7 +21,8 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry.scripts]
 pgwarehouse = 'pgwarehouse.__main__:main'
+pgwh = 'pgwarehouse.__main__:main'
```

### Comparing `pgwarehouse-0.1.3/setup.py` & `pgwarehouse-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,22 @@
  'python-dotenv>=1.0.0,<2.0.0',
  'pyyaml>=6.0,<7.0',
  'snowflake-connector-python>=3.0.1,<4.0.0',
  'tabulate>=0.9.0,<0.10.0',
  'testing-postgresql>=1.3.0,<2.0.0']
 
 entry_points = \
-{'console_scripts': ['pgwarehouse = pgwarehouse.__main__:main']}
+{'console_scripts': ['pgwarehouse = pgwarehouse.__main__:main',
+                     'pgwh = pgwarehouse.__main__:main']}
 
 setup_kwargs = {
     'name': 'pgwarehouse',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Easily sync your Postgres database to your data warehouse.',
-    'long_description': '# pgwarehouse - quickly sync Postgres data to your cloud warehouse\n\n## Introduction\n\nPostgres is an amazing, general purpose OLTP database. But it\'s not designed for heavy analytic (OLAP) usage. Analytic queries are much better served by a columnar store database like Snowflake or Clickhouse.\n\nThis package allows you to easily sync data from a Postgres database into a local or cloud data warehouse (currently [Snowflake](https://docs.snowflake.com/), [ClickHouse](https://clickhouse-docs.vercel.app/docs/en/intro), or [DuckDB](https://duckdb.org/docs/)). You can perform a one-time sync operation, or run periodic incremental syncs to keep your warehouse up to date.\n\n## Features\n\n* High performance by using `COPY` to move lots of data efficiently. `pgwarehouse` can easily sync hundreds of millions of rows of data (tens of GB) per hour.\n* Supports multiple update strategies for immutable or mutable tables.\n* Easy to configure and run.\n\n## Installation\n\n    pip install pgwarehouse\n\nNow you need to configure credentials for your **Postgres** source and the warehouse destination.\n\nYou can place Postgres credentials either in your config file or in your environment. If using the environment you need to set these variables:\n\n    PGHOST\n    PGDATABASE\n    PGUSER\n    PGPASSWORD\n    PGSCHEMA (defaults to \'public\')\n\n## Creating a config file\n\nRun this command to create a template config file:\n\n    pgwarehouse init\n\nThis will create a local `pgwarehouse_conf.yaml` file. Now you can edit your Postgres credentials in the `postgres` stanza of the config file:\n\n    postgres:\n        pghost: (defaults to $PGHOST)\n        pgdatabase: (defaults to $PGDATABASE\n        pguser: (defaults to $PGUSER)\n        pgpassword: (defaults to $PGPASSWORD)\n        pgschema: (defaults to \'public\')\n\n## Specifying the warehouse credentials\n\nAgain you can use the environment or the config file. Set these sets of vars in your env:\n\n    CLICKHOUSE_HOST\n    CLICKHOUSE_DATABASE\n    CLICKHOUSE_USER\n    CLICKHOUSE_PWD\n\nor\n\n    SNOWSQL_ACCOUNT\n    SNOWSQL_DATABASE\n    SNOWSQL_SCHEMA\n    SNOWSQL_WAREHOUSE\n    SNOWSQL_USER\n    SNOWSQL_PWD\n\nor\n\n    DUCKDB_PATH (path to the duckdb database file)\n\n(The Snowflake parameters are the same as those for the [SnowSQL](https://docs.snowflake.com/en/user-guide/snowsql-start)\nCLI tool. The `SNOWSQL_ACCOUNT` value should be your "account identifier".)\n\nor set these values in the `warehouse` stanza in the config file:\n\n    warehouse:\n        backend: (clickhouse|snowflake)\n        clickhouse_host: \n        clickhouse_database: \n        clickhouse_user:\n        clickhouse_password:\n        --or--\n        snowsql_account:\n        snowsql_database:\n        snowsql_schema:\n        snowsql_warehouse:\n        snowsql_user:\n        snowsql_pwd:\n        --or--\n        duckdb_path:\n\n# Usage\n\nOnce the credentials are configured you can start syncing data. Start by listing tables from the Postgres database:\n\n    pgwarehouse list\n\nAnd you can see which tables exist so far in the warehouse:\n\n    pgwarehouse listwh\n    \nNow use `sync` to sync a table (eg. the \'users\' table):\n\n    pgwarehouse sync users\n\nData will be downloaded from the Postgres database into CSV files on the local machine, and then those files will be uploaded to the warehouse. Running `pgwarehouse listwh` will show the new table.\n\n## Updating a table\n\nAfter the initial sync has run, you can update the warehouse table with new records by running `sync` again:\n\n    pgwarehouse sync users\n\nSee [update strategies](#table-update-strategies) for different ways to update your table on each sync.\n\n## Syncing multiple tables\n\nThere are two ways to manage multiple tables. The first is just to pass `all` in place of the table name:\n\n    pgwarehouse sync all\n\nThis will attempt to sync ALL tables from Postgres into the warehouse. This could take a while!\n\nThe other way is to specify the `tables` list in the config file:\n\n    tables:\n        - users\n        - charges\n        - logs\n\nNow when you specify `sync all` the tool will use the list of tables specified in the config file.\n\n**Pro tip!** You can add the `max_records` settings to your `postgres` configuration to limit the number\nof records copied per table. This can be useful for testing the initial sync in case you have some\nlarge tables. Set this value to something reasonable (like 10000) and then try syncrhonizing all\ntables to make sure they copy properly. Once you have verified the tables in the warehouse then you\ncan remove this setting, drop any large tables, and then copy them in full (just run `sync all` again).\n\n## Table update strategies\n\n#### New Records Only (default)\nThe default update strategy is "new records only". This is done by selecting records with a greater value\nfor their primary id column than the greatest value currently in the warehouse. This strategy is simple\nand quick, but only works for monotonically incrementing primary keys, and only finds new records.\n\n#### Reload each time\nAnother supported strategy is "reload each time". This is the simplest strategy and we simply reload the\nentire table every time we sync. This strategy should be fine for small-ish tables (like <10m rows).\n\n#### Last Modified\nFinally, if your table has a `last modified` column then you can use the "all modifications strategy".\nIn this case all records with a `last modified` timestamp greater than the maximum value found in the\nwarehouse will be selected and "upserted" into the warehouse. Records that are already present\n(via matching the primary key) will be updated, and new records will be inserted.\n\n* The Snowflake backend uses the [MERGE](https://docs.snowflake.com/en/sql-reference/sql/merge) operation. \n* The Clickhouse backend uses `ALTER TABLE .. DELETE` to remove matching records and then `INSERT` to insert the new values.\n\n### What about deletes?\n\nThere is no simple way to capture deletes - you have to reload the entire table. A common pattern is\nto apply new records on a daily basis, and reload the entire table every week to remove deleted records.\n\n### What if my table has no primary key?\n\nAll the update strategies except "reload each time" require your table to have a primary key column.\n\n## Specifying update strategy at the command line\n\n    pgwarehouse sync <table>   (defaults to NEW RECORDS)\n    pgwarehouse sync <table> last_modified=<last modified column>   (MODIFIED RECORDS)\n    pgwarehouse reload <table> (reloads the whole table)\n\n## Specifying update strategy in the config file\n\nYou can configure the update strategy selectively for each table in the config file. To do so,\nspecify the table as a nested dictionary with options:\n\n    tables:\n        - accounts\n        - users:\n            reload: true\n        - orders:\n            last_modified: updated_at\n        - shoppers\n            last_modified: update_time\n            reload: sun\n        - original_orders:\n            skip: true\n\nIn this example:\n\n* `accounts` will have new records only applied at each sync\n* `users` will be reloaded completely on each sync\n* `orders` will have modified records (found by the \'updated_at\' column) applied on each sync\n* `shoppers` will have modified records applied on each sync, except for any sync\nwhich happens on Sunday, in which case the entire table will be reloaded.\n* `original_orders` will be skipped entirely\n\nThe `reload` argument can take 3 forms:\n\n    reload: true    - reload the table every sync\n    reload: [sun,mon,tue,wed,thur,fri]  - reload if the sync occurs on this day of the week\n    reload: 1-31    - reload if the sync occurs on this numeric day of the month (don\'t use 31!)\n\n## Scheduling regular data syncs\n\n`pgwarehouse` does not including any scheduling itself, you will need an external trigger like\n`cron`, [Heroku Scheduler](https://devcenter.heroku.com/articles/scheduler), or a K8s\n[CronJob](https://kubernetes.io/docs/tasks/job/automated-tasks-with-cron-jobs/).\n\nWhen running, the tool will need access to local storage - potentially a lot if you are synchronizing\nbig tables. But nothing needs to persist between sync runs (except the config file) - the tool \nonly relies on state it can query from Postgres or the warehouse.\n\n## Troubleshooting\n\nSometimes when you are testing things out it can be helpful to do the sync in two phases:\n1)download the data, 2)upload the data. You can use `extract` and `load` for this:\n\n    pgwarehouse extract <table>     - only downloads data\n    pgwarehouse load <table>        - loads the data into the warehouse\n\nWhen the `extract` process runs, its stores data in `./pgw_data/<table name>_data`. As\nfiles are uploaded they are moved into an `archive` subdirectory. When the **next sync**\nruns then this archive directory will be cleaned up. This allows you to go examine\nthe CSV downloaded data in case the upload fails for some reason. \n\n## Limitations\n\nColumn type mapping today is [very limited](https://github.com/scottpersinger/pgwarehouse/blob/a20dc316bbdbc78317cfdd796216a847919d8755/pgwarehouse/snowflake_backend.py). More esoteric column types like JSON or ARRAY are simply\nmapped as VARCHAR columns. Some of these types are supported in the warehouse and could be\nimplemented more accurately.\n\nComposite primary keys (using multiple columns) have limited support. Today they will only work\nwith the RELOAD strategy.\n\nNon-numeric primary key types (like UUIDs) probably won\'t work unless they have a good lexigraphic\nsort that supports a `>` where clause.\n\n\n\n',
+    'long_description': '# pgwarehouse - quickly sync Postgres data to your cloud warehouse\n\n## Introduction\n\nPostgres is an amazing, general purpose OLTP database. But it\'s not designed for heavy analytic (OLAP) usage. Analytic queries are much better served by a columnar store database like Snowflake or Clickhouse.\n\nThis package allows you to easily sync data from a Postgres database into a local or cloud data warehouse (currently [Snowflake](https://docs.snowflake.com/), [ClickHouse](https://clickhouse-docs.vercel.app/docs/en/intro), or [DuckDB](https://duckdb.org/docs/)). You can perform a one-time sync operation, or run periodic incremental syncs to keep your warehouse up to date.\n\n## Features\n\n* High performance by using `COPY` to move lots of data efficiently. `pgwarehouse` can easily sync hundreds of millions of rows of data (tens of GB) per hour.\n* Supports multiple update strategies for immutable or mutable tables.\n* Easy to configure and run.\n\n## Installation\n\n    pip install pgwarehouse\n\nNow you need to configure credentials for your **Postgres** source and the warehouse destination.\n\nYou can place Postgres credentials either in your config file or in your environment. If using the environment you need to set these variables:\n\n    PGHOST\n    PGDATABASE\n    PGUSER\n    PGPASSWORD\n    PGSCHEMA (defaults to \'public\')\n\n## Creating a config file\n\nRun this command to create a template config file:\n\n    pgwarehouse init\n\nThis will create a local `pgwarehouse_conf.yaml` file. Now you can edit your Postgres credentials in the `postgres` stanza of the config file:\n\n    postgres:\n        pghost: (defaults to $PGHOST)\n        pgdatabase: (defaults to $PGDATABASE\n        pguser: (defaults to $PGUSER)\n        pgpassword: (defaults to $PGPASSWORD)\n        pgschema: (defaults to \'public\')\n\n## Specifying the warehouse credentials\n\nAgain you can use the environment or the config file. Set these sets of vars in your env:\n\n    CLICKHOUSE_HOST\n    CLICKHOUSE_DATABASE\n    CLICKHOUSE_USER\n    CLICKHOUSE_PWD\n    CLICKHOUSE_SECURE\n\nor\n\n    SNOWSQL_ACCOUNT\n    SNOWSQL_DATABASE\n    SNOWSQL_SCHEMA\n    SNOWSQL_WAREHOUSE\n    SNOWSQL_USER\n    SNOWSQL_ROLE\n    SNOWSQL_PWD\n\nor\n\n    DUCKDB_PATH (path to the duckdb database file)\n\n(The Snowflake parameters are the same as those for the [SnowSQL](https://docs.snowflake.com/en/user-guide/snowsql-start)\nCLI tool. The `SNOWSQL_ACCOUNT` value should be your "account identifier".)\n\nor set these values in the `warehouse` stanza in the config file:\n\n    warehouse:\n        backend: (clickhouse|snowflake)\n        clickhouse_host: \n        clickhouse_database: \n        clickhouse_user:\n        clickhouse_password:\n        clickhouse_secure:\n        --or--\n        snowsql_account:\n        snowsql_database:\n        snowsql_schema:\n        snowsql_warehouse:\n        snowsql_user:\n        snowsql_pwd:\n        --or--\n        duckdb_path:\n\n# Usage\n\nGeneral way for run:\n```\nsource .env.local; pgwarehouse --config .local.yaml sync users\n```\n\nOnce the credentials are configured you can start syncing data. Start by listing tables from the Postgres database:\n\n    pgwarehouse list\n\nAnd you can see which tables exist so far in the warehouse:\n\n    pgwarehouse listwh\n    \nNow use `sync` to sync a table (eg. the \'users\' table):\n\n    pgwarehouse sync users\n\nData will be downloaded from the Postgres database into CSV files on the local machine, and then those files will be uploaded to the warehouse. Running `pgwarehouse listwh` will show the new table.\n\n## Updating a table\n\nAfter the initial sync has run, you can update the warehouse table with new records by running `sync` again:\n\n    pgwarehouse sync users\n\nSee [update strategies](#table-update-strategies) for different ways to update your table on each sync.\n\n## Syncing multiple tables\n\nThere are two ways to manage multiple tables. The first is just to pass `all` in place of the table name:\n\n    pgwarehouse sync all\n\nThis will attempt to sync ALL tables from Postgres into the warehouse. This could take a while!\n\nThe other way is to specify the `tables` list in the config file:\n\n    tables:\n        - users\n        - charges\n        - logs\n\nNow when you specify `sync all` the tool will use the list of tables specified in the config file.\n\n**Pro tip!** You can add the `max_records` settings to your `postgres` configuration to limit the number\nof records copied per table. This can be useful for testing the initial sync in case you have some\nlarge tables. Set this value to something reasonable (like 10000) and then try syncrhonizing all\ntables to make sure they copy properly. Once you have verified the tables in the warehouse then you\ncan remove this setting, drop any large tables, and then copy them in full (just run `sync all` again).\n\n## Table update strategies\n\n#### New Records Only (default)\nThe default update strategy is "new records only". This is done by selecting records with a greater value\nfor their primary id column than the greatest value currently in the warehouse. This strategy is simple\nand quick, but only works for monotonically incrementing primary keys, and only finds new records.\n\n#### Reload each time\nAnother supported strategy is "reload each time". This is the simplest strategy and we simply reload the\nentire table every time we sync. This strategy should be fine for small-ish tables (like <10m rows).\n\n#### Last Modified\nFinally, if your table has a `last modified` column then you can use the "all modifications strategy".\nIn this case all records with a `last modified` timestamp greater than the maximum value found in the\nwarehouse will be selected and "upserted" into the warehouse. Records that are already present\n(via matching the primary key) will be updated, and new records will be inserted.\n\n* The Snowflake backend uses the [MERGE](https://docs.snowflake.com/en/sql-reference/sql/merge) operation. \n* The Clickhouse backend uses `ALTER TABLE .. DELETE` to remove matching records and then `INSERT` to insert the new values.\n\n### What about deletes?\n\nThere is no simple way to capture deletes - you have to reload the entire table. A common pattern is\nto apply new records on a daily basis, and reload the entire table every week to remove deleted records.\n\n### What if my table has no primary key?\n\nAll the update strategies except "reload each time" require your table to have a primary key column.\n\n## Specifying update strategy at the command line\n\n    pgwarehouse sync <table>   (defaults to NEW RECORDS)\n    pgwarehouse sync <table> last_modified=<last modified column>   (MODIFIED RECORDS)\n    pgwarehouse reload <table> (reloads the whole table)\n\n## Specifying update strategy in the config file\n\nYou can configure the update strategy selectively for each table in the config file. To do so,\nspecify the table as a nested dictionary with options:\n\n    tables:\n        - accounts\n        - users:\n            reload: true\n        - orders:\n            last_modified: updated_at\n        - shoppers\n            last_modified: update_time\n            reload: sun\n        - original_orders:\n            skip: true\n\nIn this example:\n\n* `accounts` will have new records only applied at each sync\n* `users` will be reloaded completely on each sync\n* `orders` will have modified records (found by the \'updated_at\' column) applied on each sync\n* `shoppers` will have modified records applied on each sync, except for any sync\nwhich happens on Sunday, in which case the entire table will be reloaded.\n* `original_orders` will be skipped entirely\n\nThe `reload` argument can take 3 forms:\n\n    reload: true    - reload the table every sync\n    reload: [sun,mon,tue,wed,thur,fri]  - reload if the sync occurs on this day of the week\n    reload: 1-31    - reload if the sync occurs on this numeric day of the month (don\'t use 31!)\n\n## Scheduling regular data syncs\n\n`pgwarehouse` does not including any scheduling itself, you will need an external trigger like\n`cron`, [Heroku Scheduler](https://devcenter.heroku.com/articles/scheduler), or a K8s\n[CronJob](https://kubernetes.io/docs/tasks/job/automated-tasks-with-cron-jobs/).\n\nWhen running, the tool will need access to local storage - potentially a lot if you are synchronizing\nbig tables. But nothing needs to persist between sync runs (except the config file) - the tool \nonly relies on state it can query from Postgres or the warehouse.\n\n## Troubleshooting\n\nSometimes when you are testing things out it can be helpful to do the sync in two phases:\n1)download the data, 2)upload the data. You can use `extract` and `load` for this:\n\n    pgwarehouse extract <table>     - only downloads data\n    pgwarehouse load <table>        - loads the data into the warehouse\n\nWhen the `extract` process runs, its stores data in `./pgw_data/<table name>_data`. As\nfiles are uploaded they are moved into an `archive` subdirectory. When the **next sync**\nruns then this archive directory will be cleaned up. This allows you to go examine\nthe CSV downloaded data in case the upload fails for some reason. \n\n## Development\n\nRequirements:\n```bash\nsudo apt install libpq-dev postgresql postgresql-contrib\n```\n\nRun tests:\n```poetry run python -m pytest```\n\n## Limitations\n\nColumn type mapping today is [very limited](https://github.com/scottpersinger/pgwarehouse/blob/a20dc316bbdbc78317cfdd796216a847919d8755/pgwarehouse/snowflake_backend.py). More esoteric column types like JSON or ARRAY are simply\nmapped as VARCHAR columns. Some of these types are supported in the warehouse and could be\nimplemented more accurately.\n\nComposite primary keys (using multiple columns) have limited support. Today they will only work\nwith the RELOAD strategy.\n\nNon-numeric primary key types (like UUIDs) probably won\'t work unless they have a good lexigraphic\nsort that supports a `>` where clause.\n\n\n\n',
     'author': 'Scott Persinger',
     'author_email': 'scottpersinger@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pgwarehouse-0.1.3/PKG-INFO` & `pgwarehouse-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgwarehouse
-Version: 0.1.3
+Version: 0.1.4
 Summary: Easily sync your Postgres database to your data warehouse.
 Author: Scott Persinger
 Author-email: scottpersinger@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -67,22 +67,24 @@
 
 Again you can use the environment or the config file. Set these sets of vars in your env:
 
     CLICKHOUSE_HOST
     CLICKHOUSE_DATABASE
     CLICKHOUSE_USER
     CLICKHOUSE_PWD
+    CLICKHOUSE_SECURE
 
 or
 
     SNOWSQL_ACCOUNT
     SNOWSQL_DATABASE
     SNOWSQL_SCHEMA
     SNOWSQL_WAREHOUSE
     SNOWSQL_USER
+    SNOWSQL_ROLE
     SNOWSQL_PWD
 
 or
 
     DUCKDB_PATH (path to the duckdb database file)
 
 (The Snowflake parameters are the same as those for the [SnowSQL](https://docs.snowflake.com/en/user-guide/snowsql-start)
@@ -92,26 +94,32 @@
 
     warehouse:
         backend: (clickhouse|snowflake)
         clickhouse_host: 
         clickhouse_database: 
         clickhouse_user:
         clickhouse_password:
+        clickhouse_secure:
         --or--
         snowsql_account:
         snowsql_database:
         snowsql_schema:
         snowsql_warehouse:
         snowsql_user:
         snowsql_pwd:
         --or--
         duckdb_path:
 
 # Usage
 
+General way for run:
+```
+source .env.local; pgwarehouse --config .local.yaml sync users
+```
+
 Once the credentials are configured you can start syncing data. Start by listing tables from the Postgres database:
 
     pgwarehouse list
 
 And you can see which tables exist so far in the warehouse:
 
     pgwarehouse listwh
@@ -239,14 +247,24 @@
     pgwarehouse load <table>        - loads the data into the warehouse
 
 When the `extract` process runs, its stores data in `./pgw_data/<table name>_data`. As
 files are uploaded they are moved into an `archive` subdirectory. When the **next sync**
 runs then this archive directory will be cleaned up. This allows you to go examine
 the CSV downloaded data in case the upload fails for some reason. 
 
+## Development
+
+Requirements:
+```bash
+sudo apt install libpq-dev postgresql postgresql-contrib
+```
+
+Run tests:
+```poetry run python -m pytest```
+
 ## Limitations
 
 Column type mapping today is [very limited](https://github.com/scottpersinger/pgwarehouse/blob/a20dc316bbdbc78317cfdd796216a847919d8755/pgwarehouse/snowflake_backend.py). More esoteric column types like JSON or ARRAY are simply
 mapped as VARCHAR columns. Some of these types are supported in the warehouse and could be
 implemented more accurately.
 
 Composite primary keys (using multiple columns) have limited support. Today they will only work
```

