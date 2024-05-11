# Comparing `tmp/STCAT-0.5.tar.gz` & `tmp/STCAT-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STCAT-0.5.tar", last modified: Mon May  6 09:30:08 2024, max compression
+gzip compressed data, was "STCAT-0.6.tar", last modified: Fri May 10 09:53:27 2024, max compression
```

## Comparing `STCAT-0.5.tar` & `STCAT-0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:30:08.000000 STCAT-0.5/
--rw-rw-r--   0 root         (0) root         (0)       56 2024-05-06 09:16:59.000000 STCAT-0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-06 09:20:25.000000 STCAT-0.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1147 2024-05-06 09:18:36.000000 STCAT-0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:30:08.000000 STCAT-0.5/STCAT/
--rw-rw-r--   0 root         (0) root         (0)    16590 2024-05-06 09:27:54.000000 STCAT-0.5/STCAT/STCAT.py
--rw-rw-r--   0 root         (0) root         (0)       68 2024-05-06 09:18:36.000000 STCAT-0.5/STCAT/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6109 2024-05-06 09:15:45.000000 STCAT-0.5/STCAT/annotate.py
--rw-rw-r--   0 root         (0) root         (0)    27653 2024-05-06 09:15:45.000000 STCAT-0.5/STCAT/classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:30:08.000000 STCAT-0.5/STCAT/data/
--rw-rw-r--   0 root         (0) root         (0)  1017541 2024-05-06 09:18:36.000000 STCAT-0.5/STCAT/data/T_cell.pkl
--rw-rw-r--   0 root         (0) root         (0)   549290 2024-05-06 09:18:36.000000 STCAT-0.5/STCAT/data/cd4.pkl
--rw-rw-r--   0 root         (0) root         (0)   286349 2024-05-06 09:27:54.000000 STCAT-0.5/STCAT/data/cd8.pkl
--rw-rw-r--   0 root         (0) root         (0)    11124 2024-05-06 09:19:27.000000 STCAT-0.5/STCAT/data/marker_CD4.txt
--rw-rw-r--   0 root         (0) root         (0)     5189 2024-05-06 09:18:36.000000 STCAT-0.5/STCAT/data/marker_CD8.txt
--rw-rw-r--   0 root         (0) root         (0)      233 2024-05-06 09:16:59.000000 STCAT-0.5/STCAT/logger.py
--rw-rw-r--   0 root         (0) root         (0)     7505 2024-05-06 09:27:54.000000 STCAT-0.5/STCAT/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 09:30:08.000000 STCAT-0.5/STCAT.egg-info/
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-06 09:19:33.000000 STCAT-0.5/STCAT.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      406 2024-05-06 09:20:25.000000 STCAT-0.5/STCAT.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 09:28:52.000000 STCAT-0.5/STCAT.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2024-05-06 09:17:57.000000 STCAT-0.5/STCAT.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-06 09:16:43.000000 STCAT-0.5/STCAT.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      116 2024-05-06 09:27:54.000000 STCAT-0.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-06 09:17:57.000000 STCAT-0.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      777 2024-05-06 09:18:36.000000 STCAT-0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 09:53:27.000000 STCAT-0.6/
+-rw-rw-r--   0 root         (0) root         (0)       56 2024-05-10 09:38:35.000000 STCAT-0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-10 09:42:51.000000 STCAT-0.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1147 2024-05-10 09:40:14.000000 STCAT-0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 09:53:27.000000 STCAT-0.6/STCAT/
+-rw-rw-r--   0 root         (0) root         (0)    16590 2024-05-10 09:40:14.000000 STCAT-0.6/STCAT/STCAT.py
+-rw-rw-r--   0 root         (0) root         (0)       68 2024-05-10 09:49:32.000000 STCAT-0.6/STCAT/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6109 2024-05-10 09:41:06.000000 STCAT-0.6/STCAT/annotate.py
+-rw-rw-r--   0 root         (0) root         (0)    27653 2024-05-10 09:49:32.000000 STCAT-0.6/STCAT/classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 09:53:27.000000 STCAT-0.6/STCAT/data/
+-rw-rw-r--   0 root         (0) root         (0)  1017541 2024-05-10 09:40:14.000000 STCAT-0.6/STCAT/data/T_cell.pkl
+-rw-rw-r--   0 root         (0) root         (0)   549290 2024-05-10 09:38:35.000000 STCAT-0.6/STCAT/data/cd4.pkl
+-rw-rw-r--   0 root         (0) root         (0)   286349 2024-05-10 09:40:14.000000 STCAT-0.6/STCAT/data/cd8.pkl
+-rw-rw-r--   0 root         (0) root         (0)    11314 2024-05-10 09:40:14.000000 STCAT-0.6/STCAT/data/marker_CD4.txt
+-rw-rw-r--   0 root         (0) root         (0)     5175 2024-05-10 09:37:23.000000 STCAT-0.6/STCAT/data/marker_CD8.txt
+-rw-rw-r--   0 root         (0) root         (0)      233 2024-05-10 09:40:14.000000 STCAT-0.6/STCAT/logger.py
+-rw-rw-r--   0 root         (0) root         (0)     7505 2024-05-10 09:37:23.000000 STCAT-0.6/STCAT/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 09:53:27.000000 STCAT-0.6/STCAT.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-10 09:52:08.000000 STCAT-0.6/STCAT.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      406 2024-05-10 09:40:00.000000 STCAT-0.6/STCAT.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 09:42:51.000000 STCAT-0.6/STCAT.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2024-05-10 09:43:42.000000 STCAT-0.6/STCAT.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-10 09:52:08.000000 STCAT-0.6/STCAT.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      116 2024-05-10 09:49:32.000000 STCAT-0.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 09:52:08.000000 STCAT-0.6/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      777 2024-05-10 09:40:14.000000 STCAT-0.6/setup.py
```

### Comparing `STCAT-0.5/README.md` & `STCAT-0.6/README.md`

 * *Files identical despite different names*

### Comparing `STCAT-0.5/STCAT/STCAT.py` & `STCAT-0.6/STCAT/STCAT.py`

 * *Files identical despite different names*

### Comparing `STCAT-0.5/STCAT/annotate.py` & `STCAT-0.6/STCAT/annotate.py`

 * *Files identical despite different names*

### Comparing `STCAT-0.5/STCAT/classifier.py` & `STCAT-0.6/STCAT/classifier.py`

 * *Files identical despite different names*

### Comparing `STCAT-0.5/STCAT/data/T_cell.pkl` & `STCAT-0.6/STCAT/data/T_cell.pkl`

 * *Files identical despite different names*

### Comparing `STCAT-0.5/STCAT/data/cd4.pkl` & `STCAT-0.6/STCAT/data/cd4.pkl`

 * *Files identical despite different names*

### Comparing `STCAT-0.5/STCAT/data/cd8.pkl` & `STCAT-0.6/STCAT/data/cd8.pkl`

 * *Files identical despite different names*

### Comparing `STCAT-0.5/STCAT/data/marker_CD4.txt` & `STCAT-0.6/STCAT/data/marker_CD4.txt`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9767441860465116%*

 * *Differences: {"'CD4 Tn Regulating'": "['CCR7', 'SELL', 'TCF7', 'LEF1', 'IL7R', 'FOXP3', 'IKZF2', 'IKZF4', "*

 * *                        "'IL2RA', 'ENTPD1', 'CCR4', 'ICOS', 'IL10RA', 'TGFB1', 'TIGIT', 'CTLA4', "*

 * *                        "'LAG3', 'HAVCR2', 'PDCD1']"}*

```diff
@@ -525,14 +525,35 @@
         "IFNAR2",
         "IFITM1",
         "ISG15",
         "PARP14",
         "IRF1",
         "CCR7"
     ],
