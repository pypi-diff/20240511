# Comparing `tmp/satsure_core_test-0.0.4.tar.gz` & `tmp/satsure_core_test-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure_core_test-0.0.4.tar", last modified: Thu May  9 07:13:46 2024, max compression
+gzip compressed data, was "satsure_core_test-0.0.6.tar", last modified: Sat May 11 19:52:58 2024, max compression
```

## Comparing `satsure_core_test-0.0.4.tar` & `satsure_core_test-0.0.6.tar`

### file list

```diff
@@ -1,39 +1,53 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-09 07:13:46.904507 satsure_core_test-0.0.4/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure_core_test-0.0.4/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      374 2024-05-09 07:13:46.904266 satsure_core_test-0.0.4/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure_core_test-0.0.4/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-09 07:13:46.898761 satsure_core_test-0.0.4/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure_core_test-0.0.4/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      974 2024-05-09 06:38:23.000000 satsure_core_test-0.0.4/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-09 07:13:46.899091 satsure_core_test-0.0.4/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-09 06:38:23.000000 satsure_core_test-0.0.4/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2479 2024-05-09 06:38:23.000000 satsure_core_test-0.0.4/satelite/core/downloader.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-09 07:13:46.899460 satsure_core_test-0.0.4/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-09 06:38:23.000000 satsure_core_test-0.0.4/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-09 06:38:23.000000 satsure_core_test-0.0.4/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-09 07:13:46.901009 satsure_core_test-0.0.4/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      291 2024-05-09 06:38:23.000000 satsure_core_test-0.0.4/satelite/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2427 2024-05-06 07:15:52.000000 satsure_core_test-0.0.4/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure_core_test-0.0.4/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2994 2024-05-09 04:58:53.000000 satsure_core_test-0.0.4/satelite/sentinel2/get_tiles.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3250 2024-05-09 06:38:23.000000 satsure_core_test-0.0.4/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-09 06:38:23.000000 satsure_core_test-0.0.4/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-09 07:13:46.901234 satsure_core_test-0.0.4/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-09 04:58:53.000000 satsure_core_test-0.0.4/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      747 2024-05-06 07:43:01.000000 satsure_core_test-0.0.4/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-09 07:13:46.903252 satsure_core_test-0.0.4/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-09 04:58:53.000000 satsure_core_test-0.0.4/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-06 07:43:01.000000 satsure_core_test-0.0.4/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure_core_test-0.0.4/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1322 2024-05-06 07:34:13.000000 satsure_core_test-0.0.4/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-09 06:38:23.000000 satsure_core_test-0.0.4/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-09 06:38:23.000000 satsure_core_test-0.0.4/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1545 2024-05-09 06:38:23.000000 satsure_core_test-0.0.4/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-09 07:13:46.904035 satsure_core_test-0.0.4/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      374 2024-05-09 07:13:46.000000 satsure_core_test-0.0.4/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      995 2024-05-09 07:13:46.000000 satsure_core_test-0.0.4/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-09 07:13:46.000000 satsure_core_test-0.0.4/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       75 2024-05-09 07:13:46.000000 satsure_core_test-0.0.4/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-09 07:13:46.000000 satsure_core_test-0.0.4/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-09 07:13:46.904554 satsure_core_test-0.0.4/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      379 2024-05-09 07:10:40.000000 satsure_core_test-0.0.4/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:52:58.765836 satsure_core_test-0.0.6/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure_core_test-0.0.6/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      410 2024-05-11 19:52:58.765625 satsure_core_test-0.0.6/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure_core_test-0.0.6/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:52:58.759272 satsure_core_test-0.0.6/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure_core_test-0.0.6/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      974 2024-05-11 07:38:29.000000 satsure_core_test-0.0.6/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:52:58.759586 satsure_core_test-0.0.6/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.0.6/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2479 2024-05-11 07:35:59.000000 satsure_core_test-0.0.6/satelite/core/downloader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:52:58.759986 satsure_core_test-0.0.6/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:47:03.000000 satsure_core_test-0.0.6/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3069 2024-05-11 19:47:03.000000 satsure_core_test-0.0.6/satelite/gdal/gdal_commands.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:52:58.760269 satsure_core_test-0.0.6/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.0.6/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-11 07:35:59.000000 satsure_core_test-0.0.6/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:52:58.760515 satsure_core_test-0.0.6/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:47:03.000000 satsure_core_test-0.0.6/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8390 2024-05-11 19:47:03.000000 satsure_core_test-0.0.6/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:52:58.762102 satsure_core_test-0.0.6/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      402 2024-05-11 19:47:03.000000 satsure_core_test-0.0.6/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:52:58.762420 satsure_core_test-0.0.6/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:47:03.000000 satsure_core_test-0.0.6/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2934 2024-05-11 19:47:03.000000 satsure_core_test-0.0.6/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-11 07:42:30.000000 satsure_core_test-0.0.6/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure_core_test-0.0.6/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3121 2024-05-11 19:47:03.000000 satsure_core_test-0.0.6/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:52:58.762659 satsure_core_test-0.0.6/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:47:03.000000 satsure_core_test-0.0.6/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4597 2024-05-11 19:47:03.000000 satsure_core_test-0.0.6/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2539 2024-05-11 19:47:03.000000 satsure_core_test-0.0.6/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3250 2024-05-11 07:35:59.000000 satsure_core_test-0.0.6/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-11 07:35:59.000000 satsure_core_test-0.0.6/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:52:58.762973 satsure_core_test-0.0.6/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.0.6/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      747 2024-05-06 07:43:01.000000 satsure_core_test-0.0.6/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:52:58.764853 satsure_core_test-0.0.6/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.0.6/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-06 07:43:01.000000 satsure_core_test-0.0.6/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure_core_test-0.0.6/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1322 2024-05-06 07:34:13.000000 satsure_core_test-0.0.6/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-11 19:47:03.000000 satsure_core_test-0.0.6/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-11 07:35:59.000000 satsure_core_test-0.0.6/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-11 07:35:59.000000 satsure_core_test-0.0.6/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-11 07:35:59.000000 satsure_core_test-0.0.6/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 19:52:58.765447 satsure_core_test-0.0.6/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      410 2024-05-11 19:52:58.000000 satsure_core_test-0.0.6/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1377 2024-05-11 19:52:58.000000 satsure_core_test-0.0.6/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-11 19:52:58.000000 satsure_core_test-0.0.6/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       96 2024-05-11 19:52:58.000000 satsure_core_test-0.0.6/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-11 19:52:58.000000 satsure_core_test-0.0.6/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-11 19:52:58.765869 satsure_core_test-0.0.6/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      424 2024-05-11 19:52:14.000000 satsure_core_test-0.0.6/setup.py
```

### Comparing `satsure_core_test-0.0.4/satelite/config.py` & `satsure_core_test-0.0.6/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.4/satelite/core/downloader.py` & `satsure_core_test-0.0.6/satelite/core/downloader.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.4/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure_core_test-0.0.6/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
         pd.DataFrame]:
         """
         Fetching features list using tile ids
         :param tile_list:
         :return: list
         """
         api_df_list = []
