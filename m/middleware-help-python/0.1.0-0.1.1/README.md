# Comparing `tmp/middleware-help-python-0.1.0.tar.gz` & `tmp/middleware-help-python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middleware-help-python-0.1.0.tar", last modified: Fri May 10 10:48:42 2024, max compression
+gzip compressed data, was "middleware-help-python-0.1.1.tar", last modified: Fri May 10 11:12:20 2024, max compression
```

## Comparing `middleware-help-python-0.1.0.tar` & `middleware-help-python-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 10:48:42.517958 middleware-help-python-0.1.0/
--rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      543 2024-05-10 10:48:42.515963 middleware-help-python-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 10:48:42.514965 middleware-help-python-0.1.0/middleware_help_python.egg-info/
--rw-rw-rw-   0        0        0      543 2024-05-10 10:48:42.000000 middleware-help-python-0.1.0/middleware_help_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-05-10 10:48:42.000000 middleware-help-python-0.1.0/middleware_help_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 10:48:42.000000 middleware-help-python-0.1.0/middleware_help_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-10 10:48:42.000000 middleware-help-python-0.1.0/middleware_help_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-10 10:48:42.000000 middleware-help-python-0.1.0/middleware_help_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-10 10:48:42.512971 middleware-help-python-0.1.0/middleware_helper/
--rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.1.0/middleware_helper/__init__.py
--rw-rw-rw-   0        0        0      530 2024-05-10 10:22:25.000000 middleware-help-python-0.1.0/middleware_helper/libs.py
--rw-rw-rw-   0        0        0     5097 2024-05-10 10:48:28.000000 middleware-help-python-0.1.0/middleware_helper/mysql.py
--rw-rw-rw-   0        0        0     2155 2024-04-29 08:20:12.000000 middleware-help-python-0.1.0/middleware_helper/network.py
--rw-rw-rw-   0        0        0     1267 2024-04-29 08:21:12.000000 middleware-help-python-0.1.0/middleware_helper/redis.py
--rw-rw-rw-   0        0        0       42 2024-05-10 10:48:42.517958 middleware-help-python-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1162 2024-05-10 10:48:38.000000 middleware-help-python-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 11:12:20.678452 middleware-help-python-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      543 2024-05-10 11:12:20.676458 middleware-help-python-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 11:12:20.674463 middleware-help-python-0.1.1/middleware_help_python.egg-info/
+-rw-rw-rw-   0        0        0      543 2024-05-10 11:12:20.000000 middleware-help-python-0.1.1/middleware_help_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-05-10 11:12:20.000000 middleware-help-python-0.1.1/middleware_help_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 11:12:20.000000 middleware-help-python-0.1.1/middleware_help_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-10 11:12:20.000000 middleware-help-python-0.1.1/middleware_help_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 11:12:20.000000 middleware-help-python-0.1.1/middleware_help_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 11:12:20.671470 middleware-help-python-0.1.1/middleware_helper/
+-rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.1.1/middleware_helper/__init__.py
+-rw-rw-rw-   0        0        0      530 2024-05-10 10:22:25.000000 middleware-help-python-0.1.1/middleware_helper/libs.py
+-rw-rw-rw-   0        0        0     5180 2024-05-10 11:12:04.000000 middleware-help-python-0.1.1/middleware_helper/mysql.py
+-rw-rw-rw-   0        0        0     2155 2024-04-29 08:20:12.000000 middleware-help-python-0.1.1/middleware_helper/network.py
+-rw-rw-rw-   0        0        0     1267 2024-04-29 08:21:12.000000 middleware-help-python-0.1.1/middleware_helper/redis.py
+-rw-rw-rw-   0        0        0       42 2024-05-10 11:12:20.678452 middleware-help-python-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2024-05-10 11:12:16.000000 middleware-help-python-0.1.1/setup.py
```

### Comparing `middleware-help-python-0.1.0/LICENSE` & `middleware-help-python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.1.0/PKG-INFO` & `middleware-help-python-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.1.0/middleware_help_python.egg-info/PKG-INFO` & `middleware-help-python-0.1.1/middleware_help_python.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.1.0/middleware_helper/libs.py` & `middleware-help-python-0.1.1/middleware_helper/libs.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.1.0/middleware_helper/mysql.py` & `middleware-help-python-0.1.1/middleware_helper/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         # 获取查询结果
         records = cursor.fetchall()
         # 获取列名
         column_names = cursor.column_names
         result_list = cls.convert_tuple_to_dict(records=records, column_names=column_names)
         return result_list
 
-    def execute_sql(self, sql: str, action: str):
+    def execute_sql(self, sql: str, action: str, is_need_close: bool = True) -> list:
         results = None
         if self.conn and self.conn.is_connected():
             cursor: CMySQLCursor = self.conn.cursor()
             if action in ("insert", "update", "delete"):
                 try:
                     cursor.execute(sql)
                     self.conn.commit()
@@ -100,16 +100,17 @@
                 try:
                     # 获取查询结果
                     results = self.cursor_query_data(sql=sql, cursor=cursor)
                 except Exception as e:
                     logger.error(e)
             else:
                 pass
-            cursor.close()
-            self.conn.close()
+            if is_need_close is True:
+                cursor.close()
+                self.conn.close()
         else:
             logger.error("当前连接不正常.")
         return results
 
     @classmethod
     def convert_key_value_str(cls, **kwargs) -> tuple:
         field_list, value_list = list(), list()
```

### Comparing `middleware-help-python-0.1.0/middleware_helper/network.py` & `middleware-help-python-0.1.1/middleware_helper/network.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.1.0/middleware_helper/redis.py` & `middleware-help-python-0.1.1/middleware_helper/redis.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.1.0/setup.py` & `middleware-help-python-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='middleware-help-python',
-    version='0.1.0',
+    version='0.1.1',
     description='This is my middleware help package',
     long_description='This is my middleware help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/middleware-help-python',
     packages=find_packages(),
     install_requires=[
```

