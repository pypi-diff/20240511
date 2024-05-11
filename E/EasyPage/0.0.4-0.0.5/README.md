# Comparing `tmp/EasyPage-0.0.4.tar.gz` & `tmp/EasyPage-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyPage-0.0.4.tar", last modified: Thu Apr 25 09:16:12 2024, max compression
+gzip compressed data, was "EasyPage-0.0.5.tar", last modified: Sat May 11 02:36:28 2024, max compression
```

## Comparing `EasyPage-0.0.4.tar` & `EasyPage-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 09:16:12.835894 EasyPage-0.0.4/
-drwxrwxrwx   0        0        0        0 2024-04-25 09:16:12.595474 EasyPage-0.0.4/EasyPage.egg-info/
--rw-rw-rw-   0        0        0      286 2024-04-25 09:16:12.000000 EasyPage-0.0.4/EasyPage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2024-04-25 09:16:12.000000 EasyPage-0.0.4/EasyPage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 09:16:12.000000 EasyPage-0.0.4/EasyPage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-04-25 09:16:12.000000 EasyPage-0.0.4/EasyPage.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-25 09:16:12.000000 EasyPage-0.0.4/EasyPage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      286 2024-04-25 09:16:12.834925 EasyPage-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-25 09:16:12.676926 EasyPage-0.0.4/easypage/
--rw-rw-rw-   0        0        0       81 2024-04-22 09:13:20.000000 EasyPage-0.0.4/easypage/__init__.py
--rw-rw-rw-   0        0        0     3243 2024-04-22 08:15:25.000000 EasyPage-0.0.4/easypage/cdp.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:16:12.792364 EasyPage-0.0.4/easypage/cdp_method/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.4/easypage/cdp_method/__init__.py
--rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.4/easypage/cdp_method/browser.py
--rw-rw-rw-   0        0        0    12414 2024-04-24 09:08:35.000000 EasyPage-0.0.4/easypage/cdp_method/dom.py
--rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.4/easypage/cdp_method/emulation.py
--rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.4/easypage/cdp_method/fetch.py
--rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.4/easypage/cdp_method/input.py
--rw-rw-rw-   0        0        0     3598 2024-04-24 11:46:26.000000 EasyPage-0.0.4/easypage/cdp_method/network.py
--rw-rw-rw-   0        0        0     5659 2024-04-24 09:12:45.000000 EasyPage-0.0.4/easypage/cdp_method/page.py
--rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.4/easypage/cdp_method/runtime.py
--rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.4/easypage/cdp_method/security.py
--rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.4/easypage/cdp_method/storage.py
--rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.4/easypage/cdp_method/target.py
--rw-rw-rw-   0        0        0    15969 2024-04-25 08:53:50.000000 EasyPage-0.0.4/easypage/conn.py
--rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.4/easypage/definition.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:16:12.812915 EasyPage-0.0.4/easypage/driver/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.4/easypage/driver/__init__.py
--rw-rw-rw-   0        0        0     6188 2024-04-24 14:23:36.000000 EasyPage-0.0.4/easypage/driver/browser.py
--rw-rw-rw-   0        0        0     1587 2024-04-24 02:49:07.000000 EasyPage-0.0.4/easypage/driver/driver.py
--rw-rw-rw-   0        0        0    25744 2024-04-25 09:15:57.000000 EasyPage-0.0.4/easypage/driver/page.py
--rw-rw-rw-   0        0        0     1462 2024-04-24 08:29:43.000000 EasyPage-0.0.4/easypage/errors.py
--rw-rw-rw-   0        0        0     2074 2024-04-22 08:51:10.000000 EasyPage-0.0.4/easypage/logger.py
--rw-rw-rw-   0        0        0     4095 2024-04-25 08:18:53.000000 EasyPage-0.0.4/easypage/main.py
--rw-rw-rw-   0        0        0     4106 2024-04-25 08:20:54.000000 EasyPage-0.0.4/easypage/operate.py
--rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.4/easypage/options.py
--rw-rw-rw-   0        0        0     2787 2024-04-22 08:05:28.000000 EasyPage-0.0.4/easypage/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-25 09:16:12.823887 EasyPage-0.0.4/easypage/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.4/easypage/utils/__init__.py
--rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.4/easypage/utils/browser_utils.py
--rw-rw-rw-   0        0        0     1134 2024-04-24 06:28:10.000000 EasyPage-0.0.4/easypage/utils/other_utils.py
--rw-rw-rw-   0        0        0       42 2024-04-25 09:16:12.835894 EasyPage-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      599 2024-04-25 09:16:07.000000 EasyPage-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:36:28.112760 EasyPage-0.0.5/
+drwxrwxrwx   0        0        0        0 2024-05-11 02:36:27.884188 EasyPage-0.0.5/EasyPage.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-05-11 02:36:27.000000 EasyPage-0.0.5/EasyPage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      980 2024-05-11 02:36:27.000000 EasyPage-0.0.5/EasyPage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 02:36:27.000000 EasyPage-0.0.5/EasyPage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-11 02:36:27.000000 EasyPage-0.0.5/EasyPage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-11 02:36:27.000000 EasyPage-0.0.5/EasyPage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      286 2024-05-11 02:36:28.111759 EasyPage-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 02:36:27.943192 EasyPage-0.0.5/easypage/
+-rw-rw-rw-   0        0        0      177 2024-05-09 12:16:34.000000 EasyPage-0.0.5/easypage/__init__.py
+-rw-rw-rw-   0        0        0     3231 2024-05-07 14:06:28.000000 EasyPage-0.0.5/easypage/cdp.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:36:28.083759 EasyPage-0.0.5/easypage/cdp_method/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.5/easypage/cdp_method/__init__.py
+-rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.5/easypage/cdp_method/browser.py
+-rw-rw-rw-   0        0        0    12414 2024-04-24 09:08:35.000000 EasyPage-0.0.5/easypage/cdp_method/dom.py
+-rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.5/easypage/cdp_method/emulation.py
+-rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.5/easypage/cdp_method/fetch.py
+-rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.5/easypage/cdp_method/input.py
+-rw-rw-rw-   0        0        0     4467 2024-05-07 11:18:55.000000 EasyPage-0.0.5/easypage/cdp_method/network.py
+-rw-rw-rw-   0        0        0     5659 2024-04-24 09:12:45.000000 EasyPage-0.0.5/easypage/cdp_method/page.py
+-rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.5/easypage/cdp_method/runtime.py
+-rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.5/easypage/cdp_method/security.py
+-rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.5/easypage/cdp_method/storage.py
+-rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.5/easypage/cdp_method/target.py
+-rw-rw-rw-   0        0        0    17686 2024-05-10 01:15:20.000000 EasyPage-0.0.5/easypage/conn.py
+-rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.5/easypage/definition.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:36:28.100756 EasyPage-0.0.5/easypage/driver/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.5/easypage/driver/__init__.py
+-rw-rw-rw-   0        0        0     7794 2024-05-11 02:20:43.000000 EasyPage-0.0.5/easypage/driver/browser.py
+-rw-rw-rw-   0        0        0      928 2024-05-09 09:58:08.000000 EasyPage-0.0.5/easypage/driver/driver.py
+-rw-rw-rw-   0        0        0    35291 2024-05-11 02:24:38.000000 EasyPage-0.0.5/easypage/driver/page.py
+-rw-rw-rw-   0        0        0     1462 2024-04-24 08:29:43.000000 EasyPage-0.0.5/easypage/errors.py
+-rw-rw-rw-   0        0        0     5762 2024-05-11 02:30:56.000000 EasyPage-0.0.5/easypage/listener.py
+-rw-rw-rw-   0        0        0     2093 2024-05-09 07:29:23.000000 EasyPage-0.0.5/easypage/logger.py
+-rw-rw-rw-   0        0        0     4581 2024-05-11 02:18:48.000000 EasyPage-0.0.5/easypage/main.py
+-rw-rw-rw-   0        0        0     4106 2024-04-25 08:20:54.000000 EasyPage-0.0.5/easypage/operate.py
+-rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.5/easypage/options.py
+-rw-rw-rw-   0        0        0     1805 2024-05-10 01:35:17.000000 EasyPage-0.0.5/easypage/request.py
+-rw-rw-rw-   0        0        0     4390 2024-05-10 01:15:20.000000 EasyPage-0.0.5/easypage/response.py
+-rw-rw-rw-   0        0        0     2787 2024-04-22 08:05:28.000000 EasyPage-0.0.5/easypage/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-11 02:36:28.109756 EasyPage-0.0.5/easypage/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.5/easypage/utils/__init__.py
+-rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.5/easypage/utils/browser_utils.py
+-rw-rw-rw-   0        0        0     2182 2024-05-09 08:03:26.000000 EasyPage-0.0.5/easypage/utils/other_utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-11 02:36:28.112760 EasyPage-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      599 2024-05-11 02:36:10.000000 EasyPage-0.0.5/setup.py
```

### Comparing `EasyPage-0.0.4/EasyPage.egg-info/SOURCES.txt` & `EasyPage-0.0.5/EasyPage.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 EasyPage.egg-info/requires.txt
 EasyPage.egg-info/top_level.txt
 easypage/__init__.py
 easypage/cdp.py
 easypage/conn.py
 easypage/definition.py
 easypage/errors.py
