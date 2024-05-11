# Comparing `tmp/starparser-1.56.tar.gz` & `tmp/starparser-1.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starparser-1.56.tar", last modified: Sat Apr 20 08:52:32 2024, max compression
+gzip compressed data, was "starparser-1.57.tar", last modified: Sat May 11 20:28:40 2024, max compression
```

## Comparing `starparser-1.56.tar` & `starparser-1.57.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-20 08:52:32.201653 starparser-1.56/
--rw-r--r--   0 chaaban    (501) staff       (20)     1069 2023-06-05 21:07:33.000000 starparser-1.56/LICENSE.txt
--rw-r--r--   0 chaaban    (501) staff       (20)    36912 2024-04-20 08:52:32.201526 starparser-1.56/PKG-INFO
--rw-r--r--   0 chaaban    (501) staff       (20)    36609 2024-04-08 21:18:39.000000 starparser-1.56/README.md
--rw-r--r--   0 chaaban    (501) staff       (20)       38 2024-04-20 08:52:32.201712 starparser-1.56/setup.cfg
--rw-r--r--   0 chaaban    (501) staff       (20)      880 2023-08-26 16:02:58.000000 starparser-1.56/setup.py
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-20 08:52:32.200545 starparser-1.56/starparser/
--rw-r--r--   0 chaaban    (501) staff       (20)       82 2024-04-20 08:51:20.000000 starparser-1.56/starparser/__init__.py
--rw-r--r--   0 chaaban    (501) staff       (20)      119 2023-08-11 15:52:04.000000 starparser-1.56/starparser/__main__.py
--rw-r--r--   0 chaaban    (501) staff       (20)    20433 2024-04-07 12:48:12.000000 starparser-1.56/starparser/argparser.py
--rw-r--r--   0 chaaban    (501) staff       (20)     9351 2024-01-27 11:30:44.000000 starparser-1.56/starparser/columnplay.py
--rw-r--r--   0 chaaban    (501) staff       (20)    52470 2024-04-07 12:48:26.000000 starparser-1.56/starparser/decisiontree.py
--rw-r--r--   0 chaaban    (501) staff       (20)    10501 2024-04-08 15:16:19.000000 starparser-1.56/starparser/fileparser.py
--rw-r--r--   0 chaaban    (501) staff       (20)    22907 2024-04-20 08:37:29.000000 starparser-1.56/starparser/particleplay.py
--rw-r--r--   0 chaaban    (501) staff       (20)    26805 2023-09-02 00:09:18.000000 starparser-1.56/starparser/plots.py
--rw-r--r--   0 chaaban    (501) staff       (20)    13056 2023-08-26 18:27:37.000000 starparser-1.56/starparser/specialparticles.py
--rw-r--r--   0 chaaban    (501) staff       (20)     1890 2023-08-11 15:52:04.000000 starparser-1.56/starparser/splits.py
-drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-04-20 08:52:32.201329 starparser-1.56/starparser.egg-info/
--rw-r--r--   0 chaaban    (501) staff       (20)    36912 2024-04-20 08:52:32.000000 starparser-1.56/starparser.egg-info/PKG-INFO
--rw-r--r--   0 chaaban    (501) staff       (20)      482 2024-04-20 08:52:32.000000 starparser-1.56/starparser.egg-info/SOURCES.txt
--rw-r--r--   0 chaaban    (501) staff       (20)        1 2024-04-20 08:52:32.000000 starparser-1.56/starparser.egg-info/dependency_links.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       56 2024-04-20 08:52:32.000000 starparser-1.56/starparser.egg-info/entry_points.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       30 2024-04-20 08:52:32.000000 starparser-1.56/starparser.egg-info/requires.txt
--rw-r--r--   0 chaaban    (501) staff       (20)       11 2024-04-20 08:52:32.000000 starparser-1.56/starparser.egg-info/top_level.txt
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-05-11 20:28:40.233284 starparser-1.57/
+-rw-r--r--   0 chaaban    (501) staff       (20)     1069 2023-06-05 21:07:33.000000 starparser-1.57/LICENSE.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)    36912 2024-05-11 20:28:40.233151 starparser-1.57/PKG-INFO
+-rw-r--r--   0 chaaban    (501) staff       (20)    36609 2024-04-08 21:18:39.000000 starparser-1.57/README.md
+-rw-r--r--   0 chaaban    (501) staff       (20)       38 2024-05-11 20:28:40.233347 starparser-1.57/setup.cfg
+-rw-r--r--   0 chaaban    (501) staff       (20)      880 2023-08-26 16:02:58.000000 starparser-1.57/setup.py
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-05-11 20:28:40.232161 starparser-1.57/starparser/
+-rw-r--r--   0 chaaban    (501) staff       (20)       82 2024-05-11 20:27:45.000000 starparser-1.57/starparser/__init__.py
+-rw-r--r--   0 chaaban    (501) staff       (20)      119 2023-08-11 15:52:04.000000 starparser-1.57/starparser/__main__.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    20433 2024-04-07 12:48:12.000000 starparser-1.57/starparser/argparser.py
+-rw-r--r--   0 chaaban    (501) staff       (20)     9351 2024-01-27 11:30:44.000000 starparser-1.57/starparser/columnplay.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    52470 2024-04-07 12:48:26.000000 starparser-1.57/starparser/decisiontree.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    10501 2024-04-08 15:16:19.000000 starparser-1.57/starparser/fileparser.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    22907 2024-04-20 08:37:29.000000 starparser-1.57/starparser/particleplay.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    26805 2024-05-11 20:27:37.000000 starparser-1.57/starparser/plots.py
+-rw-r--r--   0 chaaban    (501) staff       (20)    13056 2023-08-26 18:27:37.000000 starparser-1.57/starparser/specialparticles.py
+-rw-r--r--   0 chaaban    (501) staff       (20)     1890 2023-08-11 15:52:04.000000 starparser-1.57/starparser/splits.py
+drwxr-xr-x   0 chaaban    (501) staff       (20)        0 2024-05-11 20:28:40.232958 starparser-1.57/starparser.egg-info/
+-rw-r--r--   0 chaaban    (501) staff       (20)    36912 2024-05-11 20:28:40.000000 starparser-1.57/starparser.egg-info/PKG-INFO
+-rw-r--r--   0 chaaban    (501) staff       (20)      482 2024-05-11 20:28:40.000000 starparser-1.57/starparser.egg-info/SOURCES.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)        1 2024-05-11 20:28:40.000000 starparser-1.57/starparser.egg-info/dependency_links.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       56 2024-05-11 20:28:40.000000 starparser-1.57/starparser.egg-info/entry_points.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       30 2024-05-11 20:28:40.000000 starparser-1.57/starparser.egg-info/requires.txt
+-rw-r--r--   0 chaaban    (501) staff       (20)       11 2024-05-11 20:28:40.000000 starparser-1.57/starparser.egg-info/top_level.txt
```

### Comparing `starparser-1.56/LICENSE.txt` & `starparser-1.57/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starparser-1.56/PKG-INFO` & `starparser-1.57/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starparser
-Version: 1.56
+Version: 1.57
 Summary: Manipulate and mine Relion star files.
 Home-page: http://pypi.python.org/pypi/starparser/
 Author: Sami Chaaban
 Author-email: chaaban@mrc-lmb.cam.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `starparser-1.56/README.md` & `starparser-1.57/README.md`

 * *Files identical despite different names*

