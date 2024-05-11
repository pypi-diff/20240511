# Comparing `tmp/sindapi-0.0.8.tar.gz` & `tmp/sindapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sindapi-0.0.8.tar", last modified: Sat Apr 13 08:56:01 2024, max compression
+gzip compressed data, was "sindapi-0.0.9.tar", last modified: Sat Apr 13 13:07:56 2024, max compression
```

## Comparing `sindapi-0.0.8.tar` & `sindapi-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 08:56:01.323677 sindapi-0.0.8/
--rw-rw-rw-   0        0        0      334 2024-04-13 08:56:01.323677 sindapi-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-13 08:56:01.323677 sindapi-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      440 2024-04-13 08:54:00.000000 sindapi-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:56:01.278910 sindapi-0.0.8/sindapi/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:46:37.000000 sindapi-0.0.8/sindapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:56:01.308635 sindapi-0.0.8/sindapi/sindmap/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:43:26.000000 sindapi-0.0.8/sindapi/sindmap/__init__.py
--rw-rw-rw-   0        0        0      197 2024-04-09 10:01:35.000000 sindapi-0.0.8/sindapi/sindmap/drivable_area.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:56:01.308635 sindapi-0.0.8/sindapi/sindmap/intersection/
--rw-rw-rw-   0        0        0        0 2024-04-05 06:38:33.000000 sindapi-0.0.8/sindapi/sindmap/intersection/__init__.py
--rw-rw-rw-   0        0        0    10765 2024-04-09 08:57:10.000000 sindapi-0.0.8/sindapi/sindmap/intersection/intersection.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:56:01.308635 sindapi-0.0.8/sindapi/sindmap/lane/
--rw-rw-rw-   0        0        0        0 2024-04-05 15:13:39.000000 sindapi-0.0.8/sindapi/sindmap/lane/__init__.py
--rw-rw-rw-   0        0        0    10258 2024-04-09 08:56:55.000000 sindapi-0.0.8/sindapi/sindmap/lane/lane_segment.py
--rw-rw-rw-   0        0        0     4503 2024-04-10 14:52:17.000000 sindapi-0.0.8/sindapi/sindmap/map_api.py
--rw-rw-rw-   0        0        0     1483 2024-04-09 12:32:07.000000 sindapi-0.0.8/sindapi/sindmap/pedestrian_crossing.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:56:01.308635 sindapi-0.0.8/sindapi/sindmap/stretch/
--rw-rw-rw-   0        0        0        0 2024-04-05 06:15:01.000000 sindapi-0.0.8/sindapi/sindmap/stretch/__init__.py
--rw-rw-rw-   0        0        0     1450 2024-04-09 08:47:01.000000 sindapi-0.0.8/sindapi/sindmap/stretch/stretch.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:56:01.308635 sindapi-0.0.8/sindapi/sindmap/traffic_light/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:05:17.000000 sindapi-0.0.8/sindapi/sindmap/traffic_light/__init__.py
--rw-rw-rw-   0        0        0     1498 2024-04-11 09:39:33.000000 sindapi-0.0.8/sindapi/sindmap/traffic_light/traffic_light.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:56:01.308635 sindapi-0.0.8/sindapi/sindmap/utils/
--rw-rw-rw-   0        0        0        0 2024-04-05 09:04:36.000000 sindapi-0.0.8/sindapi/sindmap/utils/__init__.py
--rw-rw-rw-   0        0        0     1955 2024-04-09 12:32:07.000000 sindapi-0.0.8/sindapi/sindmap/utils/map_primitives.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:56:01.308635 sindapi-0.0.8/sindapi/sindtrack/
--rw-rw-rw-   0        0        0        0 2024-04-09 12:17:04.000000 sindapi-0.0.8/sindapi/sindtrack/__init__.py
--rw-rw-rw-   0        0        0     4587 2024-04-13 08:53:45.000000 sindapi-0.0.8/sindapi/sindtrack/data_schema.py
--rw-rw-rw-   0        0        0    12157 2024-04-13 08:41:42.000000 sindapi-0.0.8/sindapi/sindtrack/process_raw_data.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:56:01.323677 sindapi-0.0.8/sindapi/sindtrack/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 12:17:04.000000 sindapi-0.0.8/sindapi/sindtrack/utils/__init__.py
--rw-rw-rw-   0        0        0      561 2024-04-11 08:39:35.000000 sindapi-0.0.8/sindapi/sindtrack/utils/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:56:01.323677 sindapi-0.0.8/sindapi/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:46:37.000000 sindapi-0.0.8/sindapi/utils/__init__.py
--rw-rw-rw-   0        0        0      473 2024-04-05 14:52:09.000000 sindapi-0.0.8/sindapi/utils/typing.py
-drwxrwxrwx   0        0        0        0 2024-04-13 08:56:01.292521 sindapi-0.0.8/sindapi.egg-info/
--rw-rw-rw-   0        0        0      334 2024-04-13 08:56:01.000000 sindapi-0.0.8/sindapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      923 2024-04-13 08:56:01.000000 sindapi-0.0.8/sindapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 08:56:01.000000 sindapi-0.0.8/sindapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-13 08:56:01.000000 sindapi-0.0.8/sindapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-13 08:56:01.000000 sindapi-0.0.8/sindapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 13:07:56.232273 sindapi-0.0.9/
+-rw-rw-rw-   0        0        0      334 2024-04-13 13:07:56.230275 sindapi-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-13 13:07:56.232273 sindapi-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      440 2024-04-13 13:05:45.000000 sindapi-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 13:07:56.175648 sindapi-0.0.9/sindapi/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:46:37.000000 sindapi-0.0.9/sindapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 13:07:56.212265 sindapi-0.0.9/sindapi/sindmap/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:43:26.000000 sindapi-0.0.9/sindapi/sindmap/__init__.py
+-rw-rw-rw-   0        0        0      197 2024-04-09 10:01:35.000000 sindapi-0.0.9/sindapi/sindmap/drivable_area.py
+drwxrwxrwx   0        0        0        0 2024-04-13 13:07:56.214266 sindapi-0.0.9/sindapi/sindmap/intersection/
+-rw-rw-rw-   0        0        0        0 2024-04-05 06:38:33.000000 sindapi-0.0.9/sindapi/sindmap/intersection/__init__.py
+-rw-rw-rw-   0        0        0    10765 2024-04-09 08:57:10.000000 sindapi-0.0.9/sindapi/sindmap/intersection/intersection.py
+drwxrwxrwx   0        0        0        0 2024-04-13 13:07:56.218277 sindapi-0.0.9/sindapi/sindmap/lane/
+-rw-rw-rw-   0        0        0        0 2024-04-05 15:13:39.000000 sindapi-0.0.9/sindapi/sindmap/lane/__init__.py
+-rw-rw-rw-   0        0        0    10258 2024-04-09 08:56:55.000000 sindapi-0.0.9/sindapi/sindmap/lane/lane_segment.py
+-rw-rw-rw-   0        0        0     4510 2024-04-13 13:06:02.000000 sindapi-0.0.9/sindapi/sindmap/map_api.py
+-rw-rw-rw-   0        0        0     1483 2024-04-09 12:32:07.000000 sindapi-0.0.9/sindapi/sindmap/pedestrian_crossing.py
+drwxrwxrwx   0        0        0        0 2024-04-13 13:07:56.220266 sindapi-0.0.9/sindapi/sindmap/stretch/
+-rw-rw-rw-   0        0        0        0 2024-04-05 06:15:01.000000 sindapi-0.0.9/sindapi/sindmap/stretch/__init__.py
+-rw-rw-rw-   0        0        0     1450 2024-04-09 08:47:01.000000 sindapi-0.0.9/sindapi/sindmap/stretch/stretch.py
+drwxrwxrwx   0        0        0        0 2024-04-13 13:07:56.222273 sindapi-0.0.9/sindapi/sindmap/traffic_light/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:05:17.000000 sindapi-0.0.9/sindapi/sindmap/traffic_light/__init__.py
+-rw-rw-rw-   0        0        0     1498 2024-04-11 09:39:33.000000 sindapi-0.0.9/sindapi/sindmap/traffic_light/traffic_light.py
+drwxrwxrwx   0        0        0        0 2024-04-13 13:07:56.223273 sindapi-0.0.9/sindapi/sindmap/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-05 09:04:36.000000 sindapi-0.0.9/sindapi/sindmap/utils/__init__.py
+-rw-rw-rw-   0        0        0     1955 2024-04-09 12:32:07.000000 sindapi-0.0.9/sindapi/sindmap/utils/map_primitives.py
+drwxrwxrwx   0        0        0        0 2024-04-13 13:07:56.226273 sindapi-0.0.9/sindapi/sindtrack/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:17:04.000000 sindapi-0.0.9/sindapi/sindtrack/__init__.py
+-rw-rw-rw-   0        0        0     4587 2024-04-13 08:53:45.000000 sindapi-0.0.9/sindapi/sindtrack/data_schema.py
+-rw-rw-rw-   0        0        0    12157 2024-04-13 08:41:42.000000 sindapi-0.0.9/sindapi/sindtrack/process_raw_data.py
+drwxrwxrwx   0        0        0        0 2024-04-13 13:07:56.227273 sindapi-0.0.9/sindapi/sindtrack/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 12:17:04.000000 sindapi-0.0.9/sindapi/sindtrack/utils/__init__.py
+-rw-rw-rw-   0        0        0      561 2024-04-11 08:39:35.000000 sindapi-0.0.9/sindapi/sindtrack/utils/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-13 13:07:56.229275 sindapi-0.0.9/sindapi/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:46:37.000000 sindapi-0.0.9/sindapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-04-05 14:52:09.000000 sindapi-0.0.9/sindapi/utils/typing.py
+drwxrwxrwx   0        0        0        0 2024-04-13 13:07:56.209265 sindapi-0.0.9/sindapi.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-04-13 13:07:56.000000 sindapi-0.0.9/sindapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2024-04-13 13:07:56.000000 sindapi-0.0.9/sindapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 13:07:56.000000 sindapi-0.0.9/sindapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-13 13:07:56.000000 sindapi-0.0.9/sindapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-13 13:07:56.000000 sindapi-0.0.9/sindapi.egg-info/top_level.txt
```

### Comparing `sindapi-0.0.8/sindapi/sindmap/intersection/intersection.py` & `sindapi-0.0.9/sindapi/sindmap/intersection/intersection.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.8/sindapi/sindmap/lane/lane_segment.py` & `sindapi-0.0.9/sindapi/sindmap/lane/lane_segment.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.8/sindapi/sindmap/map_api.py` & `sindapi-0.0.9/sindapi/sindmap/map_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class SinDStaticMap:
     city_name: str
     vector_drivable_areas: Dict[int, DrivableArea]
     vector_pedestrian_crossings: Dict[int, PedestrianCrossing]
     vector_stretches: Dict[int, Stretch]
     vector_intersections: Dict[int, Intersection]
     vector_lane_segments: Dict[int, LaneSegment]
