# Comparing `tmp/hagworm-5.9.8.tar.gz` & `tmp/hagworm-5.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagworm-5.9.8.tar", last modified: Fri Dec 15 03:15:46 2023, max compression
+gzip compressed data, was "hagworm-5.9.9.tar", last modified: Fri Dec 15 04:33:37 2023, max compression
```

## Comparing `hagworm-5.9.8.tar` & `hagworm-5.9.9.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:46.176331 hagworm-5.9.8/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)    11362 2023-03-01 02:07:14.000000 hagworm-5.9.8/LICENSE
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     5979 2023-12-15 03:15:46.174332 hagworm-5.9.8/PKG-INFO
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     5502 2023-11-18 05:32:45.000000 hagworm-5.9.8/README.md
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:44.870009 hagworm-5.9.8/example/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-03-01 02:07:14.000000 hagworm-5.9.8/example/__init__.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:44.927081 hagworm-5.9.8/example/fastapi_demo/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)       61 2023-05-26 07:33:49.000000 hagworm-5.9.8/example/fastapi_demo/__init__.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:44.961658 hagworm-5.9.8/example/fastapi_demo/controller/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)      211 2023-11-18 05:32:45.000000 hagworm-5.9.8/example/fastapi_demo/controller/__init__.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)      397 2023-11-23 00:48:29.000000 hagworm-5.9.8/example/fastapi_demo/controller/home.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)      860 2023-11-18 05:32:45.000000 hagworm-5.9.8/example/fastapi_demo/gunicorn.config.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1245 2023-11-18 05:32:45.000000 hagworm-5.9.8/example/fastapi_demo/main.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:44.978657 hagworm-5.9.8/example/fastapi_demo/model/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)       61 2023-05-26 07:33:49.000000 hagworm-5.9.8/example/fastapi_demo/model/__init__.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:44.996671 hagworm-5.9.8/example/fastapi_demo/service/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2609 2023-11-18 05:32:45.000000 hagworm-5.9.8/example/fastapi_demo/service/__init__.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2041 2023-11-18 05:32:45.000000 hagworm-5.9.8/example/fastapi_demo/setting.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1095 2023-11-18 05:32:45.000000 hagworm-5.9.8/example/main_tcp.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)      801 2023-11-27 09:37:15.000000 hagworm-5.9.8/example/main_test.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:45.009710 hagworm-5.9.8/hagworm/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1291 2023-12-15 03:15:06.000000 hagworm-5.9.8/hagworm/__init__.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:45.436345 hagworm-5.9.8/hagworm/extend/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-03-01 02:07:14.000000 hagworm-5.9.8/hagworm/extend/__init__.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:45.769350 hagworm-5.9.8/hagworm/extend/asyncio/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-03-01 02:07:14.000000 hagworm-5.9.8/hagworm/extend/asyncio/__init__.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)    11877 2023-11-27 06:23:10.000000 hagworm-5.9.8/hagworm/extend/asyncio/base.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3604 2023-11-18 08:33:48.000000 hagworm-5.9.8/hagworm/extend/asyncio/buffer.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2561 2023-11-27 08:55:49.000000 hagworm-5.9.8/hagworm/extend/asyncio/command.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3385 2023-11-18 08:16:32.000000 hagworm-5.9.8/hagworm/extend/asyncio/event.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1558 2023-11-25 01:52:39.000000 hagworm-5.9.8/hagworm/extend/asyncio/file.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     5484 2023-11-18 07:46:08.000000 hagworm-5.9.8/hagworm/extend/asyncio/future.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3077 2023-11-18 07:24:30.000000 hagworm-5.9.8/hagworm/extend/asyncio/mail.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3470 2023-11-25 01:58:29.000000 hagworm-5.9.8/hagworm/extend/asyncio/mongo.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)    10438 2023-11-25 05:19:55.000000 hagworm-5.9.8/hagworm/extend/asyncio/mysql.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)    10723 2023-11-25 01:58:41.000000 hagworm-5.9.8/hagworm/extend/asyncio/net.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     4533 2023-11-18 06:57:15.000000 hagworm-5.9.8/hagworm/extend/asyncio/ntp.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1445 2023-11-18 05:32:45.000000 hagworm-5.9.8/hagworm/extend/asyncio/pool.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)    12500 2023-11-18 08:52:57.000000 hagworm-5.9.8/hagworm/extend/asyncio/redis.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)    10439 2023-12-05 08:17:38.000000 hagworm-5.9.8/hagworm/extend/asyncio/socket.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     9805 2023-11-25 01:37:38.000000 hagworm-5.9.8/hagworm/extend/asyncio/task.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1360 2023-03-01 02:07:14.000000 hagworm-5.9.8/hagworm/extend/asyncio/transaction.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)    24841 2023-12-11 06:35:57.000000 hagworm-5.9.8/hagworm/extend/base.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2821 2023-11-20 07:56:14.000000 hagworm-5.9.8/hagworm/extend/cache.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1827 2023-11-20 07:20:35.000000 hagworm-5.9.8/hagworm/extend/compile.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     5346 2023-11-27 01:39:13.000000 hagworm-5.9.8/hagworm/extend/config.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1522 2023-11-25 02:01:03.000000 hagworm-5.9.8/hagworm/extend/crypto.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1538 2023-11-20 05:53:19.000000 hagworm-5.9.8/hagworm/extend/error.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1295 2023-11-25 01:29:46.000000 hagworm-5.9.8/hagworm/extend/event.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     4364 2023-11-25 02:01:33.000000 hagworm-5.9.8/hagworm/extend/igraph.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2255 2023-11-20 03:37:48.000000 hagworm-5.9.8/hagworm/extend/interface.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)    15456 2023-11-25 01:58:05.000000 hagworm-5.9.8/hagworm/extend/logging.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1928 2023-11-20 03:24:22.000000 hagworm-5.9.8/hagworm/extend/media.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1875 2023-11-28 02:49:50.000000 hagworm-5.9.8/hagworm/extend/metaclass.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     4630 2023-11-25 01:24:59.000000 hagworm-5.9.8/hagworm/extend/process.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)      606 2023-11-20 01:55:01.000000 hagworm-5.9.8/hagworm/extend/qrcode.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     7274 2023-12-02 06:37:24.000000 hagworm-5.9.8/hagworm/extend/struct.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3449 2023-11-20 01:38:33.000000 hagworm-5.9.8/hagworm/extend/text.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2549 2023-11-25 02:00:23.000000 hagworm-5.9.8/hagworm/extend/trace.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3007 2023-11-18 05:38:11.000000 hagworm-5.9.8/hagworm/extend/transaction.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     6613 2023-11-20 00:47:06.000000 hagworm-5.9.8/hagworm/extend/validator.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:45.812758 hagworm-5.9.8/hagworm/frame/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-03-01 02:07:14.000000 hagworm-5.9.8/hagworm/frame/__init__.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:45.914296 hagworm-5.9.8/hagworm/frame/fastapi/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-03-01 02:07:14.000000 hagworm-5.9.8/hagworm/frame/fastapi/__init__.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     7914 2023-12-11 06:31:39.000000 hagworm-5.9.8/hagworm/frame/fastapi/base.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3904 2023-12-02 06:11:53.000000 hagworm-5.9.8/hagworm/frame/fastapi/field.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1658 2023-11-30 05:01:31.000000 hagworm-5.9.8/hagworm/frame/fastapi/model.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1084 2023-11-18 05:32:45.000000 hagworm-5.9.8/hagworm/frame/fastapi/response.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1304 2023-11-18 05:32:45.000000 hagworm-5.9.8/hagworm/frame/gunicorn.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     4343 2023-11-27 07:32:31.000000 hagworm-5.9.8/hagworm/frame/stress_tests.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:45.934296 hagworm-5.9.8/hagworm/third/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-03-01 02:07:14.000000 hagworm-5.9.8/hagworm/third/__init__.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:45.999815 hagworm-5.9.8/hagworm/third/grpc/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)       61 2023-06-07 06:33:27.000000 hagworm-5.9.8/hagworm/third/grpc/__init__.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     8257 2023-11-25 01:29:12.000000 hagworm-5.9.8/hagworm/third/grpc/client.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     4912 2023-11-21 01:26:22.000000 hagworm-5.9.8/hagworm/third/grpc/server.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:46.066817 hagworm-5.9.8/hagworm/third/nacos/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-10-25 02:03:54.000000 hagworm-5.9.8/hagworm/third/nacos/__init__.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)    11473 2023-11-20 09:46:13.000000 hagworm-5.9.8/hagworm/third/nacos/client.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1352 2023-11-18 05:32:45.000000 hagworm-5.9.8/hagworm/third/nacos/config.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:46.155329 hagworm-5.9.8/hagworm/third/rabbitmq/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)      452 2023-11-29 02:38:25.000000 hagworm-5.9.8/hagworm/third/rabbitmq/__init__.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3982 2023-11-18 05:32:45.000000 hagworm-5.9.8/hagworm/third/rabbitmq/consume.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     5219 2023-11-21 09:26:07.000000 hagworm-5.9.8/hagworm/third/rabbitmq/publish.py
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     6776 2023-11-18 05:32:45.000000 hagworm-5.9.8/hagworm/third/rabbitmq/rpc.py
-drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 03:15:45.076709 hagworm-5.9.8/hagworm.egg-info/
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     5979 2023-12-15 03:15:44.000000 hagworm-5.9.8/hagworm.egg-info/PKG-INFO
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2200 2023-12-15 03:15:44.000000 hagworm-5.9.8/hagworm.egg-info/SOURCES.txt
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)        1 2023-12-15 03:15:44.000000 hagworm-5.9.8/hagworm.egg-info/dependency_links.txt
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)      669 2023-12-15 03:15:44.000000 hagworm-5.9.8/hagworm.egg-info/requires.txt
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)       16 2023-12-15 03:15:44.000000 hagworm-5.9.8/hagworm.egg-info/top_level.txt
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)       38 2023-12-15 03:15:46.177331 hagworm-5.9.8/setup.cfg
--rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1976 2023-12-15 03:13:46.000000 hagworm-5.9.8/setup.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:37.845627 hagworm-5.9.9/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)    11362 2023-03-01 02:07:14.000000 hagworm-5.9.9/LICENSE
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     5979 2023-12-15 04:33:37.843626 hagworm-5.9.9/PKG-INFO
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     5502 2023-11-18 05:32:45.000000 hagworm-5.9.9/README.md
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:36.656475 hagworm-5.9.9/example/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-03-01 02:07:14.000000 hagworm-5.9.9/example/__init__.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:36.710007 hagworm-5.9.9/example/fastapi_demo/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)       61 2023-05-26 07:33:49.000000 hagworm-5.9.9/example/fastapi_demo/__init__.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:36.743525 hagworm-5.9.9/example/fastapi_demo/controller/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)      211 2023-11-18 05:32:45.000000 hagworm-5.9.9/example/fastapi_demo/controller/__init__.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)      397 2023-11-23 00:48:29.000000 hagworm-5.9.9/example/fastapi_demo/controller/home.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)      860 2023-11-18 05:32:45.000000 hagworm-5.9.9/example/fastapi_demo/gunicorn.config.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1245 2023-11-18 05:32:45.000000 hagworm-5.9.9/example/fastapi_demo/main.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:36.760155 hagworm-5.9.9/example/fastapi_demo/model/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)       61 2023-05-26 07:33:49.000000 hagworm-5.9.9/example/fastapi_demo/model/__init__.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:36.777664 hagworm-5.9.9/example/fastapi_demo/service/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2609 2023-11-18 05:32:45.000000 hagworm-5.9.9/example/fastapi_demo/service/__init__.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2041 2023-11-18 05:32:45.000000 hagworm-5.9.9/example/fastapi_demo/setting.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1095 2023-11-18 05:32:45.000000 hagworm-5.9.9/example/main_tcp.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)      801 2023-11-27 09:37:15.000000 hagworm-5.9.9/example/main_test.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:36.790664 hagworm-5.9.9/hagworm/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1291 2023-12-15 03:29:33.000000 hagworm-5.9.9/hagworm/__init__.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:37.146896 hagworm-5.9.9/hagworm/extend/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-03-01 02:07:14.000000 hagworm-5.9.9/hagworm/extend/__init__.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:37.475475 hagworm-5.9.9/hagworm/extend/asyncio/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-03-01 02:07:14.000000 hagworm-5.9.9/hagworm/extend/asyncio/__init__.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)    11877 2023-11-27 06:23:10.000000 hagworm-5.9.9/hagworm/extend/asyncio/base.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3601 2023-12-15 03:20:38.000000 hagworm-5.9.9/hagworm/extend/asyncio/buffer.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2561 2023-11-27 08:55:49.000000 hagworm-5.9.9/hagworm/extend/asyncio/command.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3385 2023-11-18 08:16:32.000000 hagworm-5.9.9/hagworm/extend/asyncio/event.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1558 2023-11-25 01:52:39.000000 hagworm-5.9.9/hagworm/extend/asyncio/file.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     5484 2023-11-18 07:46:08.000000 hagworm-5.9.9/hagworm/extend/asyncio/future.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3077 2023-11-18 07:24:30.000000 hagworm-5.9.9/hagworm/extend/asyncio/mail.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3470 2023-11-25 01:58:29.000000 hagworm-5.9.9/hagworm/extend/asyncio/mongo.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)    10438 2023-11-25 05:19:55.000000 hagworm-5.9.9/hagworm/extend/asyncio/mysql.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)    10723 2023-11-25 01:58:41.000000 hagworm-5.9.9/hagworm/extend/asyncio/net.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     4533 2023-11-18 06:57:15.000000 hagworm-5.9.9/hagworm/extend/asyncio/ntp.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1445 2023-11-18 05:32:45.000000 hagworm-5.9.9/hagworm/extend/asyncio/pool.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)    12500 2023-11-18 08:52:57.000000 hagworm-5.9.9/hagworm/extend/asyncio/redis.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)    10439 2023-12-05 08:17:38.000000 hagworm-5.9.9/hagworm/extend/asyncio/socket.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     9805 2023-11-25 01:37:38.000000 hagworm-5.9.9/hagworm/extend/asyncio/task.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1360 2023-03-01 02:07:14.000000 hagworm-5.9.9/hagworm/extend/asyncio/transaction.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)    24841 2023-12-11 06:35:57.000000 hagworm-5.9.9/hagworm/extend/base.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2821 2023-11-20 07:56:14.000000 hagworm-5.9.9/hagworm/extend/cache.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1827 2023-11-20 07:20:35.000000 hagworm-5.9.9/hagworm/extend/compile.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     5346 2023-11-27 01:39:13.000000 hagworm-5.9.9/hagworm/extend/config.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1522 2023-11-25 02:01:03.000000 hagworm-5.9.9/hagworm/extend/crypto.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1538 2023-11-20 05:53:19.000000 hagworm-5.9.9/hagworm/extend/error.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1295 2023-11-25 01:29:46.000000 hagworm-5.9.9/hagworm/extend/event.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     4364 2023-11-25 02:01:33.000000 hagworm-5.9.9/hagworm/extend/igraph.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2255 2023-11-20 03:37:48.000000 hagworm-5.9.9/hagworm/extend/interface.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)    15456 2023-11-25 01:58:05.000000 hagworm-5.9.9/hagworm/extend/logging.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1928 2023-11-20 03:24:22.000000 hagworm-5.9.9/hagworm/extend/media.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1875 2023-11-28 02:49:50.000000 hagworm-5.9.9/hagworm/extend/metaclass.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     4630 2023-11-25 01:24:59.000000 hagworm-5.9.9/hagworm/extend/process.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)      606 2023-11-20 01:55:01.000000 hagworm-5.9.9/hagworm/extend/qrcode.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     7274 2023-12-02 06:37:24.000000 hagworm-5.9.9/hagworm/extend/struct.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3449 2023-11-20 01:38:33.000000 hagworm-5.9.9/hagworm/extend/text.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2549 2023-11-25 02:00:23.000000 hagworm-5.9.9/hagworm/extend/trace.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3007 2023-11-18 05:38:11.000000 hagworm-5.9.9/hagworm/extend/transaction.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     6613 2023-11-20 00:47:06.000000 hagworm-5.9.9/hagworm/extend/validator.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:37.516064 hagworm-5.9.9/hagworm/frame/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-03-01 02:07:14.000000 hagworm-5.9.9/hagworm/frame/__init__.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:37.602118 hagworm-5.9.9/hagworm/frame/fastapi/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-03-01 02:07:14.000000 hagworm-5.9.9/hagworm/frame/fastapi/__init__.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     7914 2023-12-11 06:31:39.000000 hagworm-5.9.9/hagworm/frame/fastapi/base.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3904 2023-12-02 06:11:53.000000 hagworm-5.9.9/hagworm/frame/fastapi/field.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1658 2023-11-30 05:01:31.000000 hagworm-5.9.9/hagworm/frame/fastapi/model.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1084 2023-11-18 05:32:45.000000 hagworm-5.9.9/hagworm/frame/fastapi/response.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1304 2023-11-18 05:32:45.000000 hagworm-5.9.9/hagworm/frame/gunicorn.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     4343 2023-11-27 07:32:31.000000 hagworm-5.9.9/hagworm/frame/stress_tests.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:37.616177 hagworm-5.9.9/hagworm/third/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-03-01 02:07:14.000000 hagworm-5.9.9/hagworm/third/__init__.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:37.673537 hagworm-5.9.9/hagworm/third/grpc/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)       61 2023-06-07 06:33:27.000000 hagworm-5.9.9/hagworm/third/grpc/__init__.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     8257 2023-11-25 01:29:12.000000 hagworm-5.9.9/hagworm/third/grpc/client.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     4912 2023-11-21 01:26:22.000000 hagworm-5.9.9/hagworm/third/grpc/server.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:37.738542 hagworm-5.9.9/hagworm/third/nacos/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)       58 2023-10-25 02:03:54.000000 hagworm-5.9.9/hagworm/third/nacos/__init__.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)    11473 2023-11-20 09:46:13.000000 hagworm-5.9.9/hagworm/third/nacos/client.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1352 2023-11-18 05:32:45.000000 hagworm-5.9.9/hagworm/third/nacos/config.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:37.825621 hagworm-5.9.9/hagworm/third/rabbitmq/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)      452 2023-11-29 02:38:25.000000 hagworm-5.9.9/hagworm/third/rabbitmq/__init__.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     3982 2023-11-18 05:32:45.000000 hagworm-5.9.9/hagworm/third/rabbitmq/consume.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     5219 2023-11-21 09:26:07.000000 hagworm-5.9.9/hagworm/third/rabbitmq/publish.py
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     6776 2023-11-18 05:32:45.000000 hagworm-5.9.9/hagworm/third/rabbitmq/rpc.py
+drwxrwxrwx   0 wsb       (1000) wsb       (1000)        0 2023-12-15 04:33:36.857692 hagworm-5.9.9/hagworm.egg-info/
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     5979 2023-12-15 04:33:36.000000 hagworm-5.9.9/hagworm.egg-info/PKG-INFO
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     2200 2023-12-15 04:33:36.000000 hagworm-5.9.9/hagworm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)        1 2023-12-15 04:33:36.000000 hagworm-5.9.9/hagworm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)      669 2023-12-15 04:33:36.000000 hagworm-5.9.9/hagworm.egg-info/requires.txt
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)       16 2023-12-15 04:33:36.000000 hagworm-5.9.9/hagworm.egg-info/top_level.txt
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)       38 2023-12-15 04:33:37.846625 hagworm-5.9.9/setup.cfg
+-rwxrwxrwx   0 wsb       (1000) wsb       (1000)     1976 2023-12-15 03:13:46.000000 hagworm-5.9.9/setup.py
```

### Comparing `hagworm-5.9.8/LICENSE` & `hagworm-5.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/PKG-INFO` & `hagworm-5.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.9.8
+Version: 5.9.9
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Platform: all
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hagworm-5.9.8/README.md` & `hagworm-5.9.9/README.md`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/example/fastapi_demo/gunicorn.config.py` & `hagworm-5.9.9/example/fastapi_demo/gunicorn.config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/example/fastapi_demo/main.py` & `hagworm-5.9.9/example/fastapi_demo/main.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/example/fastapi_demo/service/__init__.py` & `hagworm-5.9.9/example/fastapi_demo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/example/fastapi_demo/setting.py` & `hagworm-5.9.9/example/fastapi_demo/setting.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/example/main_tcp.py` & `hagworm-5.9.9/example/main_tcp.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/example/main_test.py` & `hagworm-5.9.9/example/main_test.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/__init__.py` & `hagworm-5.9.9/hagworm/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 __author__ = r'wsb310@gmail.com'
 
-__version__ = r'5.9.8'
+__version__ = r'5.9.9'
 
 hagworm_label = f'Hagworm v{__version__}'
 
 hagworm_slogan = f'''
 \033[48;2;255;13;104m                                                                    \033[0m
 \033[38;2;255;255;255;48;2;255;13;104m   ██   ██  █████   ██████  ██     ██  ██████  ██████  ███    ███   \033[0m
 \033[38;2;255;255;255;48;2;255;13;104m   ██   ██ ██   ██ ██       ██     ██ ██    ██ ██   ██ ████  ████   \033[0m
```

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/base.py` & `hagworm-5.9.9/hagworm/extend/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/buffer.py` & `hagworm-5.9.9/hagworm/extend/asyncio/buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
                 raise err
 
             except Exception as err:
 
                 Utils.log.error(str(err))
 
