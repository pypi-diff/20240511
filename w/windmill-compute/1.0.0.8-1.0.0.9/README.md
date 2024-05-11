# Comparing `tmp/windmill_compute-1.0.0.8-py3-none-any.whl.zip` & `tmp/windmill_compute-1.0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8543 bytes, number of entries: 11
--rw-r--r--  2.0 unx      213 b- defN 24-Mar-22 07:47 windmillcomputev1/__init__.py
--rw-r--r--  2.0 unx      213 b- defN 24-Mar-18 09:40 windmillcomputev1/client/__init__.py
--rw-r--r--  2.0 unx      905 b- defN 24-Mar-18 09:40 windmillcomputev1/client/compute_api_compute.py
--rw-r--r--  2.0 unx    11261 b- defN 24-Mar-19 09:10 windmillcomputev1/client/compute_client.py
+Zip file size: 8616 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      213 b- defN 24-Mar-22 08:45 windmillcomputev1/__init__.py
+-rw-r--r--  2.0 unx      213 b- defN 24-Mar-22 07:47 windmillcomputev1/client/__init__.py
+-rw-r--r--  2.0 unx      905 b- defN 24-Mar-22 07:47 windmillcomputev1/client/compute_api_compute.py
+-rw-r--r--  2.0 unx    11693 b- defN 24-Mar-22 08:33 windmillcomputev1/client/compute_client.py
 -rw-r--r--  2.0 unx     2085 b- defN 24-Mar-22 07:46 windmillcomputev1/filesystem/__init__.py
 -rw-r--r--  2.0 unx     1774 b- defN 24-Mar-22 07:46 windmillcomputev1/filesystem/blobstore.py
 -rw-r--r--  2.0 unx     4410 b- defN 24-Mar-22 07:46 windmillcomputev1/filesystem/s3.py
--rw-r--r--  2.0 unx      682 b- defN 24-Mar-22 07:47 windmill_compute-1.0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-22 07:47 windmill_compute-1.0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-Mar-22 07:47 windmill_compute-1.0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1007 b- defN 24-Mar-22 07:47 windmill_compute-1.0.0.8.dist-info/RECORD
-11 files, 22660 bytes uncompressed, 6803 bytes compressed:  70.0%
+-rw-r--r--  2.0 unx      682 b- defN 24-Mar-22 08:45 windmill_compute-1.0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-22 08:45 windmill_compute-1.0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-Mar-22 08:45 windmill_compute-1.0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1007 b- defN 24-Mar-22 08:45 windmill_compute-1.0.0.9.dist-info/RECORD
+11 files, 23092 bytes uncompressed, 6876 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: windmillcomputev1/filesystem/blobstore.py
 Comment: 
 
 Filename: windmillcomputev1/filesystem/s3.py
 Comment: 
 
-Filename: windmill_compute-1.0.0.8.dist-info/METADATA
+Filename: windmill_compute-1.0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: windmill_compute-1.0.0.8.dist-info/WHEEL
+Filename: windmill_compute-1.0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: windmill_compute-1.0.0.8.dist-info/top_level.txt
+Filename: windmill_compute-1.0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: windmill_compute-1.0.0.8.dist-info/RECORD
+Filename: windmill_compute-1.0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## windmillcomputev1/client/compute_client.py

```diff
@@ -234,24 +234,34 @@
         return blobstore(*blobstore_config(filesystem=filesystem))
 
     @staticmethod
     def _first(values: List):
         assert len(values) > 0, "empty list"
         return values[0]
 
-    def list_flavour(self):
+    def list_flavour(self,
+                     cluster_name: Optional[str] = "",
+                     name: Optional[str] = "",
+                     marker: Optional[str] = "",
+                     max_keys: Optional[str] = ""):
         """
         list_flavour
         Args:
 
         Returns:
             http request response
         """
+        params = {"name": name,
+                  "marker": marker,
+                  "maxKeys": max_keys}
+        if cluster_name:
+            params["clusterName"] = cluster_name
         return self._send_request(http_method=http_methods.GET,
-                                  path=bytes("/v1/flavours", encoding="utf-8"))
+                                  path=bytes("/v1/flavours", encoding="utf-8"),
+                                  params=params)
 
     def get_flavour(self, local_name: str):
         """
         Gets compute object from specified workspace.
         :param local_name:
         :return:
         """
```

## Comparing `windmill_compute-1.0.0.8.dist-info/METADATA` & `windmill_compute-1.0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-compute
-Version: 1.0.0.8
+Version: 1.0.0.9
 Summary: sdk in python for windmill compute
 Home-page: https://console.cloud.baidu-int.com/devops/icode/repos/baidu/themis/windmill-compute/tree/master
 Author: yangtingyu01
 Author-email: yangtingyu01@baidu.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `windmill_compute-1.0.0.8.dist-info/RECORD` & `windmill_compute-1.0.0.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 windmillcomputev1/__init__.py,sha256=f2GyH-DYr84jGbwxEiy24uBoFe9W7sujdenZ-oj1yUs,213
 windmillcomputev1/client/__init__.py,sha256=f2GyH-DYr84jGbwxEiy24uBoFe9W7sujdenZ-oj1yUs,213
 windmillcomputev1/client/compute_api_compute.py,sha256=qErlgtJr5br649GZppsQ3EaLYQNbWCV16F_lZB4PUBU,905
-windmillcomputev1/client/compute_client.py,sha256=HK143HRy4nfN-5TA5TaSpn2AJODo2ecyB_xp8y21nxo,11261
+windmillcomputev1/client/compute_client.py,sha256=mcLi3M9vAEG_9TVcO5WP3-E43L2HiLkFMAuTz5UyrRs,11693
 windmillcomputev1/filesystem/__init__.py,sha256=fdDfm4MRbaEOEIQBu-xeZZ44cQfPgUTqS3VxRQJOF6k,2085
 windmillcomputev1/filesystem/blobstore.py,sha256=2VAQzJjqsrCjC8Sf1uX2zgNRO5_cDQBtAsSLkT7AoWg,1774
 windmillcomputev1/filesystem/s3.py,sha256=g1pwBIbk1-tdtTcOo_XGYPgKLgzSHEXwOhH354ejx48,4410
-windmill_compute-1.0.0.8.dist-info/METADATA,sha256=oNM0Z-WvJyoFbuBEE0S5SbQEL7iSg76pU_Leuup7o9k,682
-windmill_compute-1.0.0.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-windmill_compute-1.0.0.8.dist-info/top_level.txt,sha256=9oI_GzShN98tsziMo0Zs39Q6PYtnfmEQh1Auj9y16KA,18
-windmill_compute-1.0.0.8.dist-info/RECORD,,
+windmill_compute-1.0.0.9.dist-info/METADATA,sha256=4J45L9L4zw7bnqZjMAI-3ODZ7gVk7NNfmu8qZFa_jjk,682
+windmill_compute-1.0.0.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+windmill_compute-1.0.0.9.dist-info/top_level.txt,sha256=9oI_GzShN98tsziMo0Zs39Q6PYtnfmEQh1Auj9y16KA,18
+windmill_compute-1.0.0.9.dist-info/RECORD,,
```

