# Comparing `tmp/FlowVisor-0.1.4.tar.gz` & `tmp/FlowVisor-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowVisor-0.1.4.tar", last modified: Thu May  9 19:18:06 2024, max compression
+gzip compressed data, was "FlowVisor-0.1.5.tar", last modified: Sat May 11 06:00:17 2024, max compression
```

## Comparing `FlowVisor-0.1.4.tar` & `FlowVisor-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-09 19:18:06.511158 FlowVisor-0.1.4/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-09 19:18:06.507158 FlowVisor-0.1.4/FlowVisor.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-09 19:18:06.000000 FlowVisor-0.1.4/FlowVisor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-09 19:18:06.000000 FlowVisor-0.1.4/FlowVisor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-09 19:18:06.000000 FlowVisor-0.1.4/FlowVisor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-09 19:18:06.000000 FlowVisor-0.1.4/FlowVisor.egg-info/entry_points.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       52 2024-05-09 19:18:06.000000 FlowVisor-0.1.4/FlowVisor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-09 19:18:06.000000 FlowVisor-0.1.4/FlowVisor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.4/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-09 19:18:06.511158 FlowVisor-0.1.4/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.4/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-09 19:18:06.511158 FlowVisor-0.1.4/flowvisor/
--rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.1.4/flowvisor/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-09 19:18:06.511158 FlowVisor-0.1.4/flowvisor/cli/
--rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.4/flowvisor/cli/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.4/flowvisor/cli/add_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.4/flowvisor/cli/remove_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.4/flowvisor/cli/vis_file.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    15931 2024-05-09 09:31:09.000000 FlowVisor-0.1.4/flowvisor/flowvisor.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     1751 2024-05-09 19:13:08.000000 FlowVisor-0.1.4/flowvisor/flowvisor_config.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     6185 2024-05-09 19:17:48.000000 FlowVisor-0.1.4/flowvisor/flowvisor_verifier.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8004 2024-05-09 07:05:50.000000 FlowVisor-0.1.4/flowvisor/function_node.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       98 2024-05-09 06:06:21.000000 FlowVisor-0.1.4/flowvisor/logger.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.1.4/flowvisor/sankey.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.4/flowvisor/time_tracker.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      292 2024-05-08 15:25:05.000000 FlowVisor-0.1.4/flowvisor/time_value.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.1.4/flowvisor/timer.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.1.4/flowvisor/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-09 19:18:06.511158 FlowVisor-0.1.4/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.4/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-11 06:00:17.583484 FlowVisor-0.1.5/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-11 06:00:17.583484 FlowVisor-0.1.5/FlowVisor.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-11 06:00:17.000000 FlowVisor-0.1.5/FlowVisor.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-11 06:00:17.000000 FlowVisor-0.1.5/FlowVisor.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-11 06:00:17.000000 FlowVisor-0.1.5/FlowVisor.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-11 06:00:17.000000 FlowVisor-0.1.5/FlowVisor.egg-info/entry_points.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       59 2024-05-11 06:00:17.000000 FlowVisor-0.1.5/FlowVisor.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-11 06:00:17.000000 FlowVisor-0.1.5/FlowVisor.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.1.5/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3697 2024-05-11 06:00:17.583484 FlowVisor-0.1.5/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3016 2024-04-25 13:11:25.000000 FlowVisor-0.1.5/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-11 06:00:17.583484 FlowVisor-0.1.5/flowvisor/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.1.5/flowvisor/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-11 06:00:17.583484 FlowVisor-0.1.5/flowvisor/cli/
+-rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.1.5/flowvisor/cli/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.1.5/flowvisor/cli/add_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.1.5/flowvisor/cli/remove_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      911 2024-04-25 13:10:38.000000 FlowVisor-0.1.5/flowvisor/cli/vis_file.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)    16418 2024-05-11 05:55:43.000000 FlowVisor-0.1.5/flowvisor/flowvisor.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2030 2024-05-11 05:24:19.000000 FlowVisor-0.1.5/flowvisor/flowvisor_config.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     7894 2024-05-11 05:40:17.000000 FlowVisor-0.1.5/flowvisor/flowvisor_verifier.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8004 2024-05-09 07:05:50.000000 FlowVisor-0.1.5/flowvisor/function_node.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       98 2024-05-09 06:06:21.000000 FlowVisor-0.1.5/flowvisor/logger.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.1.5/flowvisor/sankey.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.1.5/flowvisor/time_tracker.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      292 2024-05-08 15:25:05.000000 FlowVisor-0.1.5/flowvisor/time_value.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.1.5/flowvisor/timer.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.1.5/flowvisor/utils.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-11 06:00:17.583484 FlowVisor-0.1.5/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.1.5/setup.py
```

### Comparing `FlowVisor-0.1.4/FlowVisor.egg-info/PKG-INFO` & `FlowVisor-0.1.5/FlowVisor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.4
+Version: 0.1.5
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.1.4/FlowVisor.egg-info/SOURCES.txt` & `FlowVisor-0.1.5/FlowVisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.4/LICENSE` & `FlowVisor-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.4/PKG-INFO` & `FlowVisor-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.1.4
+Version: 0.1.5
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.1.4/README.md` & `FlowVisor-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.4/flowvisor/cli/add_vis.py` & `FlowVisor-0.1.5/flowvisor/cli/add_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.4/flowvisor/cli/remove_vis.py` & `FlowVisor-0.1.5/flowvisor/cli/remove_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.4/flowvisor/cli/vis_file.py` & `FlowVisor-0.1.5/flowvisor/cli/vis_file.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.4/flowvisor/flowvisor.py` & `FlowVisor-0.1.5/flowvisor/flowvisor.py`

 * *Files 2% similar despite different names*

```diff
@@ -438,19 +438,33 @@
     def enable_dev_mode():
         """
         Enables the dev mode.
         """
         FlowVisor.CONFIG.dev_mode = True
 
     @staticmethod
