# Comparing `tmp/gcp_pal-1.0.8.tar.gz` & `tmp/gcp_pal-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_pal-1.0.8.tar", max compression
+gzip compressed data, was "gcp_pal-1.0.9.tar", max compression
```

## Comparing `gcp_pal-1.0.8.tar` & `gcp_pal-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    28062 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/README.md
--rw-r--r--   0        0        0      865 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/__init__.py
--rw-r--r--   0        0        0    31457 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/bigquery.py
--rw-r--r--   0        0        0    13156 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/cloudfunctions.py
--rw-r--r--   0        0        0    13920 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/cloudrun.py
--rw-r--r--   0        0        0     7754 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/cloudscheduler.py
--rw-r--r--   0        0        0       42 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/config/__init__.py
--rw-r--r--   0        0        0     1094 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/config/vars.py
--rw-r--r--   0        0        0    26783 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/dataplex.py
--rw-r--r--   0        0        0    12490 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/firestore.py
--rw-r--r--   0        0        0     3170 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/project.py
--rw-r--r--   0        0        0     1674 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/pubsub.py
--rw-r--r--   0        0        0     3873 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/pydocker.py
--rw-r--r--   0        0        0     6975 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/pylogging.py
--rw-r--r--   0        0        0     4737 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/request.py
--rw-r--r--   0        0        0    23631 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/schema.py
--rw-r--r--   0        0        0     6332 2024-04-30 10:30:09.059612 gcp_pal-1.0.8/gcp_pal/secretmanager.py
--rw-r--r--   0        0        0       88 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/gcp_pal/storage/__init__.py
--rw-r--r--   0        0        0     8735 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/gcp_pal/storage/parquet.py
--rw-r--r--   0        0        0    17224 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/gcp_pal/storage/storage.py
--rw-r--r--   0        0        0       82 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/gcp_pal/utils/__init__.py
--rw-r--r--   0        0        0      935 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/gcp_pal/utils/lazy_loader.py
--rw-r--r--   0        0        0    11431 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/gcp_pal/utils/utils.py
--rw-r--r--   0        0        0     1051 2024-04-30 10:30:09.063612 gcp_pal-1.0.8/pyproject.toml
--rw-r--r--   0        0        0    28511 1970-01-01 00:00:00.000000 gcp_pal-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    28062 2024-04-30 15:29:07.779518 gcp_pal-1.0.9/README.md
+-rw-r--r--   0        0        0      865 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/__init__.py
+-rw-r--r--   0        0        0    31457 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/bigquery.py
+-rw-r--r--   0        0        0    13156 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/cloudfunctions.py
+-rw-r--r--   0        0        0    13920 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/cloudrun.py
+-rw-r--r--   0        0        0     7754 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/cloudscheduler.py
+-rw-r--r--   0        0        0       42 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/config/__init__.py
+-rw-r--r--   0        0        0     1094 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/config/vars.py
+-rw-r--r--   0        0        0    29002 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/dataplex.py
+-rw-r--r--   0        0        0    12490 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/firestore.py
+-rw-r--r--   0        0        0     3170 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/project.py
+-rw-r--r--   0        0        0     1674 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/pubsub.py
+-rw-r--r--   0        0        0     3873 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/pydocker.py
+-rw-r--r--   0        0        0     6975 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/pylogging.py
+-rw-r--r--   0        0        0     4737 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/request.py
+-rw-r--r--   0        0        0    23631 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/schema.py
+-rw-r--r--   0        0        0     6332 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/secretmanager.py
+-rw-r--r--   0        0        0       88 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/storage/__init__.py
+-rw-r--r--   0        0        0     8735 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/storage/parquet.py
+-rw-r--r--   0        0        0    17224 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/storage/storage.py
+-rw-r--r--   0        0        0       82 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/utils/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/utils/lazy_loader.py
+-rw-r--r--   0        0        0    11431 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/gcp_pal/utils/utils.py
+-rw-r--r--   0        0        0     1051 2024-04-30 15:29:07.783518 gcp_pal-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0    28511 1970-01-01 00:00:00.000000 gcp_pal-1.0.9/PKG-INFO
```

### Comparing `gcp_pal-1.0.8/README.md` & `gcp_pal-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/__init__.py` & `gcp_pal-1.0.9/gcp_pal/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/bigquery.py` & `gcp_pal-1.0.9/gcp_pal/bigquery.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/cloudfunctions.py` & `gcp_pal-1.0.9/gcp_pal/cloudfunctions.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/cloudrun.py` & `gcp_pal-1.0.9/gcp_pal/cloudrun.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/cloudscheduler.py` & `gcp_pal-1.0.9/gcp_pal/cloudscheduler.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/config/vars.py` & `gcp_pal-1.0.9/gcp_pal/config/vars.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/dataplex.py` & `gcp_pal-1.0.9/gcp_pal/dataplex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import threading
 from gcp_pal.utils import try_import
 
 try_import("google.cloud.dataplex_v1", "Dataplex")
 try_import("google.api_core.exceptions", "Dataplex")
 import google.api_core.exceptions
 from google.cloud.dataplex_v1 import DataplexServiceClient
 from google.cloud.dataplex_v1.types import Lake, Zone, Asset
