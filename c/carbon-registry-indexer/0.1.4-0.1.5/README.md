# Comparing `tmp/carbon-registry-indexer-0.1.4.tar.gz` & `tmp/carbon-registry-indexer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbon-registry-indexer-0.1.4.tar", last modified: Sat May 11 06:29:41 2024, max compression
+gzip compressed data, was "carbon-registry-indexer-0.1.5.tar", last modified: Sat May 11 06:37:25 2024, max compression
```

## Comparing `carbon-registry-indexer-0.1.4.tar` & `carbon-registry-indexer-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 06:29:41.074787 carbon-registry-indexer-0.1.4/
--rw-rw-rw-   0        0        0     1061 2024-05-11 06:08:04.000000 carbon-registry-indexer-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1397 2024-05-11 06:29:41.074787 carbon-registry-indexer-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      431 2024-05-10 15:34:37.000000 carbon-registry-indexer-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 06:29:41.058782 carbon-registry-indexer-0.1.4/carbon-registry-indexer/
--rw-rw-rw-   0        0        0    16921 2024-05-10 16:36:49.000000 carbon-registry-indexer-0.1.4/carbon-registry-indexer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:29:41.062785 carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/
--rw-rw-rw-   0        0        0      467 2024-05-10 11:35:06.000000 carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/__init__.py
--rw-rw-rw-   0        0        0    10104 2024-05-10 11:09:42.000000 carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/constants.py
--rw-rw-rw-   0        0        0    15848 2024-05-10 15:23:00.000000 carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/sync_acr.py
--rw-rw-rw-   0        0        0     4056 2024-05-10 11:33:26.000000 carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/sync_cadt.py
--rw-rw-rw-   0        0        0    17876 2024-05-10 15:22:50.000000 carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/sync_car.py
--rw-rw-rw-   0        0        0    10328 2024-05-09 09:57:43.000000 carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/sync_gs.py
--rw-rw-rw-   0        0        0    18116 2024-05-10 12:19:26.000000 carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:29:41.064786 carbon-registry-indexer-0.1.4/carbon-registry-indexer/models/
--rw-rw-rw-   0        0        0        0 2024-04-03 10:49:14.000000 carbon-registry-indexer-0.1.4/carbon-registry-indexer/models/__init__.py
--rw-rw-rw-   0        0        0    54117 2024-05-09 16:06:08.000000 carbon-registry-indexer-0.1.4/carbon-registry-indexer/models/enums.py
--rw-rw-rw-   0        0        0     8063 2024-05-08 09:13:55.000000 carbon-registry-indexer-0.1.4/carbon-registry-indexer/models/target.py
-drwxrwxrwx   0        0        0        0 2024-05-11 06:29:41.073784 carbon-registry-indexer-0.1.4/carbon_registry_indexer.egg-info/
--rw-rw-rw-   0        0        0     1397 2024-05-11 06:29:40.000000 carbon-registry-indexer-0.1.4/carbon_registry_indexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      771 2024-05-11 06:29:41.000000 carbon-registry-indexer-0.1.4/carbon_registry_indexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 06:29:40.000000 carbon-registry-indexer-0.1.4/carbon_registry_indexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-05-11 06:29:40.000000 carbon-registry-indexer-0.1.4/carbon_registry_indexer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-11 06:29:40.000000 carbon-registry-indexer-0.1.4/carbon_registry_indexer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-11 06:29:41.075784 carbon-registry-indexer-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1229 2024-05-11 06:29:33.000000 carbon-registry-indexer-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:37:25.607214 carbon-registry-indexer-0.1.5/
+-rw-rw-rw-   0        0        0     1061 2024-05-11 06:08:04.000000 carbon-registry-indexer-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1397 2024-05-11 06:37:25.607214 carbon-registry-indexer-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-05-10 15:34:37.000000 carbon-registry-indexer-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 06:37:25.591149 carbon-registry-indexer-0.1.5/carbon_registry_indexer/
+-rw-rw-rw-   0        0        0    16921 2024-05-10 16:36:49.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:37:25.604207 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/
+-rw-rw-rw-   0        0        0      467 2024-05-10 11:35:06.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/__init__.py
+-rw-rw-rw-   0        0        0    10104 2024-05-10 11:09:42.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/constants.py
+-rw-rw-rw-   0        0        0    15848 2024-05-10 15:23:00.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_acr.py
+-rw-rw-rw-   0        0        0     4056 2024-05-10 11:33:26.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_cadt.py
+-rw-rw-rw-   0        0        0    17876 2024-05-10 15:22:50.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_car.py
+-rw-rw-rw-   0        0        0    10328 2024-05-09 09:57:43.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_gs.py
+-rw-rw-rw-   0        0        0    18116 2024-05-10 12:19:26.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:37:25.606212 carbon-registry-indexer-0.1.5/carbon_registry_indexer/models/
+-rw-rw-rw-   0        0        0        0 2024-04-03 10:49:14.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/models/__init__.py
+-rw-rw-rw-   0        0        0    54117 2024-05-09 16:06:08.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/models/enums.py
+-rw-rw-rw-   0        0        0     8063 2024-05-08 09:13:55.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer/models/target.py
+drwxrwxrwx   0        0        0        0 2024-05-11 06:37:25.606212 carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/
+-rw-rw-rw-   0        0        0     1397 2024-05-11 06:37:25.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      771 2024-05-11 06:37:25.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 06:37:25.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-11 06:37:25.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-11 06:37:25.000000 carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-11 06:37:25.608212 carbon-registry-indexer-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2024-05-11 06:37:23.000000 carbon-registry-indexer-0.1.5/setup.py
```

### Comparing `carbon-registry-indexer-0.1.4/LICENSE` & `carbon-registry-indexer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.4/PKG-INFO` & `carbon-registry-indexer-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbon-registry-indexer
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library designed to streamline the aggregation of carbon data from multiple registries, each with its own data format, into a unified schema in CSV/Parquet formats.
 Home-page: https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer
 Download-URL: https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer/archive/refs/tags/v_01.tar.gz
 Author: Gautam P
 Author-email: gautam@carbonmarketshq.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `carbon-registry-indexer-0.1.4/carbon-registry-indexer/__init__.py` & `carbon-registry-indexer-0.1.5/carbon_registry_indexer/__init__.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/constants.py` & `carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/constants.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/sync_acr.py` & `carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_acr.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/sync_cadt.py` & `carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_cadt.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/sync_car.py` & `carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_car.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/sync_gs.py` & `carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/sync_gs.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.4/carbon-registry-indexer/integrations/utils.py` & `carbon-registry-indexer-0.1.5/carbon_registry_indexer/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.4/carbon-registry-indexer/models/enums.py` & `carbon-registry-indexer-0.1.5/carbon_registry_indexer/models/enums.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.4/carbon-registry-indexer/models/target.py` & `carbon-registry-indexer-0.1.5/carbon_registry_indexer/models/target.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.4/carbon_registry_indexer.egg-info/PKG-INFO` & `carbon-registry-indexer-0.1.5/carbon_registry_indexer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbon-registry-indexer
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python library designed to streamline the aggregation of carbon data from multiple registries, each with its own data format, into a unified schema in CSV/Parquet formats.
 Home-page: https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer
 Download-URL: https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer/archive/refs/tags/v_01.tar.gz
 Author: Gautam P
 Author-email: gautam@carbonmarketshq.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `carbon-registry-indexer-0.1.4/setup.py` & `carbon-registry-indexer-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name='carbon-registry-indexer',
-    version='0.1.4',
+    version='0.1.5',
     license='MIT',
     description='A Python library designed to streamline the aggregation of carbon data from multiple registries, each with its own data format, into a unified schema in CSV/Parquet formats.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer', 
     download_url='https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer/archive/refs/tags/v_01.tar.gz',
     author='Gautam P',
```