-    def set_config(config: FlowVisorConfig):
+    def set_config(config: dict):
         """
         Sets the configuration.
         """
-        FlowVisor.CONFIG = config
+
+        FlowVisor.CONFIG = FlowVisorConfig.from_dict(config)
+
+    @staticmethod
+    def auto_verifier_mode(verifier_limit=10, file_name="flowvisor_verifier.json"):
+        """
+        Automatically enables the verifier mode.
+        """
+        count = FlowVisorVerifier.get_count_of_file(file_name)
+        if count < verifier_limit:
+            FlowVisor.enable_verifier_mode()
+            return
+        logger.log(
+            f"Verifier mode not enabled. Count of calls is {count} and the limit is {verifier_limit}"
+        )
 
     @staticmethod
     def enable_verifier_mode():
         """
         Enables the verifier mode.
         """
         FlowVisor.VERIFIER_MODE = True
```

### Comparing `FlowVisor-0.1.4/flowvisor/flowvisor_config.py` & `FlowVisor-0.1.5/flowvisor/flowvisor_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -53,7 +53,17 @@
             s += (
                 "Advanced Overhead reduction: "
                 + utils.get_time_as_string(self.advanced_overhead_reduction)
                 + "\n"
             )
         s += "Exclusive Time Mode: " + str(self.exclusive_time_mode) + "\n"
         return s
+
+    @staticmethod
+    def from_dict(config_dict: dict):
+        """
+        Create a FlowVisorConfig object from a dictionary
+        """
+        config = FlowVisorConfig()
+        for key in config_dict:
+            setattr(config, key, config_dict[key])
+        return config
```

### Comparing `FlowVisor-0.1.4/flowvisor/flowvisor_verifier.py` & `FlowVisor-0.1.5/flowvisor/flowvisor_verifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,48 +35,59 @@
         print(f"Function {func.__name__} took {time_str} seconds")
         return res
 
     return wrapper
 
 
 class FlowVisorVerifier:
+    """
+    FlowVisor verifier class
+    """
 
     ENTRIES = []
 
     @staticmethod
-    def add_entry(func, time: float):
+    def add_entry(func, time_value: float):
+        """
+        Add an entry to the verifier
+        """
         FlowVisorVerifier.ENTRIES.append(
-            {"id": utils.function_to_id(func), "time": time}
+            {"id": utils.function_to_id(func), "time": time_value}
         )
 
     @staticmethod
     def summaries_entries(entries):
+        """
+        Summarize the entries by adding the time of the same id
+        """
         new_entries = []
         for entry in entries:
             id_exists = False
             for new_entry in new_entries:
                 if new_entry["id"] == entry["id"]:
                     new_entry["time"] += entry["time"]
                     id_exists = True
                     break
             if not id_exists:
                 new_entries.append(entry)
         return new_entries
 
     @staticmethod
     def export(file_name: str):
-        file_name = utils.apply_file_end(file_name, "json")
+        """
+        Export the verifier entries to a file
+        """
         new_entries = FlowVisorVerifier.summaries_entries(FlowVisorVerifier.ENTRIES)
         device_name = utils.get_device_name()
         meta = {"device_name": device_name, "count": 0}
         old_data = None
 
