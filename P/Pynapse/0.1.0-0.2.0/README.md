# Comparing `tmp/pynapse-0.1.0.tar.gz` & `tmp/pynapse-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynapse-0.1.0.tar", last modified: Sat May 11 02:55:14 2024, max compression
+gzip compressed data, was "pynapse-0.2.0.tar", last modified: Sat May 11 03:55:43 2024, max compression
```

## Comparing `pynapse-0.1.0.tar` & `pynapse-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 02:55:14.242519 pynapse-0.1.0/
--rw-rw-rw-   0        0        0       76 2024-05-11 02:55:14.239531 pynapse-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-11 02:55:14.205904 pynapse-0.1.0/Pynapse/
--rw-rw-rw-   0        0        0      151 2024-05-11 02:36:57.000000 pynapse-0.1.0/Pynapse/__init__.py
--rw-rw-rw-   0        0        0     2574 2024-05-11 02:35:49.000000 pynapse-0.1.0/Pynapse/main.py
-drwxrwxrwx   0        0        0        0 2024-05-11 02:55:14.237532 pynapse-0.1.0/Pynapse.egg-info/
--rw-rw-rw-   0        0        0       76 2024-05-11 02:55:13.000000 pynapse-0.1.0/Pynapse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-11 02:55:13.000000 pynapse-0.1.0/Pynapse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 02:55:13.000000 pynapse-0.1.0/Pynapse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-11 02:55:13.000000 pynapse-0.1.0/Pynapse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-11 02:55:13.000000 pynapse-0.1.0/Pynapse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 02:55:14.243527 pynapse-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      179 2024-05-11 02:53:16.000000 pynapse-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:55:43.753703 pynapse-0.2.0/
+-rw-rw-rw-   0        0        0       76 2024-05-11 03:55:43.751708 pynapse-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 03:55:43.725436 pynapse-0.2.0/Pynapse/
+-rw-rw-rw-   0        0        0      151 2024-05-11 02:36:57.000000 pynapse-0.2.0/Pynapse/__init__.py
+-rw-rw-rw-   0        0        0     2743 2024-05-11 03:54:04.000000 pynapse-0.2.0/Pynapse/main.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:55:43.750711 pynapse-0.2.0/Pynapse.egg-info/
+-rw-rw-rw-   0        0        0       76 2024-05-11 03:55:43.000000 pynapse-0.2.0/Pynapse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-11 03:55:43.000000 pynapse-0.2.0/Pynapse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 03:55:43.000000 pynapse-0.2.0/Pynapse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-11 03:55:43.000000 pynapse-0.2.0/Pynapse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-11 03:55:43.000000 pynapse-0.2.0/Pynapse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-11 03:19:58.000000 pynapse-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-11 03:55:43.753703 pynapse-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      179 2024-05-11 03:22:02.000000 pynapse-0.2.0/setup.py
```

### Comparing `pynapse-0.1.0/Pynapse/main.py` & `pynapse-0.2.0/Pynapse/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,23 @@
 
             #update weights and biases
             for layer in self.layers:
                 if hasattr(layer, 'weights'):
                     layer.weights -= lr * layer.dweights
                     layer.biases -= lr * layer.dbiases
 
+class Bin_Round:
+    def Bin_Round(X):
+        if X >= 0.5:
+            return 1
+        elif X < 0.5:
+            return 0
+        else:
+            return 2
+
 class Net_Save:
     def save(file_name, dense_list):
         data = {}
         for i, dense in enumerate(dense_list):
             if hasattr(dense, 'weights'):
                 data[f'dense_{i}_weights'] = dense.weights.tolist()
                 data[f'dense_{i}_biases'] = dense.biases.tolist()
```