### Comparing `starparser-1.56/setup.py` & `starparser-1.57/setup.py`

 * *Files identical despite different names*

### Comparing `starparser-1.56/starparser/argparser.py` & `starparser-1.57/starparser/argparser.py`

 * *Files identical despite different names*

### Comparing `starparser-1.56/starparser/columnplay.py` & `starparser-1.57/starparser/columnplay.py`

 * *Files identical despite different names*

### Comparing `starparser-1.56/starparser/decisiontree.py` & `starparser-1.57/starparser/decisiontree.py`

 * *Files identical despite different names*

### Comparing `starparser-1.56/starparser/fileparser.py` & `starparser-1.57/starparser/fileparser.py`

 * *Files identical despite different names*

### Comparing `starparser-1.56/starparser/particleplay.py` & `starparser-1.57/starparser/particleplay.py`

 * *Files identical despite different names*

### Comparing `starparser-1.56/starparser/plots.py` & `starparser-1.57/starparser/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,15 +524,15 @@
     file1xloc = file1parts.columns.get_loc("_rlnCoordinateX")+1
     file1yloc = file1parts.columns.get_loc("_rlnCoordinateY")+1
 
     #Do the same for the second star file if it has values. The original micrograph names don't 
     #need to be preserved.
     if not file2parts.empty:
         
-        if "_rlnMicrogrpahName" not in file2parts:
+        if "_rlnMicrographName" not in file2parts:
             print("\n>> Error: the second star file does not have a _rlnMicrographName column.\n")
             sys.exit()
 
         file2parts["_rlnMicrographName"] = file2parts["_rlnMicrographName"].str.split('/').str[-1]
 
         file2mics = file2parts.groupby(["_rlnMicrographName"])
```

### Comparing `starparser-1.56/starparser/specialparticles.py` & `starparser-1.57/starparser/specialparticles.py`

 * *Files identical despite different names*

### Comparing `starparser-1.56/starparser/splits.py` & `starparser-1.57/starparser/splits.py`

 * *Files identical despite different names*

### Comparing `starparser-1.56/starparser.egg-info/PKG-INFO` & `starparser-1.57/starparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starparser
-Version: 1.56
+Version: 1.57
 Summary: Manipulate and mine Relion star files.
 Home-page: http://pypi.python.org/pypi/starparser/
 Author: Sami Chaaban
 Author-email: chaaban@mrc-lmb.cam.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

