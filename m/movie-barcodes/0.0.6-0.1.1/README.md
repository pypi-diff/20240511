# Comparing `tmp/movie-barcodes-0.0.6.tar.gz` & `tmp/movie-barcodes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movie-barcodes-0.0.6.tar", last modified: Thu May  9 10:16:45 2024, max compression
+gzip compressed data, was "movie-barcodes-0.1.1.tar", last modified: Sat May 11 09:41:42 2024, max compression
```

## Comparing `movie-barcodes-0.0.6.tar` & `movie-barcodes-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:16:45.039558 movie-barcodes-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-09 10:16:45.039558 movie-barcodes-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:16:45.035558 movie-barcodes-0.0.6/movie_barcodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-09 10:16:44.000000 movie-barcodes-0.0.6/movie_barcodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 10:16:45.000000 movie-barcodes-0.0.6/movie_barcodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:16:44.000000 movie-barcodes-0.0.6/movie_barcodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 10:16:44.000000 movie-barcodes-0.0.6/movie_barcodes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-09 10:16:44.000000 movie-barcodes-0.0.6/movie_barcodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 10:16:44.000000 movie-barcodes-0.0.6/movie_barcodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-09 10:16:45.039558 movie-barcodes-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:16:45.039558 movie-barcodes-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/src/barcode_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/src/color_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/src/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/src/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/src/video_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:16:45.039558 movie-barcodes-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/tests/test_barcode_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/tests/test_color_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/tests/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-05-09 10:16:30.000000 movie-barcodes-0.0.6/tests/test_video_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:41:42.310133 movie-barcodes-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-11 09:41:42.310133 movie-barcodes-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:41:42.310133 movie-barcodes-0.1.1/movie_barcodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-11 09:41:42.000000 movie-barcodes-0.1.1/movie_barcodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-11 09:41:42.000000 movie-barcodes-0.1.1/movie_barcodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 09:41:42.000000 movie-barcodes-0.1.1/movie_barcodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 09:41:42.000000 movie-barcodes-0.1.1/movie_barcodes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-11 09:41:42.000000 movie-barcodes-0.1.1/movie_barcodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-11 09:41:42.000000 movie-barcodes-0.1.1/movie_barcodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-11 09:41:42.310133 movie-barcodes-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:41:42.310133 movie-barcodes-0.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/src/barcode_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/src/color_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/src/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/src/video_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 09:41:42.310133 movie-barcodes-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/tests/test_barcode_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/tests/test_color_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/tests/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-05-11 09:41:26.000000 movie-barcodes-0.1.1/tests/test_video_processing.py
```

### Comparing `movie-barcodes-0.0.6/LICENSE` & `movie-barcodes-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.6/PKG-INFO` & `movie-barcodes-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: movie-barcodes
-Version: 0.0.6
-Summary: Compress every frame of a movie in a single color barcode.Transform entire movies into stunning single-barcode visualizations.Capture the essence of cinematic storytelling through dominant color extraction from each frame.
-Home-page: https://github.com/Wazzabeee/movie-barcodes
-Author: Clément Delteil
-Author-email: clement45.delteil45@gmail.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: lint
-Provides-Extra: dev
-License-File: LICENSE
-
 # Movie Barcodes
 The Lodger: A Story of the London Fog (1927) - Alfred Hitchcock - [Public Domain](https://archive.org/details/TheLodgerAStoryOfTheLondonFog_579)
 
 Circular Barcode           |  Horizontal Barcode
 :-------------------------:|:-------------------------:
 ![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/thelodgerastoryofthelondonfog_circular.png)  |  ![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/thelodgerastoryofthelondonfog_horizontal.png)
 
@@ -108,13 +92,29 @@
 # Todo
 
 - [ ] Optimize K-means to speed up the process
 - [ ] Add a small GUI with all options available
 - [ ] Add option to modify the barcode's height (current is frame's height)
 - [ ] Ensure the software can handle various video formats beyond MP4
 - [ ] Allow the software to process multiple videos at once