+easypage/listener.py
 easypage/logger.py
 easypage/main.py
 easypage/operate.py
 easypage/options.py
+easypage/request.py
+easypage/response.py
 easypage/settings.py
 easypage/cdp_method/__init__.py
 easypage/cdp_method/browser.py
 easypage/cdp_method/dom.py
 easypage/cdp_method/emulation.py
 easypage/cdp_method/fetch.py
 easypage/cdp_method/input.py
```

### Comparing `EasyPage-0.0.4/easypage/cdp_method/browser.py` & `EasyPage-0.0.5/easypage/cdp_method/browser.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/cdp_method/dom.py` & `EasyPage-0.0.5/easypage/cdp_method/dom.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/cdp_method/emulation.py` & `EasyPage-0.0.5/easypage/cdp_method/emulation.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/cdp_method/fetch.py` & `EasyPage-0.0.5/easypage/cdp_method/fetch.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/cdp_method/input.py` & `EasyPage-0.0.5/easypage/cdp_method/input.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/cdp_method/network.py` & `EasyPage-0.0.5/easypage/cdp_method/network.py`

 * *Files 11% similar despite different names*

```diff
@@ -109,7 +109,34 @@
             method="Network.setCacheDisabled",
             params={
                 "cacheDisabled": cache_disabled
             },
             raise_err=raise_err,
             need_callback=need_callback,
         )
+
+    def get_response_body(
+            self,
+            request_id: str,
+            raise_err: bool = False,
+            need_callback: bool = True,
+    ) -> Tuple[bool, dict]:
+        """
+        获取响应体
+
+        这个方法会导致卡住，所以不能直接拿到结果
+
+        https://chromedevtools.github.io/devtools-protocol/tot/Network/#method-getResponseBody
+
+        :param request_id:
+        :param raise_err: 接收到错误消息时，是否抛出，默认为 False
+        :param need_callback: 接收到消息时，是否返回，默认为 True
+        :return:
+        """
+        return self.__conn.send(
+            method="Network.getResponseBody",
+            params={
+                "requestId": request_id
+            },
+            raise_err=raise_err,
+            need_callback=need_callback
+        )
```

### Comparing `EasyPage-0.0.4/easypage/cdp_method/page.py` & `EasyPage-0.0.5/easypage/cdp_method/page.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/cdp_method/runtime.py` & `EasyPage-0.0.5/easypage/cdp_method/runtime.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/cdp_method/security.py` & `EasyPage-0.0.5/easypage/cdp_method/security.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/cdp_method/storage.py` & `EasyPage-0.0.5/easypage/cdp_method/storage.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/cdp_method/target.py` & `EasyPage-0.0.5/easypage/cdp_method/target.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/conn.py` & `EasyPage-0.0.5/easypage/conn.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import typing
 import asyncio
 import threading
 import traceback
 import websocket
 import websockets
 from threading import Lock
-from easypage import errors
+from easypage import errors, settings
 from pyee import EventEmitter
 from easypage.logger import logger
 from queue import SimpleQueue, Empty
 from websockets.legacy import client
 
 TYPE_PAGE = "page"
 TYPE_BROWSER = "browser"
@@ -274,31 +274,33 @@
         self.__id += 1
         self.__lock.release()
         return self.__id
 
 
 class Conn(EventEmitter):
 
