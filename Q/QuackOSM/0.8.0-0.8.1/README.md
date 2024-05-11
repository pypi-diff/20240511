# Comparing `tmp/quackosm-0.8.0.tar.gz` & `tmp/quackosm-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quackosm-0.8.0.tar", last modified: Thu May  9 08:31:35 2024, max compression
+gzip compressed data, was "quackosm-0.8.1.tar", last modified: Sat May 11 19:24:12 2024, max compression
```

## Comparing `quackosm-0.8.0.tar` & `quackosm-0.8.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11339 2024-05-09 08:31:06.335242 quackosm-0.8.0/LICENSE
--rw-r--r--   0        0        0    27910 2024-05-09 08:31:06.335242 quackosm-0.8.0/README.md
--rw-r--r--   0        0        0     4538 2024-05-09 08:31:35.423438 quackosm-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      560 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/__init__.py
--rw-r--r--   0        0        0      464 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/__main__.py
--rw-r--r--   0        0        0      127 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/_constants.py
--rw-r--r--   0        0        0      181 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/_exceptions.py
--rw-r--r--   0        0        0     6497 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/_osm_tags_filters.py
--rw-r--r--   0        0        0     1188 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/_osm_way_polygon_features.py
--rw-r--r--   0        0        0    11246 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/_rich_progress.py
--rw-r--r--   0        0        0      717 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/_typing.py
--rw-r--r--   0        0        0    24503 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/cli.py
--rw-r--r--   0        0        0     2031 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/conftest.py
--rw-r--r--   0        0        0    54717 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/functions.py
--rw-r--r--   0        0        0    19193 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_extracts/__init__.py
--rw-r--r--   0        0        0     2320 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_extracts/_poly_parser.py
--rw-r--r--   0        0        0     2941 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_extracts/bbbike.py
--rw-r--r--   0        0        0      251 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_extracts/extract.py
--rw-r--r--   0        0        0     1709 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_extracts/geofabrik.py
--rw-r--r--   0        0        0     4376 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_extracts/osm_fr.py
--rw-r--r--   0        0        0     3362 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/osm_way_polygon_features.json
--rw-r--r--   0        0        0   112604 2024-05-09 08:31:06.347242 quackosm-0.8.0/quackosm/pbf_file_reader.py
--rw-r--r--   0        0        0       33 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0       38 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/base/__init__.py
--rw-r--r--   0        0        0      746 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/base/conftest.py
--rw-r--r--   0        0        0    24603 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/base/test_cli.py
--rw-r--r--   0        0        0     5422 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/base/test_osm_extracts.py
--rw-r--r--   0        0        0    29285 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/base/test_osm_tags_filtering.py
--rw-r--r--   0        0        0    37132 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/base/test_pbf_file_reader.py
--rw-r--r--   0        0        0       43 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/benchmark/__init__.py
--rw-r--r--   0        0        0      945 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/benchmark/test_big_file.py
--rw-r--r--   0        0        0      238 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0     1456 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/optional_imports/test_optional_cli_dependency.py
--rw-r--r--   0        0        0      342 2024-05-09 08:31:06.347242 quackosm-0.8.0/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   537903 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/monaco.osm.pbf
--rw-r--r--   0        0        0    91717 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/monaco_boundary.geojson
--rw-r--r--   0        0        0      112 2024-05-09 08:31:06.351242 quackosm-0.8.0/tests/test_files/osm_tags_filter.json
--rw-r--r--   0        0        0    29811 1970-01-01 00:00:00.000000 quackosm-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-05-11 19:23:45.877475 quackosm-0.8.1/LICENSE
+-rw-r--r--   0        0        0    27547 2024-05-11 19:23:45.877475 quackosm-0.8.1/README.md
+-rw-r--r--   0        0        0     4511 2024-05-11 19:24:12.505586 quackosm-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      602 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/__init__.py
+-rw-r--r--   0        0        0      464 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/__main__.py
+-rw-r--r--   0        0        0      127 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/_constants.py
+-rw-r--r--   0        0        0      181 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/_exceptions.py
+-rw-r--r--   0        0        0     6497 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/_osm_tags_filters.py
+-rw-r--r--   0        0        0     1188 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/_osm_way_polygon_features.py
+-rw-r--r--   0        0        0    11246 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/_rich_progress.py
+-rw-r--r--   0        0        0      717 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/_typing.py
+-rw-r--r--   0        0        0    24561 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/cli.py
+-rw-r--r--   0        0        0     1558 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/conftest.py
+-rw-r--r--   0        0        0    55918 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/functions.py
+-rw-r--r--   0        0        0    19193 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/osm_extracts/__init__.py
+-rw-r--r--   0        0        0     2320 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/osm_extracts/_poly_parser.py
+-rw-r--r--   0        0        0     2941 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/osm_extracts/bbbike.py
+-rw-r--r--   0        0        0      251 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/osm_extracts/extract.py
+-rw-r--r--   0        0        0     1709 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/osm_extracts/geofabrik.py
+-rw-r--r--   0        0        0     4376 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/osm_extracts/osm_fr.py
+-rw-r--r--   0        0        0     3362 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/osm_way_polygon_features.json
+-rw-r--r--   0        0        0   112979 2024-05-11 19:23:45.885475 quackosm-0.8.1/quackosm/pbf_file_reader.py
+-rw-r--r--   0        0        0       33 2024-05-11 19:23:45.885475 quackosm-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-11 19:23:45.885475 quackosm-0.8.1/tests/base/__init__.py
+-rw-r--r--   0        0        0      746 2024-05-11 19:23:45.885475 quackosm-0.8.1/tests/base/conftest.py
+-rw-r--r--   0        0        0    24603 2024-05-11 19:23:45.885475 quackosm-0.8.1/tests/base/test_cli.py
+-rw-r--r--   0        0        0     5422 2024-05-11 19:23:45.885475 quackosm-0.8.1/tests/base/test_osm_extracts.py
+-rw-r--r--   0        0        0    29321 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/base/test_osm_tags_filtering.py
+-rw-r--r--   0        0        0    39749 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/base/test_pbf_file_reader.py
+-rw-r--r--   0        0        0       43 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/benchmark/__init__.py
+-rw-r--r--   0        0        0      949 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/benchmark/test_big_file.py
+-rw-r--r--   0        0        0      238 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/conftest.py
+-rw-r--r--   0        0        0     1437 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/optional_imports/test_optional_cli_dependency.py
+-rw-r--r--   0        0        0      342 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   537903 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/test_files/monaco.osm.pbf
+-rw-r--r--   0        0        0    91717 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/test_files/monaco_boundary.geojson
+-rw-r--r--   0        0        0      112 2024-05-11 19:23:45.889475 quackosm-0.8.1/tests/test_files/osm_tags_filter.json
+-rw-r--r--   0        0        0    29448 1970-01-01 00:00:00.000000 quackosm-0.8.1/PKG-INFO
```

### Comparing `quackosm-0.8.0/LICENSE` & `quackosm-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/README.md` & `quackosm-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
 ### If you already have downloaded the PBF file 📁🗺️
 
 #### Load data as a GeoDataFrame
 
 ```python
 >>> import quackosm as qosm
->>> qosm.get_features_gdf(monaco_pbf_path)
+>>> qosm.convert_pbf_to_geodataframe(monaco_pbf_path)
                                               tags                      geometry
 feature_id
 node/10005045289                {'shop': 'bakery'}      POINT (7.42245 43.73105)
 node/10020887517  {'leisure': 'swimming_pool', ...      POINT (7.41316 43.73384)
 node/10021298117  {'leisure': 'swimming_pool', ...      POINT (7.42777 43.74277)
 node/10021298717  {'leisure': 'swimming_pool', ...      POINT (7.42630 43.74097)
 node/10025656383  {'ferry': 'yes', 'name': 'Qua...      POINT (7.42550 43.73690)
@@ -135,15 +135,15 @@
 [7906 rows x 2 columns]
 ```
 
 #### Just convert PBF to GeoParquet
 
 ```python
 >>> import quackosm as qosm
->>> gpq_path = qosm.convert_pbf_to_gpq(monaco_pbf_path)
+>>> gpq_path = qosm.convert_pbf_to_parquet(monaco_pbf_path)
 >>> gpq_path.as_posix()
 'files/monaco_nofilter_noclip_compact.parquet'
 ```
 
 #### Inspect the file with duckdb
 
 ```python
@@ -184,65 +184,63 @@
 └────────────────────────────────────────────────────────────────────────────────────────┘
 ```
 
 #### Use as CLI
 
 ```console
 $ quackosm monaco.osm.pbf
-⠙ [   1/32] Reading nodes • 0:00:00
+⠋ [   1/32] Reading nodes • 0:00:00
 ⠋ [   2/32] Filtering nodes - intersection • 0:00:00
-⠙ [   3/32] Filtering nodes - tags • 0:00:00
+⠋ [   3/32] Filtering nodes - tags • 0:00:00
 ⠋ [   4/32] Calculating distinct filtered nodes ids • 0:00:00
-⠙ [   5/32] Reading ways • 0:00:00
+⠋ [   5/32] Reading ways • 0:00:00
 ⠋ [   6/32] Unnesting ways • 0:00:00
-⠹ [   7/32] Filtering ways - valid refs • 0:00:00
+⠋ [   7/32] Filtering ways - valid refs • 0:00:00
 ⠋ [   8/32] Filtering ways - intersection • 0:00:00
-⠙ [   9/32] Filtering ways - tags • 0:00:00
+⠋ [   9/32] Filtering ways - tags • 0:00:00
 ⠋ [  10/32] Calculating distinct filtered ways ids • 0:00:00
 ⠋ [  11/32] Reading relations • 0:00:00
 ⠋ [  12/32] Unnesting relations • 0:00:00
-⠹ [  13/32] Filtering relations - valid refs • 0:00:00
+⠸ [  13/32] Filtering relations - valid refs • 0:00:00
 ⠋ [  14/32] Filtering relations - intersection • 0:00:00
-⠙ [  15/32] Filtering relations - tags • 0:00:00
+⠋ [  15/32] Filtering relations - tags • 0:00:00
 ⠋ [  16/32] Calculating distinct filtered relations ids • 0:00:00
-⠙ [  17/32] Loading required ways - by relations • 0:00:00
+⠋ [  17/32] Loading required ways - by relations • 0:00:00
 ⠋ [  18/32] Calculating distinct required ways ids • 0:00:00
-⠙ [  19/32] Saving filtered nodes with geometries • 0:00:00
+⠋ [  19/32] Saving filtered nodes with geometries • 0:00:00
 ⠋ [20.1/32] Grouping filtered ways - assigning groups • 0:00:00
 ⠧ [20.2/32] Grouping filtered ways - joining with nodes • 0:00:00
 ⠋ [20.3/32] Grouping filtered ways - partitioning by group • 0:00:00
   [  21/32] Saving filtered ways with linestrings 100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1/1 • 0:00:00 < 0:00:00 •
 ⠋ [22.1/32] Grouping required ways - assigning groups • 0:00:00
 ⠧ [22.2/32] Grouping required ways - joining with nodes • 0:00:00
 ⠋ [22.3/32] Grouping required ways - partitioning by group • 0:00:00
   [  23/32] Saving required ways with linestrings 100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1/1 • 0:00:00 < 0:00:00 •
-⠹ [  24/32] Saving filtered ways with geometries • 0:00:00
-⠸ [  25/32] Saving valid relations parts • 0:00:00
-⠋ [26.1/32] Saving relations inner parts - valid geometries • 0:00:00
-⠋ [26.2/32] Saving relations inner parts - invalid geometries • 0:00:00
-⠋ [27.1/32] Saving relations outer parts - valid geometries • 0:00:00
-⠋ [27.2/32] Saving relations outer parts - invalid geometries • 0:00:00
+⠙ [  24/32] Saving filtered ways with geometries • 0:00:00
+⠋ [  25/32] Saving valid relations parts • 0:00:00
+⠋ [  26/32] Saving relations inner parts • 0:00:00
+⠋ [  27/32] Saving relations outer parts • 0:00:00
 ⠋ [  28/32] Saving relations outer parts with holes • 0:00:00
 ⠋ [  29/32] Saving relations outer parts without holes • 0:00:00
-⠙ [  30/32] Saving filtered relations with geometries • 0:00:00
-⠹ [31.1/32] Saving valid features • 0:00:00
+⠋ [  30/32] Saving filtered relations with geometries • 0:00:00
+⠋ [  31/32] Saving all features • 0:00:00
 ⠋ [  32/32] Saving final geoparquet file • 0:00:00
-Finished operation in 0:00:06
+Finished operation in 0:00:03
 files/monaco_nofilter_noclip_compact.parquet
 ```
 
 ### Let the QuackOSM automatically download the required OSM PBF files for you 🔎🌍
 
 #### Load data as a GeoDataFrame
 
 ```python
 >>> import quackosm as qosm
 >>> import osmnx as ox
 >>> geometry = ox.geocode_to_gdf("Vatican City").unary_union
->>> qosm.get_features_gdf_from_geometry(geometry)
+>>> qosm.convert_geometry_to_geodataframe(geometry)
                                               tags                      geometry
 feature_id
 node/10253371713   {'crossing': 'uncontrolled',...     POINT (12.45603 41.90454)
 node/10253371714               {'highway': 'stop'}     POINT (12.45705 41.90400)
 node/10253371715               {'highway': 'stop'}     POINT (12.45242 41.90164)
 node/10253371720     {'artwork_type': 'statue',...     POINT (12.45147 41.90484)
 node/10253371738               {'natural': 'tree'}     POINT (12.45595 41.90609)
@@ -260,15 +258,15 @@
 
 ```python
 >>> import quackosm as qosm
 >>> from shapely import from_wkt
 >>> geometry = from_wkt(
 ...     "POLYGON ((14.4861 35.9107, 14.4861 35.8811, 14.5331 35.8811, 14.5331 35.9107, 14.4861 35.9107))"
 ... )
->>> gpq_path = qosm.convert_geometry_to_gpq(geometry)
+>>> gpq_path = qosm.convert_geometry_to_parquet(geometry)
 >>> gpq_path.as_posix()
 'files/4b2967088a8fe31cdc15401e29bff9b7b882565cd8143e90443f39f2dc5fe6de_nofilter_compact.parquet'
 ```
 
 #### Inspect the file with duckdb
 
 ```python
@@ -309,55 +307,53 @@
 └────────────────────────────────────────────────────────────────────────────────────────┘
 ```
 
 #### Use as CLI
 
 ```console
 $ quackosm --geom-filter-geocode "Shibuya, Tokyo"
-100%|██████████████████████████████████████| 45.7M/45.7M [00:00<00:00, 259GB/s]
-⠦ [   1/32] Reading nodes • 0:00:05
-⠋ [   2/32] Filtering nodes - intersection • 0:00:00
-⠦ [   3/32] Filtering nodes - tags • 0:00:00
+100%|██████████████████████████████████████| 46.3M/46.3M [00:00<00:00, 327GB/s]
+⠋ [   1/32] Reading nodes • 0:00:01
+⠹ [   2/32] Filtering nodes - intersection • 0:00:00
+⠋ [   3/32] Filtering nodes - tags • 0:00:00
 ⠋ [   4/32] Calculating distinct filtered nodes ids • 0:00:00
-⠏ [   5/32] Reading ways • 0:00:04
-⠦ [   6/32] Unnesting ways • 0:00:02
-⠴ [   7/32] Filtering ways - valid refs • 0:00:02
-⠙ [   8/32] Filtering ways - intersection • 0:00:01
-⠹ [   9/32] Filtering ways - tags • 0:00:00
+⠸ [   5/32] Reading ways • 0:00:03
+⠴ [   6/32] Unnesting ways • 0:00:01
+⠼ [   7/32] Filtering ways - valid refs • 0:00:00
+⠹ [   8/32] Filtering ways - intersection • 0:00:00
+⠋ [   9/32] Filtering ways - tags • 0:00:00
 ⠋ [  10/32] Calculating distinct filtered ways ids • 0:00:00
-⠴ [  11/32] Reading relations • 0:00:00
-⠴ [  12/32] Unnesting relations • 0:00:00
-⠹ [  13/32] Filtering relations - valid refs • 0:00:00
-⠙ [  14/32] Filtering relations - intersection • 0:00:00
-⠙ [  15/32] Filtering relations - tags • 0:00:00
+⠼ [  11/32] Reading relations • 0:00:00
+⠸ [  12/32] Unnesting relations • 0:00:00
+⠋ [  13/32] Filtering relations - valid refs • 0:00:00
+⠋ [  14/32] Filtering relations - intersection • 0:00:00
+⠋ [  15/32] Filtering relations - tags • 0:00:00
 ⠋ [  16/32] Calculating distinct filtered relations ids • 0:00:00
-⠙ [  17/32] Loading required ways - by relations • 0:00:00
+⠋ [  17/32] Loading required ways - by relations • 0:00:00
 ⠋ [  18/32] Calculating distinct required ways ids • 0:00:00
-⠋ [  19/32] Saving filtered nodes with geometries • 0:00:00
+⠹ [  19/32] Saving filtered nodes with geometries • 0:00:00
 ⠋ [20.1/32] Grouping filtered ways - assigning groups • 0:00:00
-⠴ [20.2/32] Grouping filtered ways - joining with nodes • 0:00:03
-⠹ [20.3/32] Grouping filtered ways - partitioning by group • 0:00:00
-  [  21/32] Saving filtered ways with linestrings 100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1/1 • 0:00:01 < 0:00:00 •
+⠼ [20.2/32] Grouping filtered ways - joining with nodes • 0:00:01
+⠋ [20.3/32] Grouping filtered ways - partitioning by group • 0:00:00
+  [  21/32] Saving filtered ways with linestrings 100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1/1 • 0:00:00 < 0:00:00 •
 ⠋ [22.1/32] Grouping required ways - assigning groups • 0:00:00
-⠴ [22.2/32] Grouping required ways - joining with nodes • 0:00:03
+⠼ [22.2/32] Grouping required ways - joining with nodes • 0:00:01
 ⠋ [22.3/32] Grouping required ways - partitioning by group • 0:00:00
   [  23/32] Saving required ways with linestrings 100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1/1 • 0:00:00 < 0:00:00 •
-⠋ [  24/32] Saving filtered ways with geometries • 0:00:01
-⠸ [  25/32] Saving valid relations parts • 0:00:00
-⠋ [26.1/32] Saving relations inner parts - valid geometries • 0:00:00
-⠋ [26.2/32] Saving relations inner parts - invalid geometries • 0:00:00
-⠙ [27.1/32] Saving relations outer parts - valid geometries • 0:00:00
-⠋ [27.2/32] Saving relations outer parts - invalid geometries • 0:00:00
+⠴ [  24/32] Saving filtered ways with geometries • 0:00:00
+⠋ [  25/32] Saving valid relations parts • 0:00:00
+⠋ [  26/32] Saving relations inner parts • 0:00:00
+⠋ [  27/32] Saving relations outer parts • 0:00:00
 ⠋ [  28/32] Saving relations outer parts with holes • 0:00:00
 ⠋ [  29/32] Saving relations outer parts without holes • 0:00:00
