# Comparing `tmp/sqlexecx-0.5.0.tar.gz` & `tmp/sqlexecx-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlexecx-0.5.0.tar", last modified: Fri May 10 13:25:13 2024, max compression
+gzip compressed data, was "sqlexecx-0.6.0.tar", last modified: Fri May 10 23:58:50 2024, max compression
```

## Comparing `sqlexecx-0.5.0.tar` & `sqlexecx-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 13:25:13.924386 sqlexecx-0.5.0/
--rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlexecx-0.5.0/LICENSE
--rw-r--r--   0 summy      (501) staff       (20)     7526 2024-05-10 13:25:13.922973 sqlexecx-0.5.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlexecx-0.5.0/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-10 13:25:13.924687 sqlexecx-0.5.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1328 2024-05-10 13:25:09.000000 sqlexecx-0.5.0/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 13:25:13.908932 sqlexecx-0.5.0/sqlexecx/
--rw-r--r--   0 summy      (501) staff       (20)     2468 2024-05-05 01:28:17.000000 sqlexecx-0.5.0/sqlexecx/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)      641 2024-04-26 08:01:55.000000 sqlexecx-0.5.0/sqlexecx/constant.py
--rw-r--r--   0 summy      (501) staff       (20)     8887 2024-05-04 09:44:00.000000 sqlexecx-0.5.0/sqlexecx/dialect.py
--rw-r--r--   0 summy      (501) staff       (20)    18673 2024-05-10 13:23:17.000000 sqlexecx-0.5.0/sqlexecx/exec.py
--rw-r--r--   0 summy      (501) staff       (20)     1936 2024-04-25 04:18:32.000000 sqlexecx-0.5.0/sqlexecx/loader.py
--rw-r--r--   0 summy      (501) staff       (20)      822 2024-05-04 04:35:42.000000 sqlexecx-0.5.0/sqlexecx/log_support.py
--rw-r--r--   0 summy      (501) staff       (20)     3231 2024-05-10 12:27:13.000000 sqlexecx-0.5.0/sqlexecx/page_exec.py
--rw-r--r--   0 summy      (501) staff       (20)    20095 2024-05-10 12:27:13.000000 sqlexecx-0.5.0/sqlexecx/sql_exec.py
--rw-r--r--   0 summy      (501) staff       (20)     3076 2024-05-04 04:36:08.000000 sqlexecx-0.5.0/sqlexecx/sql_support.py
--rw-r--r--   0 summy      (501) staff       (20)    19204 2024-05-10 13:23:17.000000 sqlexecx-0.5.0/sqlexecx/table_exec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 13:25:13.914648 sqlexecx-0.5.0/sqlexecx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     7526 2024-05-10 13:25:13.000000 sqlexecx-0.5.0/sqlexecx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      442 2024-05-10 13:25:13.000000 sqlexecx-0.5.0/sqlexecx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-10 13:25:13.000000 sqlexecx-0.5.0/sqlexecx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-10 13:25:13.000000 sqlexecx-0.5.0/sqlexecx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       20 2024-05-10 13:25:13.000000 sqlexecx-0.5.0/sqlexecx.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)        9 2024-05-10 13:25:13.000000 sqlexecx-0.5.0/sqlexecx.egg-info/top_level.txt
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 13:25:13.915636 sqlexecx-0.5.0/test/
--rw-r--r--   0 summy      (501) staff       (20)     1192 2024-04-08 10:07:10.000000 sqlexecx-0.5.0/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 23:58:50.460435 sqlexecx-0.6.0/
+-rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlexecx-0.6.0/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     7526 2024-05-10 23:58:50.459665 sqlexecx-0.6.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlexecx-0.6.0/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-10 23:58:50.460812 sqlexecx-0.6.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1328 2024-05-10 23:58:47.000000 sqlexecx-0.6.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 23:58:50.451519 sqlexecx-0.6.0/sqlexecx/
+-rw-r--r--   0 summy      (501) staff       (20)     2468 2024-05-05 01:28:17.000000 sqlexecx-0.6.0/sqlexecx/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)      641 2024-04-26 08:01:55.000000 sqlexecx-0.6.0/sqlexecx/constant.py
+-rw-r--r--   0 summy      (501) staff       (20)     8887 2024-05-04 09:44:00.000000 sqlexecx-0.6.0/sqlexecx/dialect.py
+-rw-r--r--   0 summy      (501) staff       (20)    18730 2024-05-10 23:58:33.000000 sqlexecx-0.6.0/sqlexecx/exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     1936 2024-04-25 04:18:32.000000 sqlexecx-0.6.0/sqlexecx/loader.py
+-rw-r--r--   0 summy      (501) staff       (20)      822 2024-05-04 04:35:42.000000 sqlexecx-0.6.0/sqlexecx/log_support.py
+-rw-r--r--   0 summy      (501) staff       (20)     3197 2024-05-10 23:58:33.000000 sqlexecx-0.6.0/sqlexecx/page_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)    19932 2024-05-10 23:58:33.000000 sqlexecx-0.6.0/sqlexecx/sql_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     3076 2024-05-04 04:36:08.000000 sqlexecx-0.6.0/sqlexecx/sql_support.py
+-rw-r--r--   0 summy      (501) staff       (20)    21504 2024-05-10 23:58:33.000000 sqlexecx-0.6.0/sqlexecx/table_exec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 23:58:50.457009 sqlexecx-0.6.0/sqlexecx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     7526 2024-05-10 23:58:50.000000 sqlexecx-0.6.0/sqlexecx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      442 2024-05-10 23:58:50.000000 sqlexecx-0.6.0/sqlexecx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-10 23:58:50.000000 sqlexecx-0.6.0/sqlexecx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-10 23:58:50.000000 sqlexecx-0.6.0/sqlexecx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       20 2024-05-10 23:58:50.000000 sqlexecx-0.6.0/sqlexecx.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)        9 2024-05-10 23:58:50.000000 sqlexecx-0.6.0/sqlexecx.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 23:58:50.457897 sqlexecx-0.6.0/test/
+-rw-r--r--   0 summy      (501) staff       (20)     1192 2024-04-08 10:07:10.000000 sqlexecx-0.6.0/test/test.py
```

### Comparing `sqlexecx-0.5.0/LICENSE` & `sqlexecx-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.5.0/PKG-INFO` & `sqlexecx-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlexecx
-Version: 0.5.0
+Version: 0.6.0
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions.     It blocked the differences in various databases. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
```

### Comparing `sqlexecx-0.5.0/README.rst` & `sqlexecx-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.5.0/setup.py` & `sqlexecx-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 setup(
     name='sqlexecx',
     packages=['sqlexecx'],
     description="A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions.\
      It blocked the differences in various databases. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.5.0',
+    version='0.6.0',
     install_requires=[
         'sqlexecutorx>=0.8.0',
     ],
     url='https://gitee.com/summry/sqlexecx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Database', 'Python', 'RDB'],