-        for tileId in tile_list:
+        for tile_id in tile_list:
             url = (
                 f'https://catalogue.dataspace.copernicus.eu/resto/api/collections/Sentinel2/search.json?cloudCover=[{self.cloud_cover_perc}]'
                 f'&startDate={self.start_date}T00:00:00Z&completionDate={self.end_date}T23:59:59Z&'
                 f'productType={self.METADATA[self.processing_level]["producttype"]}&'
-                f'processingLevel={self.METADATA[self.processing_level]["processinglevel"]}&tileId={tileId}&maxRecords=1000')
+                f'processingLevel={self.METADATA[self.processing_level]["processinglevel"]}&tileId={tile_id}&maxRecords=1000')
             response = requests.get(url)
             json = response.json()
             df = pd.DataFrame.from_dict(json["features"])
             # Extract specific keys from the 'metadata' column
             df["productIdentifier"] = df["properties"].apply(
                 lambda x: x.get("productIdentifier")
             )
```

### Comparing `satsure_core_test-0.0.4/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure_core_test-0.0.6/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.4/satelite/sentinel2/get_tiles.py` & `satsure_core_test-0.0.6/satelite/sentinel2/get_tiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 class GetTiles:
     """To get tiles from different resources"""
 
     def __init__(self):
         self.session = Session.create()
 
     def fetch_tile_from_db(self, sql_query, geom_):
