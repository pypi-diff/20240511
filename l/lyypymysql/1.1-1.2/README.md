# Comparing `tmp/lyypymysql-1.1.tar.gz` & `tmp/lyypymysql-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyypymysql-1.1.tar", last modified: Tue May  7 14:58:31 2024, max compression
+gzip compressed data, was "lyypymysql-1.2.tar", last modified: Sat May 11 03:50:36 2024, max compression
```

## Comparing `lyypymysql-1.1.tar` & `lyypymysql-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 14:58:31.041156 lyypymysql-1.1/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyypymysql-1.1/LICENSE
--rw-rw-rw-   0        0        0      147 2024-05-07 14:58:31.040153 lyypymysql-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyypymysql-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 14:58:31.038828 lyypymysql-1.1/lyypymysql.egg-info/
--rw-rw-rw-   0        0        0      147 2024-05-07 14:58:30.000000 lyypymysql-1.1/lyypymysql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-05-07 14:58:30.000000 lyypymysql-1.1/lyypymysql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 14:58:30.000000 lyypymysql-1.1/lyypymysql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-07 14:58:30.000000 lyypymysql-1.1/lyypymysql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7281 2024-05-07 14:58:23.000000 lyypymysql-1.1/lyypymysql.py
--rw-rw-rw-   0        0        0       42 2024-05-07 14:58:31.041156 lyypymysql-1.1/setup.cfg
--rw-rw-rw-   0        0        0      250 2024-05-07 14:58:29.000000 lyypymysql-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:50:36.945586 lyypymysql-1.2/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyypymysql-1.2/LICENSE
+-rw-rw-rw-   0        0        0      147 2024-05-11 03:50:36.944576 lyypymysql-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyypymysql-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 03:50:36.943558 lyypymysql-1.2/lyypymysql.egg-info/
+-rw-rw-rw-   0        0        0      147 2024-05-11 03:50:36.000000 lyypymysql-1.2/lyypymysql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2024-05-11 03:50:36.000000 lyypymysql-1.2/lyypymysql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 03:50:36.000000 lyypymysql-1.2/lyypymysql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-11 03:50:36.000000 lyypymysql-1.2/lyypymysql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9032 2024-05-11 03:44:07.000000 lyypymysql-1.2/lyypymysql.py
+-rw-rw-rw-   0        0        0       42 2024-05-11 03:50:36.945586 lyypymysql-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      250 2024-05-11 03:50:35.000000 lyypymysql-1.2/setup.py
```

### Comparing `lyypymysql-1.1/LICENSE` & `lyypymysql-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lyypymysql-1.1/lyypymysql.py` & `lyypymysql-1.2/lyypymysql.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,56 @@
 import pymysql
-import pandas as pd
 import sys
 
 lastid = 0
 
+import mysql.connector
+
+class _mysqlid():
+    def __init__(self):
+        self.username="cy"
+        self.server="rm-7xvcw05tn97onu88s7o.mysql.rds.aliyuncs.com:3306"
+        self.db = "fpdb"
+        self.full_engine_text=f'mysql+pymysql://{self.username}:{self.password}@{self.server}/{self.db}?charset=utf8'
+        
+
+class mysql_class():
+    def __init__(self,password):
+        
+        self.username,self.password, self.db,self.server = "cy",password, "fpdb","rm-7xvcw05tn97onu88s7o.mysql.rds.aliyuncs.com:3306"
+        self.conn = mysql.connector.connect(user=self.username, password=password,host=self.server, database=self.db)
+        self.cursor = self.conn.cursor()
+
+        # thread_conn = threading.Thread(target=self.get_engine_conn,daemon=True)
+        # thread_conn.start()
+    def get_connector(self,before_notice="",after_notice=""):
+        if not hasattr(self,"conn") or not hasattr(self,"cursor")  or self.conn is None or not self.conn.is_connected():
+            try:
+                print(before_notice)
+                self.conn = mysql.connector.connect(user=self.username, password=self.password,host=self.server, database=self.db)
+                self.cursor = self.conn.cursor()
+                print(after_notice)
+            except mysql.connector.Error as err:
+                print(f"连接失败: {err}")
+                return None, None
+        else:
+            print("mysql.connector已经连接")
+            
+    def execute_query(self, query):
+        self.conn.ping(reconnect=True)
+        cursor = self.conn.cursor()
+        cursor.execute(query)
+        result = cursor.fetchall()
+        cursor.close()
+        return result
+
+    def close_connection(self):
+        self.conn.close()
+
+
 class lyymysql_class():
 
     def __init__(self, conn):
         self.conn = conn
 
     def create_mysql_table(self, conn, table_name, debug=False):
         sqlquery = "CREATE TABLE if not exists `" + table_name + "` (`id` INT NOT NULL AUTO_INCREMENT,\
```

