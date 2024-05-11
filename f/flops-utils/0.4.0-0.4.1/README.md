# Comparing `tmp/flops_utils-0.4.0.tar.gz` & `tmp/flops_utils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.4.0.tar", max compression
+gzip compressed data, was "flops_utils-0.4.1.tar", max compression
```

## Comparing `flops_utils-0.4.0.tar` & `flops_utils-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.4.0/README.md
--rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.4.0/flops_utils/logging.py
--rw-r--r--   0        0        0      782 2024-05-05 12:55:14.703088 flops_utils-0.4.0/flops_utils/ml_model_flavor_wrapper.py
--rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.4.0/flops_utils/ml_repo_files_wrapper.py
--rw-r--r--   0        0        0     2632 2024-05-05 10:09:52.795212 flops_utils-0.4.0/flops_utils/ml_repo_templates.py
--rw-r--r--   0        0        0     1441 2024-05-11 09:55:30.969946 flops_utils-0.4.0/flops_utils/notifications.py
--rw-r--r--   0        0        0     2180 2024-05-11 18:03:51.996035 flops_utils-0.4.0/flops_utils/timer.py
--rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.4.0/flops_utils/types.py
--rw-r--r--   0        0        0      455 2024-05-11 18:06:16.740038 flops_utils-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 flops_utils-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.4.1/README.md
+-rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.4.1/flops_utils/logging.py
+-rw-r--r--   0        0        0      782 2024-05-05 12:55:14.703088 flops_utils-0.4.1/flops_utils/ml_model_flavor_wrapper.py
+-rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.4.1/flops_utils/ml_repo_files_wrapper.py
+-rw-r--r--   0        0        0     2632 2024-05-05 10:09:52.795212 flops_utils-0.4.1/flops_utils/ml_repo_templates.py
+-rw-r--r--   0        0        0     1441 2024-05-11 09:55:30.969946 flops_utils-0.4.1/flops_utils/notifications.py
+-rw-r--r--   0        0        0     2339 2024-05-11 18:20:37.624055 flops_utils-0.4.1/flops_utils/timer.py
+-rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.4.1/flops_utils/types.py
+-rw-r--r--   0        0        0      455 2024-05-11 18:20:44.416055 flops_utils-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 flops_utils-0.4.1/PKG-INFO
```

### Comparing `flops_utils-0.4.0/flops_utils/logging.py` & `flops_utils-0.4.1/flops_utils/logging.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.0/flops_utils/ml_model_flavor_wrapper.py` & `flops_utils-0.4.1/flops_utils/ml_model_flavor_wrapper.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.0/flops_utils/ml_repo_templates.py` & `flops_utils-0.4.1/flops_utils/ml_repo_templates.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.0/flops_utils/notifications.py` & `flops_utils-0.4.1/flops_utils/notifications.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.0/flops_utils/timer.py` & `flops_utils-0.4.1/flops_utils/timer.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,24 +43,29 @@
     time_frames: Dict[str, TimeFrame] = {}
 
     def create_new_time_stamp(self, name: str) -> datetime:
         new_timestamp = datetime.now()
         self.time_stamps[name] = new_timestamp
         return new_timestamp
 
-    def create_new_time_frame(self, name: str) -> TimeFrame:
+    def start_new_time_frame(self, name: str) -> TimeFrame:
         new_time_frame = TimeFrame()
         self.time_frames[name] = new_time_frame
         return new_time_frame
 
+    def end_time_frame(self, name: str) -> TimeFrame:
+        time_frame = self.time_frames[name]
+        time_frame.end_time_frame()
+        return time_frame
+
     def get_timestamp(self, name: str) -> datetime:
         return self.time_stamps.get(name, self.create_new_time_stamp(name))
 
     def get_time_frame(self, name: str) -> TimeFrame:
-        return self.time_frames.get(name, self.create_new_time_frame(name))
+        return self.time_frames.get(name, self.start_new_time_frame(name))
 
     def get_duration_between_timestamps(
         self,
         timestamp_a_name: str,
         timestamp_b_name: str,
         human_readable: bool = False,
     ) -> Union[float, str]:
```

### Comparing `flops_utils-0.4.0/PKG-INFO` & `flops_utils-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flops_utils
-Version: 0.4.0
+Version: 0.4.1
 Summary: A library containing commong utilities for FLOps
 Author: Alexander Malyuk
 Author-email: malyuk.alexander1999@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

