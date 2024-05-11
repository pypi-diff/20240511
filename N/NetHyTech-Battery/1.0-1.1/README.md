# Comparing `tmp/NetHyTech_Battery-1.0-py3-none-any.whl.zip` & `tmp/NetHyTech_Battery-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 14981 bytes, number of entries: 6
+Zip file size: 14982 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat    62182 b- defN 24-May-05 17:54 NetHyTech_Battery/DLG.py
 -rw-rw-rw-  2.0 fat     1296 b- defN 24-May-11 05:03 NetHyTech_Battery/__init__.py
--rw-rw-rw-  2.0 fat     1928 b- defN 24-May-11 05:14 NetHyTech_Battery-1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 05:14 NetHyTech_Battery-1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 24-May-11 05:14 NetHyTech_Battery-1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      498 b- defN 24-May-11 05:14 NetHyTech_Battery-1.0.dist-info/RECORD
-6 files, 66014 bytes uncompressed, 14077 bytes compressed:  78.7%
+-rw-rw-rw-  2.0 fat     1951 b- defN 24-May-11 07:38 NetHyTech_Battery-1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 07:38 NetHyTech_Battery-1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 24-May-11 07:38 NetHyTech_Battery-1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      498 b- defN 24-May-11 07:38 NetHyTech_Battery-1.1.dist-info/RECORD
+6 files, 66037 bytes uncompressed, 14078 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: NetHyTech_Battery/DLG.py
 Comment: 
 
 Filename: NetHyTech_Battery/__init__.py
 Comment: 
 
-Filename: NetHyTech_Battery-1.0.dist-info/METADATA
+Filename: NetHyTech_Battery-1.1.dist-info/METADATA
 Comment: 
 
-Filename: NetHyTech_Battery-1.0.dist-info/WHEEL
+Filename: NetHyTech_Battery-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: NetHyTech_Battery-1.0.dist-info/top_level.txt
+Filename: NetHyTech_Battery-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: NetHyTech_Battery-1.0.dist-info/RECORD
+Filename: NetHyTech_Battery-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `NetHyTech_Battery-1.0.dist-info/METADATA` & `NetHyTech_Battery-1.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: NetHyTech-Battery
-Version: 1.0
+Version: 1.1
 Summary: Package for Battery Functions
 Home-page: https://github.com/AnubhavChaturvedi-GitHub/NetHyTech-Battery
 Author: Anubhav Chaturvedi
 Author-email: chaturvedianubhav520@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: psttil
+Requires-Dist: random
 
 
 # NetHyTech-Battery
 
 NetHyTech-Battery is a Python package that provides functionalities for monitoring battery status and generating alerts based on battery percentage and power plug status.
 
 ## Installation
```