-    def __init__(self, address: str, driver_type: DRIVER_TYPE, driver_id: str):
+    def __init__(self, address: str, driver_type: DRIVER_TYPE, driver_id: str, timeout: int = None):
         """
         # 页面连接
         ws://127.0.0.1:9223/devtools/page/87B827CF2CAF710C997699F858467545
 
         # 浏览器连接
         ws://127.0.0.1:9223/devtools/browser/0909caac-09eb-4f48-a481-5de5decb3583
 
         :param address: 连接地址，如：127.0.0.1:9223
         :param driver_type: 控制类型，如：TYPE_PAGE
         :param driver_id: 对应 id，如：87B827CF2CAF710C997699F858467545
+        :param timeout: 配置的超时时间
         """
         super().__init__()
         self.address = address
         self.driver_id = driver_id
         self.driver_type = driver_type
         self.driver_url = f"ws://{address}/devtools/{driver_type}/{driver_id}"
+        self.timeout = timeout or settings.TIMEOUT
 
         self.__lock = threading.Lock()
         self.__id: int = 0
         self.__stop: bool = False
         self.__ws: WebSocket = None  # type:ignore
         self.__result_monitor = {}  # 存储结果
         self.__new_conn()
@@ -307,25 +309,25 @@
         """
         与浏览器建立连接
 
         :return:
         """
         self.__ws = websocket.create_connection(
             url=self.driver_url,
-            enable_multithread=True,
+            enable_multithread=False,
             suppress_origin=True
         )
         threading.Thread(target=self.__recv_result, daemon=True).start()
 
     def send(
             self,
             method: str,
             params: dict = None,
             raise_err: bool = False,
-            need_callback: bool = True
+            need_callback: bool = True,
     ) -> typing.Tuple[bool, dict]:
         """
         同步发送消息
 
         使用：status, value = send(method="", raise_err=False, params={})
 
         返回的结果是有两个值：
@@ -334,62 +336,94 @@
 
         :param method:
         :param params:
         :param raise_err: 接收到错误消息时，是否抛出，默认为 False
         :param need_callback: 接收到消息时，是否返回，默认为 True
         :return
         """
+        # 发送消息
+        status, msg = self.__send(
+            method=method,
+            params=params,
+            need_callback=need_callback
+        )
+
+        if not status:
+            return False, dict()
+        elif not need_callback:
+            return True, msg
+
+        # 等待信息接收
+        start_time = time.time()
+        while not self.__stop:
+            if self.closed():
+                break
+
+            try:
+                recv_msg = self.__result_monitor[msg["id"]].get(timeout=0.1)  # 短等待，避免有问题卡着
+                if "result" in recv_msg:
+                    return True, recv_msg["result"]
+                elif "error" in recv_msg:
+                    if raise_err:
+                        raise errors.CDPRecvErrorMsg(recv_msg["error"])
+                    return False, recv_msg["error"]
+
+                logger.error("没有结果：{}", recv_msg)
+            except Empty:
+                if time.time() - start_time >= self.timeout:
+                    self.__remove_result(msg_id=msg["id"])
+                    if raise_err:
+                        raise errors.CDPRecvTimeout(msg)
+                    logger.error("接收超时：{}", msg)
+                    break
+
+    def __send(
+            self,
+            method: str,
+            params: dict = None,
+            need_callback: bool = True,
+    ) -> typing.Tuple[bool, dict]:
+        """
+        同步发送消息
+
+        使用：status, value = send(method="", raise_err=False, params={})
+
+        返回的结果是有两个值：
+            - status 表示当前消息是否有错误发生（raise_err 为 True 时直接抛出）
+            - value 是对应浏览器返回的消息，是一个 dict
+
+        :param method:
+        :param params:
+        :param need_callback: 接收到消息时，是否返回，默认为 True
+        :return
+        """
         # 构建消息
         msg = {
             "id": self.__get_id,
             "method": method,  # 在此示例中启用网络事件
             "params": params
         }
 
-        self.__result_monitor[msg["id"]] = SimpleQueue()
+        if need_callback:
+            self.__result_monitor[msg["id"]] = SimpleQueue()
 
         msg_json = json.dumps(msg)
         logger.debug("[SEND] {}", msg_json)
 
         # 发送信息
         try:
             self.__ws.send(msg_json)
-
-            if not need_callback:
-                return True, dict()
-
-            # 等待信息接收
-            start_time = time.time()
-            while not self.__stop:
-                if self.closed():
-                    break
-
-                try:
-                    recv_msg = self.__result_monitor[msg["id"]].get(timeout=0.1)  # 短等待，避免有问题卡着
-                    if "result" in recv_msg:
-                        return True, recv_msg["result"]
-                    elif "error" in recv_msg:
-                        if raise_err:
-                            raise errors.CDPRecvErrorMsg(recv_msg["error"])
-                        return False, recv_msg["error"]
-
-                    logger.error("没有结果：{}", recv_msg)
-                except Empty:
-                    if time.time() - start_time >= 30:
-                        self.__remove_result(msg_id=msg['id'])
-                        if raise_err:
-                            raise errors.CDPRecvTimeout(msg)
-                        logger.error("接收超时：{}", msg)
-                        break
+            return True, msg
         except (errors.CDPRecvTimeout, errors.CDPRecvErrorMsg):
             raise
         except (websocket.WebSocketConnectionClosedException, ConnectionResetError):
             logger.warning("连接已断开：{}", self.driver_url)
         except:
             traceback.print_exc()
