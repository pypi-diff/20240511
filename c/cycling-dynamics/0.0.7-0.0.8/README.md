# Comparing `tmp/cycling_dynamics-0.0.7.tar.gz` & `tmp/cycling_dynamics-0.0.8.tar.gz`

## Comparing `cycling_dynamics-0.0.7.tar` & `cycling_dynamics-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,31 @@
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/requirements.txt
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/ruff.toml
--rw-r--r--   0        0        0  4361810 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/note_books/Critical Power.ipynb
--rw-r--r--   0        0        0   290283 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/note_books/examples.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/src/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/src/cycling_dynamics/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/src/cycling_dynamics/__init__.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/src/cycling_dynamics/calc.py
--rw-r--r--   0        0        0    12458 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/src/cycling_dynamics/critical_power.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/src/cycling_dynamics/load_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/src/cycling_dynamics/models.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/src/cycling_dynamics/plots.py
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/src/cycling_dynamics/stats.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/tests/test_critical_power.py
--rw-r--r--   0        0        0   140591 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT ROAM 3FF5-53-0.fit
--rw-r--r--   0        0        0   140591 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT_ROAM_3FF5-53-0.fit
--rw-r--r--   0        0        0   152253 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT ROAM 3FF5-54-0.fit
--rw-r--r--   0        0        0   152253 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT_ROAM_3FF5-54-0.fit
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/tests/test_data/power_profile_2.csv
--rw-r--r--   0        0        0   197110 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/tests/test_data/vincent_lap_1_24HOP_14012433014_ACTIVITY.fit
--rw-r--r--   0        0        0   186596 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/tests/test_data/vincent_lap_2_24HOP_14010180820_ACTIVITY.fit
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/LICENSE.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/README.md
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/qodana.yaml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/ruff.toml
+-rw-r--r--   0        0        0   660177 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/note_books/Critical Power.ipynb
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/note_books/Surface.ipynb
+-rw-r--r--   0        0        0   290283 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/note_books/examples.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/__init__.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/calc.py
+-rw-r--r--   0        0        0    12441 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/critical_power.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/load_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/models.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/plots.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/stats.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/surface.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_critical_power.py
+-rw-r--r--   0        0        0   140591 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT ROAM 3FF5-53-0.fit
+-rw-r--r--   0        0        0   140591 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT_ROAM_3FF5-53-0.fit
+-rw-r--r--   0        0        0   152253 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT ROAM 3FF5-54-0.fit
+-rw-r--r--   0        0        0   152253 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT_ROAM_3FF5-54-0.fit
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/power_profile_2.csv
+-rw-r--r--   0        0        0   197110 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/vincent_lap_1_24HOP_14012433014_ACTIVITY.fit
+-rw-r--r--   0        0        0   186596 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/vincent_lap_2_24HOP_14010180820_ACTIVITY.fit
+-rw-r--r--   0        0        0   431114 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/vincent_mtb_id_surface_14517623900_ACTIVITY.fit
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/LICENSE.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/README.md
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/PKG-INFO
```

### Comparing `cycling_dynamics-0.0.7/ruff.toml` & `cycling_dynamics-0.0.8/ruff.toml`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/note_books/examples.ipynb` & `cycling_dynamics-0.0.8/note_books/examples.ipynb`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/src/cycling_dynamics/calc.py` & `cycling_dynamics-0.0.8/src/cycling_dynamics/calc.py`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/src/cycling_dynamics/critical_power.py` & `cycling_dynamics-0.0.8/src/cycling_dynamics/critical_power.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Critical power related code"""
 
 import logging
 import warnings
 from dataclasses import asdict, dataclass
 
 import pandas as pd
-from cycling_dynamics.load_data import load_fit_file
+from load_data import load_fit_file
 
 logging.basicConfig(level=logging.INFO)
 
 
 @dataclass
 class CPPoint:
     """Dataclass to hold critical power data"""
```

### Comparing `cycling_dynamics-0.0.7/src/cycling_dynamics/load_data.py` & `cycling_dynamics-0.0.8/src/cycling_dynamics/load_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def load_fit_file(file_path, add_metrics=True, rolling_window=30) -> pd.DataFrame:
     logging.info("Loading FIT file")
     stream = Stream.from_file(file_path)
     decoder = Decoder(stream)
     if not decoder.is_fit():
         logging.error(f"File is not FIT: {file_path}")
-        raise f"File is not FIT: {file_path}"
+        raise ValueError("File is not FIT: {file_path}")
     messages, errors = decoder.read()
     if errors:
         logging.error(f"Errors: {errors}")
         raise f"Errors: {errors}"
     df = pd.DataFrame(messages["record_mesgs"])
     df["position_lat"] = df["position_lat"] / 1e7
     df["position_long"] = df["position_long"] / 1e7
