# Comparing `tmp/unitradeapi-0.121.tar.gz` & `tmp/unitradeapi-0.122.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitradeapi-0.121.tar", last modified: Sat May 11 12:20:56 2024, max compression
+gzip compressed data, was "unitradeapi-0.122.tar", last modified: Sat May 11 12:43:43 2024, max compression
```

## Comparing `unitradeapi-0.121.tar` & `unitradeapi-0.122.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-11 12:20:56.866320 unitradeapi-0.121/
--rw-r--r--   0 andrey     (501) staff       (20)     1061 2024-01-30 06:02:09.000000 unitradeapi-0.121/LICENSE.md
--rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-05-11 12:20:56.866022 unitradeapi-0.121/PKG-INFO
--rw-r--r--   0 andrey     (501) staff       (20)     1721 2024-02-28 11:26:00.000000 unitradeapi-0.121/README.md
--rw-r--r--   0 andrey     (501) staff       (20)       38 2024-05-11 12:20:56.866366 unitradeapi-0.121/setup.cfg
--rw-r--r--   0 andrey     (501) staff       (20)      706 2024-05-11 06:58:32.000000 unitradeapi-0.121/setup.py
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-11 12:20:56.864866 unitradeapi-0.121/unitradeapi/
--rw-r--r--   0 andrey     (501) staff       (20)      265 2024-01-22 09:41:08.000000 unitradeapi-0.121/unitradeapi/__init__.py
--rw-r--r--   0 andrey     (501) staff       (20)    22252 2024-01-08 11:14:26.000000 unitradeapi-0.121/unitradeapi/binance.py
--rw-r--r--   0 andrey     (501) staff       (20)    16339 2024-05-11 12:07:20.000000 unitradeapi-0.121/unitradeapi/bybit.py
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-11 12:20:56.865805 unitradeapi-0.121/unitradeapi.egg-info/
--rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-05-11 12:20:56.000000 unitradeapi-0.121/unitradeapi.egg-info/PKG-INFO
--rw-r--r--   0 andrey     (501) staff       (20)      271 2024-05-11 12:20:56.000000 unitradeapi-0.121/unitradeapi.egg-info/SOURCES.txt
--rw-r--r--   0 andrey     (501) staff       (20)        1 2024-05-11 12:20:56.000000 unitradeapi-0.121/unitradeapi.egg-info/dependency_links.txt
--rw-r--r--   0 andrey     (501) staff       (20)       36 2024-05-11 12:20:56.000000 unitradeapi-0.121/unitradeapi.egg-info/requires.txt
--rw-r--r--   0 andrey     (501) staff       (20)       12 2024-05-11 12:20:56.000000 unitradeapi-0.121/unitradeapi.egg-info/top_level.txt
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-11 12:43:43.231727 unitradeapi-0.122/
+-rw-r--r--   0 andrey     (501) staff       (20)     1061 2024-01-30 06:02:09.000000 unitradeapi-0.122/LICENSE.md
+-rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-05-11 12:43:43.231490 unitradeapi-0.122/PKG-INFO
+-rw-r--r--   0 andrey     (501) staff       (20)     1721 2024-02-28 11:26:00.000000 unitradeapi-0.122/README.md
+-rw-r--r--   0 andrey     (501) staff       (20)       38 2024-05-11 12:43:43.231769 unitradeapi-0.122/setup.cfg
+-rw-r--r--   0 andrey     (501) staff       (20)      706 2024-05-11 12:43:28.000000 unitradeapi-0.122/setup.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-11 12:43:43.230137 unitradeapi-0.122/unitradeapi/
+-rw-r--r--   0 andrey     (501) staff       (20)      265 2024-01-22 09:41:08.000000 unitradeapi-0.122/unitradeapi/__init__.py
+-rw-r--r--   0 andrey     (501) staff       (20)    22252 2024-01-08 11:14:26.000000 unitradeapi-0.122/unitradeapi/binance.py
+-rw-r--r--   0 andrey     (501) staff       (20)    16341 2024-05-11 12:43:28.000000 unitradeapi-0.122/unitradeapi/bybit.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-11 12:43:43.231173 unitradeapi-0.122/unitradeapi.egg-info/
+-rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-05-11 12:43:43.000000 unitradeapi-0.122/unitradeapi.egg-info/PKG-INFO
+-rw-r--r--   0 andrey     (501) staff       (20)      271 2024-05-11 12:43:43.000000 unitradeapi-0.122/unitradeapi.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey     (501) staff       (20)        1 2024-05-11 12:43:43.000000 unitradeapi-0.122/unitradeapi.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey     (501) staff       (20)       36 2024-05-11 12:43:43.000000 unitradeapi-0.122/unitradeapi.egg-info/requires.txt
+-rw-r--r--   0 andrey     (501) staff       (20)       12 2024-05-11 12:43:43.000000 unitradeapi-0.122/unitradeapi.egg-info/top_level.txt
```

### Comparing `unitradeapi-0.121/LICENSE.md` & `unitradeapi-0.122/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitradeapi-0.121/PKG-INFO` & `unitradeapi-0.122/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitradeapi
-Version: 0.121
+Version: 0.122
 Summary: Binance, Bybit API
 Home-page: https://github.com/plv88/UniCryptTradeAPI
 Author: plv88
 Author-email: plv.andrey88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `unitradeapi-0.121/README.md` & `unitradeapi-0.122/README.md`

 * *Files identical despite different names*

### Comparing `unitradeapi-0.121/setup.py` & `unitradeapi-0.122/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='unitradeapi',
-    version='0.121',
+    version='0.122',
     packages=find_packages(),
     description='Binance, Bybit API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='plv88',
     author_email='plv.andrey88@gmail.com',
     url='https://github.com/plv88/UniCryptTradeAPI',
```

### Comparing `unitradeapi-0.121/unitradeapi/binance.py` & `unitradeapi-0.122/unitradeapi/binance.py`

 * *Files identical despite different names*

### Comparing `unitradeapi-0.121/unitradeapi/bybit.py` & `unitradeapi-0.122/unitradeapi/bybit.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,15 +373,15 @@
         # mes_to_log = f'{def_name} Error: {error}, traceback: {traceback.format_exc()}'
         self._logger.error(mes_to_log)
         print(mes_to_log)
         if self.count_reconnect <= 3:
             self.count_reconnect += 1
             self.reconnect()
         else:
-            self.queue.put('exit')
+            # self.queue.put('exit')
             exit()
 
     def reconnect(self):
         if self._is_running:
             mes_to_log = f'SyncBybitWebsocketPublic Reconnect {self.count_reconnect}'
             self._logger.warning(mes_to_log)
             print(mes_to_log)
```

### Comparing `unitradeapi-0.121/unitradeapi.egg-info/PKG-INFO` & `unitradeapi-0.122/unitradeapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitradeapi
-Version: 0.121
+Version: 0.122
 Summary: Binance, Bybit API
 Home-page: https://github.com/plv88/UniCryptTradeAPI
 Author: plv88
 Author-email: plv.andrey88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

