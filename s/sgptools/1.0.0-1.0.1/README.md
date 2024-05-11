# Comparing `tmp/sgptools-1.0.0.tar.gz` & `tmp/sgptools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgptools-1.0.0.tar", last modified: Wed May  8 22:21:37 2024, max compression
+gzip compressed data, was "sgptools-1.0.1.tar", last modified: Sat May 11 03:02:35 2024, max compression
```

## Comparing `sgptools-1.0.0.tar` & `sgptools-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxr-x   0 kalvik    (1000) kalvik    (1000)        0 2024-05-08 22:21:37.500016 sgptools-1.0.0/
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)      313 2024-05-08 22:21:37.500016 sgptools-1.0.0/PKG-INFO
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)     4448 2024-05-08 22:07:31.000000 sgptools-1.0.0/README.md
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)       38 2024-05-08 22:21:37.500016 sgptools-1.0.0/setup.cfg
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)      408 2024-05-08 22:21:14.000000 sgptools-1.0.0/setup.py
-drwxrwxr-x   0 kalvik    (1000) kalvik    (1000)        0 2024-05-08 22:21:37.500016 sgptools-1.0.0/sgptools/
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)       69 2024-04-18 20:59:17.000000 sgptools-1.0.0/sgptools/__init__.py
-drwxrwxr-x   0 kalvik    (1000) kalvik    (1000)        0 2024-05-08 22:21:37.500016 sgptools-1.0.0/sgptools/kernels/
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)        0 2024-05-07 21:03:14.000000 sgptools-1.0.0/sgptools/kernels/__init__.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)     6709 2024-05-08 16:11:42.000000 sgptools-1.0.0/sgptools/kernels/neural_kernel.py
-drwxrwxr-x   0 kalvik    (1000) kalvik    (1000)        0 2024-05-08 22:21:37.500016 sgptools-1.0.0/sgptools/models/
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)      682 2024-05-08 16:53:16.000000 sgptools-1.0.0/sgptools/models/__init__.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)     3640 2024-05-07 18:13:24.000000 sgptools-1.0.0/sgptools/models/bo.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)     8138 2024-05-07 18:14:16.000000 sgptools-1.0.0/sgptools/models/cma_es.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)     2940 2024-05-08 15:52:49.000000 sgptools-1.0.0/sgptools/models/continuous_sgp.py
-drwxrwxr-x   0 kalvik    (1000) kalvik    (1000)        0 2024-05-08 22:21:37.500016 sgptools-1.0.0/sgptools/models/core/
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)      482 2024-05-08 16:13:46.000000 sgptools-1.0.0/sgptools/models/core/__init__.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)     3492 2024-05-08 16:11:22.000000 sgptools-1.0.0/sgptools/models/core/augmented_gpr.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)     7180 2024-05-08 16:11:27.000000 sgptools-1.0.0/sgptools/models/core/augmented_sgpr.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)    11466 2024-05-08 16:11:31.000000 sgptools-1.0.0/sgptools/models/core/osgpr.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)    16341 2024-05-08 16:54:33.000000 sgptools-1.0.0/sgptools/models/core/transformations.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)     4870 2024-05-07 16:30:06.000000 sgptools-1.0.0/sgptools/models/greedy_mi.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)     4462 2024-05-08 13:56:51.000000 sgptools-1.0.0/sgptools/models/greedy_sgp.py
-drwxrwxr-x   0 kalvik    (1000) kalvik    (1000)        0 2024-05-08 22:21:37.500016 sgptools-1.0.0/sgptools/utils/
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)      376 2024-05-08 17:10:26.000000 sgptools-1.0.0/sgptools/utils/__init__.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)    11617 2024-04-26 19:18:26.000000 sgptools-1.0.0/sgptools/utils/data.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)     6292 2024-05-08 14:12:30.000000 sgptools-1.0.0/sgptools/utils/gpflow.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)     5806 2024-05-08 14:47:33.000000 sgptools-1.0.0/sgptools/utils/metrics.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)     4123 2024-05-08 15:18:40.000000 sgptools-1.0.0/sgptools/utils/misc.py
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)     5857 2024-05-08 15:28:38.000000 sgptools-1.0.0/sgptools/utils/tsp.py
-drwxrwxr-x   0 kalvik    (1000) kalvik    (1000)        0 2024-05-08 22:21:37.500016 sgptools-1.0.0/sgptools.egg-info/
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)      313 2024-05-08 22:21:37.000000 sgptools-1.0.0/sgptools.egg-info/PKG-INFO
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)      725 2024-05-08 22:21:37.000000 sgptools-1.0.0/sgptools.egg-info/SOURCES.txt
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)        1 2024-05-08 22:21:37.000000 sgptools-1.0.0/sgptools.egg-info/dependency_links.txt
--rw-rw-r--   0 kalvik    (1000) kalvik    (1000)        9 2024-05-08 22:21:37.000000 sgptools-1.0.0/sgptools.egg-info/top_level.txt
+drwxr-xr-x   0 kjakkala  (1000) kjakkala  (1000)        0 2024-05-11 03:02:35.005247 sgptools-1.0.1/
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)    11357 2024-05-11 00:28:24.000000 sgptools-1.0.1/LICENSE.txt
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)      320 2024-05-11 03:02:35.005247 sgptools-1.0.1/PKG-INFO
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     4949 2024-05-11 02:41:14.000000 sgptools-1.0.1/README.md
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)       38 2024-05-11 03:02:35.005247 sgptools-1.0.1/setup.cfg
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     1056 2024-05-11 02:56:05.000000 sgptools-1.0.1/setup.py
+drwxr-xr-x   0 kjakkala  (1000) kjakkala  (1000)        0 2024-05-11 03:02:35.005247 sgptools-1.0.1/sgptools/
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)      449 2024-05-11 02:56:14.000000 sgptools-1.0.1/sgptools/__init__.py
+drwxr-xr-x   0 kjakkala  (1000) kjakkala  (1000)        0 2024-05-11 03:02:35.005247 sgptools-1.0.1/sgptools/kernels/
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)        0 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/kernels/__init__.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     6709 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/kernels/neural_kernel.py
+drwxr-xr-x   0 kjakkala  (1000) kjakkala  (1000)        0 2024-05-11 03:02:35.005247 sgptools-1.0.1/sgptools/models/
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)      682 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/models/__init__.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     3640 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/models/bo.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     8138 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/models/cma_es.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     2940 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/models/continuous_sgp.py
+drwxr-xr-x   0 kjakkala  (1000) kjakkala  (1000)        0 2024-05-11 03:02:35.005247 sgptools-1.0.1/sgptools/models/core/
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)      482 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/models/core/__init__.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     3492 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/models/core/augmented_gpr.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     7180 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/models/core/augmented_sgpr.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)    11466 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/models/core/osgpr.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)    16341 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/models/core/transformations.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     4870 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/models/greedy_mi.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     4462 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/models/greedy_sgp.py
+drwxr-xr-x   0 kjakkala  (1000) kjakkala  (1000)        0 2024-05-11 03:02:35.005247 sgptools-1.0.1/sgptools/utils/
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)      376 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/utils/__init__.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)    11617 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/utils/data.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     6292 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/utils/gpflow.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     5806 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/utils/metrics.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     4123 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/utils/misc.py
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)     5857 2024-05-11 00:28:25.000000 sgptools-1.0.1/sgptools/utils/tsp.py
+drwxr-xr-x   0 kjakkala  (1000) kjakkala  (1000)        0 2024-05-11 03:02:35.005247 sgptools-1.0.1/sgptools.egg-info/
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)      320 2024-05-11 03:02:34.000000 sgptools-1.0.1/sgptools.egg-info/PKG-INFO
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)      768 2024-05-11 03:02:34.000000 sgptools-1.0.1/sgptools.egg-info/SOURCES.txt
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)        1 2024-05-11 03:02:34.000000 sgptools-1.0.1/sgptools.egg-info/dependency_links.txt
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)      255 2024-05-11 03:02:34.000000 sgptools-1.0.1/sgptools.egg-info/requires.txt
+-rw-r--r--   0 kjakkala  (1000) kjakkala  (1000)        9 2024-05-11 03:02:34.000000 sgptools-1.0.1/sgptools.egg-info/top_level.txt
```

### Comparing `sgptools-1.0.0/README.md` & `sgptools-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,45 @@
 <div style="text-align:left">
