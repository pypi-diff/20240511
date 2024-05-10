# Comparing `tmp/xmonkey_namonica-0.1.8.tar.gz` & `tmp/xmonkey_namonica-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmonkey_namonica-0.1.8.tar", last modified: Wed May  8 06:21:05 2024, max compression
+gzip compressed data, was "xmonkey_namonica-0.1.9.tar", last modified: Wed May  8 20:45:39 2024, max compression
```

## Comparing `xmonkey_namonica-0.1.8.tar` & `xmonkey_namonica-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-08 06:21:05.167772 xmonkey_namonica-0.1.8/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.8/LICENSE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      322 2024-05-08 06:21:05.167598 xmonkey_namonica-0.1.8/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2349 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/README.md
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-05-08 06:21:05.167818 xmonkey_namonica-0.1.8/setup.cfg
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      498 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/setup.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-08 06:21:05.164998 xmonkey_namonica-0.1.8/xmonkey_namonica/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2509 2024-05-02 22:56:57.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/cli.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4244 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/common.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-08 06:21:05.167165 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1091 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/base_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2977 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/cargo_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4064 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/conda_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5853 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/gem_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4148 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/gen_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4544 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/github_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6040 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/golang_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2793 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/npm_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3011 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/nuget_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3160 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/pypi_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3481 2024-05-07 21:08:49.000000 xmonkey_namonica-0.1.8/xmonkey_namonica/utils.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-08 06:21:05.167423 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      322 2024-05-08 06:21:05.000000 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      836 2024-05-08 06:21:05.000000 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/SOURCES.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-05-08 06:21:05.000000 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/dependency_links.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-05-08 06:21:05.000000 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/entry_points.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       82 2024-05-08 06:21:05.000000 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/requires.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-05-08 06:21:05.000000 xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/top_level.txt
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-08 20:45:39.922562 xmonkey_namonica-0.1.9/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.9/LICENSE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       40 2024-05-08 20:18:58.000000 xmonkey_namonica-0.1.9/MANIFEST.in
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      625 2024-05-08 20:45:39.922385 xmonkey_namonica-0.1.9/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2349 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.9/README.md
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-05-08 20:45:39.922593 xmonkey_namonica-0.1.9/setup.cfg
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      946 2024-05-08 20:45:35.000000 xmonkey_namonica-0.1.9/setup.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-08 20:45:39.915778 xmonkey_namonica-0.1.9/xmonkey_namonica/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2509 2024-05-02 22:56:57.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/cli.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5146 2024-05-08 20:45:35.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/common.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-08 20:45:39.917545 xmonkey_namonica-0.1.9/xmonkey_namonica/datasets/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    60265 2024-05-07 21:17:49.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/datasets/naive_bayes_model.pkl
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)   243674 2024-05-07 21:17:49.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/datasets/tfidf_data.pkl
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-08 20:45:39.922055 xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1091 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/base_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2977 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/cargo_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4064 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/conda_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5853 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/gem_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4148 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/gen_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4544 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/github_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6040 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/golang_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2793 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/npm_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3011 2024-05-08 06:21:00.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/nuget_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3136 2024-05-08 20:45:35.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/pypi_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3481 2024-05-07 21:08:49.000000 xmonkey_namonica-0.1.9/xmonkey_namonica/utils.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-05-08 20:45:39.922203 xmonkey_namonica-0.1.9/xmonkey_namonica.egg-info/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      625 2024-05-08 20:45:39.000000 xmonkey_namonica-0.1.9/xmonkey_namonica.egg-info/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      937 2024-05-08 20:45:39.000000 xmonkey_namonica-0.1.9/xmonkey_namonica.egg-info/SOURCES.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-05-08 20:45:39.000000 xmonkey_namonica-0.1.9/xmonkey_namonica.egg-info/dependency_links.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-05-08 20:45:39.000000 xmonkey_namonica-0.1.9/xmonkey_namonica.egg-info/entry_points.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       82 2024-05-08 20:45:39.000000 xmonkey_namonica-0.1.9/xmonkey_namonica.egg-info/requires.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-05-08 20:45:39.000000 xmonkey_namonica-0.1.9/xmonkey_namonica.egg-info/top_level.txt
```

### Comparing `xmonkey_namonica-0.1.8/LICENSE` & `xmonkey_namonica-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.8/README.md` & `xmonkey_namonica-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica/cli.py` & `xmonkey_namonica-0.1.9/xmonkey_namonica/cli.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica/common.py` & `xmonkey_namonica-0.1.9/xmonkey_namonica/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 import re
 import json
