# Comparing `tmp/market-engine-0.1.8.tar.gz` & `tmp/market-engine-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-engine-0.1.8.tar", last modified: Wed Jul 26 20:27:11 2023, max compression
+gzip compressed data, was "market-engine-0.1.9.tar", last modified: Wed Jul 26 20:28:43 2023, max compression
```

## Comparing `market-engine-0.1.8.tar` & `market-engine-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 20:27:11.307980 market-engine-0.1.8/
--rw-rw-rw-   0        0        0      216 2023-07-26 20:27:11.307980 market-engine-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 20:27:11.299978 market-engine-0.1.8/market_engine/
-drwxrwxrwx   0        0        0        0 2023-07-26 20:27:11.305477 market-engine-0.1.8/market_engine/API/
--rw-rw-rw-   0        0        0     3166 2023-07-25 21:19:06.000000 market-engine-0.1.8/market_engine/API/ManifestAPI.py
--rw-rw-rw-   0        0        0     6246 2023-07-26 20:21:41.000000 market-engine-0.1.8/market_engine/API/MarketAPI.py
--rw-rw-rw-   0        0        0     6633 2023-07-25 22:30:19.000000 market-engine-0.1.8/market_engine/API/RelicsRunAPI.py
--rw-rw-rw-   0        0        0        0 2023-07-24 20:09:05.000000 market-engine-0.1.8/market_engine/API/__init__.py
--rw-rw-rw-   0        0        0     7954 2023-07-26 01:21:00.000000 market-engine-0.1.8/market_engine/Common.py
--rw-rw-rw-   0        0        0    41618 2023-07-26 20:17:10.000000 market-engine-0.1.8/market_engine/ManifestParser.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:27:11.306976 market-engine-0.1.8/market_engine/Models/
--rw-rw-rw-   0        0        0    27054 2023-07-26 20:26:47.000000 market-engine-0.1.8/market_engine/Models/MarketDatabase.py
--rw-rw-rw-   0        0        0    12476 2023-07-26 19:57:21.000000 market-engine-0.1.8/market_engine/Models/MarketItem.py
--rw-rw-rw-   0        0        0     7066 2023-07-26 19:57:21.000000 market-engine-0.1.8/market_engine/Models/MarketUser.py
--rw-rw-rw-   0        0        0        0 2023-07-25 16:48:26.000000 market-engine-0.1.8/market_engine/Models/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.1.8/market_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 20:27:11.301977 market-engine-0.1.8/market_engine.egg-info/
--rw-rw-rw-   0        0        0      216 2023-07-26 20:27:11.000000 market-engine-0.1.8/market_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      544 2023-07-26 20:27:11.000000 market-engine-0.1.8/market_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 20:27:11.000000 market-engine-0.1.8/market_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      251 2023-07-26 20:27:11.000000 market-engine-0.1.8/market_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 20:27:11.000000 market-engine-0.1.8/market_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 20:27:11.307980 market-engine-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-07-26 20:27:05.000000 market-engine-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:28:43.064091 market-engine-0.1.9/
+-rw-rw-rw-   0        0        0      216 2023-07-26 20:28:43.063590 market-engine-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 20:28:43.058076 market-engine-0.1.9/market_engine/
+drwxrwxrwx   0        0        0        0 2023-07-26 20:28:43.062090 market-engine-0.1.9/market_engine/API/
+-rw-rw-rw-   0        0        0     3166 2023-07-25 21:19:06.000000 market-engine-0.1.9/market_engine/API/ManifestAPI.py
+-rw-rw-rw-   0        0        0     6246 2023-07-26 20:21:41.000000 market-engine-0.1.9/market_engine/API/MarketAPI.py
+-rw-rw-rw-   0        0        0     6633 2023-07-25 22:30:19.000000 market-engine-0.1.9/market_engine/API/RelicsRunAPI.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 20:09:05.000000 market-engine-0.1.9/market_engine/API/__init__.py
+-rw-rw-rw-   0        0        0     7954 2023-07-26 01:21:00.000000 market-engine-0.1.9/market_engine/Common.py
+-rw-rw-rw-   0        0        0    41618 2023-07-26 20:17:10.000000 market-engine-0.1.9/market_engine/ManifestParser.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:28:43.063090 market-engine-0.1.9/market_engine/Models/
+-rw-rw-rw-   0        0        0    27046 2023-07-26 20:28:22.000000 market-engine-0.1.9/market_engine/Models/MarketDatabase.py
+-rw-rw-rw-   0        0        0    12476 2023-07-26 19:57:21.000000 market-engine-0.1.9/market_engine/Models/MarketItem.py
+-rw-rw-rw-   0        0        0     7066 2023-07-26 19:57:21.000000 market-engine-0.1.9/market_engine/Models/MarketUser.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 16:48:26.000000 market-engine-0.1.9/market_engine/Models/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 19:06:03.000000 market-engine-0.1.9/market_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:28:43.060092 market-engine-0.1.9/market_engine.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-07-26 20:28:43.000000 market-engine-0.1.9/market_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      544 2023-07-26 20:28:43.000000 market-engine-0.1.9/market_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 20:28:43.000000 market-engine-0.1.9/market_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      251 2023-07-26 20:28:43.000000 market-engine-0.1.9/market_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 20:28:43.000000 market-engine-0.1.9/market_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 20:28:43.064091 market-engine-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-26 20:28:39.000000 market-engine-0.1.9/setup.py
```

### Comparing `market-engine-0.1.8/market_engine/API/ManifestAPI.py` & `market-engine-0.1.9/market_engine/API/ManifestAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.8/market_engine/API/MarketAPI.py` & `market-engine-0.1.9/market_engine/API/MarketAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.8/market_engine/API/RelicsRunAPI.py` & `market-engine-0.1.9/market_engine/API/RelicsRunAPI.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.8/market_engine/Common.py` & `market-engine-0.1.9/market_engine/Common.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.8/market_engine/ManifestParser.py` & `market-engine-0.1.9/market_engine/ManifestParser.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.8/market_engine/Models/MarketDatabase.py` & `market-engine-0.1.9/market_engine/Models/MarketDatabase.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
         """
         if items is None or item_ids is None:
             return
 
         data_list = [
             (item['id'], item['item_name'], item['url_name'], item['thumb'],
              item_info[item['id']]['mod_max_rank'])
-            for item in items if item in item['id'] in item_info]
+            for item in items if item['id'] in item_info]
 
         new_item_ids = {}
         for item, item_id in item_ids.items():
             if item_id not in [x['id'] for x in items]:
                 new_item_ids[item] = item_id
         data_list.extend([(new_item_ids[item], item, None, None, None) for item in new_item_ids])
```

### Comparing `market-engine-0.1.8/market_engine/Models/MarketItem.py` & `market-engine-0.1.9/market_engine/Models/MarketItem.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.8/market_engine/Models/MarketUser.py` & `market-engine-0.1.9/market_engine/Models/MarketUser.py`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.8/market_engine.egg-info/SOURCES.txt` & `market-engine-0.1.9/market_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `market-engine-0.1.8/setup.py` & `market-engine-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='market-engine',
-    version='0.1.8',
+    version='0.1.9',
     description='Engine for easily getting the orders, statistics, and other stats from warframe.market.',
     author='Jacob McBride',
     author_email='jake55111@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiohttp~=3.8.4',
         'discord~=2.2.2',
```