@@ -628,14 +629,17 @@
             msg = (
                 f"Dataplex - Lake '{self.lake}' is not empty. Deleting all its zones..."
             )
             log(msg)
             lake = Dataplex(
                 lake=self.lake, project=self.project, location=self.location
             )
+            lake_assets = lake.ls_assets(full_id=True)
+            for asset in lake_assets:
+                Dataplex(path=asset).delete()
             zones = lake.ls_zones(full_id=True)
             for zone in zones:
                 Dataplex(path=zone).delete()
             self._refresh_client()
             output = self.client.delete_lake(name=name)
         except google.api_core.exceptions.NotFound as e:
             if errors == "ignore":
@@ -655,31 +659,35 @@
         Args:
         - name (str): The full resource ID of the zone.
 
         Returns:
         - (dict): The response of the delete operation.
         """
         name = name or f"{self.parent}/zones/{self.zone}"
+        log(f"Dataplex - Deleting zone: '{self.path}'...")
         try:
             output = self.client.delete_zone(name=name)
         except google.api_core.exceptions.FailedPrecondition as e:
             msg = f"Dataplex - Zone '{self.path}' is not empty. Deleting all its assets..."
             log(msg)
-            assets = self.ls_assets(name=name, full_id=True)
-            for asset in assets:
-                Dataplex(path=asset).delete()
+            zone = Dataplex(
+                lake=self.lake,
+                zone=self.zone,
+                project=self.project,
+                location=self.location,
+            )
+            self._delete_parallel(zone.ls_assets(full_id=True))
             self._refresh_client()
             output = self.client.delete_zone(name=name)
         except google.api_core.exceptions.NotFound as e:
             if errors == "ignore":
                 log(f"Dataplex - Zone '{self.path}' does not exist to delete.")
                 return
             raise e
         if wait_to_complete:
-            log(f"Dataplex - Waiting for zone deletion...")
             output = output.result(timeout=600)
         log(f"Dataplex - Zone deleted: '{self.path}'.")
         return output
 
     def delete_asset(self, name: str = None, errors="ignore", wait_to_complete=True):
         """
         Deletes the asset resource.
@@ -688,27 +696,84 @@
         - name (str): The full resource ID of the asset.
         - wait_to_complete (bool): If True, waits until the operation is completed.
 
         Returns:
         - (dict): The response of the delete operation.
         """
         name = name or f"{self.parent}/assets/{self.asset}"
+        log(f"Dataplex - Deleting asset: '{self.path}'...")
         try:
             output = self.client.delete_asset(name=name)
         except google.api_core.exceptions.NotFound as e:
             if errors == "ignore":
                 log(f"Dataplex - Asset '{self.path}' does not exist to delete.")
                 return
             raise e
         if wait_to_complete:
-            log(f"Dataplex - Waiting for asset deletion...")
             output = output.result(timeout=600)
         log(f"Dataplex - Asset deleted: '{self.path}'.")
         return output
 
+    def delete_lake(self, name: str = None, errors="ignore", wait_to_complete=True):
+        """
+        Deletes the lake resource using parallel deletion for assets and zones.
+
+        Args:
+        - name (str): The full resource ID of the lake.
+
+        Returns:
+        - (dict): The response of the delete operation.
+        """
+        name = name or f"{self.parent}/lakes/{self.lake}"
+        try:
+            output = self.client.delete_lake(name=name)
+        except google.api_core.exceptions.FailedPrecondition:
+            log(
+                f"Dataplex - Lake '{self.lake}' is not empty. Deleting all its zones and assets..."
+            )
+            lake = Dataplex(
+                lake=self.lake, project=self.project, location=self.location
+            )
+
+            # Deleting all assets in all zones in the lake
+            self._delete_parallel(lake.ls_assets(full_id=True))
+
+            # Deleting zones in the lake
+            self._delete_parallel(lake.ls_zones(full_id=True))
+
+            self._refresh_client()
+            output = self.client.delete_lake(name=name)
+        except google.api_core.exceptions.NotFound:
+            if errors == "ignore":
+                log(f"Dataplex - Lake '{self.lake}' does not exist to delete.")
+                return
+            raise
+        if wait_to_complete:
+            log(f"Dataplex - Waiting for the lake deletion...")
+            output = output.result(timeout=600)
+        log(f"Dataplex - Lake deleted: '{self.lake}'.")
+        return output
+
+    def _delete_parallel(self, items):
+        """
+        Deletes items in parallel using threading.
+
+        Args:
+        - items (list): List of full resource IDs of assets or zones to delete.
+        """
+        threads = []
+        for item in items:
+            thread = threading.Thread(
+                target=lambda item=item: Dataplex(path=item).delete()
+            )
+            thread.start()
+            threads.append(thread)
+        for thread in threads:
+            thread.join()
+
     def delete(self, name: str = None, errors="ignore", wait_to_complete=True):
         """
         Deletes the resource.
 
         Args:
         - name (str): The full resource ID of the resource.
         - errors (str): If "ignore", the operation will be ignored if the resource does not exist.