-- [ ] Add examples to Readme
 - [ ] Develop POC on Hugging Face Space
+- [ ] Remove the logs creation when using package
 
 # More Examples
-## Circular Barcodes
-## Horizontal Barcodes
+## Your Name (Kimi no Nawa)
+```python
+movie-barcodes --input_video_path "Your Name.mp4" --barcode_type "circular"
+movie-barcodes --input_video_path "Your Name.mp4" --width 1920 --barcode_type "horizontal"
+```
+Circular Barcode           |  Horizontal Barcode
+:-------------------------:|:-------------------------:
+![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/your_name_avg_circular.png)  |  ![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/your_name_avg_horizontal.png)
+## Drive
+```python
+movie-barcodes --input_video_path "Drive.mp4" --barcode_type "circular"
+movie-barcodes --input_video_path "Drive.mp4" --width 1920 --barcode_type "horizontal"
+```
+Circular Barcode           |  Horizontal Barcode
+:-------------------------:|:-------------------------:
+![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/drive_avg_circular.png)  |  ![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/drive_avg_horizontal.png)
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `movie-barcodes-0.0.6/README.md` & `movie-barcodes-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: movie-barcodes
+Version: 0.1.1
+Summary: Compress every frame of a movie in a single color barcode.Transform entire movies into stunning single-barcode visualizations.Capture the essence of cinematic storytelling through dominant color extraction from each frame.
+Home-page: https://github.com/Wazzabeee/movie-barcodes
+Author: Clément Delteil
+Author-email: clement45.delteil45@gmail.com
+Keywords: visualization,python,opencv,color extraction,data science,machine learning,movies,computer vision,multiprocessing,parallel computing,barcode,image processing,multithreading,data visualization,video processing,color barcode
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: lint
+Provides-Extra: dev
+License-File: LICENSE
+
 # Movie Barcodes
 The Lodger: A Story of the London Fog (1927) - Alfred Hitchcock - [Public Domain](https://archive.org/details/TheLodgerAStoryOfTheLondonFog_579)
 
 Circular Barcode           |  Horizontal Barcode
 :-------------------------:|:-------------------------:
 ![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/thelodgerastoryofthelondonfog_circular.png)  |  ![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/thelodgerastoryofthelondonfog_horizontal.png)
 
@@ -92,13 +113,29 @@
 # Todo
 
 - [ ] Optimize K-means to speed up the process
 - [ ] Add a small GUI with all options available
 - [ ] Add option to modify the barcode's height (current is frame's height)
 - [ ] Ensure the software can handle various video formats beyond MP4
 - [ ] Allow the software to process multiple videos at once
-- [ ] Add examples to Readme
 - [ ] Develop POC on Hugging Face Space
+- [ ] Remove the logs creation when using package
 
 # More Examples
-## Circular Barcodes
-## Horizontal Barcodes
+## Your Name (Kimi no Nawa)
+```python
+movie-barcodes --input_video_path "Your Name.mp4" --barcode_type "circular"
+movie-barcodes --input_video_path "Your Name.mp4" --width 1920 --barcode_type "horizontal"
+```
+Circular Barcode           |  Horizontal Barcode
+:-------------------------:|:-------------------------:
+![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/your_name_avg_circular.png)  |  ![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/your_name_avg_horizontal.png)
+## Drive
+```python
+movie-barcodes --input_video_path "Drive.mp4" --barcode_type "circular"
+movie-barcodes --input_video_path "Drive.mp4" --width 1920 --barcode_type "horizontal"
+```
+Circular Barcode           |  Horizontal Barcode
+:-------------------------:|:-------------------------:
+![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/drive_avg_circular.png)  |  ![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/drive_avg_horizontal.png)
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `movie-barcodes-0.0.6/movie_barcodes.egg-info/PKG-INFO` & `movie-barcodes-0.1.1/movie_barcodes.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: movie-barcodes
-Version: 0.0.6
+Version: 0.1.1
 Summary: Compress every frame of a movie in a single color barcode.Transform entire movies into stunning single-barcode visualizations.Capture the essence of cinematic storytelling through dominant color extraction from each frame.
 Home-page: https://github.com/Wazzabeee/movie-barcodes
 Author: Clément Delteil
 Author-email: clement45.delteil45@gmail.com
