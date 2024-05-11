# Comparing `tmp/splicon-1.0.1.tar.gz` & `tmp/splicon-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splicon-1.0.1.tar", last modified: Wed May  1 16:38:48 2024, max compression
+gzip compressed data, was "splicon-1.0.2.tar", last modified: Sat May 11 09:32:45 2024, max compression
```

## Comparing `splicon-1.0.1.tar` & `splicon-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sschimper  (1000) sschimper  (1000)        0 2024-05-01 16:38:48.750089 splicon-1.0.1/
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1308 2024-05-01 16:38:48.750089 splicon-1.0.1/PKG-INFO
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)      715 2024-05-01 16:35:31.000000 splicon-1.0.1/README.md
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       38 2024-05-01 16:38:48.750089 splicon-1.0.1/setup.cfg
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1396 2024-05-01 16:37:23.000000 splicon-1.0.1/setup.py
-drwxrwxr-x   0 sschimper  (1000) sschimper  (1000)        0 2024-05-01 16:38:48.750089 splicon-1.0.1/splicon/
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)        0 2024-05-01 11:50:51.000000 splicon-1.0.1/splicon/__init__.py
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1564 2024-05-01 16:37:37.000000 splicon-1.0.1/splicon/splicon.py
-drwxrwxr-x   0 sschimper  (1000) sschimper  (1000)        0 2024-05-01 16:38:48.750089 splicon-1.0.1/splicon.egg-info/
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1308 2024-05-01 16:38:48.000000 splicon-1.0.1/splicon.egg-info/PKG-INFO
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)      245 2024-05-01 16:38:48.000000 splicon-1.0.1/splicon.egg-info/SOURCES.txt
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)        1 2024-05-01 16:38:48.000000 splicon-1.0.1/splicon.egg-info/dependency_links.txt
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       65 2024-05-01 16:38:48.000000 splicon-1.0.1/splicon.egg-info/entry_points.txt
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       16 2024-05-01 16:38:48.000000 splicon-1.0.1/splicon.egg-info/requires.txt
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)        8 2024-05-01 16:38:48.000000 splicon-1.0.1/splicon.egg-info/top_level.txt
+drwxrwxr-x   0 sschimper  (1000) sschimper  (1000)        0 2024-05-11 09:32:45.041095 splicon-1.0.2/
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1335 2024-05-11 09:32:45.041095 splicon-1.0.2/PKG-INFO
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)      742 2024-05-11 09:30:31.000000 splicon-1.0.2/README.md
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       38 2024-05-11 09:32:45.041095 splicon-1.0.2/setup.cfg
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1396 2024-05-11 09:31:20.000000 splicon-1.0.2/setup.py
+drwxrwxr-x   0 sschimper  (1000) sschimper  (1000)        0 2024-05-11 09:32:45.041095 splicon-1.0.2/splicon/
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)        0 2024-05-01 11:50:51.000000 splicon-1.0.2/splicon/__init__.py
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1564 2024-05-11 09:31:27.000000 splicon-1.0.2/splicon/splicon.py
+drwxrwxr-x   0 sschimper  (1000) sschimper  (1000)        0 2024-05-11 09:32:45.041095 splicon-1.0.2/splicon.egg-info/
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1335 2024-05-11 09:32:45.000000 splicon-1.0.2/splicon.egg-info/PKG-INFO
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)      245 2024-05-11 09:32:45.000000 splicon-1.0.2/splicon.egg-info/SOURCES.txt
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)        1 2024-05-11 09:32:45.000000 splicon-1.0.2/splicon.egg-info/dependency_links.txt
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       65 2024-05-11 09:32:45.000000 splicon-1.0.2/splicon.egg-info/entry_points.txt
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       16 2024-05-11 09:32:45.000000 splicon-1.0.2/splicon.egg-info/requires.txt
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)        8 2024-05-11 09:32:45.000000 splicon-1.0.2/splicon.egg-info/top_level.txt
```

### Comparing `splicon-1.0.1/PKG-INFO` & `splicon-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splicon
-Version: 1.0.1
+Version: 1.0.2
 Summary: Create Splunk icons for App/Add-On Development
 Home-page: UNKNOWN
 Author: Sebastian Schimper
 Author-email: sebastianschimper@gmail.com
 License: UNKNOWN
 Keywords: python,splunk,icon,development
 Platform: UNKNOWN
@@ -21,15 +21,17 @@
 
 Creates icons to be used for developing Splunk apps and add-ons via resizing a provided image.
 More information about Splunk"s required image sizes can be found here:
 https://dev.splunk.com/enterprise/docs/developapps/createapps#Add-icons-to-your-app
 
 ## Installation
 
-// todo
+```console
+pip install splicon
+```
 
 ## Usage
 
 ```console
 splicon [-h] [-d DESTINATION] [-v] filename
 ```
```

### Comparing `splicon-1.0.1/setup.py` & `splicon-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DESCRIPTION = "Create Splunk icons for App/Add-On Development"
 LONG_DESCRIPTION = """
 Creates icons to be used for developing Splunk apps and add-ons via resizing a provided image.\n
 More information about Splunk"s required image sizes can be found here:\n
 https://dev.splunk.com/enterprise/docs/developapps/createapps#Add-icons-to-your-app
 """
```

### Comparing `splicon-1.0.1/splicon/splicon.py` & `splicon-1.0.2/splicon/splicon.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
                         More information about Splunk"s required image sizes can be found here:\n
                         https://dev.splunk.com/enterprise/docs/developapps/createapps#Add-icons-to-your-app
                         """
     )
 
     parser.add_argument("filename", help="Image file from which the Splunk icons are generated.")           
     parser.add_argument("-d", "--destination", help="Directory/Folder for storing the processed icons.")
-    parser.add_argument("-v", "--version", action="version", version="1.0.1", help="Prints the version.")
+    parser.add_argument("-v", "--version", action="version", version="1.0.2", help="Prints the version.")
     args = parser.parse_args()
 
     output_directory = "."
     if (args.destination):
         output_directory = args.destination
 
     with Image.open(args.filename) as im:
```

### Comparing `splicon-1.0.1/splicon.egg-info/PKG-INFO` & `splicon-1.0.2/splicon.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splicon
-Version: 1.0.1
+Version: 1.0.2
 Summary: Create Splunk icons for App/Add-On Development
 Home-page: UNKNOWN
 Author: Sebastian Schimper
 Author-email: sebastianschimper@gmail.com
 License: UNKNOWN
 Keywords: python,splunk,icon,development
 Platform: UNKNOWN
@@ -21,15 +21,17 @@
 
 Creates icons to be used for developing Splunk apps and add-ons via resizing a provided image.
 More information about Splunk"s required image sizes can be found here:
 https://dev.splunk.com/enterprise/docs/developapps/createapps#Add-icons-to-your-app
 
 ## Installation
 
-// todo
+```console
+pip install splicon
+```
 
 ## Usage
 
 ```console
 splicon [-h] [-d DESTINATION] [-v] filename
 ```
```