+            raise
 
         return False, dict()
 
     def __recv_result(self):
         """
         接收消息、事件处理
 
@@ -409,22 +443,37 @@
                 if self.__stop:
                     return
                 else:
                     self.__stop = True
                     raise
 
             # 消息处理
-            if msg.get("id") and msg.get("id") in self.__result_monitor:
+            if msg.get("id"):
+                has_error = False
                 if msg.get("error"):
                     logger.error("[RECV] {}", msg["error"])
-                self.__add_result(msg_id=msg["id"], result=msg)
+                    has_error = True
+
+                # 消息 id 存在的话就是需要立刻回调
+                if msg["id"] in self.__result_monitor:
+                    self.__add_result(msg_id=msg["id"], result=msg)
+                else:
+                    # 判断响应-body 获取事件的触发
+                    event_name = f"Network.getResponseBody-{msg['id']}"
+                    if event_name in self._events:
+                        if has_error:
+                            self.emit(event=event_name, status=False, body_data=msg["error"])
+                        else:
+                            self.emit(event=event_name, status=True, body_data=msg["result"])
+
             elif "method" in msg:
                 method = msg.get("method", "")
                 params = msg.get("params", {})
-                self.emit(method, **params)
+                if method in self._events:
+                    self.emit(event=method, **params)
 
     def closed(self) -> bool:
         """
         判断连接是否断开，同时做一点处理
 
         :return:
         """
```

### Comparing `EasyPage-0.0.4/easypage/driver/browser.py` & `EasyPage-0.0.5/easypage/driver/browser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """
     浏览器 driver
 """
-from typing import Tuple, Union, Dict, List
-
+from typing import Tuple, Union, Dict, List, Callable
 from easypage import definition, errors
 from easypage.driver.page import PageDriver
+from easypage.listener import Listener
 from easypage.logger import logger
 from easypage.conn import TYPE_BROWSER, TYPE_PAGE
 from easypage.driver.driver import Driver
 from easypage.options import BrowserOptions
+from easypage.utils.other_utils import DoublyLinkedDict
 
 
 class BrowserDriver(Driver):
-    PAGES: Dict[str, "PageDriver"] = {}
-    CONTEXTS: Dict[str, Union["BrowserDriver", "ContextDriver"]] = {}
+    PAGES: Dict[str, "PageDriver"] = {}  # {page_id:page_driver}
+    CONTEXTS: Dict[str, Union["BrowserDriver", "ContextDriver"]] = {}  # {context_id:context_driver}
+    PAGE_CONTENT_MAPS: Dict[str, str] = {}  # {page_id:context_id}
+    CONTENT_PAGE_MAPS: Dict[str, List[str]] = {}  # {context_id:[page_id]}
+
+    # TODO CONTEXT 对 PAGE 是一对多的，不能用双向表
 
     def __init__(self, opts: BrowserOptions, driver_id: str):
         """
 
         :param opts:
         :param driver_id:
         """
@@ -25,22 +30,23 @@
 
         # 获取基本信息
         _, targets = self.cdp.target.get_targets()
         self._context_id = targets['targetInfos'][0]['browserContextId']
         self._proxy = self._opts.proxy
         self.__class__.CONTEXTS[self._context_id] = self
         self.__create_page_driver(targets['targetInfos'])  # 启动时创建页面的 driver
+        self.__listener = Listener(context_id=self._context_id)
 
         # 启用事件
         self.cdp.target.set_discover_targets()
 
         # 事件监听
-        self.on(event="Target.targetCreated", callback=self.__on_target_target_created)
-        self.on(event="Target.targetInfoChanged", callback=self.__on_target_target_info_changed)
-        self.on(event="Target.targetDestroyed", callback=self.__on_target_target_destroyed)
+        self.cdp.on(event="Target.targetCreated", callback=self.__on_target_target_created)
+        self.cdp.on(event="Target.targetInfoChanged", callback=self.__on_target_target_info_changed)
+        self.cdp.on(event="Target.targetDestroyed", callback=self.__on_target_target_destroyed)
 
     def __create_page_driver(self, target_infos: List[Dict]):
         """
         根据 target_infos 创建页面的连接
 
         :param target_infos: 启动时所有的页面信息
         :return:
@@ -53,17 +59,32 @@
             proxy = self.__class__.CONTEXTS[context_id]._proxy if context_id in self.__class__.CONTEXTS else None
 
             # 创建 driver
             page_driver = PageDriver(
                 opts=self._opts,
                 driver_id=target_info["targetId"],  # 页面的 targetId
                 context_id=context_id,  # 页面的上下文 id
+                context_driver=self.__class__.CONTEXTS[context_id],
                 proxy=proxy,
             )
             self.__class__.PAGES[target_info["targetId"]] = page_driver
+            self.__class__.PAGE_CONTENT_MAPS[target_info["targetId"]] = context_id
+
+            if context_id not in self.__class__.CONTENT_PAGE_MAPS:
+                self.__class__.CONTENT_PAGE_MAPS[context_id] = []
+            self.__class__.CONTENT_PAGE_MAPS[context_id].append(target_info["targetId"])
+
+    @property
+    def listen(self) -> Listener:
+        """
+        事件监听
+
+        :return:
+        """
+        return self.__listener
 
     def new_context(self, proxy: definition.Proxy = None, **kwargs) -> "ContextDriver":
         """
         创建新上下文（类似于隐身模式）
 
         :param proxy:
         :param kwargs:
@@ -161,29 +182,35 @@
         :param args:
         :param kwargs:
         :return:
         """
         target_id = kwargs["targetId"]
 
         if target_id in self.__class__.PAGES:
-            del self.__class__.PAGES[target_id]
+            if "target_id" in self.__class__.PAGES:
+                del self.__class__.PAGES[target_id]
+
+            if "target_id" in self.__class__.PAGE_CONTENT_MAPS:
+                context_id = self.__class__.PAGE_CONTENT_MAPS.pop(target_id)
+                self.__class__.CONTENT_PAGE_MAPS[context_id].remove(target_id)
 
 
 class ContextDriver:
 
     def __init__(self, browser_driver: BrowserDriver, context_id: str, proxy: definition.Proxy = None):
         """
 
         :param browser_driver:
         :param context_id:
         :param proxy: 代理
         """
         self._browser_driver = browser_driver
         self._context_id = context_id
         self._proxy = proxy
+        self.__listener = Listener(context_id=self._context_id)
 
     def new_page(
             self,
             new_window: bool = False,
             **kwargs
     ) -> "PageDriver":
         """
@@ -196,14 +223,29 @@
         return self._browser_driver.new_page(
             new_window=new_window,
             context_id=self._context_id,
             proxy=self._proxy,
             **kwargs
         )
 
+    @property
+    def listen(self) -> Listener:
+        """
+        事件监听
+
+        :return:
+        """
+        return self.__listener
+
     def close(self):
         """
         关闭上下文
 
         :return:
         """
         self._browser_driver.cdp.target.close_target(target_id=self._context_id)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
```

### Comparing `EasyPage-0.0.4/easypage/driver/driver.py` & `EasyPage-0.0.5/easypage/driver/driver.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """
     Driver 的基类
 """
-from typing import Callable
-
 from easypage.cdp import CDP
 from abc import abstractmethod
 from easypage.conn import Conn, DRIVER_TYPE
 from easypage.options import BrowserOptions
 
 
 class Driver:
@@ -17,48 +15,19 @@
         :param driver_type:
         :param driver_id:
         """
         self._opts = opts
         self.__conn = Conn(
             address=opts.address,
             driver_type=driver_type,
-            driver_id=driver_id
+            driver_id=driver_id,
+            timeout=opts.timeout
         )
         self.__cdp = CDP(conn=self.__conn)
 
