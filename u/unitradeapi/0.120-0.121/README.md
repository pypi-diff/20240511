# Comparing `tmp/unitradeapi-0.120.tar.gz` & `tmp/unitradeapi-0.121.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitradeapi-0.120.tar", last modified: Tue Apr 23 12:41:31 2024, max compression
+gzip compressed data, was "unitradeapi-0.121.tar", last modified: Sat May 11 12:20:56 2024, max compression
```

## Comparing `unitradeapi-0.120.tar` & `unitradeapi-0.121.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-04-23 12:41:31.833402 unitradeapi-0.120/
--rw-r--r--   0 andrey     (501) staff       (20)     1061 2024-01-30 06:02:09.000000 unitradeapi-0.120/LICENSE.md
--rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-04-23 12:41:31.832971 unitradeapi-0.120/PKG-INFO
--rw-r--r--   0 andrey     (501) staff       (20)     1721 2024-02-28 11:26:00.000000 unitradeapi-0.120/README.md
--rw-r--r--   0 andrey     (501) staff       (20)       38 2024-04-23 12:41:31.833467 unitradeapi-0.120/setup.cfg
--rw-r--r--   0 andrey     (501) staff       (20)      706 2024-04-23 12:41:18.000000 unitradeapi-0.120/setup.py
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-04-23 12:41:31.831417 unitradeapi-0.120/unitradeapi/
--rw-r--r--   0 andrey     (501) staff       (20)      265 2024-01-22 09:41:08.000000 unitradeapi-0.120/unitradeapi/__init__.py
--rw-r--r--   0 andrey     (501) staff       (20)    22252 2024-01-08 11:14:26.000000 unitradeapi-0.120/unitradeapi/binance.py
--rw-r--r--   0 andrey     (501) staff       (20)    15405 2024-04-23 12:36:18.000000 unitradeapi-0.120/unitradeapi/bybit.py
-drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-04-23 12:41:31.832523 unitradeapi-0.120/unitradeapi.egg-info/
--rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-04-23 12:41:31.000000 unitradeapi-0.120/unitradeapi.egg-info/PKG-INFO
--rw-r--r--   0 andrey     (501) staff       (20)      271 2024-04-23 12:41:31.000000 unitradeapi-0.120/unitradeapi.egg-info/SOURCES.txt
--rw-r--r--   0 andrey     (501) staff       (20)        1 2024-04-23 12:41:31.000000 unitradeapi-0.120/unitradeapi.egg-info/dependency_links.txt
--rw-r--r--   0 andrey     (501) staff       (20)       36 2024-04-23 12:41:31.000000 unitradeapi-0.120/unitradeapi.egg-info/requires.txt
--rw-r--r--   0 andrey     (501) staff       (20)       12 2024-04-23 12:41:31.000000 unitradeapi-0.120/unitradeapi.egg-info/top_level.txt
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-11 12:20:56.866320 unitradeapi-0.121/
+-rw-r--r--   0 andrey     (501) staff       (20)     1061 2024-01-30 06:02:09.000000 unitradeapi-0.121/LICENSE.md
+-rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-05-11 12:20:56.866022 unitradeapi-0.121/PKG-INFO
+-rw-r--r--   0 andrey     (501) staff       (20)     1721 2024-02-28 11:26:00.000000 unitradeapi-0.121/README.md
+-rw-r--r--   0 andrey     (501) staff       (20)       38 2024-05-11 12:20:56.866366 unitradeapi-0.121/setup.cfg
+-rw-r--r--   0 andrey     (501) staff       (20)      706 2024-05-11 06:58:32.000000 unitradeapi-0.121/setup.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-11 12:20:56.864866 unitradeapi-0.121/unitradeapi/
+-rw-r--r--   0 andrey     (501) staff       (20)      265 2024-01-22 09:41:08.000000 unitradeapi-0.121/unitradeapi/__init__.py
+-rw-r--r--   0 andrey     (501) staff       (20)    22252 2024-01-08 11:14:26.000000 unitradeapi-0.121/unitradeapi/binance.py
+-rw-r--r--   0 andrey     (501) staff       (20)    16339 2024-05-11 12:07:20.000000 unitradeapi-0.121/unitradeapi/bybit.py
+drwxr-xr-x   0 andrey     (501) staff       (20)        0 2024-05-11 12:20:56.865805 unitradeapi-0.121/unitradeapi.egg-info/
+-rw-r--r--   0 andrey     (501) staff       (20)     2174 2024-05-11 12:20:56.000000 unitradeapi-0.121/unitradeapi.egg-info/PKG-INFO
+-rw-r--r--   0 andrey     (501) staff       (20)      271 2024-05-11 12:20:56.000000 unitradeapi-0.121/unitradeapi.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey     (501) staff       (20)        1 2024-05-11 12:20:56.000000 unitradeapi-0.121/unitradeapi.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey     (501) staff       (20)       36 2024-05-11 12:20:56.000000 unitradeapi-0.121/unitradeapi.egg-info/requires.txt
+-rw-r--r--   0 andrey     (501) staff       (20)       12 2024-05-11 12:20:56.000000 unitradeapi-0.121/unitradeapi.egg-info/top_level.txt
```

### Comparing `unitradeapi-0.120/LICENSE.md` & `unitradeapi-0.121/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitradeapi-0.120/PKG-INFO` & `unitradeapi-0.121/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitradeapi
-Version: 0.120
+Version: 0.121
 Summary: Binance, Bybit API
 Home-page: https://github.com/plv88/UniCryptTradeAPI
 Author: plv88
 Author-email: plv.andrey88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `unitradeapi-0.120/README.md` & `unitradeapi-0.121/README.md`

 * *Files identical despite different names*