```

### Comparing `sqlexecx-0.5.0/sqlexecx/__init__.py` & `sqlexecx-0.6.0/sqlexecx/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.5.0/sqlexecx/constant.py` & `sqlexecx-0.6.0/sqlexecx/constant.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.5.0/sqlexecx/dialect.py` & `sqlexecx-0.6.0/sqlexecx/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.5.0/sqlexecx/exec.py` & `sqlexecx-0.6.0/sqlexecx/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
     sql, args = sql_support.try_mapping('sqlexecx.get', sql, *args, **kwargs)
     return do_get(sql, *args)
 
 
 def select(sql: str, *args, **kwargs):
     """
-    Execute select SQL and return unique result or list results(tuple).
+    Execute select SQL and return list results(tuple).
 
     Examples
     --------
     >>> import sqlexecx as db
     >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=?'
     >>> db.select(sql, '张三', 20)
     [(3, '张三', 20)]
@@ -305,15 +305,15 @@
     sql, args = sql_support.limit_one_sql_args(sql, *args)
     sql = Dialect.before_execute(sql)
     return _get(sql, *args)
 
 
 def do_select(sql: str, *args):
     """
-    Execute select SQL and return unique result or list results(tuple).
+    Execute select SQL and return list results(tuple).
 
     Examples
     --------
     >>> import sqlexecx as db
     >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=?'
     >>> db.do_select(sql, '张三', 20)
     [(3, '张三', 20)]
