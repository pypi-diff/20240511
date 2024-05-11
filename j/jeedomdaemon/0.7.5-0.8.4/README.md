# Comparing `tmp/jeedomdaemon-0.7.5.tar.gz` & `tmp/jeedomdaemon-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeedomdaemon-0.7.5.tar", last modified: Sat Apr 27 06:13:50 2024, max compression
+gzip compressed data, was "jeedomdaemon-0.8.4.tar", last modified: Fri May 10 16:27:41 2024, max compression
```

## Comparing `jeedomdaemon-0.7.5.tar` & `jeedomdaemon-0.8.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:13:50.211341 jeedomdaemon-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-27 06:13:46.000000 jeedomdaemon-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-27 06:13:50.211341 jeedomdaemon-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-27 06:13:46.000000 jeedomdaemon-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:13:50.211341 jeedomdaemon-0.7.5/jeedomdaemon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 06:13:46.000000 jeedomdaemon-0.7.5/jeedomdaemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-27 06:13:46.000000 jeedomdaemon-0.7.5/jeedomdaemon/aio_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-27 06:13:46.000000 jeedomdaemon-0.7.5/jeedomdaemon/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-27 06:13:46.000000 jeedomdaemon-0.7.5/jeedomdaemon/base_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-27 06:13:46.000000 jeedomdaemon-0.7.5/jeedomdaemon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:13:50.211341 jeedomdaemon-0.7.5/jeedomdaemon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-27 06:13:50.000000 jeedomdaemon-0.7.5/jeedomdaemon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-27 06:13:50.000000 jeedomdaemon-0.7.5/jeedomdaemon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 06:13:50.000000 jeedomdaemon-0.7.5/jeedomdaemon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-27 06:13:50.000000 jeedomdaemon-0.7.5/jeedomdaemon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-27 06:13:50.000000 jeedomdaemon-0.7.5/jeedomdaemon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 06:13:50.211341 jeedomdaemon-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-27 06:13:46.000000 jeedomdaemon-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:13:50.211341 jeedomdaemon-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 06:13:46.000000 jeedomdaemon-0.7.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-27 06:13:46.000000 jeedomdaemon-0.7.5/tests/base_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-27 06:13:46.000000 jeedomdaemon-0.7.5/tests/base_daemon_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:27:41.735116 jeedomdaemon-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 16:27:37.000000 jeedomdaemon-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-10 16:27:41.735116 jeedomdaemon-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-10 16:27:37.000000 jeedomdaemon-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:27:41.735116 jeedomdaemon-0.8.4/jeedomdaemon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:27:37.000000 jeedomdaemon-0.8.4/jeedomdaemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-10 16:27:37.000000 jeedomdaemon-0.8.4/jeedomdaemon/aio_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-10 16:27:37.000000 jeedomdaemon-0.8.4/jeedomdaemon/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-10 16:27:37.000000 jeedomdaemon-0.8.4/jeedomdaemon/base_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-10 16:27:37.000000 jeedomdaemon-0.8.4/jeedomdaemon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:27:41.735116 jeedomdaemon-0.8.4/jeedomdaemon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-10 16:27:41.000000 jeedomdaemon-0.8.4/jeedomdaemon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-10 16:27:41.000000 jeedomdaemon-0.8.4/jeedomdaemon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 16:27:41.000000 jeedomdaemon-0.8.4/jeedomdaemon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 16:27:41.000000 jeedomdaemon-0.8.4/jeedomdaemon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 16:27:41.000000 jeedomdaemon-0.8.4/jeedomdaemon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 16:27:41.735116 jeedomdaemon-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-10 16:27:37.000000 jeedomdaemon-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:27:41.735116 jeedomdaemon-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:27:37.000000 jeedomdaemon-0.8.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-10 16:27:37.000000 jeedomdaemon-0.8.4/tests/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-10 16:27:37.000000 jeedomdaemon-0.8.4/tests/base_daemon_test.py
```

### Comparing `jeedomdaemon-0.7.5/LICENSE` & `jeedomdaemon-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.5/PKG-INFO` & `jeedomdaemon-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeedomdaemon
-Version: 0.7.5
+Version: 0.8.4
 Summary: A base to implement Jeedom daemon in python
 Home-page: https://github.com/Mips2648/jeedom-daemon-py
 Author: Mips
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
```

### Comparing `jeedomdaemon-0.7.5/README.md` & `jeedomdaemon-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.5/jeedomdaemon/aio_connector.py` & `jeedomdaemon-0.8.4/jeedomdaemon/aio_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         return asyncio.run_coroutine_threadsafe(self.send_to_jeedom(payload), _loop)
 
     async def send_to_jeedom(self, payload):
         """
         Will send the payload provided.
         return true or false if successful
         """
