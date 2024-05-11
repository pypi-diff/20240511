# Comparing `tmp/uxsim-1.2.0.tar.gz` & `tmp/uxsim-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uxsim-1.2.0.tar", last modified: Thu Apr 25 08:29:05 2024, max compression
+gzip compressed data, was "uxsim-1.3.0.tar", last modified: Sat May 11 08:24:47 2024, max compression
```

## Comparing `uxsim-1.2.0.tar` & `uxsim-1.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.412792 uxsim-1.2.0/
--rw-rw-rw-   0        0        0     1086 2023-08-01 08:45:01.000000 uxsim-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       21 2024-03-26 06:39:30.000000 uxsim-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    12071 2024-04-25 08:29:05.411792 uxsim-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    11171 2024-04-25 08:28:20.000000 uxsim-1.2.0/README.md
--rw-rw-rw-   0        0        0     1123 2024-04-06 11:27:18.000000 uxsim-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-25 08:29:05.412792 uxsim-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.344791 uxsim-1.2.0/tests/
--rw-rw-rw-   0        0        0     1523 2024-04-01 12:42:22.000000 uxsim-1.2.0/tests/test_examples.py
--rw-rw-rw-   0        0        0     6971 2024-04-25 08:28:20.000000 uxsim-1.2.0/tests/test_other_functions.py
--rw-rw-rw-   0        0        0     1682 2024-04-01 12:42:22.000000 uxsim-1.2.0/tests/test_result_gui_viewer.py
--rw-rw-rw-   0        0        0     3326 2024-04-01 12:42:22.000000 uxsim-1.2.0/tests/test_verification_exceptional.py
--rw-rw-rw-   0        0        0    69329 2024-04-25 08:28:20.000000 uxsim-1.2.0/tests/test_verification_multilane.py
--rw-rw-rw-   0        0        0    42414 2024-04-01 12:42:58.000000 uxsim-1.2.0/tests/test_verification_node.py
--rw-rw-rw-   0        0        0    26886 2024-04-15 10:46:18.000000 uxsim-1.2.0/tests/test_verification_route_choice.py
--rw-rw-rw-   0        0        0     3784 2024-04-01 12:42:22.000000 uxsim-1.2.0/tests/test_verification_sioux_falls.py
--rw-rw-rw-   0        0        0    39162 2024-04-01 12:42:22.000000 uxsim-1.2.0/tests/test_verification_straight_road.py
--rw-rw-rw-   0        0        0     9443 2024-04-25 08:28:20.000000 uxsim-1.2.0/tests/test_verification_taxi.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.349792 uxsim-1.2.0/uxsim/
-drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.376792 uxsim-1.2.0/uxsim/OSMImporter/
--rw-rw-rw-   0        0        0    16334 2024-04-09 08:40:41.000000 uxsim-1.2.0/uxsim/OSMImporter/OSMImporter.py
--rw-rw-rw-   0        0        0       26 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/OSMImporter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.378792 uxsim-1.2.0/uxsim/ResultGUIViewer/
--rw-rw-rw-   0        0        0    16823 2024-04-09 09:16:07.000000 uxsim-1.2.0/uxsim/ResultGUIViewer/ResultGUIViewer.py
--rw-rw-rw-   0        0        0       30 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/ResultGUIViewer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.380792 uxsim-1.2.0/uxsim/TaxiHandler/
--rw-rw-rw-   0        0        0    11724 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/TaxiHandler/TaxiHandler.py
--rw-rw-rw-   0        0        0       26 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/TaxiHandler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.383791 uxsim-1.2.0/uxsim/Utilities/
--rw-rw-rw-   0        0        0      153 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/Utilities/Utilities.py
--rw-rw-rw-   0        0        0       24 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/Utilities/__init__.py
--rw-rw-rw-   0        0        0      193 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/__init__.py
--rw-rw-rw-   0        0        0    57254 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/analyzer.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.409791 uxsim-1.2.0/uxsim/files/
--rw-rw-rw-   0        0        0 10695124 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/files/HackGen-Regular.ttf
--rw-rw-rw-   0        0        0    58464 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/files/Inconsolata.otf
--rw-rw-rw-   0        0        0     5951 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/files/LICENSE_of_HackGen-Regular
--rw-rw-rw-   0        0        0     4486 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/files/Licence_of_Inconsolata.otf.txt
--rw-rw-rw-   0        0        0       47 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/files/README.md
--rw-rw-rw-   0        0        0        0 2024-04-01 12:42:22.000000 uxsim-1.2.0/uxsim/files/__init__.py
--rw-rw-rw-   0        0        0     4939 2024-04-15 10:46:18.000000 uxsim-1.2.0/uxsim/utils.py
--rw-rw-rw-   0        0        0    81926 2024-04-25 08:28:20.000000 uxsim-1.2.0/uxsim/uxsim.py
-drwxrwxrwx   0        0        0        0 2024-04-25 08:29:05.410792 uxsim-1.2.0/uxsim.egg-info/
--rw-rw-rw-   0        0        0    12071 2024-04-25 08:29:05.000000 uxsim-1.2.0/uxsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1045 2024-04-25 08:29:05.000000 uxsim-1.2.0/uxsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 08:29:05.000000 uxsim-1.2.0/uxsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2024-04-25 08:29:05.000000 uxsim-1.2.0/uxsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-25 08:29:05.000000 uxsim-1.2.0/uxsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 08:24:47.204678 uxsim-1.3.0/
+-rw-rw-rw-   0        0        0     1086 2023-08-01 08:45:01.000000 uxsim-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0       21 2024-03-26 06:39:30.000000 uxsim-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12423 2024-05-11 08:24:47.202572 uxsim-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11288 2024-04-30 09:15:28.000000 uxsim-1.3.0/README.md
+-rw-rw-rw-   0        0        0     1330 2024-05-02 07:25:27.000000 uxsim-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 08:24:47.204678 uxsim-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 08:24:47.142426 uxsim-1.3.0/tests/
+-rw-rw-rw-   0        0        0     1523 2024-04-26 02:10:45.000000 uxsim-1.3.0/tests/test_examples.py
+-rw-rw-rw-   0        0        0     6727 2024-04-30 11:00:32.000000 uxsim-1.3.0/tests/test_other_functions.py
+-rw-rw-rw-   0        0        0     1682 2024-04-26 02:10:45.000000 uxsim-1.3.0/tests/test_result_gui_viewer.py
+-rw-rw-rw-   0        0        0     3326 2024-04-26 02:10:45.000000 uxsim-1.3.0/tests/test_verification_exceptional.py
+-rw-rw-rw-   0        0        0    69329 2024-04-26 02:10:45.000000 uxsim-1.3.0/tests/test_verification_multilane.py
+-rw-rw-rw-   0        0        0    42414 2024-04-26 02:10:45.000000 uxsim-1.3.0/tests/test_verification_node.py
+-rw-rw-rw-   0        0        0    26886 2024-04-26 02:10:45.000000 uxsim-1.3.0/tests/test_verification_route_choice.py
+-rw-rw-rw-   0        0        0     3784 2024-04-26 02:10:45.000000 uxsim-1.3.0/tests/test_verification_sioux_falls.py
+-rw-rw-rw-   0        0        0    39162 2024-04-26 02:10:45.000000 uxsim-1.3.0/tests/test_verification_straight_road.py
+-rw-rw-rw-   0        0        0     9363 2024-05-10 01:59:16.000000 uxsim-1.3.0/tests/test_verification_taxi.py
+drwxrwxrwx   0        0        0        0 2024-05-11 08:24:47.148426 uxsim-1.3.0/uxsim/
+drwxrwxrwx   0        0        0        0 2024-05-11 08:24:47.171427 uxsim-1.3.0/uxsim/OSMImporter/
+-rw-rw-rw-   0        0        0    17009 2024-04-30 10:57:13.000000 uxsim-1.3.0/uxsim/OSMImporter/OSMImporter.py
+-rw-rw-rw-   0        0        0       26 2024-04-26 02:10:45.000000 uxsim-1.3.0/uxsim/OSMImporter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 08:24:47.173426 uxsim-1.3.0/uxsim/ResultGUIViewer/
+-rw-rw-rw-   0        0        0    20878 2024-05-11 07:29:04.000000 uxsim-1.3.0/uxsim/ResultGUIViewer/ResultGUIViewer.py
+-rw-rw-rw-   0        0        0       30 2024-04-26 02:10:45.000000 uxsim-1.3.0/uxsim/ResultGUIViewer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 08:24:47.175427 uxsim-1.3.0/uxsim/TaxiHandler/
+-rw-rw-rw-   0        0        0    11724 2024-04-26 02:10:45.000000 uxsim-1.3.0/uxsim/TaxiHandler/TaxiHandler.py
+-rw-rw-rw-   0        0        0       26 2024-04-26 02:10:45.000000 uxsim-1.3.0/uxsim/TaxiHandler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 08:24:47.177427 uxsim-1.3.0/uxsim/Utilities/
+-rw-rw-rw-   0        0        0     2954 2024-05-11 08:22:51.000000 uxsim-1.3.0/uxsim/Utilities/Utilities.py
+-rw-rw-rw-   0        0        0       24 2024-04-26 02:10:45.000000 uxsim-1.3.0/uxsim/Utilities/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-05-11 08:24:26.000000 uxsim-1.3.0/uxsim/__init__.py
+-rw-rw-rw-   0        0        0    58661 2024-05-11 07:03:30.000000 uxsim-1.3.0/uxsim/analyzer.py
+drwxrwxrwx   0        0        0        0 2024-05-11 08:24:47.200574 uxsim-1.3.0/uxsim/files/
+-rw-rw-rw-   0        0        0 10695124 2024-04-26 02:10:45.000000 uxsim-1.3.0/uxsim/files/HackGen-Regular.ttf
+-rw-rw-rw-   0        0        0    58464 2024-04-26 02:10:45.000000 uxsim-1.3.0/uxsim/files/Inconsolata.otf
+-rw-rw-rw-   0        0        0     5951 2024-04-26 02:10:45.000000 uxsim-1.3.0/uxsim/files/LICENSE_of_HackGen-Regular
+-rw-rw-rw-   0        0        0     4486 2024-04-26 02:10:45.000000 uxsim-1.3.0/uxsim/files/Licence_of_Inconsolata.otf.txt
+-rw-rw-rw-   0        0        0       47 2024-04-26 02:10:45.000000 uxsim-1.3.0/uxsim/files/README.md
+-rw-rw-rw-   0        0        0        0 2024-04-26 02:10:45.000000 uxsim-1.3.0/uxsim/files/__init__.py
+-rw-rw-rw-   0        0        0     5290 2024-05-09 10:31:26.000000 uxsim-1.3.0/uxsim/utils.py
+-rw-rw-rw-   0        0        0    83580 2024-05-09 05:53:46.000000 uxsim-1.3.0/uxsim/uxsim.py
+drwxrwxrwx   0        0        0        0 2024-05-11 08:24:47.201571 uxsim-1.3.0/uxsim.egg-info/
+-rw-rw-rw-   0        0        0    12423 2024-05-11 08:24:47.000000 uxsim-1.3.0/uxsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1045 2024-05-11 08:24:47.000000 uxsim-1.3.0/uxsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 08:24:47.000000 uxsim-1.3.0/uxsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2024-05-11 08:24:47.000000 uxsim-1.3.0/uxsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-11 08:24:47.000000 uxsim-1.3.0/uxsim.egg-info/top_level.txt
```

### Comparing `uxsim-1.2.0/LICENSE` & `uxsim-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/PKG-INFO` & `uxsim-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: uxsim
-Version: 1.2.0
+Version: 1.3.0
 Summary: UXsim: traffic flow simulator
 Author-email: Toru Seo <seo.t.aa@m.titech.ac.jp>
 License: MIT License
 Project-URL: Homepage, https://github.com/toruseo/UXsim
 Project-URL: Documentation, https://toruseo.jp/UXsim/docs
 Project-URL: Issues, https://github.com/toruseo/UXsim/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.5
 Requires-Dist: matplotlib>=3.5.2
 Requires-Dist: pillow>=9.2.0
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: scipy>=1.9.1
 Requires-Dist: pandas>=1.4.4
 Requires-Dist: PyQt5>=5.15.7