@@ -728,31 +793,29 @@
         return output
 
 
 if __name__ == "__main__":
     # Example: Create a Dataplex object
     from gcp_pal import BigQuery
 
-    print(Dataplex().ls(level="assets", full_id=False))
-
-    # lake_name = "artem-lake3"
-    # zone_name = "artem-zone3"
+    lake_name = "artem-lake1"
+    zone_name = "artem-zone1"
     # Dataplex(path=lake_name).create_lake()
     # Dataplex(path=f"{lake_name}/{zone_name}").create_zone(
     #     zone_type="raw", location_type="single-region"
     # )
-    # # BigQuery(dataset="dataplex_dataset1").create()
-    # # BigQuery(dataset="dataplex_dataset2").create()
+    # BigQuery(dataset="dataplex_dataset1").create()
+    # BigQuery(dataset="dataplex_dataset2").create()
     # Dataplex(
     #     path=f"{lake_name}/{zone_name}/test-asset1",
     # ).create_asset(
     #     asset_source="dataplex_dataset1",
     #     asset_type="bigquery",
     # )
     # Dataplex(
     #     path=f"{lake_name}/{zone_name}/test-asset2",
     # ).create_asset(
     #     asset_source="dataplex_dataset2",
     #     asset_type="bigquery",
     # )
 
-    # Dataplex(lake_name, location="europe-west2").delete()
+    Dataplex(lake_name, location="europe-west2").delete()
```

### Comparing `gcp_pal-1.0.8/gcp_pal/firestore.py` & `gcp_pal-1.0.9/gcp_pal/firestore.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/project.py` & `gcp_pal-1.0.9/gcp_pal/project.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/pubsub.py` & `gcp_pal-1.0.9/gcp_pal/pubsub.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/pydocker.py` & `gcp_pal-1.0.9/gcp_pal/pydocker.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/pylogging.py` & `gcp_pal-1.0.9/gcp_pal/pylogging.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/request.py` & `gcp_pal-1.0.9/gcp_pal/request.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/schema.py` & `gcp_pal-1.0.9/gcp_pal/schema.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/secretmanager.py` & `gcp_pal-1.0.9/gcp_pal/secretmanager.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/storage/parquet.py` & `gcp_pal-1.0.9/gcp_pal/storage/parquet.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/storage/storage.py` & `gcp_pal-1.0.9/gcp_pal/storage/storage.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/utils/lazy_loader.py` & `gcp_pal-1.0.9/gcp_pal/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/gcp_pal/utils/utils.py` & `gcp_pal-1.0.9/gcp_pal/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.8/pyproject.toml` & `gcp_pal-1.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcp-pal"
-version = "1.0.8"
+version = "1.0.9"
 description = "Set of utilities for interacting with Google Cloud Platform"
 authors = ["VitaminB16 <artemiy.nosov@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gcp_pal-1.0.8/PKG-INFO` & `gcp_pal-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-pal
-Version: 1.0.8
+Version: 1.0.9
 Summary: Set of utilities for interacting with Google Cloud Platform
 Author: VitaminB16
 Author-email: artemiy.nosov@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

