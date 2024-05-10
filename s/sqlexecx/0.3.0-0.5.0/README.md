# Comparing `tmp/sqlexecx-0.3.0.tar.gz` & `tmp/sqlexecx-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlexecx-0.3.0.tar", last modified: Fri May 10 12:27:21 2024, max compression
+gzip compressed data, was "sqlexecx-0.5.0.tar", last modified: Fri May 10 13:25:13 2024, max compression
```

## Comparing `sqlexecx-0.3.0.tar` & `sqlexecx-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 12:27:21.594502 sqlexecx-0.3.0/
--rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlexecx-0.3.0/LICENSE
--rw-r--r--   0 summy      (501) staff       (20)     7526 2024-05-10 12:27:21.593293 sqlexecx-0.3.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlexecx-0.3.0/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-10 12:27:21.594796 sqlexecx-0.3.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1328 2024-05-10 12:27:13.000000 sqlexecx-0.3.0/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 12:27:21.583775 sqlexecx-0.3.0/sqlexecx/
--rw-r--r--   0 summy      (501) staff       (20)     2468 2024-05-05 01:28:17.000000 sqlexecx-0.3.0/sqlexecx/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)      641 2024-04-26 08:01:55.000000 sqlexecx-0.3.0/sqlexecx/constant.py
--rw-r--r--   0 summy      (501) staff       (20)     8887 2024-05-04 09:44:00.000000 sqlexecx-0.3.0/sqlexecx/dialect.py
--rw-r--r--   0 summy      (501) staff       (20)    18625 2024-05-04 08:51:07.000000 sqlexecx-0.3.0/sqlexecx/exec.py
--rw-r--r--   0 summy      (501) staff       (20)     1936 2024-04-25 04:18:32.000000 sqlexecx-0.3.0/sqlexecx/loader.py
--rw-r--r--   0 summy      (501) staff       (20)      822 2024-05-04 04:35:42.000000 sqlexecx-0.3.0/sqlexecx/log_support.py
--rw-r--r--   0 summy      (501) staff       (20)     3231 2024-05-10 12:27:13.000000 sqlexecx-0.3.0/sqlexecx/page_exec.py
--rw-r--r--   0 summy      (501) staff       (20)    20095 2024-05-10 12:27:13.000000 sqlexecx-0.3.0/sqlexecx/sql_exec.py
--rw-r--r--   0 summy      (501) staff       (20)     3076 2024-05-04 04:36:08.000000 sqlexecx-0.3.0/sqlexecx/sql_support.py
--rw-r--r--   0 summy      (501) staff       (20)    18712 2024-05-10 12:27:13.000000 sqlexecx-0.3.0/sqlexecx/table_exec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 12:27:21.590549 sqlexecx-0.3.0/sqlexecx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     7526 2024-05-10 12:27:21.000000 sqlexecx-0.3.0/sqlexecx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      442 2024-05-10 12:27:21.000000 sqlexecx-0.3.0/sqlexecx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-10 12:27:21.000000 sqlexecx-0.3.0/sqlexecx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-10 12:27:21.000000 sqlexecx-0.3.0/sqlexecx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       20 2024-05-10 12:27:21.000000 sqlexecx-0.3.0/sqlexecx.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)        9 2024-05-10 12:27:21.000000 sqlexecx-0.3.0/sqlexecx.egg-info/top_level.txt
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 12:27:21.591460 sqlexecx-0.3.0/test/
--rw-r--r--   0 summy      (501) staff       (20)     1192 2024-04-08 10:07:10.000000 sqlexecx-0.3.0/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 13:25:13.924386 sqlexecx-0.5.0/
+-rw-r--r--   0 summy      (501) staff       (20)    11357 2024-01-23 07:49:56.000000 sqlexecx-0.5.0/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     7526 2024-05-10 13:25:13.922973 sqlexecx-0.5.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     6974 2024-03-29 02:19:13.000000 sqlexecx-0.5.0/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-10 13:25:13.924687 sqlexecx-0.5.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1328 2024-05-10 13:25:09.000000 sqlexecx-0.5.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 13:25:13.908932 sqlexecx-0.5.0/sqlexecx/
+-rw-r--r--   0 summy      (501) staff       (20)     2468 2024-05-05 01:28:17.000000 sqlexecx-0.5.0/sqlexecx/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)      641 2024-04-26 08:01:55.000000 sqlexecx-0.5.0/sqlexecx/constant.py
+-rw-r--r--   0 summy      (501) staff       (20)     8887 2024-05-04 09:44:00.000000 sqlexecx-0.5.0/sqlexecx/dialect.py
+-rw-r--r--   0 summy      (501) staff       (20)    18673 2024-05-10 13:23:17.000000 sqlexecx-0.5.0/sqlexecx/exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     1936 2024-04-25 04:18:32.000000 sqlexecx-0.5.0/sqlexecx/loader.py
+-rw-r--r--   0 summy      (501) staff       (20)      822 2024-05-04 04:35:42.000000 sqlexecx-0.5.0/sqlexecx/log_support.py
+-rw-r--r--   0 summy      (501) staff       (20)     3231 2024-05-10 12:27:13.000000 sqlexecx-0.5.0/sqlexecx/page_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)    20095 2024-05-10 12:27:13.000000 sqlexecx-0.5.0/sqlexecx/sql_exec.py
+-rw-r--r--   0 summy      (501) staff       (20)     3076 2024-05-04 04:36:08.000000 sqlexecx-0.5.0/sqlexecx/sql_support.py
+-rw-r--r--   0 summy      (501) staff       (20)    19204 2024-05-10 13:23:17.000000 sqlexecx-0.5.0/sqlexecx/table_exec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 13:25:13.914648 sqlexecx-0.5.0/sqlexecx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     7526 2024-05-10 13:25:13.000000 sqlexecx-0.5.0/sqlexecx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      442 2024-05-10 13:25:13.000000 sqlexecx-0.5.0/sqlexecx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-10 13:25:13.000000 sqlexecx-0.5.0/sqlexecx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-10 13:25:13.000000 sqlexecx-0.5.0/sqlexecx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       20 2024-05-10 13:25:13.000000 sqlexecx-0.5.0/sqlexecx.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)        9 2024-05-10 13:25:13.000000 sqlexecx-0.5.0/sqlexecx.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-10 13:25:13.915636 sqlexecx-0.5.0/test/
+-rw-r--r--   0 summy      (501) staff       (20)     1192 2024-04-08 10:07:10.000000 sqlexecx-0.5.0/test/test.py
```

### Comparing `sqlexecx-0.3.0/LICENSE` & `sqlexecx-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.3.0/PKG-INFO` & `sqlexecx-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlexecx
-Version: 0.3.0
+Version: 0.5.0
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions.     It blocked the differences in various databases. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
```

### Comparing `sqlexecx-0.3.0/README.rst` & `sqlexecx-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.3.0/setup.py` & `sqlexecx-0.5.0/setup.py`

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
-    version='0.3.0',
+    version='0.5.0',
     install_requires=[
         'sqlexecutorx>=0.8.0',
     ],
     url='https://gitee.com/summry/sqlexecx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Database', 'Python', 'RDB'],
```