-    async def append(self, data: typing.Any, timeout: typing.Optional[int, float] = None):
+    async def append(self, data: typing.Any, timeout: typing.Union[int, float] = None):
 
         await asyncio.wait_for(
             self._slice_data.put(data),
             timeout
         )
 
         if self._slice_data.qsize() >= self._slice_size:
```

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/command.py` & `hagworm-5.9.9/hagworm/extend/asyncio/command.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/event.py` & `hagworm-5.9.9/hagworm/extend/asyncio/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/file.py` & `hagworm-5.9.9/hagworm/extend/asyncio/file.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/future.py` & `hagworm-5.9.9/hagworm/extend/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/mail.py` & `hagworm-5.9.9/hagworm/extend/asyncio/mail.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/mongo.py` & `hagworm-5.9.9/hagworm/extend/asyncio/mongo.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/mysql.py` & `hagworm-5.9.9/hagworm/extend/asyncio/mysql.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/net.py` & `hagworm-5.9.9/hagworm/extend/asyncio/net.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/ntp.py` & `hagworm-5.9.9/hagworm/extend/asyncio/ntp.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/pool.py` & `hagworm-5.9.9/hagworm/extend/asyncio/pool.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/redis.py` & `hagworm-5.9.9/hagworm/extend/asyncio/redis.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/socket.py` & `hagworm-5.9.9/hagworm/extend/asyncio/socket.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/task.py` & `hagworm-5.9.9/hagworm/extend/asyncio/task.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/asyncio/transaction.py` & `hagworm-5.9.9/hagworm/extend/asyncio/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/base.py` & `hagworm-5.9.9/hagworm/extend/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/cache.py` & `hagworm-5.9.9/hagworm/extend/cache.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/compile.py` & `hagworm-5.9.9/hagworm/extend/compile.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/config.py` & `hagworm-5.9.9/hagworm/extend/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/crypto.py` & `hagworm-5.9.9/hagworm/extend/crypto.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/error.py` & `hagworm-5.9.9/hagworm/extend/error.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/event.py` & `hagworm-5.9.9/hagworm/extend/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/igraph.py` & `hagworm-5.9.9/hagworm/extend/igraph.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/interface.py` & `hagworm-5.9.9/hagworm/extend/interface.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/logging.py` & `hagworm-5.9.9/hagworm/extend/logging.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/media.py` & `hagworm-5.9.9/hagworm/extend/media.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/metaclass.py` & `hagworm-5.9.9/hagworm/extend/metaclass.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/process.py` & `hagworm-5.9.9/hagworm/extend/process.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/qrcode.py` & `hagworm-5.9.9/hagworm/extend/qrcode.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/struct.py` & `hagworm-5.9.9/hagworm/extend/struct.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/text.py` & `hagworm-5.9.9/hagworm/extend/text.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/trace.py` & `hagworm-5.9.9/hagworm/extend/trace.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/transaction.py` & `hagworm-5.9.9/hagworm/extend/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/extend/validator.py` & `hagworm-5.9.9/hagworm/extend/validator.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/frame/fastapi/base.py` & `hagworm-5.9.9/hagworm/frame/fastapi/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/frame/fastapi/field.py` & `hagworm-5.9.9/hagworm/frame/fastapi/field.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/frame/fastapi/model.py` & `hagworm-5.9.9/hagworm/frame/fastapi/model.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/frame/fastapi/response.py` & `hagworm-5.9.9/hagworm/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/frame/gunicorn.py` & `hagworm-5.9.9/hagworm/frame/gunicorn.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/frame/stress_tests.py` & `hagworm-5.9.9/hagworm/frame/stress_tests.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/third/grpc/client.py` & `hagworm-5.9.9/hagworm/third/grpc/client.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/third/grpc/server.py` & `hagworm-5.9.9/hagworm/third/grpc/server.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/third/nacos/client.py` & `hagworm-5.9.9/hagworm/third/nacos/client.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/third/nacos/config.py` & `hagworm-5.9.9/hagworm/third/nacos/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/third/rabbitmq/consume.py` & `hagworm-5.9.9/hagworm/third/rabbitmq/consume.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/third/rabbitmq/publish.py` & `hagworm-5.9.9/hagworm/third/rabbitmq/publish.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm/third/rabbitmq/rpc.py` & `hagworm-5.9.9/hagworm/third/rabbitmq/rpc.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm.egg-info/PKG-INFO` & `hagworm-5.9.9/hagworm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.9.8
+Version: 5.9.9
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Platform: all
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hagworm-5.9.8/hagworm.egg-info/SOURCES.txt` & `hagworm-5.9.9/hagworm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/hagworm.egg-info/requires.txt` & `hagworm-5.9.9/hagworm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.9.8/setup.py` & `hagworm-5.9.9/setup.py`

 * *Files identical despite different names*