-    def on(self, event: str, callback: Callable):
-        """
-        新增事件
-
-        :param event:
-        :param callback:
-        :return:
-        """
-        self.__conn.on(event=event, f=callback)
-
-    def once(self, event: str, callback: Callable):
-        """
-        新增事件，并且只执行一次
-
-        :param event:
-        :param callback:
-        :return:
-        """
-        self.__conn.once(event=event, f=callback)
-
-    def emit(self, *args, **kwargs):
-        """
-        触发事件
-
-        :param args:
-        :param kwargs:
-        :return:
-        """
-        self.__conn.emit(*args, **kwargs)
-
     @property
     def cdp(self) -> CDP:
         """
         获取 Chrome DevTools Protocol 实例
 
         :return:
         """
```

### Comparing `EasyPage-0.0.4/easypage/driver/page.py` & `EasyPage-0.0.5/easypage/driver/page.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,81 @@
 """
     页面 driver
 """
+import json
+import re
+import threading
 import time
 import base64
 import websocket
 from pathlib import Path
 from parsel import Selector
 from bs4 import BeautifulSoup
+from easypage.listener import Listener
 from easypage.logger import logger
-from typing import Tuple, Union, List
 from easypage.driver.driver import Driver
 from easypage.options import BrowserOptions
+from typing import Tuple, Union, List, Callable
 from easypage import definition, errors, operate
 from easypage.conn import TYPE_PAGE, DRIVER_TYPE
+from easypage.request import Request
+from easypage.response import Response
 from easypage.utils import other_utils, browser_utils
 
 
 class PageDriver(Driver):
-    def __init__(self, opts: BrowserOptions, driver_id: str, context_id: str = None, proxy: definition.Proxy = None):
+    def __init__(
+            self,
+            opts: BrowserOptions,
+            driver_id: str,
+            context_id: str,
+            context_driver,
+            proxy: definition.Proxy = None
+    ):
         """
 
-        :param opts:
-        :param driver_id:
+        :param opts: 配置
+        :param driver_id: driver_id
+        :param context_id: 所属上下文 id
+        :param context_driver: 所属上下文 driver
+        :param proxy: 代理
         """
         super().__init__(opts, TYPE_PAGE, driver_id)
         self._driver_id = driver_id
         self._context_id = context_id
         self._proxy = proxy
         self._opts = opts
+        self._context_driver = context_driver
 
+        # TODO 查找一下是否有可能出现未捕获到请求，但是出现响应的情况
         # 预设参数
-        self.__loading = False
-        self.__requests_cache = {}
+        self.__loading: bool = True
+        self.__requests_cache = {}  # 可能会有相同请求，request_id 也一样，所以不能移除
+        self.__response_cache = {}
 
+        # TODO 考虑根据不同的条件去设置是否启动监听避免额外的资源消耗，可以根据事件在 Listener 进行驱动
         # 启用事件
         self.cdp.dom.enable()
         self.cdp.page.enable()
         self.cdp.security.set_ignore_certificate_errors()
         self.cdp.fetch.enable(handle_auth_requests=True)
+        self.cdp.network.enable()
 
         # 事件监听
