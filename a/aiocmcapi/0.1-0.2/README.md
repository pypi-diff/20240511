# Comparing `tmp/aiocmcapi-0.1.tar.gz` & `tmp/aiocmcapi-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocmcapi-0.1.tar", last modified: Sat May 11 21:21:25 2024, max compression
+gzip compressed data, was "aiocmcapi-0.2.tar", last modified: Sat May 11 21:37:46 2024, max compression
```

## Comparing `aiocmcapi-0.1.tar` & `aiocmcapi-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 21:21:25.645000 aiocmcapi-0.1/
--rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.1/LICENSE
--rw-rw-rw-   0        0        0     2014 2024-05-11 21:21:25.644001 aiocmcapi-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2024-05-11 21:20:54.000000 aiocmcapi-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 21:21:25.643000 aiocmcapi-0.1/aiocmcapi.egg-info/
--rw-rw-rw-   0        0        0     2014 2024-05-11 21:21:25.000000 aiocmcapi-0.1/aiocmcapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2024-05-11 21:21:25.000000 aiocmcapi-0.1/aiocmcapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 21:21:25.000000 aiocmcapi-0.1/aiocmcapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-11 21:21:25.000000 aiocmcapi-0.1/aiocmcapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      368 2024-05-11 21:20:23.000000 aiocmcapi-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 21:21:25.645000 aiocmcapi-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 21:37:46.019805 aiocmcapi-0.2/
+-rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.2/LICENSE
+-rw-rw-rw-   0        0        0     2014 2024-05-11 21:37:46.018806 aiocmcapi-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2024-05-11 21:20:54.000000 aiocmcapi-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 21:37:46.018806 aiocmcapi-0.2/aiocmcapi.egg-info/
+-rw-rw-rw-   0        0        0     2014 2024-05-11 21:37:45.000000 aiocmcapi-0.2/aiocmcapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2024-05-11 21:37:46.000000 aiocmcapi-0.2/aiocmcapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 21:37:46.000000 aiocmcapi-0.2/aiocmcapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-11 21:37:46.000000 aiocmcapi-0.2/aiocmcapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      368 2024-05-11 21:37:40.000000 aiocmcapi-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 21:37:46.019805 aiocmcapi-0.2/setup.cfg
```

### Comparing `aiocmcapi-0.1/LICENSE` & `aiocmcapi-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.1/PKG-INFO` & `aiocmcapi-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocmcapi
-Version: 0.1
+Version: 0.2
 Summary: Async wrapper for CoinMarketCap API
 Author-email: alobuzy <amozebus@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiocmcapi
```

### Comparing `aiocmcapi-0.1/README.md` & `aiocmcapi-0.2/README.md`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.1/aiocmcapi.egg-info/PKG-INFO` & `aiocmcapi-0.2/aiocmcapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocmcapi
-Version: 0.1
+Version: 0.2
 Summary: Async wrapper for CoinMarketCap API
 Author-email: alobuzy <amozebus@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # aiocmcapi
```

