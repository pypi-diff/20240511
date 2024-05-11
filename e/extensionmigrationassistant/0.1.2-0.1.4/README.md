# Comparing `tmp/extensionmigrationassistant-0.1.2-py3-none-any.whl.zip` & `tmp/extensionmigrationassistant-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 19043 bytes, number of entries: 11
+Zip file size: 19102 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat     6093 b- defN 24-May-09 11:06 assessment/SCTAssessmentReportTemplate.html
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-10 08:45 assessment/__init__.py
--rw-rw-rw-  2.0 fat    15867 b- defN 24-May-11 13:00 assessment/assessment.py
+-rw-rw-rw-  2.0 fat    16108 b- defN 24-May-11 16:06 assessment/assessment.py
 -rw-rw-rw-  2.0 fat    47417 b- defN 24-May-02 16:10 assessment/awssctcomplexitymatrix.csv
 -rw-rw-rw-  2.0 fat    25115 b- defN 24-May-08 10:59 assessment/sct_input.csv
--rw-rw-rw-  2.0 fat     1091 b- defN 24-May-11 13:01 extensionmigrationassistant-0.1.2.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     6356 b- defN 24-May-11 13:01 extensionmigrationassistant-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 13:01 extensionmigrationassistant-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       68 b- defN 24-May-11 13:01 extensionmigrationassistant-0.1.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       11 b- defN 24-May-11 13:01 extensionmigrationassistant-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1040 b- defN 24-May-11 13:01 extensionmigrationassistant-0.1.2.dist-info/RECORD
-11 files, 103150 bytes uncompressed, 17239 bytes compressed:  83.3%
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-May-11 16:07 extensionmigrationassistant-0.1.4.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     6356 b- defN 24-May-11 16:07 extensionmigrationassistant-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 16:07 extensionmigrationassistant-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       68 b- defN 24-May-11 16:07 extensionmigrationassistant-0.1.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       11 b- defN 24-May-11 16:07 extensionmigrationassistant-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1040 b- defN 24-May-11 16:07 extensionmigrationassistant-0.1.4.dist-info/RECORD
+11 files, 103391 bytes uncompressed, 17298 bytes compressed:  83.3%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: assessment/awssctcomplexitymatrix.csv
 Comment: 
 
 Filename: assessment/sct_input.csv
 Comment: 
 
-Filename: extensionmigrationassistant-0.1.2.dist-info/LICENSE.txt
+Filename: extensionmigrationassistant-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: extensionmigrationassistant-0.1.2.dist-info/METADATA
+Filename: extensionmigrationassistant-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: extensionmigrationassistant-0.1.2.dist-info/WHEEL
+Filename: extensionmigrationassistant-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: extensionmigrationassistant-0.1.2.dist-info/entry_points.txt
+Filename: extensionmigrationassistant-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: extensionmigrationassistant-0.1.2.dist-info/top_level.txt
+Filename: extensionmigrationassistant-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: extensionmigrationassistant-0.1.2.dist-info/RECORD
+Filename: extensionmigrationassistant-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## assessment/assessment.py

```diff
@@ -4,18 +4,20 @@
 from jinja2 import Environment, FileSystemLoader
 from matplotlib import pyplot as plt
 import os
 import shutil
 import argparse
 import numpy as np
 from argparse import RawTextHelpFormatter
+import pkg_resources
 
 def load_template():
     try:
-        env = Environment(loader=FileSystemLoader(r''))
+        template_path = pkg_resources.resource_filename(__name__, "")
+        env = Environment(loader=FileSystemLoader(template_path))
         template = env.get_template('SCTAssessmentReportTemplate.html')
         return template
     except Exception as e:
         print(f"{e}\nUnable to load SCTAssessmentReportTemplate.html")
 
 def connection_arguments():
     parser = argparse.ArgumentParser(description=r'Assess AWS Schema Conversion Tool Extensions dependencies and provide conversion efforts to native PostgreSQL.' , formatter_class=RawTextHelpFormatter)
@@ -34,16 +36,18 @@
         conn = engine.connect()
         return conn,args,parser
     except Exception as e:
         print(e)
 
 def read_data_from_csv():
     try:
-        data = pd.read_csv(os.path.join(r"sct_input.csv"))
-        aws_df = pd.read_csv(os.path.join(r"awssctcomplexitymatrix.csv"))
+        data_file_path = pkg_resources.resource_filename(__name__, 'sct_input.csv')
+        aws_file_path = pkg_resources.resource_filename(__name__, 'awssctcomplexitymatrix.csv')
+        data = pd.read_csv(data_file_path)
+        aws_df = pd.read_csv(aws_file_path)
         return data,aws_df
     except Exception as e:
         print(e)
     
 def output_dir(args, file_name):
     if args.outputpath:
         parent_directory = args.outputpath
@@ -327,15 +331,15 @@
             print(f"Extension Assesment Report zip file is created successfully")
         else:
             print("Unable to create Extension Assesment Report zip")
     else:
         print(fr"AWS SCT Extension Schema's(aws_%_ext) does not exists in database - {args.database}")
 
     
-    
+main()
```

## Comparing `extensionmigrationassistant-0.1.2.dist-info/LICENSE.txt` & `extensionmigrationassistant-0.1.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `extensionmigrationassistant-0.1.2.dist-info/METADATA` & `extensionmigrationassistant-0.1.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extensionmigrationassistant
-Version: 0.1.2
+Version: 0.1.4
 Summary: Description of your package
 Home-page: https://github.com/dcgadmin/extensionmigrationassistant.git
 Author: DataCloudGaze
 Author-email: contact@datacloudgaze.com
 License: MIT License
         
         Copyright (c) 2023 DataCloudGaze
```

