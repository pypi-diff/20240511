# Comparing `tmp/duwi_smart_sdk-0.2.4.tar.gz` & `tmp/duwi_smart_sdk-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.2.4.tar", last modified: Fri May 10 01:28:58 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.2.5.tar", last modified: Sat May 11 03:23:12 2024, max compression
```

## Comparing `duwi_smart_sdk-0.2.4.tar` & `duwi_smart_sdk-0.2.5.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 01:28:58.818329 duwi_smart_sdk-0.2.4/
--rw-rw-rw-   0        0        0      885 2024-05-10 01:28:58.818329 duwi_smart_sdk-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-05-09 02:50:27.000000 duwi_smart_sdk-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 01:28:58.765428 duwi_smart_sdk-0.2.4/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:28:58.782628 duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     2063 2024-05-10 00:47:56.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/account.py
--rw-rw-rw-   0        0        0     1739 2024-05-10 00:48:21.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     4512 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2623 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/floor.py
--rw-rw-rw-   0        0        0     2651 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     2121 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     2731 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/room.py
--rw-rw-rw-   0        0        0     4768 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:28:58.787511 duwi_smart_sdk-0.2.4/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:28:58.788485 duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:28:58.790990 duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:28:58.798804 duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/resp/floor.py
--rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/resp/house.py
--rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/resp/room.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:28:58.803486 duwi_smart_sdk-0.2.4/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:28:58.773239 duwi_smart_sdk-0.2.4/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      885 2024-05-10 01:28:58.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1396 2024-05-10 01:28:58.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 01:28:58.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-10 01:28:58.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-10 01:28:58.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-10 01:28:58.000000 duwi_smart_sdk-0.2.4/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 01:28:58.819284 duwi_smart_sdk-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      936 2024-05-10 01:28:31.000000 duwi_smart_sdk-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:28:58.804463 duwi_smart_sdk-0.2.4/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.4/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:28:58.815376 duwi_smart_sdk-0.2.4/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.2.4/test/api/__init__.py
--rw-rw-rw-   0        0        0      948 2024-05-08 01:12:43.000000 duwi_smart_sdk-0.2.4/test/api/test_control.py
--rw-rw-rw-   0        0        0      813 2024-05-09 03:37:26.000000 duwi_smart_sdk-0.2.4/test/api/test_discover.py
--rw-rw-rw-   0        0        0      780 2024-05-09 07:45:49.000000 duwi_smart_sdk-0.2.4/test/api/test_floor.py
--rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.2.4/test/api/test_house.py
--rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.2.4/test/api/test_login.py
--rw-rw-rw-   0        0        0      724 2024-05-09 07:16:53.000000 duwi_smart_sdk-0.2.4/test/api/test_room.py
--rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.2.4/test/api/test_ws.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:28:58.817330 duwi_smart_sdk-0.2.4/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.4/test/util/__init__.py
--rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.2.4/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:23:12.747760 duwi_smart_sdk-0.2.5/
+-rw-rw-rw-   0        0        0      900 2024-05-11 03:23:12.746756 duwi_smart_sdk-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-05-10 01:36:43.000000 duwi_smart_sdk-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 03:23:12.696449 duwi_smart_sdk-0.2.5/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:23:12.713766 duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     2441 2024-05-11 03:12:54.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/account.py
+-rw-rw-rw-   0        0        0     1739 2024-05-10 00:48:21.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     4512 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2623 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/floor.py
+-rw-rw-rw-   0        0        0     2651 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     2121 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     2731 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/room.py
+-rw-rw-rw-   0        0        0     4768 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:23:12.718999 duwi_smart_sdk-0.2.5/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:23:12.719996 duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:23:12.721997 duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:23:12.729738 duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/resp/floor.py
+-rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/resp/house.py
+-rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/resp/room.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:23:12.733738 duwi_smart_sdk-0.2.5/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:23:12.745251 duwi_smart_sdk-0.2.5/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      900 2024-05-11 03:23:12.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1421 2024-05-11 03:23:12.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 03:23:12.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-11 03:23:12.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-11 03:23:12.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-11 03:23:12.000000 duwi_smart_sdk-0.2.5/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 03:23:12.747760 duwi_smart_sdk-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      936 2024-05-11 03:22:33.000000 duwi_smart_sdk-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:23:12.734738 duwi_smart_sdk-0.2.5/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.5/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:23:12.743252 duwi_smart_sdk-0.2.5/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.2.5/test/api/__init__.py
+-rw-rw-rw-   0        0        0      723 2024-05-11 03:19:03.000000 duwi_smart_sdk-0.2.5/test/api/test_account.py
+-rw-rw-rw-   0        0        0      948 2024-05-08 01:12:43.000000 duwi_smart_sdk-0.2.5/test/api/test_control.py
+-rw-rw-rw-   0        0        0      813 2024-05-09 03:37:26.000000 duwi_smart_sdk-0.2.5/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      780 2024-05-09 07:45:49.000000 duwi_smart_sdk-0.2.5/test/api/test_floor.py
+-rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.2.5/test/api/test_house.py
+-rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.2.5/test/api/test_login.py
+-rw-rw-rw-   0        0        0      724 2024-05-09 07:16:53.000000 duwi_smart_sdk-0.2.5/test/api/test_room.py
+-rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.2.5/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:23:12.745251 duwi_smart_sdk-0.2.5/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.5/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.2.5/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.2.4/PKG-INFO` & `duwi_smart_sdk-0.2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.2.4
+Version: 0.2.5
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+Requires-Dist: websockets
+Requires-Dist: aiohttp
 
 install sdk
 ```shell
 pip install duwi-smart-sdk
 ```
 
 Update existing dependencies
 ```shell
 pip install --upgrade duwi-smart-sdk
 ```
 
 token 
 ```txt
-pypi-AgEIcHlwaS5vcmcCJDI3MzRiNTIxLWJlZDItNDRkOS05MDE3LTUwZWU4MWYzOWUxOAACFlsxLFsiZHV3aS1zbWFydC1zZGsiXV0AAixbMixbIjc3ZDI4OTZlLTZjNDItNDNmNy04YzhmLTAyYTdkZTU1MDAyYyJdXQAABiDUtvKJ8ubT31ZBAWErsXvQKGJ4jWpbn_XYvLgGu04NbA
+pypi-AgEIcHlwaS5vcmcCJDUyMDJlZGQwLTFlNmItNGVlOS05NDJlLWQwYzQ2YmFiYjhkNAACKlszLCJjZGM0YzM1My1mY2JkLTQ0ZjMtYjlmYS02ZDIyYTNkNmM4MjgiXQAABiAyj3lns3YOwHEf6xDCkwpwtknlR791kwAOy8JWcuxZhA
 ```
