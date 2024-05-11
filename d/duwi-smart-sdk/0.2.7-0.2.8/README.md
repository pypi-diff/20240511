# Comparing `tmp/duwi_smart_sdk-0.2.7.tar.gz` & `tmp/duwi_smart_sdk-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.2.7.tar", last modified: Sat May 11 04:12:07 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.2.8.tar", last modified: Sat May 11 04:16:43 2024, max compression
```

## Comparing `duwi_smart_sdk-0.2.7.tar` & `duwi_smart_sdk-0.2.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 04:12:07.001564 duwi_smart_sdk-0.2.7/
--rw-rw-rw-   0        0        0      900 2024-05-11 04:12:07.000564 duwi_smart_sdk-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-05-10 01:36:43.000000 duwi_smart_sdk-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 04:12:06.948707 duwi_smart_sdk-0.2.7/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 04:12:06.966878 duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     2443 2024-05-11 04:09:56.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/account.py
--rw-rw-rw-   0        0        0     1739 2024-05-10 00:48:21.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     4512 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2623 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/floor.py
--rw-rw-rw-   0        0        0     2651 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     2121 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     2731 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/room.py
--rw-rw-rw-   0        0        0     4768 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-11 04:12:06.971380 duwi_smart_sdk-0.2.7/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-11 04:12:06.972380 duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 04:12:06.974380 duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-11 04:12:06.982542 duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/resp/floor.py
--rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/resp/house.py
--rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/resp/room.py
-drwxrwxrwx   0        0        0        0 2024-05-11 04:12:06.986542 duwi_smart_sdk-0.2.7/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-11 04:12:06.999564 duwi_smart_sdk-0.2.7/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      900 2024-05-11 04:12:06.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1421 2024-05-11 04:12:06.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 04:12:06.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-11 04:12:06.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-11 04:12:06.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-11 04:12:06.000000 duwi_smart_sdk-0.2.7/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 04:12:07.001564 duwi_smart_sdk-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      936 2024-05-11 04:11:28.000000 duwi_smart_sdk-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-11 04:12:06.987542 duwi_smart_sdk-0.2.7/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.7/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 04:12:06.997053 duwi_smart_sdk-0.2.7/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.2.7/test/api/__init__.py
--rw-rw-rw-   0        0        0      723 2024-05-11 03:19:03.000000 duwi_smart_sdk-0.2.7/test/api/test_account.py
--rw-rw-rw-   0        0        0      948 2024-05-08 01:12:43.000000 duwi_smart_sdk-0.2.7/test/api/test_control.py
--rw-rw-rw-   0        0        0      813 2024-05-09 03:37:26.000000 duwi_smart_sdk-0.2.7/test/api/test_discover.py
--rw-rw-rw-   0        0        0      780 2024-05-09 07:45:49.000000 duwi_smart_sdk-0.2.7/test/api/test_floor.py
--rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.2.7/test/api/test_house.py
--rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.2.7/test/api/test_login.py
--rw-rw-rw-   0        0        0      724 2024-05-09 07:16:53.000000 duwi_smart_sdk-0.2.7/test/api/test_room.py
--rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.2.7/test/api/test_ws.py
-drwxrwxrwx   0        0        0        0 2024-05-11 04:12:06.998558 duwi_smart_sdk-0.2.7/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.7/test/util/__init__.py
--rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.2.7/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:16:43.720950 duwi_smart_sdk-0.2.8/
+-rw-rw-rw-   0        0        0      900 2024-05-11 04:16:43.718994 duwi_smart_sdk-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-05-10 01:36:43.000000 duwi_smart_sdk-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 04:16:43.647849 duwi_smart_sdk-0.2.8/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:16:43.675863 duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     2441 2024-05-11 04:16:06.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/account.py
+-rw-rw-rw-   0        0        0     1739 2024-05-10 00:48:21.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     4512 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2623 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/floor.py
+-rw-rw-rw-   0        0        0     2651 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     2121 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     2731 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/room.py
+-rw-rw-rw-   0        0        0     4768 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:16:43.680888 duwi_smart_sdk-0.2.8/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:16:43.681888 duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:16:43.683889 duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:16:43.694397 duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/resp/floor.py
+-rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/resp/house.py
+-rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/resp/room.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:16:43.699913 duwi_smart_sdk-0.2.8/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:16:43.717429 duwi_smart_sdk-0.2.8/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      900 2024-05-11 04:16:43.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1421 2024-05-11 04:16:43.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 04:16:43.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-11 04:16:43.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-11 04:16:43.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-11 04:16:43.000000 duwi_smart_sdk-0.2.8/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 04:16:43.720950 duwi_smart_sdk-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      936 2024-05-11 04:16:35.000000 duwi_smart_sdk-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:16:43.701910 duwi_smart_sdk-0.2.8/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.8/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:16:43.714429 duwi_smart_sdk-0.2.8/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.2.8/test/api/__init__.py
+-rw-rw-rw-   0        0        0      723 2024-05-11 03:19:03.000000 duwi_smart_sdk-0.2.8/test/api/test_account.py
+-rw-rw-rw-   0        0        0      948 2024-05-08 01:12:43.000000 duwi_smart_sdk-0.2.8/test/api/test_control.py
+-rw-rw-rw-   0        0        0      813 2024-05-09 03:37:26.000000 duwi_smart_sdk-0.2.8/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      780 2024-05-09 07:45:49.000000 duwi_smart_sdk-0.2.8/test/api/test_floor.py
+-rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.2.8/test/api/test_house.py
+-rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.2.8/test/api/test_login.py
+-rw-rw-rw-   0        0        0      724 2024-05-09 07:16:53.000000 duwi_smart_sdk-0.2.8/test/api/test_room.py
+-rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.2.8/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:16:43.716439 duwi_smart_sdk-0.2.8/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.8/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.2.8/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.2.7/PKG-INFO` & `duwi_smart_sdk-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.2.7
+Version: 0.2.8
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/account.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,22 +22,22 @@
         self._app_version = app_version
         self._client_version = client_version
         self._client_model = client_model
 
     async def auth(self, app_key: str, app_secret: str) -> tuple[str, AuthToken | None]:
         self._app_key = app_key
         self._app_secret = app_secret