-    map_id: Optional[str]
+    map_id: Optional[str] = None
     split_distance: float = None
     segment_point_num: int = None
 
     @classmethod
     def from_cfg(cls, config_path):
         with config_path.open('r') as file:
             config = yaml.safe_load(file)
```

### Comparing `sindapi-0.0.8/sindapi/sindmap/pedestrian_crossing.py` & `sindapi-0.0.9/sindapi/sindmap/pedestrian_crossing.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.8/sindapi/sindmap/stretch/stretch.py` & `sindapi-0.0.9/sindapi/sindmap/stretch/stretch.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.8/sindapi/sindmap/traffic_light/traffic_light.py` & `sindapi-0.0.9/sindapi/sindmap/traffic_light/traffic_light.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.8/sindapi/sindmap/utils/map_primitives.py` & `sindapi-0.0.9/sindapi/sindmap/utils/map_primitives.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.8/sindapi/sindtrack/data_schema.py` & `sindapi-0.0.9/sindapi/sindtrack/data_schema.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.8/sindapi/sindtrack/process_raw_data.py` & `sindapi-0.0.9/sindapi/sindtrack/process_raw_data.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.8/sindapi/sindtrack/utils/constants.py` & `sindapi-0.0.9/sindapi/sindtrack/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sindapi-0.0.8/sindapi.egg-info/SOURCES.txt` & `sindapi-0.0.9/sindapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