@@ -493,15 +493,15 @@
     logger.debug("Exec func 'sqlexecx.%s' \n\t Table: '%s', args: %s" % ('batch_insert', table_name, args))
     sql, args = sql_support.batch_insert_sql_args(table_name, *args)
     return batch_execute(sql, *args)
 
 
 def load(sql: str, *args, **kwargs) -> Loader:
     """
-    Execute select SQL and return Loader instance
+    Execute select SQL and return a Loader instance
 
     :param sql: SQL to be executed
     :return: Loader
 
     Examples
     --------
     >>> import sqlexecx as db
@@ -514,39 +514,39 @@
     """
     sql, args = sql_support.try_mapping('sqlexecx.csv', sql, *args, **kwargs)
     return do_load(sql, *args)
 
 
 def do_load(sql: str, *args) -> Loader:
     """
-    Execute select SQL and return Loader instance
+    Execute select SQL and return a Loader instance
 
     :param sql: SQL to be executed
     :return: Loader
 
     Examples
     --------
     >>> import sqlexecx as db
     >>> sql = 'SELECT id, name, age FROM person WHERE name=? and age=?'
     >>> db.do_load(sql, '张三', 20)
     Lodder()
     """
-
     sql = Dialect.before_execute(sql)
     return Loader(*_do_select(sql, *args))
 
 
 def insert_from_csv(file_name: str, table_name: str, delimiter=',', header=True, columns: Collection[str] = None, encoding='utf-8') -> int:
     """
-    Read data from csv file, and insert into table
+    Insert data into table from a csv file and return effected rowcount.
 
     Examples
     --------
     >>> import sqlexecx as db
     >>> db.insert_from_csv('test.csv', 'person')
+    20
     """
 
     import csv
     sql = None
     if columns and len(columns) > 0:
         sql = sql_support.insert_sql(table_name.strip(), columns)
     elif not header:
@@ -568,35 +568,36 @@
         lines = lines[1:]
 
     return batch_execute(sql, lines)
 
 
 def insert_from_df(df, table_name: str, columns: Collection[str] = None) -> int:
     """
-    Insert data into table from pandas DataFrame
+    Insert data into table from pandas DataFrame and return effected rowcount.
 
     Examples
     --------
     >>> import sqlexecx as db
     >>> db.insert_from_df(df, 'person')
     """
 
     columns = columns if columns and len(columns) > 0 else df.columns.tolist()
     sql = sql_support.insert_sql(table_name.strip(), columns)
     return batch_execute(sql, df.values.tolist())
 
 
 def insert_from_json(file_name: str, table_name: str, encoding='utf-8') -> int:
     """
-    Read data from json file, and insert into table
+    Insert data into table from a json file and return effected rowcount.
 
     Examples
     --------
     >>> import sqlexecx as db
     >>> db.insert_from_json('test.json', 'person')
+    20
 
     many rows json file example:
     [{"id": 1, "name": "张三", "age": 55}, ...]
 
     one row json file example:
     {"id": 1, "name": "张三", "age": 55}
     """
```

### Comparing `sqlexecx-0.5.0/sqlexecx/loader.py` & `sqlexecx-0.6.0/sqlexecx/loader.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.5.0/sqlexecx/log_support.py` & `sqlexecx-0.6.0/sqlexecx/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.5.0/sqlexecx/page_exec.py` & `sqlexecx-0.6.0/sqlexecx/page_exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
              SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
         """
         return self.exec.query_page(sql, self.page_num, self.page_size, *args, **kwargs)
 
     def select(self, sql: str, *args, **kwargs):
         """
