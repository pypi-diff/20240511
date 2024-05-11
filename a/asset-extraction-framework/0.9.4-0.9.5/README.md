# Comparing `tmp/asset_extraction_framework-0.9.4.tar.gz` & `tmp/asset_extraction_framework-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asset_extraction_framework-0.9.4.tar", last modified: Sat Jan  6 20:34:11 2024, max compression
+gzip compressed data, was "asset_extraction_framework-0.9.5.tar", last modified: Wed Jan 10 23:43:29 2024, max compression
```

## Comparing `asset_extraction_framework-0.9.4.tar` & `asset_extraction_framework-0.9.5.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 20:34:11.860756 asset_extraction_framework-0.9.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 20:34:11.852756 asset_extraction_framework-0.9.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 20:34:11.856756 asset_extraction_framework-0.9.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)    38874 2024-01-06 20:34:11.860756 asset_extraction_framework-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 20:34:11.856756 asset_extraction_framework-0.9.4/asset_extraction_framework/
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/asset_extraction_framework/Application.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/asset_extraction_framework/Asserts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 20:34:11.856756 asset_extraction_framework-0.9.4/asset_extraction_framework/Asset/
--rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/asset_extraction_framework/Asset/Animation.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/asset_extraction_framework/Asset/Asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/asset_extraction_framework/Asset/BoundingBox.py
--rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/asset_extraction_framework/Asset/Image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/asset_extraction_framework/Asset/Palette.py
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/asset_extraction_framework/Asset/Sound.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/asset_extraction_framework/Asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/asset_extraction_framework/CommandLine.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4813 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/asset_extraction_framework/File.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/asset_extraction_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 20:34:11.856756 asset_extraction_framework-0.9.4/asset_extraction_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    38874 2024-01-06 20:34:11.000000 asset_extraction_framework-0.9.4/asset_extraction_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-01-06 20:34:11.000000 asset_extraction_framework-0.9.4/asset_extraction_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 20:34:11.000000 asset_extraction_framework-0.9.4/asset_extraction_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-06 20:34:11.000000 asset_extraction_framework-0.9.4/asset_extraction_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-06 20:34:11.000000 asset_extraction_framework-0.9.4/asset_extraction_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 20:34:11.860756 asset_extraction_framework-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-06 20:34:03.000000 asset_extraction_framework-0.9.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:43:29.868603 asset_extraction_framework-0.9.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:43:29.864603 asset_extraction_framework-0.9.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:43:29.864603 asset_extraction_framework-0.9.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)    38903 2024-01-10 23:43:29.868603 asset_extraction_framework-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:43:29.868603 asset_extraction_framework-0.9.5/asset_extraction_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/asset_extraction_framework/Application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/asset_extraction_framework/Asserts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:43:29.868603 asset_extraction_framework-0.9.5/asset_extraction_framework/Asset/
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/asset_extraction_framework/Asset/Animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/asset_extraction_framework/Asset/Asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/asset_extraction_framework/Asset/BoundingBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/asset_extraction_framework/Asset/Image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/asset_extraction_framework/Asset/Palette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/asset_extraction_framework/Asset/Sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/asset_extraction_framework/Asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/asset_extraction_framework/CommandLine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/asset_extraction_framework/Exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4813 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/asset_extraction_framework/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/asset_extraction_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 23:43:29.868603 asset_extraction_framework-0.9.5/asset_extraction_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    38903 2024-01-10 23:43:29.000000 asset_extraction_framework-0.9.5/asset_extraction_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-01-10 23:43:29.000000 asset_extraction_framework-0.9.5/asset_extraction_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 23:43:29.000000 asset_extraction_framework-0.9.5/asset_extraction_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-10 23:43:29.000000 asset_extraction_framework-0.9.5/asset_extraction_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-10 23:43:29.000000 asset_extraction_framework-0.9.5/asset_extraction_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 23:43:29.868603 asset_extraction_framework-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-10 23:43:21.000000 asset_extraction_framework-0.9.5/tox.ini
```

### Comparing `asset_extraction_framework-0.9.4/.github/workflows/publish-to-pypi.yml` & `asset_extraction_framework-0.9.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.4/.github/workflows/run-tox.yml` & `asset_extraction_framework-0.9.5/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.4/.gitignore` & `asset_extraction_framework-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.4/COPYING` & `asset_extraction_framework-0.9.5/COPYING`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.4/PKG-INFO` & `asset_extraction_framework-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset_extraction_framework
-Version: 0.9.4
+Version: 0.9.5
 Summary: Toolkit to help extract multimedia assets from legacy software
 Author: npjg
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -633,14 +633,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: Pillow>=9.2.0
 Requires-Dist: numpy>=1.23.0
 Requires-Dist: jsons>=1.6.2
+Requires-Dist: hexdump2>=1.1
 
 `assets` is a reverse-engineering framework for extracting multimedia assets from legacy software.
 
 Unlike [`mrcrowbar`](https://github.com/moralrecordings/mrcrowbar) and other reverse-engineering packages, 
 this library is not designed for editing data in-place. `assets` instead focuses on extraction. 
 
 You write the code that converts the data from your application into a standard format (pixels and PCM audio).
```

### Comparing `asset_extraction_framework-0.9.4/README.md` & `asset_extraction_framework-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.4/asset_extraction_framework/Application.py` & `asset_extraction_framework-0.9.5/asset_extraction_framework/Application.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,22 @@
 from PIL import Image
 from PIL import ImagePalette
 import mmap
 
 ## Uses regular expressions to link the filenames of application files,
 ## as defined by regular expressions, to file parser classes in this application.
 class FileDetectionEntry:
-    def __init__(self, filename_regex: str, case_sensitive: bool, file_processor):
+    def __init__(self, filename_regex: str, case_sensitive: bool, file_processor, filename_sorting_algorithm = sorted):
         self.filename_regex = filename_regex
         self.case_sensitive = case_sensitive
         self.file_processor = file_processor
+        # When enumerating files in a directory, filename order cannot be relied upon 
+        # and is an artifact of the filesystem. So this allows you to define a custom
+        # sorting algorithm.
+        self.filename_sorting_algorithm = filename_sorting_algorithm
 
 ## Represents an application whose assets we wish to export.
 ## An application contains a collection of files, which each
 ## contain a collection of assets.
 class Application:
     def __init__(self, application_name: str):
         # CREATE A PLACE TO STORE THE FILES.
@@ -43,15 +47,20 @@
 
             for path in paths:
                 # CHECK IF THE PATH IS A DIRECTORY.
                 # If so, descend into the directory to process each file.
                 # TODO: Will this recurse forever? Is that a good thing?
                 path_is_directory = os.path.isdir(path)
                 if path_is_directory:
-                    for filename in os.listdir(path):
+                    # Filename sorting order cannot be relied upon and is an artifact of the filesystem.
+                    # This option brings some sanity to that.
+                    directory_listing = os.listdir(path)
+                    if file_detection_entry.filename_sorting_algorithm is not None:
+                        directory_listing = file_detection_entry.filename_sorting_algorithm(directory_listing)
+                    for filename in directory_listing:
                         # PROCESS ANY FILES IN THE SUB-DIRECTORY.
                         # Because the listdir function only returns the filename,
                         # it must be joined with the parent directory path.
                         sub_directory_path = [os.path.join(path, filename)]
                         # TODO: Document why only the first file detection entry is passed in
                         # to the recursive processor. This is to enforce the correct ordering.
                         self.process(sub_directory_path, [file_detection_entry])
```

### Comparing `asset_extraction_framework-0.9.4/asset_extraction_framework/Asserts.py` & `asset_extraction_framework-0.9.5/asset_extraction_framework/Asserts.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.4/asset_extraction_framework/Asset/Animation.py` & `asset_extraction_framework-0.9.5/asset_extraction_framework/Asset/Animation.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.4/asset_extraction_framework/Asset/BoundingBox.py` & `asset_extraction_framework-0.9.5/asset_extraction_framework/Asset/BoundingBox.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.4/asset_extraction_framework/Asset/Image.py` & `asset_extraction_framework-0.9.5/asset_extraction_framework/Asset/Image.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.4/asset_extraction_framework/Asset/Palette.py` & `asset_extraction_framework-0.9.5/asset_extraction_framework/Asset/Palette.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.4/asset_extraction_framework/Asset/Sound.py` & `asset_extraction_framework-0.9.5/asset_extraction_framework/Asset/Sound.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.4/asset_extraction_framework/CommandLine.py` & `asset_extraction_framework-0.9.5/asset_extraction_framework/CommandLine.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.4/asset_extraction_framework/File.py` & `asset_extraction_framework-0.9.5/asset_extraction_framework/File.py`

 * *Files identical despite different names*

### Comparing `asset_extraction_framework-0.9.4/asset_extraction_framework.egg-info/PKG-INFO` & `asset_extraction_framework-0.9.5/asset_extraction_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asset_extraction_framework
-Version: 0.9.4
+Version: 0.9.5
 Summary: Toolkit to help extract multimedia assets from legacy software
 Author: npjg
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -633,14 +633,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: Pillow>=9.2.0
 Requires-Dist: numpy>=1.23.0
 Requires-Dist: jsons>=1.6.2
+Requires-Dist: hexdump2>=1.1
 
 `assets` is a reverse-engineering framework for extracting multimedia assets from legacy software.
 
 Unlike [`mrcrowbar`](https://github.com/moralrecordings/mrcrowbar) and other reverse-engineering packages, 
 this library is not designed for editing data in-place. `assets` instead focuses on extraction. 
 
 You write the code that converts the data from your application into a standard format (pixels and PCM audio).
```

### Comparing `asset_extraction_framework-0.9.4/asset_extraction_framework.egg-info/SOURCES.txt` & `asset_extraction_framework-0.9.5/asset_extraction_framework.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 tox.ini
 .github/workflows/publish-to-pypi.yml
 .github/workflows/run-tox.yml
 asset_extraction_framework/Application.py
 asset_extraction_framework/Asserts.py
 asset_extraction_framework/CommandLine.py
+asset_extraction_framework/Exceptions.py
 asset_extraction_framework/File.py
 asset_extraction_framework/__init__.py
 asset_extraction_framework.egg-info/PKG-INFO
 asset_extraction_framework.egg-info/SOURCES.txt
 asset_extraction_framework.egg-info/dependency_links.txt
 asset_extraction_framework.egg-info/requires.txt
 asset_extraction_framework.egg-info/top_level.txt
```

### Comparing `asset_extraction_framework-0.9.4/pyproject.toml` & `asset_extraction_framework-0.9.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     "Programming Language :: Python :: 3",
 ]
 keywords = ["struct", "reverse-engineering", "self-document"]
 requires-python = ">=3.9"
 dependencies = [
     "Pillow>=9.2.0",
     "numpy>=1.23.0",
-    "jsons>=1.6.2"
+    "jsons>=1.6.2",
+    "hexdump2>=1.1"
 ]
 
 [tool.setuptools_scm]
 # Empty since no extra settings are needed, presence enables setuptools_scm.
 
 [project.urls]
 Homepage = "https://github.com/npjg/asset_extraction_framework"
```

