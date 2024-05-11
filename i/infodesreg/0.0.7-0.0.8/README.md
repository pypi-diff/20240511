# Comparing `tmp/infodesreg-0.0.7.tar.gz` & `tmp/infodesreg-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infodesreg-0.0.7.tar", last modified: Sat Apr 27 18:17:55 2024, max compression
+gzip compressed data, was "infodesreg-0.0.8.tar", last modified: Sat May 11 15:24:46 2024, max compression
```

## Comparing `infodesreg-0.0.7.tar` & `infodesreg-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-27 18:17:55.410247 infodesreg-0.0.7/
--rw-r--r--   0 firuzjuraev   (501) staff       (20)     1073 2024-04-26 17:42:23.000000 infodesreg-0.0.7/LICENSE
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-27 18:17:55.410073 infodesreg-0.0.7/PKG-INFO
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      202 2024-04-26 17:42:07.000000 infodesreg-0.0.7/README.md
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      491 2024-04-27 18:17:47.000000 infodesreg-0.0.7/pyproject.toml
--rw-r--r--   0 firuzjuraev   (501) staff       (20)       38 2024-04-27 18:17:55.410309 infodesreg-0.0.7/setup.cfg
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-27 18:17:55.408088 infodesreg-0.0.7/src/
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-27 18:17:55.409099 infodesreg-0.0.7/src/infodesreg/
--rw-r--r--   0 firuzjuraev   (501) staff       (20)       41 2024-04-27 17:45:56.000000 infodesreg-0.0.7/src/infodesreg/__init__.py
--rw-r--r--   0 firuzjuraev   (501) staff       (20)     6606 2024-04-27 18:17:15.000000 infodesreg-0.0.7/src/infodesreg/des.py
-drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-04-27 18:17:55.409897 infodesreg-0.0.7/src/infodesreg.egg-info/
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      713 2024-04-27 18:17:55.000000 infodesreg-0.0.7/src/infodesreg.egg-info/PKG-INFO
--rw-r--r--   0 firuzjuraev   (501) staff       (20)      233 2024-04-27 18:17:55.000000 infodesreg-0.0.7/src/infodesreg.egg-info/SOURCES.txt
--rw-r--r--   0 firuzjuraev   (501) staff       (20)        1 2024-04-27 18:17:55.000000 infodesreg-0.0.7/src/infodesreg.egg-info/dependency_links.txt
--rw-r--r--   0 firuzjuraev   (501) staff       (20)       11 2024-04-27 18:17:55.000000 infodesreg-0.0.7/src/infodesreg.egg-info/top_level.txt
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-05-11 15:24:46.579703 infodesreg-0.0.8/
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)     1073 2024-04-26 17:42:23.000000 infodesreg-0.0.8/LICENSE
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)     3718 2024-05-11 15:24:46.579530 infodesreg-0.0.8/PKG-INFO
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)     3208 2024-05-11 15:04:26.000000 infodesreg-0.0.8/README.md
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      491 2024-05-11 15:24:25.000000 infodesreg-0.0.8/pyproject.toml
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)       38 2024-05-11 15:24:46.579741 infodesreg-0.0.8/setup.cfg
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-05-11 15:24:46.577654 infodesreg-0.0.8/src/
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-05-11 15:24:46.578497 infodesreg-0.0.8/src/infodesreg/
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)       41 2024-04-27 17:45:56.000000 infodesreg-0.0.8/src/infodesreg/__init__.py
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)     6850 2024-05-11 15:04:54.000000 infodesreg-0.0.8/src/infodesreg/des.py
+drwxr-xr-x   0 firuzjuraev   (501) staff       (20)        0 2024-05-11 15:24:46.579363 infodesreg-0.0.8/src/infodesreg.egg-info/
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)     3718 2024-05-11 15:24:46.000000 infodesreg-0.0.8/src/infodesreg.egg-info/PKG-INFO
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)      233 2024-05-11 15:24:46.000000 infodesreg-0.0.8/src/infodesreg.egg-info/SOURCES.txt
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)        1 2024-05-11 15:24:46.000000 infodesreg-0.0.8/src/infodesreg.egg-info/dependency_links.txt
+-rw-r--r--   0 firuzjuraev   (501) staff       (20)       11 2024-05-11 15:24:46.000000 infodesreg-0.0.8/src/infodesreg.egg-info/top_level.txt
```

### Comparing `infodesreg-0.0.7/LICENSE` & `infodesreg-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `infodesreg-0.0.7/src/infodesreg/des.py` & `infodesreg-0.0.8/src/infodesreg/des.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,14 +159,20 @@
         for i in range(X.shape[0]):
             query = X.iloc[[i]] 
 
             pred = self.predict_single_sample(query)
             preds.append(pred) 
         
         return preds  
+    
+    
+    def score(self, X, y): 
+        preds = self.predict(X) 
+        
+        return mean_squared_error(y, preds)
 
 
 
 
 class DRS(BaseDER): 
     def __init__(self, pool_regressors=None, k=7, knn_metric='minkowski', metrics='mse', threshold=0.2):
         super(DRS, self).__init__(pool_regressors=pool_regressors, k=k, knn_metric=knn_metric, metrics=metrics, threshold=threshold) 
@@ -211,8 +217,14 @@
 
         for i in range(X.shape[0]):
             query = X.iloc[[i]] 
 
             pred = self.predict_single_sample(query)
             preds.append(pred) 
         
-        return preds 
+        return preds 
+    
+
+    def score(self, X, y): 
+        preds = self.predict(X) 
+        
+        return mean_squared_error(y, preds)
```