-        Execute select SQL and return unique result or list results(tuple).
+        Execute select SQL and return list results(tuple).
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.page(1, 10).select('SELECT id, name, age FROM person WHERE name=? and age=?', '张三', 20)
         [(3, '张三', 20)]
         >>> db.page(1, 10).select('SELECT id, name, age FROM person WHERE name=:name and age=:age', name='张三', age=20)
@@ -58,15 +58,15 @@
         Execute select SQL and return list results(dict).
         sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
         """
         return self.exec.do_query_page(sql, self.page_num, self.page_size, *args)
 
     def do_select(self, sql: str, *args):
         """
-        Execute select SQL and return unique result or list results(tuple).
+        Execute select SQL and return list results(tuple).
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.page(1, 10).do_select('SELECT id, name, age FROM person WHERE name=? and age=? LIMIT 1', '张三', 20)
         (3, '张三', 20)
         """
```

### Comparing `sqlexecx-0.5.0/sqlexecx/sql_exec.py` & `sqlexecx-0.6.0/sqlexecx/sql_exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,41 +24,41 @@
         >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').page(1, 10).query(name='张三', age=20)
         [{'id': 3, 'name': '张三', 'age': 20}]
         """
         return self.page_exec.query(self.sql, *args, **kwargs)
 
     def select(self, *args, **kwargs):
         """
-        Execute select SQL and return unique result or list results(tuple).
+        Execute select SQL and return list results(tuple).
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').page(1, 10).select('张三', 20)
         [(3, '张三', 20)]
         >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').page(1, 10).select(name='张三', age=20)
         [(3, '张三', 20)]
         """
         return self.page_exec.select(self.sql, *args, **kwargs)
 
     def do_query(self, *args):
         """
-        Execute select SQL and return unique result or list results(tuple).
+        Execute select SQL and return list results(tuple).
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').page(1, 10).do_query('张三', 20)
         [{'id': 3, 'name': '张三', 'age': 20}]
         """
         return self.page_exec.do_query(self.sql, *args)
 
     def do_select(self, *args):
         """
-        Execute select SQL and return unique result or list results(tuple).
+        Execute select SQL and return list results(tuple).
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').page(1, 10).do_select('张三', 20)
         [(3, '张三', 20)]
         """
@@ -84,15 +84,15 @@
         >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').param(name='张三', age=20).page(1, 10).query()
         [{'id': 3, 'name': '张三', 'age': 20}]
         """
         return self.sql_page_exec.query(*self.args, **self.kwargs)
 
     def select(self):
         """
-        Execute select SQL and return unique result or list results(tuple).
+        Execute select SQL and return list results(tuple).
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').param('张三', 20).page(1, 10).select()
         [(3, '张三', 20)]
         >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').param(name='张三', age=20).page(1, 10).select()
@@ -172,15 +172,15 @@
         >>> db.sql('SELECT count(1) FROM person WHERE name=:name and age=:age LIMIT 1').param(name='张三', age=20).get()
         1
         """
         return self.sql_exec.get(*self.args, **self.kwargs)
 
     def select(self):
         """
-        Execute select SQL and return unique result or list results(tuple).
+        Execute select SQL and return list results(tuple).
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').param('张三', 18).select()
         [(3, '张三', 20)]
         >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').param(name='张三', age=20).select()
@@ -347,15 +347,15 @@
         >>> db.sql('SELECT count(1) FROM person WHERE name=:name and age=:age LIMIT 1').get(name='张三', age=20)
         1
         """
         return self.exec.get(self.sql, *args, **kwargs)
 
     def select(self, *args, **kwargs):
         """
-        Execute select SQL and return unique result or list results(tuple).
+        Execute select SQL and return list results(tuple).
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').select('张三', 20)
         [(3, '张三', 20)]
         >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').select(name='张三', age=20)
@@ -446,15 +446,15 @@
         >>> db.sql('SELECT count(1) FROM person WHERE name=? and age=? LIMIT 1').do_get('张三', 20)
         1
         """
         return self.exec.do_get(self.sql, *args)
 
     def do_select(self, *args):
         """