-        if os.path.exists(file_name):
-            with open(file_name, "r", encoding="utf-8") as f:
-                existing_content = json.load(f)
+        existing_content = FlowVisorVerifier.read_existing_file(file_name)
+
+        if existing_content is not None:
             meta = existing_content["meta"]
             old_data = existing_content["data"]
             new_entries = FlowVisorVerifier.avarage_entries(
                 old_data, new_entries, meta["count"]
             )
 
         new_entries = FlowVisorVerifier.set_min_max(old_data, new_entries)
@@ -92,14 +103,17 @@
         }
 
         with open(file_name, "w", encoding="utf-8") as f:
             json.dump(content, f, indent=4)
 
     @staticmethod
     def avarage_entries(old_data, new_data, count):
+        """
+        Avergae the entries
+        """
         for entry in new_data:
             id_exists = False
             for old_entry in old_data:
                 if old_entry["id"] == entry["id"]:
                     old_entry["time"] = (old_entry["time"] * count + entry["time"]) / (
                         count + 1
                     )
@@ -108,14 +122,24 @@
             if not id_exists:
                 old_data.append(entry)
 
         return old_data
 
     @staticmethod
     def set_min_max(old_data, new_data):
+        """
+        Sets the min and max values for the entries
+
+        Args:
+            old_data (dict): The old data
+            new_data (dict): The new data
+
+        Returns:
+            dict: The new data with min and max values
+        """
         if old_data is None:
             for entry in new_data:
                 entry["min"] = entry["time"]
                 entry["max"] = entry["time"]
             return new_data
 
         for entry in new_data:
@@ -130,16 +154,15 @@
     def verify(nodes: List[FunctionNode], verify_file_name: str, threshold: float):
         verify_file_name = utils.apply_file_end(verify_file_name, "json")
 
         if not os.path.exists(verify_file_name):
             logger.log(f"Verify file {verify_file_name} not found...")
             return
 
-        with open(verify_file_name, "r", encoding="utf-8") as f:
-            content = json.load(f)
+        content = FlowVisorVerifier.read_existing_file(verify_file_name)
 
         is_verified = True
         device_name = content["meta"]["device_name"]
         if device_name != utils.get_device_name():
             logger.log(
                 f"🚨 WARNING 🚨 Verifier file is not clean: Wrong device {device_name}"
             )
@@ -176,12 +199,58 @@
             logger.log("All functions are verified! ✅")
         else:
             logger.log("Some functions are not verified! ❌")
         return is_verified
 
     @staticmethod
     def is_function_verified(entry, node_time, threshold):
+        max_value = entry["max"]
+        min_value = entry["min"]
         mean_time = entry["time"]
-        interval = entry["max"] - entry["min"]
-        offset = max(interval, mean_time * threshold)
+        interval = max_value - min_value
 
-        return mean_time - offset <= node_time and node_time <= mean_time + offset
+        offset_interval = interval * threshold
+        offset_meean = mean_time * threshold
+
+        if offset_interval > offset_meean:
+            return (
+                min_value - offset_interval <= node_time
+                and node_time <= max_value + offset_interval
+            )
+        return (
+            mean_time - offset_meean <= node_time
+            and node_time <= mean_time + offset_meean
+        )
+
+    @staticmethod
+    def read_existing_file(file_name: str):
+        """
+        Read the existing verifier file
+
+        Args:
+            file_name (str): The file name
+
+        Returns:
+            dict: The content of the file or None if the file does not exist
+        """
+        file_name = utils.apply_file_end(file_name, "json")
+        if not os.path.exists(file_name):
+            return None
+        with open(file_name, "r", encoding="utf-8") as f:
+            content = json.load(f)
+        return content
+
+    @staticmethod
+    def get_count_of_file(file_name: str):
+        """
+        Get the calls of a file
+
+        Args:
+            file_name (str): The file name
+
+        Returns:
+            int: The number of calls
+        """
+        content = FlowVisorVerifier.read_existing_file(file_name)
+        if content is None:
+            return 0
+        return content["meta"]["count"]
```

### Comparing `FlowVisor-0.1.4/flowvisor/function_node.py` & `FlowVisor-0.1.5/flowvisor/function_node.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.4/flowvisor/sankey.py` & `FlowVisor-0.1.5/flowvisor/sankey.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.4/flowvisor/time_tracker.py` & `FlowVisor-0.1.5/flowvisor/time_tracker.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.4/flowvisor/utils.py` & `FlowVisor-0.1.5/flowvisor/utils.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.1.4/setup.py` & `FlowVisor-0.1.5/setup.py`

 * *Files identical despite different names*