-        status, auth_token = await self.login2("", "")
+        status, auth_token = await self.login("", "")
 
         if status == Code.LOGIN_ERROR.value:
             return Code.SUCCESS.value, None
         else:
             return Code.APP_KEY_ERROR.value, None
 
-    async def login2(self, phone: str, password: str) -> tuple[str, AuthToken | None]:
+    async def login(self, phone: str, password: str) -> tuple[str, AuthToken | None]:
         # 更新body的内容，传入phone和password
         body = {
             "phone": phone,
             "password": password,
         }
         body_string = json.dumps(body, separators=(',', ':'))
         sign = md5_encrypt(body_string + self._app_secret + str(current_timestamp()))
```

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/floor.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/room.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/const/status.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/resp/floor.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/resp/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/model/resp/room.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/model/resp/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.2.7
+Version: 0.2.8
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.2.7/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.2.8/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/setup.py` & `duwi_smart_sdk-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.7'
+VERSION = '0.2.8'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.2.7/test/api/test_account.py` & `duwi_smart_sdk-0.2.8/test/api/test_account.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/test/api/test_control.py` & `duwi_smart_sdk-0.2.8/test/api/test_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/test/api/test_discover.py` & `duwi_smart_sdk-0.2.8/test/api/test_discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/test/api/test_floor.py` & `duwi_smart_sdk-0.2.8/test/api/test_floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/test/api/test_house.py` & `duwi_smart_sdk-0.2.8/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/test/api/test_login.py` & `duwi_smart_sdk-0.2.8/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/test/api/test_room.py` & `duwi_smart_sdk-0.2.8/test/api/test_room.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/test/api/test_ws.py` & `duwi_smart_sdk-0.2.8/test/api/test_ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.7/test/util/test_http.py` & `duwi_smart_sdk-0.2.8/test/util/test_http.py`

 * *Files identical despite different names*

