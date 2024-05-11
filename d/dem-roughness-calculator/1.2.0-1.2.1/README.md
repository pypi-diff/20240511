# Comparing `tmp/dem_roughness_calculator-1.2.0.tar.gz` & `tmp/dem_roughness_calculator-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dem_roughness_calculator-1.2.0.tar", last modified: Fri May 10 23:32:53 2024, max compression
+gzip compressed data, was "dem_roughness_calculator-1.2.1.tar", last modified: Fri May 10 23:45:28 2024, max compression
```

## Comparing `dem_roughness_calculator-1.2.0.tar` & `dem_roughness_calculator-1.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-10 23:32:53.000000 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-10 23:32:53.000000 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:32:53.000000 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-10 23:32:53.000000 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-10 23:32:53.000000 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 23:32:53.000000 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.084403 dem_roughness_calculator-1.2.0/roughness_calculator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.084403 dem_roughness_calculator-1.2.0/roughness_calculator/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/classes/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    17276 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/classes/processing_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/roughness_calculator/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/encapsulating_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/footer_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/header_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/parameter_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/path_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/preview_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/log_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/roughness_calculator/old_entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/old_entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/old_entry_points/demcli.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/old_entry_points/demgui.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:45:28.400886 dem_roughness_calculator-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-10 23:45:28.400886 dem_roughness_calculator-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:45:28.400886 dem_roughness_calculator-1.2.1/dem_roughness_calculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-10 23:45:28.000000 dem_roughness_calculator-1.2.1/dem_roughness_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-10 23:45:28.000000 dem_roughness_calculator-1.2.1/dem_roughness_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:45:28.000000 dem_roughness_calculator-1.2.1/dem_roughness_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-10 23:45:28.000000 dem_roughness_calculator-1.2.1/dem_roughness_calculator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-10 23:45:28.000000 dem_roughness_calculator-1.2.1/dem_roughness_calculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 23:45:28.000000 dem_roughness_calculator-1.2.1/dem_roughness_calculator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:45:28.396886 dem_roughness_calculator-1.2.1/roughness_calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:45:28.396886 dem_roughness_calculator-1.2.1/roughness_calculator/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17276 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:45:28.396886 dem_roughness_calculator-1.2.1/roughness_calculator/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/gui/encapsulating_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/gui/header_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/gui/preview_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/log_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:45:28.396886 dem_roughness_calculator-1.2.1/roughness_calculator/old_entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/old_entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/old_entry_points/demcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/roughness_calculator/old_entry_points/demgui.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 23:45:28.400886 dem_roughness_calculator-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:45:28.400886 dem_roughness_calculator-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-10 23:45:20.000000 dem_roughness_calculator-1.2.1/tests/test_application_driver.py
```

### Comparing `dem_roughness_calculator-1.2.0/LICENSE` & `dem_roughness_calculator-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.0/PKG-INFO` & `dem_roughness_calculator-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dem-roughness-calculator
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/dem-roughness-calculator
 Author: lbatschelet
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dem_roughness_calculator-1.2.0/README.md` & `dem_roughness_calculator-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/PKG-INFO` & `dem_roughness_calculator-1.2.1/dem_roughness_calculator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dem-roughness-calculator
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/dem-roughness-calculator
 Author: lbatschelet
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/SOURCES.txt` & `dem_roughness_calculator-1.2.1/dem_roughness_calculator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.0/roughness_calculator/classes/application_driver.py` & `dem_roughness_calculator-1.2.1/roughness_calculator/classes/application_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 application_driver.py
 ---------------------
-Version: 1.2.0
+Version: 1.2.1
 Author: Lukas Batschelet
 Date: 11.05.2024
 ---------------------
 This module contains the ApplicationDriver class which is responsible for running the application.
 It acts as a sort of interface between the calling User Interface (UI) and the GeoTIFFProcessor class.
 This enables the separation of concerns and allows for easier testing and maintenance of the code.
 (i.e. the UI does not need to know how the processing is done, it just needs to know how to call the processing.)
