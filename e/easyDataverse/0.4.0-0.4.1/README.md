# Comparing `tmp/easydataverse-0.4.0.tar.gz` & `tmp/easydataverse-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydataverse-0.4.0.tar", max compression
+gzip compressed data, was "easydataverse-0.4.1.tar", max compression
```

## Comparing `easydataverse-0.4.0.tar` & `easydataverse-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2024-05-09 20:41:59.766842 easydataverse-0.4.0/LICENSE
--rw-r--r--   0        0        0     3771 2024-05-09 20:41:59.766842 easydataverse-0.4.0/Readme.md
--rw-r--r--   0        0        0      155 2024-05-09 20:41:59.766842 easydataverse-0.4.0/easyDataverse/__init__.py
--rw-r--r--   0        0        0    13437 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/base.py
--rw-r--r--   0        0        0    11339 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/classgen.py
--rw-r--r--   0        0        0     1867 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/connect.py
--rw-r--r--   0        0        0    12760 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/dataset.py
--rw-r--r--   0        0        0    18696 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/dataverse.py
--rw-r--r--   0        0        0     5958 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/downloader.py
--rw-r--r--   0        0        0     4402 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/uploader.py
--rw-r--r--   0        0        0      174 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/utils.py
--rw-r--r--   0        0        0      867 2024-05-09 20:41:59.770842 easydataverse-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5027 1970-01-01 00:00:00.000000 easydataverse-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-11 12:52:29.222305 easydataverse-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3726 2024-05-11 12:52:29.222305 easydataverse-0.4.1/Readme.md
+-rw-r--r--   0        0        0      155 2024-05-11 12:52:29.222305 easydataverse-0.4.1/easyDataverse/__init__.py
+-rw-r--r--   0        0        0    13437 2024-05-11 12:52:29.222305 easydataverse-0.4.1/easyDataverse/base.py
+-rw-r--r--   0        0        0    11339 2024-05-11 12:52:29.222305 easydataverse-0.4.1/easyDataverse/classgen.py
+-rw-r--r--   0        0        0     1867 2024-05-11 12:52:29.222305 easydataverse-0.4.1/easyDataverse/connect.py
+-rw-r--r--   0        0        0    12763 2024-05-11 12:52:29.222305 easydataverse-0.4.1/easyDataverse/dataset.py
+-rw-r--r--   0        0        0    18696 2024-05-11 12:52:29.222305 easydataverse-0.4.1/easyDataverse/dataverse.py
+-rw-r--r--   0        0        0     5958 2024-05-11 12:52:29.222305 easydataverse-0.4.1/easyDataverse/downloader.py
+-rw-r--r--   0        0        0     4402 2024-05-11 12:52:29.222305 easydataverse-0.4.1/easyDataverse/uploader.py
+-rw-r--r--   0        0        0      174 2024-05-11 12:52:29.226305 easydataverse-0.4.1/easyDataverse/utils.py
+-rw-r--r--   0        0        0      867 2024-05-11 12:52:29.226305 easydataverse-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4982 1970-01-01 00:00:00.000000 easydataverse-0.4.1/PKG-INFO
```

### Comparing `easydataverse-0.4.0/LICENSE` & `easydataverse-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easydataverse-0.4.0/Readme.md` & `easydataverse-0.4.1/Readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,23 +18,21 @@
 
 ## ⚡️ Quick start
 
 Get started with EasyDataverse by running the following command
 
 ```bash
 # Using PyPI
-python -m pip install easyDataverse
+pip install easyDataverse
 ```
 
 Or build by source
 
 ```bash
-git clone https://github.com/gdcc/easyDataverse.git
-cd easyDataverse
-python setup.py install
+pip install git+https://github.com/gdcc/easyDataverse.git
 ```
 
 ## ⚙️ Quickstart
 
 ### Dataset creation
 
 EasyDataverse is capable of connecting to a given Dataverse installation and fetch all metadata fields and their properties. This allows you to create a dataset object with all the metadata fields and their properties given at the Dataverse installation.
```

### Comparing `easydataverse-0.4.0/easyDataverse/base.py` & `easydataverse-0.4.1/easyDataverse/base.py`

 * *Files identical despite different names*

### Comparing `easydataverse-0.4.0/easyDataverse/classgen.py` & `easydataverse-0.4.1/easyDataverse/classgen.py`

 * *Files identical despite different names*

### Comparing `easydataverse-0.4.0/easyDataverse/connect.py` & `easydataverse-0.4.1/easyDataverse/connect.py`

 * *Files identical despite different names*

### Comparing `easydataverse-0.4.0/easyDataverse/dataset.py` & `easydataverse-0.4.1/easyDataverse/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             dirpath (str): Path to the directory
             include_hidden (bool, optional): Whether or not hidden folders "." should be included. Defaults to False.
             ignores (List[str], optional): List of extensions/directories that should be ignored. Defaults to [].
         """
 
         self.files += add_directory(
             directory=dirpath,
-            directory_label=dv_dir,
+            rootDirectoryLabel=dv_dir,
             ignore=ignores,
         )
 
     @staticmethod
     def _has_hidden_dir(path: str, dirpath: str) -> bool:
         """Checks whether a hidden directory ('.') exists in a path."""
```

### Comparing `easydataverse-0.4.0/easyDataverse/dataverse.py` & `easydataverse-0.4.1/easyDataverse/dataverse.py`

 * *Files identical despite different names*

### Comparing `easydataverse-0.4.0/easyDataverse/downloader.py` & `easydataverse-0.4.1/easyDataverse/downloader.py`

 * *Files identical despite different names*

### Comparing `easydataverse-0.4.0/easyDataverse/uploader.py` & `easydataverse-0.4.1/easyDataverse/uploader.py`

 * *Files identical despite different names*

### Comparing `easydataverse-0.4.0/pyproject.toml` & `easydataverse-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyDataverse"
-version = "0.4.0"
+version = "0.4.1"
 description = "Lightweight Dataverse interface in Python to upload, download and update datasets found in Dataverse instances."
 authors = ["Jan Range <jan.range@simtech.uni-stuttgart.de>"]
 license = "MIT License"
 readme = "Readme.md"
 packages = [{ include = "easyDataverse" }]
 
 [tool.poetry.dependencies]
```

### Comparing `easydataverse-0.4.0/PKG-INFO` & `easydataverse-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyDataverse
-Version: 0.4.0
+Version: 0.4.1
 Summary: Lightweight Dataverse interface in Python to upload, download and update datasets found in Dataverse instances.
 License: MIT
 Author: Jan Range
 Author-email: jan.range@simtech.uni-stuttgart.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -49,23 +49,21 @@
 
 ## ⚡️ Quick start
 
 Get started with EasyDataverse by running the following command
 
 ```bash
 # Using PyPI
-python -m pip install easyDataverse
+pip install easyDataverse
 ```
 
 Or build by source
 
 ```bash
-git clone https://github.com/gdcc/easyDataverse.git
-cd easyDataverse
-python setup.py install
+pip install git+https://github.com/gdcc/easyDataverse.git
 ```
 
 ## ⚙️ Quickstart
 
 ### Dataset creation
 
 EasyDataverse is capable of connecting to a given Dataverse installation and fetch all metadata fields and their properties. This allows you to create a dataset object with all the metadata fields and their properties given at the Dataverse installation.
```