-        Execute select SQL and return unique result or list results(tuple).
+        Execute select SQL and return list results(tuple).
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=? LIMIT 1').do_select('张三', 20)
         (3, '张三', 20)
         """
@@ -513,55 +513,55 @@
         >>> db.sql('INSERT INTO person(name, age) VALUES(:name, :age)').batch_execute(sql, *args)
         2
         """
         return self.exec.batch_execute(self.sql, *args)
 
     def load(self, *args, **kwargs) -> Loader:
         """
-        Execute select SQL and return Loader instance
+        Execute select SQL and return a Loader instance
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').load('张三', 20)
         Lodder()
         >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').load(name='张三', age=20)
         Lodder()
         """
         return self.exec.load(self.sql, *args, **kwargs)
 
     def do_load(self, *args) -> Loader:
         """
-        Execute select SQL and return Loader instance
+        Execute select SQL and return a Loader instance
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').load('张三', 20)
         Lodder()
         """
         return self.exec.do_load(self.sql, *args)
 
     def param(self, *args, **kwargs) -> Param:
         """
-        Execute select SQL and return Param instance
+        Get a Param instance
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').param('张三', 20)
         Param()
         >>> db.sql('SELECT id, name, age FROM person WHERE name=:name and age=:age').param(name='张三', age=20)
         Param()
         """
         return Param(self, *args, **kwargs)
 
     def page(self, page_num=1, page_size=10) -> SqlPageExec:
         """
-        Execute select SQL and return SqlPageExec instance
+        Get a SqlPageExec instance
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.sql('SELECT id, name, age FROM person WHERE name=? and age=?').page(1, 10)
         SqlPageExec()
         """