### Comparing `sqlexecx-0.3.0/sqlexecx/__init__.py` & `sqlexecx-0.5.0/sqlexecx/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.3.0/sqlexecx/constant.py` & `sqlexecx-0.5.0/sqlexecx/constant.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.3.0/sqlexecx/dialect.py` & `sqlexecx-0.5.0/sqlexecx/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.3.0/sqlexecx/exec.py` & `sqlexecx-0.5.0/sqlexecx/exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,25 +473,25 @@
     sql = Dialect.before_execute(sql)
     args = sql_support.get_batch_args(*args)
     return _batch_execute(sql, *args)
 
 
 def batch_insert(table_name: str, *args):
     """
-    Batch insert
+    Batch insert data into table and return effect rowcount
 
     :param table_name: table name
     :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
 
     Examples
     --------
     >>> import sqlexecx as db
     >>> args =  [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
-    >>> db.batch_execute(sql, *args)
+    >>> db.batch_execute('person', *args)
     2
     """
     logger.debug("Exec func 'sqlexecx.%s' \n\t Table: '%s', args: %s" % ('batch_insert', table_name, args))
     sql, args = sql_support.batch_insert_sql_args(table_name, *args)
     return batch_execute(sql, *args)
```

### Comparing `sqlexecx-0.3.0/sqlexecx/loader.py` & `sqlexecx-0.5.0/sqlexecx/loader.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.3.0/sqlexecx/log_support.py` & `sqlexecx-0.5.0/sqlexecx/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.3.0/sqlexecx/page_exec.py` & `sqlexecx-0.5.0/sqlexecx/page_exec.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.3.0/sqlexecx/sql_exec.py` & `sqlexecx-0.5.0/sqlexecx/sql_exec.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.3.0/sqlexecx/sql_support.py` & `sqlexecx-0.5.0/sqlexecx/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlexecx-0.3.0/sqlexecx/table_exec.py` & `sqlexecx-0.5.0/sqlexecx/table_exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,39 +355,60 @@
         return self.exec.save(self.table, **kwargs)
 
     def save_select_key(self, select_key: str, **kwargs):
         """
         Insert data into table, return primary key.
 
         :param select_key: sql for select primary key
-        :param kwargs:
         :return: Primary key
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> select_key = 'SELECT LAST_INSERT_ID()'
+        >>> db.table('person').save_select_key(select_key, name='张三', age=20)
+        3
         """
         return self.exec.save_select_key(select_key, self.table, **kwargs)
 
     def batch_insert(self, *args):
         """
-        Execute sql return effect rowcount
-        :param args: [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
+        Batch insert data into table and return effect rowcount
+
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> args = [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
+        >>> db.table('person').batch_execute(*args)
+        2
         """
         return self.exec.batch_insert(self.table, *args)
 
     def get(self, column: str):
         """
         Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
+
         MultiColumnsError: Expect only one column.
 
-        sqlexecx.table('person').get('count(1)')
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').get('count(1)')
+        3
         """
         sql = get_table_select_sql(self.table, '', LIMIT_1, column)
         return self.exec.do_get(sql, LIMIT_1)
 
     def count(self):
         """
-        sqlexecx.table('person').count()
+        Examples
+        --------
+        >>> import sqlexecx as db
+        >>> db.table('person').count()
+        3
         """
         return self.get(SELECT_COUNT)
 
     def select(self, *columns):
         """
         sqlexecx.table('person').select('name', 'age')
         """
```

### Comparing `sqlexecx-0.3.0/sqlexecx.egg-info/PKG-INFO` & `sqlexecx-0.5.0/sqlexecx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlexecx
-Version: 0.3.0
+Version: 0.5.0
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage connections and transactions.     It blocked the differences in various databases. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
```

### Comparing `sqlexecx-0.3.0/test/test.py` & `sqlexecx-0.5.0/test/test.py`

 * *Files identical despite different names*