+import pickle
+from pkg_resources import resource_filename
 from urllib.parse import unquote, urlparse, parse_qs
 from urllib.parse import urlparse, parse_qs, unquote
 from .utils import download_file, temp_directory, extract_zip, extract_tar
 
 
 class PackageManager:
     @staticmethod
@@ -77,14 +79,26 @@
                 return file.read()
         except Exception as e:
             print(f"Error reading file {file_path}: {str(e)}")
             raise
 
     @staticmethod
     def scan_for_copyright(temp_dir):
+        naive_bayes_model_path = resource_filename(
+            __name__,
+            'datasets/naive_bayes_model.pkl'
+        )
+        tfidf_data_path = resource_filename(
+            __name__,
+            'datasets/tfidf_data.pkl'
+        )
+        with open(naive_bayes_model_path, 'rb') as f:
+            classifier = pickle.load(f)
+        with open(tfidf_data_path, 'rb') as f:
+            _, _, _, _, vectorizer = pickle.load(f)
         copyrights = []
         pattern = "[^0-9<>,.()@a-zA-Z-\s]+"
         for root, _, files in os.walk(temp_dir):
             for file in files:
                 file_path = os.path.join(root, file)
                 try:
                     with open(file_path, 'r', encoding='utf-8') as f:
@@ -95,18 +109,25 @@
                                 and len(clean_line) <= 50
                             ):
                                 clean_line = re.sub(pattern, "", clean_line)
                                 if (
                                     clean_line.startswith('copyright')
                                     or " copyright" in clean_line
                                 ):
-                                    copyrights.append({
-                                        "file": file_path,
-                                        "line": clean_line
-                                    })
+                                    input_tfidf = vectorizer.transform(
+                                        [clean_line]
+                                    )
+                                    prediction = classifier.predict(
+                                        input_tfidf
+                                    )[0]
+                                    if 'copyright' in prediction:
+                                        copyrights.append({
+                                            "file": file_path,
+                                            "line": clean_line
+                                        })
                 except UnicodeDecodeError:
                     continue
         return copyrights
 
     @staticmethod
     def serialize_output(data):
         return json.dumps(data, indent=4)
```

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/base_handler.py` & `xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/cargo_handler.py` & `xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/cargo_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/conda_handler.py` & `xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/conda_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/gem_handler.py` & `xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/gem_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/gen_handler.py` & `xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/gen_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/github_handler.py` & `xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/github_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/golang_handler.py` & `xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/golang_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/npm_handler.py` & `xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/npm_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/nuget_handler.py` & `xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/nuget_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica/handlers/pypi_handler.py` & `xmonkey_namonica-0.1.9/xmonkey_namonica/handlers/pypi_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         return self.results
 
     def get_license(self, pkg_name):
         url = f"https://pypi.org/pypi/{pkg_name}/json"
         response = requests.get(url)
         if response.status_code == 200:
             data = response.json()
-            print(data)
             license_info = data['info'].get('license')
             if not license_info:
                 classifiers = data['info'].get('classifiers', [])
                 for classifier in classifiers:
                     if "License ::" in classifier:
                         license_info = classifier.split(" :: ")[-1]
                         break
```

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica/utils.py` & `xmonkey_namonica-0.1.9/xmonkey_namonica/utils.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.8/xmonkey_namonica.egg-info/SOURCES.txt` & `xmonkey_namonica-0.1.9/xmonkey_namonica.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 xmonkey_namonica/__init__.py
 xmonkey_namonica/cli.py
 xmonkey_namonica/common.py
 xmonkey_namonica/utils.py
 xmonkey_namonica.egg-info/PKG-INFO
 xmonkey_namonica.egg-info/SOURCES.txt
 xmonkey_namonica.egg-info/dependency_links.txt
 xmonkey_namonica.egg-info/entry_points.txt
 xmonkey_namonica.egg-info/requires.txt
 xmonkey_namonica.egg-info/top_level.txt
+xmonkey_namonica/datasets/naive_bayes_model.pkl
+xmonkey_namonica/datasets/tfidf_data.pkl
 xmonkey_namonica/handlers/__init__.py
 xmonkey_namonica/handlers/base_handler.py
 xmonkey_namonica/handlers/cargo_handler.py
 xmonkey_namonica/handlers/conda_handler.py
 xmonkey_namonica/handlers/gem_handler.py
 xmonkey_namonica/handlers/gen_handler.py
 xmonkey_namonica/handlers/github_handler.py
```

