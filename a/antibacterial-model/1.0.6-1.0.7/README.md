# Comparing `tmp/antibacterial-model-1.0.6.tar.gz` & `tmp/antibacterial-model-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antibacterial-model-1.0.6.tar", last modified: Fri May 10 11:11:20 2024, max compression
+gzip compressed data, was "antibacterial-model-1.0.7.tar", last modified: Sat May 11 15:21:17 2024, max compression
```

## Comparing `antibacterial-model-1.0.6.tar` & `antibacterial-model-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 11:11:20.128194 antibacterial-model-1.0.6/
--rw-rw-rw-   0        0        0      773 2024-05-10 11:11:20.127198 antibacterial-model-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      104 2024-05-10 10:25:58.000000 antibacterial-model-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 11:11:20.037187 antibacterial-model-1.0.6/antibacterial_model/
--rw-rw-rw-   0        0        0      168 2024-05-10 10:45:14.000000 antibacterial-model-1.0.6/antibacterial_model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 11:11:20.124193 antibacterial-model-1.0.6/antibacterial_model/data/
--rw-rw-rw-   0        0        0 16991105 2024-05-10 08:51:19.000000 antibacterial-model-1.0.6/antibacterial_model/data/anti-bact-data.csv
--rw-rw-rw-   0        0        0     7993 2024-04-08 15:16:20.000000 antibacterial-model-1.0.6/antibacterial_model/data/anti-bact-model.pkl
--rw-rw-rw-   0        0        0     4308 2024-05-10 10:38:18.000000 antibacterial-model-1.0.6/antibacterial_model/model.py
-drwxrwxrwx   0        0        0        0 2024-05-10 11:11:20.069194 antibacterial-model-1.0.6/antibacterial_model.egg-info/
--rw-rw-rw-   0        0        0      773 2024-05-10 11:11:19.000000 antibacterial-model-1.0.6/antibacterial_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2024-05-10 11:11:19.000000 antibacterial-model-1.0.6/antibacterial_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 11:11:19.000000 antibacterial-model-1.0.6/antibacterial_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2024-05-10 11:11:19.000000 antibacterial-model-1.0.6/antibacterial_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-10 11:11:19.000000 antibacterial-model-1.0.6/antibacterial_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 11:11:20.129194 antibacterial-model-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1119 2024-05-10 11:10:55.000000 antibacterial-model-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 15:21:17.196967 antibacterial-model-1.0.7/
+-rw-rw-rw-   0        0        0     3160 2024-05-11 15:21:17.195979 antibacterial-model-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2473 2024-05-11 15:21:07.000000 antibacterial-model-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 15:21:17.083946 antibacterial-model-1.0.7/antibacterial_model/
+-rw-rw-rw-   0        0        0      168 2024-05-10 10:45:14.000000 antibacterial-model-1.0.7/antibacterial_model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 15:21:17.193957 antibacterial-model-1.0.7/antibacterial_model/data/
+-rw-rw-rw-   0        0        0 16991105 2024-05-10 08:51:19.000000 antibacterial-model-1.0.7/antibacterial_model/data/anti-bact-data.csv
+-rw-rw-rw-   0        0        0     7993 2024-04-08 15:16:20.000000 antibacterial-model-1.0.7/antibacterial_model/data/anti-bact-model.pkl
+-rw-rw-rw-   0        0        0     4308 2024-05-10 10:38:18.000000 antibacterial-model-1.0.7/antibacterial_model/model.py
+drwxrwxrwx   0        0        0        0 2024-05-11 15:21:17.128949 antibacterial-model-1.0.7/antibacterial_model.egg-info/
+-rw-rw-rw-   0        0        0     3160 2024-05-11 15:21:16.000000 antibacterial-model-1.0.7/antibacterial_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2024-05-11 15:21:16.000000 antibacterial-model-1.0.7/antibacterial_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 15:21:16.000000 antibacterial-model-1.0.7/antibacterial_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-05-11 15:21:16.000000 antibacterial-model-1.0.7/antibacterial_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-11 15:21:16.000000 antibacterial-model-1.0.7/antibacterial_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 15:21:17.196967 antibacterial-model-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2024-05-11 15:21:02.000000 antibacterial-model-1.0.7/setup.py
```

### Comparing `antibacterial-model-1.0.6/antibacterial_model/data/anti-bact-data.csv` & `antibacterial-model-1.0.7/antibacterial_model/data/anti-bact-data.csv`

 * *Files identical despite different names*

### Comparing `antibacterial-model-1.0.6/antibacterial_model/data/anti-bact-model.pkl` & `antibacterial-model-1.0.7/antibacterial_model/data/anti-bact-model.pkl`

 * *Files identical despite different names*

### Comparing `antibacterial-model-1.0.6/antibacterial_model/model.py` & `antibacterial-model-1.0.7/antibacterial_model/model.py`

 * *Files identical despite different names*

### Comparing `antibacterial-model-1.0.6/setup.py` & `antibacterial-model-1.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='antibacterial-model',
-    version='1.0.6',
+    version='1.0.7',
     description='A model for predicting antibacterial activity from SMILES strings',
-    author='Chonthicha Arbsuwan',
+    author='Chonthicha Arbsuwan, Jiratchaya Nakbang',
     author_email='chon7599@gmail.com',
     packages=find_packages(),
     install_requires=[
         'numpy==1.24.1',
         'rdkit==2023.3.3',
         'scikit-learn==1.2.1',
         'joblib==1.2.0',
```