```

### Comparing `dem_roughness_calculator-1.2.0/roughness_calculator/classes/defaults.py` & `dem_roughness_calculator-1.2.1/roughness_calculator/classes/defaults.py`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.0/roughness_calculator/classes/geo_tiff_processor.py` & `dem_roughness_calculator-1.2.1/roughness_calculator/classes/geo_tiff_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 geo_tiff_processor.py
 ---------------------
-Version: 1.2.0
+Version: 1.2.1
 Author: Lukas Batschelet
 Date: 11.05.2024
 ---------------------
 This module contains the GeoTIFFProcessor class which is responsible for processing GeoTIFF files.
 It provides methods for loading, processing, and saving GeoTIFF files.
 Until now, only a method to calculate the roughness of a GeoTIFF file has been implemented.
 """
```

### Comparing `dem_roughness_calculator-1.2.0/roughness_calculator/classes/processing_parameters.py` & `dem_roughness_calculator-1.2.1/roughness_calculator/classes/processing_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 processing_parameters.py
 ---
-Version: 1.2.0
+Version: 1.2.1
 Author: Lukas Batschelet
 Date: 11.05.2024
 ---
 Class to encapsulate the processing parameters for the surface roughness calculator application.
 The used dataclass decorator is a Python 3.7 feature that allows for the creation of classes with
 attributes and methods without the need for boilerplate code. The dataclass decorator automatically
 generates special methods like __init__(), __repr__(), and __eq__() based on the attributes defined
```

### Comparing `dem_roughness_calculator-1.2.0/roughness_calculator/cli_main.py` & `dem_roughness_calculator-1.2.1/roughness_calculator/cli_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 cli_main.py
 -----------
-Version: 1.2.0
+Version: 1.2.1
 Author: Lukas Batschelet
 Date: 11.05.2024
 -----------
 """
 import argparse
 import logging
 import sys
```

### Comparing `dem_roughness_calculator-1.2.0/roughness_calculator/gui/encapsulating_frame.py` & `dem_roughness_calculator-1.2.1/roughness_calculator/gui/encapsulating_frame.py`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.0/roughness_calculator/gui/footer_frame.py` & `dem_roughness_calculator-1.2.1/roughness_calculator/gui/footer_frame.py`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.0/roughness_calculator/gui/header_frame.py` & `dem_roughness_calculator-1.2.1/roughness_calculator/gui/header_frame.py`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.0/roughness_calculator/gui/parameter_input.py` & `dem_roughness_calculator-1.2.1/roughness_calculator/gui/parameter_input.py`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.0/roughness_calculator/gui/path_frame.py` & `dem_roughness_calculator-1.2.1/roughness_calculator/gui/path_frame.py`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.0/roughness_calculator/gui/preview_image.py` & `dem_roughness_calculator-1.2.1/roughness_calculator/gui/preview_image.py`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.2.0/roughness_calculator/gui_main.py` & `dem_roughness_calculator-1.2.1/roughness_calculator/gui_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 gui_main.py
 -----------
-Version: 1.2.0
+Version: 1.2.1
 Author: Lukas Batschelet
 Date: 11.05.2024
 -----------
 This module contains the main GUI class for the Surface Roughness Calculator application.
 """
 
 import logging
```

### Comparing `dem_roughness_calculator-1.2.0/roughness_calculator/log_config.py` & `dem_roughness_calculator-1.2.1/roughness_calculator/log_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 log_config.py
 -----------
-Version: 1.2.0
+Version: 1.2.1
 Author: Lukas Batschelet
 Date: 11.05.2024
 -----------
 This module sets up the logging for the application.
 """
 
 import logging
```

### Comparing `dem_roughness_calculator-1.2.0/setup.py` & `dem_roughness_calculator-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 # Read the contents of your requirements file
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='dem-roughness-calculator',
-    version='1.2.0',
+    version='1.2.1',
     packages=find_packages(),  # Automatically find all packages in the directory
     url='https://github.com/lbatschelet/dem-roughness-calculator',
     license='GPL-3.0',
     author='lbatschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     install_requires=requirements,  # Install dependencies from requirements.txt
     python_requires='>=3.12',  # Specify Python version requirement
     entry_points={
         'console_scripts': [
-            'surface-roughness=roughness_calculator.main:main',
+            'surface-roughness=main:main',
             'demgui=roughness_calculator.old_entry_points.demgui:main',
             'demcli=roughness_calculator.old_entry_points.demcli:main',
         ]
     },
     classifiers=[
         'Development Status :: 4 - Beta',  # Update as appropriate for your release cycle
         'Intended Audience :: Science/Research',
```