```

### Comparing `sqlexecx-0.5.0/sqlexecx/sql_support.py` & `sqlexecx-0.6.0/sqlexecx/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.5.0/sqlexecx/table_exec.py` & `sqlexecx-0.6.0/sqlexecx/table_exec.py`

 * *Files 14% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     def __init__(self, where_exec, *columns):
         self._where_exec = where_exec
         self.columns = columns
 
     def get(self):
         """
-        Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+        Select data from table and expected one int and only one int result, SQL contain 'limit'.
         MultiColumnsError: Expect only one column.
 
         sqlexecx.table('person').columns('name').where(id=1).get()
         """
         return self._where_exec.get(self.columns[0])
 
     def select(self):
@@ -133,15 +133,16 @@
     def __init__(self, _exec, table_name, **kwargs):
         self.exec = _exec
         self.table = table_name
         self.where_condition = kwargs
 
     def get(self, column: str):
         """
-        Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+        Select data from table and expected one int and only one int result, SQL contain 'limit'.
+        
         MultiColumnsError: Expect only one column.
 
         sqlexecx.table('person').where(name='李四').get('id')
         """
         sql, args = self.get_select_one_sql_args(column)
         return self.exec.do_get(sql, *args, LIMIT_1)
 
@@ -381,15 +382,15 @@
         >>> db.table('person').batch_execute(*args)
         2
         """
         return self.exec.batch_insert(self.table, *args)
 
     def get(self, column: str):
         """
-        Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+        Select data from table and expected one int and only one int result, SQL contain 'limit'.
 
         MultiColumnsError: Expect only one column.
 
         Examples
         --------
         >>> import sqlexecx as db
         >>> db.table('person').get('count(1)')
@@ -406,81 +407,173 @@
         >>> db.table('person').count()
         3
         """
         return self.get(SELECT_COUNT)
 
     def select(self, *columns):
         """
-        sqlexecx.table('person').select('name', 'age')
+        Select data from table and return list results(tuple).
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').select('id', 'name', 'age')
+        [(3, '张三', 20)]
         """
         sql = get_table_select_sql(self.table, '', 0, *columns)
         return self.exec.do_select(sql)
 
     def select_one(self, *columns):
         """
-        sqlexecx.table('person').select_one('name', 'age')
+        Select data from table and return unique result(tuple), SQL contain 'limit'.
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').do_select_one('id', 'name', 'age')
+        (3, '张三', 20)
         """
         sql = get_table_select_sql(self.table, '', LIMIT_1, *columns)
         return self.exec.do_select_one(sql, LIMIT_1)
 
     def query(self, *columns):
         """
-        sqlexecx.table('person').query('name', 'age')
+        Select data from table and return list results(dict).
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').query('id', 'name', 'age')
+        [{'id': 3, 'name': '张三', 'age': 20}]
         """
         sql = get_table_select_sql(self.table, '', 0, *columns)
         return self.exec.do_query(sql)
 
     def query_one(self, *columns):
         """
-        sqlexecx.table('person').query_one('name', 'age')
+        Select data from table and return unique result(dict), SQL contain 'limit'.
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').query_one('id', 'name', 'age')
+        {'id': 3, 'name': '张三', 'age': 20}
         """
         sql = get_table_select_sql(self.table, '', LIMIT_1, *columns)
         return self.exec.do_query_one(sql, LIMIT_1)
 
     def load(self, *columns) -> Loader:
         """
-        sqlexecx.table('person').load('name', 'age')
+        Execute select SQL and return a Loader instance
+
+        :return: Loader
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').load('id', 'name', 'age')
+        Lodder()
         """
         sql = get_table_select_sql(self.table, '', 0, *columns)
-
         return self.exec.do_load(sql)
 
     def insert_from_csv(self, file_name: str, delimiter=',', header=True, columns: Tuple[str] = None, encoding='utf-8'):
         """
-        sqlexecx.table('person').insert_from_csv('test.csv')
+        Insert data into table from a csv file and return effected rowcount.
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').insert_from_csv('test.csv')
+        20
         """
         return self.exec.insert_from_csv(file_name, self.table, delimiter, header, columns, encoding=encoding)
 
     def insert_from_df(self, df, columns: Tuple[str] = None):
         """
-        sqlexecx.table('person').insert_from_df(df)
+        Insert data into table from pandas DataFrame and return effected rowcount.
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').insert_from_df(df)
+        20
         """
         return self.exec.insert_from_df(df, self.table, columns)
 
     def insert_from_json(self, file_name: str, encoding='utf-8'):
         """
-        sqlexecx.table('person').insert_from_json('test.csv')
+        Insert data into table from a json file and return effected rowcount.
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').insert_from_json('test.json')
+        20
         """
         return self.exec.insert_from_json(file_name, self.table, encoding=encoding)
 
     def truncate(self) -> int:
-        """ sqlexecx.table('person').truncate() """
+        """
+        Truncate table and return effected rowcount
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').truncate()
+        1
+        """
         return self.exec.truncate(self.table)
 
     def drop(self) -> int:
-        """ sqlexecx.table('person').drop() """
+        """
+        Drop table and return effected rowcount
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').drop()
+        1
+        """
         return self.exec.drop(self.table)
 
     def where(self, **kwargs) -> WhereExec:
+        """
+        Get a WhereExec instance
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').where(name='张三', age=20)
+        WhereExec()
+        """
         return WhereExec(self.exec, self.table, **kwargs)
 
     def columns(self, *columns) -> ColumnExec:
+        """
+        Get a ColumnExec instance
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').columns('id', 'name', 'age')
+        ColumnExec()
+        """
         return ColumnExec(self, *columns)
 
     def page(self, page_num=1, page_size=10) -> TablePageExec:
+        """
+        Get a TablePageExec instance
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').page(1, 10)
+        TablePageExec()
+        """
         return TablePageExec(self,  page_num, page_size)
 
 
 def table(table_name: str) -> TableExec:
     """
     Get a TableExec instance
```

### Comparing `sqlexecx-0.5.0/sqlexecx.egg-info/PKG-INFO` & `sqlexecx-0.6.0/sqlexecx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlexecx
-Version: 0.5.0
+Version: 0.6.0
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions.     It blocked the differences in various databases. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
```

### Comparing `sqlexecx-0.5.0/test/test.py` & `sqlexecx-0.6.0/test/test.py`

 * *Files identical despite different names*

