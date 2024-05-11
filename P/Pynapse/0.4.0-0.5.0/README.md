# Comparing `tmp/pynapse-0.4.0.tar.gz` & `tmp/pynapse-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynapse-0.4.0.tar", last modified: Sat May 11 04:27:50 2024, max compression
+gzip compressed data, was "pynapse-0.5.0.tar", last modified: Sat May 11 04:30:25 2024, max compression
```

## Comparing `pynapse-0.4.0.tar` & `pynapse-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 04:27:50.824306 pynapse-0.4.0/
--rw-rw-rw-   0        0        0     1831 2024-05-11 04:27:50.822310 pynapse-0.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-11 04:27:50.776433 pynapse-0.4.0/Pynapse/
--rw-rw-rw-   0        0        0      180 2024-05-11 04:02:14.000000 pynapse-0.4.0/Pynapse/__init__.py
--rw-rw-rw-   0        0        0     2743 2024-05-11 03:54:04.000000 pynapse-0.4.0/Pynapse/main.py
-drwxrwxrwx   0        0        0        0 2024-05-11 04:27:50.818327 pynapse-0.4.0/Pynapse.egg-info/
--rw-rw-rw-   0        0        0     1831 2024-05-11 04:27:50.000000 pynapse-0.4.0/Pynapse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-11 04:27:50.000000 pynapse-0.4.0/Pynapse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 04:27:50.000000 pynapse-0.4.0/Pynapse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-11 04:27:50.000000 pynapse-0.4.0/Pynapse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-11 04:27:50.000000 pynapse-0.4.0/Pynapse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1710 2024-05-11 04:24:55.000000 pynapse-0.4.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-11 04:27:50.825302 pynapse-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      316 2024-05-11 04:27:36.000000 pynapse-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:30:25.456611 pynapse-0.5.0/
+-rw-rw-rw-   0        0        0     1835 2024-05-11 04:30:25.455614 pynapse-0.5.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 04:30:25.423797 pynapse-0.5.0/Pynapse/
+-rw-rw-rw-   0        0        0      180 2024-05-11 04:02:14.000000 pynapse-0.5.0/Pynapse/__init__.py
+-rw-rw-rw-   0        0        0     2743 2024-05-11 03:54:04.000000 pynapse-0.5.0/Pynapse/main.py
+drwxrwxrwx   0        0        0        0 2024-05-11 04:30:25.453636 pynapse-0.5.0/Pynapse.egg-info/
+-rw-rw-rw-   0        0        0     1835 2024-05-11 04:30:25.000000 pynapse-0.5.0/Pynapse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-11 04:30:25.000000 pynapse-0.5.0/Pynapse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 04:30:25.000000 pynapse-0.5.0/Pynapse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-11 04:30:25.000000 pynapse-0.5.0/Pynapse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-11 04:30:25.000000 pynapse-0.5.0/Pynapse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1714 2024-05-11 04:30:15.000000 pynapse-0.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-11 04:30:25.457608 pynapse-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      316 2024-05-11 04:29:34.000000 pynapse-0.5.0/setup.py
```

### Comparing `pynapse-0.4.0/PKG-INFO` & `pynapse-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: Pynapse
-Version: 0.4.0
-Description-Content-Type: text/markdown
-Requires-Dist: numpy
-
 # VERSION
 
 *MAJOR.MINOR.PATCH*
 
 # USAGE EXAMPLES
 
 ### VIDEO
@@ -45,8 +39,8 @@
 
 prediction = Bin_Round.Bin_Round(net.forward(np.array([[1,0]])))
 print(prediction)                                   # Round the output of the output of the output layer to binary 1 or 0    e.g. 1
 ```
 
 
 # WHY CALLED "Pynapse"
-#### This module has been called "Pynapse" gor Python and Synapse
+#### This module has been called "Pynapse" meaning Python and Synapse
```

### Comparing `pynapse-0.4.0/Pynapse/main.py` & `pynapse-0.5.0/Pynapse/main.py`

 * *Files identical despite different names*

### Comparing `pynapse-0.4.0/Pynapse.egg-info/PKG-INFO` & `pynapse-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pynapse
-Version: 0.4.0
+Version: 0.5.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 
 # VERSION
 
 *MAJOR.MINOR.PATCH*
 
@@ -45,8 +45,8 @@
 
 prediction = Bin_Round.Bin_Round(net.forward(np.array([[1,0]])))
 print(prediction)                                   # Round the output of the output of the output layer to binary 1 or 0    e.g. 1
 ```
 
 
 # WHY CALLED "Pynapse"
-#### This module has been called "Pynapse" gor Python and Synapse
+#### This module has been called "Pynapse" meaning Python and Synapse
```

### Comparing `pynapse-0.4.0/README.md` & `pynapse-0.5.0/Pynapse.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: Pynapse
+Version: 0.5.0
+Description-Content-Type: text/markdown
+Requires-Dist: numpy
+
 # VERSION
 
 *MAJOR.MINOR.PATCH*
 
 # USAGE EXAMPLES
 
 ### VIDEO
@@ -39,8 +45,8 @@
 
 prediction = Bin_Round.Bin_Round(net.forward(np.array([[1,0]])))
 print(prediction)                                   # Round the output of the output of the output layer to binary 1 or 0    e.g. 1
 ```
 
 
 # WHY CALLED "Pynapse"
-#### This module has been called "Pynapse" gor Python and Synapse
+#### This module has been called "Pynapse" meaning Python and Synapse
```

