# Comparing `tmp/gy_redis-0.1.6.tar.gz` & `tmp/gy_redis-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gy_redis-0.1.6.tar", last modified: Sat Apr  8 13:16:21 2023, max compression
+gzip compressed data, was "dist\gy_redis-0.1.7.tar", last modified: Sat May 11 08:55:26 2024, max compression
```

## Comparing `gy_redis-0.1.6.tar` & `gy_redis-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 13:16:21.203122 gy_redis-0.1.6/
--rw-rw-rw-   0        0        0     1091 2023-01-26 09:08:23.000000 gy_redis-0.1.6/LICENSE
--rw-rw-rw-   0        0        0        0 2023-01-26 08:36:13.000000 gy_redis-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      725 2023-04-08 13:16:21.203122 gy_redis-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-03-08 06:28:44.000000 gy_redis-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 13:16:21.196542 gy_redis-0.1.6/gy_redis/
--rw-rw-rw-   0        0        0      823 2023-03-30 14:17:50.000000 gy_redis-0.1.6/gy_redis/__init__.py
--rw-rw-rw-   0        0        0     6928 2023-04-08 13:14:39.000000 gy_redis-0.1.6/gy_redis/handler.py
--rw-rw-rw-   0        0        0     1329 2023-03-30 14:17:50.000000 gy_redis-0.1.6/gy_redis/manager.py
-drwxrwxrwx   0        0        0        0 2023-04-08 13:16:21.201858 gy_redis-0.1.6/gy_redis.egg-info/
--rw-rw-rw-   0        0        0      725 2023-04-08 13:16:21.000000 gy_redis-0.1.6/gy_redis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-04-08 13:16:21.000000 gy_redis-0.1.6/gy_redis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       31 2023-04-08 13:16:21.000000 gy_redis-0.1.6/gy_redis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-08 13:16:21.000000 gy_redis-0.1.6/gy_redis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-08 13:16:21.000000 gy_redis-0.1.6/gy_redis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-01-30 22:59:06.000000 gy_redis-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 13:16:21.203122 gy_redis-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1043 2023-04-08 13:15:07.000000 gy_redis-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 08:55:26.750096 gy_redis-0.1.7/
+-rw-rw-rw-   0        0        0     1091 2023-01-26 09:08:23.000000 gy_redis-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-01-26 08:36:13.000000 gy_redis-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      789 2024-05-11 08:55:26.749077 gy_redis-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-05-11 08:14:08.000000 gy_redis-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 08:55:26.725446 gy_redis-0.1.7/gy_redis/
+-rw-rw-rw-   0        0        0      823 2023-03-30 14:17:50.000000 gy_redis-0.1.7/gy_redis/__init__.py
+-rw-rw-rw-   0        0        0     6907 2024-05-11 05:10:25.000000 gy_redis-0.1.7/gy_redis/handler.py
+-rw-rw-rw-   0        0        0     1329 2023-03-30 14:17:50.000000 gy_redis-0.1.7/gy_redis/manager.py
+drwxrwxrwx   0        0        0        0 2024-05-11 08:55:26.747458 gy_redis-0.1.7/gy_redis.egg-info/
+-rw-rw-rw-   0        0        0      789 2024-05-11 08:55:26.000000 gy_redis-0.1.7/gy_redis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-11 08:55:26.000000 gy_redis-0.1.7/gy_redis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       31 2024-05-11 08:55:26.000000 gy_redis-0.1.7/gy_redis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-11 08:55:26.000000 gy_redis-0.1.7/gy_redis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-11 08:55:26.000000 gy_redis-0.1.7/gy_redis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-01-30 22:59:06.000000 gy_redis-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 08:55:26.750096 gy_redis-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1043 2024-05-11 08:54:40.000000 gy_redis-0.1.7/setup.py
```

### Comparing `gy_redis-0.1.6/LICENSE` & `gy_redis-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gy_redis-0.1.6/PKG-INFO` & `gy_redis-0.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gy_redis
-Version: 0.1.6
+Version: 0.1.7
 Summary: GuanYu for test
 Home-page: https://github.com/guanyuhoujeff/gy-redis
 Author: jeff7522553
 Author-email: jeff7522553@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,18 +12,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gy-redis
 
 ## pip package
 ```
-pip install gy-redis
+pip install gy-redis -U
 ```
 
 ## build package
+First change the version or related information of setup.py
 ```
 python setup.py sdist bdist_wheel 
 ```
 
 ## push pypitest
 ```
 python -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
```

### Comparing `gy_redis-0.1.6/gy_redis/__init__.py` & `gy_redis-0.1.7/gy_redis/__init__.py`

 * *Files identical despite different names*

### Comparing `gy_redis-0.1.6/gy_redis/handler.py` & `gy_redis-0.1.7/gy_redis/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         else:
             return False
         
     @property
     def pub_sub(self) -> redis.client.PubSub:
         return  self._pub_sub
 
-
 class RedisConnector:
     ## python SingleTon
     _instance = None 
     def __new__(cls, *args, **kwargs): 
         if cls._instance is None: 
             cls._instance = super().__new__(cls) 
         return cls._instance
@@ -131,28 +130,27 @@
 
     def stopPubsubJob(self):
         if not self._pubsub_job is None and self._pubsub_job.is_alive:
             self._pubsub_job.stop()
             self._self_value_stream_sub.dispose()
     
     def __del__(self):
-        self._self_value_stream_sub.dispose()
+        self.stopPubsubJob()
 
 
     def buildPubsub(self, run_in_thread=True):
         self._pubsub_job = RedisPubsubJob(
             pub_sub=self._redis_connector.slaver_client.pubsub(ignore_subscribe_messages = True), 
             run_in_thread=run_in_thread
         )
 
     @property
     def pubsub_job(self):
         return self._pubsub_job
 
-
 class RedisDictHandler(RedisHandlerInterface):
     def __init__(self, redis_client: Union[redis.Redis, redis.Sentinel], topic: str, sentinel_name : Optional[str]=None) -> None:
         super().__init__(redis_client, topic, sentinel_name)
         
     def _convertReadValue(self, value) -> Optional[dict]:
         if isinstance(value, bytes):
             value = json.loads(value.decode())
```

### Comparing `gy_redis-0.1.6/gy_redis/manager.py` & `gy_redis-0.1.7/gy_redis/manager.py`

 * *Files identical despite different names*

### Comparing `gy_redis-0.1.6/gy_redis.egg-info/PKG-INFO` & `gy_redis-0.1.7/gy_redis.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gy-redis
-Version: 0.1.6
+Version: 0.1.7
 Summary: GuanYu for test
 Home-page: https://github.com/guanyuhoujeff/gy-redis
 Author: jeff7522553
 Author-email: jeff7522553@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,18 +12,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gy-redis
 
 ## pip package
 ```
-pip install gy-redis
+pip install gy-redis -U
 ```
 
 ## build package
+First change the version or related information of setup.py
 ```
 python setup.py sdist bdist_wheel 
 ```
 
 ## push pypitest
 ```
 python -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*
```

### Comparing `gy_redis-0.1.6/setup.py` & `gy_redis-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
      'reactivex>=4.0.4',
      'opencv-python>=4.3.0',
 ]
 
 
 setuptools.setup(
     name="gy_redis", # 
-    version="0.1.6",
+    version="0.1.7",
     author="jeff7522553",
     author_email="jeff7522553@gmail.com",
     description="GuanYu for test",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/guanyuhoujeff/gy-redis",
     packages=setuptools.find_packages(),
```