```

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/account.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/account.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,24 @@
         self._url = URL
         self._app_key = app_key
         self._app_secret = app_secret
         self._app_version = app_version
         self._client_version = client_version
         self._client_model = client_model
 
+    async def auth(self, app_key: str, app_secret: str) -> tuple[str, AuthToken | None]:
+        self._app_key = app_key
+        self._app_secret = app_secret
+        status, auth_token = await self.login("", "")
+
+        if status == Code.LOGIN_ERROR.value:
+            return Code.SUCCESS.value, None
+        else:
+            return Code.APP_KEY_ERROR.value, None
+
     async def login(self, phone: str, password: str) -> tuple[str, AuthToken | None]:
         # 更新body的内容，传入phone和password
         body = {
             "phone": phone,
             "password": password,
         }
         body_string = json.dumps(body, separators=(',', ':'))
```

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/floor.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/room.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/const/status.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/resp/floor.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/resp/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/model/resp/room.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/model/resp/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
-Name: duwi-smart-sdk
-Version: 0.2.4
+Name: duwi_smart_sdk
+Version: 0.2.5
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+Requires-Dist: websockets
+Requires-Dist: aiohttp
 
 install sdk
 ```shell
 pip install duwi-smart-sdk
 ```
 
 Update existing dependencies
 ```shell
 pip install --upgrade duwi-smart-sdk
 ```
 
 token 
 ```txt
-pypi-AgEIcHlwaS5vcmcCJDI3MzRiNTIxLWJlZDItNDRkOS05MDE3LTUwZWU4MWYzOWUxOAACFlsxLFsiZHV3aS1zbWFydC1zZGsiXV0AAixbMixbIjc3ZDI4OTZlLTZjNDItNDNmNy04YzhmLTAyYTdkZTU1MDAyYyJdXQAABiDUtvKJ8ubT31ZBAWErsXvQKGJ4jWpbn_XYvLgGu04NbA
+pypi-AgEIcHlwaS5vcmcCJDUyMDJlZGQwLTFlNmItNGVlOS05NDJlLWQwYzQ2YmFiYjhkNAACKlszLCJjZGM0YzM1My1mY2JkLTQ0ZjMtYjlmYS02ZDIyYTNkNmM4MjgiXQAABiAyj3lns3YOwHEf6xDCkwpwtknlR791kwAOy8JWcuxZhA
 ```
```

### Comparing `duwi_smart_sdk-0.2.4/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.2.5/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 duwi_smart_sdk/model/resp/room.py
 duwi_smart_sdk/util/__init__.py
 duwi_smart_sdk/util/http.py
 duwi_smart_sdk/util/sign.py
 duwi_smart_sdk/util/timestamp.py
 test/__init__.py
 test/api/__init__.py
+test/api/test_account.py
 test/api/test_control.py
 test/api/test_discover.py
 test/api/test_floor.py
 test/api/test_house.py
 test/api/test_login.py
 test/api/test_room.py
 test/api/test_ws.py
```

### Comparing `duwi_smart_sdk-0.2.4/setup.py` & `duwi_smart_sdk-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.4'
+VERSION = '0.2.5'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.2.4/test/api/test_control.py` & `duwi_smart_sdk-0.2.5/test/api/test_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/test/api/test_discover.py` & `duwi_smart_sdk-0.2.5/test/api/test_discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/test/api/test_floor.py` & `duwi_smart_sdk-0.2.5/test/api/test_floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/test/api/test_house.py` & `duwi_smart_sdk-0.2.5/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/test/api/test_login.py` & `duwi_smart_sdk-0.2.5/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/test/api/test_room.py` & `duwi_smart_sdk-0.2.5/test/api/test_room.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/test/api/test_ws.py` & `duwi_smart_sdk-0.2.5/test/api/test_ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.4/test/util/test_http.py` & `duwi_smart_sdk-0.2.5/test/util/test_http.py`

 * *Files identical despite different names*