-        self.on(event='Page.loadEventFired', callback=self.__on_page_load_event_fired)
-        self.on(event='Page.frameStartedLoading', callback=self.__on_page_frame_started_loading)
-        self.on(event='Page.frameStoppedLoading', callback=self.__on_page_frame_stopped_loading)
-        self.on(event='Fetch.requestPaused', callback=self.__on_fetch_request_paused)
-        self.on(event='Fetch.authRequired', callback=self.__on_fetch_auth_required)
+        self.cdp.on(event='Page.lifecycleEvent', callback=self.__on_page_life_cycle_event)
+        self.cdp.on(event='Page.loadEventFired', callback=self.__on_page_load_event_fired)
+        self.cdp.on(event='Page.frameStartedLoading', callback=self.__on_page_frame_started_loading)
+        self.cdp.on(event='Page.frameStoppedLoading', callback=self.__on_page_frame_stopped_loading)
+        self.cdp.on(event='Fetch.requestPaused', callback=self.__on_fetch_request_paused)
+        self.cdp.on(event='Fetch.authRequired', callback=self.__on_fetch_auth_required)
+        self.cdp.on(event='Network.requestWillBeSent', callback=self.__on_network_request_will_be_sent)
+        self.cdp.on(event='Network.requestWillBeSentExtraInfo',
+                    callback=self.__on_network_request_will_be_sent_extra_info)
+        self.cdp.on(event='Network.responseReceived', callback=self.__on_network_response_received)
+        self.cdp.on(event='Network.loadingFinished', callback=self.__on_network_loading_finished)
 
     def get(self, url, **kwargs) -> Tuple[bool, Union[None, str]]:
         """
         访问某个页面
 
         返回的第一个值是请求命令是否成功
         返回的第二个值是当请求失败的时候发送原因，比如设置的代理访问不通
@@ -136,15 +163,15 @@
             return status, result
 
         if 'value' in result['result']:
             return True, result['result']['value']
         else:
             return False, result['result']['description']
 
-    def iframes(self) -> List['IframeElement']:
+    def iframes(self) -> List["Element"]:
         """
         获取所有的 iframe
 
         :return:
         """
         # operate.pages(self._opts.address)
 
@@ -153,33 +180,88 @@
         status, new_node_ids = self.cdp.dom.query_selector_all(
             selector="iframe",
         )
         if not new_node_ids or not status:
             return elements
 
         for node_id in new_node_ids['nodeIds']:
-            status, frame_id = self.cdp.dom.describe_node(nodeId=node_id)
-            if not frame_id or not status:
+            # 获取 frameId
+            status, frame_detail = self.cdp.dom.describe_node(nodeId=node_id)
+            if not frame_detail or not status:
                 continue
+            frame_id = frame_detail['node']['frameId']
 
-            frame_id = frame_id['node']['frameId']
+            # 判断是否同域
+            status, frame_tree = self.cdp.page.get_frame_tree()
+            if not status:
+                continue
+            frame_tree = frame_tree["frameTree"]
 
-            try:
-                # TODO 需要思考需不需要加入 BrowserDriver，如何管理
-                elements.append(IframeElement(
-                    opts=self._opts,
-                    driver_id=frame_id,
-                    context_id=self._context_id,
-                    proxy=self._proxy
+            """
+                小知识点
+                同域名的情况下，再次查询实际上是基于 iframe 的 document
+                所以这里在新建 iframe 的时候是要基于 iframe document 的 nodeId，这点和普通元素不一样
+                
+                不同域名的情况下，实际上就是另一个 page 去对待即可
+            """
+            if frame_id in json.dumps(frame_tree, ensure_ascii=False):  # 同域的话会获取到比如在 'childFrames' 内
+                elements.append(Element(
+                    node_id=frame_detail["node"]["contentDocument"]['nodeId'],
+                    page=self,
+                    is_iframe=True,
+                    iframe_node_id=node_id,
+                    iframe_owner_page=self
                 ))
-            except websocket.WebSocketBadStatusException:
-                logger.warning("当前 iframe 可能已不在页面上：{}", frame_id)
+            else:
+                try:
+                    page_driver = PageDriver(
+                        opts=self._opts,
+                        driver_id=frame_id,  # 页面的 targetId
+                        context_id=self._context_id,  # 页面的上下文 id
+                        context_driver=self._context_driver,
+                        proxy=self._proxy,
+                    )
+                    status, iframe_dom = page_driver.cdp.dom.get_document()
+                    if not status:
+                        continue
+                    elements.append(Element(
+                        node_id=iframe_dom['root']['nodeId'],  # 这里的原理和上面一样，直接放 dom 的 id
+                        page=page_driver,
+                        is_iframe=True,
+                        iframe_node_id=node_id,
+                        iframe_owner_page=self
+                    ))
+                except websocket.WebSocketBadStatusException:
+                    logger.warning("当前 iframe 可能已不在页面上：{}", frame_id)
 
         return elements
 
+    def iframe_search(self, attr_name: str, attr_value: str, is_regex: bool = False) -> "Element":
+        """
+        这里是提供了一组可以通过指定属性，通过【正则、in】去匹配属性值的方法
+
+        :param attr_name: 需要去判断的属性名
+        :param attr_value: 对应属性名
+        :param is_regex: 为 False 时通过 in 判断，为 True 时通过 re 正则判断
+        :return:
+        """
+        iframes = self.iframes()
+
+        for iframe in iframes:
+            if not iframe.attrs.get(attr_name):
+                continue
+
+            attr = iframe.attrs[attr_name]
+
+            if is_regex:
+                if re.search(attr_value, attr):
+                    return iframe
+            elif attr_value in attr:
+                return iframe
+
     def cookies(self, only_key_val: bool = True, domain: str = None) -> Union[List[dict], dict]:
         """
         获取 cookie
 
         :param only_key_val: 是否仅返回 {name:'',value:''} 形式
         :param domain: 指定域名
         :return: [{'name': '', 'value': '', 'domain': '', 'path': '', 'expires': -1, 'size': 161, 'httpOnly': True, 'secure': True, 'session': True, 'sameSite': 'Strict', 'priority': 'Medium', 'sameParty': False, 'sourceScheme': 'Secure', 'sourcePort': 443}]
@@ -280,15 +362,18 @@
         :param timeout:
         :return:
         """
         timeout = timeout or self._opts.timeout
 
         start_time = time.time()
         while time.time() - start_time < timeout:
-            if not self.__loading:
+            # if not self.__loading:
+            #     return
+            if self.eval_js(js="document.readyState")[-1] == "complete":
+                self.__loading = False
                 return
             time.sleep(0.1)
 
     def wait_for_selector(
             self,
             selector: str,
             timeout: int = None,
@@ -380,19 +465,38 @@
 
         status, html = self.cdp.dom.get_outer_html(backendNodeId=back_end_node_id)
         if not status:
             return ""
 
         return html["outerHTML"]
 
+    @property
+    def listen(self) -> Listener:
+        """
+        事件监听
+
+        :return:
+        """
+        return self._context_driver.listen
+
     """
        事件监听
     """
 
     @other_utils.catch_error
+    def __on_page_life_cycle_event(self, *args, **kwargs):
+        """
+        针对顶级页面生命周期事件（如导航、加载、绘制等）触发
+
+        :return:
+        """
+        self.__loading = True
+        logger.debug("页面开始加载：{}", kwargs)
+
+    @other_utils.catch_error
     def __on_page_load_event_fired(self, *args, **kwargs):
         """
         页面加载完成将会被触发
 
         :return:
         """
         self.__loading = False
@@ -425,21 +529,70 @@
 
         https://chromedevtools.github.io/devtools-protocol/tot/Fetch/#event-requestPaused
 
         :param args:
         :param kwargs: {"method":"Fetch.requestPaused","params":{"requestId":"interception-job-1.0","request":{"url":"https://www.baidu.com/","method":"GET","headers":{"Accept":"text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7","Upgrade-Insecure-Requests":"1","User-Agent":"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36","sec-ch-ua":"\"Chromium\";v=\"125\", \"Not.A/Brand\";v=\"24\"","sec-ch-ua-mobile":"?0","sec-ch-ua-platform":"\"Windows\""},"initialPriority":"VeryHigh","referrerPolicy":"strict-origin-when-cross-origin"},"frameId":"E361A685E14EAEC054BEF17592DF25DF","resourceType":"Document"}}
         :return:
         """
-        request_id = kwargs['requestId']
-        self.__requests_cache[request_id] = kwargs['request']
+        request_id = kwargs["requestId"]
+        network_id = kwargs.get("networkId")  # fetch 的 networkId 就是 network 的 requestId
 
         self.cdp.fetch.continue_request(
             request_id=request_id,
         )
 