-<img width="472" src="static/SGP-Tools.png">
+<img width="472" src="docs/assets/SGP-Tools.png">
 </div>
 
 # SGP-based Optimization Tools
-Software suite for [Sensor Placement](https://itskalvik.com/publication/sgp-sp) (SP) and [Informative Path Planning](https://itskalvik.com/publication/sgp-ipp) (IPP)
+Software Suite for [Sensor Placement](https://itskalvik.com/publication/sgp-sp) (SP) and [Informative Path Planning](https://itskalvik.com/publication/sgp-ipp) (IPP). 
+
+The library includes python code for the following:
+- Greedy algorithm-based approaches
+- Bayesian optimization-based approaches
+- Genetic algorithm-based approaches
+- Sparse Gaussian process (SGP)-based approaches
 
 <p align="center">
-  <img alt="Light" src="static/point_sensing.gif" width="45%">
+  <img alt="Light" src="docs/assets/point_sensing.gif" width="45%">
 &nbsp; &nbsp; &nbsp; &nbsp;
-  <img alt="Dark" src="static/non-point_sensing.gif" width="45%">
+  <img alt="Dark" src="docs/assets/non-point_sensing.gif" width="45%">
 </p>
 
+## Installation
+The library is available as a ```pip``` package. To install the package, run the following command:
+
+```
+sudo apt-get install libhdf5-dev python3-pip -y
+python3 -m pip install sgptools
+```
+
+Installation from source:
+
+```
+sudo apt-get install libhdf5-dev python3-pip -y
+python3 -m pip install -r requirements.txt
+python3 -m pip install -e .
+```
+
+## Quick Start
+Please refer to the [demos](https://github.com/itskalvik/sgp-tools/tree/master/demos) folder for Jupyter notebooks demonstrating all the methods included in the library :smile:
+
 ## Method Summary
 [![Video Summary](https://res.cloudinary.com/marcomontalbano/image/upload/v1713536416/video_to_markdown/images/youtube--G-RKFa1vNHM-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://www.youtube.com/embed/G-RKFa1vNHM?si=PLmrmkCwXRj7mc4A "Video Summary")
 
 ## Codemap
 - `demos/`: Jupyter notebooks with code to demonstrate each method in the library
     - `IPP.ipynb`: SGP-based IPP (point, non-point, continuous sensing, distance constrained, and multi-robot)
     - `IPPBaselines.ipynb`: SGP-based IPP approach and baseline methods
@@ -44,25 +69,14 @@
 ## Datasets
 * The Intel lab temperature dataset can be downloaded from [here](http://db.csail.mit.edu/labdata/labdata.html)
 * The ROMS ocean salinity dataset can be downloaded from [here](https://oceanmodeling.ucsc.edu/ccsnrt/#txtOverview)
 * The Precipitation dataset can be downloaded from [here](http://research.jisao.washington.edu/data_sets/widmann/)
 * The US soil moisture dataset can be downloaded from [here](https://www.drought.gov/data-maps-tools/nasa-sport-lis-soil-moisture-products)
 * The US elevation dataset can be downloaded from [here](https://coast.noaa.gov/digitalcoast/)
 
-## Installation
-Run the following commands to install the package
-
-```
-sudo apt-get install libhdf5-dev netcdf-bin libnetcdf-dev python3-pip -y
-git clone https://github.com/itskalvik/sgp_tools.git
-cd sgp_tools
-python3 -m pip install -r requirements.txt
-python3 -m pip install -e .
-```
-
 ## About SGP-Tools
 Please consider citing the following papers if you use SGP-Tools in your academic work :smile:
 
 ```
 @misc{JakkalaA23SP,
 AUTHOR={Kalvik Jakkala and Srinivas Akella},
 TITLE={Efficient Sensor Placement from Regression with Sparse Gaussian Processes in Continuous and Discrete Spaces},
```

### Comparing `sgptools-1.0.0/sgptools/kernels/neural_kernel.py` & `sgptools-1.0.1/sgptools/kernels/neural_kernel.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/models/__init__.py` & `sgptools-1.0.1/sgptools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/models/bo.py` & `sgptools-1.0.1/sgptools/models/bo.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/models/cma_es.py` & `sgptools-1.0.1/sgptools/models/cma_es.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/models/continuous_sgp.py` & `sgptools-1.0.1/sgptools/models/continuous_sgp.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/models/core/augmented_gpr.py` & `sgptools-1.0.1/sgptools/models/core/augmented_gpr.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/models/core/augmented_sgpr.py` & `sgptools-1.0.1/sgptools/models/core/augmented_sgpr.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/models/core/osgpr.py` & `sgptools-1.0.1/sgptools/models/core/osgpr.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/models/core/transformations.py` & `sgptools-1.0.1/sgptools/models/core/transformations.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/models/greedy_mi.py` & `sgptools-1.0.1/sgptools/models/greedy_mi.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/models/greedy_sgp.py` & `sgptools-1.0.1/sgptools/models/greedy_sgp.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/utils/data.py` & `sgptools-1.0.1/sgptools/utils/data.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/utils/gpflow.py` & `sgptools-1.0.1/sgptools/utils/gpflow.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/utils/metrics.py` & `sgptools-1.0.1/sgptools/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/utils/misc.py` & `sgptools-1.0.1/sgptools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools/utils/tsp.py` & `sgptools-1.0.1/sgptools/utils/tsp.py`

 * *Files identical despite different names*

### Comparing `sgptools-1.0.0/sgptools.egg-info/SOURCES.txt` & `sgptools-1.0.1/sgptools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+LICENSE.txt
 README.md
 setup.py
 sgptools/__init__.py
 sgptools.egg-info/PKG-INFO
 sgptools.egg-info/SOURCES.txt
 sgptools.egg-info/dependency_links.txt
+sgptools.egg-info/requires.txt
 sgptools.egg-info/top_level.txt
 sgptools/kernels/__init__.py
 sgptools/kernels/neural_kernel.py
 sgptools/models/__init__.py
 sgptools/models/bo.py
 sgptools/models/cma_es.py
 sgptools/models/continuous_sgp.py
```

