# Comparing `tmp/monteprediction-1.0.8.tar.gz` & `tmp/monteprediction-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monteprediction-1.0.8.tar", last modified: Wed May  8 02:25:08 2024, max compression
+gzip compressed data, was "monteprediction-1.0.9.tar", last modified: Sat May 11 01:26:38 2024, max compression
```

## Comparing `monteprediction-1.0.8.tar` & `monteprediction-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:25:08.193405 monteprediction-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-08 02:24:56.000000 monteprediction-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-08 02:25:08.193405 monteprediction-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-08 02:24:56.000000 monteprediction-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:25:08.193405 monteprediction-1.0.8/monteprediction/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-08 02:24:56.000000 monteprediction-1.0.8/monteprediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 02:24:56.000000 monteprediction-1.0.8/monteprediction/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-08 02:24:56.000000 monteprediction-1.0.8/monteprediction/calendarutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-08 02:24:56.000000 monteprediction-1.0.8/monteprediction/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-08 02:24:56.000000 monteprediction-1.0.8/monteprediction/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-08 02:24:56.000000 monteprediction-1.0.8/monteprediction/truth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 02:24:56.000000 monteprediction-1.0.8/monteprediction/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:25:08.193405 monteprediction-1.0.8/monteprediction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-08 02:25:08.000000 monteprediction-1.0.8/monteprediction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-08 02:25:08.000000 monteprediction-1.0.8/monteprediction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 02:25:08.000000 monteprediction-1.0.8/monteprediction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 02:25:08.000000 monteprediction-1.0.8/monteprediction.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 02:25:08.000000 monteprediction-1.0.8/monteprediction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 02:25:08.000000 monteprediction-1.0.8/monteprediction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 02:25:08.193405 monteprediction-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-08 02:24:56.000000 monteprediction-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:25:08.193405 monteprediction-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-08 02:24:56.000000 monteprediction-1.0.8/tests/test_calendarutil.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-08 02:24:56.000000 monteprediction-1.0.8/tests/test_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:26:38.985567 monteprediction-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-11 01:26:30.000000 monteprediction-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-11 01:26:38.985567 monteprediction-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-11 01:26:30.000000 monteprediction-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:26:38.981567 monteprediction-1.0.9/monteprediction/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-11 01:26:30.000000 monteprediction-1.0.9/monteprediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-11 01:26:30.000000 monteprediction-1.0.9/monteprediction/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-11 01:26:30.000000 monteprediction-1.0.9/monteprediction/calendarutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-11 01:26:30.000000 monteprediction-1.0.9/monteprediction/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-11 01:26:30.000000 monteprediction-1.0.9/monteprediction/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-11 01:26:30.000000 monteprediction-1.0.9/monteprediction/truth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-11 01:26:30.000000 monteprediction-1.0.9/monteprediction/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:26:38.985567 monteprediction-1.0.9/monteprediction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-11 01:26:38.000000 monteprediction-1.0.9/monteprediction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-11 01:26:38.000000 monteprediction-1.0.9/monteprediction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:26:38.000000 monteprediction-1.0.9/monteprediction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-11 01:26:38.000000 monteprediction-1.0.9/monteprediction.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 01:26:38.000000 monteprediction-1.0.9/monteprediction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 01:26:38.000000 monteprediction-1.0.9/monteprediction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 01:26:38.985567 monteprediction-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-11 01:26:30.000000 monteprediction-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:26:38.985567 monteprediction-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-11 01:26:30.000000 monteprediction-1.0.9/tests/test_calendarutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-11 01:26:30.000000 monteprediction-1.0.9/tests/test_scoring.py
```

### Comparing `monteprediction-1.0.8/LICENSE` & `monteprediction-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.8/PKG-INFO` & `monteprediction-1.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: monteprediction
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Weekly Monte Carlo Game
 Home-page: https://github.com/microprediction/monteprediction
 Author: microprediction
 Author-email: peter.cotton@microprediction.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: yfinance
+Requires-Dist: python-dateutil
 
 # monteprediction
 Monte Prediction Utilities
```

### Comparing `monteprediction-1.0.8/monteprediction/scoring.py` & `monteprediction-1.0.9/monteprediction/scoring.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.8/monteprediction/submission.py` & `monteprediction-1.0.9/monteprediction/submission.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.8/monteprediction/truth.py` & `monteprediction-1.0.9/monteprediction/truth.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.8/monteprediction/verification.py` & `monteprediction-1.0.9/monteprediction/verification.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.8/monteprediction.egg-info/PKG-INFO` & `monteprediction-1.0.9/monteprediction.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: monteprediction
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Weekly Monte Carlo Game
 Home-page: https://github.com/microprediction/monteprediction
 Author: microprediction
 Author-email: peter.cotton@microprediction.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: yfinance
+Requires-Dist: python-dateutil
 
 # monteprediction
 Monte Prediction Utilities
```

### Comparing `monteprediction-1.0.8/setup.py` & `monteprediction-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="monteprediction",
-    version="1.0.8",
+    version="1.0.9",
     description="A Weekly Monte Carlo Game",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/microprediction/monteprediction",
     author="microprediction",
     author_email="peter.cotton@microprediction.com",
     license="MIT",
@@ -20,14 +20,14 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
     ],
     packages=["monteprediction"],
     test_suite='pytest',
     tests_require=['pytest'],
     include_package_data=True,
-    install_requires=['numpy','pandas','yfinance'],
+    install_requires=['numpy','pandas','yfinance','python-dateutil'],
     entry_points={
         "console_scripts": [
             "monteprediction=monteprediction.__main__:main",
         ]
     },
 )
```

### Comparing `monteprediction-1.0.8/tests/test_calendarutil.py` & `monteprediction-1.0.9/tests/test_calendarutil.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.8/tests/test_scoring.py` & `monteprediction-1.0.9/tests/test_scoring.py`

 * *Files identical despite different names*