-⠙ [  30/32] Saving filtered relations with geometries • 0:00:00
-⠸ [31.1/32] Saving valid features • 0:00:00
+⠋ [  30/32] Saving filtered relations with geometries • 0:00:00
+⠙ [  31/32] Saving all features • 0:00:00
 ⠋ [  32/32] Saving final geoparquet file • 0:00:00
-Finished operation in 0:00:39
-files/9ae2b160eb7556991148f5a2693aaf4b38bbb225c3700a6bfe9e5e54f48b987e_nofilter_compact.parquet
+Finished operation in 0:00:13
+files/78580cf29b5ba1073366a257e1909bfeee43c9f5859e48fb3b2d592028bb58aa_nofilter_compact.parquet
 ```
 
 CLI Help output (`QuackOSM -h`):
 ![CLI Help output](https://raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/cli_help.png)
 
 You can find full API + more examples in the [docs](https://kraina-ai.github.io/quackosm/).
```

#### html2text {}

```diff
@@ -34,28 +34,28 @@
 files services - `beautifulsoup4`: For parsing HTML files and scraping required
 information Optional: - `typer[all] (>=0.9.0)` (click, colorama, rich,
 shellingham): For CLI - `osmnx (>=1.3.0)`: For geocoding of strings in CLI -
 `h3 (>=4.0.0b1)`: For reading H3 strings in CLI - `s2 (>=0.1.9)`: For
 transforming S2 indexes into geometries - `python-geohash (>=0.8)`: For
 transforming GeoHash indexes into geometries ## Usage ### If you already have
 downloaded the PBF file ððºï¸ #### Load data as a GeoDataFrame ```python