+        if not network_id:
+            return
+
+        # 请求输出
+        request = Request(kwargs)
+        # logger.warning("requests 存入：{}", network_id)
+        self.__requests_cache[network_id] = request
+
+        # 请求触发
+        self.listen._on_request(request=request)
+
+    @other_utils.catch_error
+    def __on_network_request_will_be_sent(self, *args, **kwargs):
+        """
+        请求监听
+
+        有时候 fetch 监听不到，需要通过这里监听
+
+        https://chromedevtools.github.io/devtools-protocol/tot/Network/#event-requestWillBeSent
+
+        :param args:
+        :param kwargs:
+        :return:
+        """
+        request_id = kwargs['requestId']
+
+        if request_id not in self.__requests_cache:
+            # logger.warning("request_will_be_sent 存入：{}", request_id)
+
+            request = Request(kwargs)
+
+            self.__requests_cache[request_id] = request
+
+            # 请求触发
+            self.listen._on_request(request=request)
+
+    @other_utils.catch_error
+    def __on_network_request_will_be_sent_extra_info(self, *args, **kwargs):
+        """
+        请求监听
+
+        https://chromedevtools.github.io/devtools-protocol/tot/Network/#event-requestWillBeSentExtraInfo
+
+        :param args:
+        :param kwargs:
+        :return:
+        """
+        request_id = kwargs['requestId']
+
     @other_utils.catch_error
     def __on_fetch_auth_required(self, *args, **kwargs):
         """
         监听 authRequired
 
         https://chromedevtools.github.io/devtools-protocol/tot/Fetch/#event-authRequired
 
@@ -464,14 +617,62 @@
 
         self.cdp.fetch.continue_with_auth(
             request_id=request_id,
             user=user,
             pwd=pwd,
         )
 
+    @other_utils.catch_error
+    def __on_network_response_received(self, *args, **kwargs):
+        """
+        响应监听
+
+        https://chromedevtools.github.io/devtools-protocol/tot/Network/#event-responseReceived
+
+        :param args:
+        :param kwargs:
+        :return:
+        """
+        request_id = kwargs["requestId"]
+
+        # 存储响应
+        self.__response_cache[request_id] = kwargs
+
+    @other_utils.catch_error
+    def __on_network_loading_finished(self, *args, **kwargs):
+        """
+        响应结束
+
+        https://chromedevtools.github.io/devtools-protocol/tot/Network/#event-loadingFinished
+
+        :param args:
+        :param kwargs:
+        :return:
+        """
+        request_id = kwargs["requestId"]
+
+        # 获取请求
+        if request_id not in self.__requests_cache:
+            logger.warning("请求缓存无该 id：{}", request_id)
+            return
+        request_cache = self.__requests_cache[request_id]
+        response_cache = self.__response_cache[request_id]
+
+        # 存储输出
+        response = Response(response_cache, request_cache, self.cdp)
+
+        # 触发响应
+        self.listen._on_response(response, self.cdp)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
+
 
 """
     动作链
 """
 
 
 # modifiers
@@ -686,25 +887,47 @@
 
 """
     元素
 """
 
 
 class Element(ActionChain):
-    def __init__(self, node_id: int, page: PageDriver):
+    def __init__(
+            self,
+            node_id: int,
+            page: PageDriver,
+            is_iframe: bool = False,
+            iframe_node_id: int = None,
+            iframe_owner_page: PageDriver = None
+    ):
         """
         生成节点
 
-        :param node_id 当前节点的 id
-        :param page PageDriver 对象
+        如果是 iframe 那么这里获取的实际上就是 iframe 的 dom 而不是 iframe 自身
+        :param node_id 当前节点的 id（iframe 的话就是 iframe document 的 node_id）
+        :param page PageDriver 对象（iframe 的话就是 iframe 自身的 driver）
+        :param is_iframe 是不是 iframe
+        :param iframe_node_id iframe 自身的 node_id
+        :param iframe_owner_page iframe 所在页面
         :return:
         """
-        super().__init__(node_id, page)
+        if is_iframe:
+            super().__init__(iframe_node_id, iframe_owner_page)
+        else:
+            super().__init__(node_id, page)
+
+        self._back_end_node_id = None
+        self._obj_id = None
+        self._is_iframe = is_iframe
+        self._iframe_node_id = iframe_node_id
+        self._iframe_owner_page = iframe_owner_page
+        self._iframe_page = page
+        self._iframe_document_node_id = node_id
 
-        self.__tagName: str = None
+        self.__tagName: str = None if not is_iframe else "iframe"  # type:ignore
 
     def query_selector(
             self,
             selector: str,
             raise_err: bool = False
     ) -> Union['Element', None, errors.ElementNotFound]:
         """
@@ -712,14 +935,20 @@
 
         通过这种绕一圈的书写方式，就可以有编辑器的提示了
 
         :param selector: 选择器（支持 css、xpath）
         :param raise_err: 是否报错
         :return:
         """
+        if self._is_iframe:
+            return self._iframe_page.query_selector(
+                selector=selector,
+                node_id=self._iframe_document_node_id,
+                raise_err=raise_err
+            )
         return self.page.query_selector(
             selector=selector,
             node_id=self.node_id,
             raise_err=raise_err
         )
 
     def query_selector_all(
@@ -730,30 +959,37 @@
         """
         选择元素
 
         :param selector: 选择器（支持 css、xpath）
         :param raise_err: 是否报错
         :return:
         """
+        if self._is_iframe:
+            return self._iframe_page.query_selector_all(
+                selector=selector,
+                node_id=self._iframe_document_node_id,
+                raise_err=raise_err
+            )
         return self.page.query_selector_all(
             selector=selector,
+            node_id=self.node_id,
             raise_err=raise_err,
         )
 
     def eval_js_on_selector(self, js: str, **kwargs):
         """
         执行 js 脚本（会自动使用 function 包裹，不然无法执行）
 
         学习链接：https://chromedevtools.github.io/devtools-protocol/tot/Runtime/#method-evaluate
 
         :param js: 路径或者 js 字符串
         :return:
         """
         js = "function (){ %s }" % js
-        return self.page.cdp.runtime.call_function_on(js=js, object_id=self._object_id, **kwargs)
+        return self.page.cdp.runtime.call_function_on(js=js, object_id=self.object_id, **kwargs)
 
     def click(self, count: int = 1, button: str = "left", raise_err: bool = True, simulation: bool = True):
         """
         执行点击
 
         :param count: 点击次数
         :param button: 代表鼠标的按键，如：none（不触发按键，代表光标）, left（左击）, middle（滚轮）, right（右击）, back（后退）, forward（前进）
@@ -809,14 +1045,17 @@
         :return:
         """
         status, attrs = self.page.cdp.dom.get_attributes(node_id=self.node_id)
 
         if not status:
             return {}
 
+        attrs_list = attrs["attributes"]
+        attrs = dict(zip(attrs_list[::2], attrs_list[1::2]))
+
         return attrs or {}
 
     @property
     def tag_name(self) -> str:
         """
         节点名称
 
