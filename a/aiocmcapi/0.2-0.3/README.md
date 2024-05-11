# Comparing `tmp/aiocmcapi-0.2.tar.gz` & `tmp/aiocmcapi-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocmcapi-0.2.tar", last modified: Sat May 11 21:37:46 2024, max compression
+gzip compressed data, was "aiocmcapi-0.3.tar", last modified: Sat May 11 21:41:42 2024, max compression
```

## Comparing `aiocmcapi-0.2.tar` & `aiocmcapi-0.3.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 21:37:46.019805 aiocmcapi-0.2/
--rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.2/LICENSE
--rw-rw-rw-   0        0        0     2014 2024-05-11 21:37:46.018806 aiocmcapi-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2024-05-11 21:20:54.000000 aiocmcapi-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 21:37:46.018806 aiocmcapi-0.2/aiocmcapi.egg-info/
--rw-rw-rw-   0        0        0     2014 2024-05-11 21:37:45.000000 aiocmcapi-0.2/aiocmcapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2024-05-11 21:37:46.000000 aiocmcapi-0.2/aiocmcapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 21:37:46.000000 aiocmcapi-0.2/aiocmcapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-11 21:37:46.000000 aiocmcapi-0.2/aiocmcapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      368 2024-05-11 21:37:40.000000 aiocmcapi-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 21:37:46.019805 aiocmcapi-0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 21:41:42.816321 aiocmcapi-0.3/
+-rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.3/LICENSE
+-rw-rw-rw-   0        0        0     2014 2024-05-11 21:41:42.815320 aiocmcapi-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2024-05-11 21:20:54.000000 aiocmcapi-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 21:41:42.811322 aiocmcapi-0.3/aiocmcapi/
+-rw-rw-rw-   0        0        0       61 2024-05-11 21:41:23.000000 aiocmcapi-0.3/aiocmcapi/__init__.py
+-rw-rw-rw-   0        0        0      748 2024-05-11 19:22:47.000000 aiocmcapi-0.3/aiocmcapi/client.py
+-rw-rw-rw-   0        0        0      922 2024-05-11 21:33:51.000000 aiocmcapi-0.3/aiocmcapi/currency.py
+drwxrwxrwx   0        0        0        0 2024-05-11 21:41:42.815320 aiocmcapi-0.3/aiocmcapi.egg-info/
+-rw-rw-rw-   0        0        0     2014 2024-05-11 21:41:42.000000 aiocmcapi-0.3/aiocmcapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-11 21:41:42.000000 aiocmcapi-0.3/aiocmcapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 21:41:42.000000 aiocmcapi-0.3/aiocmcapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-11 21:41:42.000000 aiocmcapi-0.3/aiocmcapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      368 2024-05-11 21:40:36.000000 aiocmcapi-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 21:41:42.816321 aiocmcapi-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      129 2024-05-11 21:40:33.000000 aiocmcapi-0.3/setup.py
```

### Comparing `aiocmcapi-0.2/LICENSE` & `aiocmcapi-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.2/PKG-INFO` & `aiocmcapi-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocmcapi
-Version: 0.2
+Version: 0.3
 Summary: Async wrapper for CoinMarketCap API
 Author-email: alobuzy <amozebus@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiocmcapi
```

### Comparing `aiocmcapi-0.2/README.md` & `aiocmcapi-0.3/README.md`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.2/aiocmcapi.egg-info/PKG-INFO` & `aiocmcapi-0.3/aiocmcapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocmcapi
-Version: 0.2
+Version: 0.3
 Summary: Async wrapper for CoinMarketCap API
 Author-email: alobuzy <amozebus@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiocmcapi
```

