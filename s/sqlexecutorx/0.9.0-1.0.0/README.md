# Comparing `tmp/sqlexecutorx-0.9.0.tar.gz` & `tmp/sqlexecutorx-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlexecutorx-0.9.0.tar", last modified: Mon May  6 02:42:30 2024, max compression
+gzip compressed data, was "sqlexecutorx-1.0.0.tar", last modified: Sat May 11 00:29:55 2024, max compression
```

## Comparing `sqlexecutorx-0.9.0.tar` & `sqlexecutorx-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-06 02:42:30.584761 sqlexecutorx-0.9.0/
--rw-rw-r--   0 summy      (501) staff       (20)    11357 2024-03-14 05:16:15.000000 sqlexecutorx-0.9.0/LICENSE
--rw-r--r--   0 summy      (501) staff       (20)     2027 2024-05-06 02:42:30.584046 sqlexecutorx-0.9.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     1577 2024-05-04 03:23:13.000000 sqlexecutorx-0.9.0/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-06 02:42:30.585092 sqlexecutorx-0.9.0/setup.cfg
--rw-rw-r--   0 summy      (501) staff       (20)     1168 2024-05-06 02:42:23.000000 sqlexecutorx-0.9.0/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-06 02:42:30.574273 sqlexecutorx-0.9.0/sqlexecutorx/
--rw-rw-r--   0 summy      (501) staff       (20)     1373 2024-05-05 01:28:17.000000 sqlexecutorx-0.9.0/sqlexecutorx/__init__.py
--rw-rw-r--   0 summy      (501) staff       (20)      209 2024-05-04 03:22:15.000000 sqlexecutorx-0.9.0/sqlexecutorx/constant.py
--rw-rw-r--   0 summy      (501) staff       (20)    11285 2024-05-05 01:22:27.000000 sqlexecutorx-0.9.0/sqlexecutorx/core.py
--rw-r--r--   0 summy      (501) staff       (20)      901 2024-03-23 15:57:10.000000 sqlexecutorx-0.9.0/sqlexecutorx/engine.py
--rw-rw-r--   0 summy      (501) staff       (20)     2063 2024-05-05 02:01:30.000000 sqlexecutorx-0.9.0/sqlexecutorx/init_import.py
--rw-rw-r--   0 summy      (501) staff       (20)      739 2024-05-06 02:41:09.000000 sqlexecutorx-0.9.0/sqlexecutorx/log_support.py
--rw-rw-r--   0 summy      (501) staff       (20)     1031 2024-05-04 03:22:15.000000 sqlexecutorx-0.9.0/sqlexecutorx/pooling.py
--rw-r--r--   0 summy      (501) staff       (20)      422 2024-03-29 05:50:43.000000 sqlexecutorx-0.9.0/sqlexecutorx/sql_support.py
--rw-rw-r--   0 summy      (501) staff       (20)     3892 2024-03-25 02:25:33.000000 sqlexecutorx-0.9.0/sqlexecutorx/support.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-06 02:42:30.582888 sqlexecutorx-0.9.0/sqlexecutorx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     2027 2024-05-06 02:42:30.000000 sqlexecutorx-0.9.0/sqlexecutorx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      432 2024-05-06 02:42:30.000000 sqlexecutorx-0.9.0/sqlexecutorx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-06 02:42:30.000000 sqlexecutorx-0.9.0/sqlexecutorx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-05 02:08:23.000000 sqlexecutorx-0.9.0/sqlexecutorx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-06 02:42:30.000000 sqlexecutorx-0.9.0/sqlexecutorx.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-11 00:29:55.734527 sqlexecutorx-1.0.0/
+-rw-rw-r--   0 summy      (501) staff       (20)    11357 2024-03-14 05:16:15.000000 sqlexecutorx-1.0.0/LICENSE
+-rw-r--r--   0 summy      (501) staff       (20)     2027 2024-05-11 00:29:55.731834 sqlexecutorx-1.0.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     1577 2024-05-04 03:23:13.000000 sqlexecutorx-1.0.0/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-11 00:29:55.734778 sqlexecutorx-1.0.0/setup.cfg
+-rw-rw-r--   0 summy      (501) staff       (20)     1168 2024-05-11 00:27:43.000000 sqlexecutorx-1.0.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-11 00:29:55.722515 sqlexecutorx-1.0.0/sqlexecutorx/
+-rw-rw-r--   0 summy      (501) staff       (20)     1373 2024-05-05 01:28:17.000000 sqlexecutorx-1.0.0/sqlexecutorx/__init__.py
+-rw-rw-r--   0 summy      (501) staff       (20)      209 2024-05-04 03:22:15.000000 sqlexecutorx-1.0.0/sqlexecutorx/constant.py
+-rw-rw-r--   0 summy      (501) staff       (20)    11421 2024-05-11 00:25:41.000000 sqlexecutorx-1.0.0/sqlexecutorx/core.py
+-rw-r--r--   0 summy      (501) staff       (20)      901 2024-03-23 15:57:10.000000 sqlexecutorx-1.0.0/sqlexecutorx/engine.py
+-rw-rw-r--   0 summy      (501) staff       (20)     2063 2024-05-05 02:01:30.000000 sqlexecutorx-1.0.0/sqlexecutorx/init_import.py
+-rw-rw-r--   0 summy      (501) staff       (20)      739 2024-05-06 02:41:09.000000 sqlexecutorx-1.0.0/sqlexecutorx/log_support.py
+-rw-rw-r--   0 summy      (501) staff       (20)     1031 2024-05-04 03:22:15.000000 sqlexecutorx-1.0.0/sqlexecutorx/pooling.py
+-rw-r--r--   0 summy      (501) staff       (20)      422 2024-03-29 05:50:43.000000 sqlexecutorx-1.0.0/sqlexecutorx/sql_support.py
+-rw-rw-r--   0 summy      (501) staff       (20)     3892 2024-03-25 02:25:33.000000 sqlexecutorx-1.0.0/sqlexecutorx/support.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-11 00:29:55.730689 sqlexecutorx-1.0.0/sqlexecutorx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     2027 2024-05-11 00:29:55.000000 sqlexecutorx-1.0.0/sqlexecutorx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      432 2024-05-11 00:29:55.000000 sqlexecutorx-1.0.0/sqlexecutorx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-11 00:29:55.000000 sqlexecutorx-1.0.0/sqlexecutorx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-11 00:29:55.000000 sqlexecutorx-1.0.0/sqlexecutorx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-11 00:29:55.000000 sqlexecutorx-1.0.0/sqlexecutorx.egg-info/top_level.txt
```

### Comparing `sqlexecutorx-0.9.0/LICENSE` & `sqlexecutorx-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.9.0/PKG-INFO` & `sqlexecutorx-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlexecutorx
-Version: 0.9.0
+Version: 1.0.0
 Summary: A simple thread safe sql executor for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecutorx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