-        self._logger.debug('Send to jeedom :  %s', payload)
+        self._logger.debug('Send to jeedom: %s', payload)
         async with self._jeedom_session.post(self._callback_url + '?apikey=' + self._api_key, json=payload) as resp:
             if resp.status != 200:
                 self._logger.error('Error on send request to jeedom, return %s-%s', resp.status, resp.reason)
                 return False
         return True
 
     async def add_change(self, key: str, value):
```

### Comparing `jeedomdaemon-0.7.5/jeedomdaemon/base_config.py` & `jeedomdaemon-0.8.4/jeedomdaemon/base_config.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.5/jeedomdaemon/base_daemon.py` & `jeedomdaemon-0.8.4/jeedomdaemon/base_daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from .aio_connector import Publisher, Listener
 from .base_config import BaseConfig
 
 class BaseDaemon:
     """Base daemon class"""
     def __init__(self,
                  config: BaseConfig = BaseConfig(),
-                 on_start_cb: Callable[...,Awaitable[None]] | None = None,
+                 on_start_cb: Callable[..., Awaitable[None]] | None = None,
                  on_message_cb: Callable[[list], Awaitable[None]] | None = None,
-                 on_stop_cb: Callable[..., None] | None = None,
+                 on_stop_cb: Callable[..., Awaitable[None]] | None = None,
                  ) -> None:
         self._config = config
         self._config.parse()
         self.__listen_task: asyncio.Task[None] | None = None
         self._loop = None
         self._jeedom_publisher: Publisher | None = None
         self._logger = logging.getLogger(__name__)
@@ -84,32 +84,32 @@
             self._jeedom_publisher.create_send_task()
 
             await self.__add_signal_handler()
             await asyncio.sleep(1) # allow  all tasks to start
 
             await self.__listen_task
 
-    def stop(self):
+    async def stop(self):
         """ Stop your daemon if need be"""
+
         if self.__on_stop_cb is not None:
-            self.__on_stop_cb()
+            await self.__on_stop_cb()
 
         tasks = [t for t in asyncio.all_tasks() if t is not asyncio.current_task()]
-        tasks = asyncio.all_tasks()
         self._logger.info("Cancelling %i outstanding tasks", len(tasks))
         for task in tasks:
             task.cancel()
         try:
             asyncio.gather(*tasks, return_exceptions=True)
         except BaseException as e: # pylint: disable=broad-exception-caught
             self._logger.warning("Some exception occured during cancellation: %s", e)
 
     def __ask_exit(self, sig):
         self._logger.info("Signal %i caught, exiting...", sig)
-        self.stop()
+        asyncio.run_coroutine_threadsafe(self.stop(), self._loop)
 
     async def __add_signal_handler(self):
         self._loop.add_signal_handler(signal.SIGINT, functools.partial(self.__ask_exit, signal.SIGINT))
         self._loop.add_signal_handler(signal.SIGTERM, functools.partial(self.__ask_exit, signal.SIGTERM))
 
     async def __on_socket_message(self, message):
         if message['apikey'] != self._config.api_key:
```

### Comparing `jeedomdaemon-0.7.5/jeedomdaemon/utils.py` & `jeedomdaemon-0.8.4/jeedomdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.5/jeedomdaemon.egg-info/PKG-INFO` & `jeedomdaemon-0.8.4/jeedomdaemon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeedomdaemon
-Version: 0.7.5
+Version: 0.8.4
 Summary: A base to implement Jeedom daemon in python
 Home-page: https://github.com/Mips2648/jeedom-daemon-py
 Author: Mips
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
```

### Comparing `jeedomdaemon-0.7.5/setup.py` & `jeedomdaemon-0.8.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     author='Mips',
     # author_email='',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
     install_requires=['aiohttp'],
     # *strongly* suggested for sharing
-    version='0.7.5',
+    version='0.8.4',
     # The license can be anything you like
     license='MIT',
     description='A base to implement Jeedom daemon in python',
     # We will also need a readme eventually (there will be a warning)
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
 )
```

### Comparing `jeedomdaemon-0.7.5/tests/base_config_test.py` & `jeedomdaemon-0.8.4/tests/base_config_test.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.7.5/tests/base_daemon_test.py` & `jeedomdaemon-0.8.4/tests/base_daemon_test.py`

 * *Files identical despite different names*