+Keywords: visualization,python,opencv,color extraction,data science,machine learning,movies,computer vision,multiprocessing,parallel computing,barcode,image processing,multithreading,data visualization,video processing,color barcode
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: dev
 License-File: LICENSE
 
 # Movie Barcodes
@@ -108,13 +113,29 @@
 # Todo
 
 - [ ] Optimize K-means to speed up the process
 - [ ] Add a small GUI with all options available
 - [ ] Add option to modify the barcode's height (current is frame's height)
 - [ ] Ensure the software can handle various video formats beyond MP4
 - [ ] Allow the software to process multiple videos at once
-- [ ] Add examples to Readme
 - [ ] Develop POC on Hugging Face Space
+- [ ] Remove the logs creation when using package
 
 # More Examples
-## Circular Barcodes
-## Horizontal Barcodes
+## Your Name (Kimi no Nawa)
+```python
+movie-barcodes --input_video_path "Your Name.mp4" --barcode_type "circular"
+movie-barcodes --input_video_path "Your Name.mp4" --width 1920 --barcode_type "horizontal"
+```
+Circular Barcode           |  Horizontal Barcode
+:-------------------------:|:-------------------------:
+![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/your_name_avg_circular.png)  |  ![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/your_name_avg_horizontal.png)
+## Drive
+```python
+movie-barcodes --input_video_path "Drive.mp4" --barcode_type "circular"
+movie-barcodes --input_video_path "Drive.mp4" --width 1920 --barcode_type "horizontal"
+```
+Circular Barcode           |  Horizontal Barcode
+:-------------------------:|:-------------------------:
+![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/drive_avg_circular.png)  |  ![](https://raw.githubusercontent.com/Wazzabeee/movie_color_barcode/main/examples/drive_avg_horizontal.png)
+
+
```

### Comparing `movie-barcodes-0.0.6/movie_barcodes.egg-info/SOURCES.txt` & `movie-barcodes-0.1.1/movie_barcodes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.6/setup.py` & `movie-barcodes-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,16 +41,38 @@
     "Capture the essence of cinematic storytelling through dominant color extraction from each frame.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Wazzabeee/movie-barcodes",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
         "Programming Language :: Python",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.10",
     entry_points={
         "console_scripts": [
             "movie-barcodes=src.main:main",
         ],
     },
+    keywords=[
+        "visualization",
+        "python",
+        "opencv",
+        "color extraction",
+        "data science",
+        "machine learning",
+        "movies",
+        "computer vision",
+        "multiprocessing",
+        "parallel computing",
+        "barcode",
+        "image processing",
+        "multithreading",
+        "data visualization",
+        "video processing",
+        "color barcode",
+    ],
 )
```

### Comparing `movie-barcodes-0.0.6/src/barcode_generation.py` & `movie-barcodes-0.1.1/src/barcode_generation.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.6/src/color_extraction.py` & `movie-barcodes-0.1.1/src/color_extraction.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.6/src/main.py` & `movie-barcodes-0.1.1/src/main.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.6/src/utility.py` & `movie-barcodes-0.1.1/src/utility.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.6/src/video_processing.py` & `movie-barcodes-0.1.1/src/video_processing.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.6/tests/test_barcode_generation.py` & `movie-barcodes-0.1.1/tests/test_barcode_generation.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.6/tests/test_color_extraction.py` & `movie-barcodes-0.1.1/tests/test_color_extraction.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.6/tests/test_integration.py` & `movie-barcodes-0.1.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.6/tests/test_utility.py` & `movie-barcodes-0.1.1/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `movie-barcodes-0.0.6/tests/test_video_processing.py` & `movie-barcodes-0.1.1/tests/test_video_processing.py`

 * *Files identical despite different names*