@@ -829,17 +1068,26 @@
         return self.__tagName
 
     @property
     def html(self) -> str:
         """
         html 文本
 
+        iframe 获取的是 iframe document 的 html
+
         :return: <input type="submit" id="su" value="百度一下" class="bg s_btn">
         """
-        status, html = self.page.cdp.dom.get_outer_html(backendNodeId=self._back_end_node_id)
+        if self._is_iframe:
+            describe_status, node = self._iframe_page.cdp.dom.describe_node(nodeId=self._iframe_document_node_id)
+            if not describe_status:
+                return ""
+            iframe_document_back_end_node_id = node['node']['backendNodeId']
+            status, html = self._iframe_page.cdp.dom.get_outer_html(backendNodeId=iframe_document_back_end_node_id)
+        else:
+            status, html = self.page.cdp.dom.get_outer_html(backendNodeId=self.back_end_node_id)
 
         if not status:
             return ""
 
         return html["outerHTML"]
 
     @property
@@ -866,34 +1114,38 @@
         获取 bs4 解析器
 
         :return:
         """
         return BeautifulSoup(self.html, "lxml")
 
     @property
-    def _back_end_node_id(self) -> int:
+    def back_end_node_id(self) -> int:
         """
         获取 backendNodeId
 
         :return:
         """
-        _, node = self.page.cdp.dom.describe_node(nodeId=self.node_id)
+        if not self._back_end_node_id:
+            _, node = self.page.cdp.dom.describe_node(nodeId=self.node_id)
+            self._back_end_node_id = node['node']['backendNodeId']
 
-        return node['node']['backendNodeId']
+        return self._back_end_node_id
 
     @property
-    def _object_id(self) -> str:
+    def object_id(self) -> str:
         """
         获取 object_id
 
         :return:
         """
-        _, node = self.page.cdp.dom.resolve_node(backendNodeId=self._back_end_node_id)
+        if not self._obj_id:
+            _, node = self.page.cdp.dom.resolve_node(backendNodeId=self.back_end_node_id)
+            self._obj_id = node['object']['objectId']
 
-        return node['object']['objectId']
+        return self._obj_id
 
     def __repr__(self):
         attrs = self.attrs
         attrs_text = ' '.join([f'{i}="{attrs[i]}"' for i in attrs.keys()])
         return f"<{self.__class__.__name__} {self.tag_name} {attrs_text}>"
```

### Comparing `EasyPage-0.0.4/easypage/errors.py` & `EasyPage-0.0.5/easypage/errors.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/logger.py` & `EasyPage-0.0.5/easypage/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,7 +74,8 @@
             self.logger.critical(msg)
 
 
 if settings.SYSTEM_TYPE == 'linux':
     logger = Logger()
 else:
     from loguru import logger
+# logger = Logger()
```

### Comparing `EasyPage-0.0.4/easypage/main.py` & `EasyPage-0.0.5/easypage/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             reuse_close: bool = False
     ):
         """
 
         :param opts: 配置
         :param log_level: 日志等级（如：logging 模块的 logging.WARNING）
         :param reuse: 是否复用已经存在的浏览器（根据 opts 内的端口判断复用，无法复用则创建新端口）
-        :param reuse_close: 复用浏览器时，是否在结束时关闭浏览器并清理资源（默认关闭）
+        :param reuse_close: 复用浏览器时，是否在结束时关闭浏览器并清理资源（默认不关闭）
         """
         # 配置日志等级
         log_level = log_level or settings.LOGGER_LEVEL
         # TODO: 临时处理，为了通过 loguru，后续需要修改
         if not settings.SYSTEM_TYPE.startswith("win"):
             logger.logger.setLevel(log_level)
 
@@ -37,25 +37,39 @@
 
         self._proc: "Popen" = None  # type: ignore
         self._start_browser()
 
         self._browser_driver_id = browser_utils.parse_driver_id(operate.browser(opts.address))[0]
         self._browser_driver = BrowserDriver(opts=self._opts, driver_id=self._browser_driver_id)
 
-    @staticmethod
-    def pages() -> List["PageDriver"]:
+    @property
+    def browser(self) -> "BrowserDriver":
+        return self._browser_driver
+
+    @property
+    def page(self) -> "PageDriver":
+        """
+        默认页面
+
+        :return:
+        """
+        default_page_id = BrowserDriver.CONTENT_PAGE_MAPS[self.browser._context_id][0]
+        return BrowserDriver.PAGES[default_page_id]
+
+    @property
+    def pages(self) -> List["PageDriver"]:
         """
         获取所有的当前页面
 
         :return:
         """
         return list(BrowserDriver.PAGES.values())
 
-    @staticmethod
-    def contexts() -> List["ContextDriver"]:
+    @property
+    def contexts(self) -> List["ContextDriver"]:
         """
         获取指定上下文
 
         :return:
         """
         return list(BrowserDriver.CONTEXTS.values())
 
@@ -88,15 +102,19 @@
                 if self._reuse_close:
                     atexit.register(self.close)
                 return
 
         # 打开新的浏览器
         from easypage import operate
         self._proc = operate.new_browser(opts=self._opts)
-        atexit.register(self.close)
+        if not self._reuse:
+            atexit.register(self.close)
+
+        if self._reuse and self._reuse_close:
+            atexit.register(self.close)
 
         # 等待浏览器打开
         operate.wait_connection(opts=self._opts)
 
     def close(self):
         """
         关闭浏览器，清理资源，如删除资源文件夹
```

### Comparing `EasyPage-0.0.4/easypage/operate.py` & `EasyPage-0.0.5/easypage/operate.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/options.py` & `EasyPage-0.0.5/easypage/options.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/settings.py` & `EasyPage-0.0.5/easypage/settings.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/easypage/utils/browser_utils.py` & `EasyPage-0.0.5/easypage/utils/browser_utils.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.4/setup.py` & `EasyPage-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EasyPage',
-    version='0.0.4',
+    version='0.0.5',
     author='leviathangk',
     author_email='1015295213@qq.com',
     description='基于 CDP 协议，简洁快速的浏览器控制 API',
     keywords=['EasyPage', 'page', 'browser'],
     packages=find_packages(),
     install_requires=[
         "lxml",
```