### Comparing `unitradeapi-0.120/setup.py` & `unitradeapi-0.121/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='unitradeapi',
-    version='0.120',
+    version='0.121',
     packages=find_packages(),
     description='Binance, Bybit API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='plv88',
     author_email='plv.andrey88@gmail.com',
     url='https://github.com/plv88/UniCryptTradeAPI',
```

### Comparing `unitradeapi-0.120/unitradeapi/binance.py` & `unitradeapi-0.121/unitradeapi/binance.py`

 * *Files identical despite different names*

### Comparing `unitradeapi-0.120/unitradeapi/bybit.py` & `unitradeapi-0.121/unitradeapi/bybit.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 # import _thread
 import threading
 import hmac
 import hashlib
 import aiohttp
 
 
-
-
 class GeneralBybit:
     _main_url = r'https://api.bybit.com'
 
     def _syns_request_template(self, end_point, par=None, method='get'):
         def_name = sys._getframe().f_code.co_name
         match method.lower():
             case 'get':
@@ -75,15 +73,14 @@
         end_point = '/v5/market/instruments-info'
         params = {
             'category': self.category,
             'status': 'Trading'
         }
         return self._syns_request_template(end_point=end_point, method='get', par=params)
 
-
     def get_symbols_in_trading(self):
         result = self.get_instruments_info().get('result')
         if result:
             return [el.get('symbol') for el in result.get('list') if el.get('status') == 'Trading']
         return None
 
     def get_ticker(self, symbol):
@@ -209,16 +206,14 @@
             params['startTime'] = start_time
         if end_time:
             params['endTime'] = end_time
         params['sign'] = self.__create_signature(params)
         return self._syns_request_template(end_point=end_point, method='get', par=params)
 
 
-
-
 class AsyncBybitPrivate(GeneralBybit):
     def __init__(self, category, api_key, api_secret):
         self._logger = Logger('AsyncBybitPrivate', type_log='w').logger
         self.category = category
         self.api_key = api_key
         self.api_secret = api_secret
 
@@ -296,15 +291,15 @@
             # Обновляем курсор для следующего запроса
             cursor = response.get('nextPageCursor')
             if not cursor:
                 break  # Выход из цикла, если больше нет страниц для загрузки
         return all_logs
 
 
-#Websockets
+# Websockets
 class SyncBybitWebsocketPublic:
     _dict_urls = {
         'spot': 'wss://stream.bybit.com/v5/public/spot',
         'der': 'wss://stream.bybit.com/v5/public/linear',
         'der_auth': 'wss://stream.bybit.com/v5/private',
         'spot_auth': 'wss://stream.bybit.com/v5/private'
     }
