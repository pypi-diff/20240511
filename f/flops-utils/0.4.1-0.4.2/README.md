# Comparing `tmp/flops_utils-0.4.1.tar.gz` & `tmp/flops_utils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.4.1.tar", max compression
+gzip compressed data, was "flops_utils-0.4.2.tar", max compression
```

## Comparing `flops_utils-0.4.1.tar` & `flops_utils-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.4.1/README.md
--rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.4.1/flops_utils/logging.py
--rw-r--r--   0        0        0      782 2024-05-05 12:55:14.703088 flops_utils-0.4.1/flops_utils/ml_model_flavor_wrapper.py
--rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.4.1/flops_utils/ml_repo_files_wrapper.py
--rw-r--r--   0        0        0     2632 2024-05-05 10:09:52.795212 flops_utils-0.4.1/flops_utils/ml_repo_templates.py
--rw-r--r--   0        0        0     1441 2024-05-11 09:55:30.969946 flops_utils-0.4.1/flops_utils/notifications.py
--rw-r--r--   0        0        0     2339 2024-05-11 18:20:37.624055 flops_utils-0.4.1/flops_utils/timer.py
--rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.4.1/flops_utils/types.py
--rw-r--r--   0        0        0      455 2024-05-11 18:20:44.416055 flops_utils-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 flops_utils-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.4.2/README.md
+-rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.4.2/flops_utils/logging.py
+-rw-r--r--   0        0        0      782 2024-05-05 12:55:14.703088 flops_utils-0.4.2/flops_utils/ml_model_flavor_wrapper.py
+-rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.4.2/flops_utils/ml_repo_files_wrapper.py
+-rw-r--r--   0        0        0     2632 2024-05-05 10:09:52.795212 flops_utils-0.4.2/flops_utils/ml_repo_templates.py
+-rw-r--r--   0        0        0     1441 2024-05-11 09:55:30.969946 flops_utils-0.4.2/flops_utils/notifications.py
+-rw-r--r--   0        0        0     2357 2024-05-11 18:40:01.636077 flops_utils-0.4.2/flops_utils/timer.py
+-rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.4.2/flops_utils/types.py
+-rw-r--r--   0        0        0      457 2024-05-11 18:41:35.680079 flops_utils-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.4.2/PKG-INFO
```

### Comparing `flops_utils-0.4.1/flops_utils/logging.py` & `flops_utils-0.4.2/flops_utils/logging.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.1/flops_utils/ml_model_flavor_wrapper.py` & `flops_utils-0.4.2/flops_utils/ml_model_flavor_wrapper.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.1/flops_utils/ml_repo_templates.py` & `flops_utils-0.4.2/flops_utils/ml_repo_templates.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.1/flops_utils/notifications.py` & `flops_utils-0.4.2/flops_utils/notifications.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.4.1/flops_utils/timer.py` & `flops_utils-0.4.2/flops_utils/timer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Dict, Union
 
-from pydantic import BaseModel, Field
-
 
 def _get_duration(
     start: datetime,
     end: datetime,
     human_readable: bool = False,
 ) -> Union[float, str]:
     duration = end - start
@@ -18,31 +17,33 @@
     human_readable_res = ""
     if minutes:
         human_readable_res += f"'{minutes}' minutes and "
     human_readable_res += f"{seconds} seconds"
     return human_readable_res
 
 
-class TimeFrame(BaseModel):
-    start_time: datetime = Field(datetime.now(), init=False)
-    end_time: datetime = Field(None, init=False)
+@dataclass
+class TimeFrame:
+    start_time: datetime = field(default=datetime.now(), init=False)
+    end_time: datetime = field(default=None, init=False)
 
     def end_time_frame(self) -> datetime:
         self.end_time = datetime.now()
         return self.end_time
 
     def get_duration(self, human_readable: bool = False) -> Union[float, str]:
         return _get_duration(
             start=self.start_time,
             end=(self.end_time or self.end_time_frame()),
             human_readable=human_readable,
         )
 
 
-class Timer(BaseModel):
+@dataclass
+class Timer:
     time_stamps: Dict[str, datetime] = {}
     time_frames: Dict[str, TimeFrame] = {}
 
     def create_new_time_stamp(self, name: str) -> datetime:
         new_timestamp = datetime.now()
         self.time_stamps[name] = new_timestamp
         return new_timestamp
```