+        """
+            Fetch tile from database
+        :param sql_query:
+        :param geom_:
+        :return:
+        """
+
         result = self.session.execute(sql_query,
                                       {"geojson_geometry": str(geom_)})
         return result.fetchall()
 
     def get_tile_from_geom(self, geom_list: list) -> list:
         """generate tile from in geom
         :rtype: list
```

### Comparing `satsure_core_test-0.0.4/satelite/sentinel2/s2_l1c_urls.py` & `satsure_core_test-0.0.6/satelite/sentinel2/s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.4/satelite/sentinel2/s2_l2a_urls.py` & `satsure_core_test-0.0.6/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.4/satelite/tests/conftest.py` & `satsure_core_test-0.0.6/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.4/satelite/tests/sentinel2/test_get_tile.py` & `satsure_core_test-0.0.6/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.4/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure_core_test-0.0.6/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.4/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure_core_test-0.0.6/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.0.4/satelite/tests/sentinel2/test_validate.py` & `satsure_core_test-0.0.6/satelite/tests/sentinel2/test_validate.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,19 +18,19 @@
         errors = {"tile_code": (
             f"tile_codes expected a non empty str, got {type([])}",
             [], TypeError),
             "from_date": (
                 f"from_date expected a string of form: YYYY-MM-DD, got {type(12)}",
                 12, TypeError),
             "download_path": (
-                f"download_path expected a PosixPath, got {type("path")}",
+                f"download_path expected a PosixPath, got {type('str')}",
                 "path", TypeError),
 
             "bands": (
-                f"bands expected a tuple / list, got {type("path")}",
+                f"bands expected a tuple / list, got {type('str')}",
                 "path", TypeError),
 
         }
 
         for error in errors:
             current = params.copy()
             assert_val, value, err_type = errors[error]
```

### Comparing `satsure_core_test-0.0.4/satsure_core_test.egg-info/SOURCES.txt` & `satsure_core_test-0.0.6/satsure_core_test.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 LICENCE.txt
 README.md
 setup.py
 satelite/__init__.py
 satelite/config.py
 satelite/core/__init__.py
 satelite/core/downloader.py
+satelite/gdal/__init__.py
+satelite/gdal/gdal_commands.py
 satelite/models/__init__.py
 satelite/models/s2_enum.py
+satelite/raster/__init__.py
+satelite/raster/raster.py
 satelite/sentinel2/__init__.py
 satelite/sentinel2/fetch_unique_tile_date.py
 satelite/sentinel2/fetch_unique_tile_date_pystac.py
 satelite/sentinel2/get_tiles.py
+satelite/sentinel2/mosaic_same_bands.py
 satelite/sentinel2/s2_l1c_urls.py
 satelite/sentinel2/s2_l2a_urls.py
+satelite/sentinel2/band_stack/__init__.py
+satelite/sentinel2/band_stack/generate_band_stack.py
+satelite/sentinel2/indices/__init__.py
+satelite/sentinel2/indices/general_indices.py
 satelite/tests/__init__.py
 satelite/tests/conftest.py
 satelite/tests/sentinel2/__init__.py
 satelite/tests/sentinel2/test_fetch_unique_tile_date.py
 satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
 satelite/tests/sentinel2/test_get_tile.py
+satelite/tests/sentinel2/test_mosaic_same_bands.py
 satelite/tests/sentinel2/test_s2_l1c_urls.py
 satelite/tests/sentinel2/test_s2_l2a_urls.py
 satelite/tests/sentinel2/test_validate.py
 satsure_core_test.egg-info/PKG-INFO
 satsure_core_test.egg-info/SOURCES.txt
 satsure_core_test.egg-info/dependency_links.txt
 satsure_core_test.egg-info/requires.txt
```

