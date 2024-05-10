# Comparing `tmp/dem_roughness_calculator-1.1.0.tar.gz` & `tmp/dem_roughness_calculator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dem_roughness_calculator-1.1.0.tar", last modified: Thu May  9 14:48:39 2024, max compression
+gzip compressed data, was "dem_roughness_calculator-1.2.0.tar", last modified: Fri May 10 23:32:53 2024, max compression
```

## Comparing `dem_roughness_calculator-1.1.0.tar` & `dem_roughness_calculator-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:39.003421 dem_roughness_calculator-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-09 14:48:39.003421 dem_roughness_calculator-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:39.003421 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-09 14:48:38.000000 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-09 14:48:38.000000 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:48:38.000000 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-09 14:48:38.000000 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 14:48:38.000000 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-09 14:48:38.000000 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:38.999421 dem_roughness_calculator-1.1.0/roughness_calculator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:38.999421 dem_roughness_calculator-1.1.0/roughness_calculator/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/classes/processing_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    21398 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/log_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:38.999421 dem_roughness_calculator-1.1.0/roughness_calculator/old_entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/old_entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/old_entry_points/demcli.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/old_entry_points/demgui.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:48:39.003421 dem_roughness_calculator-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:39.003421 dem_roughness_calculator-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-10 23:32:53.000000 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-10 23:32:53.000000 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:32:53.000000 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-10 23:32:53.000000 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-10 23:32:53.000000 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 23:32:53.000000 dem_roughness_calculator-1.2.0/dem_roughness_calculator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.084403 dem_roughness_calculator-1.2.0/roughness_calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.084403 dem_roughness_calculator-1.2.0/roughness_calculator/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17276 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/roughness_calculator/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/encapsulating_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/header_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui/preview_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/log_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/roughness_calculator/old_entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/old_entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/old_entry_points/demcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/roughness_calculator/old_entry_points/demgui.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:53.088403 dem_roughness_calculator-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-10 23:32:45.000000 dem_roughness_calculator-1.2.0/tests/test_application_driver.py
```

### Comparing `dem_roughness_calculator-1.1.0/README.md` & `dem_roughness_calculator-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -93,8 +93,8 @@
 
 ## Contributing
 
 We welcome contributions! If you have suggestions or want to report bugs, please use the [Issues](https://github.com/lbatschelet/dem-roughness-calculator/issues) section of this repository.
 
 ## License
 
-This project is licensed under the GPL-3.0 License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `dem_roughness_calculator-1.1.0/roughness_calculator/classes/application_driver.py` & `dem_roughness_calculator-1.2.0/roughness_calculator/classes/application_driver.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,89 +1,54 @@
 """
 application_driver.py
 ---------------------
-Version: 1.1.0
+Version: 1.2.0
 Author: Lukas Batschelet
-Date: 09.05.2024
+Date: 11.05.2024
 ---------------------
 This module contains the ApplicationDriver class which is responsible for running the application.
 It acts as a sort of interface between the calling User Interface (UI) and the GeoTIFFProcessor class.
 This enables the separation of concerns and allows for easier testing and maintenance of the code.
 (i.e. the UI does not need to know how the processing is done, it just needs to know how to call the processing.)
 """
 import datetime
 import logging
 import os
-from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import rasterio
 from PIL import Image
 
+from .defaults import Defaults
 from .geo_tiff_processor import GeoTIFFProcessor
 from .processing_parameters import ProcessingParameters
-from ..log_config import setup_logging
-
-# Ensure the logger is set up (optional if you know `log_config.py` is already imported elsewhere)
-setup_logging()
 
 logger = logging.getLogger(__name__)
 
 
-def check_positive_number(value: Union[int, float], parameter_name: str) -> float:
-    """
-    Validates that the given parameter is a positive number.
-
-    This function attempts to convert the input value to a float and checks if it is a positive number.
-    If the value is not a positive number, it raises a ValueError with a descriptive error message.
-    If the value is a positive number, it logs a confirmation message and returns the value.
-
-    Args:
-        value (Union[int, float]): The value to be checked.
-        parameter_name (str): The name of the parameter, used in error messages.
-
-    Returns:
-        float: The validated value, guaranteed to be a positive number.
-
-    Raises:
-        ValueError: If the value is not a positive number or cannot be converted to a float.
-    """
-    try:
-        # Attempt to convert the value to a float
-        value = float(value)
-        # If the value is not a positive number, raise a ValueError
-        if value <= 0:
-            raise ValueError(f"{parameter_name} must be a positive number, got {value}.")
-    except ValueError:
-        # If the value cannot be converted to a float, raise a ValueError
-        raise ValueError(f"{parameter_name} must be a positive number, got {value}.")
-    # If the value is a positive number, log a confirmation message
-    logging.info(f"Valid {parameter_name}: {value}")
-
-    return value
-
-
 class ApplicationDriver:
     def __init__(self, params: ProcessingParameters):
         """
         Initializes the ApplicationDriver with necessary parameters for processing a GeoTIFF file.
 
         Args:
             params (ProcessingParameters): The processing parameters for the ApplicationDriver.
 
         Raises:
             FileNotFoundError: If the input path or output directory is not valid.
         """
 
+        self.params = params
+
         self.input_path = params.input_path  # Store the path to the input GeoTIFF file
         self.output_dir = params.output_dir  # Store the path to the output directory if provided
 
         # Attempt to create an output filename if an output directory is provided
-        self.output_path = self.create_output_filename() if params.output_dir else None
+        self.output_path = ApplicationDriver.create_output_filename(params, include_path=True) if params.output_dir else None
 
         # Store additional processing parameters
         self.window_size = params.window_size
         self.band_number = params.band_number
         self.high_value_threshold = params.high_value_threshold
         self.category_thresholds = params.category_thresholds
 
@@ -119,15 +84,15 @@
 
         # Otherwise, generate a preview of the processed data
         else:
             self.produce_preview()
 
         logging.info("Processing completed.")
 
-    def produce_preview(self, nodata_value: int = -9999) -> None:
+    def produce_preview(self, nodata_value: int = Defaults.NODATA_VALUE) -> None:
         """
         Generates a preview image from the processed data stored in self.processed_data.
         This method avoids re-reading the data from file, making it more efficient.
         Uses pseudo-color to represent the data visually, ensuring nodata values are transparent.
 
         Args:
             nodata_value (int, optional): The value representing 'no data' in the dataset. Defaults to -9999.
@@ -171,15 +136,18 @@
             logging.info("Preview generated successfully.")
         except Exception as e:
             logging.error(f"Failed to produce preview: {str(e)}")
             self.preview = None
             # Raise a new error, preserving the original traceback
             raise RuntimeError("Failed to produce preview due to an error.") from e
 
-    def save_processed_data(self, output_path: str, nodata: int = -9999, dtype: str = 'float32') -> None:
+    def save_processed_data(self,
+                            output_path: str,
+                            nodata: int = Defaults.NODATA_VALUE,
+                            dtype: str = Defaults.DTYPE) -> None:
         """
         Saves the processed data to a GeoTIFF file using the stored profile.
 
         Args:
             output_path (str): The path where the processed data will be saved.
             nodata (int, optional): The value representing 'no data' in the dataset. Defaults to -9999.
             dtype (str, optional): The data type of the output GeoTIFF file. Defaults to 'float32'.
@@ -191,43 +159,66 @@
         if self.processed_data is None or self.processor.profile is None:
             logging.error("Processed data or profile is not available for saving.")
             raise ValueError("Processed data or profile is missing.")
 
         # Update the profile with the provided data type and nodata value
         self.processor.profile.update(dtype=dtype, nodata=nodata)
 
+        # Calculate the new pixel size, width, and height based on the window size
+        pixel_size = self.window_size
+        width = int((self.processor.profile['width'] * self.processor.profile['transform'][0]) / pixel_size)
+        height = int((self.processor.profile['height'] * abs(self.processor.profile['transform'][4])) / pixel_size)
+
+        # Update the transform, width, and height in the profile
+        self.processor.profile['transform'] = rasterio.Affine(pixel_size, 0, self.processor.profile['transform'][2], 0, -pixel_size, self.processor.profile['transform'][5])
+        self.processor.profile['width'] = width
+        self.processor.profile['height'] = height
+
         # Open the output path as a new GeoTIFF file in write mode
         with rasterio.open(output_path, 'w', **self.processor.profile) as dst:
             # Write the processed data to the first band of the GeoTIFF file
             dst.write(self.processed_data, 1)
 
         logging.info(f"Processed data saved to {output_path}")
 
-    def create_output_filename(self) -> str:
+    @staticmethod
+    def create_output_filename(params: ProcessingParameters, include_path: bool = True) -> str:
         """
         Generates a filename based on the input file, current date, and processing parameters.
 
-        The filename is generated in the following format: YYYYMMDD_basename_Surface-Roughness_windowSize-meter.tif
+        The filename is generated in the following format: YYYYMMDD_basename_Surface-Roughness_windowSize-meter_threshold1_threshold2_...
+
+        Args:
+            params (ProcessingParameters): The processing parameters.
+            include_path (bool): Whether to include the path in the filename.
 
         Returns:
-            str: The generated filename with the full path.
+            str: The generated filename with the full path if include_path is True, otherwise just the filename.
         """
         # Extract the base name from the input path (excluding the extension)
-        base_name = os.path.splitext(os.path.basename(self.input_path))[0]
+        base_name = os.path.splitext(os.path.basename(params.input_path))[0]
 
         # Get the current date in the format YYYYMMDD
         current_date = datetime.datetime.now().strftime("%Y%m%d")
 
-        # Construct the new filename using the current date, base name, and window size
-        new_filename = f"{current_date}_{base_name}_Surface-Roughness_{self.window_size}-meter.tif"
-
-        # Join the output directory path with the new filename to get the full path
-        full_path = os.path.join(self.output_dir, new_filename)
-
-        return full_path
+        # Convert the category thresholds to a string with the format threshold1_threshold2_...
+        # If category_thresholds is None, use an empty string
+        thresholds_str = ""
+        if params.category_thresholds is not None:
+            thresholds_str = "_" + "_".join(str(threshold) for threshold in params.category_thresholds)
+
+        # Construct the new filename using the current date, base name, window size, and category thresholds
+        new_filename = f"{current_date}_{base_name}_Surface-Roughness_{params.window_size}-meter{thresholds_str}.tif"
+
+        if include_path:
+            # Join the output directory path with the new filename to get the full path
+            full_path = os.path.join(os.path.dirname(params.input_path), new_filename)
+            return full_path
+        else:
+            return new_filename
 
     def get_preview(self) -> Image:
         """
         Retrieves the generated preview if available.
 
         This method checks if a preview image has been generated and is available.
         If the preview is available, it is returned. If not, an error message is logged and a RuntimeError is raised.
```

### Comparing `dem_roughness_calculator-1.1.0/roughness_calculator/classes/geo_tiff_processor.py` & `dem_roughness_calculator-1.2.0/roughness_calculator/classes/geo_tiff_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """
 geo_tiff_processor.py
 ---------------------
-Version: 1.1.0
+Version: 1.2.0
 Author: Lukas Batschelet
-Date: 09.05.2024
+Date: 11.05.2024
 ---------------------
 This module contains the GeoTIFFProcessor class which is responsible for processing GeoTIFF files.
 It provides methods for loading, processing, and saving GeoTIFF files.
 Until now, only a method to calculate the roughness of a GeoTIFF file has been implemented.
 """
+import logging
+from typing import Optional, List, Tuple
+
 import numpy as np
 import rasterio
-import logging
 
+from .defaults import Defaults
 from .processing_parameters import ProcessingParameters
-from ..log_config import setup_logging
-from typing import Optional, List, Tuple
-
-# Ensure the logger is set up (optional if you know `log_config.py` is already imported elsewhere)
-setup_logging()
 
 logger = logging.getLogger(__name__)
 
 
 class GeoTIFFProcessor:
     """
     Main class in this module, responsible for processing GeoTIFF files.
@@ -33,33 +31,37 @@
         band_number (int): The band number to be processed. Default 1.
         high_value_threshold (float): The threshold for high values to be filtered out. Default 10.0.
         category_thresholds (Optional[List[float]]): The thresholds for categorizing the roughness values.
         dataset (Optional[rasterio.DatasetReader]): The rasterio dataset object representing the GeoTIFF file.
         processed_data (Optional[np.ndarray]): The processed data.
         profile (Optional[Dict]): The profile of the GeoTIFF file.
     """
+
     def __init__(self, params: ProcessingParameters) -> None:
         """
         Initializes the GeoTIFFProcessor with the given parameters.
 
         Args:
             params (ProcessingParameters): The processing parameters for the GeoTIFFProcessor.
         """
+        logger.info("Initializing GeoTIFFProcessor...")
         # Store the input parameters
         self.input_path = params.input_path
         self.window_size = params.window_size
         self.band_number = params.band_number
         self.high_value_threshold = params.high_value_threshold
         self.category_thresholds = params.category_thresholds
 
         # Initialize the dataset, processed_data, and profile attributes to None
         self.dataset = None
         self.processed_data = None
         self.profile = None
 
+        logger.info(f"GeoTIFFProcessor initialized with parameters: {params}")
+
     def process_tiff(self) -> np.ndarray:
         """
         Main method for processing the GeoTIFF file.
         Returns the processed data instead of saving it directly.
 
         This method loads the GeoTIFF file, logs its metadata, reads the specified band, calculates the roughness,
         applies nodata values, filters out high values, and applies thresholds if they are defined.
@@ -67,14 +69,15 @@
 
         Returns:
             np.ndarray: The processed data.
 
         Raises:
             RuntimeError: If the TIFF dataset could not be opened, or an error occurred during processing.
         """
+        logger.info("Processing GeoTIFF file...")
         try:
             # Load the GeoTIFF file
             self.load_tiff()
             # Raise an error if the dataset could not be opened
             if not self.dataset:
                 raise RuntimeError("TIFF dataset could not be opened.")
 
@@ -240,24 +243,24 @@
         try:
             with rasterio.open(self.input_path) as src:
                 logger.info(f"GeoTIFF metadata: {src.meta}")
         except rasterio.errors.RasterioIOError as e:
             logger.error(f"Failed to open GeoTIFF: {e}")
             raise ValueError(f"Invalid GeoTIFF file: {self.input_path}")
 
-    def apply_filter(self, roughness: np.ndarray, nodata_value: int = -9999) -> np.ndarray:
+    def apply_filter(self, roughness: np.ndarray, nodata_value: int = Defaults.NODATA_VALUE) -> np.ndarray:
         """
         Filters out high values from the roughness array.
 
         This method replaces values in the roughness array that are greater than the high value
         threshold with a nodata value.
 
         Args:
             roughness (np.ndarray): The roughness array.
-            nodata_value (int, optional): The value to replace high values with. Defaults to -9999.
+            nodata_value (int, optional): The value to replace high values with.
 
         Returns:
             np.ndarray: The roughness array with high values replaced by the nodata value.
 
         Raises:
             ValueError: If no roughness data is provided.
         """
@@ -266,15 +269,15 @@
             raise ValueError("Roughness data is required for filtering.")
 
         roughness[roughness > self.high_value_threshold] = nodata_value
         logging.info("High values filtered from the roughness data.")
 
         return roughness
 
-    def apply_nodata(self, roughness: np.ndarray, nodata_value: int = -9999) -> np.ndarray:
+    def apply_nodata(self, roughness: np.ndarray, nodata_value: int = Defaults.NODATA_VALUE) -> np.ndarray:
         """
         Applies nodata value and filters out zero values from the roughness array.
 
         This method replaces zero values in the roughness array with a nodata value.
 
         Args:
             roughness (np.ndarray): The roughness array.
@@ -325,21 +328,21 @@
             # Return the pixel size
             return pixel_size
         except AttributeError as e:
             # Log the error and raise the original exception
             logging.error("Error accessing transform of the dataset: " + str(e))
             raise
 
-    def apply_thresholds(self, data: np.ndarray, nodata_value: int = -9999) -> np.ndarray:
+    def apply_thresholds(self, data: np.ndarray, nodata_value: int = Defaults.NODATA_VALUE) -> np.ndarray:
         """
         Applies thresholds to the data array.
 
         This method replaces values in the data array that are within certain ranges defined by the category thresholds
-        with the corresponding threshold value. Values greater than the highest threshold and less than or equal to the
-        high value threshold are replaced with the high value threshold.
+        with the corresponding category number. Values greater than or equal to the highest threshold and less than or
+        equal to the high value threshold are replaced with the highest category number.
 
         Args:
             data (np.ndarray): The data array.
             nodata_value (int, optional): The value to replace nodata values with. Defaults to -9999.
 
         Returns:
             np.ndarray: The data array with values replaced based on the thresholds.
@@ -362,20 +365,20 @@
         # Initialize the categorized data array with nodata values
         categorized_data = np.full(data.shape, nodata_value, dtype=data.dtype)
 
         # Loop over the category thresholds
         for i, threshold in enumerate(self.category_thresholds):
             # Create a mask for values within the current threshold range
             if i == 0:
-                mask = (data > 0) & (data <= threshold) & valid_mask
+                mask = (data >= 0) & (data < threshold) & valid_mask
             else:
-                mask = (data > self.category_thresholds[i - 1]) & (data <= threshold) & valid_mask
-            # Replace values within the current threshold range with the threshold value
-            categorized_data[mask] = threshold
+                mask = (data >= self.category_thresholds[i - 1]) & (data < threshold) & valid_mask
+            # Replace values within the current threshold range with the category number
+            categorized_data[mask] = i
 
         # Create a mask for values within the high value range
-        high_value_mask = (data > self.category_thresholds[-1]) & (data <= self.high_value_threshold) & valid_mask
-        # Replace values within the high value range with the high value threshold
-        categorized_data[high_value_mask] = self.high_value_threshold
+        high_value_mask = (data >= self.category_thresholds[-1]) & (data <= self.high_value_threshold) & valid_mask
+        # Replace values within the high value range with the highest category number
+        categorized_data[high_value_mask] = len(self.category_thresholds)
 
         logging.info("Data categorized based on thresholds.")
         return categorized_data
```

### Comparing `dem_roughness_calculator-1.1.0/roughness_calculator/classes/processing_parameters.py` & `dem_roughness_calculator-1.2.0/roughness_calculator/classes/processing_parameters.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,33 @@
 """
 processing_parameters.py
 ---
-Version: 1.1.0
+Version: 1.2.0
 Author: Lukas Batschelet
-Date: 09.05.2024
+Date: 11.05.2024
 ---
 Class to encapsulate the processing parameters for the surface roughness calculator application.
 The used dataclass decorator is a Python 3.7 feature that allows for the creation of classes with
 attributes and methods without the need for boilerplate code. The dataclass decorator automatically
 generates special methods like __init__(), __repr__(), and __eq__() based on the attributes defined
 in the class.
 """
 
-from dataclasses import dataclass, field
+import logging
 import os
+from dataclasses import dataclass, field
 from typing import Optional, List
 
-import logging
-
 import rasterio
 
-from ..log_config import setup_logging
-
-setup_logging()
+from .defaults import Defaults
 
 logger = logging.getLogger(__name__)
 
 
-class Defaults:
-    """Constants for default values used in processing parameters."""
-    OUTPUT_DIR = None
-    WINDOW_SIZE = 1.0
-    BAND_NUMBER = 1
-    HIGH_VALUE_THRESHOLD = 10.0
-    CATEGORY_THRESHOLDS = None
-
-
 @dataclass
 class ProcessingParameters:
     """
     A class to encapsulate the processing parameters for an application,
     ensuring all parameters are validated and converted upon instantiation.
 
     Attributes:
@@ -47,27 +35,31 @@
         output_dir (Optional[str]): The directory where the output should be saved. Optional.
         window_size (float): The size of the window to use for processing. Defaults to 1.0.
         band_number (int): The specific band to process. Defaults to 1.
         high_value_threshold (float): Threshold for identifying high values. Defaults to 10.0.
         category_thresholds (Optional[List[float]]): List of thresholds for categorizing data. Optional.
     """
     input_path: str
-    output_dir: Optional[str] = None
+    output_dir: Optional[str] = field(default_factory=lambda: Defaults.OUTPUT_DIR)
     window_size: float = field(default_factory=lambda: Defaults.WINDOW_SIZE)
     band_number: int = field(default_factory=lambda: Defaults.BAND_NUMBER)
     high_value_threshold: float = field(default_factory=lambda: Defaults.HIGH_VALUE_THRESHOLD)
-    category_thresholds: Optional[List[float]] = None
+    category_thresholds: Optional[List[float]] = field(default_factory=lambda: Defaults.CATEGORY_THRESHOLDS)
 
     def __post_init__(self):
+        logger.info("Initializing ProcessingParameters...")
+
         # Validate input_path with updated method that raises exceptions
         self.validate_input_path(self.input_path)
 
         # Validate output_dir if provided
         if self.output_dir:
             self.validate_output_dir(self.output_dir)
+        else:
+            logger.info("No output directory provided.")
 
             # Validate band_number
         self.validate_band_number(self.input_path, self.band_number)
 
         if self.window_size <= 0:
             raise ValueError("Window size must be positive.")
         if self.high_value_threshold <= 0:
@@ -93,83 +85,133 @@
         category_thresholds = cls.convert_to_float_list(params.get('category_thresholds', Defaults.CATEGORY_THRESHOLDS))
 
         # Construct and return an instance with validated and converted parameters
         return cls(input_path, output_dir, window_size, band_number, high_value_threshold, category_thresholds)
 
     @staticmethod
     def validate_input_path(path: str) -> bool:
-        """Validates that the input path is a file, exists, and is a GeoTIFF."""
+        """
+        Validates that the input path is a valid GeoTIFF file.
+        :param path: Path to the input file
+        :return: bool indicating if the input path is valid
+        """
+        logger.debug("Validating input path...")
         if not os.path.exists(path):
             raise FileNotFoundError(f"The input path {path} does not exist.")
         if not os.path.isfile(path):
             raise ValueError(f"The input path {path} is not a file.")
         if not ProcessingParameters.is_tiff_file(path):
             raise ValueError(f"The input file {path} is not a GeoTIFF.")
+        logger.info(f"Input path {path} is a valid GeoTIFF.")
         return True
 
     @staticmethod
     def is_tiff_file(filepath: str) -> bool:
         """
-        Checks if the file at the given path is a TIFF file by reading the first 4 bytes of the file.
-
-        This method reads the magic number to determine if it's a TIFF file and logs accordingly.
+        Checks if the file at the given path is a valid GeoTIFF file.
+        :param filepath: Path to the file to check
+        :return: bool indicating if the file is a valid GeoTIFF
         """
+        logger.debug(f"Checking if file is a valid GeoTIFF: {filepath}")
         try:
             with open(filepath, 'rb') as file:
                 magic_number = file.read(4)
             if magic_number not in (b'II\x2A\x00', b'MM\x00\x2A'):
                 logger.info("File does not have a valid TIFF magic number.")
                 return False
             # Confirm with rasterio open
             with rasterio.open(filepath) as src:
                 logger.info(f"TIFF file opened successfully with rasterio: {src.meta}")
+            logger.info("File is a valid GeoTIFF.")
             return True
         except (IOError, rasterio.errors.RasterioIOError) as e:
             logger.error(f"Failed to open or process TIFF file: {e}")
             return False
 
     @staticmethod
     def validate_output_dir(path: str):
-        """Checks if the output directory exists and is a directory."""
+        """
+        Validates that the output directory exists and is a directory.
+        :param path: Path to the output directory
+        :return: None
+        """
+        logger.debug("Validating output directory...")
         if not os.path.exists(path):
             raise FileNotFoundError(f"The output directory {path} does not exist.")
         if not os.path.isdir(path):
             raise ValueError(f"The output path {path} is not a directory.")
+        logger.info(f"Output directory {path} is valid.")
 
     @staticmethod
     def convert_to_float_list(value_str: Optional[str]) -> Optional[List[float]]:
-        """Converts a comma-separated string of numbers into a list of floats."""
+        """
+        Converts a comma-separated string of values to a list of floats.
+        :param value_str: Input string of comma-separated values
+        :return: List of floats or None if the input is None
+        """
+        logger.debug("Converting string to float list...")
         if not value_str:
+            logger.info("No category thresholds provided.")
             return None
+        logger.info("String converted to float list.")
         return [float(x.strip()) for x in value_str.split(',')]
 
     @staticmethod
     def sort_thresholds(thresholds: List[float]) -> List[float]:
+        """
+        Sorts the category thresholds and logs a warning if they were not initially sorted.
+        :param thresholds: List of thresholds to sort
+        :return: Sorted list of thresholds
+        """
+        logger.debug("Sorting category thresholds...")
         sorted_thresholds = sorted(thresholds)
         if sorted_thresholds != thresholds:
             logger.warning("Category thresholds were not initially sorted.")
             logger.info(f"Sorted thresholds: {sorted_thresholds}")
+        logger.info("Category thresholds are sorted.")
         return sorted_thresholds
 
     @staticmethod
     def check_max_threshold(thresholds: List[float], high_value_threshold: float) -> List[float]:
+        """
+        Removes thresholds that exceed the high value threshold and logs a warning.
+        :param thresholds: List of thresholds to check
+        :param high_value_threshold: singular threshold to compare against
+        :return: List of valid thresholds
+        """
+        logger.debug("Checking max thresholds...")
         valid_thresholds = [t for t in thresholds if t < high_value_threshold]
         if len(valid_thresholds) != len(thresholds):
             logger.warning("Some thresholds exceeded the high value threshold and were removed.")
             logger.info(f"Valid thresholds: {valid_thresholds}")
+        logger.info("All thresholds are below the high value threshold.")
         return valid_thresholds
 
     @staticmethod
     def check_positive_thresholds(thresholds: List[float]) -> List[float]:
+        """
+        Removes non-positive thresholds from the list and logs a warning.
+        :param thresholds: List of thresholds to check if positive
+        :return: List of positive thresholds
+        """
+        logger.debug("Checking positive thresholds...")
         valid_thresholds = [t for t in thresholds if t > 0]
         if len(valid_thresholds) != len(thresholds):
             logger.warning("Non-positive thresholds were removed.")
             logger.info(f"Valid thresholds: {valid_thresholds}")
+        logger.info("All thresholds are positive.")
         return valid_thresholds
 
     @staticmethod
     def validate_band_number(path: str, band_number: int) -> bool:
-        """Validates that the band number is within the valid range for the GeoTIFF file."""
+        """
+        Validates that the band number is within the valid range for the GeoTIFF file.
+        :param path: Path to the GeoTIFF file
+        :param band_number: Band number to validate
+        :return: bool indicating if the band number is valid
+        """
+        logger.debug("Validating band number...")
         with rasterio.open(path) as src:
             if band_number < 1 or band_number > src.count:
                 raise ValueError(f"The band number {band_number} is not valid for the GeoTIFF file {path}.")
+        logger.info(f"Band number {band_number} is valid for the GeoTIFF file {path}.")
         return True
```

### Comparing `dem_roughness_calculator-1.1.0/roughness_calculator/cli_main.py` & `dem_roughness_calculator-1.2.0/roughness_calculator/cli_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """
 cli_main.py
 -----------
-Version: 1.1.0
+Version: 1.2.0
 Author: Lukas Batschelet
-Date: 09.05.2024
+Date: 11.05.2024
 -----------
 """
 import argparse
 import logging
 import sys
 
 from roughness_calculator.classes.application_driver import ApplicationDriver
 from roughness_calculator.classes.processing_parameters import ProcessingParameters
-from .log_config import setup_logging
-
-# Ensure the logger is set up (optional if you know `log_config.py` is already imported elsewhere)
-setup_logging()
 
 logger = logging.getLogger(__name__)
 
 
 class CLIMain:
     def __init__(self) -> None:
         """
@@ -94,15 +90,15 @@
 
     This method initializes the CLIMain class and runs it.
 
     Returns:
         None
     """
     # Initialize the CLIMain class
-    cli = CLIMain()
+    cli_main = CLIMain()
 
     # Run the CLIMain class
-    cli.run()
+    cli_main.run()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `dem_roughness_calculator-1.1.0/setup.py` & `dem_roughness_calculator-1.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements file
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='dem-roughness-calculator',
-    version='1.1.0',
+    version='1.2.0',
     packages=find_packages(),  # Automatically find all packages in the directory
     url='https://github.com/lbatschelet/dem-roughness-calculator',
     license='GPL-3.0',
     author='lbatschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     install_requires=requirements,  # Install dependencies from requirements.txt
     python_requires='>=3.12',  # Specify Python version requirement
```