```

### Comparing `sqlexecutorx-0.9.0/README.rst` & `sqlexecutorx-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.9.0/setup.py` & `sqlexecutorx-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 setup(
     name='sqlexecutorx',
     packages=['sqlexecutorx'],
     description="A simple thread safe sql executor for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.0',
+    version='1.0.0',
     url='https://gitee.com/summry/sqlexecutorx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Database', 'Python', 'RDB'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlexecutorx-0.9.0/sqlexecutorx/__init__.py` & `sqlexecutorx-1.0.0/sqlexecutorx/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.9.0/sqlexecutorx/core.py` & `sqlexecutorx-1.0.0/sqlexecutorx/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # !/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 import functools
+from typing import List, Tuple
 from .log_support import logger
 from .engine import Engine, Driver
 from .init_import import import_driver
 from .sql_support import limit_one_sql
 from .log_support import do_sql_log, do_save_log
 from .constant import PARAM_DRIVER, PARAM_DEBUG, PARAM_POOL_SIZE, MODULE, PARAM_SHOW_SQL
 from .support import DBCtx, ConnectionCtx, TransactionCtx, try_commit, DBError, DB_LOCK, Dict, MultiColumnsError
@@ -169,15 +170,15 @@
 
     if _DB_CTX is not None:
         _DB_CTX.release()
         _DB_CTX = None
 
 
 @with_connection
-def execute(sql: str, *args):
+def execute(sql: str, *args) -> int:
     """
     Execute sql return effect rowcount
 
     :param sql: SQL
     :param args:
     :return: Effect rowcount
 
@@ -259,39 +260,39 @@
             return result[0]
         msg = "Exec func 'sqlexecutorx.%s' expect only one column but %d." % ('do_get', len(result))
         logger.error('%s  \n\t sql: %s \n\t args: %s' % (msg, sql, args))
         raise MultiColumnsError(msg)
     return None
 
 
-def select(sql: str, *args):
+def select(sql: str, *args) -> List[Tuple]:
     """
     Examples
     --------
     >>> import sqlexecutorx as db
     >>> sql = 'SELECT id, name, age FROM person WHERE name=%s and age=%s'
     >>> db.select(sql, '张三', 20)
     [(3, '张三', 20)]
     """
     return do_select(sql, *args)[0]
 
 
-def select_one(sql: str, *args):
+def select_one(sql: str, *args) -> Tuple:
     """
     Examples
     --------
     >>> import sqlexecutorx as db
     >>> sql = 'SELECT id, name, age FROM person WHERE name=%s and age=%s LIMIT 1'
     >>> db.select_one(sql, '张三', 20)
     (3, '张三', 20)
     """
     return do_select_one(sql, *args)[0]
 
 
-def query(sql: str, *args):
+def query(sql: str, *args) -> List[dict]:
     """
     Execute select SQL and return list results(dict).
 
     Examples
     --------
     >>> import sqlexecutorx as db
     >>> sql = 'SELECT id, name, age FROM person WHERE name=%s and age=%s'
@@ -301,15 +302,15 @@
     results, description = do_select(sql, *args)
     if results and description:
         names = list(map(lambda x: x[0], description))
         return list(map(lambda x: Dict(names, x), results))
     return results
 
 
-def query_one(sql: str, *args):
+def query_one(sql: str, *args) -> dict:
     """
     Execute select SQL and return unique result(dict), SQL contain 'limit'.
 
     Examples
     --------
     >>> import sqlexecutorx as db
     >>> sql = 'SELECT id, name, age FROM person WHERE name=%s and age=%s LIMIT 1'
@@ -321,15 +322,15 @@
     if result and description:
         names = list(map(lambda x: x[0], description))
         return Dict(names, result)
     return result
 
 
 @with_connection
-def do_select(sql: str, *args):
+def do_select(sql: str, *args) -> Tuple[List, Tuple]:
     """
     Execute select SQL and return results and description
 
     Examples
     --------
     >>> import sqlexecutorx as db
     >>> sql = 'SELECT id, name, age FROM person WHERE name=%s and age=%s limit 1'
@@ -350,15 +351,15 @@
         return cursor.fetchall(), cursor.description
     finally:
         if cursor:
             cursor.close()
 
 
 @with_connection
-def do_select_one(sql: str, *args):
+def do_select_one(sql: str, *args) -> Tuple[Tuple, Tuple]:
     """
     Execute select SQL and return result and description
 
     Examples
     --------
     >>> import sqlexecutorx as db
     >>> sql = 'SELECT id, name, age FROM person WHERE name=%s and age=%s limit 1'
@@ -381,15 +382,15 @@
         return cursor.fetchone(), cursor.description
     finally:
         if cursor:
             cursor.close()
 
 
 @with_connection
-def batch_execute(sql: str, *args):
+def batch_execute(sql: str, *args) -> int:
     """
     Batch execute sql return effected rowcount
 
     :param sql: SQL to execute
     :param args: All number must have same size.
     :return: Effect rowcount
```

### Comparing `sqlexecutorx-0.9.0/sqlexecutorx/engine.py` & `sqlexecutorx-1.0.0/sqlexecutorx/engine.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.9.0/sqlexecutorx/init_import.py` & `sqlexecutorx-1.0.0/sqlexecutorx/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.9.0/sqlexecutorx/log_support.py` & `sqlexecutorx-1.0.0/sqlexecutorx/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.9.0/sqlexecutorx/pooling.py` & `sqlexecutorx-1.0.0/sqlexecutorx/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.9.0/sqlexecutorx/support.py` & `sqlexecutorx-1.0.0/sqlexecutorx/support.py`

 * *Files identical despite different names*

### Comparing `sqlexecutorx-0.9.0/sqlexecutorx.egg-info/PKG-INFO` & `sqlexecutorx-1.0.0/sqlexecutorx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlexecutorx
-Version: 0.9.0
+Version: 1.0.0
 Summary: A simple thread safe sql executor for Python with connection pool. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlexecutorx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Database,Python,RDB
 Platform: UNKNOWN
```