@@ -312,22 +307,33 @@
     def __init__(self, trade_type, queue, topics):
         if trade_type not in self._dict_urls:
             raise ValueError(f"trade_type '{trade_type}' is not valid.")
         self.trade_type = trade_type
         self._logger = Logger('SyncBybitWebsocketPublic', type_log='w').logger
         self.queue = queue
         self.topics = topics
+        self.websocket_app = None
+        self.heartbeat_thread = None
+        self._is_running = None
+        self.reconnect_delay = 20  # Задержка перед повторным подключением
+        self.count_reconnect = 0
+
+        self.connect()
+
+    def connect(self):
+        self._is_running = True
+        print('connect')
         self.websocket_app = websocket.WebSocketApp(
-            url=self._dict_urls.get(trade_type),
+            url=self._dict_urls.get(self.trade_type),
             on_message=self.on_message,
             on_close=self.on_close,
             on_error=self.on_error,
             on_open=self.on_open,
         )
-        self._is_running = True
+        self.websocket_app.run_forever()
 
     def __del__(self):
         self.stop()
 
     def send_heartbeat(self, _wsapp):
         while self._is_running:  # Проверьте, что соединение должно быть открыто
             try:
@@ -343,39 +349,60 @@
                 msg = "WebSocket connection is closed, stopping heartbeat."
                 self._logger.warning(msg)
                 print(msg)
                 break
 
     def on_open(self, _wsapp):
         print("Connection opened")
-        heartbeat_thread = threading.Thread(target=self.send_heartbeat, args=(_wsapp,))
-        heartbeat_thread.start()
+        self.heartbeat_thread = threading.Thread(target=self.send_heartbeat, args=(_wsapp,))
+        self.heartbeat_thread.daemon = True
+        self.heartbeat_thread.start()
         data = {
             "op": "subscribe",
             "args": self.topics
         }
         _wsapp.send(json.dumps(data))
 
     @staticmethod
     def on_close(_wsapp, close_status_code, close_msg):
         if close_status_code is not None and close_msg is not None:
             print(f"Close connection by server, status {close_status_code}, close message {close_msg}")
 
     def on_error(self, _wsapp, error):
         def_name = sys._getframe().f_code.co_name
-        mes_to_log = f'{def_name} Error: {error}, traceback: {traceback.format_exc()}'
+        mes_to_log = f'{def_name} Error: {error}'
+        # mes_to_log = f'{def_name} Error: {error}, traceback: {traceback.format_exc()}'
         self._logger.error(mes_to_log)
         print(mes_to_log)
-        raise TypeError(mes_to_log)
+        if self.count_reconnect <= 3:
+            self.count_reconnect += 1
+            self.reconnect()
+        else:
+            self.queue.put('exit')
+            exit()
+
+    def reconnect(self):
+        if self._is_running:
+            mes_to_log = f'SyncBybitWebsocketPublic Reconnect {self.count_reconnect}'
+            self._logger.warning(mes_to_log)
+            print(mes_to_log)
+            time.sleep(self.reconnect_delay)
+            self.stop()
+            self.connect()
+        else:
+            mes_to_log = f'reconnect not self._is_running'
+            self._logger.error(mes_to_log)
+            raise mes_to_log
+
 
     def stop(self):
-        self._is_running = False  # Установите флаг в False, чтобы остановить пинг
+        self._is_running = False
         if self.websocket_app:
             self.websocket_app.close()
-        if hasattr(self, 'heartbeat_thread'):
-            self.heartbeat_thread.join()  # Дождитесь завершения потока пинга
+        if self.heartbeat_thread or hasattr(self, 'heartbeat_thread'):
+            self.heartbeat_thread.join()
 
     def on_message(self, _wsapp, message):
         parsed = json.loads(message)
         parsed['trade_type'] = self.trade_type
-        # print(len(parsed), parsed)
-        self.queue.put(parsed)
+        print(len(parsed), parsed)
+        self.queue.put(parsed)
```

### Comparing `unitradeapi-0.120/unitradeapi.egg-info/PKG-INFO` & `unitradeapi-0.121/unitradeapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitradeapi
-Version: 0.120
+Version: 0.121
 Summary: Binance, Bybit API
 Home-page: https://github.com/plv88/UniCryptTradeAPI
 Author: plv88
 Author-email: plv.andrey88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