+    "CD4 Tn Regulating": [
+        "CCR7",
+        "SELL",
+        "TCF7",
+        "LEF1",
+        "IL7R",
+        "FOXP3",
+        "IKZF2",
+        "IKZF4",
+        "IL2RA",
+        "ENTPD1",
+        "CCR4",
+        "ICOS",
+        "IL10RA",
+        "TGFB1",
+        "TIGIT",
+        "CTLA4",
+        "LAG3",
+        "HAVCR2",
+        "PDCD1"
+    ],
     "CD4 Treg": [
         "FOXP3",
         "CTLA4",
         "IL2RA",
         "IKZF2",
         "TNFRSF9",
         "TIGIT",
```

### Comparing `STCAT-0.5/STCAT/data/marker_CD8.txt` & `STCAT-0.6/STCAT/data/marker_CD8.txt`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9130434782608695%*

 * *Differences: {"'CD8 T'": "['CD8']", 'delete': "['CD8 T Heterogeneous']"}*

```diff
@@ -127,15 +127,15 @@
         "MAPK9",
         "TERF2",
         "IFNAR1",
         "CDKN2A",
         "CDKN1A",
         "MAPK14"
     ],
-    "CD8 T Heterogeneous": [
+    "CD8 T": [
         "CD8"
     ],
     "CD8 Tc": [
         "PLEK",
         "KLRG1",
         "GNLY",
         "FCRL6",
```

### Comparing `STCAT-0.5/STCAT/models.py` & `STCAT-0.6/STCAT/models.py`

 * *Files identical despite different names*

### Comparing `STCAT-0.5/setup.py` & `STCAT-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def get_requirements():
     with open("requirements.txt", "rt", encoding="utf-8") as fh:
         return [line.strip() for line in fh.readlines()]
 
 setuptools.setup(
     name='STCAT',
-    version='0.5',
+    version='0.6',
     packages=setuptools.find_packages(),
     install_requires=get_requirements(),
     include_package_data=True,
     python_requires='>=3.8',
     url="https://github.com/GuoBioinfoLab/STCAT",
     description="An automated T cell type annotation tool for scRNA-seq datasets.",
     classifiers=[
```