```

### Comparing `cycling_dynamics-0.0.7/src/cycling_dynamics/plots.py` & `cycling_dynamics-0.0.8/src/cycling_dynamics/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 
 
 def plot_critical_power_intensity(
-    df, width: int = 15, intervals: list[int, ...] = [15, 30, 60, 120, 300, 600, 900, 1200]
+    df, width: int = 15, intervals: list[int, ...] = (15, 30, 60, 120, 300, 600, 900, 1200)
 ) -> px.bar:
     """Plot the critical power intensity
     df: this is the dataframe from get_critical_power_intensity(df, cp=None)
     """
     if "seconds" not in df.columns:
         df["seconds"] = df.index + 1
     number_of_intervals = len(intervals)
```

### Comparing `cycling_dynamics-0.0.7/src/cycling_dynamics/stats.py` & `cycling_dynamics-0.0.8/src/cycling_dynamics/stats.py`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/tests/test_critical_power.py` & `cycling_dynamics-0.0.8/tests/test_critical_power.py`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT ROAM 3FF5-53-0.fit` & `cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT ROAM 3FF5-53-0.fit`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT_ROAM_3FF5-53-0.fit` & `cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT_ROAM_3FF5-53-0.fit`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT ROAM 3FF5-54-0.fit` & `cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT ROAM 3FF5-54-0.fit`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT_ROAM_3FF5-54-0.fit` & `cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT_ROAM_3FF5-54-0.fit`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/tests/test_data/power_profile_2.csv` & `cycling_dynamics-0.0.8/tests/test_data/power_profile_2.csv`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/tests/test_data/vincent_lap_1_24HOP_14012433014_ACTIVITY.fit` & `cycling_dynamics-0.0.8/tests/test_data/vincent_lap_1_24HOP_14012433014_ACTIVITY.fit`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/tests/test_data/vincent_lap_2_24HOP_14010180820_ACTIVITY.fit` & `cycling_dynamics-0.0.8/tests/test_data/vincent_lap_2_24HOP_14010180820_ACTIVITY.fit`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/.gitignore` & `cycling_dynamics-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/LICENSE.md` & `cycling_dynamics-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/README.md` & `cycling_dynamics-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.7/pyproject.toml` & `cycling_dynamics-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "cycling-dynamics"
 dynamic = ["version"]
 description = 'Cycling (Bicycling) models of motion, air drag, rolling resistance, power calculations.'
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.12"
 license = "MIT"
 keywords = ["cycling", "bicycle", "dynamics", "speed", "Rolling Resistance", "Air Resistance", "Calculations", "Marginal Gains"]
 authors = [
   { name = "Vincent Davis", email = "v@heteroskedastic.org" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["numpy==1.26.4",
-    "pandas==2.2.1",
-    "pyarrow==15.0.2",
-    "matplotlib==3.8.3",
+    "pandas>=2.2",
+    "pyarrow>=16.0",
+    "matplotlib>=3.8.3",
     "garmin-fit-sdk==21.133.0",
-    "plotly==5.20.0",
+    "plotly>=5.20.0",
 ]
 
 [project.urls]
 Documentation = "https://github.com/vincentdavis/cycling-dynamics#readme"
 Issues = "https://github.com/vincentdavis/cycling-dynamics/issues"
 Source = "https://github.com/vincentdavis/cycling-dynamics"
```

### Comparing `cycling_dynamics-0.0.7/PKG-INFO` & `cycling_dynamics-0.0.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: cycling-dynamics
-Version: 0.0.7
+Version: 0.0.8
 Summary: Cycling (Bicycling) models of motion, air drag, rolling resistance, power calculations.
 Project-URL: Documentation, https://github.com/vincentdavis/cycling-dynamics#readme
 Project-URL: Issues, https://github.com/vincentdavis/cycling-dynamics/issues
 Project-URL: Source, https://github.com/vincentdavis/cycling-dynamics
 Author-email: Vincent Davis <v@heteroskedastic.org>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: Air Resistance,Calculations,Marginal Gains,Rolling Resistance,bicycle,cycling,dynamics,speed
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.11
+Requires-Python: >=3.12
 Requires-Dist: garmin-fit-sdk==21.133.0
-Requires-Dist: matplotlib==3.8.3
+Requires-Dist: matplotlib>=3.8.3
 Requires-Dist: numpy==1.26.4
-Requires-Dist: pandas==2.2.1
-Requires-Dist: plotly==5.20.0
-Requires-Dist: pyarrow==15.0.2
+Requires-Dist: pandas>=2.2
+Requires-Dist: plotly>=5.20.0
+Requires-Dist: pyarrow>=16.0
 Description-Content-Type: text/markdown
 
 # Cycling Dynamics
 Cycling (Bicycling) models of motion, air drag, rolling resistance, power calculations.
 
 This project is in activly being developed and has incomplete methods, models, stats and functions.
```