->>> import quackosm as qosm >>> qosm.get_features_gdf(monaco_pbf_path) tags
-geometry feature_id node/10005045289 {'shop': 'bakery'} POINT (7.42245
-43.73105) node/10020887517 {'leisure': 'swimming_pool', ... POINT (7.41316
-43.73384) node/10021298117 {'leisure': 'swimming_pool', ... POINT (7.42777
-43.74277) node/10021298717 {'leisure': 'swimming_pool', ... POINT (7.42630
-43.74097) node/10025656383 {'ferry': 'yes', 'name': 'Qua... POINT (7.42550
-43.73690) ... ... ... way/990669427 {'amenity': 'shelter', 'shelt... POLYGON (
-(7.41461 43.7338... way/990669428 {'highway': 'secondary', 'jun... LINESTRING
-(7.41366 43.73... way/990669429 {'highway': 'secondary', 'jun... LINESTRING
-(7.41376 43.73... way/990848785 {'addr:city': 'Monaco', 'addr... POLYGON (
-(7.41426 43.7339... way/993121275 {'building': 'yes', 'name': ... POLYGON (
-(7.43214 43.7481... [7906 rows x 2 columns] ``` #### Just convert PBF to
-GeoParquet ```python >>> import quackosm as qosm >>> gpq_path =
-qosm.convert_pbf_to_gpq(monaco_pbf_path) >>> gpq_path.as_posix() 'files/
+>>> import quackosm as qosm >>> qosm.convert_pbf_to_geodataframe
+(monaco_pbf_path) tags geometry feature_id node/10005045289 {'shop': 'bakery'}
+POINT (7.42245 43.73105) node/10020887517 {'leisure': 'swimming_pool', ...
+POINT (7.41316 43.73384) node/10021298117 {'leisure': 'swimming_pool', ...
+POINT (7.42777 43.74277) node/10021298717 {'leisure': 'swimming_pool', ...
+POINT (7.42630 43.74097) node/10025656383 {'ferry': 'yes', 'name': 'Qua...
+POINT (7.42550 43.73690) ... ... ... way/990669427 {'amenity': 'shelter',
+'shelt... POLYGON ((7.41461 43.7338... way/990669428 {'highway': 'secondary',
+'jun... LINESTRING (7.41366 43.73... way/990669429 {'highway': 'secondary',
+'jun... LINESTRING (7.41376 43.73... way/990848785 {'addr:city': 'Monaco',
+'addr... POLYGON ((7.41426 43.7339... way/993121275 {'building': 'yes', 'name':
+... POLYGON ((7.43214 43.7481... [7906 rows x 2 columns] ``` #### Just convert
+PBF to GeoParquet ```python >>> import quackosm as qosm >>> gpq_path =
+qosm.convert_pbf_to_parquet(monaco_pbf_path) >>> gpq_path.as_posix() 'files/
 monaco_nofilter_noclip_compact.parquet' ``` #### Inspect the file with duckdb
 ```python >>> import duckdb >>> duckdb.load_extension('spatial') >>>
 duckdb.read_parquet(str(gpq_path)).project( ... "* REPLACE (ST_GeomFromWKB
 (geometry) AS geometry)" ... ).order("feature_id")
 ââââââââââââââââââââ¬âââââââââââââââââââââââ¬âââââââââââââââââââââââââââââââââââââââââââââââ
 â feature_id â tags â geometry â â varchar â map(varchar, varchâ¦
 â geometry â
@@ -84,67 +84,65 @@
 {highway=secondaryâ¦ â LINESTRING (7.4137621 43.7334251, 7.413746â¦ â â
 way/990848785 â {addr:city=Monaco,â¦ â POLYGON ((7.4142551 43.7339622,
 7.4143113 â¦ â â way/993121275 â {building=yes, namâ¦ â POLYGON (
 (7.4321416 43.7481309, 7.4321638 â¦ â
 ââââââââââââââââââââ´âââââââââââââââââââââââ´âââââââââââââââââââââââââââââââââââââââââââââââ¤
 â 7906 rows (20 shown) 3 columns â
 ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
-``` #### Use as CLI ```console $ quackosm monaco.osm.pbf â  [ 1/32] Reading
-nodes â¢ 0:00:00 â  [ 2/32] Filtering nodes - intersection â¢ 0:00:00 â 
+``` #### Use as CLI ```console $ quackosm monaco.osm.pbf â  [ 1/32] Reading
+nodes â¢ 0:00:00 â  [ 2/32] Filtering nodes - intersection â¢ 0:00:00 â 
 [ 3/32] Filtering nodes - tags â¢ 0:00:00 â  [ 4/32] Calculating distinct
-filtered nodes ids â¢ 0:00:00 â  [ 5/32] Reading ways â¢ 0:00:00 â  [ 6/32]
-Unnesting ways â¢ 0:00:00 â ¹ [ 7/32] Filtering ways - valid refs â¢ 0:00:00
-â  [ 8/32] Filtering ways - intersection â¢ 0:00:00 â  [ 9/32] Filtering
+filtered nodes ids â¢ 0:00:00 â  [ 5/32] Reading ways â¢ 0:00:00 â  [ 6/32]
+Unnesting ways â¢ 0:00:00 â  [ 7/32] Filtering ways - valid refs â¢ 0:00:00
+â  [ 8/32] Filtering ways - intersection â¢ 0:00:00 â  [ 9/32] Filtering
 ways - tags â¢ 0:00:00 â  [ 10/32] Calculating distinct filtered ways ids â¢
 0:00:00 â  [ 11/32] Reading relations â¢ 0:00:00 â  [ 12/32] Unnesting
-relations â¢ 0:00:00 â ¹ [ 13/32] Filtering relations - valid refs â¢ 0:00:00
-â  [ 14/32] Filtering relations - intersection â¢ 0:00:00 â  [ 15/32]
+relations â¢ 0:00:00 â ¸ [ 13/32] Filtering relations - valid refs â¢ 0:00:00
+â  [ 14/32] Filtering relations - intersection â¢ 0:00:00 â  [ 15/32]
 Filtering relations - tags â¢ 0:00:00 â  [ 16/32] Calculating distinct
-filtered relations ids â¢ 0:00:00 â  [ 17/32] Loading required ways - by
+filtered relations ids â¢ 0:00:00 â  [ 17/32] Loading required ways - by
 relations â¢ 0:00:00 â  [ 18/32] Calculating distinct required ways ids â¢
-0:00:00 â  [ 19/32] Saving filtered nodes with geometries â¢ 0:00:00 â 
+0:00:00 â  [ 19/32] Saving filtered nodes with geometries â¢ 0:00:00 â 
 [20.1/32] Grouping filtered ways - assigning groups â¢ 0:00:00 â § [20.2/32]
 Grouping filtered ways - joining with nodes â¢ 0:00:00 â  [20.3/32] Grouping
 filtered ways - partitioning by group â¢ 0:00:00 [ 21/32] Saving filtered ways
 with linestrings 100%
 ââââââââââââââââââââââââââââââââââââââââ
 1/1 â¢ 0:00:00 < 0:00:00 â¢ â  [22.1/32] Grouping required ways - assigning
 groups â¢ 0:00:00 â § [22.2/32] Grouping required ways - joining with nodes
 â¢ 0:00:00 â  [22.3/32] Grouping required ways - partitioning by group â¢ 0:
 00:00 [ 23/32] Saving required ways with linestrings 100%
 ââââââââââââââââââââââââââââââââââââââââ
-1/1 â¢ 0:00:00 < 0:00:00 â¢ â ¹ [ 24/32] Saving filtered ways with geometries
-â¢ 0:00:00 â ¸ [ 25/32] Saving valid relations parts â¢ 0:00:00 â  [26.1/32]
-Saving relations inner parts - valid geometries â¢ 0:00:00 â  [26.2/32]
-Saving relations inner parts - invalid geometries â¢ 0:00:00 â  [27.1/32]
-Saving relations outer parts - valid geometries â¢ 0:00:00 â  [27.2/32]
-Saving relations outer parts - invalid geometries â¢ 0:00:00 â  [ 28/32]
-Saving relations outer parts with holes â¢ 0:00:00 â  [ 29/32] Saving
-relations outer parts without holes â¢ 0:00:00 â  [ 30/32] Saving filtered
-relations with geometries â¢ 0:00:00 â ¹ [31.1/32] Saving valid features â¢
-0:00:00 â  [ 32/32] Saving final geoparquet file â¢ 0:00:00 Finished
-operation in 0:00:06 files/monaco_nofilter_noclip_compact.parquet ``` ### Let
-the QuackOSM automatically download the required OSM PBF files for you ðð
-#### Load data as a GeoDataFrame ```python >>> import quackosm as qosm >>>
-import osmnx as ox >>> geometry = ox.geocode_to_gdf("Vatican City").unary_union
->>> qosm.get_features_gdf_from_geometry(geometry) tags geometry feature_id
-node/10253371713 {'crossing': 'uncontrolled',... POINT (12.45603 41.90454)
-node/10253371714 {'highway': 'stop'} POINT (12.45705 41.90400) node/10253371715
+1/1 â¢ 0:00:00 < 0:00:00 â¢ â  [ 24/32] Saving filtered ways with geometries
+â¢ 0:00:00 â  [ 25/32] Saving valid relations parts â¢ 0:00:00 â  [ 26/32]
+Saving relations inner parts â¢ 0:00:00 â  [ 27/32] Saving relations outer
+parts â¢ 0:00:00 â  [ 28/32] Saving relations outer parts with holes â¢ 0:
+00:00 â  [ 29/32] Saving relations outer parts without holes â¢ 0:00:00 â 
+[ 30/32] Saving filtered relations with geometries â¢ 0:00:00 â  [ 31/32]
+Saving all features â¢ 0:00:00 â  [ 32/32] Saving final geoparquet file â¢
+0:00:00 Finished operation in 0:00:03 files/
+monaco_nofilter_noclip_compact.parquet ``` ### Let the QuackOSM automatically
+download the required OSM PBF files for you ðð #### Load data as a
+GeoDataFrame ```python >>> import quackosm as qosm >>> import osmnx as ox >>>
+geometry = ox.geocode_to_gdf("Vatican City").unary_union >>>
+qosm.convert_geometry_to_geodataframe(geometry) tags geometry feature_id node/
+10253371713 {'crossing': 'uncontrolled',... POINT (12.45603 41.90454) node/
+10253371714 {'highway': 'stop'} POINT (12.45705 41.90400) node/10253371715
 {'highway': 'stop'} POINT (12.45242 41.90164) node/10253371720 {'artwork_type':
 'statue',... POINT (12.45147 41.90484) node/10253371738 {'natural': 'tree'}
 POINT (12.45595 41.90609) ... ... ... way/983015528 {'barrier': 'hedge',
 'height'... POLYGON ((12.45027 41.901... way/983015529 {'barrier': 'hedge',
 'height'... POLYGON ((12.45028 41.901... way/983015530 {'barrier': 'hedge',
 'height'... POLYGON ((12.45023 41.901... way/998561138 {'barrier': 'bollard',
 'bicyc... LINESTRING (12.45821 41.9... way/998561139 {'barrier': 'bollard',
 'bicyc... LINESTRING (12.45828 41.9... [3286 rows x 2 columns] ``` #### Just
 convert geometry to GeoParquet ```python >>> import quackosm as qosm >>> from
 shapely import from_wkt >>> geometry = from_wkt( ... "POLYGON ((14.4861
 35.9107, 14.4861 35.8811, 14.5331 35.8811, 14.5331 35.9107, 14.4861 35.9107))"
-... ) >>> gpq_path = qosm.convert_geometry_to_gpq(geometry) >>>
+... ) >>> gpq_path = qosm.convert_geometry_to_parquet(geometry) >>>
 gpq_path.as_posix() 'files/
 4b2967088a8fe31cdc15401e29bff9b7b882565cd8143e90443f39f2dc5fe6de_nofilter_compact.parquet'
 ``` #### Inspect the file with duckdb ```python >>> import duckdb >>>
 duckdb.load_extension('spatial') >>> duckdb.read_parquet(str(gpq_path)).project
 ( ... "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)" ... ).order
 ("feature_id")
 ââââââââââââââââââââ¬âââââââââââââââââââââââ¬âââââââââââââââââââââââââââââââââââââââââââââââ
@@ -179,49 +177,46 @@
 (14.5221083 35.8864287, 14.5221â¦ â
 ââââââââââââââââââââ´âââââââââââââââââââââââ´âââââââââââââââââââââââââââââââââââââââââââââââ¤
 â ? rows (>9999 rows, 20 shown) 3 columns â
 ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
 ``` #### Use as CLI ```console $ quackosm --geom-filter-geocode "Shibuya,
 Tokyo"
 100%|ââââââââââââââââââââââââââââââââââââââ|
-45.7M/45.7M [00:00<00:00, 259GB/s] â ¦ [ 1/32] Reading nodes â¢ 0:00:05 â 
-[ 2/32] Filtering nodes - intersection â¢ 0:00:00 â ¦ [ 3/32] Filtering nodes
+46.3M/46.3M [00:00<00:00, 327GB/s] â  [ 1/32] Reading nodes â¢ 0:00:01 â ¹
+[ 2/32] Filtering nodes - intersection â¢ 0:00:00 â  [ 3/32] Filtering nodes
 - tags â¢ 0:00:00 â  [ 4/32] Calculating distinct filtered nodes ids â¢ 0:
-00:00 â  [ 5/32] Reading ways â¢ 0:00:04 â ¦ [ 6/32] Unnesting ways â¢ 0:00:
-02 â ´ [ 7/32] Filtering ways - valid refs â¢ 0:00:02 â  [ 8/32] Filtering
-ways - intersection â¢ 0:00:01 â ¹ [ 9/32] Filtering ways - tags â¢ 0:00:00
-â  [ 10/32] Calculating distinct filtered ways ids â¢ 0:00:00 â ´ [ 11/32]
-Reading relations â¢ 0:00:00 â ´ [ 12/32] Unnesting relations â¢ 0:00:00 â ¹
-[ 13/32] Filtering relations - valid refs â¢ 0:00:00 â  [ 14/32] Filtering
-relations - intersection â¢ 0:00:00 â  [ 15/32] Filtering relations - tags
+00:00 â ¸ [ 5/32] Reading ways â¢ 0:00:03 â ´ [ 6/32] Unnesting ways â¢ 0:00:
+01 â ¼ [ 7/32] Filtering ways - valid refs â¢ 0:00:00 â ¹ [ 8/32] Filtering
+ways - intersection â¢ 0:00:00 â  [ 9/32] Filtering ways - tags â¢ 0:00:00
+â  [ 10/32] Calculating distinct filtered ways ids â¢ 0:00:00 â ¼ [ 11/32]
+Reading relations â¢ 0:00:00 â ¸ [ 12/32] Unnesting relations â¢ 0:00:00 â 
+[ 13/32] Filtering relations - valid refs â¢ 0:00:00 â  [ 14/32] Filtering
+relations - intersection â¢ 0:00:00 â  [ 15/32] Filtering relations - tags
 â¢ 0:00:00 â  [ 16/32] Calculating distinct filtered relations ids â¢ 0:00:
-00 â  [ 17/32] Loading required ways - by relations â¢ 0:00:00 â  [ 18/32]
-Calculating distinct required ways ids â¢ 0:00:00 â  [ 19/32] Saving filtered
+00 â  [ 17/32] Loading required ways - by relations â¢ 0:00:00 â  [ 18/32]
+Calculating distinct required ways ids â¢ 0:00:00 â ¹ [ 19/32] Saving filtered
 nodes with geometries â¢ 0:00:00 â  [20.1/32] Grouping filtered ways -
-assigning groups â¢ 0:00:00 â ´ [20.2/32] Grouping filtered ways - joining
-with nodes â¢ 0:00:03 â ¹ [20.3/32] Grouping filtered ways - partitioning by
+assigning groups â¢ 0:00:00 â ¼ [20.2/32] Grouping filtered ways - joining
+with nodes â¢ 0:00:01 â  [20.3/32] Grouping filtered ways - partitioning by
 group â¢ 0:00:00 [ 21/32] Saving filtered ways with linestrings 100%
 ââââââââââââââââââââââââââââââââââââââââ
-1/1 â¢ 0:00:01 < 0:00:00 â¢ â  [22.1/32] Grouping required ways - assigning
-groups â¢ 0:00:00 â ´ [22.2/32] Grouping required ways - joining with nodes
-â¢ 0:00:03 â  [22.3/32] Grouping required ways - partitioning by group â¢ 0:
+1/1 â¢ 0:00:00 < 0:00:00 â¢ â  [22.1/32] Grouping required ways - assigning
+groups â¢ 0:00:00 â ¼ [22.2/32] Grouping required ways - joining with nodes
+â¢ 0:00:01 â  [22.3/32] Grouping required ways - partitioning by group â¢ 0:
 00:00 [ 23/32] Saving required ways with linestrings 100%
 ââââââââââââââââââââââââââââââââââââââââ
-1/1 â¢ 0:00:00 < 0:00:00 â¢ â  [ 24/32] Saving filtered ways with geometries
-â¢ 0:00:01 â ¸ [ 25/32] Saving valid relations parts â¢ 0:00:00 â  [26.1/32]
-Saving relations inner parts - valid geometries â¢ 0:00:00 â  [26.2/32]
-Saving relations inner parts - invalid geometries â¢ 0:00:00 â  [27.1/32]
-Saving relations outer parts - valid geometries â¢ 0:00:00 â  [27.2/32]
-Saving relations outer parts - invalid geometries â¢ 0:00:00 â  [ 28/32]
-Saving relations outer parts with holes â¢ 0:00:00 â  [ 29/32] Saving
-relations outer parts without holes â¢ 0:00:00 â  [ 30/32] Saving filtered
-relations with geometries â¢ 0:00:00 â ¸ [31.1/32] Saving valid features â¢
-0:00:00 â  [ 32/32] Saving final geoparquet file â¢ 0:00:00 Finished
-operation in 0:00:39 files/
-9ae2b160eb7556991148f5a2693aaf4b38bbb225c3700a6bfe9e5e54f48b987e_nofilter_compact.parquet
+1/1 â¢ 0:00:00 < 0:00:00 â¢ â ´ [ 24/32] Saving filtered ways with geometries
+â¢ 0:00:00 â  [ 25/32] Saving valid relations parts â¢ 0:00:00 â  [ 26/32]
+Saving relations inner parts â¢ 0:00:00 â  [ 27/32] Saving relations outer
+parts â¢ 0:00:00 â  [ 28/32] Saving relations outer parts with holes â¢ 0:
+00:00 â  [ 29/32] Saving relations outer parts without holes â¢ 0:00:00 â 
+[ 30/32] Saving filtered relations with geometries â¢ 0:00:00 â  [ 31/32]
+Saving all features â¢ 0:00:00 â  [ 32/32] Saving final geoparquet file â¢
+0:00:00 Finished operation in 0:00:13 files/
+78580cf29b5ba1073366a257e1909bfeee43c9f5859e48fb3b2d592028bb58aa_nofilter_compact.parquet
 ``` CLI Help output (`QuackOSM -h`): ![CLI Help output](https://
 raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/
 cli_help.png) You can find full API + more examples in the [docs](https://
 kraina-ai.github.io/quackosm/). ## How does it work? ### Basic logic QuackOSM
 utilizes `ST_ReadOSM` function from `DuckDB`'s `Spatial` extension to read raw
 data from the PBF file: - **Nodes** with coordinates and tags; - **Ways** with
 nodes refs and tags; - **Relations** with nodes and ways refs, ref roles and
```

### Comparing `quackosm-0.8.0/pyproject.toml` & `quackosm-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "QuackOSM"
-version = "0.8.0"
+version = "0.8.1"
 description = "An open-source tool for reading OpenStreetMap PBF files using DuckDB"
 authors = [
     { name = "Kamil Raczycki", email = "kraczycki@kraina.ai" },
 ]
 dependencies = [
     "geopandas>=0.6",
     "shapely>=2",
@@ -83,15 +83,14 @@
 test = [
     "pytest>=7.0.0",
     "tox-pdm",
     "pytest-mock>=3.3.0",
     "requests-mock",
     "pytest-check",
     "pytest-parametrization",
-    "pytest-xdist>=3.4.0",
     "pytest-doctestplus",
     "srai>=0.6.2",
 ]
 docs = [
     "mkdocs",
     "mkdocs-material",
     "mkdocs-mermaid2-plugin",
@@ -188,15 +187,15 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.8.0"
+current_version = "0.8.1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore(CI/CD): bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `quackosm-0.8.0/quackosm/_osm_tags_filters.py` & `quackosm-0.8.1/quackosm/_osm_tags_filters.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/quackosm/_osm_way_polygon_features.py` & `quackosm-0.8.1/quackosm/_osm_way_polygon_features.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/quackosm/_rich_progress.py` & `quackosm-0.8.1/quackosm/_rich_progress.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/quackosm/_typing.py` & `quackosm-0.8.1/quackosm/_typing.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/quackosm/cli.py` & `quackosm-0.8.1/quackosm/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from s2 import s2
 from shapely import from_geojson, from_wkt
 from shapely.geometry import Polygon, box
 
 from quackosm import __app_name__, __version__
 from quackosm._osm_tags_filters import GroupedOsmTagsFilter, OsmTagsFilter
 from quackosm._typing import is_expected_type
-from quackosm.functions import convert_geometry_to_gpq, convert_pbf_to_gpq
+from quackosm.functions import convert_geometry_to_parquet, convert_pbf_to_parquet
 from quackosm.osm_extracts import OsmExtractSource
 
 app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]}, rich_markup_mode="rich")
 
 
 def _version_callback(value: bool) -> None:
     if value:
@@ -548,15 +548,16 @@
             is_eager=True,
         ),
     ] = None,
 ) -> None:
     """
     QuackOSM CLI.
 
-    Wraps convert_pbf_to_gpq function and print final path to the saved geoparquet file at the end.
+    Wraps convert_pbf_to_parquet and convert_geometry_to_parquet functions and prints final path to
+    the saved geoparquet file at the end.
     """
     number_of_geometries_provided = sum(
         geom is not None
         for geom in (
             geom_filter_file,
             geom_filter_geocode,
             geom_filter_geojson,
@@ -602,15 +603,15 @@
     if transient_mode:
         verbosity_mode = "transient"
     elif silent_mode:
         verbosity_mode = "silent"
 
     logging.disable(logging.CRITICAL)
     if pbf_file:
-        geoparquet_path = convert_pbf_to_gpq(
+        geoparquet_path = convert_pbf_to_parquet(
             pbf_path=pbf_file,
             tags_filter=osm_tags_filter or osm_tags_filter_file,  # type: ignore
             keep_all_tags=keep_all_tags,
             geometry_filter=geometry_filter_value,
             explode_tags=explode_tags,
             ignore_cache=ignore_cache,
             working_directory=working_directory,
@@ -621,15 +622,15 @@
                 else None
             ),
             filter_osm_ids=filter_osm_ids,  # type: ignore
             save_as_wkt=wkt_result,
             verbosity_mode=verbosity_mode,
         )
     else:
-        geoparquet_path = convert_geometry_to_gpq(
+        geoparquet_path = convert_geometry_to_parquet(
             geometry_filter=geometry_filter_value,
             osm_extract_source=osm_extract_source,
             tags_filter=osm_tags_filter or osm_tags_filter_file,  # type: ignore
             keep_all_tags=keep_all_tags,
             explode_tags=explode_tags,
             ignore_cache=ignore_cache,
             working_directory=working_directory,
```

### Comparing `quackosm-0.8.0/quackosm/functions.py` & `quackosm-0.8.1/quackosm/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,32 @@
 """
 
 from collections.abc import Iterable
 from pathlib import Path
 from typing import Any, Literal, Optional, Union
 
 import geopandas as gpd
+from pandas.util._decorators import deprecate, deprecate_kwarg
 from shapely.geometry.base import BaseGeometry
 
 from quackosm._osm_tags_filters import GroupedOsmTagsFilter, OsmTagsFilter
 from quackosm._osm_way_polygon_features import OsmWayPolygonConfig
 from quackosm.osm_extracts import OsmExtractSource
 from quackosm.pbf_file_reader import PbfFileReader
 
+__all__ = [
+    "convert_pbf_to_parquet",
+    "convert_geometry_to_parquet",
+    "convert_pbf_to_geodataframe",
+    "convert_geometry_to_geodataframe",
+]
 
-def convert_pbf_to_gpq(
-    pbf_path: Union[str, Path],
+
+def convert_pbf_to_parquet(
+    pbf_path: Union[str, Path, Iterable[Union[str, Path]]],
     tags_filter: Optional[Union[OsmTagsFilter, GroupedOsmTagsFilter]] = None,
     geometry_filter: Optional[BaseGeometry] = None,
     result_file_path: Optional[Union[str, Path]] = None,
     keep_all_tags: bool = False,
     explode_tags: Optional[bool] = None,
     ignore_cache: bool = False,
     filter_osm_ids: Optional[list[str]] = None,
@@ -33,15 +41,16 @@
     debug_memory: bool = False,
     debug_times: bool = False,
 ) -> Path:
     """
     Convert PBF file to GeoParquet file.
 
     Args:
-        pbf_path (Union[str, Path]): Pbf file to be parsed to GeoParquet.
+        pbf_path (Union[str, Path, Iterable[Union[str, Path]]]):
+            Path or list of paths of `*.osm.pbf` files to be parsed.
         tags_filter (Union[OsmTagsFilter, GroupedOsmTagsFilter], optional): A dictionary
             specifying which tags to download.
             The keys should be OSM tags (e.g. `building`, `amenity`).
             The values should either be `True` for retrieving all objects with the tag,
             string for retrieving a single tag-value pair
             or list of strings for retrieving all values specified in the list.
             `tags={'leisure': 'park}` would return parks from the area.
@@ -88,16 +97,15 @@
         Path: Path to the generated GeoParquet file.
 
     Examples:
         Get OSM data from a PBF file.
 
         Tags will be kept in a single column.
         >>> import quackosm as qosm
-        >>> gpq_path = qosm.convert_pbf_to_gpq(monaco_pbf_path)
-        Finished operation in ...
+        >>> gpq_path = qosm.convert_pbf_to_parquet(monaco_pbf_path) # doctest: +IGNORE_RESULT
         >>> gpq_path.as_posix()
         'files/monaco_nofilter_noclip_compact.parquet'
 
         Inspect the file with duckdb
         >>> import duckdb
         >>> duckdb.load_extension('spatial')
         >>> duckdb.read_parquet(str(gpq_path)).project(
@@ -133,19 +141,18 @@
         ├──────────────────┴──────────────────────┴──────────────────────────────────────────────┤
         │ 7906 rows (20 shown)                                                         3 columns │
         └────────────────────────────────────────────────────────────────────────────────────────┘
 
         Get only buildings, amenities and highways from a PBF file.
 
         Tags will be split into separate columns because of applying the filter.
-        >>> gpq_path = qosm.convert_pbf_to_gpq(
+        >>> gpq_path = qosm.convert_pbf_to_parquet(
         ...     monaco_pbf_path,
         ...     tags_filter={"building": True, "amenity": True, "highway": True}
-        ... )
-        Finished operation in ...
+        ... ) # doctest: +IGNORE_RESULT
         >>> gpq_path.as_posix()
         'files/monaco_6593ca69098459d039054bc5fe0a87c56681e29a5f59d38ce3485c03cb0e9374_noclip_exploded.parquet'
 
         Inspect the file with duckdb
         >>> duckdb.read_parquet(str(gpq_path)).project(
         ...     "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)"
         ... ).order("feature_id") # doctest: +SKIP
@@ -180,24 +187,23 @@
         │ 5772 rows (20 shown)                                                         5 columns │
         └────────────────────────────────────────────────────────────────────────────────────────┘
 
         Get features for Malé - the capital city of Maldives
 
         Tags will be kept in a single column.
         >>> from shapely.geometry import box
-        >>> gpq_path = qosm.convert_pbf_to_gpq(
+        >>> gpq_path = qosm.convert_pbf_to_parquet(
         ...     maldives_pbf_path,
         ...     geometry_filter=box(
         ...         minx=73.4975872,
         ...         miny=4.1663240,
         ...         maxx=73.5215528,
         ...         maxy=4.1818121
         ...     )
-        ... )
-        Finished operation in ...
+        ... ) # doctest: +IGNORE_RESULT
         >>> gpq_path.as_posix()
         'files/maldives_nofilter_4eeabb20ccd8aefeaa80b9a46a202ab985fd454760823b7012cc7778498a085b_compact.parquet'
 
         Inspect the file with duckdb
         >>> duckdb.read_parquet(str(gpq_path)).project(
         ...     "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)"
         ... ).order("feature_id") # doctest: +SKIP
@@ -236,26 +242,26 @@
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         verbosity_mode=verbosity_mode,
         debug_memory=debug_memory,
         debug_times=debug_times,
-    ).convert_pbf_to_gpq(
+    ).convert_pbf_to_parquet(
         pbf_path=pbf_path,
         result_file_path=result_file_path,
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
         save_as_wkt=save_as_wkt,
     )
 
 
-def convert_geometry_to_gpq(
+def convert_geometry_to_parquet(
     geometry_filter: BaseGeometry = None,
     osm_extract_source: Union[OsmExtractSource, str] = OsmExtractSource.geofabrik,
     tags_filter: Optional[Union[OsmTagsFilter, GroupedOsmTagsFilter]] = None,
     result_file_path: Optional[Union[str, Path]] = None,
     keep_all_tags: bool = False,
     explode_tags: Optional[bool] = None,
     ignore_cache: bool = False,
@@ -334,16 +340,15 @@
 
         >>> import quackosm as qosm
         >>> from shapely import from_wkt
         >>> wkt = (
         ...     "POLYGON ((7.41644 43.73598, 7.41644 43.73142, 7.42378 43.73142,"
         ...     " 7.42378 43.73598, 7.41644 43.73598))"
         ... )
-        >>> gpq_path = qosm.convert_geometry_to_gpq(from_wkt(wkt))
-        Finished operation in ...
+        >>> gpq_path = qosm.convert_geometry_to_parquet(from_wkt(wkt)) # doctest: +IGNORE_RESULT
         >>> gpq_path.as_posix()
         'files/bf4b33debfd6d3e605555340606df6ce7eea934958c1f3477aca0ccf79e7929f_nofilter_compact.parquet'
 
         Inspect the file with duckdb
         >>> import duckdb
         >>> duckdb.load_extension('spatial')
         >>> duckdb.read_parquet(str(gpq_path)).project(
@@ -378,19 +383,18 @@
         │ way/952419573    │ {highway=primary, …  │ LINESTRING (7.4173897 43.7316435, 7.417372…  │
         ├──────────────────┴──────────────────────┴──────────────────────────────────────────────┤
         │ 1384 rows (20 shown)                                                                   │
         └────────────────────────────────────────────────────────────────────────────────────────┘
 
         Making sure that you are using specific OSM extract source - here Geofabrik.
 
-        >>> gpq_path = qosm.convert_geometry_to_gpq(
+        >>> gpq_path = qosm.convert_geometry_to_parquet(
         ...     from_wkt(wkt),
         ...     osm_extract_source='Geofabrik',
-        ... )
-        Finished operation in ...
+        ... ) # doctest: +IGNORE_RESULT
         >>> gpq_path.as_posix()
         'files/bf4b33debfd6d3e605555340606df6ce7eea934958c1f3477aca0ccf79e7929f_nofilter_compact.parquet'
 
         Inspect the file with duckdb
         >>> duckdb.read_parquet(str(gpq_path)).project(
         ...     "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)"
         ... ).order("feature_id") # doctest: +SKIP
@@ -431,26 +435,27 @@
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         osm_extract_source=osm_extract_source,
         verbosity_mode=verbosity_mode,
         allow_uncovered_geometry=allow_uncovered_geometry,
         debug_memory=debug_memory,
         debug_times=debug_times,
-    ).convert_geometry_filter_to_gpq(
+    ).convert_geometry_to_parquet(
         result_file_path=result_file_path,
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
         save_as_wkt=save_as_wkt,
     )
 
 
-def get_features_gdf(
-    file_paths: Union[str, Path, Iterable[Union[str, Path]]],
+@deprecate_kwarg(old_arg_name="file_paths", new_arg_name="pbf_path")  # type: ignore
+def convert_pbf_to_geodataframe(
+    pbf_path: Union[str, Path, Iterable[Union[str, Path]]],
     tags_filter: Optional[Union[OsmTagsFilter, GroupedOsmTagsFilter]] = None,
     geometry_filter: Optional[BaseGeometry] = None,
     keep_all_tags: bool = False,
     explode_tags: Optional[bool] = None,
     ignore_cache: bool = False,
     filter_osm_ids: Optional[list[str]] = None,
     working_directory: Union[str, Path] = "files",
@@ -462,15 +467,15 @@
     """
     Get features GeoDataFrame from a PBF file or list of PBF files.
 
     Function can parse multiple PBF files and returns a single GeoDataFrame with loaded
     OSM objects.
 
     Args:
-        file_paths (Union[str, Path, Iterable[Union[str, Path]]]):
+        pbf_path (Union[str, Path, Iterable[Union[str, Path]]]):
             Path or list of paths of `*.osm.pbf` files to be parsed.
         tags_filter (Union[OsmTagsFilter, GroupedOsmTagsFilter], optional): A dictionary
             specifying which tags to download.
             The keys should be OSM tags (e.g. `building`, `amenity`).
             The values should either be `True` for retrieving all objects with the tag,
             string for retrieving a single tag-value pair
             or list of strings for retrieving all values specified in the list.
@@ -512,16 +517,15 @@
         gpd.GeoDataFrame: GeoDataFrame with OSM features.
 
     Examples:
         Get OSM data from a PBF file.
 
         Tags will be kept in a single column.
         >>> import quackosm as qosm
-        >>> gdf = qosm.get_features_gdf(monaco_pbf_path)
-        Finished operation in ...
+        >>> gdf = qosm.convert_pbf_to_geodataframe(monaco_pbf_path) # doctest: +IGNORE_RESULT
         >>> gdf.sort_index()
                                                       tags                      geometry
         feature_id
         node/10005045289                {'shop': 'bakery'}      POINT (7.42245 43.73105)
         node/10020887517  {'leisure': 'swimming_pool', ...      POINT (7.41316 43.73384)
         node/10021298117  {'leisure': 'swimming_pool', ...      POINT (7.42777 43.74277)
         node/10021298717  {'leisure': 'swimming_pool', ...      POINT (7.42630 43.74097)
@@ -534,18 +538,17 @@
         way/993121275      {'building': 'yes', 'name': ...  POLYGON ((7.43214 43.7481...
         <BLANKLINE>
         [7906 rows x 2 columns]
 
         Get only buildings from a PBF file.
 
         Tags will be split into separate columns because of applying the filter.
-        >>> gdf = qosm.get_features_gdf(
+        >>> gdf = qosm.convert_pbf_to_geodataframe(
         ...     monaco_pbf_path, tags_filter={"building": True}
-        ... )
-        Finished operation in ...
+        ... ) # doctest: +IGNORE_RESULT
         >>> gdf.sort_index()
                               building                                           geometry
         feature_id
         relation/11384697          yes  POLYGON ((7.42749 43.73125, 7.42672 43.73063, ...
         relation/11484092        hotel  POLYGON ((7.41790 43.72483, 7.41783 43.72486, ...
         relation/11484093   apartments  POLYGON ((7.41815 43.72561, 7.41836 43.72547, ...
         relation/11484094  residential  POLYGON ((7.41753 43.72583, 7.41753 43.72563, ...
@@ -559,24 +562,23 @@
         <BLANKLINE>
         [1283 rows x 2 columns]
 
         Get features for Malé - the capital city of Maldives
 
         Tags will be kept in a single column.
         >>> from shapely.geometry import box
-        >>> gdf = qosm.get_features_gdf(
+        >>> gdf = qosm.convert_pbf_to_geodataframe(
         ...     maldives_pbf_path,
         ...     geometry_filter=box(
         ...         minx=73.4975872,
         ...         miny=4.1663240,
         ...         maxx=73.5215528,
         ...         maxy=4.1818121
         ...     )
-        ... )
-        Finished operation in ...
+        ... ) # doctest: +IGNORE_RESULT
         >>> gdf.sort_index()
                                                    tags                                     geometry
         feature_id
         node/10010180778  {'brand': 'Ooredoo', 'bran...                     POINT (73.51790 4.17521)
         node/10062500171  {'contact:facebook': 'http...                     POINT (73.50958 4.17245)
         node/10078084764  {'addr:city': 'Male'', 'ad...                     POINT (73.50480 4.17267)
         node/10078086040  {'addr:city': 'Malé', 'add...                     POINT (73.50317 4.17596)
@@ -591,30 +593,29 @@
         [2140 rows x 2 columns]
 
 
         Get features grouped into catgegories for Christmas Island
 
         Even though we apply the filter, the tags will be kept in a single column
         because of manual `explode_tags` value setting.
-        >>> gdf = qosm.get_features_gdf(
+        >>> gdf = qosm.convert_pbf_to_geodataframe(
         ...     kiribati_pbf_path,
         ...     tags_filter={
         ...         "highway": {"highway": True},
         ...         "tree": {"natural": "tree"},
         ...         "building": {"building": True},
         ...     },
         ...     geometry_filter=box(
         ...         minx=-157.6046004,
         ...         miny=1.6724409,
         ...         maxx=-157.1379507,
         ...         maxy=2.075240
         ...     ),
         ...     explode_tags=False,
-        ... )
-        Finished operation in ...
+        ... ) # doctest: +IGNORE_RESULT
         >>> gdf.sort_index()
                                                   tags                                      geometry
         feature_id
         node/2377661784  {'building': 'building=ruin'}                    POINT (-157.18826 1.75186)
         node/4150479646       {'tree': 'natural=tree'}                    POINT (-157.36152 1.98363)
         node/4396875565       {'tree': 'natural=tree'}                    POINT (-157.36143 1.98364)
         node/4396875566       {'tree': 'natural=tree'}                    POINT (-157.36135 1.98364)
@@ -632,24 +633,24 @@
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         verbosity_mode=verbosity_mode,
         debug_memory=debug_memory,
         debug_times=debug_times,
-    ).get_features_gdf(
-        file_paths=file_paths,
+    ).convert_pbf_to_geodataframe(
+        pbf_path=pbf_path,
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
     )
 
 
-def get_features_gdf_from_geometry(
+def convert_geometry_to_geodataframe(
     geometry_filter: BaseGeometry = None,
     osm_extract_source: Union[OsmExtractSource, str] = OsmExtractSource.geofabrik,
     tags_filter: Optional[Union[OsmTagsFilter, GroupedOsmTagsFilter]] = None,
     keep_all_tags: bool = False,
     explode_tags: Optional[bool] = None,
     ignore_cache: bool = False,
     filter_osm_ids: Optional[list[str]] = None,
@@ -720,16 +721,15 @@
 
         >>> import quackosm as qosm
         >>> from shapely import from_wkt
         >>> wkt = (
         ...     "POLYGON ((7.41644 43.73598, 7.41644 43.73142, 7.42378 43.73142,"
         ...     " 7.42378 43.73598, 7.41644 43.73598))"
         ... )
-        >>> gdf = qosm.get_features_gdf_from_geometry(from_wkt(wkt))
-        Finished operation in ...
+        >>> gdf = qosm.convert_geometry_to_geodataframe(from_wkt(wkt)) # doctest: +IGNORE_RESULT
         >>> gdf.sort_index()
                                                   tags                                      geometry
         feature_id
         node/10068880335     {'amenity': 'bench', '...                      POINT (7.41869 43.73215)
         node/10196648824  {'contact:city': 'Monaco'...                      POINT (7.41938 43.73375)
         node/10601158089  {'addr:city': 'Monaco', '...                      POINT (7.42131 43.73362)
         node/10672624925  {'addr:city': 'Monaco', '...                      POINT (7.42157 43.73517)
@@ -741,19 +741,18 @@
         way/952419572     {'highway': 'primary', 'j...  LINESTRING (7.41731 43.73168, 7.41728 43....
         way/952419573     {'highway': 'primary', 'j...  LINESTRING (7.41739 43.73164, 7.41737 43....
         <BLANKLINE>
         [1384 rows x 2 columns]
 
         Making sure that you are using specific OSM extract source - here Geofabrik.
 
-        >>> gdf = qosm.get_features_gdf_from_geometry(
+        >>> gdf = qosm.convert_geometry_to_geodataframe(
         ...     from_wkt(wkt),
         ...     osm_extract_source='Geofabrik',
-        ... )
-        Finished operation in ...
+        ... ) # doctest: +IGNORE_RESULT
         >>> gdf.sort_index()
                                                   tags                                      geometry
         feature_id
         node/10068880335       {'amenity': 'bench',...                      POINT (7.41869 43.73215)
         node/10196648824  {'contact:city': 'Monaco'...                      POINT (7.41938 43.73375)
         node/10601158089    {'addr:city': 'Monaco',...                      POINT (7.42131 43.73362)
         node/10672624925    {'addr:city': 'Monaco',...                      POINT (7.42157 43.73517)
@@ -773,13 +772,42 @@
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         osm_extract_source=osm_extract_source,
         verbosity_mode=verbosity_mode,
         allow_uncovered_geometry=allow_uncovered_geometry,
         debug_memory=debug_memory,
         debug_times=debug_times,
-    ).get_features_gdf_from_geometry(
+    ).convert_geometry_to_geodataframe(
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
     )
+
+
+convert_pbf_to_gpq = deprecate(
+    "convert_pbf_to_gpq",
+    convert_pbf_to_parquet,
+    "0.8.1",
+    msg="Use `convert_pbf_to_parquet` instead. Deprecated since 0.8.1 version.",
+)
+
+convert_geometry_to_gpq = deprecate(
+    "convert_geometry_to_gpq",
+    convert_geometry_to_parquet,
+    "0.8.1",
+    msg="Use `convert_geometry_to_parquet` instead. Deprecated since 0.8.1 version.",
+)
+
+get_features_gdf = deprecate(
+    "get_features_gdf",
+    convert_pbf_to_geodataframe,
+    "0.8.1",
+    msg="Use `convert_pbf_to_geodataframe` instead. Deprecated since 0.8.1 version.",
+)
+
+get_features_gdf_from_geometry = deprecate(
+    "get_features_gdf_from_geometry",
+    convert_geometry_to_geodataframe,
+    "0.8.1",
+    msg="Use `convert_geometry_to_geodataframe` instead. Deprecated since 0.8.1 version.",
+)
```

### Comparing `quackosm-0.8.0/quackosm/osm_extracts/__init__.py` & `quackosm-0.8.1/quackosm/osm_extracts/__init__.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/quackosm/osm_extracts/_poly_parser.py` & `quackosm-0.8.1/quackosm/osm_extracts/_poly_parser.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/quackosm/osm_extracts/bbbike.py` & `quackosm-0.8.1/quackosm/osm_extracts/bbbike.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/quackosm/osm_extracts/geofabrik.py` & `quackosm-0.8.1/quackosm/osm_extracts/geofabrik.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/quackosm/osm_extracts/osm_fr.py` & `quackosm-0.8.1/quackosm/osm_extracts/osm_fr.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/quackosm/osm_way_polygon_features.json` & `quackosm-0.8.1/quackosm/osm_way_polygon_features.json`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/quackosm/pbf_file_reader.py` & `quackosm-0.8.1/quackosm/pbf_file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import geopandas as gpd
 import polars as pl
 import psutil
 import pyarrow as pa
 import pyarrow.parquet as pq
 import shapely.wkt as wktlib
 from geoarrow.pyarrow import io
+from pandas.util._decorators import deprecate, deprecate_kwarg
 from pyarrow_ops import drop_duplicates
 from shapely.geometry import LinearRing, Polygon
 from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
 
 from quackosm._constants import FEATURES_INDEX, GEOMETRY_COLUMN, WGS84_CRS
 from quackosm._exceptions import EmptyResultWarning, InvalidGeometryFilter
 from quackosm._osm_tags_filters import (
@@ -200,29 +201,58 @@
 
         self.osm_way_polygon_features_config: OsmWayPolygonConfig = (
             osm_way_polygon_features_config
             if isinstance(osm_way_polygon_features_config, OsmWayPolygonConfig)
             else parse_dict_to_config_object(osm_way_polygon_features_config)
         )
 
-    def convert_pbf_to_gpq(
+        self.convert_pbf_to_gpq = deprecate(
+            "convert_pbf_to_gpq",
+            self.convert_pbf_to_parquet,
+            "0.8.1",
+            msg="Use `convert_pbf_to_parquet` instead. Deprecated since 0.8.1 version.",
+        )
+
+        self.convert_geometry_filter_to_gpq = deprecate(
+            "convert_geometry_filter_to_gpq",
+            self.convert_geometry_to_parquet,
+            "0.8.1",
+            msg="Use `convert_geometry_to_parquet` instead. Deprecated since 0.8.1 version.",
+        )
+
+        self.get_features_gdf = deprecate(
+            "get_features_gdf",
+            self.convert_pbf_to_geodataframe,
+            "0.8.1",
+            msg="Use `convert_pbf_to_geodataframe` instead. Deprecated since 0.8.1 version.",
+        )
+
+        self.get_features_gdf_from_geometry = deprecate(
+            "get_features_gdf_from_geometry",
+            self.convert_geometry_to_geodataframe,
+            "0.8.1",
+            msg="Use `convert_geometry_to_geodataframe` instead. Deprecated since 0.8.1 version.",
+        )
+
+    def convert_pbf_to_parquet(
         self,
-        pbf_path: Union[str, Path],
+        pbf_path: Union[str, Path, Iterable[Union[str, Path]]],
         result_file_path: Optional[Union[str, Path]] = None,
         keep_all_tags: bool = False,
         explode_tags: Optional[bool] = None,
         ignore_cache: bool = False,
         filter_osm_ids: Optional[list[str]] = None,
         save_as_wkt: bool = False,
     ) -> Path:
         """
         Convert PBF file to GeoParquet file.
 
         Args:
-            pbf_path (Union[str, Path]): Pbf file to be parsed to GeoParquet.
+            pbf_path (Union[str, Path, Iterable[Union[str, Path]]]):
+                Path or list of paths of `*.osm.pbf` files to be parsed.
             result_file_path (Union[str, Path], optional): Where to save
                 the geoparquet file. If not provided, will be generated based on hashes
                 from provided tags filter and geometry filter. Defaults to `None`.
             keep_all_tags (bool, optional): Works only with the `tags_filter` parameter.
                 Whether to keep all tags related to the element, or return only those defined
                 in the `tags_filter`. When `True`, will override the optional grouping defined
                 in the `tags_filter`. Defaults to `False`.
@@ -238,21 +268,147 @@
             save_as_wkt (bool): Whether to save the file with geometry in the WKT form instead
                 of WKB. If `True`, it will be saved as a `.parquet` file, because it won't be
                 in the GeoParquet standard. Defaults to `False`.
 
         Returns:
             Path: Path to the generated GeoParquet file.
         """
-        created_task_progress_tracker = False
-        if self.task_progress_tracker is None or not self.task_progress_tracker.is_new():
-            created_task_progress_tracker = True
-            self.task_progress_tracker = TaskProgressTracker(
-                verbosity_mode=self.verbosity_mode, debug=self.debug_times
+        if isinstance(pbf_path, (str, Path)):
+            pbf_path = [pbf_path]
+        else:
+            pbf_path = list(pbf_path)
+
+        if filter_osm_ids is None:
+            filter_osm_ids = []
+
+        if explode_tags is None:
+            explode_tags = (
+                self.tags_filter is not None and self.is_tags_filter_positive and not keep_all_tags
+            )
+
+        parsed_geoparquet_files = []
+        total_files = len(pbf_path)
+        self.task_progress_tracker = TaskProgressTracker(
+            verbosity_mode=self.verbosity_mode,
+            total_major_steps=total_files,
+            debug=self.debug_memory,
+        )
+        if total_files == 1:
+            parsed_geoparquet_file = self._convert_single_pbf_to_parquet(
+                pbf_path[0],
+                result_file_path=result_file_path,
+                keep_all_tags=keep_all_tags,
+                explode_tags=explode_tags,
+                ignore_cache=ignore_cache,
+                filter_osm_ids=filter_osm_ids,
+                save_as_wkt=save_as_wkt,
             )
+            self.task_progress_tracker.stop()
+            return parsed_geoparquet_file
+        else:
+            result_file_path = Path(
+                result_file_path
+                or self._generate_result_file_path(
+                    pbf_path,
+                    filter_osm_ids=filter_osm_ids,
+                    keep_all_tags=keep_all_tags,
+                    explode_tags=explode_tags,
+                    save_as_wkt=save_as_wkt,
+                )
+            )
+
+            if result_file_path.exists() and not ignore_cache:
+                return result_file_path
+            elif result_file_path.with_suffix(".geoparquet").exists() and not ignore_cache:
+                warnings.warn(
+                    (
+                        "Found existing result file with `.geoparquet` extension."
+                        " Users are enouraged to change the extension manually"
+                        " to `.parquet` for old files. Files with `.geoparquet`"
+                        " extension will be backwards supported, but reusing them"
+                        " will result in this warning."
+                    ),
+                    DeprecationWarning,
+                    stacklevel=0,
+                )
+                return result_file_path.with_suffix(".geoparquet")
+
+            for file_idx, single_pbf_path in enumerate(pbf_path):
+                self.task_progress_tracker.reset_steps(file_idx + 1)
+                parsed_geoparquet_file = self._convert_single_pbf_to_parquet(
+                    single_pbf_path,
+                    keep_all_tags=keep_all_tags,
+                    explode_tags=explode_tags,
+                    ignore_cache=ignore_cache,
+                    filter_osm_ids=filter_osm_ids,
+                    save_as_wkt=save_as_wkt,
+                )
+                parsed_geoparquet_files.append(parsed_geoparquet_file)
 
+            if parsed_geoparquet_files:
+                with tempfile.TemporaryDirectory(
+                    dir=self.working_directory.resolve()
+                ) as tmp_dir_name:
+                    if self.debug_memory:
+                        tmp_dir_name = self._prepare_debug_directory()  # type: ignore[assignment] # noqa: PLW2901
+
+                    try:
+                        joined_parquet_table = self._drop_duplicated_features_in_pyarrow_table(
+                            parsed_geoparquet_files
+                        )
+                    except pa.ArrowInvalid:
+                        tmp_dir_path = Path(tmp_dir_name)
+                        try:
+                            joined_parquet_table = self._drop_duplicated_features_in_joined_table(
+                                parsed_geoparquet_files, tmp_dir_path
+                            )
+                        except MemoryError:
+                            joined_parquet_table = (
+                                self._drop_duplicated_features_in_joined_table_one_by_one(
+                                    parsed_geoparquet_files, tmp_dir_path
+                                )
+                            )
+            else:
+                warnings.warn(
+                    "Found 0 extracts covering the geometry. Returning empty result.",
+                    EmptyResultWarning,
+                    stacklevel=0,
+                )
+                if save_as_wkt:
+                    geometry_column = ga.as_wkt(gpd.GeoSeries([], crs=WGS84_CRS))
+                else:
+                    geometry_column = ga.as_wkb(gpd.GeoSeries([], crs=WGS84_CRS))
+                joined_parquet_table = pa.table(
+                    [pa.array([], type=pa.string()), geometry_column],
+                    names=[FEATURES_INDEX, GEOMETRY_COLUMN],
+                )
+
+            if save_as_wkt:
+                pq.write_table(joined_parquet_table, result_file_path)
+            else:
+                io.write_geoparquet_table(
+                    joined_parquet_table,
+                    result_file_path,
+                    primary_geometry_column=GEOMETRY_COLUMN,
+                )
+
+            self.task_progress_tracker.stop()
+
+        return Path(result_file_path)
+
+    def _convert_single_pbf_to_parquet(
+        self,
+        pbf_path: Union[str, Path],
+        result_file_path: Optional[Union[str, Path]] = None,
+        keep_all_tags: bool = False,
+        explode_tags: Optional[bool] = None,
+        ignore_cache: bool = False,
+        filter_osm_ids: Optional[list[str]] = None,
+        save_as_wkt: bool = False,
+    ) -> Path:
         if filter_osm_ids is None:
             filter_osm_ids = []
 
         if explode_tags is None:
             explode_tags = (
                 self.tags_filter is not None and self.is_tags_filter_positive and not keep_all_tags
             )
@@ -284,18 +440,16 @@
                 )
 
                 return parsed_geoparquet_file
             finally:
                 if self.connection is not None:
                     self.connection.close()
                     self.connection = None
-                if created_task_progress_tracker:
-                    self.task_progress_tracker.stop()
 
-    def convert_geometry_filter_to_gpq(
+    def convert_geometry_to_parquet(
         self,
         result_file_path: Optional[Union[str, Path]] = None,
         keep_all_tags: bool = False,
         explode_tags: Optional[bool] = None,
         ignore_cache: bool = False,
         filter_osm_ids: Optional[list[str]] = None,
         save_as_wkt: bool = False,
@@ -350,136 +504,63 @@
                 filter_osm_ids=filter_osm_ids,
                 keep_all_tags=keep_all_tags,
                 explode_tags=explode_tags,
                 save_as_wkt=save_as_wkt,
             )
         )
 
+        if result_file_path.exists() and not ignore_cache:
+            return result_file_path
+        elif result_file_path.with_suffix(".geoparquet").exists() and not ignore_cache:
+            warnings.warn(
+                (
+                    "Found existing result file with `.geoparquet` extension."
+                    " Users are enouraged to change the extension manually"
+                    " to `.parquet` for old files. Files with `.geoparquet`"
+                    " extension will be backwards supported, but reusing them"
+                    " will result in this warning."
+                ),
+                DeprecationWarning,
+                stacklevel=0,
+            )
+            return result_file_path.with_suffix(".geoparquet")
+
         matching_extracts = find_smallest_containing_extract(
             self.geometry_filter,
             self.osm_extract_source,
             allow_uncovered_geometry=self.allow_uncovered_geometry,
         )
+        pbf_files = download_extracts_pbf_files(matching_extracts, self.working_directory)
+        return self.convert_pbf_to_parquet(
+            pbf_files,
+            result_file_path=result_file_path,
+            keep_all_tags=keep_all_tags,
+            explode_tags=explode_tags,
+            ignore_cache=ignore_cache,
+            filter_osm_ids=filter_osm_ids,
+            save_as_wkt=save_as_wkt,
+        )
 
-        if len(matching_extracts) == 1:
-            pbf_files = download_extracts_pbf_files(matching_extracts, self.working_directory)
-            return self.convert_pbf_to_gpq(
-                pbf_files[0],
-                result_file_path=result_file_path,
-                keep_all_tags=keep_all_tags,
-                explode_tags=explode_tags,
-                ignore_cache=ignore_cache,
-                filter_osm_ids=filter_osm_ids,
-                save_as_wkt=save_as_wkt,
-            )
-        else:
-            if result_file_path.with_suffix(".geoparquet").exists() and not ignore_cache:
-                warnings.warn(
-                    (
-                        "Found existing result file with `.geoparquet` extension."
-                        " Users are enouraged to change the extension manually"
-                        " to `.parquet` for old files. Files with `.geoparquet`"
-                        " extension will be backwards supported, but reusing them"
-                        " will result in this warning."
-                    ),
-                    DeprecationWarning,
-                    stacklevel=0,
-                )
-                return result_file_path.with_suffix(".geoparquet")
-            if not result_file_path.exists() or ignore_cache:
-                pbf_files = download_extracts_pbf_files(matching_extracts, self.working_directory)
-
-                parsed_geoparquet_files = []
-                total_files = len(pbf_files)
-                self.task_progress_tracker = TaskProgressTracker(
-                    verbosity_mode=self.verbosity_mode,
-                    total_major_steps=total_files,
-                    debug=self.debug_times,
-                )
-                for file_idx, file_path in enumerate(pbf_files):
-                    self.task_progress_tracker.reset_steps(file_idx + 1)
-                    parsed_geoparquet_file = self.convert_pbf_to_gpq(
-                        file_path,
-                        keep_all_tags=keep_all_tags,
-                        explode_tags=explode_tags,
-                        ignore_cache=ignore_cache,
-                        filter_osm_ids=filter_osm_ids,
-                        save_as_wkt=save_as_wkt,
-                    )
-                    parsed_geoparquet_files.append(parsed_geoparquet_file)
-
-                if parsed_geoparquet_files:
-                    with tempfile.TemporaryDirectory(
-                        dir=self.working_directory.resolve()
-                    ) as tmp_dir_name:
-                        if self.debug_memory:
-                            tmp_dir_name = self._prepare_debug_directory()  # type: ignore[assignment] # noqa: PLW2901
-
-                        try:
-                            joined_parquet_table = self._drop_duplicated_features_in_pyarrow_table(
-                                parsed_geoparquet_files
-                            )
-                        except pa.ArrowInvalid:
-                            tmp_dir_path = Path(tmp_dir_name)
-                            try:
-                                joined_parquet_table = (
-                                    self._drop_duplicated_features_in_joined_table(
-                                        parsed_geoparquet_files, tmp_dir_path
-                                    )
-                                )
-                            except MemoryError:
-                                joined_parquet_table = (
-                                    self._drop_duplicated_features_in_joined_table_one_by_one(
-                                        parsed_geoparquet_files, tmp_dir_path
-                                    )
-                                )
-                else:
-                    warnings.warn(
-                        "Found 0 extracts covering the geometry. Returning empty result.",
-                        EmptyResultWarning,
-                        stacklevel=0,
-                    )
-                    if save_as_wkt:
-                        geometry_column = ga.as_wkt(gpd.GeoSeries([], crs=WGS84_CRS))
-                    else:
-                        geometry_column = ga.as_wkb(gpd.GeoSeries([], crs=WGS84_CRS))
-                    joined_parquet_table = pa.table(
-                        [pa.array([], type=pa.string()), geometry_column],
-                        names=[FEATURES_INDEX, GEOMETRY_COLUMN],
-                    )
-
-                if save_as_wkt:
-                    pq.write_table(joined_parquet_table, result_file_path)
-                else:
-                    io.write_geoparquet_table(
-                        joined_parquet_table,
-                        result_file_path,
-                        primary_geometry_column=GEOMETRY_COLUMN,
-                    )
-
-                self.task_progress_tracker.stop()
-
-        return Path(result_file_path)
-
-    def get_features_gdf(
+    @deprecate_kwarg(old_arg_name="file_paths", new_arg_name="pbf_path")  # type: ignore
+    def convert_pbf_to_geodataframe(
         self,
-        file_paths: Union[str, Path, Iterable[Union[str, Path]]],
+        pbf_path: Union[str, Path, Iterable[Union[str, Path]]],
         keep_all_tags: bool = False,
         explode_tags: Optional[bool] = None,
         ignore_cache: bool = False,
         filter_osm_ids: Optional[list[str]] = None,
     ) -> gpd.GeoDataFrame:
         """
         Get features GeoDataFrame from a list of PBF files.
 
         Function parses multiple PBF files and returns a single GeoDataFrame with parsed
         OSM objects.
 
         Args:
-            file_paths (Union[str, Path, Iterable[Union[str, Path]]]):
+            pbf_path (Union[str, Path, Iterable[Union[str, Path]]]):
                 Path or list of paths of `*.osm.pbf` files to be parsed.
             keep_all_tags (bool, optional): Works only with the `tags_filter` parameter.
                 Whether to keep all tags related to the element, or return only those defined
                 in the `tags_filter`. When `True`, will override the optional grouping defined
                 in the `tags_filter`. Defaults to `False`.
             explode_tags (bool, optional): Whether to split tags into columns based on OSM tag keys.
                 If `None`, will be set based on `tags_filter` and `keep_all_tags` parameters.
@@ -490,87 +571,33 @@
             filter_osm_ids: (list[str], optional): List of OSM features ids to read from the file.
                 Have to be in the form of 'node/<id>', 'way/<id>' or 'relation/<id>'.
                 Defaults to an empty list.
 
         Returns:
             gpd.GeoDataFrame: GeoDataFrame with OSM features.
         """
-        if isinstance(file_paths, (str, Path)):
-            file_paths = [file_paths]
-
-        if filter_osm_ids is None:
-            filter_osm_ids = []
-
-        if explode_tags is None:
-            explode_tags = (
-                self.tags_filter is not None and self.is_tags_filter_positive and not keep_all_tags
-            )
+        if isinstance(pbf_path, (str, Path)):
+            pbf_path = [pbf_path]
 
-        parsed_geoparquet_files = []
-        total_files = len(list(file_paths))
-        self.task_progress_tracker = TaskProgressTracker(
-            verbosity_mode=self.verbosity_mode,
-            total_major_steps=total_files,
-            debug=self.debug_memory,
+        parsed_geoparquet_file = self.convert_pbf_to_parquet(
+            pbf_path=pbf_path,
+            keep_all_tags=keep_all_tags,
+            explode_tags=explode_tags,
+            ignore_cache=ignore_cache,
+            filter_osm_ids=filter_osm_ids,
         )
-        for file_idx, file_path in enumerate(file_paths):
-            self.task_progress_tracker.reset_steps(file_idx + 1)
-            parsed_geoparquet_file = self.convert_pbf_to_gpq(
-                file_path,
-                keep_all_tags=keep_all_tags,
-                explode_tags=explode_tags,
-                ignore_cache=ignore_cache,
-                filter_osm_ids=filter_osm_ids,
-            )
-            parsed_geoparquet_files.append(parsed_geoparquet_file)
-
-        if parsed_geoparquet_files:
-            with tempfile.TemporaryDirectory(dir=self.working_directory.resolve()) as tmp_dir_name:
-                if self.debug_memory:
-                    tmp_dir_name = self._prepare_debug_directory()  # type: ignore[assignment] # noqa: PLW2901
-
-                try:
-                    joined_parquet_table = self._drop_duplicated_features_in_pyarrow_table(
-                        parsed_geoparquet_files
-                    )
-                except pa.ArrowInvalid:
-                    tmp_dir_path = Path(tmp_dir_name)
-                    try:
-                        joined_parquet_table = self._drop_duplicated_features_in_joined_table(
-                            parsed_geoparquet_files, tmp_dir_path
-                        )
-                    except MemoryError:
-                        joined_parquet_table = (
-                            self._drop_duplicated_features_in_joined_table_one_by_one(
-                                parsed_geoparquet_files, tmp_dir_path
-                            )
-                        )
-
-                gdf_parquet = gpd.GeoDataFrame(
-                    data=joined_parquet_table.drop(GEOMETRY_COLUMN).to_pandas(
-                        maps_as_pydicts="strict"
-                    ),
-                    geometry=ga.to_geopandas(joined_parquet_table.column(GEOMETRY_COLUMN)),
-                ).set_index(FEATURES_INDEX)
-        else:
-            warnings.warn(
-                "Found 0 extracts covering the geometry. Returning empty result.",
-                EmptyResultWarning,
-                stacklevel=0,
-            )
-            gdf_parquet = gpd.GeoDataFrame(
-                data={FEATURES_INDEX: []},
-                geometry=gpd.GeoSeries([], crs=WGS84_CRS),
-            ).set_index(FEATURES_INDEX)
-
-        self.task_progress_tracker.stop()
+        joined_parquet_table = io.read_geoparquet_table(parsed_geoparquet_file)
+        gdf_parquet = gpd.GeoDataFrame(
+            data=joined_parquet_table.drop(GEOMETRY_COLUMN).to_pandas(maps_as_pydicts="strict"),
+            geometry=ga.to_geopandas(joined_parquet_table.column(GEOMETRY_COLUMN)),
+        ).set_index(FEATURES_INDEX)
 
         return gdf_parquet
 
-    def get_features_gdf_from_geometry(
+    def convert_geometry_to_geodataframe(
         self,
         keep_all_tags: bool = False,
         explode_tags: Optional[bool] = None,
         ignore_cache: bool = False,
         filter_osm_ids: Optional[list[str]] = None,
     ) -> gpd.GeoDataFrame:
         """
@@ -593,15 +620,15 @@
             filter_osm_ids: (list[str], optional): List of OSM features ids to read from the file.
                 Have to be in the form of 'node/<id>', 'way/<id>' or 'relation/<id>'.
                 Defaults to an empty list.
 
         Returns:
             gpd.GeoDataFrame: GeoDataFrame with OSM features.
         """
-        parsed_geoparquet_file = self.convert_geometry_filter_to_gpq(
+        parsed_geoparquet_file = self.convert_geometry_to_parquet(
             keep_all_tags=keep_all_tags,
             explode_tags=explode_tags,
             ignore_cache=ignore_cache,
             filter_osm_ids=filter_osm_ids,
         )
         joined_parquet_table = io.read_geoparquet_table(parsed_geoparquet_file)
         gdf_parquet = gpd.GeoDataFrame(
@@ -705,138 +732,142 @@
         result_file_path: Path,
         filter_osm_ids: list[str],
         keep_all_tags: bool = False,
         explode_tags: bool = True,
         ignore_cache: bool = False,
         save_as_wkt: bool = False,
     ) -> Path:
-        if result_file_path.with_suffix(".geoparquet").exists() and not ignore_cache:
+        if result_file_path.exists() and not ignore_cache:
+            return result_file_path
+        elif result_file_path.with_suffix(".geoparquet").exists() and not ignore_cache:
             warnings.warn(
                 (
                     "Found existing result file with `.geoparquet` extension."
                     " Users are enouraged to change the extension manually"
                     " to `.parquet` for old files. Files with `.geoparquet`"
                     " extension will be backwards supported, but reusing them"
                     " will result in this warning."
                 ),
                 DeprecationWarning,
                 stacklevel=0,
             )
             return result_file_path.with_suffix(".geoparquet")
 
-        if not result_file_path.exists() or ignore_cache:
-
-            elements = self.connection.sql(f"SELECT * FROM ST_READOSM('{Path(pbf_path)}');")
+        elements = self.connection.sql(f"SELECT * FROM ST_READOSM('{Path(pbf_path)}');")
 
-            if self.tags_filter is None:
-                self.expanded_tags_filter = None
-                self.merged_tags_filter = None
-            else:
-                self.expanded_tags_filter = self._expand_osm_tags_filter(elements)
-                self.merged_tags_filter = merge_osm_tags_filter(
-                    cast(Union[GroupedOsmTagsFilter, OsmTagsFilter], self.expanded_tags_filter)
-                )
+        if self.tags_filter is None:
+            self.expanded_tags_filter = None
+            self.merged_tags_filter = None
+        else:
+            self.expanded_tags_filter = self._expand_osm_tags_filter(elements)
+            self.merged_tags_filter = merge_osm_tags_filter(
+                cast(Union[GroupedOsmTagsFilter, OsmTagsFilter], self.expanded_tags_filter)
+            )
 
-            converted_osm_parquet_files = self._prefilter_elements_ids(elements, filter_osm_ids)
+        converted_osm_parquet_files = self._prefilter_elements_ids(elements, filter_osm_ids)
 
-            self._delete_directories(
-                [
-                    "nodes_filtered_non_distinct_ids",
-                    "nodes_prepared_ids",
-                    "ways_valid_ids",
-                    "ways_filtered_non_distinct_ids",
-                    "relations_valid_ids",
-                    "relations_ids",
-                ],
-            )
+        self._delete_directories(
+            [
+                "nodes_filtered_non_distinct_ids",
+                "nodes_prepared_ids",
+                "ways_valid_ids",
+                "ways_filtered_non_distinct_ids",
+                "relations_valid_ids",
+                "relations_ids",
+            ],
+        )
 
-            filtered_nodes_with_geometry_path = self._get_filtered_nodes_with_geometry(
-                converted_osm_parquet_files
-            )
-            self._delete_directories("nodes_filtered_ids")
+        filtered_nodes_with_geometry_path = self._get_filtered_nodes_with_geometry(
+            converted_osm_parquet_files
+        )
+        self._delete_directories("nodes_filtered_ids")
 
-            filtered_ways_with_linestrings = self._get_filtered_ways_with_linestrings(
-                osm_parquet_files=converted_osm_parquet_files
-            )
-            required_ways_with_linestrings = self._get_required_ways_with_linestrings(
-                osm_parquet_files=converted_osm_parquet_files
-            )
-            self._delete_directories(
-                [
-                    "nodes_valid_with_tags",
-                    "ways_required_grouped",
-                    "ways_required_ids",
-                    "ways_with_unnested_nodes_refs",
-                    "required_ways_ids_grouped",
-                    "required_ways_grouped",
-                    "required_ways_tmp",
-                    "filtered_ways_ids_grouped",
-                    "filtered_ways_grouped",
-                    "filtered_ways_tmp",
-                ],
-            )
+        filtered_ways_with_linestrings = self._get_filtered_ways_with_linestrings(
+            osm_parquet_files=converted_osm_parquet_files
+        )
+        required_ways_with_linestrings = self._get_required_ways_with_linestrings(
+            osm_parquet_files=converted_osm_parquet_files
+        )
+        self._delete_directories(
+            [
+                "nodes_valid_with_tags",
+                "ways_required_grouped",
+                "ways_required_ids",
+                "ways_with_unnested_nodes_refs",
+                "required_ways_ids_grouped",
+                "required_ways_grouped",
+                "required_ways_tmp",
+                "filtered_ways_ids_grouped",
+                "filtered_ways_grouped",
+                "filtered_ways_tmp",
+            ],
+        )
 
-            filtered_ways_with_proper_geometry_path = self._get_filtered_ways_with_proper_geometry(
-                converted_osm_parquet_files, filtered_ways_with_linestrings
-            )
-            self._delete_directories(
-                [
-                    "ways_prepared_ids",
-                    "ways_filtered_ids",
-                    "ways_all_with_tags",
-                    "filtered_ways_with_linestrings",
-                ],
-            )
+        filtered_ways_with_proper_geometry_path = self._get_filtered_ways_with_proper_geometry(
+            converted_osm_parquet_files, filtered_ways_with_linestrings
+        )
+        self._delete_directories(
+            [
+                "ways_prepared_ids",
+                "ways_filtered_ids",
+                "ways_all_with_tags",
+                "filtered_ways_with_linestrings",
+            ],
+        )
 
-            filtered_relations_with_geometry_path = self._get_filtered_relations_with_geometry(
-                converted_osm_parquet_files, required_ways_with_linestrings
-            )
-            self._delete_directories(
-                [
-                    "relations_all_with_tags",
-                    "relations_with_unnested_way_refs",
-                    "relations_filtered_ids",
-                    "required_ways_with_linestrings",
-                    "valid_relation_parts",
-                    "relation_inner_parts",
-                    "relation_outer_parts",
-                    "relation_outer_parts_with_holes",
-                    "relation_outer_parts_without_holes",
-                ],
-            )
+        filtered_relations_with_geometry_path = self._get_filtered_relations_with_geometry(
+            converted_osm_parquet_files, required_ways_with_linestrings
+        )
+        self._delete_directories(
+            [
+                "relations_all_with_tags",
+                "relations_with_unnested_way_refs",
+                "relations_filtered_ids",
+                "required_ways_with_linestrings",
+                "valid_relation_parts",
+                "relation_inner_parts",
+                "relation_outer_parts",
+                "relation_outer_parts_with_holes",
+                "relation_outer_parts_without_holes",
+            ],
+        )
 
-            parsed_geometries = self.connection.sql(
-                f"""
-                SELECT * FROM read_parquet([
-                    '{filtered_nodes_with_geometry_path}/**',
-                    '{filtered_ways_with_proper_geometry_path}/**',
-                    '{filtered_relations_with_geometry_path}/**'
-                ]);
-                """
-            )
+        parsed_geometries = self.connection.sql(
+            f"""
+            SELECT * FROM read_parquet([
+                '{filtered_nodes_with_geometry_path}/**',
+                '{filtered_ways_with_proper_geometry_path}/**',
+                '{filtered_relations_with_geometry_path}/**'
+            ]);
+            """
+        )
 
-            self._concatenate_results_to_geoparquet(
-                parsed_geometries=parsed_geometries,
-                save_file_path=result_file_path,
-                keep_all_tags=keep_all_tags,
-                explode_tags=explode_tags,
-                save_as_wkt=save_as_wkt,
-            )
+        self._concatenate_results_to_geoparquet(
+            parsed_geometries=parsed_geometries,
+            save_file_path=result_file_path,
+            keep_all_tags=keep_all_tags,
+            explode_tags=explode_tags,
+            save_as_wkt=save_as_wkt,
+        )
 
         return result_file_path
 
     def _generate_result_file_path(
         self,
-        pbf_file_path: Union[str, Path],
+        pbf_path: Union[str, Path, Iterable[Union[str, Path]]],
         keep_all_tags: bool,
         explode_tags: bool,
         filter_osm_ids: list[str],
         save_as_wkt: bool,
     ) -> Path:
-        pbf_file_name = Path(pbf_file_path).name.removesuffix(".osm.pbf")
+        if isinstance(pbf_path, (str, Path)):
+            pbf_path = [pbf_path]
+        pbf_file_name = "_".join(
+            [Path(pbf_file_path).name.removesuffix(".osm.pbf") for pbf_file_path in pbf_path]
+        )
 
         osm_filter_tags_hash_part = "nofilter"
         if self.tags_filter is not None:
             keep_all_tags_part = "" if not keep_all_tags else "_alltags"
             h = hashlib.new("sha256")
             h.update(json.dumps(self.tags_filter).encode())
             osm_filter_tags_hash_part = f"{h.hexdigest()}{keep_all_tags_part}"
@@ -2503,16 +2534,17 @@
     local_db_file = "db.duckdb" if is_main_connection else f"{secrets.token_hex(16)}.duckdb"
     connection = duckdb.connect(
         database=str(tmp_dir_path / local_db_file),
         config=dict(preserve_insertion_order=False),
     )
     connection.sql("SET enable_progress_bar = false;")
     connection.sql("SET enable_progress_bar_print = false;")
+
+    connection.install_extension("spatial")
     for extension_name in ("parquet", "spatial"):
-        connection.install_extension(extension_name)
         connection.load_extension(extension_name)
 
     connection.sql(
         """
         CREATE OR REPLACE MACRO linestring_to_linestring_geometry(ls) AS
         ls::struct(x DECIMAL(10, 7), y DECIMAL(10, 7))[]::LINESTRING_2D::GEOMETRY;
     """
```

### Comparing `quackosm-0.8.0/tests/base/conftest.py` & `quackosm-0.8.1/tests/base/conftest.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/tests/base/test_cli.py` & `quackosm-0.8.1/tests/base/test_cli.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/tests/base/test_osm_extracts.py` & `quackosm-0.8.1/tests/base/test_osm_extracts.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/tests/base/test_osm_tags_filtering.py` & `quackosm-0.8.1/tests/base/test_osm_tags_filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,16 +197,16 @@
 def test_pbf_reader(
     test_file_name: str,
     query: OsmTagsFilter,
     expected_result_length: int,
     expected_features_columns_length: int,
 ):
     """Test proper files loading in `PbfFileReader`."""
-    features_gdf = PbfFileReader(tags_filter=query).get_features_gdf(
-        file_paths=[Path(__file__).parent.parent / "test_files" / test_file_name],
+    features_gdf = PbfFileReader(tags_filter=query).convert_pbf_to_geodataframe(
+        pbf_path=[Path(__file__).parent.parent / "test_files" / test_file_name],
         explode_tags=True,
         ignore_cache=True,
     )
     assert (
         len(features_gdf) == expected_result_length
     ), f"Mismatched result length ({len(features_gdf)}, {expected_result_length})"
     assert len(features_gdf.columns) == expected_features_columns_length + 1, (
@@ -250,16 +250,16 @@
     filter_osm_id: str,
     osm_tags_filter: Union[OsmTagsFilter, GroupedOsmTagsFilter],
     keep_all_tags: bool,
     expected_tags_keys: list[str],
 ):
     """Test proper tags reading with filtering on osm_id in `PbfFileReader`."""
     file_name = "monaco.osm.pbf"
-    features_gdf = PbfFileReader(tags_filter=osm_tags_filter).get_features_gdf(
-        file_paths=[Path(__file__).parent.parent / "test_files" / file_name],
+    features_gdf = PbfFileReader(tags_filter=osm_tags_filter).convert_pbf_to_geodataframe(
+        pbf_path=[Path(__file__).parent.parent / "test_files" / file_name],
         ignore_cache=True,
         filter_osm_ids=[filter_osm_id],
         explode_tags=False,
         keep_all_tags=keep_all_tags,
     )
     assert len(features_gdf) == 1
     returned_tags_keys = list(features_gdf.iloc[0].tags.keys())
@@ -891,16 +891,16 @@
     expected_result_length: int,
     expected_top_10_ids: list[str],
     expected_no_columns: int,
     expected_top_10_columns: list[str],
 ):
     """Test proper tags reading with filtering in `PbfFileReader`."""
     file_name = "monaco.osm.pbf"
-    features_gdf = PbfFileReader(tags_filter=osm_tags_filter).get_features_gdf(
-        file_paths=[Path(__file__).parent.parent / "test_files" / file_name],
+    features_gdf = PbfFileReader(tags_filter=osm_tags_filter).convert_pbf_to_geodataframe(
+        pbf_path=[Path(__file__).parent.parent / "test_files" / file_name],
         ignore_cache=True,
         explode_tags=True,
     )
     assert (
         len(features_gdf) == expected_result_length
     ), f"Mismatched result length ({len(features_gdf)}, {expected_result_length})"
     ut.assertListEqual(list(features_gdf.sort_index().head(10).index), expected_top_10_ids)
@@ -925,12 +925,12 @@
 )
 def test_incorrect_osm_tags_filters(
     osm_tags_filter: Union[OsmTagsFilter, GroupedOsmTagsFilter],
 ) -> None:
     """Test wrong tags reading with filtering in `PbfFileReader`."""
     with pytest.raises(ValueError):
         file_name = "monaco.osm.pbf"
-        PbfFileReader(tags_filter=osm_tags_filter).get_features_gdf(
-            file_paths=[Path(__file__).parent.parent / "test_files" / file_name],
+        PbfFileReader(tags_filter=osm_tags_filter).convert_pbf_to_geodataframe(
+            pbf_path=[Path(__file__).parent.parent / "test_files" / file_name],
             ignore_cache=True,
             explode_tags=False,
         )
```

### Comparing `quackosm-0.8.0/tests/base/test_pbf_file_reader.py` & `quackosm-0.8.1/tests/base/test_pbf_file_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Tests for PbfFileReader."""
 
 import json
 import warnings
+from functools import partial
 from pathlib import Path
-from typing import Optional, Union, cast
+from typing import Any, Callable, Optional, Union, cast
 from unittest import TestCase
 
 import duckdb
 import geopandas as gpd
 import pandas as pd
 import pyarrow as pa
 import pytest
@@ -27,15 +28,20 @@
 )
 from shapely.geometry.base import BaseGeometry
 from shapely.ops import unary_union
 from srai.geometry import remove_interiors
 from srai.loaders.download import download_file
 from srai.loaders.osm_loaders.filters import GEOFABRIK_LAYERS, HEX2VEC_FILTER
 
-from quackosm import convert_geometry_to_gpq, convert_pbf_to_gpq, get_features_gdf
+from quackosm import (
+    convert_geometry_to_parquet,
+    convert_pbf_to_geodataframe,
+    convert_pbf_to_parquet,
+    functions,
+)
 from quackosm._constants import FEATURES_INDEX, WGS84_CRS
 from quackosm._exceptions import (
     GeometryNotCoveredError,
     GeometryNotCoveredWarning,
     InvalidGeometryFilter,
 )
 from quackosm._osm_tags_filters import GroupedOsmTagsFilter, OsmTagsFilter
@@ -61,30 +67,30 @@
     tags_filter: Optional[Union[OsmTagsFilter, GroupedOsmTagsFilter]],
     explode_tags: Optional[bool],
     keep_all_tags: bool,
     save_as_wkt: bool,
 ):
     """Test if pbf to geoparquet conversion works."""
     pbf_file = Path(__file__).parent.parent / "test_files" / "monaco.osm.pbf"
-    PbfFileReader(tags_filter=tags_filter).convert_pbf_to_gpq(
+    PbfFileReader(tags_filter=tags_filter).convert_pbf_to_parquet(
         pbf_path=pbf_file,
         ignore_cache=True,
         explode_tags=explode_tags,
         keep_all_tags=keep_all_tags,
         save_as_wkt=save_as_wkt,
     )
 
 
 def test_pbf_reader_geometry_filtering():  # type: ignore
     """Test proper spatial data filtering in `PbfFileReader`."""
     file_name = "d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf"
     features_gdf = PbfFileReader(
         tags_filter=HEX2VEC_FILTER, geometry_filter=Polygon([(0, 0), (0, 1), (1, 1), (1, 0)])
-    ).get_features_gdf(
-        file_paths=[Path(__file__).parent.parent / "test_files" / file_name],
+    ).convert_pbf_to_geodataframe(
+        pbf_path=[Path(__file__).parent.parent / "test_files" / file_name],
         explode_tags=True,
         ignore_cache=True,
     )
     assert len(features_gdf) == 0
 
 
 @pytest.mark.parametrize(
@@ -111,20 +117,20 @@
         == PbfFileReader(geometry_filter=oriented_b)._get_oriented_geometry_filter()
     )
 
 
 def test_unique_osm_ids_duplicated_file():  # type: ignore
     """Test if function returns results without duplicated features."""
     monaco_file_path = Path(__file__).parent.parent / "test_files" / "monaco.osm.pbf"
-    result_gdf = PbfFileReader().get_features_gdf(
-        file_paths=[monaco_file_path, monaco_file_path], ignore_cache=True
+    result_gdf = PbfFileReader().convert_pbf_to_geodataframe(
+        pbf_path=[monaco_file_path, monaco_file_path], ignore_cache=True
     )
 
-    single_result_gdf = PbfFileReader().get_features_gdf(
-        file_paths=[monaco_file_path], ignore_cache=True
+    single_result_gdf = PbfFileReader().convert_pbf_to_geodataframe(
+        pbf_path=[monaco_file_path], ignore_cache=True
     )
 
     assert result_gdf.index.is_unique
     assert len(result_gdf.index) == len(single_result_gdf.index)
 
 
 def test_unique_osm_ids_real_example():  # type: ignore
@@ -132,30 +138,30 @@
     andorra_geometry = from_wkt(
         "POLYGON ((1.382599544073372 42.67676873293743, 1.382599544073372 42.40065303248514,"
         " 1.8092269635579328 42.40065303248514, 1.8092269635579328 42.67676873293743,"
         " 1.382599544073372 42.67676873293743))"
     )
     result_gdf = PbfFileReader(
         geometry_filter=andorra_geometry, osm_extract_source=OsmExtractSource.any
-    ).get_features_gdf_from_geometry(ignore_cache=True)
+    ).convert_geometry_to_geodataframe(ignore_cache=True)
 
     assert result_gdf.index.is_unique
 
 
 def test_antwerpen_and_brussels_invalid_linear_ring() -> None:
     """Test if properly filters out invalid linear rings."""
     antwerpen_and_brussels_geometry = from_wkt(
         "POLYGON ((4.331278527313799 51.173447782908625,"
         " 4.331278527313799 50.89211829585622, 4.413826045759777 50.89211829585622,"
         " 4.413826045759777 51.173447782908625, 4.331278527313799 51.173447782908625))"
     )
 
     result_gdf = PbfFileReader(
         geometry_filter=antwerpen_and_brussels_geometry, osm_extract_source=OsmExtractSource.bbbike
-    ).get_features_gdf_from_geometry(ignore_cache=True)
+    ).convert_geometry_to_geodataframe(ignore_cache=True)
 
     assert result_gdf.index.is_unique
 
 
 @pytest.mark.parametrize("operation_mode", ["gdf", "gpq"])  # type: ignore
 @pytest.mark.parametrize("patch_methods", [0, 1, 2])  # type: ignore
 def test_combining_files_different_techniques(
@@ -174,29 +180,29 @@
         mocker.patch(
             "quackosm.pbf_file_reader.PbfFileReader._drop_duplicated_features_in_joined_table",
             side_effect=MemoryError(),
         )
 
     if operation_mode == "gdf":
         monaco_file_path = Path(__file__).parent.parent / "test_files" / "monaco.osm.pbf"
-        result_gdf = get_features_gdf(
-            file_paths=[
+        result_gdf = convert_pbf_to_geodataframe(
+            pbf_path=[
                 monaco_file_path,
                 monaco_file_path,
             ],
             ignore_cache=True,
         )
-        single_result_gdf = PbfFileReader(debug_memory=True, debug_times=True).get_features_gdf(
-            file_paths=[monaco_file_path], ignore_cache=True
-        )
+        single_result_gdf = PbfFileReader(
+            debug_memory=True, debug_times=True
+        ).convert_pbf_to_geodataframe(pbf_path=[monaco_file_path], ignore_cache=True)
 
         assert result_gdf.index.is_unique
         assert len(result_gdf.index) == len(single_result_gdf.index)
     elif operation_mode == "gpq":
-        result = convert_geometry_to_gpq(
+        result = convert_geometry_to_parquet(
             geometry_filter=from_wkt(
                 "POLYGON ((4.331278527313799 51.173447782908625,"
                 " 4.331278527313799 50.89211829585622, 4.413826045759777 50.89211829585622,"
                 " 4.413826045759777 51.173447782908625, 4.331278527313799 51.173447782908625))"
             ),
             osm_extract_source="BBBike",
             ignore_cache=True,
@@ -212,15 +218,15 @@
 
     Extracted from issue https://github.com/kraina-ai/quackosm/issues/42
     """
     geo = box(minx=-85.904275, miny=38.056361, maxx=-85.502994, maxy=38.383253)
     tags: OsmTagsFilter = {"military": ["airfield"], "leisure": ["park"]}
     result_gdf = PbfFileReader(
         tags_filter=tags, geometry_filter=geo, osm_extract_source=OsmExtractSource.geofabrik
-    ).get_features_gdf_from_geometry(explode_tags=True)
+    ).convert_geometry_to_geodataframe(explode_tags=True)
     assert result_gdf.index.is_unique
 
 
 @pytest.mark.parametrize(  # type: ignore
     "filter_osm_ids,expected_result_length",
     [
         (
@@ -240,16 +246,16 @@
         ),
         (["way/0", "node/0", "relation/0"], 0),
     ],
 )
 def test_pbf_reader_features_ids_filtering(filter_osm_ids: list[str], expected_result_length: int):
     """Test proper features ids filtering in `PbfFileReader`."""
     file_name = "d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf"
-    features_gdf = PbfFileReader().get_features_gdf(
-        file_paths=[Path(__file__).parent.parent / "test_files" / file_name],
+    features_gdf = PbfFileReader().convert_pbf_to_geodataframe(
+        pbf_path=[Path(__file__).parent.parent / "test_files" / file_name],
         ignore_cache=True,
         filter_osm_ids=filter_osm_ids,
     )
     assert len(features_gdf) == expected_result_length
 
 
 @pytest.mark.parametrize(
@@ -264,15 +270,15 @@
     with expectation:
         geometry = from_wkt(
             "POLYGON ((-43.064 29.673, -43.064 29.644, -43.017 29.644,"
             " -43.017 29.673, -43.064 29.673))"
         )
         features_gdf = PbfFileReader(
             geometry_filter=geometry, allow_uncovered_geometry=allow_uncovered_geometry
-        ).get_features_gdf_from_geometry(ignore_cache=True)
+        ).convert_geometry_to_geodataframe(ignore_cache=True)
         assert len(features_gdf) == 0
 
 
 @pytest.mark.parametrize(  # type: ignore
     "geometry",
     [
         box(
@@ -326,24 +332,24 @@
     with pytest.raises(InvalidGeometryFilter):
         PbfFileReader(geometry_filter=geometry)
 
 
 def test_geoparquet_deprecation_warning() -> None:
     """Test if warning is properly displayed."""
     monaco_file_path = Path(__file__).parent.parent / "test_files" / "monaco.osm.pbf"
-    convert_pbf_to_gpq(
+    result_path = convert_pbf_to_parquet(
         monaco_file_path,
         ignore_cache=True,
-        result_file_path="files/monaco_nofilter_noclip_compact.geoparquet",
     )
+    result_path.rename(result_path.with_suffix(".geoparquet"))
     with pytest.warns(DeprecationWarning):
-        convert_pbf_to_gpq(monaco_file_path, ignore_cache=False)
+        convert_pbf_to_parquet(monaco_file_path, ignore_cache=False)
 
     with pytest.warns(DeprecationWarning):
-        get_features_gdf(monaco_file_path, ignore_cache=False)
+        convert_pbf_to_geodataframe(monaco_file_path, ignore_cache=False)
 
 
 @pytest.mark.parametrize(  # type: ignore
     "geometry",
     [
         box(
             minx=7.416486207767861,
@@ -366,14 +372,88 @@
         BaseGeometry, PbfFileReader(geometry_filter=geometry)._get_oriented_geometry_filter()
     )
     intersection_area = geometry.intersection(oriented_geometry).area
     iou = intersection_area / (geometry.area + oriented_geometry.area - intersection_area)
     ut.assertAlmostEqual(iou, 1, delta=1e-4)
 
 
+@pytest.mark.parametrize(  # type: ignore
+    "func,new_function_name",
+    [
+        (
+            partial(
+                functions.get_features_gdf,
+                file_paths=Path(__file__).parent.parent / "test_files" / "monaco.osm.pbf",
+            ),
+            "convert_pbf_to_geodataframe",
+        ),
+        (
+            partial(
+                functions.get_features_gdf,
+                pbf_path=Path(__file__).parent.parent / "test_files" / "monaco.osm.pbf",
+            ),
+            "convert_pbf_to_geodataframe",
+        ),
+        (
+            partial(functions.get_features_gdf_from_geometry, geometry_filter=geometry_box()),
+            "convert_geometry_to_geodataframe",
+        ),
+        (
+            partial(
+                functions.convert_pbf_to_gpq,
+                pbf_path=Path(__file__).parent.parent / "test_files" / "monaco.osm.pbf",
+            ),
+            "convert_pbf_to_parquet",
+        ),
+        (
+            partial(
+                functions.convert_geometry_to_gpq,
+                geometry_filter=geometry_box(),
+            ),
+            "convert_geometry_to_parquet",
+        ),
+        (
+            partial(
+                PbfFileReader().get_features_gdf,
+                file_paths=Path(__file__).parent.parent / "test_files" / "monaco.osm.pbf",
+            ),
+            "convert_pbf_to_geodataframe",
+        ),
+        (
+            partial(
+                PbfFileReader().get_features_gdf,
+                pbf_path=Path(__file__).parent.parent / "test_files" / "monaco.osm.pbf",
+            ),
+            "convert_pbf_to_geodataframe",
+        ),
+        (
+            PbfFileReader(geometry_filter=geometry_box()).get_features_gdf_from_geometry,
+            "convert_geometry_to_geodataframe",
+        ),
+        (
+            partial(
+                PbfFileReader().convert_pbf_to_gpq,
+                pbf_path=Path(__file__).parent.parent / "test_files" / "monaco.osm.pbf",
+            ),
+            "convert_pbf_to_parquet",
+        ),
+        (
+            PbfFileReader(geometry_filter=geometry_box()).convert_geometry_filter_to_gpq,
+            "convert_geometry_to_parquet",
+        ),
+    ],
+)
+def test_deprecation(func: Callable[[], Any], new_function_name: str):
+    """Test if deprecation works."""
+    with pytest.warns(FutureWarning) as record:
+        func()
+
+    assert new_function_name in str(record[0].message)
+
+
 def check_if_relation_in_osm_is_valid_based_on_tags(pbf_file: str, relation_id: str) -> bool:
     """Check if given relation in OSM is valid."""
     duckdb.load_extension("spatial")
     return cast(
         bool,
         duckdb.sql(
             f"SELECT list_contains(ref_roles, 'outer') FROM ST_READOSM('{pbf_file}') "
@@ -556,15 +636,17 @@
     pbf_file_path = Path(__file__).parent.parent / "files" / f"{extract_name}.osm.pbf"
     download_file(pbf_file_download_url, str(pbf_file_path), force_download=True)
     gpq_file_download_url = LFS_DIRECTORY_URL + f"{extract_name}-latest.geoparquet"
     gpq_file_path = Path(__file__).parent.parent / "files" / f"{extract_name}.parquet"
     download_file(gpq_file_download_url, str(gpq_file_path), force_download=True)
 
     reader = PbfFileReader()
-    duckdb_gdf = reader.get_features_gdf([pbf_file_path], explode_tags=False, ignore_cache=True)
+    duckdb_gdf = reader.convert_pbf_to_geodataframe(
+        [pbf_file_path], explode_tags=False, ignore_cache=True
+    )
     gdal_gdf = gpd.read_parquet(gpq_file_path)
     gdal_gdf["tags"] = gdal_gdf["tags"].apply(json.loads)
 
     gdal_index = gdal_gdf.index
     duckdb_index = duckdb_gdf.index
 
     missing_in_duckdb = gdal_index.difference(duckdb_index)
```

### Comparing `quackosm-0.8.0/tests/benchmark/test_big_file.py` & `quackosm-0.8.1/tests/benchmark/test_big_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     download_file(
         f"https://download.geofabrik.de/europe/{extract_name}-latest.osm.pbf", str(file_name)
     )
 
     reader = PbfFileReader(working_directory=files_dir, verbosity_mode="verbose")
     # Reset rows_per_group value to test automatic downscaling
     reader.rows_per_group = PbfFileReader.ROWS_PER_GROUP_MEMORY_CONFIG[24]
-    reader.convert_pbf_to_gpq(pbf_path=file_name, ignore_cache=True)
+    reader.convert_pbf_to_parquet(pbf_path=file_name, ignore_cache=True)
```

### Comparing `quackosm-0.8.0/tests/optional_imports/test_optional_cli_dependency.py` & `quackosm-0.8.1/tests/optional_imports/test_optional_cli_dependency.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 def optional_packages() -> list[str]:
     """Get a list with optional packages."""
     return [
         "typer",
         "click",
         "osmnx",
         "h3",
-        "h3ronpy",
         "s2",
         "geohash",
     ]
 
 
 @pytest.fixture(autouse=True)  # type: ignore
 def cleanup_imports():
```

### Comparing `quackosm-0.8.0/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `quackosm-0.8.1/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `quackosm-0.8.1/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `quackosm-0.8.1/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/tests/test_files/monaco.osm.pbf` & `quackosm-0.8.1/tests/test_files/monaco.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/tests/test_files/monaco_boundary.geojson` & `quackosm-0.8.1/tests/test_files/monaco_boundary.geojson`

 * *Files identical despite different names*

### Comparing `quackosm-0.8.0/PKG-INFO` & `quackosm-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuackOSM
-Version: 0.8.0
+Version: 0.8.1
 Summary: An open-source tool for reading OpenStreetMap PBF files using DuckDB
 Author-Email: Kamil Raczycki <kraczycki@kraina.ai>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: GIS
@@ -160,15 +160,15 @@
 
 ### If you already have downloaded the PBF file 📁🗺️
 
 #### Load data as a GeoDataFrame
 
 ```python
 >>> import quackosm as qosm
->>> qosm.get_features_gdf(monaco_pbf_path)
+>>> qosm.convert_pbf_to_geodataframe(monaco_pbf_path)
                                               tags                      geometry
 feature_id
 node/10005045289                {'shop': 'bakery'}      POINT (7.42245 43.73105)
 node/10020887517  {'leisure': 'swimming_pool', ...      POINT (7.41316 43.73384)
 node/10021298117  {'leisure': 'swimming_pool', ...      POINT (7.42777 43.74277)
 node/10021298717  {'leisure': 'swimming_pool', ...      POINT (7.42630 43.74097)
 node/10025656383  {'ferry': 'yes', 'name': 'Qua...      POINT (7.42550 43.73690)
@@ -182,15 +182,15 @@
 [7906 rows x 2 columns]
 ```
 
 #### Just convert PBF to GeoParquet
 
 ```python
 >>> import quackosm as qosm
->>> gpq_path = qosm.convert_pbf_to_gpq(monaco_pbf_path)
+>>> gpq_path = qosm.convert_pbf_to_parquet(monaco_pbf_path)
 >>> gpq_path.as_posix()
 'files/monaco_nofilter_noclip_compact.parquet'
 ```
 
 #### Inspect the file with duckdb
 
 ```python
@@ -231,65 +231,63 @@
 └────────────────────────────────────────────────────────────────────────────────────────┘
 ```
 
 #### Use as CLI
 
 ```console
 $ quackosm monaco.osm.pbf
-⠙ [   1/32] Reading nodes • 0:00:00
+⠋ [   1/32] Reading nodes • 0:00:00
 ⠋ [   2/32] Filtering nodes - intersection • 0:00:00
-⠙ [   3/32] Filtering nodes - tags • 0:00:00
+⠋ [   3/32] Filtering nodes - tags • 0:00:00
 ⠋ [   4/32] Calculating distinct filtered nodes ids • 0:00:00
-⠙ [   5/32] Reading ways • 0:00:00
+⠋ [   5/32] Reading ways • 0:00:00
 ⠋ [   6/32] Unnesting ways • 0:00:00
-⠹ [   7/32] Filtering ways - valid refs • 0:00:00
+⠋ [   7/32] Filtering ways - valid refs • 0:00:00
 ⠋ [   8/32] Filtering ways - intersection • 0:00:00
-⠙ [   9/32] Filtering ways - tags • 0:00:00
+⠋ [   9/32] Filtering ways - tags • 0:00:00
 ⠋ [  10/32] Calculating distinct filtered ways ids • 0:00:00
 ⠋ [  11/32] Reading relations • 0:00:00
 ⠋ [  12/32] Unnesting relations • 0:00:00
-⠹ [  13/32] Filtering relations - valid refs • 0:00:00
+⠸ [  13/32] Filtering relations - valid refs • 0:00:00
 ⠋ [  14/32] Filtering relations - intersection • 0:00:00
-⠙ [  15/32] Filtering relations - tags • 0:00:00
+⠋ [  15/32] Filtering relations - tags • 0:00:00
 ⠋ [  16/32] Calculating distinct filtered relations ids • 0:00:00
-⠙ [  17/32] Loading required ways - by relations • 0:00:00
+⠋ [  17/32] Loading required ways - by relations • 0:00:00
 ⠋ [  18/32] Calculating distinct required ways ids • 0:00:00
-⠙ [  19/32] Saving filtered nodes with geometries • 0:00:00
+⠋ [  19/32] Saving filtered nodes with geometries • 0:00:00
 ⠋ [20.1/32] Grouping filtered ways - assigning groups • 0:00:00
 ⠧ [20.2/32] Grouping filtered ways - joining with nodes • 0:00:00
 ⠋ [20.3/32] Grouping filtered ways - partitioning by group • 0:00:00
   [  21/32] Saving filtered ways with linestrings 100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1/1 • 0:00:00 < 0:00:00 •
 ⠋ [22.1/32] Grouping required ways - assigning groups • 0:00:00
 ⠧ [22.2/32] Grouping required ways - joining with nodes • 0:00:00
 ⠋ [22.3/32] Grouping required ways - partitioning by group • 0:00:00
   [  23/32] Saving required ways with linestrings 100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1/1 • 0:00:00 < 0:00:00 •
-⠹ [  24/32] Saving filtered ways with geometries • 0:00:00
-⠸ [  25/32] Saving valid relations parts • 0:00:00
-⠋ [26.1/32] Saving relations inner parts - valid geometries • 0:00:00
-⠋ [26.2/32] Saving relations inner parts - invalid geometries • 0:00:00
-⠋ [27.1/32] Saving relations outer parts - valid geometries • 0:00:00
-⠋ [27.2/32] Saving relations outer parts - invalid geometries • 0:00:00
+⠙ [  24/32] Saving filtered ways with geometries • 0:00:00
+⠋ [  25/32] Saving valid relations parts • 0:00:00
+⠋ [  26/32] Saving relations inner parts • 0:00:00
+⠋ [  27/32] Saving relations outer parts • 0:00:00
 ⠋ [  28/32] Saving relations outer parts with holes • 0:00:00
 ⠋ [  29/32] Saving relations outer parts without holes • 0:00:00
-⠙ [  30/32] Saving filtered relations with geometries • 0:00:00
-⠹ [31.1/32] Saving valid features • 0:00:00
+⠋ [  30/32] Saving filtered relations with geometries • 0:00:00
+⠋ [  31/32] Saving all features • 0:00:00
 ⠋ [  32/32] Saving final geoparquet file • 0:00:00
-Finished operation in 0:00:06
+Finished operation in 0:00:03
 files/monaco_nofilter_noclip_compact.parquet
 ```
 
 ### Let the QuackOSM automatically download the required OSM PBF files for you 🔎🌍
 
 #### Load data as a GeoDataFrame
 
 ```python
 >>> import quackosm as qosm
 >>> import osmnx as ox
 >>> geometry = ox.geocode_to_gdf("Vatican City").unary_union
->>> qosm.get_features_gdf_from_geometry(geometry)
+>>> qosm.convert_geometry_to_geodataframe(geometry)
                                               tags                      geometry
 feature_id
 node/10253371713   {'crossing': 'uncontrolled',...     POINT (12.45603 41.90454)
 node/10253371714               {'highway': 'stop'}     POINT (12.45705 41.90400)
 node/10253371715               {'highway': 'stop'}     POINT (12.45242 41.90164)
 node/10253371720     {'artwork_type': 'statue',...     POINT (12.45147 41.90484)
 node/10253371738               {'natural': 'tree'}     POINT (12.45595 41.90609)
@@ -307,15 +305,15 @@
 
 ```python
 >>> import quackosm as qosm
 >>> from shapely import from_wkt
 >>> geometry = from_wkt(
 ...     "POLYGON ((14.4861 35.9107, 14.4861 35.8811, 14.5331 35.8811, 14.5331 35.9107, 14.4861 35.9107))"
 ... )
->>> gpq_path = qosm.convert_geometry_to_gpq(geometry)
+>>> gpq_path = qosm.convert_geometry_to_parquet(geometry)
 >>> gpq_path.as_posix()
 'files/4b2967088a8fe31cdc15401e29bff9b7b882565cd8143e90443f39f2dc5fe6de_nofilter_compact.parquet'
 ```
 
 #### Inspect the file with duckdb
 
 ```python
@@ -356,55 +354,53 @@
 └────────────────────────────────────────────────────────────────────────────────────────┘
 ```
 
 #### Use as CLI
 
 ```console
 $ quackosm --geom-filter-geocode "Shibuya, Tokyo"
-100%|██████████████████████████████████████| 45.7M/45.7M [00:00<00:00, 259GB/s]
-⠦ [   1/32] Reading nodes • 0:00:05
-⠋ [   2/32] Filtering nodes - intersection • 0:00:00
-⠦ [   3/32] Filtering nodes - tags • 0:00:00
+100%|██████████████████████████████████████| 46.3M/46.3M [00:00<00:00, 327GB/s]
+⠋ [   1/32] Reading nodes • 0:00:01
+⠹ [   2/32] Filtering nodes - intersection • 0:00:00
+⠋ [   3/32] Filtering nodes - tags • 0:00:00
 ⠋ [   4/32] Calculating distinct filtered nodes ids • 0:00:00
-⠏ [   5/32] Reading ways • 0:00:04
-⠦ [   6/32] Unnesting ways • 0:00:02
-⠴ [   7/32] Filtering ways - valid refs • 0:00:02
-⠙ [   8/32] Filtering ways - intersection • 0:00:01
-⠹ [   9/32] Filtering ways - tags • 0:00:00
+⠸ [   5/32] Reading ways • 0:00:03
+⠴ [   6/32] Unnesting ways • 0:00:01
+⠼ [   7/32] Filtering ways - valid refs • 0:00:00
+⠹ [   8/32] Filtering ways - intersection • 0:00:00
+⠋ [   9/32] Filtering ways - tags • 0:00:00
 ⠋ [  10/32] Calculating distinct filtered ways ids • 0:00:00
-⠴ [  11/32] Reading relations • 0:00:00
-⠴ [  12/32] Unnesting relations • 0:00:00
-⠹ [  13/32] Filtering relations - valid refs • 0:00:00
-⠙ [  14/32] Filtering relations - intersection • 0:00:00
-⠙ [  15/32] Filtering relations - tags • 0:00:00
+⠼ [  11/32] Reading relations • 0:00:00
+⠸ [  12/32] Unnesting relations • 0:00:00
+⠋ [  13/32] Filtering relations - valid refs • 0:00:00
+⠋ [  14/32] Filtering relations - intersection • 0:00:00
+⠋ [  15/32] Filtering relations - tags • 0:00:00
 ⠋ [  16/32] Calculating distinct filtered relations ids • 0:00:00
-⠙ [  17/32] Loading required ways - by relations • 0:00:00
+⠋ [  17/32] Loading required ways - by relations • 0:00:00
 ⠋ [  18/32] Calculating distinct required ways ids • 0:00:00
-⠋ [  19/32] Saving filtered nodes with geometries • 0:00:00
+⠹ [  19/32] Saving filtered nodes with geometries • 0:00:00
 ⠋ [20.1/32] Grouping filtered ways - assigning groups • 0:00:00
-⠴ [20.2/32] Grouping filtered ways - joining with nodes • 0:00:03
-⠹ [20.3/32] Grouping filtered ways - partitioning by group • 0:00:00
-  [  21/32] Saving filtered ways with linestrings 100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1/1 • 0:00:01 < 0:00:00 •
+⠼ [20.2/32] Grouping filtered ways - joining with nodes • 0:00:01
+⠋ [20.3/32] Grouping filtered ways - partitioning by group • 0:00:00
+  [  21/32] Saving filtered ways with linestrings 100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1/1 • 0:00:00 < 0:00:00 •
 ⠋ [22.1/32] Grouping required ways - assigning groups • 0:00:00
-⠴ [22.2/32] Grouping required ways - joining with nodes • 0:00:03
+⠼ [22.2/32] Grouping required ways - joining with nodes • 0:00:01
 ⠋ [22.3/32] Grouping required ways - partitioning by group • 0:00:00
   [  23/32] Saving required ways with linestrings 100% ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1/1 • 0:00:00 < 0:00:00 •
-⠋ [  24/32] Saving filtered ways with geometries • 0:00:01
-⠸ [  25/32] Saving valid relations parts • 0:00:00
-⠋ [26.1/32] Saving relations inner parts - valid geometries • 0:00:00
-⠋ [26.2/32] Saving relations inner parts - invalid geometries • 0:00:00
-⠙ [27.1/32] Saving relations outer parts - valid geometries • 0:00:00
-⠋ [27.2/32] Saving relations outer parts - invalid geometries • 0:00:00
+⠴ [  24/32] Saving filtered ways with geometries • 0:00:00
+⠋ [  25/32] Saving valid relations parts • 0:00:00
+⠋ [  26/32] Saving relations inner parts • 0:00:00
+⠋ [  27/32] Saving relations outer parts • 0:00:00
 ⠋ [  28/32] Saving relations outer parts with holes • 0:00:00
 ⠋ [  29/32] Saving relations outer parts without holes • 0:00:00
-⠙ [  30/32] Saving filtered relations with geometries • 0:00:00
-⠸ [31.1/32] Saving valid features • 0:00:00
+⠋ [  30/32] Saving filtered relations with geometries • 0:00:00
+⠙ [  31/32] Saving all features • 0:00:00
 ⠋ [  32/32] Saving final geoparquet file • 0:00:00
-Finished operation in 0:00:39
-files/9ae2b160eb7556991148f5a2693aaf4b38bbb225c3700a6bfe9e5e54f48b987e_nofilter_compact.parquet
+Finished operation in 0:00:13
+files/78580cf29b5ba1073366a257e1909bfeee43c9f5859e48fb3b2d592028bb58aa_nofilter_compact.parquet
 ```
 
 CLI Help output (`QuackOSM -h`):
 ![CLI Help output](https://raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/cli_help.png)
 
 You can find full API + more examples in the [docs](https://kraina-ai.github.io/quackosm/).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: QuackOSM Version: 0.8.0 Summary: An open-source
+Metadata-Version: 2.1 Name: QuackOSM Version: 0.8.1 Summary: An open-source
 tool for reading OpenStreetMap PBF files using DuckDB Author-Email: Kamil
 Raczycki
 kraina.ai> License: Apache-2.0 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: GIS Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
@@ -60,28 +60,28 @@
 files services - `beautifulsoup4`: For parsing HTML files and scraping required
 information Optional: - `typer[all] (>=0.9.0)` (click, colorama, rich,
 shellingham): For CLI - `osmnx (>=1.3.0)`: For geocoding of strings in CLI -
 `h3 (>=4.0.0b1)`: For reading H3 strings in CLI - `s2 (>=0.1.9)`: For
 transforming S2 indexes into geometries - `python-geohash (>=0.8)`: For
 transforming GeoHash indexes into geometries ## Usage ### If you already have
 downloaded the PBF file ððºï¸ #### Load data as a GeoDataFrame ```python
->>> import quackosm as qosm >>> qosm.get_features_gdf(monaco_pbf_path) tags
-geometry feature_id node/10005045289 {'shop': 'bakery'} POINT (7.42245
-43.73105) node/10020887517 {'leisure': 'swimming_pool', ... POINT (7.41316
-43.73384) node/10021298117 {'leisure': 'swimming_pool', ... POINT (7.42777
-43.74277) node/10021298717 {'leisure': 'swimming_pool', ... POINT (7.42630
-43.74097) node/10025656383 {'ferry': 'yes', 'name': 'Qua... POINT (7.42550
-43.73690) ... ... ... way/990669427 {'amenity': 'shelter', 'shelt... POLYGON (
-(7.41461 43.7338... way/990669428 {'highway': 'secondary', 'jun... LINESTRING
-(7.41366 43.73... way/990669429 {'highway': 'secondary', 'jun... LINESTRING
-(7.41376 43.73... way/990848785 {'addr:city': 'Monaco', 'addr... POLYGON (
-(7.41426 43.7339... way/993121275 {'building': 'yes', 'name': ... POLYGON (
-(7.43214 43.7481... [7906 rows x 2 columns] ``` #### Just convert PBF to
-GeoParquet ```python >>> import quackosm as qosm >>> gpq_path =
-qosm.convert_pbf_to_gpq(monaco_pbf_path) >>> gpq_path.as_posix() 'files/
+>>> import quackosm as qosm >>> qosm.convert_pbf_to_geodataframe
+(monaco_pbf_path) tags geometry feature_id node/10005045289 {'shop': 'bakery'}
+POINT (7.42245 43.73105) node/10020887517 {'leisure': 'swimming_pool', ...
+POINT (7.41316 43.73384) node/10021298117 {'leisure': 'swimming_pool', ...
+POINT (7.42777 43.74277) node/10021298717 {'leisure': 'swimming_pool', ...
+POINT (7.42630 43.74097) node/10025656383 {'ferry': 'yes', 'name': 'Qua...
+POINT (7.42550 43.73690) ... ... ... way/990669427 {'amenity': 'shelter',
+'shelt... POLYGON ((7.41461 43.7338... way/990669428 {'highway': 'secondary',
+'jun... LINESTRING (7.41366 43.73... way/990669429 {'highway': 'secondary',
+'jun... LINESTRING (7.41376 43.73... way/990848785 {'addr:city': 'Monaco',
+'addr... POLYGON ((7.41426 43.7339... way/993121275 {'building': 'yes', 'name':
+... POLYGON ((7.43214 43.7481... [7906 rows x 2 columns] ``` #### Just convert
+PBF to GeoParquet ```python >>> import quackosm as qosm >>> gpq_path =
+qosm.convert_pbf_to_parquet(monaco_pbf_path) >>> gpq_path.as_posix() 'files/
 monaco_nofilter_noclip_compact.parquet' ``` #### Inspect the file with duckdb
 ```python >>> import duckdb >>> duckdb.load_extension('spatial') >>>
 duckdb.read_parquet(str(gpq_path)).project( ... "* REPLACE (ST_GeomFromWKB
 (geometry) AS geometry)" ... ).order("feature_id")
 ââââââââââââââââââââ¬âââââââââââââââââââââââ¬âââââââââââââââââââââââââââââââââââââââââââââââ
 â feature_id â tags â geometry â â varchar â map(varchar, varchâ¦
 â geometry â
@@ -110,67 +110,65 @@
 {highway=secondaryâ¦ â LINESTRING (7.4137621 43.7334251, 7.413746â¦ â â
 way/990848785 â {addr:city=Monaco,â¦ â POLYGON ((7.4142551 43.7339622,
 7.4143113 â¦ â â way/993121275 â {building=yes, namâ¦ â POLYGON (
 (7.4321416 43.7481309, 7.4321638 â¦ â
 ââââââââââââââââââââ´âââââââââââââââââââââââ´âââââââââââââââââââââââââââââââââââââââââââââââ¤
 â 7906 rows (20 shown) 3 columns â
 ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
-``` #### Use as CLI ```console $ quackosm monaco.osm.pbf â  [ 1/32] Reading
-nodes â¢ 0:00:00 â  [ 2/32] Filtering nodes - intersection â¢ 0:00:00 â 
+``` #### Use as CLI ```console $ quackosm monaco.osm.pbf â  [ 1/32] Reading
+nodes â¢ 0:00:00 â  [ 2/32] Filtering nodes - intersection â¢ 0:00:00 â 
 [ 3/32] Filtering nodes - tags â¢ 0:00:00 â  [ 4/32] Calculating distinct
-filtered nodes ids â¢ 0:00:00 â  [ 5/32] Reading ways â¢ 0:00:00 â  [ 6/32]
-Unnesting ways â¢ 0:00:00 â ¹ [ 7/32] Filtering ways - valid refs â¢ 0:00:00
-â  [ 8/32] Filtering ways - intersection â¢ 0:00:00 â  [ 9/32] Filtering
+filtered nodes ids â¢ 0:00:00 â  [ 5/32] Reading ways â¢ 0:00:00 â  [ 6/32]
+Unnesting ways â¢ 0:00:00 â  [ 7/32] Filtering ways - valid refs â¢ 0:00:00
+â  [ 8/32] Filtering ways - intersection â¢ 0:00:00 â  [ 9/32] Filtering
 ways - tags â¢ 0:00:00 â  [ 10/32] Calculating distinct filtered ways ids â¢
 0:00:00 â  [ 11/32] Reading relations â¢ 0:00:00 â  [ 12/32] Unnesting
-relations â¢ 0:00:00 â ¹ [ 13/32] Filtering relations - valid refs â¢ 0:00:00
-â  [ 14/32] Filtering relations - intersection â¢ 0:00:00 â  [ 15/32]
+relations â¢ 0:00:00 â ¸ [ 13/32] Filtering relations - valid refs â¢ 0:00:00
+â  [ 14/32] Filtering relations - intersection â¢ 0:00:00 â  [ 15/32]
 Filtering relations - tags â¢ 0:00:00 â  [ 16/32] Calculating distinct
-filtered relations ids â¢ 0:00:00 â  [ 17/32] Loading required ways - by
+filtered relations ids â¢ 0:00:00 â  [ 17/32] Loading required ways - by
 relations â¢ 0:00:00 â  [ 18/32] Calculating distinct required ways ids â¢
-0:00:00 â  [ 19/32] Saving filtered nodes with geometries â¢ 0:00:00 â 
+0:00:00 â  [ 19/32] Saving filtered nodes with geometries â¢ 0:00:00 â 
 [20.1/32] Grouping filtered ways - assigning groups â¢ 0:00:00 â § [20.2/32]
 Grouping filtered ways - joining with nodes â¢ 0:00:00 â  [20.3/32] Grouping
 filtered ways - partitioning by group â¢ 0:00:00 [ 21/32] Saving filtered ways
 with linestrings 100%
 ââââââââââââââââââââââââââââââââââââââââ
 1/1 â¢ 0:00:00 < 0:00:00 â¢ â  [22.1/32] Grouping required ways - assigning
 groups â¢ 0:00:00 â § [22.2/32] Grouping required ways - joining with nodes
 â¢ 0:00:00 â  [22.3/32] Grouping required ways - partitioning by group â¢ 0:
 00:00 [ 23/32] Saving required ways with linestrings 100%
 ââââââââââââââââââââââââââââââââââââââââ
-1/1 â¢ 0:00:00 < 0:00:00 â¢ â ¹ [ 24/32] Saving filtered ways with geometries
-â¢ 0:00:00 â ¸ [ 25/32] Saving valid relations parts â¢ 0:00:00 â  [26.1/32]
-Saving relations inner parts - valid geometries â¢ 0:00:00 â  [26.2/32]
-Saving relations inner parts - invalid geometries â¢ 0:00:00 â  [27.1/32]
-Saving relations outer parts - valid geometries â¢ 0:00:00 â  [27.2/32]
-Saving relations outer parts - invalid geometries â¢ 0:00:00 â  [ 28/32]
-Saving relations outer parts with holes â¢ 0:00:00 â  [ 29/32] Saving
-relations outer parts without holes â¢ 0:00:00 â  [ 30/32] Saving filtered
-relations with geometries â¢ 0:00:00 â ¹ [31.1/32] Saving valid features â¢
-0:00:00 â  [ 32/32] Saving final geoparquet file â¢ 0:00:00 Finished
-operation in 0:00:06 files/monaco_nofilter_noclip_compact.parquet ``` ### Let
-the QuackOSM automatically download the required OSM PBF files for you ðð
-#### Load data as a GeoDataFrame ```python >>> import quackosm as qosm >>>
-import osmnx as ox >>> geometry = ox.geocode_to_gdf("Vatican City").unary_union
->>> qosm.get_features_gdf_from_geometry(geometry) tags geometry feature_id
-node/10253371713 {'crossing': 'uncontrolled',... POINT (12.45603 41.90454)
-node/10253371714 {'highway': 'stop'} POINT (12.45705 41.90400) node/10253371715
+1/1 â¢ 0:00:00 < 0:00:00 â¢ â  [ 24/32] Saving filtered ways with geometries
+â¢ 0:00:00 â  [ 25/32] Saving valid relations parts â¢ 0:00:00 â  [ 26/32]
+Saving relations inner parts â¢ 0:00:00 â  [ 27/32] Saving relations outer
+parts â¢ 0:00:00 â  [ 28/32] Saving relations outer parts with holes â¢ 0:
+00:00 â  [ 29/32] Saving relations outer parts without holes â¢ 0:00:00 â 
+[ 30/32] Saving filtered relations with geometries â¢ 0:00:00 â  [ 31/32]
+Saving all features â¢ 0:00:00 â  [ 32/32] Saving final geoparquet file â¢
+0:00:00 Finished operation in 0:00:03 files/
+monaco_nofilter_noclip_compact.parquet ``` ### Let the QuackOSM automatically
+download the required OSM PBF files for you ðð #### Load data as a
+GeoDataFrame ```python >>> import quackosm as qosm >>> import osmnx as ox >>>
+geometry = ox.geocode_to_gdf("Vatican City").unary_union >>>
+qosm.convert_geometry_to_geodataframe(geometry) tags geometry feature_id node/
+10253371713 {'crossing': 'uncontrolled',... POINT (12.45603 41.90454) node/
+10253371714 {'highway': 'stop'} POINT (12.45705 41.90400) node/10253371715
 {'highway': 'stop'} POINT (12.45242 41.90164) node/10253371720 {'artwork_type':
 'statue',... POINT (12.45147 41.90484) node/10253371738 {'natural': 'tree'}
 POINT (12.45595 41.90609) ... ... ... way/983015528 {'barrier': 'hedge',
 'height'... POLYGON ((12.45027 41.901... way/983015529 {'barrier': 'hedge',
 'height'... POLYGON ((12.45028 41.901... way/983015530 {'barrier': 'hedge',
 'height'... POLYGON ((12.45023 41.901... way/998561138 {'barrier': 'bollard',
 'bicyc... LINESTRING (12.45821 41.9... way/998561139 {'barrier': 'bollard',
 'bicyc... LINESTRING (12.45828 41.9... [3286 rows x 2 columns] ``` #### Just
 convert geometry to GeoParquet ```python >>> import quackosm as qosm >>> from
 shapely import from_wkt >>> geometry = from_wkt( ... "POLYGON ((14.4861
 35.9107, 14.4861 35.8811, 14.5331 35.8811, 14.5331 35.9107, 14.4861 35.9107))"
-... ) >>> gpq_path = qosm.convert_geometry_to_gpq(geometry) >>>
+... ) >>> gpq_path = qosm.convert_geometry_to_parquet(geometry) >>>
 gpq_path.as_posix() 'files/
 4b2967088a8fe31cdc15401e29bff9b7b882565cd8143e90443f39f2dc5fe6de_nofilter_compact.parquet'
 ``` #### Inspect the file with duckdb ```python >>> import duckdb >>>
 duckdb.load_extension('spatial') >>> duckdb.read_parquet(str(gpq_path)).project
 ( ... "* REPLACE (ST_GeomFromWKB(geometry) AS geometry)" ... ).order
 ("feature_id")
 ââââââââââââââââââââ¬âââââââââââââââââââââââ¬âââââââââââââââââââââââââââââââââââââââââââââââ
@@ -205,49 +203,46 @@
 (14.5221083 35.8864287, 14.5221â¦ â
 ââââââââââââââââââââ´âââââââââââââââââââââââ´âââââââââââââââââââââââââââââââââââââââââââââââ¤
 â ? rows (>9999 rows, 20 shown) 3 columns â
 ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
 ``` #### Use as CLI ```console $ quackosm --geom-filter-geocode "Shibuya,
 Tokyo"
 100%|ââââââââââââââââââââââââââââââââââââââ|
-45.7M/45.7M [00:00<00:00, 259GB/s] â ¦ [ 1/32] Reading nodes â¢ 0:00:05 â 
-[ 2/32] Filtering nodes - intersection â¢ 0:00:00 â ¦ [ 3/32] Filtering nodes
+46.3M/46.3M [00:00<00:00, 327GB/s] â  [ 1/32] Reading nodes â¢ 0:00:01 â ¹
+[ 2/32] Filtering nodes - intersection â¢ 0:00:00 â  [ 3/32] Filtering nodes
 - tags â¢ 0:00:00 â  [ 4/32] Calculating distinct filtered nodes ids â¢ 0:
-00:00 â  [ 5/32] Reading ways â¢ 0:00:04 â ¦ [ 6/32] Unnesting ways â¢ 0:00:
-02 â ´ [ 7/32] Filtering ways - valid refs â¢ 0:00:02 â  [ 8/32] Filtering
-ways - intersection â¢ 0:00:01 â ¹ [ 9/32] Filtering ways - tags â¢ 0:00:00
-â  [ 10/32] Calculating distinct filtered ways ids â¢ 0:00:00 â ´ [ 11/32]
-Reading relations â¢ 0:00:00 â ´ [ 12/32] Unnesting relations â¢ 0:00:00 â ¹
-[ 13/32] Filtering relations - valid refs â¢ 0:00:00 â  [ 14/32] Filtering
-relations - intersection â¢ 0:00:00 â  [ 15/32] Filtering relations - tags
+00:00 â ¸ [ 5/32] Reading ways â¢ 0:00:03 â ´ [ 6/32] Unnesting ways â¢ 0:00:
+01 â ¼ [ 7/32] Filtering ways - valid refs â¢ 0:00:00 â ¹ [ 8/32] Filtering
+ways - intersection â¢ 0:00:00 â  [ 9/32] Filtering ways - tags â¢ 0:00:00
+â  [ 10/32] Calculating distinct filtered ways ids â¢ 0:00:00 â ¼ [ 11/32]
+Reading relations â¢ 0:00:00 â ¸ [ 12/32] Unnesting relations â¢ 0:00:00 â 
+[ 13/32] Filtering relations - valid refs â¢ 0:00:00 â  [ 14/32] Filtering
+relations - intersection â¢ 0:00:00 â  [ 15/32] Filtering relations - tags
 â¢ 0:00:00 â  [ 16/32] Calculating distinct filtered relations ids â¢ 0:00:
-00 â  [ 17/32] Loading required ways - by relations â¢ 0:00:00 â  [ 18/32]
-Calculating distinct required ways ids â¢ 0:00:00 â  [ 19/32] Saving filtered
+00 â  [ 17/32] Loading required ways - by relations â¢ 0:00:00 â  [ 18/32]
+Calculating distinct required ways ids â¢ 0:00:00 â ¹ [ 19/32] Saving filtered
 nodes with geometries â¢ 0:00:00 â  [20.1/32] Grouping filtered ways -
-assigning groups â¢ 0:00:00 â ´ [20.2/32] Grouping filtered ways - joining
-with nodes â¢ 0:00:03 â ¹ [20.3/32] Grouping filtered ways - partitioning by
+assigning groups â¢ 0:00:00 â ¼ [20.2/32] Grouping filtered ways - joining
+with nodes â¢ 0:00:01 â  [20.3/32] Grouping filtered ways - partitioning by
 group â¢ 0:00:00 [ 21/32] Saving filtered ways with linestrings 100%
 ââââââââââââââââââââââââââââââââââââââââ
-1/1 â¢ 0:00:01 < 0:00:00 â¢ â  [22.1/32] Grouping required ways - assigning
-groups â¢ 0:00:00 â ´ [22.2/32] Grouping required ways - joining with nodes
-â¢ 0:00:03 â  [22.3/32] Grouping required ways - partitioning by group â¢ 0:
+1/1 â¢ 0:00:00 < 0:00:00 â¢ â  [22.1/32] Grouping required ways - assigning
+groups â¢ 0:00:00 â ¼ [22.2/32] Grouping required ways - joining with nodes
+â¢ 0:00:01 â  [22.3/32] Grouping required ways - partitioning by group â¢ 0:
 00:00 [ 23/32] Saving required ways with linestrings 100%
 ââââââââââââââââââââââââââââââââââââââââ
-1/1 â¢ 0:00:00 < 0:00:00 â¢ â  [ 24/32] Saving filtered ways with geometries
-â¢ 0:00:01 â ¸ [ 25/32] Saving valid relations parts â¢ 0:00:00 â  [26.1/32]
-Saving relations inner parts - valid geometries â¢ 0:00:00 â  [26.2/32]
-Saving relations inner parts - invalid geometries â¢ 0:00:00 â  [27.1/32]
-Saving relations outer parts - valid geometries â¢ 0:00:00 â  [27.2/32]
-Saving relations outer parts - invalid geometries â¢ 0:00:00 â  [ 28/32]
-Saving relations outer parts with holes â¢ 0:00:00 â  [ 29/32] Saving
-relations outer parts without holes â¢ 0:00:00 â  [ 30/32] Saving filtered
-relations with geometries â¢ 0:00:00 â ¸ [31.1/32] Saving valid features â¢
-0:00:00 â  [ 32/32] Saving final geoparquet file â¢ 0:00:00 Finished
-operation in 0:00:39 files/
-9ae2b160eb7556991148f5a2693aaf4b38bbb225c3700a6bfe9e5e54f48b987e_nofilter_compact.parquet
+1/1 â¢ 0:00:00 < 0:00:00 â¢ â ´ [ 24/32] Saving filtered ways with geometries
+â¢ 0:00:00 â  [ 25/32] Saving valid relations parts â¢ 0:00:00 â  [ 26/32]
+Saving relations inner parts â¢ 0:00:00 â  [ 27/32] Saving relations outer
+parts â¢ 0:00:00 â  [ 28/32] Saving relations outer parts with holes â¢ 0:
+00:00 â  [ 29/32] Saving relations outer parts without holes â¢ 0:00:00 â 
+[ 30/32] Saving filtered relations with geometries â¢ 0:00:00 â  [ 31/32]
+Saving all features â¢ 0:00:00 â  [ 32/32] Saving final geoparquet file â¢
+0:00:00 Finished operation in 0:00:13 files/
+78580cf29b5ba1073366a257e1909bfeee43c9f5859e48fb3b2d592028bb58aa_nofilter_compact.parquet
 ``` CLI Help output (`QuackOSM -h`): ![CLI Help output](https://
 raw.githubusercontent.com/kraina-ai/quackosm/main/docs/assets/images/
 cli_help.png) You can find full API + more examples in the [docs](https://
 kraina-ai.github.io/quackosm/). ## How does it work? ### Basic logic QuackOSM
 utilizes `ST_ReadOSM` function from `DuckDB`'s `Spatial` extension to read raw
 data from the PBF file: - **Nodes** with coordinates and tags; - **Ways** with
 nodes refs and tags; - **Relations** with nodes and ways refs, ref roles and
```