+Requires-Dist: dill>=0.3.8
 
 # UXsim: Network traffic flow simulator in pure Python
 
 [![PyPi](https://img.shields.io/pypi/v/uxsim.svg)](https://pypi.python.org/pypi/uxsim)
 [![Demo in Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb)
 [![arXiv](https://img.shields.io/badge/arXiv-2309.17114-b31b1b.svg)](http://dx.doi.org/10.48550/arXiv.2309.17114)
 [![Static Badge](https://img.shields.io/badge/readme-English%20%F0%9F%87%BA%F0%9F%87%B8%20-%20darkblue)](https://github.com/toruseo/UXsim/blob/main/README.md)
@@ -218,16 +223,16 @@
 
 ## Terms of Use & License
 
 UXsim is released under the MIT License. You are free to use it as long as the source is acknowledged.
 
 When publishing works based on UXsim, please cite:
 
-- Toru Seo. Macroscopic Traffic Flow Simulation: Fundamental Mathematical Theory and Python Implementation. Corona Publishing Co., Ltd., 2023.
-- Toru Seo. UXsim: An open source macroscopic and mesoscopic traffic simulator in Python-a technical overview. arXiv preprint arXiv: 2309.17114, 2023
+- Toru Seo. [Macroscopic Traffic Flow Simulation: Fundamental Mathematical Theory and Python Implementation](https://toruseo.github.io/misc/MacroTrafficSim_English_summary.pdf). Corona Publishing Co., Ltd., 2023.
+- Toru Seo. [UXsim: An open source macroscopic and mesoscopic traffic simulator in Python-a technical overview](http://dx.doi.org/10.48550/arXiv.2309.17114). arXiv preprint arXiv: 2309.17114, 2023
 
 ## Contributing and Discussion
 
 Contributions are welcome!
 Please see the [Contributing Guideline](https://github.com/toruseo/UXsim/blob/main/.github/CONTRIBUTING.md).
 
 If you have any questions or suggestions, please post them to the [Issues](https://github.com/toruseo/UXsim/issues) or [Discussions](https://github.com/toruseo/UXsim/discussions) (in English or Japanese).
```

### Comparing `uxsim-1.2.0/README.md` & `uxsim-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -193,16 +193,16 @@
 
 ## Terms of Use & License
 
 UXsim is released under the MIT License. You are free to use it as long as the source is acknowledged.
 
 When publishing works based on UXsim, please cite:
 
-- Toru Seo. Macroscopic Traffic Flow Simulation: Fundamental Mathematical Theory and Python Implementation. Corona Publishing Co., Ltd., 2023.
-- Toru Seo. UXsim: An open source macroscopic and mesoscopic traffic simulator in Python-a technical overview. arXiv preprint arXiv: 2309.17114, 2023
+- Toru Seo. [Macroscopic Traffic Flow Simulation: Fundamental Mathematical Theory and Python Implementation](https://toruseo.github.io/misc/MacroTrafficSim_English_summary.pdf). Corona Publishing Co., Ltd., 2023.
+- Toru Seo. [UXsim: An open source macroscopic and mesoscopic traffic simulator in Python-a technical overview](http://dx.doi.org/10.48550/arXiv.2309.17114). arXiv preprint arXiv: 2309.17114, 2023
 
 ## Contributing and Discussion
 
 Contributions are welcome!
 Please see the [Contributing Guideline](https://github.com/toruseo/UXsim/blob/main/.github/CONTRIBUTING.md).
 
 If you have any questions or suggestions, please post them to the [Issues](https://github.com/toruseo/UXsim/issues) or [Discussions](https://github.com/toruseo/UXsim/discussions) (in English or Japanese).
```

### Comparing `uxsim-1.2.0/pyproject.toml` & `uxsim-1.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -8,26 +8,31 @@
 readme = "README.md"
 authors = [{name = "Toru Seo", email = "seo.t.aa@m.titech.ac.jp"}]
 license = {text = "MIT License"}
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "numpy>=1.21.5",
     "matplotlib>=3.5.2",
     "pillow>=9.2.0",
     "tqdm>=4.64.1",
     "scipy>=1.9.1",
     "pandas>=1.4.4",
-    "PyQt5>=5.15.7"
+    "PyQt5>=5.15.7",
+    "dill>=0.3.8"
 ]
 dynamic = ["version"] # Version is read from uxsim/__init__.py
 
 [project.urls]
 Homepage = "https://github.com/toruseo/UXsim"
 Documentation = "https://toruseo.jp/UXsim/docs"
 Issues = "https://github.com/toruseo/UXsim/issues"
```

### Comparing `uxsim-1.2.0/tests/test_examples.py` & `uxsim-1.3.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/tests/test_other_functions.py` & `uxsim-1.3.0/tests/test_other_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,29 +68,27 @@
 
     # Save the results to CSV
     W.analyzer.output_data()
 
     assert True
 
 @pytest.mark.filterwarnings("ignore::UserWarning")
-@pytest.mark.filterwarnings("ignore::DeprecationWarning") #TODO: Current usage of OSMnx will be deprecated in the future. Need to update.
-@pytest.mark.filterwarnings("ignore:Iteration over multi-part geometries is deprecated")
 def test_osm_import():
     from uxsim.OSMImporter import OSMImporter
 
     W = World(
         name="",
         deltan=5,
         tmax=7200,
         print_mode=1, save_mode=1, show_mode=0, 
         random_seed=0
     )
 
     #Tokyo highway
-    nodes, links = OSMImporter.import_osm_data(north=35.817, south=35.570, east=139.881, west=139.583, custom_filter='["highway"~"motorway"]')
+    nodes, links = OSMImporter.import_osm_data(bbox=(35.817, 35.570, 139.881, 139.583), custom_filter='["highway"~"motorway"]')
     nodes, links = OSMImporter.osm_network_postprocessing(nodes, links, node_merge_threshold=0.005, node_merge_iteration=5, enforce_bidirectional=True)  # merge threshold distance: 0.005 degree ~= 500 m. `enforce_bidirectional` makes all links bidirectional, so that network is not fragmented (but the original network topology is not preserved rigorously).
     OSMImporter.osm_network_visualize(nodes, links, show_link_name=0, show_mode=0, save_mode=0)
     OSMImporter.osm_network_to_World(W, nodes, links, default_jam_density=0.2, coef_degree_to_meter=111000)
     W.show_network()
     
     # set demand to central Tokyo from surroundings
     W.adddemand_area2area(139.70, 35.60, 0, 139.75, 35.68, 0.05, 0, 3600, volume=5000)
```

### Comparing `uxsim-1.2.0/tests/test_result_gui_viewer.py` & `uxsim-1.3.0/tests/test_result_gui_viewer.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/tests/test_verification_exceptional.py` & `uxsim-1.3.0/tests/test_verification_exceptional.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/tests/test_verification_multilane.py` & `uxsim-1.3.0/tests/test_verification_multilane.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/tests/test_verification_node.py` & `uxsim-1.3.0/tests/test_verification_node.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/tests/test_verification_route_choice.py` & `uxsim-1.3.0/tests/test_verification_route_choice.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/tests/test_verification_sioux_falls.py` & `uxsim-1.3.0/tests/test_verification_sioux_falls.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/tests/test_verification_straight_road.py` & `uxsim-1.3.0/tests/test_verification_straight_road.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/tests/test_verification_taxi.py` & `uxsim-1.3.0/tests/test_verification_taxi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """
-This script verifies whether UXsim outputs plausible solutions for exceptional or uncommon situations.
-The behavior of UXsim may be updated in the future.
+This script verifies whether UXsim outputs reasonable solutions with taxis.
 """
 
 import pytest
 from uxsim import *
 from uxsim.TaxiHandler import *
 from math import sin, cos, pi
```

### Comparing `uxsim-1.2.0/uxsim/OSMImporter/OSMImporter.py` & `uxsim-1.3.0/uxsim/OSMImporter/OSMImporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import warnings
 
 class OSMImporter:
     """
     OpenStreetMap importer using OSMnx.
     Work in progress. Import from OSM is experimental and may not work as expected. It is functional but may produce inappropriate networks for simulation, such as too many nodes, too many deadends, fragmented networks.
     """
-    def import_osm_data(north, south, east, west, custom_filter='["highway"~"trunk|primary"]', 
+    def import_osm_data(north=None, south=None, east=None, west=None, bbox=None, custom_filter='["highway"~"trunk|primary"]', 
                         default_number_of_lanes_mortorway=3, default_number_of_lanes_trunk=3, 
                         default_number_of_lanes_primary=2, default_number_of_lanes_secondary=2, 
                         default_number_of_lanes_residential=1, default_number_of_lanes_tertiary=1, 
                         default_number_of_lanes_others=1, 
                         default_maxspeed_mortorway=100, default_maxspeed_trunk=60, 
                         default_maxspeed_primary=50, default_maxspeed_secondary=50, 
                         default_maxspeed_residential=30, default_maxspeed_tertiary=30, 
@@ -38,14 +38,16 @@
         """
         Import road network data from OpenStreetMap using OSMnx.
 
         Parameters
         ----------
         north, south, east, west: float
             The latitudes and longitudes of the area to be imported.
+        bbox: list
+            The bounding box of the area to be imported. The order is [north, south, east, west]. This is prioritized than north, south, east, west arguments.
         custom_filter: str
             The filter to be used for importing the data. 
             The default is '["highway"~"trunk|primary"]', which means that only trunk and primary roads (usually correspond to major arterial roads) are imported.
         default_number_of_lanes_*: int
             The default number of lanes for * {road_type}.
         default_maxspeed_*: float
             The default maximum speed for * {road_type}.    
@@ -64,15 +66,22 @@
 
         try:
             import osmnx as ox
         except:
             raise ImportError("Optional module 'osmnx' is not installed. Please install it by 'pip install osmnx' to use this function.")
 
         print("Start downloading OSM data. This may take some time.")
-        G = ox.graph.graph_from_bbox(north=north, south=south, east=east, west=west, network_type="drive", 
+        if bbox is not None:
+            try:
+                G = ox.graph.graph_from_bbox(bbox=bbox, network_type="drive", custom_filter=custom_filter)
+            except TypeError: #version issue?
+                warnings.warn("OSMnx version may be too old. Update is recommended.")
+                G = ox.graph.graph_from_bbox(north=bbox[0], south=bbox[1], east=bbox[2], west=bbox[3], network_type="drive", custom_filter=custom_filter)
+        else:
+            G = ox.graph.graph_from_bbox(north=north, south=south, east=east, west=west, network_type="drive", 
                                     custom_filter=custom_filter)
         print("Download completed")
         """
         motorway: 高速道路
         trunk: 一般国道
         primary: 主要地方道（2桁番号県道・市道）
         secondary: 一般地方道（3桁番号県道・市道）
```

### Comparing `uxsim-1.2.0/uxsim/ResultGUIViewer/ResultGUIViewer.py` & `uxsim-1.3.0/uxsim/ResultGUIViewer/ResultGUIViewer.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,18 @@
     >>> from uxsim.ResultGUIViewer import launch_World_viewer
     >>> launch_World_viewer(W)
 """
 
 import sys
 import numpy as np
 from matplotlib import colormaps
-from PyQt5.QtWidgets import QApplication, QMainWindow, QGraphicsView, QGraphicsScene, QGraphicsItem, QMenu, QSlider, QVBoxLayout, QWidget, QHBoxLayout, QLabel, QPushButton
+from PyQt5.QtWidgets import QApplication, QMainWindow, QGraphicsView, QGraphicsScene, QGraphicsItem, QMenu, QSlider, QVBoxLayout, QWidget, QHBoxLayout, QLabel, QPushButton, QInputDialog, QMessageBox, QTableView, QDialog, QFileDialog
 from PyQt5.QtGui import QPen, QColor, QPainter, QPainterPath
-from PyQt5.QtCore import Qt, QPointF, QRectF, QTimer
+from PyQt5.QtCore import Qt, QPointF, QRectF, QTimer, QAbstractTableModel
+
 
 class EdgeItem(QGraphicsItem):
     def __init__(self, name, start_node, end_node, density_list, Link):
         super().__init__()
         self.name = name
         self.start_node = start_node
         self.end_node = end_node
@@ -40,15 +41,15 @@
         path = QPainterPath(self.start_node.pos())
         dx = self.end_node.pos().x() - self.start_node.pos().x()
         dy = self.end_node.pos().y() - self.start_node.pos().y()
         
         length = (dx**2 + dy**2)**0.5
         offset = length/10
         if dx == 0:
-            offset = QPointF(0, offset if dy > 0 else -offset)
+            offset = QPointF(-offset*self.curve_direction if dy > 0 else offset*self.curve_direction, 0)
         else:
             normal = QPointF(-dy, dx)
             normal /= (normal.x()**2 + normal.y()**2)**0.5
             offset = normal * (offset * self.curve_direction)
 
         control_point = (self.start_node.pos() + self.end_node.pos()) / 2 + offset
         path.quadTo(control_point, self.end_node.pos())
@@ -61,18 +62,17 @@
         segment_length = length / num_segments
         maxlw = 10
         minlw = 0.5
 
         for i in range(num_segments):
             density = self.density_list[self.t, i]
             speed = self.Link.v_mat[self.t, i]
-            lw = max([density*self.Link.delta])*(maxlw-minlw)+minlw
+            lw = max([density*self.Link.delta*self.Link.lanes])*(maxlw-minlw)+minlw
             
             c = colormaps["viridis"](speed/self.Link.u)
-            #color = QColor(int(density/self.Link.jam_density * 255), int(density/self.Link.jam_density * 255), 0, 255)
             color = QColor(int(c[0]*255), int(c[1]*255), int(c[2]*255), 255)
             pen = QPen(color, lw)
             painter.setPen(pen)
 
             start_percent = i / num_segments
             end_percent = (i + 1) / num_segments
             start_point = path.pointAtPercent(start_percent)
@@ -123,14 +123,15 @@
             
     def set_curve_direction(self, direction):
         self.curve_direction = direction
 
     def set_show_name(self, show_name):
         self.show_name = show_name
 
+
 class NodeItem(QGraphicsItem):
     def __init__(self, name, x, y, Node):
         super().__init__()
         self.name = name
         self.setPos(x, y)
         self.Node = Node
         self.show_name = True
@@ -145,27 +146,29 @@
         if self.show_name:
             painter.setPen(QColor(0, 128, 0))
             painter.drawText(-5, 5, self.name)
             
     def set_show_name(self, show_name):
         self.show_name = show_name
 
+
 class VehicleItem(QGraphicsItem):
     def __init__(self, x, y):
         super().__init__()
         self.setPos(x, y)
         self.setZValue(2)
 
     def boundingRect(self):
         return QRectF(-5, -5, 10, 10)
 
     def paint(self, painter, option, widget):
         painter.setBrush(Qt.red)
         painter.drawEllipse(-5, -5, 10, 10)
 
+
 class GraphWidget(QGraphicsView):
     def __init__(self, nodes, edges, vehicle_list):
         super().__init__()
         self.setRenderHint(QPainter.Antialiasing)
         self.setScene(QGraphicsScene(self))
         self.setSceneRect(0, 0, 800, 800)
         self.setDragMode(QGraphicsView.ScrollHandDrag)
@@ -184,17 +187,20 @@
             name, start_node_name, end_node_name, density_list, Node = edge_data
             start_node = self.find_node(start_node_name)
             end_node = self.find_node(end_node_name)
             if start_node and end_node:
                 edge = EdgeItem(name, start_node, end_node, density_list, Node)
                 self.scene().addItem(edge)
                 self.edges.append(edge)
+        
+        self.set_vehice_items()
 
+    def set_vehice_items(self):
         self.vehicle_items = []
-        if self.show_vehicles and self.vehicle_list != None:
+        if self.vehicle_list != None:
             for t, edge_name, x in self.vehicle_list:
                 edge = self.find_edge(edge_name)
                 if edge:
                     path = edge.shape()
                     point = path.pointAtPercent(x)
                     vehicle = VehicleItem(point.x(), point.y())
                     self.scene().addItem(vehicle)
@@ -249,23 +255,24 @@
     def set_show_vehicles(self, show_vehicles):
         self.show_vehicles = show_vehicles
         for vehicle in self.vehicle_items:
             vehicle.setVisible(show_vehicles)
         self.viewport().update()
 
 class MainWindow(QMainWindow):
-    def __init__(self, W, nodes, edges, vehicle_list, tmax):
+    def __init__(self, W, nodes, edges, vehicle_list, tmax, dt):
         super().__init__()
         self.setWindowTitle("UXsim result viewer")
         self.W = W
         self.tmax = tmax
+        self.dt = dt
         self.playing = False
         self.curve_direction = 1
         self.show_names = True
-        self.show_vehicles = True
+        self.show_vehicles = False
 
         central_widget = QWidget()
         layout = QVBoxLayout()
         central_widget.setLayout(layout)
         self.setCentralWidget(central_widget)
 
         slider_layout = QHBoxLayout()
@@ -300,50 +307,76 @@
         self.timer.timeout.connect(self.update_t)
         
         menu_bar = self.menuBar()
         
         # menu_file = menu_bar.addMenu("File")
         # acrion_save_world = menu_file.addAction("Save World")
         # acrion_save_world.triggered.connect(lambda: self.save_world())
+
+        menu_data = menu_bar.addMenu("Data")
+        action_basic_stats = menu_data.addAction("Basic Statistics")
+        action_basic_stats.triggered.connect(lambda: self.show_dataframe("Basic", self.W.analyzer.basic_to_pandas()))
+        action_basic_stats = menu_data.addAction("Link Statistics")
+        action_basic_stats.triggered.connect(lambda: self.show_dataframe("Link", self.W.analyzer.link_to_pandas()))
+        action_basic_stats = menu_data.addAction("OD Demand Statistics")
+        action_basic_stats.triggered.connect(lambda: self.show_dataframe("OD Demand", self.W.analyzer.od_to_pandas()))
+        action_basic_stats = menu_data.addAction("Vehicle Trip Statistics")
+        action_basic_stats.triggered.connect(lambda: self.show_dataframe("Vehicle Trip", self.W.analyzer.vehicle_trip_to_pandas()))
+        action_basic_stats = menu_data.addAction("Vehicle Detailed Statistics")
+        action_basic_stats.triggered.connect(lambda: self.show_dataframe("Vehicle", self.W.analyzer.vehicles_to_pandas()))
         
         menu_settings = menu_bar.addMenu("Settings")
         option_curve_direction = menu_settings.addMenu("Link Curve Direction")
         curve_right_action = option_curve_direction.addAction("Right-handed")
         curve_right_action.triggered.connect(lambda: self.set_curve_direction(1))
         curve_left_action = option_curve_direction.addAction("Left-handed")
         curve_left_action.triggered.connect(lambda: self.set_curve_direction(-1))
         
         option_display = menu_settings.addMenu("Display")
         show_names_action = option_display.addAction("Show Names")
         show_names_action.setCheckable(True)
         show_names_action.setChecked(True)
         show_names_action.triggered.connect(self.toggle_show_names)
 
+        menu_Vehicle = menu_bar.addMenu("Vehicle Analysis")
+        # show_vehicles_action = menu_Vehicle.addAction("Show Vehicle")
+        # show_vehicles_action.setCheckable(True)
+        # show_vehicles_action.setChecked(False)
+        # show_vehicles_action.triggered.connect(self.toggle_show_vehicles)
+        action_show_vehicle = menu_Vehicle.addAction("Highlight Vehicle by ID")
+        action_show_vehicle.triggered.connect(self.show_vehicle_by_id)
+
         menu_Animation = menu_bar.addMenu("Export Results")
         action_csv = menu_Animation.addAction("Export Results to CSV files")
         action_csv.triggered.connect(lambda: self.W.analyzer.output_data())
         action_network_anim_detailed0 = menu_Animation.addAction("Export Network Animation (link-level)")
         action_network_anim_detailed0.triggered.connect(lambda: self.W.analyzer.network_anim(detailed=0))
         action_network_anim_detailed1 = menu_Animation.addAction("Export Network Animation (link segment-level)")
         action_network_anim_detailed1.triggered.connect(lambda: self.W.analyzer.network_anim(detailed=1))
         action_network_anim_fancy = menu_Animation.addAction("Export Network Animation (vehicle-level)")
         action_network_anim_fancy.triggered.connect(lambda: self.W.analyzer.network_fancy())
 
-        # menu_Vehicle = menu_bar.addMenu("Vehicle Analysis")
-        # show_vehicles_action = menu_Vehicle.addAction("Show Vehicles")
-        # show_vehicles_action.setCheckable(True)
-        # show_vehicles_action.setChecked(True)
-        # show_vehicles_action.triggered.connect(self.toggle_show_vehicles)
-
         self.update_graph()
 
-    def save_world(self):
-        import pickle
-        with open("World.pkl", mode="wb") as f:
-            pickle.dump(self.W, f)
+    def show_dataframe(self, title, df):
+        viewer = DataFrameViewer(df, title, self)
+        viewer.show()
+
+    def save_world(self, default_filename='untitled.pkl_dill'):
+        #TODO: do something about "maximum recursion depth exceeded in comparison" error
+        import dill as pickle
+        filename, _ = QFileDialog.getSaveFileName(None, 'Save the world', default_filename, 'Pickle (by Dill package) Files (*.pkl_dill);;All Files (*)')
+        
+        if filename:
+            try:
+                with open(filename, 'wb') as file:
+                    pickle.dump(self.W, file)
+                print(f'World saved successfully: {filename}')
+            except Exception as e:
+                print(f'Error saving object: {str(e)}')
 
     def update_graph(self):
         t = self.t_slider.value()
         edie_dt = self.graph_widget.edges[0].Link.edie_dt
         self.graph_widget.set_t(t)
         self.t_label.setText("{}/{}".format(t*edie_dt, self.tmax*edie_dt))
 
@@ -373,14 +406,68 @@
     def toggle_show_names(self):
         self.show_names = not self.show_names
         self.graph_widget.set_show_names(self.show_names)
 
     def toggle_show_vehicles(self):
         self.show_vehicles = not self.show_vehicles
         self.graph_widget.set_show_vehicles(self.show_vehicles)
+    
+    def show_vehicle_by_id(self):
+        vehicle_id, ok = QInputDialog.getText(self, "Highlight Vehicle", "<b>Enter Vehicle ID</b><br>Note that fast vehicles will be plotted as multiple dots in the animation.")
+        if ok and vehicle_id:
+            self.vehicle_id = vehicle_id
+            if vehicle_id not in self.W.VEHICLES:
+                QMessageBox.warning(self, "Vehicle ID not found", "The specified Vehicle ID was not found.")
+                return
+            veh = self.W.VEHICLES[vehicle_id]
+            self.graph_widget.vehicle_list = [(int(veh.log_t[i]/self.dt), veh.log_link[i].name, veh.log_x[i]/veh.log_link[i].length) for i in range(len(veh.log_t)) if veh.log_link[i] != -1]
+            print(veh, self.graph_widget.vehicle_list)
+
+            self.graph_widget.set_vehice_items()
+
+            self.graph_widget.set_show_vehicles(True)
+
+
+class PandasModel(QAbstractTableModel):
+    def __init__(self, data):
+        super(PandasModel, self).__init__()
+        self._data = data
+
+    def rowCount(self, parent=None):
+        return self._data.shape[0]
+
+    def columnCount(self, parent=None):
+        return self._data.shape[1]
+
+    def data(self, index, role=Qt.DisplayRole):
+        if index.isValid() and role == Qt.DisplayRole:
+            return str(self._data.iloc[index.row(), index.column()])
+        return None
+
+    def headerData(self, section, orientation, role=Qt.DisplayRole):
+        if role == Qt.DisplayRole:
+            if orientation == Qt.Horizontal:
+                return str(self._data.columns[section])
+            elif orientation == Qt.Vertical:
+                return str(self._data.index[section])
+        return None
+
+
+class DataFrameViewer(QDialog):
+    def __init__(self, data, title, parent=None):
+        super(DataFrameViewer, self).__init__(parent)
+        self.setWindowTitle(title)
+        self.setLayout(QVBoxLayout())
+        self.model = PandasModel(data)
+        self.view = QTableView()
+        self.view.setModel(self.model)
+        self.layout().addWidget(self.view)
+        
+        self.resize(1200, 600)
+
 
 def launch_World_viewer(W, return_app_window=False):
     """
     Launch the interactive viewer for the simulation result of the given World object.
 
     Parameters
     ----------
@@ -420,15 +507,15 @@
             node[2] = (maxy - node[2]) / (maxx - minx) * (xysize - xybuffer*2) + xybuffer
     else:
         for node in nodes:
             node[1] = (node[1] - minx) / (maxy - miny) * (xysize - xybuffer*2) + xybuffer
             node[2] = (maxy - node[2]) / (maxy - miny) * (xysize - xybuffer*2) + xybuffer
 
     edges = [[l.name, l.start_node.name, l.end_node.name, l.k_mat, l] for l in W.LINKS]
-    vehicle_list = None
+    dt = W.LINKS[0].edie_dt
 
     app = QApplication(sys.argv)
-    window = MainWindow(W, nodes, edges, vehicle_list, tmax)
+    window = MainWindow(W, nodes, edges, None, tmax, dt)
     window.show()
     if return_app_window:
         return app, window
     sys.exit(app.exec_())
```

### Comparing `uxsim-1.2.0/uxsim/TaxiHandler/TaxiHandler.py` & `uxsim-1.3.0/uxsim/TaxiHandler/TaxiHandler.py`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/uxsim/analyzer.py` & `uxsim-1.3.0/uxsim/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,33 @@
 import matplotlib.pyplot as plt
 import random, glob, os, csv, time
 import pandas as pd
 from PIL import Image, ImageDraw, ImageFont
 from PIL.Image import Resampling
 from tqdm.auto import tqdm
 from collections import defaultdict as ddict
-from importlib.resources import read_binary #according to official doc, this is also not recommended
+from importlib.resources import read_binary, files #TODO: according to official doc, `read_binary` is not recommended. To be replaced with `files` in the future after some testing.
 import io
 from scipy.sparse.csgraph import floyd_warshall
 
-from .utils  import *
+from .utils import *
 
 plt.rcParams["font.family"] = get_font_for_matplotlib()
 
+def load_font_data_new():
+    fname = "HackGen-Regular.ttf"
+    font_data_path = files('uxsim.files').joinpath(fname)
+    with font_data_path.open('rb') as file:
+        font_data = file.read()
+    return font_data
+
+def load_font_data():
+    font_data = read_binary("uxsim.files", "HackGen-Regular.ttf")
+    return font_data
+
 class Analyzer:
     """
     Class for analyzing and visualizing a simulation result.
     """
 
     def __init__(s, W):
         """
@@ -149,14 +160,15 @@
             l_old = None
             for i in lange(veh.log_t):
                 if veh.log_link[i] != -1:
                     l = s.W.get_link(veh.log_link[i])
                     if l_old != l:
                         l.tss.append([])
                         l.xss.append([])
+                        l.ls.append(veh.log_lane[i])
                         l.cs.append(veh.color)
                         l.names.append(veh.name)
 
                     l_old = l
                     l.tss[-1].append(veh.log_t[i])
                     l.xss[-1].append(veh.log_x[i])
 
@@ -284,14 +296,15 @@
             print(" number of completed trips:\t", s.trip_completed, "/", s.trip_all)
             #print(" number of completed trips:\t", s.trip_completed, "/", len(s.W.VEHICLES)*s.W.DELTAN)
             if s.trip_completed > 0:
                 print(f" average travel time of trips:\t {s.average_travel_time:.1f} s")
                 print(f" average delay of trips:\t {s.average_delay:.1f} s")
                 print(f" delay ratio:\t\t\t {s.average_delay/s.average_travel_time:.3f}")
 
+
     def comp_route_travel_time(s, t, route):
         pass
 
     @catch_exceptions_and_warn()
     def time_space_diagram_traj(s, links=None, figsize=(12,4), plot_signal=True, xlim=None, ylim=None):
         """
         Draws the time-space diagram of vehicle trajectories for vehicles on specified links.
@@ -305,57 +318,29 @@
             The size of the figure to be plotted, default is (12,4).
         plot_signal : bool, optional
             Plot the downstream signal red light.
         """
         if s.W.vehicle_logging_timestep_interval != 1:
             warnings.warn("vehicle_logging_timestep_interval is not 1. The plot is not exactly accurate.", LoggingWarning)
 
-        #リンク車両軌跡の時空間図
-        s.W.print(" drawing trajectories...")
         s.compute_accurate_traj()
 
         #対象がlistであればOKで，単一な場合にはlistに変換する．未指定であれば全部にする．
         if links == None:
             links = s.W.LINKS
         try:
             iter(links)
             if type(links) == str:
                 links = [links]
         except TypeError:
             links = [links]
 
-        for lll in tqdm(links, disable=(s.W.print_mode==0)):
-            l = s.W.get_link(lll)
-
-            plt.figure(figsize=figsize)
-            plt.title(l)
-            for i in range(len(l.xss)):
-                plt.plot(l.tss[i], l.xss[i], c=l.cs[i], lw=0.5)
-            if plot_signal:
-                signal_log = [i*s.W.DELTAT for i in lange(l.end_node.signal_log) if (l.end_node.signal_log[i] not in l.signal_group and len(l.end_node.signal)>1)]
-                plt.plot(signal_log, [l.length for i in lange(signal_log)], "r.")
-            plt.xlabel("time (s)")
-            plt.ylabel("space (m)")
-            if xlim == None:
-                plt.xlim([0, s.W.TMAX])
-            else:
-                plt.xlim(xlim)
-            if ylim == None:
-                plt.ylim([0, l.length])
-            else:
-                plt.ylim(ylim)
-            plt.grid()
-            plt.tight_layout()
-            if s.W.save_mode:
-                plt.savefig(f"out{s.W.name}/tsd_traj_{l.name}.png")
-            if s.W.show_mode:
-                plt.show()
-            else:
-                plt.close("all")
-
+        for lll in links:
+            s.time_space_diagram_traj_links(linkslist=[lll], figsize=figsize, plot_signal=plot_signal, xlim=xlim, ylim=ylim)
+    
     @catch_exceptions_and_warn()
     def time_space_diagram_density(s, links=None, figsize=(12,4), plot_signal=True, xlim=None, ylim=None):
         """
         Draws the time-space diagram of traffic density on specified links.
 
         Parameters
         ----------
@@ -425,21 +410,21 @@
         Parameters
         ----------
         linkslist : list of link or list of list of link
             The names of the concective links for which the time-space diagram is to be plotted.
         figsize : tuple of int, optional
             The size of the figure to be plotted, default is (12,4).
         plot_signal : bool, optional
-            Plot the signal red light.
+            Plot the signal red light. 
         """
         if s.W.vehicle_logging_timestep_interval != 1:
             warnings.warn("vehicle_logging_timestep_interval is not 1. The plot is not exactly accurate.", LoggingWarning)
             
         #複数リンクの連続した車両軌跡の時空間図
-        s.W.print(" drawing trajectories in consecutive links...")
+        s.W.print(" drawing trajectories...")
         s.compute_accurate_traj()
 
         #リンクリストのリストであればそのまま，そうでなければリスト化
         try:
             iter(linkslist[0])
             if type(linkslist[0]) == str:
                 linkslist = [linkslist]
@@ -454,15 +439,16 @@
                 linkdict[l] = d
                 d += l.length
 
             plt.figure(figsize=figsize)
             for ll in links:
                 l = s.W.get_link(ll)
                 for i in range(len(l.xss)):
-                    plt.plot(l.tss[i], np.array(l.xss[i])+linkdict[l], c=l.cs[i], lw=0.5)
+                    lane_shift = l.ls[i]/l.lanes*s.W.DELTAT/2 #vehicle with the same lane is plotted slightly shifted
+                    plt.plot(np.array(l.tss[i])+lane_shift, np.array(l.xss[i])+linkdict[l], "-", c=l.cs[i], lw=0.5)
                 if plot_signal:
                     signal_log = [i*s.W.DELTAT for i in lange(l.end_node.signal_log) if (l.end_node.signal_log[i] not in l.signal_group and len(l.end_node.signal)>1)]
                     plt.plot(signal_log, [l.length+linkdict[l] for i in lange(signal_log)], "r.")
             for l in linkdict.keys():
                 plt.plot([0, s.W.TMAX], [linkdict[l], linkdict[l]], "k--", lw=0.7)
                 plt.plot([0, s.W.TMAX], [linkdict[l]+l.length, linkdict[l]+l.length], "k--", lw=0.7)
                 plt.text(0, linkdict[l]+l.length/2, l.name, va="center", c="b")
@@ -478,15 +464,18 @@
             if ylim == None:
                 pass
             else:
                 plt.ylim(ylim)
             plt.grid()
             plt.tight_layout()
             if s.W.save_mode:
-                plt.savefig(f"out{s.W.name}/tsd_traj_links_{'-'.join([s.W.get_link(l).name for l in links])}.png")
+                if len(links) == 1:
+                    plt.savefig(f"out{s.W.name}/tsd_traj_{s.W.get_link(links[0]).name}.png")
+                else:
+                    plt.savefig(f"out{s.W.name}/tsd_traj_links_{'-'.join([s.W.get_link(l).name for l in links])}.png")
             if s.W.show_mode:
                 plt.show()
             else:
                 plt.close("all")
 
     @catch_exceptions_and_warn()
     def cumulative_curves(s, links=None, figsize=(6,4)):
@@ -561,15 +550,15 @@
         detailed : int, optional
             Determines the level of detail in the visualization.
             If set to 1, the link internals (cell) are displayed in detail.
             If set to 0, the visualization is simplified to link-level. Default is 1.
         minwidth : float, optional
             The minimum width of the link visualization. Default is 0.5.
         maxwidth : float, optional
-            The maximum width of the link visualization. Default is 12.
+            The maximum width of the link per lane visualization. Default is 12.
         left_handed : int, optional
             If set to 1, the left-handed traffic system (e.g., Japan, UK) is used. If set to 0, the right-handed one is used. Default is 1.
         tmp_anim : int, optional
             If set to 1, the visualization will be saved as a temporary animation frame. Default is 0.
         figsize : tuple of int, optional
             The size of the figure to be plotted. Default is (6, 6).
         network_font_size : int, optional
@@ -606,28 +595,28 @@
                 for i in range(xsize):
                     try:
                         k = l.k_mat[int(t/l.edie_dt), i+1]
                         v = l.v_mat[int(t/l.edie_dt), i+1]
                     except:
                         warnings.warn(f"invalid time {t} is specified for network visualization", UserWarning)
                         return -1
-                    lw[i] = k*l.delta*(maxwidth-minwidth)+minwidth
+                    lw[i] = k*l.delta*(maxwidth*l.lanes-minwidth)+minwidth
                     c[i] = plt.colormaps["viridis"](v/l.u)
                 xmid = [((xsize-i)*x1+(i+1)*x2)/(xsize+1)+vx for i in range(xsize)]
                 ymid = [((xsize-i)*y1+(i+1)*y2)/(xsize+1)+vy for i in range(xsize)]
                 plt.plot([x1]+xmid+[x2], [y1]+ymid+[y2], "k--", lw=0.25, zorder=5)
                 for i in range(xsize-1):
                     plt.plot([xmid[i], xmid[i+1]], [ymid[i], ymid[i+1]], c=c[i], lw=lw[i], zorder=6)
                 if network_font_size > 0:
                     plt.text(xmid[int(len(xmid)/2)], ymid[int(len(xmid)/2)], l.name, c="b", zorder=20, fontsize=network_font_size)
             else:
                 #簡略モード
                 k = (l.cum_arrival[int(t/s.W.DELTAT)]-l.cum_departure[int(t/s.W.DELTAT)])/l.length
                 v = l.length/l.traveltime_instant[int(t/s.W.DELTAT)]
-                width = k*l.delta*(maxwidth-minwidth)+minwidth
+                width = k*l.delta*(maxwidth*l.lanes-minwidth)+minwidth
                 c = plt.colormaps["viridis"](v/l.u)
                 xmid1, ymid1 = (2*x1+x2)/3+vx, (2*y1+y2)/3+vy
                 xmid2, ymid2 = (x1+2*x2)/3+vx, (y1+2*y2)/3+vy
                 plt.plot([x1, xmid1, xmid2, x2], [y1, ymid1, ymid2, y2], "k--", lw=0.25, zorder=5)
                 plt.plot([x1, xmid1, xmid2, x2], [y1, ymid1, ymid2, y2], c=c, lw=width, zorder=6, solid_capstyle="butt")
                 if network_font_size > 0:
                     plt.text(xmid1, ymid1, l.name, c="b", zorder=20, fontsize=network_font_size)
@@ -710,15 +699,16 @@
         maxx += buffer
         minx -= buffer
         maxy += buffer
         miny -= buffer
 
         img = Image.new("RGBA", (int(maxx-minx), int(maxy-miny)), (255, 255, 255, 255))
         draw = ImageDraw.Draw(img)
-        font_data = read_binary('uxsim.files', 'HackGen-Regular.ttf') 
+        
+        font_data = load_font_data()
         font_file_like = io.BytesIO(font_data)
         if network_font_size > 0:
             font = ImageFont.truetype(font_file_like, int(network_font_size))
 
         def flip(y):
             return img.size[1]-y
 
@@ -740,15 +730,15 @@
                 draw.text((xmid1, flip(ymid1)), l.name, font=font, fill="blue", anchor="mm")
 
         for n in s.W.NODES:
             if network_font_size > 0:
                 draw.text(((n.x)*coef-minx, flip((n.y)*coef-miny)), n.name, font=font, fill="green", anchor="mm")
                 draw.text(((n.x)*coef-minx, flip((n.y)*coef-miny)), n.name, font=font, fill="green", anchor="mm")
 
-        font_data = read_binary('uxsim.files', 'HackGen-Regular.ttf') 
+        font_data = load_font_data()
         font_file_like = io.BytesIO(font_data)
         font = ImageFont.truetype(font_file_like, int(30))
         draw.text((img.size[0]/2,20), f"t = {t :>8} (s)", font=font, fill="black", anchor="mm")
 
         img = img.resize((int((maxx-minx)/scale), int((maxy-miny)/scale)), resample=Resampling.LANCZOS)
         if image_return:
             return img
@@ -772,15 +762,15 @@
                 avev = sum(vs)/sum_vehs
             else:
                 avev = 0
 
             print(f"{s.W.TIME:>8.0f} s| {sum_vehs:>8.0f} vehs|  {avev:>4.1f} m/s| {time.time()-s.W.sim_start_time:8.2f} s", flush=True)
 
     @catch_exceptions_and_warn()
-    def network_anim(s, animation_speed_inverse=10, detailed=0, minwidth=0.5, maxwidth=12, left_handed=1, figsize=(6,6), node_size=2, network_font_size=20, timestep_skip=24):
+    def network_anim(s, animation_speed_inverse=10, detailed=0, minwidth=0.5, maxwidth=12, left_handed=1, figsize=(6,6), node_size=2, network_font_size=20, timestep_skip=24, file_name=None):
         """
         Generates an animation of the entire transportation network and its traffic states over time.
 
         Parameters
         ----------
         animation_speed_inverse : int, optional
             The inverse of the animation speed. A higher value will result in a slower animation. Default is 10.
@@ -799,14 +789,16 @@
             The size of the figures in the animation. Default is (6, 6).
         node_size : int, optional
             The size of the nodes in the animation. Default is 2.
         network_font_size : int, optional
             The font size for the network labels in the animation. Default is 20.
         timestep_skip : int, optional
             How many timesteps are skipped per frame. Large value means coarse and lightweight animation. Default is 8.
+        file_name : str, optional
+            The name of the file to which the animation is saved. It overrides the defauld name. Default is None.
 
         Notes
         -----
         This method generates an animation visualizing the entire transportation network and its traffic conditions over time.
         The animation provides information on vehicle density, velocity, link names, node locations, and more.
         The generated animation is saved to the directory `out<W.name>` with a filename based on the `detailed` parameter.
 
@@ -818,20 +810,24 @@
             if int(t/s.W.LINKS[0].edie_dt) < s.W.LINKS[0].k_mat.shape[0]:
                 if detailed:
                     #todo_later: 今後はこちらもpillowにする
                     s.network(int(t), detailed=detailed, minwidth=minwidth, maxwidth=maxwidth, left_handed=left_handed, tmp_anim=1, figsize=figsize, node_size=node_size, network_font_size=network_font_size)
                 else:
                     s.network_pillow(int(t), detailed=detailed, minwidth=minwidth, maxwidth=maxwidth, left_handed=left_handed, tmp_anim=1, figsize=figsize, node_size=node_size, network_font_size=network_font_size)
                 pics.append(Image.open(f"out{s.W.name}/tmp_anim_{t}.png"))
-        pics[0].save(f"out{s.W.name}/anim_network{detailed}.gif", save_all=True, append_images=pics[1:], optimize=False, duration=animation_speed_inverse*timestep_skip, loop=0)
+        
+        fname = f"out{s.W.name}/anim_network{detailed}.gif"
+        if file_name != None:
+            fname = file_name
+        pics[0].save(fname, save_all=True, append_images=pics[1:], optimize=False, duration=animation_speed_inverse*timestep_skip, loop=0)
         for f in glob.glob(f"out{s.W.name}/tmp_anim_*.png"):
             os.remove(f)
 
     @catch_exceptions_and_warn()
-    def network_fancy(s, animation_speed_inverse=10, figsize=6, sample_ratio=0.3, interval=5, network_font_size=0, trace_length=3, speed_coef=2):
+    def network_fancy(s, animation_speed_inverse=10, figsize=6, sample_ratio=0.3, interval=5, network_font_size=0, trace_length=3, speed_coef=2, file_name=None):
         """
         Generates a visually appealing animation of vehicles' trajectories across the entire transportation network over time.
 
         Parameters
         ----------
         animation_speed_inverse : int, optional
             The inverse of the animation speed. A higher value will result in a slower animation. Default is 10.
@@ -843,14 +839,16 @@
             The interval at which vehicle positions are sampled. Default is 5.
         network_font_size : int, optional
             The font size for the network labels in the animation. Default is 0.
         trace_length : int, optional
             The length of the vehicles' trajectory trails in the animation. Default is 3.
         speed_coef : int, optional
             A coefficient that adjusts the animation speed. Default is 2.
+        file_name : str, optional
+            The name of the file to which the animation is saved. It overrides the defauld name. Default is None.
 
         Notes
         -----
         This method generates a visually appealing animation that visualizes vehicles' trajectories across the transportation network over time.
         The animation provides information on vehicle positions, speeds, link names, node locations, and more, with Bezier curves used for smooth transitions.
         The generated animation is saved to the directory `out<W.name>` with a filename `anim_network_fancy.gif`.
 
@@ -946,15 +944,15 @@
         maxy += buffer
         miny -= buffer
 
         pics = []
         for t in tqdm(range(int(s.W.TMAX*0), int(s.W.TMAX*1), s.W.DELTAT*speed_coef)):
             img = Image.new("RGBA", (int(maxx-minx), int(maxy-miny)), (255, 255, 255, 255))
             draw = ImageDraw.Draw(img)
-            font_data = read_binary('uxsim.files', 'HackGen-Regular.ttf') 
+            font_data = load_font_data()
             font_file_like = io.BytesIO(font_data)
             if network_font_size > 0:
                 font = ImageFont.truetype(font_file_like, int(network_font_size))
 
             def flip(y):
                 return img.size[1]-y
 
@@ -973,24 +971,27 @@
                 size = 3*(1-trace["v"])
                 coords = [(l[0], flip(l[1])) for l in list(np.vstack([xs, ys]).T)]
                 draw.line(coords,
                           fill=(int(trace["c"][0]*255), int(trace["c"][1]*255), int(trace["c"][2]*255)), width=2, joint="curve")
                 draw.ellipse((xs[-1]-size, flip(ys[-1])-size, xs[-1]+size, flip(ys[-1])+size), fill=(int(trace["c"][0]*255), int(trace["c"][1]*255), int(trace["c"][2]*255)))
                 #draw.line([(x1, flip(y1)), (xmid1, flip(ymid1)), (xmid2, flip(ymid2)), (x2, flip(y2))]
 
-            font_data = read_binary('uxsim.files', 'HackGen-Regular.ttf') 
+            font_data = load_font_data()
             font_file_like = io.BytesIO(font_data)
             font = ImageFont.truetype(font_file_like, int(30))
             draw.text((img.size[0]/2,20), f"t = {t :>8} (s)", font=font, fill="black", anchor="mm")
 
             img = img.resize((int((maxx-minx)/scale), int((maxy-miny)/scale)), resample=Resampling.LANCZOS)
             img.save(f"out{s.W.name}/tmp_anim_{t}.png")
             pics.append(Image.open(f"out{s.W.name}/tmp_anim_{t}.png"))
 
-        pics[0].save(f"out{s.W.name}/anim_network_fancy.gif", save_all=True, append_images=pics[1:], optimize=False, duration=animation_speed_inverse*speed_coef, loop=0)
+        fname = f"out{s.W.name}/anim_network_fancy.gif"
+        if file_name != None:
+            fname = file_name
+        pics[0].save(fname, save_all=True, append_images=pics[1:], optimize=False, duration=animation_speed_inverse*speed_coef, loop=0)
 
         for f in glob.glob(f"out{s.W.name}/tmp_anim_*.png"):
             os.remove(f)
 
     def compute_mfd(s, links=None):
         """
         Compute network average flow and density for MFD.
@@ -1186,14 +1187,41 @@
 
     def log_vehicles_to_pandas(s):
         """
         same to `vehicles_to_pandas`, just for backward compatibility
         """
         return s.vehicles_to_pandas()
 
+    def vehicle_trip_to_pandas(s):
+        """
+        Converts the vehicle trip top to a pandas DataFrame.
+
+        Returns
+        -------
+        pd.DataFrame
+            A DataFrame containing the top of the vehicle trip logs, with the columns:
+            - 'name': the name of the vehicle (platoon).
+            - 'orig': the origin node of the vehicle's trip.
+            - 'dest': the destination node of the vehicle's trip.
+            - 'departure_time': the departure time of the vehicle.
+            - 'final_state': the final state of the vehicle.
+            - 'travel_time': the travel time of the vehicle.
+            - 'average_speed': the average speed of the vehicle.
+        """
+        out = [["name", "orig", "dest", "departure_time", "final_state", "travel_time", "average_speed"]]
+        for veh in s.W.VEHICLES.values():
+            veh_dest_name = veh.dest.name if veh.dest != None else None
+            veh_state = veh.log_state[-1]
+            veh_ave_speed = np.average([v for v in veh.log_v if v != -1])
+
+            out.append([veh.name, veh.orig.name, veh_dest_name, veh.departure_time*s.W.DELTAT, veh_state, veh.travel_time, veh_ave_speed])
+        
+        s.df_vehicle_trip = pd.DataFrame(out[1:], columns=out[0])
+        return s.df_vehicle_trip
+
     def basic_to_pandas(s):
         """
         Converts the basic stats to a pandas DataFrame.
 
         Returns
         -------
         pd.DataFrame
```

### Comparing `uxsim-1.2.0/uxsim/files/HackGen-Regular.ttf` & `uxsim-1.3.0/uxsim/files/HackGen-Regular.ttf`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/uxsim/files/Inconsolata.otf` & `uxsim-1.3.0/uxsim/files/Inconsolata.otf`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/uxsim/files/LICENSE_of_HackGen-Regular` & `uxsim-1.3.0/uxsim/files/LICENSE_of_HackGen-Regular`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/uxsim/files/Licence_of_Inconsolata.otf.txt` & `uxsim-1.3.0/uxsim/files/Licence_of_Inconsolata.otf.txt`

 * *Files identical despite different names*

### Comparing `uxsim-1.2.0/uxsim/utils.py` & `uxsim-1.3.0/uxsim/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,12 +128,25 @@
                     print(f"{lst[i]:<10}", end=" ")  # Adjust the width as necessary
                 except TypeError:
                     print(f"{str(lst[i]):<10}", end=" ")
             else:
                 print(" " * 10, end=" ")  # Adjust spacing to match the above width
         print()  # Newline after each row
 
+def display_image_in_notebook(image_path):
+    """
+    Display an image in Jupyter Notebook.
+
+    Parameters
+    ----------
+    image_path : str
+        The path to the image file to display.
+    """
+    from IPython.display import display, Image
+    with open(image_path, "rb") as f:
+        display(Image(data=f.read(), format='png'))
+
 class LoggingWarning(UserWarning):
     """
     This warns that when vehicle_logging_timestep_interval is not 1 but called vehicle logging-related functions.
     """
     pass
```

### Comparing `uxsim-1.2.0/uxsim/uxsim.py` & `uxsim-1.3.0/uxsim/uxsim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 UXsim: Macroscopic/mesoscopic traffic flow simulator in a network.
 This `uxsim.py` is the core of UXsim. It summarizes the classes and methods that are essential for the simulation.
 """
 
-import numpy as np
-import matplotlib.pyplot as plt
 import random, csv, time, math, string, warnings
 from collections import deque, OrderedDict
 from collections import defaultdict as ddict
+
+import numpy as np
+import matplotlib.pyplot as plt
 from scipy.sparse.csgraph import floyd_warshall
+import dill as pickle
 
 from .analyzer import *
-from .utils  import *
+from .utils import *
 
 class Node:
     """
     Node in a network.
     """
     def __init__(s, W, name, x, y, signal=[0], signal_offset=0, flow_capacity=None, auto_rename=False, number_of_lanes=None):
         """
@@ -370,62 +372,69 @@
             Capacity for inflow to the link.
         merge_priority : float
             The priority of the link when merging at the downstream node.
 
         Notes
         -----
         Traffic Flow Model:
+
         - The link model follows a multi-lane, single-pipe approach where FIFO is guaranteed per link and no lane changing occurs.
         - Fundamental diagram parameters such as free_flow_speed, jam_density (or jam_density_per_lane), and number_of_lanes determine the link's flow characteristics. Reaction time of drivers `REACTION_TIME` is a grobal parameter.
         - Real-time link status for external reference is maintained with attributes `speed`, `density`, `flow`, `num_vehicles`, and `num_vehicles_queue`.
 
         Traffic Flow Model Parameters:
+
         - Their definition is illustrated as https://toruseo.jp/UXsim/docs/_images/fundamental_diagram.png
         - If you are not familiar to the traffic flow theory, it is recommended that you adjust only `free_flow_speed` and `number_of_lanes` for the traffic flow model parameters, leaving the other parameters at their default values.
 
         Capacity and Bottlenecks:
+
         - The `capacity_out` and `capacity_in` parameters set the outflow and inflow capacities of the link. If not provided, the capacities are unlimited.
         - These capacities can represent bottlenecks at the beginning or end of the link.
 
         Connection to Node Model:
+
         - At the downstream end of a sending link, vehicles in all lanes have the right to be sent out, but FIFO order is maintained.
         - At the upstream end of a receiving link, all lanes can accept vehicles.
 
         Parameter Adjustments:
+
         - Some traffic flow model parameters like `free_flow_speed`, `jam_density`, `capacity_out`, `capacity_in`, and `merge_priority` can be altered during simulation to reflect changing conditions.
             
         Details on Multi-lane model:
+
         - Link model:
             - Multiple lanes with single-pipe model. FIFO is guaranteed per link. No lane changing.
             - Links have a `lanes` attribute representing the number of lanes. 
             - Each vehicle has a `lane` attribute.
             - Each vehicle follows the leader vehicle in the same lane, i.e., the vehicle `lanes` steps ahead on the link.
         - Node model: 
             - Sending links:
                 - Vehicles in all lanes at the downstream end of the link have the right to be sent out.
                 - However, to ensure link FIFO, vehicles are tried to be sent out in the order they entered the link. If a vehicle cannot be accepted, the outflow from that link stops.
             - Receiving links:  
                 - All lanes at the upstream end of the link can accept vehicles.
 
-        Details on Fundamental diagram parameters (*: input, **: alternative input):
-        - *free_flow_speed (m/s)
-        - *jam_density (veh/m/LINK)  
-        - **jam_density_per_lane (veh/m/lane)
-        - *lanes, number_of_lane (lane) 
+        Details on Fundamental diagram parameters (+: input, ++: alternative input):
+
+        - free_flow_speed (m/s)+
+        - jam_density (veh/m/LINK)+
+        - jam_density_per_lane (veh/m/lane)++
+        - lanes, number_of_lane (lane)+
         - tau: y-intercept of link FD (s/veh*LINK)
-        - REACTION_TIME (s/veh*lane) 
+        - REACTION_TIME, World.reaction_time (s/veh*lane) 
         - w (m/s)
         - capacity (veh/s/LINK)
         - capacity_per_lane (veh/s/lane)
         - delta: minimum spacing (m/veh*LINK)
         - delta_per_lane: minimum spacing in lane (m/veh*lane) 
         - q_star: capacity (veh/s/LINK)
         - k_star: critical density (veh/s/LINK)
-        - *capacity_in, capacity_out: bottleneck capacity at beginning/end of link (veh/s/LINK)
-        - *Node.flow_capacity: node flow capacity (veh/s/LINK-LIKE) 
+        - capacity_in, capacity_out: bottleneck capacity at beginning/end of link (veh/s/LINK)+
+        - Node.flow_capacity: node flow capacity (veh/s/LINK-LIKE)+
         """
 
         s.W = W
         #起点・終点ノード
         s.start_node = s.W.get_node(start_node)
         s.end_node = s.W.get_node(end_node)
 
@@ -512,14 +521,15 @@
         s._num_vehicles = -1 #車両数
         s._num_vehicles_queue = -1 #自由流速度未満の車両数
 
         #より正確な車両軌跡
         s.tss = []
         s.xss = []
         s.cs = []
+        s.ls = []
         s.names = []
 
         if eular_dx == None:
             s.eular_dx = s.length/10
             if s.eular_dx < s.u*s.W.DELTAT:
                 s.eular_dx = s.u*s.W.DELTAT
 
@@ -840,14 +850,15 @@
         #ログなど
         s.log_t = [] #時刻
         s.log_state = [] #状態
         s.log_link = [] #リンク
         s.log_x = [] #位置
         s.log_s = [] #車頭距離
         s.log_v = [] #現在速度
+        s.log_lane = [] #車線
         s.color = (random.random(), random.random(), random.random())
 
         s.log_t_link = [[int(s.departure_time*s.W.DELTAT), "home"]] #新たなリンクに入った時にその時刻とリンクのみを保存．経路分析用
 
         s.attribute = attribute
 
         s.id = len(s.W.VEHICLES)
@@ -1060,14 +1071,36 @@
                 if order == -1:
                     s.dest_list.append(s.W.get_node(dest))
                 else:
                     s.dest_list.insert(order, s.W.get_node(dest))
         else:
             raise ValueError(f"Vehicle {s.name} is not in taxi mode. Cannot add destination.")
     
+    def set_links_prefer(s, links):
+        """
+        Set the links the vehicle prefers.
+
+        Parameters
+        ----------
+        links : list of str
+            The list of link names the vehicle prefers.
+        """
+        s.links_prefer = [s.W.get_link(l) for l in links]
+    
+    def set_links_avoid(s, links):
+        """
+        Set the links the vehicle avoids.
+
+        Parameters
+        ----------
+        links : list of str
+            The list of link names the vehicle avoids.
+        """
+        s.links_avoid = [s.W.get_link(l) for l in links]
+
     def add_dests(s, dests):
         """
         Add multiple destinations to the vehicle's destination list.
 
         Parameters
         ----------
         dests : list of str | Node
@@ -1132,27 +1165,29 @@
 
                     s.log_t.append(s.W.T*s.W.DELTAT)
                     s.log_state.append(s.state)
                     s.log_link.append(-1)
                     s.log_x.append(-1)
                     s.log_s.append(-1)
                     s.log_v.append(-1)
+                    s.log_lane.append(-1)
 
                     if s.state == "wait":
                         s.W.analyzer.average_speed_count += 1
                         s.W.analyzer.average_speed += 0
                 else:
                     if len(s.log_link) == 0 or s.log_link[-1] != s.link:
                         s.log_t_link.append([s.W.T*s.W.DELTAT, s.link])
 
                     s.log_t.append(s.W.T*s.W.DELTAT)
                     s.log_state.append(s.state)
                     s.log_link.append(s.link)
                     s.log_x.append(s.x)
                     s.log_v.append(s.v)
+                    s.log_lane.append(s.lane)
                     if s.leader != None and s.link == s.leader.link:
                         s.log_s.append(s.leader.x-s.x)
                     else:
                         s.log_s.append(-1)
 
                     s.W.analyzer.average_speed_count += 1
                     s.W.analyzer.average_speed += (s.v - s.W.analyzer.average_speed)/s.W.analyzer.average_speed_count
@@ -1997,14 +2032,25 @@
         plt.tight_layout()
         if W.save_mode:
             plt.savefig(f"out{W.name}/network.png")
         if W.show_mode:
             plt.show()
         else:
             plt.close("all")
+    
+    def copy(W):
+        """
+        Copy the World object.
+
+        Returns
+        -------
+        World object
+            The copied World object.
+        """
+        return pickle.loads(pickle.dumps(W))
 
 
 class Route:
     """
     Class for a route that store concective links.
     """
     def __init__(s, W, links, name="", trust_input=False):
@@ -2015,14 +2061,25 @@
         ----------
         links : list
             List of links. The contents are Link objects.
         links_name : list
             List of name of links. The contents are str.
         trust_input : bool
             True if you trust the `links` in order to reduce the computation cost by omitting verification.
+
+        Examples
+        --------
+        >>> route = Route(W, ["l1", "l2", "l3"])
+        ... vehicle_object.links_prefer = route
+        This will enforce the vehicle to travel the route if the route covers the entire links between the OD nodes of the vehicle.
+
+        >>> route = Route(W, ["l1", "l2", "l3"])
+        ... for link in route:
+        ...     print(link)
+        This will print the links in the route.
         """
         s.W = W
         s.name = name
         s.links = []
         if trust_input == False:
             #入力データを検査する場合
             for i in range(0, len(links)-1):
@@ -2038,14 +2095,23 @@
             #検査せずそのまま使用（計算コスト削減）
             s.links = links
         s.links_name = [l.name for l in s.links]
 
     def __repr__(s):
         return f"<Route {s.name}: {s.links}>"
 
+    def __iter__(s):
+        """
+        Override `iter()` function. Iterate the links of the route.
+        """
+        return iter(s.links)
+    
+    def __len__(s):
+        return len(s.links)
+    
     def __eq__(self, other):
         """
         Override `==` operator. If the links of two route are the same, then the routes are the same.
         """
         if isinstance(other, Route):
             return self.links == other.links
         return NotImplemented
```

### Comparing `uxsim-1.2.0/uxsim.egg-info/PKG-INFO` & `uxsim-1.3.0/uxsim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: uxsim
-Version: 1.2.0
+Version: 1.3.0
 Summary: UXsim: traffic flow simulator
 Author-email: Toru Seo <seo.t.aa@m.titech.ac.jp>
 License: MIT License
 Project-URL: Homepage, https://github.com/toruseo/UXsim
 Project-URL: Documentation, https://toruseo.jp/UXsim/docs
 Project-URL: Issues, https://github.com/toruseo/UXsim/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.21.5
 Requires-Dist: matplotlib>=3.5.2
 Requires-Dist: pillow>=9.2.0
 Requires-Dist: tqdm>=4.64.1
 Requires-Dist: scipy>=1.9.1
 Requires-Dist: pandas>=1.4.4
 Requires-Dist: PyQt5>=5.15.7
+Requires-Dist: dill>=0.3.8
 
 # UXsim: Network traffic flow simulator in pure Python
 
 [![PyPi](https://img.shields.io/pypi/v/uxsim.svg)](https://pypi.python.org/pypi/uxsim)
 [![Demo in Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/toruseo/UXsim/blob/main/demos_and_examples/demo_notebook_05en_for_google_colab.ipynb)
 [![arXiv](https://img.shields.io/badge/arXiv-2309.17114-b31b1b.svg)](http://dx.doi.org/10.48550/arXiv.2309.17114)
 [![Static Badge](https://img.shields.io/badge/readme-English%20%F0%9F%87%BA%F0%9F%87%B8%20-%20darkblue)](https://github.com/toruseo/UXsim/blob/main/README.md)
@@ -218,16 +223,16 @@
 
 ## Terms of Use & License
 
 UXsim is released under the MIT License. You are free to use it as long as the source is acknowledged.
 
 When publishing works based on UXsim, please cite:
 
-- Toru Seo. Macroscopic Traffic Flow Simulation: Fundamental Mathematical Theory and Python Implementation. Corona Publishing Co., Ltd., 2023.
-- Toru Seo. UXsim: An open source macroscopic and mesoscopic traffic simulator in Python-a technical overview. arXiv preprint arXiv: 2309.17114, 2023
+- Toru Seo. [Macroscopic Traffic Flow Simulation: Fundamental Mathematical Theory and Python Implementation](https://toruseo.github.io/misc/MacroTrafficSim_English_summary.pdf). Corona Publishing Co., Ltd., 2023.
+- Toru Seo. [UXsim: An open source macroscopic and mesoscopic traffic simulator in Python-a technical overview](http://dx.doi.org/10.48550/arXiv.2309.17114). arXiv preprint arXiv: 2309.17114, 2023
 
 ## Contributing and Discussion
 
 Contributions are welcome!
 Please see the [Contributing Guideline](https://github.com/toruseo/UXsim/blob/main/.github/CONTRIBUTING.md).
 
 If you have any questions or suggestions, please post them to the [Issues](https://github.com/toruseo/UXsim/issues) or [Discussions](https://github.com/toruseo/UXsim/discussions) (in English or Japanese).
```

### Comparing `uxsim-1.2.0/uxsim.egg-info/SOURCES.txt` & `uxsim-1.3.0/uxsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

