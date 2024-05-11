# Comparing `tmp/project-arrakis-0.1.tar.gz` & `tmp/project_arrakis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project-arrakis-0.1.tar", last modified: Sun Aug  6 21:59:25 2023, max compression
+gzip compressed data, was "project_arrakis-0.1.1.tar", last modified: Sat May 11 17:58:39 2024, max compression
```

## Comparing `project-arrakis-0.1.tar` & `project_arrakis-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2023-08-06 21:59:25.978297 project-arrakis-0.1/
--rw-r--r--   0 kal        (501) staff       (20)      575 2023-08-06 21:59:25.977328 project-arrakis-0.1/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)      514 2023-08-06 21:44:50.000000 project-arrakis-0.1/README.md
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2023-08-06 21:59:25.922206 project-arrakis-0.1/project_arrakis.egg-info/
--rw-r--r--   0 kal        (501) staff       (20)      575 2023-08-06 21:59:25.000000 project-arrakis-0.1/project_arrakis.egg-info/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)      830 2023-08-06 21:59:25.000000 project-arrakis-0.1/project_arrakis.egg-info/SOURCES.txt
--rw-r--r--   0 kal        (501) staff       (20)        1 2023-08-06 21:59:25.000000 project-arrakis-0.1/project_arrakis.egg-info/dependency_links.txt
--rw-r--r--   0 kal        (501) staff       (20)        4 2023-08-06 21:59:25.000000 project-arrakis-0.1/project_arrakis.egg-info/top_level.txt
--rw-r--r--   0 kal        (501) staff       (20)       38 2023-08-06 21:59:25.978525 project-arrakis-0.1/setup.cfg
--rw-r--r--   0 kal        (501) staff       (20)      946 2023-08-06 21:58:13.000000 project-arrakis-0.1/setup.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2023-08-06 21:59:25.922522 project-arrakis-0.1/src/
--rwx------   0 kal        (501) staff       (20)      122 2023-08-06 13:37:24.000000 project-arrakis-0.1/src/__init__.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2023-08-06 21:59:25.926642 project-arrakis-0.1/src/function/
--rwx------   0 kal        (501) staff       (20)       80 2023-08-06 04:45:46.000000 project-arrakis-0.1/src/function/__init__.py
--rwx------   0 kal        (501) staff       (20)     1922 2022-01-02 13:23:15.000000 project-arrakis-0.1/src/function/timer.py
--rw-r--r--   0 kal        (501) staff       (20)     3469 2023-07-27 06:34:04.000000 project-arrakis-0.1/src/function/variables.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2023-08-06 21:59:25.930567 project-arrakis-0.1/src/io/
--rwx------   0 kal        (501) staff       (20)       88 2023-08-06 04:42:12.000000 project-arrakis-0.1/src/io/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    11420 2023-04-04 12:53:58.000000 project-arrakis-0.1/src/io/dataio.py
--rw-r--r--   0 kal        (501) staff       (20)    23028 2023-08-01 19:15:39.000000 project-arrakis-0.1/src/io/plot3dio.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2023-08-06 21:59:25.959487 project-arrakis-0.1/src/streamlines/
--rwx------   0 kal        (501) staff       (20)      251 2023-08-06 04:45:45.000000 project-arrakis-0.1/src/streamlines/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    25593 2023-08-03 22:30:30.000000 project-arrakis-0.1/src/streamlines/integration.py
--rw-r--r--   0 kal        (501) staff       (20)    13049 2023-08-01 19:15:39.000000 project-arrakis-0.1/src/streamlines/interpolation.py
--rwxr-xr-x   0 kal        (501) staff       (20)    14886 2023-07-26 07:12:35.000000 project-arrakis-0.1/src/streamlines/search.py
--rw-r--r--   0 kal        (501) staff       (20)     5981 2023-08-06 12:27:44.000000 project-arrakis-0.1/src/streamlines/stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)    36856 2023-08-05 16:37:39.000000 project-arrakis-0.1/src/streamlines/streamlines.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2023-08-06 21:59:25.961678 project-arrakis-0.1/src/test_cases/
--rw-r--r--   0 kal        (501) staff       (20)       87 2023-08-06 04:45:45.000000 project-arrakis-0.1/src/test_cases/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    10903 2023-08-03 22:22:43.000000 project-arrakis-0.1/src/test_cases/oblique_shock_data.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2023-08-06 21:59:25.975309 project-arrakis-0.1/test/
--rw-r--r--   0 kal        (501) staff       (20)      940 2023-02-24 21:13:16.000000 project-arrakis-0.1/test/test_dataio.py
--rwx------   0 kal        (501) staff       (20)      576 2022-06-01 14:49:46.000000 project-arrakis-0.1/test/test_import.py
--rwx------   0 kal        (501) staff       (20)     2446 2022-03-30 08:06:27.000000 project-arrakis-0.1/test/test_integration.py
--rwx------   0 kal        (501) staff       (20)      960 2023-07-26 07:10:11.000000 project-arrakis-0.1/test/test_interpolation.py
--rw-r--r--   0 kal        (501) staff       (20)     1080 2023-08-06 04:45:45.000000 project-arrakis-0.1/test/test_oblique_shock_data.py
--rw-r--r--   0 kal        (501) staff       (20)     2059 2023-05-08 23:08:14.000000 project-arrakis-0.1/test/test_plot.py
--rw-r--r--   0 kal        (501) staff       (20)     7327 2022-12-01 20:33:33.000000 project-arrakis-0.1/test/test_plot3dio.py
--rwx------   0 kal        (501) staff       (20)     3350 2023-04-30 08:54:26.000000 project-arrakis-0.1/test/test_search.py
--rw-r--r--   0 kal        (501) staff       (20)     1955 2023-04-12 20:16:51.000000 project-arrakis-0.1/test/test_stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)     1440 2023-01-08 08:41:04.000000 project-arrakis-0.1/test/test_terminal_run.py
--rwx------   0 kal        (501) staff       (20)     2829 2022-01-02 13:23:15.000000 project-arrakis-0.1/test/test_variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-11 17:58:39.266034 project_arrakis-0.1.1/
+-rwx------   0 kal        (501) staff       (20)     1093 2024-05-10 20:01:36.000000 project_arrakis-0.1.1/LICENSE
+-rw-r--r--   0 kal        (501) staff       (20)     1111 2024-05-11 17:58:39.265574 project_arrakis-0.1.1/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)      526 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/README.md
+-rw-r--r--   0 kal        (501) staff       (20)      723 2024-05-11 17:58:14.000000 project_arrakis-0.1.1/pyproject.toml
+-rw-r--r--   0 kal        (501) staff       (20)       38 2024-05-11 17:58:39.266143 project_arrakis-0.1.1/setup.cfg
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-11 17:58:39.237699 project_arrakis-0.1.1/src/
+-rw-r--r--   0 kal        (501) staff       (20)      127 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/src/__init__.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-11 17:58:39.240998 project_arrakis-0.1.1/src/function/
+-rw-r--r--   0 kal        (501) staff       (20)      109 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/src/function/__init__.py
+-rwx------   0 kal        (501) staff       (20)    12638 2024-03-16 20:12:32.000000 project_arrakis-0.1.1/src/function/plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     2034 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/src/function/timer.py
+-rw-r--r--   0 kal        (501) staff       (20)    11932 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/src/function/variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-11 17:58:39.243483 project_arrakis-0.1.1/src/io/
+-rw-r--r--   0 kal        (501) staff       (20)       91 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/src/io/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    14881 2024-05-06 14:50:43.000000 project_arrakis-0.1.1/src/io/dataio.py
+-rw-r--r--   0 kal        (501) staff       (20)    24440 2024-04-22 21:46:04.000000 project_arrakis-0.1.1/src/io/plot3dio.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-11 17:58:39.265047 project_arrakis-0.1.1/src/project_arrakis.egg-info/
+-rw-r--r--   0 kal        (501) staff       (20)     1111 2024-05-11 17:58:39.000000 project_arrakis-0.1.1/src/project_arrakis.egg-info/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)      901 2024-05-11 17:58:39.000000 project_arrakis-0.1.1/src/project_arrakis.egg-info/SOURCES.txt
+-rw-r--r--   0 kal        (501) staff       (20)        1 2024-05-11 17:58:39.000000 project_arrakis-0.1.1/src/project_arrakis.egg-info/dependency_links.txt
+-rw-r--r--   0 kal        (501) staff       (20)       44 2024-05-11 17:58:39.000000 project_arrakis-0.1.1/src/project_arrakis.egg-info/top_level.txt
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-11 17:58:39.251271 project_arrakis-0.1.1/src/streamlines/
+-rw-r--r--   0 kal        (501) staff       (20)      257 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/src/streamlines/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    34475 2024-05-07 13:44:18.000000 project_arrakis-0.1.1/src/streamlines/integration.py
+-rw-r--r--   0 kal        (501) staff       (20)    47345 2024-03-26 00:29:45.000000 project_arrakis-0.1.1/src/streamlines/interpolation.py
+-rwxr-xr-x   0 kal        (501) staff       (20)    15615 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/src/streamlines/search.py
+-rw-r--r--   0 kal        (501) staff       (20)     7539 2024-05-04 05:02:56.000000 project_arrakis-0.1.1/src/streamlines/stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)    39741 2024-05-05 02:24:25.000000 project_arrakis-0.1.1/src/streamlines/streamlines.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-11 17:58:39.254209 project_arrakis-0.1.1/src/test_cases/
+-rwx------   0 kal        (501) staff       (20)       89 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/src/test_cases/__init__.py
+-rwx------   0 kal        (501) staff       (20)    10011 2024-03-23 00:32:18.000000 project_arrakis-0.1.1/src/test_cases/oblique_shock_data.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-11 17:58:39.264273 project_arrakis-0.1.1/test/
+-rw-r--r--   0 kal        (501) staff       (20)     1019 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/test/test_dataio.py
+-rwx------   0 kal        (501) staff       (20)      576 2022-06-01 14:49:46.000000 project_arrakis-0.1.1/test/test_import.py
+-rwx------   0 kal        (501) staff       (20)     2446 2022-03-30 08:06:27.000000 project_arrakis-0.1.1/test/test_integration.py
+-rw-r--r--   0 kal        (501) staff       (20)     2103 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/test/test_interpolation.py
+-rwx------   0 kal        (501) staff       (20)     1238 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/test/test_oblique_shock_data.py
+-rw-r--r--   0 kal        (501) staff       (20)     2059 2023-08-17 08:22:42.000000 project_arrakis-0.1.1/test/test_plot.py
+-rw-r--r--   0 kal        (501) staff       (20)     7327 2024-04-08 14:56:14.000000 project_arrakis-0.1.1/test/test_plot3dio.py
+-rwx------   0 kal        (501) staff       (20)     2637 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/test/test_plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     3306 2024-01-23 01:40:32.000000 project_arrakis-0.1.1/test/test_search.py
+-rw-r--r--   0 kal        (501) staff       (20)     1955 2023-08-17 08:22:42.000000 project_arrakis-0.1.1/test/test_stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)     1440 2023-08-17 08:22:42.000000 project_arrakis-0.1.1/test/test_terminal_run.py
+-rwx------   0 kal        (501) staff       (20)     2829 2022-01-02 13:23:15.000000 project_arrakis-0.1.1/test/test_variables.py
```

### Comparing `project-arrakis-0.1/README.md` & `project_arrakis-0.1.1/README.md`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# project-arrakis
-
-python based particle tracking algorithms for CFD data
-
-A highly parallelized set of Lagrangian particle tracking (LPT) algorithms based on Python to post-process steady and unsteady CFD data. An advanced programming interface (API) is developed for uncertainty quantification of optical velocimetry data.
-
-# Installation:
-Run the following command in the terminal to install the package:
-```pip install project-arrakis```
-
-### LPT Algorithms:
-
+# project-arrakis
+
+python based particle tracking algorithms for CFD data
+
+A highly parallelized set of Lagrangian particle tracking (LPT) algorithms based on Python to post-process steady and unsteady CFD data. An advanced programming interface (API) is developed for uncertainty quantification of optical velocimetry data.
+
+# Installation:
+Run the following command in the terminal to install the package:
+```pip install project-arrakis```
+
+### LPT Algorithms:
+
 A sample code to start off is presented in main.py
```

### Comparing `project-arrakis-0.1/project_arrakis.egg-info/SOURCES.txt` & `project_arrakis-0.1.1/src/project_arrakis.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+LICENSE
 README.md
-setup.py
-project_arrakis.egg-info/PKG-INFO
-project_arrakis.egg-info/SOURCES.txt
-project_arrakis.egg-info/dependency_links.txt
-project_arrakis.egg-info/top_level.txt
+pyproject.toml
 src/__init__.py
 src/function/__init__.py
+src/function/plots.py
 src/function/timer.py
 src/function/variables.py
 src/io/__init__.py
 src/io/dataio.py
 src/io/plot3dio.py
+src/project_arrakis.egg-info/PKG-INFO
+src/project_arrakis.egg-info/SOURCES.txt
+src/project_arrakis.egg-info/dependency_links.txt
+src/project_arrakis.egg-info/top_level.txt
 src/streamlines/__init__.py
 src/streamlines/integration.py
 src/streamlines/interpolation.py
 src/streamlines/search.py
 src/streamlines/stochastic_model.py
 src/streamlines/streamlines.py
 src/test_cases/__init__.py
@@ -22,11 +24,12 @@
 test/test_dataio.py
 test/test_import.py
 test/test_integration.py
 test/test_interpolation.py
 test/test_oblique_shock_data.py
 test/test_plot.py
 test/test_plot3dio.py
+test/test_plots.py
 test/test_search.py
 test/test_stochastic_model.py
 test/test_terminal_run.py
 test/test_variables.py
```

### Comparing `project-arrakis-0.1/src/function/timer.py` & `project_arrakis-0.1.1/src/function/timer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,62 @@
-# timer.py
-# Credit: https://realpython.com/python-timer/
-# GitHub: https://github.com/realpython/codetiming
-
-from contextlib import ContextDecorator
-from dataclasses import dataclass, field
-import time
-from typing import Any, Callable, ClassVar, Dict, Optional
-
-
-class TimerError(Exception):
-    """A custom exception used to report errors in use of Timer class"""
-
-
-@dataclass
-class Timer(ContextDecorator):
-    """Time your code using a class, context manager, or decorator"""
-
-    timers: ClassVar[Dict[str, float]] = dict()
-    name: Optional[str] = None
-    text: str = "Elapsed time: {:0.4f} seconds"
-    logger: Optional[Callable[[str], None]] = print
-    _start_time: Optional[float] = field(default=None, init=False, repr=False)
-
-    def __post_init__(self) -> None:
-        """Initialization: add timer to dict of timers"""
-        if self.name:
-            self.timers.setdefault(self.name, 0)
-
-    def start(self) -> None:
-        """Start a new timer"""
-        if self._start_time is not None:
-            raise TimerError(f"Timer is running. Use .stop() to stop it")
-
-        self._start_time = time.perf_counter()
-
-    def stop(self) -> float:
-        """Stop the timer, and report the elapsed time"""
-        if self._start_time is None:
-            raise TimerError(f"Timer is not running. Use .start() to start it")
-
-        # Calculate elapsed time
-        elapsed_time = time.perf_counter() - self._start_time
-        self._start_time = None
-
-        # Report elapsed time
-        if self.logger:
-            self.logger(self.text.format(elapsed_time))
-        if self.name:
-            self.timers[self.name] += elapsed_time
-
-        return elapsed_time
-
-    def __enter__(self) -> "Timer":
-        """Start a new timer as a context manager"""
-        self.start()
-        return self
-
-    def __exit__(self, *exc_info: Any) -> None:
-        """Stop the context manager timer"""
-        self.stop()
+# timer.py
+# Credit: https://realpython.com/python-timer/
+# GitHub: https://github.com/realpython/codetiming
+
+from contextlib import ContextDecorator
+from dataclasses import dataclass, field
+import time
+from typing import Any, Callable, ClassVar, Dict, Optional
+
+
+class TimerError(Exception):
+    """A custom exception used to report errors in use of Timer class"""
+
+
+@dataclass
+class Timer(ContextDecorator):
+    """Time your code using a class, context manager, or decorator"""
+
+    timers: ClassVar[Dict[str, float]] = dict()
+    name: Optional[str] = None
+    text: str = "Elapsed time: {:0.4f} seconds"
+    logger: Optional[Callable[[str], None]] = print
+    _start_time: Optional[float] = field(default=None, init=False, repr=False)
+
+    def __post_init__(self) -> None:
+        """Initialization: add timer to dict of timers"""
+        self.elapsed_time = 0
+        if self.name:
+            self.timers.setdefault(self.name, 0)
+
+    def start(self) -> None:
+        """Start a new timer"""
+        if self._start_time is not None:
+            raise TimerError(f"Timer is running. Use .stop() to stop it")
+
+        self._start_time = time.perf_counter()
+
+    def stop(self) -> float:
+        """Stop the timer, and report the elapsed time"""
+        if self._start_time is None:
+            raise TimerError(f"Timer is not running. Use .start() to start it")
+
+        # Calculate elapsed time
+        self.elapsed_time = time.perf_counter() - self._start_time
+        self._start_time = None
+
+        # Report elapsed time
+        if self.logger:
+            self.logger(self.text.format(self.elapsed_time))
+        if self.name:
+            self.timers[self.name] += self.elapsed_time
+
+        return self.elapsed_time
+
+    def __enter__(self) -> "Timer":
+        """Start a new timer as a context manager"""
+        self.start()
+        return self
+
+    def __exit__(self, *exc_info: Any) -> None:
+        """Stop the context manager timer"""
+        self.stop()
```

### Comparing `project-arrakis-0.1/src/io/dataio.py` & `project_arrakis-0.1.1/src/io/dataio.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,254 +1,307 @@
-# This file contains DataIO class to read and write particle data
-
-import numpy as np
-from src.streamlines.search import Search
-from src.streamlines.interpolation import Interpolation
-from multiprocessing.pool import ThreadPool as Pool
-import multiprocessing as mp
-from scipy.interpolate import griddata
-import os
-import re
-
-
-class DataIO:
-    """
-    Use to read/write particle data
-    The process happens in four steps. Each step is described below
-        1. Reads in the scattered particle data obtained from LPT code. Two ways are available:
-            If a combined file is given, data is obtained from that --> faster
-            Else, data is read from a folder of files where each file corresponds to a particle --> slow due to for loop
-        2. Interpolates fluid data to these scattered locations. Two temp files are generated
-            interpolated_q_data.npy --> has the flow data at the scattered locations
-            new_p_data.npy --> has the particle data at scattered locations (WITH few outlier points removed)
-        3. Lagrangian to Eulerian interpolation. Two temp files are generated
-            flow_data.npy --> Fluid data interpolated to the grid
-            particle_data.npy --> Particle data interpolated to the grid
-        4. mgrid data to plot3d for visualization and syPIV usage. Output tunnel. Three files are generated
-            mgrd_to_p3d.x --> Grid file
-            mgrd_to_p3d_fluid.q --> fluid data
-            mgrd_to_p3d_particle.q --> particle data in Eulerian interpretation
-
-    Attributes
-    ----------
-    Input :
-        grid : src.io.plot3dio.GridIO
-            Grid object created from GridIO
-        flow : src.io.plot3dio.FlowIO
-            Flow object created from FlowIO
-        read_file : str
-            Combined file of all the particles generated from LPT code
-        location : str
-            Files location for individual particle data generated from the LPT code
-        x_refinement: int
-            Refinement of grid in horizontal direction
-        y_refinement: int
-            Refinement of grid in vertical direction
-    Output:
-        None
-
-    Methods
-    -------
-        compute()
-            saves the output files in the working directory
-
-        Examples
-            The test case is in test/test_dataio.py
-
-
-    author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
-    date: 12-28/2022
-    """
-
-    def __init__(self, grid, flow, read_file=None, location='.',
-                 x_refinement: int = 50, y_refinement: int = 40):
-        self.grid = grid
-        self.flow = flow
-        self.read_file = read_file
-        self.location = location
-        self.x_refinement = x_refinement
-        self.y_refinement = y_refinement
-
-    @staticmethod
-    def _natural_sort(_l: list):
-        """
-        Sorts a list in natural order of things. Humanity is weird
-        Args:
-            _l: list of strings
-
-        Returns:
-            sorted list in natural order
-
-        """
-        convert = lambda text: int(text) if text.isdigit() else text.lower()
-        alphanum_key = lambda key: [convert(c) for c in re.split('([0-9]+)', key)]
-        return sorted(_l, key=alphanum_key)
-
-    def compute(self):
-        """
-        This should interpolate the scattered particle data onto a 2D grid
-        Return a file to be used for syPIV
-        Returns:
-        """
-        # read particle files from a folder
-        # read particle data
-        try:
-            print('Trying to read from a combined file...')
-            _p_data = np.load(self.read_file)
-            print('Read from the combined file!!')
-        except:
-            print('Reading from a group of files... This will take a while!')
-            # Sort in natural order to stack particles in order
-            _files = np.array(self._natural_sort(os.listdir(self.location)))
-            _bool = []
-            for _i, _name in enumerate(_files):
-                if not _name.endswith(".npy"):
-                    _bool.append(_i)
-            _files = np.delete(_files, _bool)
-
-            _p_data = np.load(self.location + _files[0])
-            for infile in _files[1:]:
-                _temp = np.load(self.location + infile)
-                _p_data = np.vstack((_p_data, _temp))
-                print('Done with - ' + infile)
-            print('Done reading files into an array from a group of files!')
-            np.save(self.location + 'combined_file', _p_data)
-            print('**SUCCESS** combined_file.npy saved to the given location.')
-
-        _x_min, _x_max = _p_data[:, 0].min(), _p_data[:, 0].max()
-        _y_min, _y_max = _p_data[:, 1].min(), _p_data[:, 1].max()
-
-        # Get density and energy for plot3d file at locations
-        _locations = _p_data[:, :3]
-
-        def _flow_data(_point, _index, _size):
-            """
-            Internal function that interpolates data to scattered points
-            Args:
-                _point: One of the scattered points
-
-            Returns:
-                Interpolated data at each scattered point location given
-
-            """
-            _idx = Search(self.grid, _point)
-            _idx.compute(method='p-space')
-            _interp = Interpolation(self.flow, _idx)
-            _interp.compute(method='p-space')
-
-            try:
-                print(f'Done with {_index}/{_size}')
-                return _interp.q.reshape(-1)
-            except:
-                print('Returned None. Exception occurred')
-                return np.array([1], dtype=int)
-
-        try:
-            # Read back the saved file
-            _q_list = np.load(self.location + 'dataio/interpolated_q_data.npy', allow_pickle=False)
-            _p_data = np.load(self.location + 'dataio/new_p_data.npy', allow_pickle=False)
-            print('Read the available interpolated data to continue with the griddata algorithm')
-        except:
-            print('Interpolated data file is unavailable. Continuing with interpolation to scattered data!\n'
-                  'This is going to take sometime. Sit back and relax!\n'
-                  'Your PC will take off because of multi-process. Let it breathe...\n')
-            _processors = mp.cpu_count()
-            _pool = Pool(_processors)
-            _loc_len = len(_locations)
-            # Passing extra parameters to keep track of the progress. Chunk-size helps to keep it orderly
-            _q_list = _pool.starmap(_flow_data, zip(_locations, np.arange(0, _loc_len), np.repeat(_loc_len, _loc_len)),
-                                    chunksize=1)
-            _pool.close()
-
-            # Fluid data at scattered points/particle locations
-            # Some searches return None. This helps remove those locations!
-            _remove_index = [j for j in range(len(_q_list)) if np.all(_q_list[j] == 1)]
-            _q_list = np.vstack(np.delete(_q_list, _remove_index, axis=0))
-            _p_data = np.delete(_p_data, _remove_index, axis=0)
-            # _q_list = np.array([i for i in _q_list if np.all(i != 1)])
-            # Save both interpolated data and new particle data for easy future computations
-            try:
-                # Try creating the directory; if exists errors out and except
-                os.mkdir(self.location + 'dataio')
-                np.save(self.location + 'dataio/interpolated_q_data', _q_list)
-                np.save(self.location + 'dataio/new_p_data', _p_data)
-                print('Created dataio and saved interpolated flow data to scattered points.\n')
-            except:
-                np.save(self.location + 'dataio/interpolated_q_data', _q_list)
-                np.save(self.location + 'dataio/new_p_data', _p_data)
-            print('Done with interpolating flow data to scattered points.\n')
-
-        # Particle data at the scattered points/particle locations
-        # rho, x,y,z - momentum, energy per unit volume (q-file data)
-        _q_p_list = np.hstack((_q_list[:, 0].reshape(-1, 1), _p_data[:, 3:6] * _q_list[:, 0].reshape(-1, 1),
-                               _q_list[:, 4].reshape(-1, 1)))
-        # Fluid data at the scattered points/particle locations
-        _q_f_list = np.hstack((_q_list[:, 0].reshape(-1, 1), _p_data[:, 6:9] * _q_list[:, 0].reshape(-1, 1),
-                               _q_list[:, 4].reshape(-1, 1)))
-
-        # Create the grid to interpolate to
-        _xi, _yi = np.linspace(_x_min, _x_max, self.x_refinement), np.linspace(_y_min, _y_max, self.y_refinement)
-        _xi, _yi = np.meshgrid(_xi, _yi, indexing='ij')
-
-        # Function to loop through the scattered data
-        def _grid_interp(_data=None, _points=_p_data[:, :2], _x_grid=_xi, _y_grid=_yi, method='linear'):
-            """
-            Interpolate to grid data from scatter points
-            Args:
-                _points: scattered data - This is fixed, usually
-                _x_grid: grid data - fixed usually
-                _y_grid: grid data - fixed usually
-                _data: data set to be interpolated
-                method: set to linear but can be changed if needed
-
-            Returns:
-                Interpolated flow data
-
-            """
-            _data = _data.reshape(-1)
-            # Transposing to keep consistency with default xy indexing of meshgrid
-            _q = griddata(_points, _data, (_x_grid, _y_grid), method=method, fill_value=_data.max() * 2)
-
-            return _q
-
-        try:
-            # Read to see if data is available
-            _qf = np.load(self.location + 'dataio/flow_data.npy')
-            _qp = np.load(self.location + 'dataio/particle_data.npy')
-            print('Loaded available flow/particle data from numpy residual files\n')
-        except:
-            print('Interpolating data to the grid provided...\n')
-            # Interpolate scattered data onto the grid -- for flow
-            _pool = Pool(mp.cpu_count())
-            _qf = _pool.map(_grid_interp,
-                            [_q_f_list[:, 0], _q_f_list[:, 1], _q_f_list[:, 2], _q_f_list[:, 3], _q_f_list[:, 4]],
-                            chunksize=1)
-            _pool.close()
-            print(f'Done with flow data interpolation to grid.\n')
-
-            # Save the array to a file
-            # This will only happen when there are files in dataio directory
-            _qf = np.array(_qf)
-            np.save(self.location + 'dataio/flow_data', _qf)
-
-            # Interpolate scattered data onto the grid -- for particles
-            _pool = Pool(mp.cpu_count())
-            _qp_123 = _pool.map(_grid_interp, [_q_p_list[:, 1], _q_p_list[:, 2], _q_p_list[:, 3]], chunksize=1)
-            _pool.close()
-            print(f'Done with particle data interpolation to grid.\n')
-
-            # Create _qp array from known values
-            _qp = np.dstack((_qf[0], _qp_123[0], _qp_123[1], _qp_123[2], _qf[-1])).transpose((2, 0, 1))
-
-            # Save data to a temporary file
-            _qp = np.array(_qp)
-
-            # This will only happen when there are files in dataio directory
-            np.save(self.location + 'dataio/particle_data', _qp)
-
-        # Write out to plot3d format for further processing
-        self.grid.mgrd_to_p3d(_xi, _yi, out_file=self.location + 'dataio/mgrd_to_p3d.x')
-        self.flow.mgrd_to_p3d(_qf, mode='fluid', out_file=self.location + 'dataio/mgrd_to_p3d')
-        self.flow.mgrd_to_p3d(_qp, mode='particle', out_file=self.location + 'dataio/mgrd_to_p3d')
-        print('Files written to the working directory')
-
-        return
+# This file contains DataIO class to read and write particle data
+
+import numpy as np
+from src.streamlines.search import Search
+from src.streamlines.interpolation import Interpolation
+from multiprocessing import Pool
+import multiprocessing as mp
+from scipy.interpolate import griddata
+import os
+import re
+from tqdm import tqdm
+rng = np.random.default_rng()
+
+
+class DataIO:
+    """
+    Use to read/write particle data
+    The process happens in four steps. Each step is described below
+        1. Reads in the scattered particle data obtained from LPT code. Two ways are available:
+            If a combined file is given, data is obtained from that --> faster
+            Else, data is read from a folder of files where each file corresponds to a particle --> slow due to for loop
+        2. Interpolates fluid data to these scattered locations. Two temp files are generated
+            interpolated_q_data.npy --> has the flow data at the scattered locations
+            new_p_data.npy --> has the particle data at scattered locations (WITH few outlier points removed)
+        3. Lagrangian to Eulerian interpolation. Two temp files are generated
+            flow_data.npy --> Fluid data interpolated to the grid
+            particle_data.npy --> Particle data interpolated to the grid
+        4. mgrid data to plot3d for visualization and syPIV usage. Output tunnel. Three files are generated
+            mgrd_to_p3d.x --> Grid file
+            mgrd_to_p3d_fluid.q --> fluid data
+            mgrd_to_p3d_particle.q --> particle data in Eulerian interpretation
+
+    Attributes
+    ----------
+    Input :
+        grid : src.io.plot3dio.GridIO
+            Grid object created from GridIO
+        flow : src.io.plot3dio.FlowIO
+            Flow object created from FlowIO
+        read_file : str
+            Combined file of all the particles generated from LPT code
+        location : str
+            Files location for individual particle data generated from the LPT code
+        x_refinement: int
+            Refinement of grid in horizontal direction
+        y_refinement: int
+            Refinement of grid in vertical direction
+    Output:
+        None
+
+    Methods
+    -------
+        compute()
+            saves the output files in the working directory
+
+        Examples
+            The test case is in test/test_dataio.py
+
+
+    author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
+    date: 12-28/2022
+    """
+
+    def __init__(self, grid, flow, percent_data=100, read_file=None, location='.',
+                 x_refinement: int = 50, y_refinement: int = 40):
+        self.grid = grid
+        self.flow = flow
+        self.percent_data = percent_data
+        self.read_file = read_file
+        self.location = location
+        self.x_refinement = x_refinement
+        self.y_refinement = y_refinement
+
+    @staticmethod
+    def _natural_sort(_l: list):
+        """
+        Sorts a list in natural order of things. Humanity is weird
+        Args:
+            _l: list of strings
+
+        Returns:
+            sorted list in natural order
+
+        """
+        convert = lambda text: int(text) if text.isdigit() else text.lower()
+        alphanum_key = lambda key: [convert(c) for c in re.split('([0-9]+)', key)]
+        return sorted(_l, key=alphanum_key)
+
+    def _flow_data(self, _point, _index, _size):
+        """
+        Internal function that interpolates data to scattered points
+        Args:
+            _point: One of the scattered points
+
+        Returns:
+            Interpolated data at each scattered point location given
+
+        """
+        try:
+            _idx = Search(self.grid, _point)
+            _idx.compute(method='distance')
+            _interp = Interpolation(self.flow, _idx)
+            _interp.compute(method='p-space')
+            # print(f'Done with flow data interpolation {_index}/{_size}')
+            return _interp.q.reshape(-1)
+        except:
+            print(f'**Exception occurred with {_index}**')
+            return np.array([1], dtype=int)
+
+    # Function to loop through the scattered data
+    def _grid_interp(self, _data, _points, _x_grid, _y_grid, method='linear'):
+        """
+        Interpolate to grid data from scatter points
+        Args:
+            _points: scattered data - This is fixed, usually
+            _x_grid: grid data - fixed usually
+            _y_grid: grid data - fixed usually
+            _data: data set to be interpolated
+            method: set to linear but can be changed if needed
+
+        Returns:
+            Interpolated flow data
+
+        """
+        _data = _data.reshape(-1)
+        # Transposing to keep consistency with default xy indexing of meshgrid
+        # Where there's no data, fill with twice the max value
+        _q = griddata(_points, _data, (_x_grid, _y_grid), method=method, fill_value=_data.max() * 2)
+
+        return _q
+
+    def compute(self):
+        """
+        This should interpolate the scattered particle data onto a 2D grid
+        Return a file to be used for syPIV
+        Returns:
+        """
+        # read particle files from a folder
+        # read particle data
+        try:
+            print('Trying to read from a combined file...')
+            _p_data = np.load(self.read_file)
+            print('Read from the combined file!!')
+        except:
+            # TODO: Dask might save time here!
+            print('Reading from a group of files... This will take a while!')
+            # Sort in natural order to stack particles in order
+            _files = np.array(self._natural_sort(os.listdir(self.location)))
+            _bool = []
+            for _i, _name in enumerate(_files):
+                if not _name.endswith(".npy"):
+                    _bool.append(_i)
+            _files = np.delete(_files, _bool)
+
+            _p_data = np.load(self.location + _files[0])
+            for infile in _files[1:]:
+                _temp = np.load(self.location + infile)
+                _p_data = np.vstack((_p_data, _temp))
+                print('Done with - ' + infile)
+            print('Done reading files into an array from a group of files!')
+            np.save(self.location + 'combined_file', _p_data)
+            print('**SUCCESS** combined_file.npy saved to the given location.')
+
+        # p-data has the following columns
+        # x, y, z, vx, vy, vz, ux, uy, uz, time, integrated (ux, uy, uz), diameter, density
+        _x_min, _x_max = self.grid.grd_min.reshape(-1)[0], self.grid.grd_max.reshape(-1)[0]
+        _y_min, _y_max = self.grid.grd_min.reshape(-1)[1], self.grid.grd_max.reshape(-1)[1]
+
+        # Get density and energy for plot3d file at locations
+        if self.percent_data == 100:
+            pass
+        else:
+            # Get a uniform distribution of the sample
+            _p_data = rng.choice(_p_data, size=int(_p_data.shape[0] * self.percent_data / 100))
+        _locations = _p_data[:, :3]
+
+        try:
+            # Read if saved files are available
+            _q_list = np.load(self.location + 'dataio/interpolated_q_data.npy', allow_pickle=False)
+            _p_data = np.load(self.location + 'dataio/new_p_data.npy', allow_pickle=False)
+            print('Read the available interpolated data to continue with the griddata algorithm')
+        except:
+            # Run through the process of creating interpolation files
+            try:
+                # Read old interpolation files before removing outliers if available
+                _q_list = np.load(self.location + 'dataio/_old_interpolated_q_data.npy', allow_pickle=True)
+                _p_data = np.load(self.location + 'dataio/_old_p_data.npy', allow_pickle=True)
+                print('Read the available old interpolated data to continue with the outliers algorithm')
+            except:
+                # Run the interpolation process on all the scattered points
+                print('Interpolated data file is unavailable. Continuing with interpolation to scattered data!\n'
+                      'This is going to take sometime. Sit back and relax!\n'
+                      'Your PC will take off because of multi-process. Let it breathe...\n')
+                # Test serial
+                # _q_list = []
+                # _loc_len = len(_locations)
+                # for _i, _point in enumerate(_locations):
+                #     _q_list.append(self._flow_data(_point, _i, _loc_len))
+
+                # parallel
+                _processors = mp.cpu_count()
+                _pool = Pool(_processors)
+                _loc_len = len(_locations)
+                # Passing extra parameters to keep track of the progress. Chunk-size helps to keep it orderly
+                inputs = zip(_locations, np.arange(0, _loc_len), np.repeat(_loc_len, _loc_len))
+                _q_list = _pool.starmap(self._flow_data,
+                                        tqdm(inputs, total=_loc_len),
+                                        chunksize=_loc_len//_processors)
+                _pool.close()
+                _pool.join()
+
+                # Intermediate save of the data -- if the process is interrupted we can restart it from here
+                try:
+                    # Try creating the directory; if exists errors out and except
+                    os.mkdir(self.location + 'dataio')
+                    np.save(self.location + 'dataio/_old_interpolated_q_data', _q_list)
+                    np.save(self.location + 'dataio/_old_p_data', _p_data)
+                    print('Created dataio folder and saved old interpolated flow data to scattered points.\n')
+                except:
+                    np.save(self.location + 'dataio/_old_interpolated_q_data', _q_list)
+                    np.save(self.location + 'dataio/_old_new_p_data', _p_data)
+                print('Done with interpolating flow data to scattered points.\n'
+                      'Removing outliers from the data...\n')
+
+            # Fluid data at scattered points/particle locations
+            # Some searches return None. This helps remove those locations!
+            _remove_index = [j for j in range(len(_q_list)) if np.all(_q_list[j] == 1)]
+            _q_list = np.vstack(np.delete(_q_list, _remove_index, axis=0))
+            _p_data = np.delete(_p_data, _remove_index, axis=0)
+            # Remove outliers due to bad interpolation -- density cannot go beyond the flow limits
+            _remove_index = np.where(_q_list[:, 0] < self.flow.q[..., 0, :].min())
+            _q_list = np.vstack(np.delete(_q_list, _remove_index, axis=0))
+            _p_data = np.delete(_p_data, _remove_index, axis=0)
+            _remove_index = np.where(_q_list[:, 0] > self.flow.q[..., 0, :].max())
+            _q_list = np.vstack(np.delete(_q_list, _remove_index, axis=0))
+            _p_data = np.delete(_p_data, _remove_index, axis=0)
+            # Save both interpolated data and new particle data for easy future computations
+            try:
+                # Save interpolated data to files
+                np.load(self.location + 'dataio/interpolated_q_data', allow_pickle=False)
+                np.load(self.location + 'dataio/new_p_data', allow_pickle=False)
+                print('Loaded particle and flow interpolated data from existing files.\n')
+            except:
+                np.save(self.location + 'dataio/interpolated_q_data', _q_list)
+                np.save(self.location + 'dataio/new_p_data', _p_data)
+            print('Done with interpolating flow data to scattered points.\n')
+
+        # Particle data at the scattered points/particle locations
+        # rho, x,y,z - momentum, energy per unit volume (q-file data)
+        _q_p_list = np.hstack((_q_list[:, 0].reshape(-1, 1), _p_data[:, 3:6] * _q_list[:, 0].reshape(-1, 1),
+                               _q_list[:, 4].reshape(-1, 1)))
+        # Fluid data at the scattered points/particle locations
+        _q_f_list = np.hstack((_q_list[:, 0].reshape(-1, 1), _p_data[:, 6:9] * _q_list[:, 0].reshape(-1, 1),
+                               _q_list[:, 4].reshape(-1, 1)))
+
+        # Create the grid to interpolate to
+        _xi, _yi = np.linspace(_x_min, _x_max, self.x_refinement), np.linspace(_y_min, _y_max, self.y_refinement)
+        _xi, _yi = np.meshgrid(_xi, _yi, indexing='ij')
+
+        try:
+            # Read to see if data is available
+            _qf = np.load(self.location + 'dataio/flow_data.npy')
+            _qp = np.load(self.location + 'dataio/particle_data.npy')
+            print('Loaded available flow/particle data from numpy residual files\n')
+        except:
+            print('Interpolating data to the grid provided...\n')
+            # Interpolate scattered data onto the grid -- for flow
+            _pool = Pool(mp.cpu_count())
+            inputs = zip([_q_f_list[:, 0], _q_f_list[:, 1], _q_f_list[:, 2], _q_f_list[:, 3], _q_f_list[:, 4]],
+                         [_p_data[:, :2]]*5, [_xi]*5, [_yi]*5, ['linear']*5)
+            _qf = _pool.starmap(self._grid_interp,
+                                tqdm(inputs, total=5), chunksize=5)
+            _pool.close()
+            _pool.join()
+            print(f'Done with flow data interpolation to grid.\n')
+
+            # Save the array to a file
+            # This will only happen when there are files in dataio directory
+            _qf = np.array(_qf)
+            np.save(self.location + 'dataio/flow_data', _qf)
+
+            # Interpolate scattered data onto the grid -- for particles
+            _pool = Pool(mp.cpu_count())
+            inputs = zip([_q_p_list[:, 1], _q_p_list[:, 2], _q_p_list[:, 3]],
+                         [_p_data[:, :2]]*3, [_xi]*3, [_yi]*3, ['linear']*3)
+            _qp_123 = _pool.starmap(self._grid_interp,
+                                   tqdm(inputs, total=3), chunksize=3)
+            _pool.close()
+            _pool.join()
+            print(f'Done with particle data interpolation to grid.\n')
+
+            # Create _qp array from known values
+            _qp = np.dstack((_qf[0], _qp_123[0], _qp_123[1], _qp_123[2], _qf[-1])).transpose((2, 0, 1))
+
+            # Save data to a temporary file
+            _qp = np.array(_qp)
+
+            # This will only happen when there are files in dataio directory
+            np.save(self.location + 'dataio/particle_data', _qp)
+
+        # Write out to plot3d format for further processing
+        self.grid.mgrd_to_p3d(_xi, _yi, out_file=self.location + 'dataio/mgrd_to_p3d.x')
+        self.flow.mgrd_to_p3d(_qf, mode='fluid', out_file=self.location + 'dataio/mgrd_to_p3d')
+        self.flow.mgrd_to_p3d(_qp, mode='particle', out_file=self.location + 'dataio/mgrd_to_p3d')
+        print('Files written to the working directory')
+
+        return
```

### Comparing `project-arrakis-0.1/src/io/plot3dio.py` & `project_arrakis-0.1.1/src/io/plot3dio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,529 +1,544 @@
-# This file contains classes for plot3d data io
-# TODO: implement output for p3d data - Assigned to Harpreet.
-#  Each output function should be added to respective GridIO/FlowIO classes
-#  Change docstrings for doctest in test_io
-
-import numpy as np
-
-
-class GridIO:
-    """Module to read-in a grid file and output grid parameters
-
-    ...
-
-    Attributes
-    ----------
-    Input :
-        filename : str
-            name of the grid file
-    Output :
-        nb : int
-            number of blocks in the grid
-        ni, nj, nk : int
-            shape of the domain
-        grd : numpy.ndarray
-            Grid data of shape (ni, nj, nk, 3, nb)
-        grd_min: numpy.ndarray
-            min co-ordinates of each block (3, nb)
-        grd_max: numpy.ndarray
-            max co-ordinates of each block (3, nb)
-        m1 : numpy.ndarray
-            xi, eta, zeta derivatives wrt x, y, z --> shape (ni, nj, nk, 3, 3, nb)
-        m2 : numpy.ndarray
-            x, y, z derivatives wrt xi, eta, zeta --> shape (ni, nj, nk, 3, 3, nb)
-        J : numpy.ndarray
-            Jacobian determinant of m1 --> shape (ni, nj, nk, nb)
-
-
-    Methods
-    -------
-    read_grid()
-        returns the output attributes
-
-    Example:
-        grid = GridIO('plate.sp.x')  # Assume file is in the path
-        grid.read_grid()  # Call method to read the data
-        grid.compute_metrics()  # Computes m1, m2, J arrays
-        print(grid)  # prints the docstring for grid
-        # Instance attributes
-        print(grid.grd.shape)  # shape of the grid data
-        print(grid.nb)  # Number of blocks
-
-    author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
-    date: 10-05/2021
-    """
-
-    def __init__(self, filename):
-        self.filename = filename
-        self.nb = None
-        self.ni, self.nj, self.nk = None, None, None
-        self.grd = None
-        self.grd_min, self.grd_max = [], []
-        self.m1, self.m2 = None, None
-        self.J = None
-
-    def __str__(self):
-        doc = "This instance has the filename " + self.filename + "\n" + \
-              "grd attribute is of shape (ni, nj, nk, 3, nb), rows representing x,y,z coordinates for each block\n" \
-              "For example, x = grid.grd(...,0, 0), grid being the object.\n" \
-              "Use method 'read_grid' to compute grd attributes:\n" \
-              "ni, nj, nk, ng\n" \
-              "Use method 'compute_metrics' to compute grid metric attributes:\n" \
-              "m1, m2, J\n" \
-              "grd -- The grid data\n"
-        return doc
-
-    def read_grid(self, data_type='f4'):
-        """Reads in the grid file and changes the instance attributes
-
-        Parameters
-        -----------
-        data_type: str
-            Specify the data type of the grid file specified
-            Default is 'f4' for single-precision
-            For double-precision use 'f8'
-
-        Returns
-        -------
-        None
-
-        author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
-        credit: Paul Orkwis
-        date: 11-04/2021
-        """
-        with open(self.filename, 'r') as grid:
-            # Read-in number of blocks
-            self.nb = np.fromfile(grid, dtype='i4', count=1)[0]
-
-            # Read-in i, j, k for all blocks
-            _temp = np.fromfile(grid, dtype='i4', count=3 * self.nb)
-            self.ni, self.nj, self.nk = _temp[0::3], _temp[1::3], _temp[2::3]
-
-            # length of grd data
-            _nt = self.ni * self.nj * self.nk * 3
-            # read the grd data from file to temp_array
-            _temp = np.fromfile(grid, dtype=data_type, count=sum(_nt))
-
-            # pre-define grd to reduce calling pad and concatenate
-            self.grd = np.zeros((self.ni.max(), self.nj.max(), self.nk.max(), 3, self.nb))
-
-            # Reshape and assign data to grd
-            for _i in range(self.nb):
-                self.grd[0:self.ni[_i], 0:self.nj[_i], 0:self.nk[_i], 0:3, _i] = \
-                    _temp[sum(_nt[0:_i]):sum(_nt[0:_i]) + _nt[_i]] \
-                    .reshape((self.ni[_i], self.nj[_i], self.nk[_i], 3), order='F')
-
-            print("Grid data reading is successful for " + self.filename + "\n")
-
-            # Setup some parameters for further processing
-            # Find out the min and max of each block
-            for _i, _j, _k, _b in zip(self.ni, self.nj, self.nk, range(self.nb)):
-                self.grd_min.append(np.amin(self.grd[:_i, :_j, :_k, :, _b], axis=(0, 1, 2)))
-                self.grd_max.append(np.amax(self.grd[:_i, :_j, :_k, :, _b], axis=(0, 1, 2)))
-
-            # Convert lists to arrays
-            self.grd_min = np.array(self.grd_min)
-            self.grd_max = np.array(self.grd_max)
-
-    def compute_metrics(self):
-        """Calculate grid metrics from grid data.
-        Need to call read_grid() before computing metrics
-
-        Parameters
-        ----------
-
-        Returns
-        -------
-        None
-
-        Example:
-            grid = GridIO(filename)  # Assume grid is the object from GridIO
-            grid.read_grid()  # Call method to read-in grid data
-            grid.compute_metrics()  # Call method to compute grid metrics
-            print(grid)  # prints the docstring for grid metrics
-            # Instance attributes
-            print(grid.m1)  # derivatives xi, eta, zeta
-            print(grid.m2)  # derivatives x, y, z
-
-        author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
-        credit: Jacob Welsh for providing the code for single block
-        date: 12-23/2021
-        """
-        self.m1 = np.zeros((self.ni.max(), self.nj.max(), self.nk.max(), 3, 3, self.nb))
-        self.m2 = np.zeros((self.ni.max(), self.nj.max(), self.nk.max(), 3, 3, self.nb))
-        self.J = np.zeros((self.ni.max(), self.nj.max(), self.nk.max(), self.nb))
-
-        #  The for loop is to compute x, y, z derivatives wrt xi, eta, zeta
-        # for i in range(3):
-        #     self.m1[..., i, :] = np.gradient(self.grd, axis=i)
-
-        for b in range(self.nb):
-            print(f"Computing Jacobian for block {b}...")
-            for i in range(3):
-                self.m1[:self.ni[b], :self.nj[b], :self.nk[b], :, i, b] = \
-                    np.gradient(self.grd[:self.ni[b], :self.nj[b], :self.nk[b], :, b], axis=i)
-        print("Done computing Jacobian for all the blocks!!\n")
-
-        # compute Jacobian
-        for b in range(self.nb):
-            print(f"Computing Jacobian determinant for block {b}...")
-            self.J[:self.ni[b], :self.nj[b], :self.nk[b], b] = \
-                self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 0, b] * \
-                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b] -
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b]) - \
-                self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 0, b] * \
-                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b] -
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b]) + \
-                self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 0, b] * \
-                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b] -
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b])
-        print("Done computing Jacobian determinant for all the blocks!!")
-
-        # x derivatives
-        for b in range(self.nb):
-            print(f"Computing Inverse Jacobian for block {b}...")
-            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 0, 0, b] = \
-                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b] -
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b]) /\
-                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
-            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] = \
-                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b] -
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b]) /\
-                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
-            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] = \
-                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b] -
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b]) /\
-                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
-
-            # y derivative
-            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 1, 0, b] = \
-                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 0, b] -
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 0, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b]) /\
-                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
-            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b] = \
-                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 0, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b] -
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 0, b]) /\
-                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
-            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b] = \
-                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 0, b] -
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 0, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b]) /\
-                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
-
-            # z derivatives
-            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 2, 0, b] = \
-                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 0, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b] -
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 0, b]) /\
-                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
-            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b] = \
-                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 0, b] -
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 0, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b]) /\
-                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
-            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b] = \
-                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 0, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b] -
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] *
-                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 0, b]) /\
-                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
-
-        print("Done computing Inverse Jacobian for all the blocks!!")
-        print("All Grid metrics computed successfully!")
-
-    def two_to_three(self, steps: int = 5, step_size: float = None, data_type='f4'):
-        """
-        Converts 2D plot3d grid file to 3D format
-        TODO: Current limitation is that the code works only for 3d written 2d files and single block
-        Returns: None
-
-        """
-        if step_size is None:
-            print("Step size is not provided; Using minimum grid size")
-            step_size = abs(min(np.diff(self.grd[:, 0, 0, 0, 0])))
-
-        _a_temp = np.array([self.nb, self.ni, self.nj, steps], dtype='i4')
-        _x_temp = self.grd[..., 0, 0].repeat(steps, axis=2)
-        _y_temp = self.grd[..., 1, 0].repeat(steps, axis=2)
-        _z_temp = np.ones((int(self.ni), int(self.nj), steps)) * np.linspace(0, steps*step_size, steps)
-        _b_temp = np.array([_x_temp.T, _y_temp.T, _z_temp.T], dtype=data_type)
-
-        _temp_filename = self.filename.replace('.x', '_3D.x')
-        with open(_temp_filename, 'wb') as f:
-            f.write(_a_temp.tobytes())
-            f.write(_b_temp.tobytes())
-
-        print(f'\n File is successfully written in the working directory as {_temp_filename}')
-
-        return
-
-    def mgrd_to_p3d(self, xi, yi, out_file: str = 'mgrd_to_p3d.x',
-                    steps: int = 5, step_size: float = None, data_type='f4'):
-        """
-        Creates a 3d plot3d grid file;
-        This can be later used to be converted to 3d format by two_to_three
-        Returns:
-
-        """
-        if step_size is None:
-            print("Step size is not provided; Using minimum grid size")
-            step_size = abs(min(np.diff(self.grd[:, 0, 0, 0, 0])))
-
-        # Number of blocks is always 1 for this function
-        _ng, _ni, _nj, _nk = np.array([1, xi.shape[0], yi.shape[1], steps], dtype='i4')
-        _xx, _yy, _zz = np.meshgrid(xi[:, 0], yi[0], np.linspace(0, steps*step_size, steps), indexing='ij')
-        _grd = np.array([_xx.T, _yy.T, _zz.T], dtype=data_type)
-
-        with open(out_file, 'wb') as f:
-            f.write(_ng)
-            f.write(_ni)
-            f.write(_nj)
-            f.write(_nk)
-            f.write(_grd.tobytes())
-
-        print(f'\n File is successfully written in the working directory as {out_file}')
-
-        return
-
-
-class FlowIO:
-    """Module to read-in a flow file and output flow parameters
-
-    ...
-
-    Attributes
-    ----------
-    Input :
-        filename : str
-            name of the flow file
-    Output :
-        nb : int
-            number of blocks in the grid
-        ni, nj, nk : int
-            shape of the domain
-        mach, alpha, rey, time: float
-            extra numerics needed for post-processing
-        q : numpy.ndarray
-            Flow data of shape (ni, nj, nk, 5, nb)
-
-    Methods
-    -------
-    read_flow()
-        returns the output attributes
-    two_to_three()
-        converts 2D data to 3D
-    mgrd_to_p3d()
-        converts and returns meshgrid data to plot3D data
-    read_formatted_txt()
-        Reads Tecplot returned formatted text. Must contain five columns without headers
-        rho, rho-u, rho-v, rho-w, e are the five columns
-
-    Example:
-        grid = FlowIO('plate.sp.x')  # Assume file is in the path\n
-        flow.read_flow()  # Call method to read the data\n
-        print(flow)  # prints the docstring for grid\n
-        # Instance attributes\n
-        print(flow.q.shape)  # shape of the flow data\n
-        print(flow.ng)  # Number of blocks
-
-
-    author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
-    date: 10-05/2021
-    """
-
-    def __init__(self, filename):
-        self.filename = filename
-        self.nb = None
-        self.ni, self.nj, self.nk = None, None, None
-        self.mach = None
-        self.alpha = None
-        self.rey = None
-        self.time = None
-        self.q = None
-
-    def __str__(self):
-        doc = "This instance has the filename " + self.filename + "\n" + \
-              "q attribute is of shape (ni, nj, nk, 5, nb), rows representing density, momentum[*3], energy" \
-              "for every block\n" \
-              "For example, rho = flow.q(...,0,0), flow being the object for block-1.\n" \
-              "Use method 'read_flow' to compute attributes:\n" \
-              "nb, ni, nj, nk\n" \
-              "mach, alpha, rey, time\n" \
-              "q -- The flow data\n"
-        return doc
-
-    def read_flow(self, data_type='f4'):
-        """Reads in the flow file and changes the instance attributes
-
-        Parameters
-        ----------
-        data_type: str
-            Specify the data type of the flow file specified
-            Default is 'f4' for single-precision
-            For double-precision use 'f8'
-
-        Returns
-        -------
-        None
-
-        author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
-        credit: Paul Orkwis
-        date: 10-05/2021
-        """
-        with open(self.filename, 'r') as data:
-            self.nb = np.fromfile(data, dtype='i4', count=1)[0]
-
-            # Read in the i, j, k values for blocks
-            _temp = np.fromfile(data, dtype='i4', count=3 * self.nb)
-            self.ni, self.nj, self.nk = _temp[0::3], _temp[1::3], _temp[2::3]
-
-            # Read-in flow data into a temp array
-            # Less use of fromfile is more speed
-            _nt = self.ni * self.nj * self.nk * 5
-            _temp = np.fromfile(data, dtype=data_type, count=sum(_nt) + 4 * self.nb)
-
-            # Assign the dimensionless attributes
-            self.mach, self.alpha, self.rey, self.time = _temp[0:4]
-
-            # Create a mask to remove dimensionless quantities from q
-            # Indices of the first four dimensionless quantities
-            _index_array = np.array([0, 1, 2, 3])
-            for i in range(len(_nt) - 1):
-                _term = sum(_temp[0:i]) + (i + 1) * 4
-                _index_array = np.concatenate((_index_array, np.arange(_term, _term + 4)))
-            _mask = np.ones(len(_temp), dtype='bool')
-            _mask[_index_array] = 0
-            # Use the mask to remove dimensionless quantities
-            _temp = _temp[_mask]
-
-            # Pre-define q array
-            self.q = np.zeros((self.ni.max(), self.nj.max(), self.nk.max(), 5, self.nb))
-
-            # Reshape and assign data to q
-            for _i in range(self.nb):
-                self.q[0:self.ni[_i], 0:self.nj[_i], 0:self.nk[_i], 0:5, _i] = \
-                    _temp[sum(_nt[0:_i]):sum(_nt[0:_i]) + _nt[_i]] \
-                    .reshape((self.ni[_i], self.nj[_i], self.nk[_i], 5), order='F')
-
-            print("Flow data reading is successful for " + self.filename + "\n")
-
-    def two_to_three(self, steps: int = 5, data_type='f4'):
-        """
-        Converts 2D plot3d flow file to 3D format
-        TODO: Current limitation is that the code works only for 3d written 2d files and single block
-        Returns: None
-
-        """
-        # TODO: The code below needs debugging. It's not tested. mgrd_to_p3d might help!
-        _a_temp = np.array([self.nb, self.ni, self.nj, int(steps)], dtype='i4')
-        _b_temp = np.array([self.mach, self.alpha, self.rey, self.time], dtype=data_type)
-        _q0_temp = self.q[..., 0, 0].repeat(int(steps), axis=2)
-        _q1_temp = self.q[..., 1, 0].repeat(int(steps), axis=2)
-        _q2_temp = self.q[..., 2, 0].repeat(int(steps), axis=2)
-        _q3_temp = self.q[..., 3, 0].repeat(int(steps), axis=2)
-        _q4_temp = self.q[..., 4, 0].repeat(int(steps), axis=2)
-        _q_temp = np.array([_q0_temp, _q1_temp, _q2_temp, _q3_temp, _q4_temp], dtype=data_type)
-
-        _temp_filename = self.filename.replace('.q', '_3D.q')
-        with open(_temp_filename, 'wb') as f:
-            f.write(_a_temp.tobytes())
-            f.write(_b_temp.tobytes())
-            f.write(_q_temp.tobytes())
-
-        return
-
-    def mgrd_to_p3d(self, q, out_file: str = 'mgrd_to_p3d', mode: str = None, steps: int = 5, data_type='f4'):
-        """
-        Writes out data generated from scattered data interpolation to plot3d format
-        Args:
-            q:
-            out_file:
-            mode:
-            steps:
-            data_type:
-
-        Returns:
-
-        """
-        _a_temp = np.array([1, q.shape[1], q.shape[-1], int(steps)], dtype='i4')
-        _b_temp = np.array([self.mach, self.alpha, self.rey, self.time], dtype=data_type)
-        _q0 = np.expand_dims(q[0, ...], axis=2).T.repeat(int(steps), axis=0)
-        _q1 = np.expand_dims(q[1, ...], axis=2).T.repeat(int(steps), axis=0)
-        _q2 = np.expand_dims(q[2, ...], axis=2).T.repeat(int(steps), axis=0)
-        _q3 = np.expand_dims(q[3, ...], axis=2).T.repeat(int(steps), axis=0)
-        _q4 = np.expand_dims(q[4, ...], axis=2).T.repeat(int(steps), axis=0)
-        _q = np.array([_q0, _q1, _q2, _q3, _q4], dtype=data_type)
-
-        with open(out_file+'_'+mode+'.q', 'wb') as f:
-            f.write(_a_temp.tobytes())
-            f.write(_b_temp.tobytes())
-            f.write(_q.tobytes())
-
-        return
-
-    def read_formatted_txt(self, grid, data_type='f8'):
-        import os
-        """
-        Reads the formatted flow file generated from Tecplot. Needs grid object
-        Generate data from tecplot without the header, delimiter as space and have 5 variables
-        rho, rho-u, rho-v, rho-w, and e
-        Manually add all the required variables for flow object
-        Args:
-            grid: grid object related to the flow file
-            data_type: data type of the formatted text from Tecplot
-
-        Returns:
-            None
-
-        """
-        try:
-            # load the flow file if available
-            self.q = np.load(self.filename + '_temp/flow_data.npy')
-            print('**IMPORTANT** Read data from existing temp flow_data.npy file.\n')
-        except:
-            # Read the formatted data till the file ends and reshape it to (ni, nj, nk, 5, nb)
-            print('Starting flow read from the formatted text. Please wait...\n')
-            with open(self.filename, 'r') as flow:
-                self.q = np.fromfile(flow, sep=' ', dtype=data_type, count=-1)\
-                    .reshape((int(grid.nk), int(grid.nj), int(grid.ni), 5, 1)).transpose(2, 1, 0, 3, 4)
-
-            # Save as numpy file for future computations
-            try:
-                # Try creating the directory; if exists errors out and except
-                print('Trying to save to npy for future use\n')
-                os.mkdir(self.filename + '_temp')
-                np.save(self.filename + '_temp/flow_data', self.q)
-                print('Created _temp folder and saved flow data for future use.\n')
-            except:
-                np.save(self.filename + '_temp/flow_data', self.q)
-                print('Saved file for future use.\n')
-
-        # Fill in other variables
-        if self.mach is not None and self.rey is not None and self.alpha is not None and self.time is not None:
-            print('\nYour flow object is ready for further computations!\n')
-        else:
-            print('\nPlease fill out mach, rey, alpha, and time variables in the object\n')
-            print('\n** ERROR **: Try again; one of the required variables is not filled\n')
-            exit()
-
-        return
-
+# This file contains classes for plot3d data io
+# TODO: implement output for p3d data - Assigned to Harpreet.
+#  Each output function should be added to respective GridIO/FlowIO classes
+#  Change docstrings for doctest in test_io
+
+import numpy as np
+
+
+class GridIO:
+    """Module to read-in a grid file and output grid parameters
+
+    ...
+
+    Attributes
+    ----------
+    Input :
+        filename : str
+            name of the grid file
+    Output :
+        nb : int
+            number of blocks in the grid
+        ni, nj, nk : int
+            shape of the domain
+        grd : numpy.ndarray
+            Grid data of shape (ni, nj, nk, 3, nb)
+        grd_min: numpy.ndarray
+            min co-ordinates of each block (3, nb)
+        grd_max: numpy.ndarray
+            max co-ordinates of each block (3, nb)
+        m1 : numpy.ndarray
+            xi, eta, zeta derivatives wrt x, y, z --> shape (ni, nj, nk, 3, 3, nb)
+        m2 : numpy.ndarray
+            x, y, z derivatives wrt xi, eta, zeta --> shape (ni, nj, nk, 3, 3, nb)
+        J : numpy.ndarray
+            Jacobian determinant of m1 --> shape (ni, nj, nk, nb)
+
+
+    Methods
+    -------
+    read_grid()
+        returns the output attributes
+
+    Example:
+        grid = GridIO('plate.sp.x')  # Assume file is in the path
+        grid.read_grid()  # Call method to read the data
+        grid.compute_metrics()  # Computes m1, m2, J arrays
+        print(grid)  # prints the docstring for grid
+        # Instance attributes
+        print(grid.grd.shape)  # shape of the grid data
+        print(grid.nb)  # Number of blocks
+
+    author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
+    date: 10-05/2021
+    co-author: Harpreet Singh @ chhabrhh@mail.uc.edu
+    date: 01-20/2024
+    """
+
+    def __init__(self, filename):
+        self.filename = filename
+        self.nb = None
+        self.ni, self.nj, self.nk = None, None, None
+        self.grd = None
+        self.grd_min, self.grd_max = [], []
+        self.m1, self.m2 = None, None
+        self.J = None
+
+    def __str__(self):
+        doc = "This instance has the filename " + self.filename + "\n" + \
+              "grd attribute is of shape (ni, nj, nk, 3, nb), rows representing x,y,z coordinates for each block\n" \
+              "For example, x = grid.grd(...,0, 0), grid being the object.\n" \
+              "Use method 'read_grid' to compute grd attributes:\n" \
+              "ni, nj, nk, ng\n" \
+              "Use method 'compute_metrics' to compute grid metric attributes:\n" \
+              "m1, m2, J\n" \
+              "grd -- The grid data\n"
+        return doc
+
+    def read_grid(self, data_type='f4'):
+        """Reads in the grid file and changes the instance attributes
+
+        Parameters
+        -----------
+        data_type: str
+            Specify the data type of the grid file specified
+            Default is 'f4' for single-precision
+            For double-precision use 'f8'
+
+        Returns
+        -------
+        None
+
+        author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
+        credit: Paul Orkwis
+        date: 11-04/2021
+        """
+        with open(self.filename, 'r') as grid:
+            # Read-in number of blocks
+            self.nb = np.fromfile(grid, dtype='i4', count=1)[0]
+
+            # Read-in i, j, k for all blocks
+            _temp = np.fromfile(grid, dtype='i4', count=3 * self.nb)
+            self.ni, self.nj, self.nk = _temp[0::3], _temp[1::3], _temp[2::3]
+
+            # length of grd data
+            _nt = self.ni * self.nj * self.nk * 3
+            # read the grd data from file to temp_array
+            _temp = np.fromfile(grid, dtype=data_type, count=sum(_nt))
+
+            # pre-define grd to reduce calling pad and concatenate
+            self.grd = np.zeros((self.ni.max(), self.nj.max(), self.nk.max(), 3, self.nb))
+
+            # Reshape and assign data to grd
+            for _i in range(self.nb):
+                self.grd[0:self.ni[_i], 0:self.nj[_i], 0:self.nk[_i], 0:3, _i] = \
+                    _temp[sum(_nt[0:_i]):sum(_nt[0:_i]) + _nt[_i]] \
+                    .reshape((self.ni[_i], self.nj[_i], self.nk[_i], 3), order='F')
+
+            print("Grid data reading is successful for " + self.filename + "\n")
+
+            # Setup some parameters for further processing
+            # Find out the min and max of each block
+            for _i, _j, _k, _b in zip(self.ni, self.nj, self.nk, range(self.nb)):
+                self.grd_min.append(np.amin(self.grd[:_i, :_j, :_k, :, _b], axis=(0, 1, 2)))
+                self.grd_max.append(np.amax(self.grd[:_i, :_j, :_k, :, _b], axis=(0, 1, 2)))
+
+            # Convert lists to arrays
+            self.grd_min = np.array(self.grd_min)
+            self.grd_max = np.array(self.grd_max)
+
+    def compute_metrics(self):
+        """Calculate grid metrics from grid data.
+        Need to call read_grid() before computing metrics
+
+        Parameters
+        ----------
+
+        Returns
+        -------
+        None
+
+        Example:
+            grid = GridIO(filename)  # Assume grid is the object from GridIO
+            grid.read_grid()  # Call method to read-in grid data
+            grid.compute_metrics()  # Call method to compute grid metrics
+            print(grid)  # prints the docstring for grid metrics
+            # Instance attributes
+            print(grid.m1)  # derivatives xi, eta, zeta
+            print(grid.m2)  # derivatives x, y, z
+
+        author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
+        credit: Jacob Welsh for providing the code for single block
+        date: 12-23/2021
+        """
+        self.m1 = np.zeros((self.ni.max(), self.nj.max(), self.nk.max(), 3, 3, self.nb))
+        self.m2 = np.zeros((self.ni.max(), self.nj.max(), self.nk.max(), 3, 3, self.nb))
+        self.J = np.zeros((self.ni.max(), self.nj.max(), self.nk.max(), self.nb))
+
+        #  The for loop is to compute x, y, z derivatives wrt xi, eta, zeta
+        # for i in range(3):
+        #     self.m1[..., i, :] = np.gradient(self.grd, axis=i)
+
+        for b in range(self.nb):
+            print(f"Computing Jacobian for block {b}...")
+            for i in range(3):
+                self.m1[:self.ni[b], :self.nj[b], :self.nk[b], :, i, b] = \
+                    np.gradient(self.grd[:self.ni[b], :self.nj[b], :self.nk[b], :, b], axis=i)
+        print("Done computing Jacobian for all the blocks!!\n")
+
+        # compute Jacobian
+        for b in range(self.nb):
+            print(f"Computing Jacobian determinant for block {b}...")
+            self.J[:self.ni[b], :self.nj[b], :self.nk[b], b] = \
+                self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 0, b] * \
+                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b] -
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b]) - \
+                self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 0, b] * \
+                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b] -
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b]) + \
+                self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 0, b] * \
+                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b] -
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b])
+        print("Done computing Jacobian determinant for all the blocks!!")
+
+        # x derivatives
+        for b in range(self.nb):
+            print(f"Computing Inverse Jacobian for block {b}...")
+            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 0, 0, b] = \
+                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b] -
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b]) /\
+                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
+            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] = \
+                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b] -
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b]) /\
+                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
+            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] = \
+                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b] -
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b]) /\
+                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
+
+            # y derivative
+            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 1, 0, b] = \
+                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 0, b] -
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 0, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b]) /\
+                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
+            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b] = \
+                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 0, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b] -
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 0, b]) /\
+                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
+            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b] = \
+                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 2, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 0, b] -
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 0, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 2, b]) /\
+                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
+
+            # z derivatives
+            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 2, 0, b] = \
+                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 0, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b] -
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 0, b]) /\
+                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
+            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b] = \
+                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 0, b] -
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 0, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 2, 1, b]) /\
+                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
+            self.m2[:self.ni[b], :self.nj[b], :self.nk[b], 2, 2, b] = \
+                (self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 0, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 1, b] -
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 0, 1, b] *
+                 self.m1[:self.ni[b], :self.nj[b], :self.nk[b], 1, 0, b]) /\
+                self.J[:self.ni[b], :self.nj[b], :self.nk[b], b]
+
+        print("Done computing Inverse Jacobian for all the blocks!!")
+        print("All Grid metrics computed successfully!")
+
+    def two_to_three(self, steps: int = 5, step_size: float = None, data_type='f4'):
+        """
+        Converts 2D plot3d grid file to 3D format
+        TODO: Current limitation is that the code works only for 3d written 2d files and single block
+        Returns: None
+
+        """
+        if step_size is None:
+            print("Step size is not provided; Using minimum grid size")
+            step_size = abs(min(np.diff(self.grd[:, 0, 0, 0, 0])))
+
+        _a_temp = np.array([self.nb, self.ni, self.nj, steps], dtype='i4')
+        _x_temp = self.grd[..., 0, 0].repeat(steps, axis=2)
+        _y_temp = self.grd[..., 1, 0].repeat(steps, axis=2)
+        _z_temp = np.ones((int(self.ni), int(self.nj), steps)) * np.linspace(0, steps*step_size, steps)
+        _b_temp = np.array([_x_temp.T, _y_temp.T, _z_temp.T], dtype=data_type)
+
+        _temp_filename = self.filename.replace('.x', '_3D.x')
+        with open(_temp_filename, 'wb') as f:
+            f.write(_a_temp.tobytes())
+            f.write(_b_temp.tobytes())
+
+        print(f'\n File is successfully written in the working directory as {_temp_filename}')
+
+        return
+
+    def mgrd_to_p3d(self, xi, yi, out_file: str = 'mgrd_to_p3d.x',
+                    steps: int = 5, step_size: float = None, data_type='f4'):
+        """
+        Creates a 3d plot3d grid file;
+        This can be later used to be converted to 3d format by two_to_three
+        Returns:
+
+        """
+        if step_size is None:
+            print("Step size is not provided; Using minimum grid size")
+            step_size = abs(min(np.diff(self.grd[:, 0, 0, 0, 0])))
+
+        # Number of blocks is always 1 for this function
+        # Number of blocks is always 1 for this function
+        _ng, _ni, _nj, _nk = np.array([1, xi.shape[0], yi.shape[1], steps], dtype='i4')
+        _xx, _yy, _zz = np.meshgrid(xi[:, 0], yi[0], np.linspace(0, steps * step_size, steps), indexing='ij')
+        _grd = np.array([_xx.T, _yy.T, _zz.T], dtype=data_type)
+
+        with open(out_file, 'wb') as f:
+            f.write(_ng)
+            f.write(_ni)
+            f.write(_nj)
+            f.write(_nk)
+            f.write(_grd.tobytes())
+
+        print(f'\n File is successfully written in the working directory as {out_file}')
+
+        return
+
+
+class FlowIO:
+    """Module to read-in a flow file and output flow parameters
+
+    ...
+
+    Attributes
+    ----------
+    Input :
+        filename : str
+            name of the flow file
+    Output :
+        nb : int
+            number of blocks in the grid
+        ni, nj, nk : int
+            shape of the domain
+        mach, alpha, rey, time: float
+            extra numerics needed for post-processing
+        q : numpy.ndarray
+            Flow data of shape (ni, nj, nk, 5, nb)
+
+    Methods
+    -------
+    read_flow()
+        returns the output attributes
+    two_to_three()
+        converts 2D data to 3D
+    mgrd_to_p3d()
+        converts and returns meshgrid data to plot3D data
+    read_formatted_txt()
+        Reads Tecplot returned formatted text. Must contain five columns without headers
+        rho, rho-u, rho-v, rho-w, e are the five columns
+
+    Example:
+        grid = FlowIO('plate.sp.x')  # Assume file is in the path\n
+        flow.read_flow()  # Call method to read the data\n
+        print(flow)  # prints the docstring for grid\n
+        # Instance attributes\n
+        print(flow.q.shape)  # shape of the flow data\n
+        print(flow.ng)  # Number of blocks
+
+
+    author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
+    date: 10-05/2021
+    """
+
+    def __init__(self, filename):
+        self.filename = filename
+        self.nb = None
+        self.ni, self.nj, self.nk = None, None, None
+        self.mach = None
+        self.alpha = None
+        self.rey = None
+        self.time = None
+        self.q = None
+
+    def __str__(self):
+        doc = "This instance has the filename " + self.filename + "\n" + \
+              "q attribute is of shape (ni, nj, nk, 5, nb), rows representing density, momentum[*3], energy" \
+              "for every block\n" \
+              "For example, rho = flow.q(...,0,0), flow being the object for block-1.\n" \
+              "Use method 'read_flow' to compute attributes:\n" \
+              "nb, ni, nj, nk\n" \
+              "mach, alpha, rey, time\n" \
+              "q -- The flow data\n"
+        return doc
+
+    def read_flow(self, data_type='f4'):
+        """Reads in the flow file and changes the instance attributes
+
+        Parameters
+        ----------
+        data_type: str
+            Specify the data type of the flow file specified
+            Default is 'f4' for single-precision
+            For double-precision use 'f8'
+
+        Returns
+        -------
+        None
+
+        author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
+        credit: Paul Orkwis
+        date: 10-05/2021
+        """
+        with open(self.filename, 'r') as data:
+            self.nb = np.fromfile(data, dtype='i4', count=1)[0]
+
+            # Read in the i, j, k values for blocks
+            _temp = np.fromfile(data, dtype='i4', count=3 * self.nb)
+            self.ni, self.nj, self.nk = _temp[0::3], _temp[1::3], _temp[2::3]
+
+            # Read-in flow data into a temp array
+            # Less use of fromfile is more speed
+            _nt = self.ni * self.nj * self.nk * 5
+            _temp = np.fromfile(data, dtype=data_type, count=sum(_nt) + 4 * self.nb)
+
+            # Assign the dimensionless attributes
+            self.mach, self.alpha, self.rey, self.time = _temp[0:4]
+
+            # Create a mask to remove dimensionless quantities from q
+            # Indices of the first four dimensionless quantities
+            _index_array = np.array([0, 1, 2, 3])
+            for i in range(len(_nt) - 1):
+                _term = sum(_temp[0:i]) + (i + 1) * 4
+                _index_array = np.concatenate((_index_array, np.arange(_term, _term + 4)))
+            _mask = np.ones(len(_temp), dtype='bool')
+            _mask[_index_array] = 0
+            # Use the mask to remove dimensionless quantities
+            _temp = _temp[_mask]
+
+            # Pre-define q array
+            self.q = np.zeros((self.ni.max(), self.nj.max(), self.nk.max(), 5, self.nb))
+
+            # Reshape and assign data to q
+            for _i in range(self.nb):
+                self.q[0:self.ni[_i], 0:self.nj[_i], 0:self.nk[_i], 0:5, _i] = \
+                    _temp[sum(_nt[0:_i]):sum(_nt[0:_i]) + _nt[_i]] \
+                    .reshape((self.ni[_i], self.nj[_i], self.nk[_i], 5), order='F')
+
+            print("Flow data reading is successful for " + self.filename + "\n")
+
+    def two_to_three(self, steps: int = 5, data_type='f4'):
+        """
+        Converts 2D plot3d flow file to 3D format
+        TODO: Current limitation is that the code works only for 3d written 2d files and single block
+        Returns: None
+
+        """
+        # TODO: The code below needs debugging. It's not tested. mgrd_to_p3d might help!
+        _a_temp = np.array([self.nb, self.ni, self.nj, int(steps)], dtype='i4')
+        _b_temp = np.array([self.mach, self.alpha, self.rey, self.time], dtype=data_type)
+        _q0_temp = self.q[..., 0, 0].repeat(int(steps), axis=2)
+        _q1_temp = self.q[..., 1, 0].repeat(int(steps), axis=2)
+        _q2_temp = self.q[..., 2, 0].repeat(int(steps), axis=2)
+        _q3_temp = self.q[..., 3, 0].repeat(int(steps), axis=2)
+        _q4_temp = self.q[..., 4, 0].repeat(int(steps), axis=2)
+        _q_temp = np.array([_q0_temp, _q1_temp, _q2_temp, _q3_temp, _q4_temp], dtype=data_type)
+
+        _temp_filename = self.filename.replace('.q', '_3D.q')
+        with open(_temp_filename, 'wb') as f:
+            f.write(_a_temp.tobytes())
+            f.write(_b_temp.tobytes())
+            f.write(_q_temp.tobytes())
+
+        return
+
+    def mgrd_to_p3d(self, q, out_file: str = 'mgrd_to_p3d', mode: str = None, steps: int = 5, data_type='f4'):
+        """
+        Writes out data generated from scattered data interpolation to plot3d format
+        Args:
+            q:
+            out_file:
+            mode:
+            steps:
+            data_type:
+
+        Returns:
+
+        """
+        _a_temp = np.array([1, q.shape[1], q.shape[-1], int(steps)], dtype='i4')
+        _b_temp = np.array([self.mach, self.alpha, self.rey, self.time], dtype=data_type)
+        _q0 = np.expand_dims(q[0, ...], axis=2).T.repeat(int(steps), axis=0)
+        _q1 = np.expand_dims(q[1, ...], axis=2).T.repeat(int(steps), axis=0)
+        _q2 = np.expand_dims(q[2, ...], axis=2).T.repeat(int(steps), axis=0)
+        _q3 = np.expand_dims(q[3, ...], axis=2).T.repeat(int(steps), axis=0)
+        _q4 = np.expand_dims(q[4, ...], axis=2).T.repeat(int(steps), axis=0)
+        _q = np.array([_q0, _q1, _q2, _q3, _q4], dtype=data_type)
+
+        with open(out_file+'_'+mode+'.q', 'wb') as f:
+            f.write(_a_temp.tobytes())
+            f.write(_b_temp.tobytes())
+            f.write(_q.tobytes())
+
+        return
+
+    def read_formatted_txt(self, grid, data_type='f8'):
+        import os
+        """
+        Reads the formatted flow file generated from Tecplot. Needs grid object
+        Generate data from tecplot without the header, delimiter as space and have 5 variables
+        rho, rho-u, rho-v, rho-w, and e
+        Manually add all the required variables for flow object
+        Args:
+            grid: grid object related to the flow file
+            data_type: data type of the formatted text from Tecplot
+
+        Returns:
+            None
+
+        """
+        try:
+            # load the flow file if available
+            self.q = np.load(self.filename + '_temp/flow_data.npy')
+            print('**IMPORTANT** Read data from existing temp flow_data.npy file.\n')
+        except:
+            try:
+                # Read the formatted data till the file ends and reshape it to (ni, nj, nk, 5, nb)
+                print('Starting flow read from the formatted text. Please wait...\n')
+                with open(self.filename, 'r') as flow:
+                    self.q = np.fromfile(flow, sep=' ', dtype=data_type, count=-1)\
+                        .reshape((int(grid.nk), int(grid.nj), int(grid.ni), 5, 1)).transpose(2, 1, 0, 3, 4)
+                print('Flow data reading is successful for ' + self.filename + '\n')
+            except ValueError:
+                # check for 2D formatted data
+                # read the formatted data till the file ends and reshape it to (ni, nj, 1, 5, nb)
+                # and expand it to (ni, nj, nk, 5, nb)
+                with open(self.filename, 'r') as flow:
+                    self.q = np.fromfile(flow, sep=' ', dtype=data_type, count=-1)\
+                        .reshape((1, int(grid.nj), int(grid.ni), 5, 1)).transpose(2, 1, 0, 3, 4)
+                self.q = self.q.repeat(int(grid.nk), axis=2)
+                print('Flow data reading is successful for ' + self.filename + '\n')
+
+
+            # Save as numpy file for future computations
+            try:
+                # Try creating the directory; if exists errors out and except
+                print('Trying to save to npy for future use\n')
+                os.mkdir(self.filename + '_temp')
+                np.save(self.filename + '_temp/flow_data', self.q)
+                print('Created _temp folder and saved flow data for future use.\n')
+            except:
+                np.save(self.filename + '_temp/flow_data', self.q)
+                print('Saved file for future use.\n')
+
+        # Fill in other variables
+        if self.mach is not None and self.rey is not None and self.alpha is not None and self.time is not None:
+            print('\nYour flow object is ready for further computations!\n')
+        else:
+            print('\nPlease fill out mach, rey, alpha, and time variables in the object\n')
+            print('\n** ERROR **: Try again; one of the required variables is not filled\n')
+            exit()
+
+        return
+
```

### Comparing `project-arrakis-0.1/src/streamlines/integration.py` & `project_arrakis-0.1.1/src/streamlines/integration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,608 +1,799 @@
-# Integrate from given point to produce streamlines
-import numpy as np
-from src.streamlines.interpolation import Interpolation
-from src.streamlines.search import Search
-from src.function.variables import Variables
-
-
-class Integration:
-
-    def __init__(self, interp):
-        self.interp = interp
-        self.ppoint = None
-        self.cpoint = None
-        self.rk4_bool = False
-
-    def __str__(self):
-        doc = "This instance uses data from " + self.interp.flow.filename + \
-              " and integrates based on the given time step"
-        return doc
-
-    def compute(self, method='p-space', time_step=1e-6):
-        match method:
-            case 'p-space':
-                # For p-space algos; the point-in-domain check was done in search
-                if self.interp.idx.ppoint is None:
-                    self.ppoint = None
-                    return self.ppoint
-
-                # Compute required variables from plot3d data
-                q_interp = Variables(self.interp)
-                q_interp.compute_velocity()
-                # Integration for one time step
-                self.ppoint = self.interp.idx.ppoint + q_interp.velocity.reshape(3) * time_step
-
-                return self.ppoint
-
-            case 'c-space':
-                # Get inverse Jacobian from the interpolation class
-                # Using cell node data. For more accurate calculation refer to cRK4 method
-                _J_inv = self.interp.idx.grid.m2[self.interp.idx.cell[0, 0], self.interp.idx.cell[0, 1],
-                                                 self.interp.idx.cell[0, 2], :, :, self.interp.idx.block]
-
-                q_interp = Variables(self.interp)
-                q_interp.compute_velocity()
-                p_velocity = q_interp.velocity.reshape(3)
-                c_velocity = np.matmul(_J_inv, p_velocity)
-                self.cpoint = self.interp.idx.cpoint + c_velocity * time_step
-
-                # For c-space the point in-domain check is done after integration
-                if not np.all([0, 0, 0] <= self.cpoint) or not np.all(
-                        self.cpoint + 1 < [self.interp.idx.grid.ni[self.interp.idx.block],
-                                           self.interp.idx.grid.nj[self.interp.idx.block],
-                                           self.interp.idx.grid.nk[self.interp.idx.block]]):
-                    self.cpoint = None
-                    return self.cpoint
-
-                return self.cpoint
-
-            case 'pRK4':
-                """
-                This is a straight forward RK4 integration. Search for the point,
-                Interpolate the data to the point, Compute required variables,
-                Perform RK4 integration!
-                """
-
-                def _rk4_step(self, x):
-                    """
-
-                    Args:
-                        self:
-                        x: ndarray
-                            point in p-space
-
-                    Returns:
-                        k: ndarray
-                            interim RK4 variables
-
-                    """
-                    idx = Search(self.interp.idx.grid, x)
-                    idx.compute(method='p-space')
-                    # For p-space algos; the point-in-domain check was done in search
-                    if idx.ppoint is None: return None, None
-                    interp = Interpolation(self.interp.flow, idx)
-                    interp.compute()
-                    q_interp = Variables(interp)
-                    q_interp.compute_velocity()
-                    u = q_interp.velocity.reshape(3)
-                    k = time_step * u
-                    return u, k
-
-                # Start RK4 for p-space
-                # For p-space algos; the point-in-domain check was done in search
-                x0 = self.interp.idx.ppoint
-                if x0 is None: return None, None
-                q_interp = Variables(self.interp)
-                q_interp.compute_velocity()
-                u0 = q_interp.velocity.reshape(3)
-                k0 = time_step * u0
-                x1 = x0 + k0
-
-                u1, k1 = _rk4_step(self, x1)
-                if k1 is None: return None, None
-                x2 = x0 + 0.5 * k1
-
-                u2, k2 = _rk4_step(self, x2)
-                if k2 is None: return None, None
-                x3 = x0 + 0.5 * k2
-
-                u3, k3 = _rk4_step(self, x3)
-                if k3 is None: return None, None
-                x4 = x0 + 1/6 * (k0 + 2*k1 + 2*k2 + k3)
-                u4, k4 = _rk4_step(self, x4)
-                if k4 is None: return None, None
-
-                self.ppoint = x4
-
-                return self.ppoint, u4
-
-            case 'cRK4':
-                '''
-                This is a block-wise integration. Everytime the point gets out
-                a pRK4 is run to find the new block the point is located in.
-                That particular step is done in streamlines algorithm.
-                
-                All the points, x0, x1... are in c-space
-                
-                Point location is known in c-space, avoiding search.
-                Interpolates data to the point
-                RK4 integration is performed!
-                '''
-
-                def _rk4_step(self, x):
-                    """
-
-                    Args:
-                        self:
-                        x: ndarray
-                            point in c-space
-
-                    Returns:
-                        k: ndarray
-                            interim RK4 variables
-
-                    """
-                    idx = Search(self.interp.idx.grid, x)
-                    idx.block = self.interp.idx.block
-                    idx.c2p(x)  # This will change the cell attribute
-                    # In-domain check is done in search
-                    if idx.cpoint is None:
-                        self.cpoint = None
-                        self.ppoint = None
-                        return None, None, None
-                    interp = Interpolation(self.interp.flow, idx)
-                    interp.compute(method='c-space')
-                    _J_inv = interp.J_inv
-                    q_interp = Variables(interp)
-                    q_interp.compute_velocity()
-                    p_velocity = q_interp.velocity.reshape(3)
-                    c_velocity = np.matmul(_J_inv, p_velocity)
-                    k = time_step * c_velocity
-                    return k, p_velocity, c_velocity
-
-                x0 = self.interp.idx.cpoint
-                _J_inv = self.interp.J_inv
-                if x0 is None:
-                    return None, None, None
-
-                q_interp = Variables(self.interp)
-                q_interp.compute_velocity()
-                p_velocity = q_interp.velocity.reshape(3)
-                c_velocity = np.matmul(_J_inv, p_velocity)
-                k0 = time_step * c_velocity
-                x1 = x0 + k0
-
-                k1, pv1, cv1 = _rk4_step(self, x1)
-                if k1 is None:
-                    return None, None, None
-                x2 = x0 + 0.5 * k1
-
-                k2, pv2, cv2 = _rk4_step(self, x2)
-                if k2 is None:
-                    return None, None, None
-                x3 = x0 + 0.5 * k2
-
-                k3, pv3, cv3 = _rk4_step(self, x3)
-                if k3 is None:
-                    return None, None, None
-                x4 = x0 + 1/6 * (k0 + 2*k1 + 2*k2 + k3)
-                k4, pv4, cv4 = _rk4_step(self, x4)
-                if k4 is None:
-                    return None, None, None
-
-                self.cpoint = x4
-
-                return self.cpoint, pv4, cv4
-
-    def compute_ppath(self, diameter=1e-6, density=1000, velocity=None,
-                      method='pRK4', time_step=1e-4, drag_model='stokes'):
-
-        def _drag_constant(_re, _q_interp=None, _mach=None, _gamma=None, _mu=None, _model=drag_model):
-            """
-            Coefficient of drag for a spherical particle
-
-            Args:
-                _re : Relative Reynolds Number
-                _mach : Relative Mach Number
-                _model : Drag Model Name
-                    Available models are 'sphere', 'stokes', 'oseen', 'schiller_nauman',
-                    'cunningham'
-
-            Returns:
-                coefficient of drag based on local flow/particle properties
-
-            """
-            match _model:
-                case 'zero-drag':
-                    # zero drag model to simulate fluid
-                    return 0
-                case 'sphere':
-                    # ref: Fluid Mechanics, Frank M. White
-                    # This was decided by trail-and-error from VISUAL3 code
-                    if _re <= 1e-9:
-                        return 0
-                    if _re < 1e-3:
-                        return 24 / _re
-                    if 1e-3 <= _re < 0.45:
-                        return 24 / _re * (1 + 3 * _re / 16)
-                    if 0.45 <= _re < 1:
-                        # Same as above due to lack of data
-                        return 24 / _re * (1 + 3 * _re / 16)
-                    if 1 <= _re < 800:
-                        return 24 / _re * (1 + _re ** (2 / 3) / 6)
-                    if 800 <= _re < 3e5:
-                        return 0.44
-                    if 3e5 <= _re < 4e5:
-                        # Same as above due to lack of data
-                        return 0.44
-                    if _re >= 4e5:
-                        return 0.07
-
-                case 'stokes':
-                    # Stokes Drag; for creeping flow regime; Re << 1
-                    if _re <= 1e-9:
-                        return 0
-                    else:
-                        return 24/_re
-
-                case 'melling':
-                # The popular melling correction
-                    if _re <= 1e-9:
-                        return 0
-                    else:
-                        knd = _mach / _re * np.sqrt(np.pi*_gamma/2)
-                        return 24/_re * (1 + knd)**-1
-
-                case 'oseen':
-                    # Oseen's model; for creeping flow regime; Re < 1
-                    if _re <= 1e-9:
-                        return 0
-                    else:
-                        return 24/_re * (1 + 3/16 * _re)
-
-                case 'schiller-nauman':
-                    # Schiller and Nauman's model; for Re <~ 200 & M <~ 0.25
-                    if _re <= 1e-9:
-                        return 0
-                    else:
-                        return 24/_re * (1 + 0.15 * _re**0.687)
-
-                case 'cunningham':
-                    # Cunningham model; for Re << 1; M << 1; Kn <~ 0.1
-                    # Knudsen number
-                    # _r = _q_interp.density * _q_interp.velocity_magnitude * diameter / _mu
-                    if _re <= 1e-9:
-                        return 0
-                    if _re <= 1:
-                        _kn = _mach / _re * np.sqrt(_q_interp.gamma * np.pi/2)
-                        return 24/_re * (1 + 4.5*_kn)**-1
-                    if _re > 1:
-                        _kn = _mach / np.sqrt(_re)
-                        return 24/_re * (1 + 4.5*_kn)**-1
-
-                case 'henderson':
-                    # Henderson model; for all flow regimes
-                    # Simplified by ignoring sphere temperature
-                    if _re < 1e-9:
-                        return 0
-
-                    # For Mach < 1
-                    _s = _mach * np.sqrt(_gamma/2)
-                    _f1 = 24 * (_re + _s * (5.89688 * np.exp(-0.247 * _re/_s)))**-1
-                    _f2 = np.exp(-0.5*_mach/np.sqrt(_re)) * \
-                                ((4.5 + 0.38*(0.03*_re + 0.48*np.sqrt(_re))) / (1 + 0.03*_re + 0.48*np.sqrt(_re)) +
-                                 0.1*_mach**2 + 0.2*_mach**8)
-                    _f3 = (1 - np.exp(-_mach/_re))*0.6*_s
-                    _cd1 = _f1 + _f2 + _f3
-                    if _mach < 1:
-                        return _cd1
-
-                    # For Mach >= 1.75
-                    _mach_inf = _mach
-                    _re_inf = _re
-                    _s_inf = _mach_inf * np.sqrt(_gamma/2)
-                    _g1 = 0.9 + 0.34/_mach_inf**2
-                    _g2 = 1.86 * np.sqrt(_mach_inf/_re_inf) * (2 + 2/_s_inf**2 + 1.058/_s_inf - 1/_s_inf**4)
-                    _g3 = 1 + 1.86 * np.sqrt(_mach_inf/_re_inf)
-                    _cd2 = (_g1 + _g2) / _g3
-                    if _mach >= 1.75:
-                        return _cd2
-
-                    # For 1 <= Mach < 1.75; linear interpolation
-                    if 1 <= _mach < 1.75:
-                        return _cd1 + 4/3 * (_mach_inf - 1) * (_cd2 - _cd1)
-
-                case 'subramaniam-balachandar':
-                    # Model from their new book
-                    if _re < 1e-9:
-                        return 0
-
-                    if _re < 0.5:
-                        # Stokes
-                        return 24/_re
-
-                    if _re < 20:
-                        # Clift
-                        return 24/_re * (1 + 0.1315 * _re**(0.82-0.05*np.log10(_re)))
-
-                    if _re < 800:
-                        # Schiller-Naumann
-                        return 24/_re * (1 + 0.15 * _re**0.687)
-
-                    if _re < 3e5:
-                        # Clift-Gauvin
-                        return 24/_re * (1 + 0.15 * _re**0.687 + 0.42/24 * _re * (1 + 4.25e4 * _re**(-1.16))**-1)
-
-                case 'loth':
-                    # Loth's model; for all flow regimes
-                    if _re < 1e-9:
-                        return 0
-
-                    if _re < 45:
-                    # Rarefraction dominated domain
-                        import math
-                        _s = _mach * np.sqrt(_gamma/2)
-                        _cd_fm = (1 + 2 * _s**2) * np.exp(-_s**2) / (_s**3 * np.pi**0.5) + \
-                                 (4*_s**4 + 4*_s**2 - 1) * math.erf(_s) / (2*_s**4) + 2 * np.pi**0.5 / (3 * _s)
-                        _cd_fm_re = _cd_fm / (1 + (_cd_fm/1.63 - 1) * (_re/45)**0.5)
-                        _kn = (np.pi * _gamma / 2)**0.5 * _mach / _re
-                        _f_kn = (1 + _kn * (2.514 + 0.8 * np.exp(-0.55/_kn)))**-1
-                        _cd_kn_re = 24/_re * (1 + 0.15 * _re**0.687) * _f_kn
-                        _cd = (_cd_kn_re + _mach**4 * _cd_fm_re) / (1 + _mach**4)
-                        return _cd
-
-                    if _re > 45:
-                    # compression-dominated regime
-                        if _mach <= 1.45:
-                            _cm = 5/3 + 2/3 * np.tanh(3 * np.log(_mach - 0.1))
-                        if _mach > 1.45:
-                            _cm = 2.044 + 0.2 * np.exp(-1.8 * (np.log(_mach/1.5))**2)
-                        if _mach <= 0.89:
-                            _gm = 1 - 1.525 * _mach**4
-                        if _mach > 0.89:
-                            _gm = 2e-4 + 8e-4 * np.tanh(12.77 * (_mach - 2.02))
-                        _hm = 1 - 0.258 * _cm / (1 + 514 * _gm)
-                        _cd = 24/_re * (1 + 0.15 * _re**0.687) * _hm + 0.42 * _cm / (1 + 42000 * _gm / _re**1.16)
-                        return _cd
-
-                    return
-
-        def _viscosity(_temperature):
-            # Sutherland's viscosity law
-            # All temperatures must be in kelvin
-            # Formula from cfd-online
-            _c1 = 1.716e-5 * (273.15 + 110.4) / 273.15**1.5
-            _mu = _c1 * _temperature**1.5 / (_temperature + 110.4)
-            return _mu
-
-        match method:
-            case 'pRK4':
-
-                def _rk4_step(self, vp, x):
-                    """
-
-                    Args:
-                        self:
-
-                    Returns:
-                        k: ndarray
-                            interim RK4 variables
-
-                    """
-                    idx = Search(self.interp.idx.grid, x)
-                    idx.compute(method='p-space')
-                    # For p-space algos; the point-in-domain check was done in search
-                    if idx.ppoint is None:
-                        return None, None, None
-                    interp = Interpolation(self.interp.flow, idx)
-                    interp.compute()
-                    q_interp = Variables(interp)
-                    # Compute all variables
-                    q_interp.compute_mach()
-                    uf = q_interp.velocity.reshape(3)
-                    # particle dynamics
-                    _rhof = q_interp.density.reshape(-1)
-                    dp = diameter
-                    rhop = density
-                    mu = _viscosity(q_interp.temperature.reshape(-1))
-                    # Relative Reynolds Number
-                    re = _rhof * np.linalg.norm(vp - uf) * dp / mu
-                    _mach = np.linalg.norm(vp - uf) * q_interp.mach.reshape(-1) /\
-                            q_interp.velocity_magnitude.reshape(-1)
-                    _cd = _drag_constant(re, _q_interp=q_interp, _mach=_mach,
-                                         _gamma=q_interp.gamma, _mu=mu, _model=drag_model)
-                    _k = -0.75 * _rhof / (rhop * dp)
-                    _vk = _cd * _k * (vp - uf) * np.linalg.norm(vp - uf) * time_step
-                    return _vk, uf, None
-
-                # Start RK4 for p-space
-                # For p-space algos; the point-in-domain check was done in search
-                x0 = self.interp.idx.ppoint
-                if x0 is None:
-                    return None, None, None
-                q_interp = Variables(self.interp)
-                q_interp.compute_velocity()
-                u0 = q_interp.velocity.reshape(3)
-                # Assign velocity to start Rk4 step
-                if velocity is None:
-                    v0 = u0.copy()
-                else:
-                    v0 = velocity.copy()
-                vk0, uf0, temp = _rk4_step(self, v0, x0)
-                # Assign fluid velocity when vk is zero
-                # Theory: When zero drag particle is massless, hence fluid velocity
-                if np.linalg.norm(vk0) == 0:
-                    v0 = uf0.copy()
-                v1 = v0 + vk0
-                xk0 = v1 * time_step
-                x1 = x0 + xk0
-
-                vk1, uf1, temp = _rk4_step(self, v1, x1)
-                if vk1 is None:
-                    return None, None, None
-                if np.linalg.norm(vk1) == 0:
-                    v0 = uf1.copy()
-                v2 = v0 + 0.5 * vk1
-                xk1 = v2 * time_step
-                x2 = x0 + 0.5 * xk1
-                # Check for mid-RK4 blow-up issue. Happens when Cd and time-step are high
-                if np.linalg.norm(x2 - x0) >= 10 * np.linalg.norm(x1-x0):
-                    self.rk4_bool = True
-                    return x0, v0, u0
-
-                vk2, uf2, temp = _rk4_step(self, v2, x2)
-                if vk2 is None:
-                    return None, None, None
-                if np.linalg.norm(vk2) == 0:
-                    v0 = uf2.copy()
-                v3 = v0 + 0.5 * vk2
-                xk2 = v3 * time_step
-                x3 = x0 + 0.5 * xk2
-                # Check for mid-RK4 blow-up issue. Happens when Cd and time-step are high
-                if np.linalg.norm(x3 - x0) >= 10 * np.linalg.norm(x1 - x0):
-                    self.rk4_bool = True
-                    return x0, v0, u0
-
-                vk3, uf3, temp = _rk4_step(self, v3, x3)
-                if vk3 is None:
-                    return None, None, None
-                if np.linalg.norm(vk3) == 0:
-                    v0 = uf3.copy()
-                v4 = v0 + 1 / 6 * (vk0 + 2 * vk1 + 2 * vk2 + vk3)
-                xk3 = v4 * time_step
-                x4 = x0 + 1 / 6 * (xk0 + 2 * xk1 + 2 * xk2 + xk3)
-                # Check for mid-RK4 blow-up issue. Happens when Cd and time-step are high
-                if np.linalg.norm(x4 - x0) >= 10 * np.linalg.norm(x1 - x0):
-                    self.rk4_bool = True
-                    return x0, v0, u0
-
-                vk4, uf4, temp = _rk4_step(self, v4, x4)
-                if vk4 is None:
-                    return None, None, None
-
-                self.ppoint = x4
-
-                return x4, v4, uf4
-
-            case 'cRK4':
-
-                def _rk4_step(self, c_vp, x):
-                    """
-                    Returns required data for the RK4 step
-
-                    Args:
-                        self:
-                        x: ndarray
-                            point in c-space
-
-                    Returns:
-                        k: ndarray
-                            interim RK4 variables
-
-                    """
-                    if np.any(x < 0):
-                        return None, None, None, None, None
-                    idx = Search(self.interp.idx.grid, x)
-                    idx.block = self.interp.idx.block
-                    idx.c2p(x)  # This will change the cell attribute
-                    # In-domain check is done in search
-                    if idx.cpoint is None:
-                        self.cpoint = None
-                        self.ppoint = None
-                        return None, None, None, None, None
-                    interp = Interpolation(self.interp.flow, idx)
-                    interp.compute(method='c-space')
-                    _J_inv = interp.J_inv
-                    _J = interp.J
-                    q_interp = Variables(interp)
-                    # Computing mach get all the necessary variables
-                    q_interp.compute_mach()
-                    p_uf = q_interp.velocity.reshape(3)
-                    c_uf = np.matmul(_J_inv, p_uf)
-                    # particle dynamics
-                    _rhof = q_interp.density.reshape(-1)
-                    dp = diameter
-                    rhop = density
-                    # Transform particle velocity to p-space
-                    p_vp = np.matmul(_J, c_vp)
-                    mu = _viscosity(q_interp.temperature.reshape(-1))
-                    # Relative Reynolds Number
-                    re = _rhof * np.linalg.norm(c_vp - c_uf) * dp / mu
-                    _mach = np.linalg.norm(c_vp - c_uf) * q_interp.mach.reshape(-1) /\
-                            q_interp.velocity_magnitude.reshape(-1)
-                    _cd = _drag_constant(re, _q_interp=q_interp, _mach=_mach,
-                                         _gamma=q_interp.gamma, _mu=mu, _model=drag_model)
-                    _k = -0.75 * _rhof / (rhop * dp)
-                    _vk = _cd * _k * (c_vp - c_uf) * np.linalg.norm(c_vp - c_uf) * time_step
-                    return _vk, p_uf, c_uf, p_vp, c_vp
-
-                # Start RK4 for c-space
-                x0 = self.interp.idx.cpoint
-                if x0 is None:
-                    return None, None, None
-                q_interp = Variables(self.interp)
-                q_interp.compute_velocity()
-                p_u0 = q_interp.velocity.reshape(3)
-                c_u0 = np.matmul(self.interp.J_inv, p_u0)
-                # Assign velocity to start Rk4 step
-                if velocity is None:
-                    c_v0 = c_u0.copy()
-                else:
-                    c_v0 = np.matmul(self.interp.J_inv, velocity)
-                vk0, p_u0, c_u0, p_v0, c_v0 = _rk4_step(self, c_v0, x0)
-                # Assign fluid velocity when vk is zero
-                # Theory: When zero drag particle is massless, hence fluid velocity
-                if np.linalg.norm(vk0) == 0:
-                    c_v0 = c_u0.copy()
-                c_v1 = c_v0 + vk0
-                xk0 = c_v1 * time_step
-                x1 = x0 + xk0
-
-                # Integration starts
-                vk1, p_u1, c_u1, p_v1, c_v1 = _rk4_step(self, c_v1, x1)
-                # if the residual is none return; exited the domain
-                if vk1 is None:
-                    return None, None, None
-                # if zero; particle is acting like massless particle; low relative reynolds number cases
-                if np.linalg.norm(vk1) == 0:
-                    c_v0 = c_u1.copy()
-                c_v2 = c_v0 + 0.5 * vk1
-                xk1 = c_v2 * time_step
-                x2 = x0 + 0.5 * xk1
-                # Check for mid-RK4 blow up due to residuals
-                if np.linalg.norm(x2 - x0) >= 10 * np.linalg.norm(x1-x0):
-                    self.rk4_bool = True
-                    return x0, p_v0, p_u0
-
-                # Repeat three more times; RK4
-                vk2, p_u2, c_u2, p_v2, c_v2 = _rk4_step(self, c_v2, x2)
-                if vk2 is None:
-                    return None, None, None
-                if np.linalg.norm(vk2) == 0:
-                    c_v0 = c_u2.copy()
-                c_v3 = c_v0 + 0.5 * vk2
-                xk2 = c_v3 * time_step
-                x3 = x0 + 0.5 * xk2
-                if np.linalg.norm(x3 - x0) >= 10 * np.linalg.norm(x1-x0):
-                    self.rk4_bool = True
-                    return x0, p_v0, p_u0
-
-                vk3, p_u3, c_u3, p_v3, c_v3 = _rk4_step(self, c_v3, x3)
-                if vk3 is None:
-                    return None, None, None
-                if np.linalg.norm(vk3) == 0:
-                    c_v0 = c_u3.copy()
-                c_v4 = c_v0 + 1 / 6 * (vk0 + 2 * vk1 + 2 * vk2 + vk3)
-                xk3 = c_v4 * time_step
-                x4 = x0 + 1 / 6 * (xk0 + 2 * xk1 + 2 * xk2 + xk3)
-                if np.linalg.norm(x4 - x0) >= 10 * np.linalg.norm(x1-x0):
-                    self.rk4_bool = True
-                    return x0, p_v0, p_u0
-
-                vk4, p_u4, c_u4, p_v4, c_v4 = _rk4_step(self, c_v4, x4)
-                if vk4 is None:
-                    return None, None, None
-
-                self.cpoint = x4
-
-                return x4, p_u4, p_v4
+# Integrate from given point to produce streamlines
+import numpy as np
+from src.streamlines.interpolation import Interpolation
+from src.streamlines.search import Search
+from src.function.variables import Variables
+from scipy.optimize import fsolve
+
+
+class Integration:
+
+    def __init__(self, interp):
+        self.interp = interp
+        self.ppoint = None
+        self.cpoint = None
+        self.rk4_bool = False
+
+    def __str__(self):
+        doc = "This instance uses data from " + self.interp.flow.filename + \
+              " and integrates based on the given time step"
+        return doc
+
+    def compute(self, method='p-space', time_step=1e-6):
+        match method:
+            case 'p-space':
+                # For p-space algos; the point-in-domain check was done in search
+                if self.interp.idx.ppoint is None:
+                    self.ppoint = None
+                    return self.ppoint
+
+                # Compute required variables from plot3d data
+                q_interp = Variables(self.interp)
+                q_interp.compute_velocity()
+                # Integration for one time step
+                self.ppoint = self.interp.idx.ppoint + q_interp.velocity.reshape(3) * time_step
+
+                return self.ppoint
+
+            case 'c-space':
+                # Get inverse Jacobian from the interpolation class
+                # Using cell node data. For more accurate calculation refer to cRK4 method
+                _J_inv = self.interp.idx.grid.m2[self.interp.idx.cell[0, 0], self.interp.idx.cell[0, 1],
+                                                 self.interp.idx.cell[0, 2], :, :, self.interp.idx.block]
+
+                q_interp = Variables(self.interp)
+                q_interp.compute_velocity()
+                p_velocity = q_interp.velocity.reshape(3)
+                c_velocity = np.matmul(_J_inv, p_velocity)
+                self.cpoint = self.interp.idx.cpoint + c_velocity * time_step
+
+                # For c-space the point in-domain check is done after integration
+                if not np.all([0, 0, 0] <= self.cpoint) or not np.all(
+                        self.cpoint + 1 < [self.interp.idx.grid.ni[self.interp.idx.block],
+                                           self.interp.idx.grid.nj[self.interp.idx.block],
+                                           self.interp.idx.grid.nk[self.interp.idx.block]]):
+                    self.cpoint = None
+                    return self.cpoint
+
+                return self.cpoint
+
+            case 'pRK2':
+                """
+                This is a straight forward RK2 integration. Search for the point,
+                Interpolate the data to the point, Compute required variables,
+                Perform RK4 integration!
+                """
+
+                def _rk2_step(self, x):
+                    """
+
+                    Args:
+                        self:
+                        x: ndarray
+                            point in p-space
+
+                    Returns:
+                        k: ndarray
+                            interim RK4 variables
+
+                    """
+                    idx = Search(self.interp.idx.grid, x)
+                    idx.compute(method='p-space')
+                    # For p-space algos; the point-in-domain check was done in search
+                    if idx.ppoint is None: return None, None
+                    interp = Interpolation(self.interp.flow, idx)
+                    interp.adaptive = self.interp.adaptive
+                    interp.rbf_kernel = self.interp.rbf_kernel
+                    interp.compute(method=self.interp.method)
+                    q_interp = Variables(interp)
+                    q_interp.compute_velocity()
+                    u = q_interp.velocity.reshape(3)
+                    k = time_step * u
+                    return u, k
+
+                # Start RK4 for p-space
+                # For p-space algos; the point-in-domain check was done in search
+                x0 = self.interp.idx.ppoint
+                if x0 is None: return None, None
+                q_interp = Variables(self.interp)
+                q_interp.compute_velocity()
+                u0 = q_interp.velocity.reshape(3)
+                k0 = time_step * u0
+                x1 = x0 + k0
+
+                u1, k1 = _rk2_step(self, x1)
+                if k1 is None: return None, None
+
+                x_new = x0 + 1/2 * (k0 + k1)
+                u_new, k_new = _rk2_step(self, x_new)
+                if k_new is None: return None, None
+
+                self.ppoint = x_new
+
+                return self.ppoint, u_new
+
+            case 'cRK2':
+                '''
+                This is a block-wise integration. Everytime the point gets out
+                a pRK4 is run to find the new block the point is located in.
+                That particular step is done in streamlines algorithm.
+
+                All the points, x0, x1... are in c-space
+
+                Point location is known in c-space, avoiding search.
+                Interpolates data to the point
+                RK4 integration is performed!
+                '''
+
+                def _rk2_step(self, x):
+                    """
+
+                    Args:
+                        self:
+                        x: ndarray
+                            point in c-space
+
+                    Returns:
+                        k: ndarray
+                            interim RK2 variables
+
+                    """
+                    idx = Search(self.interp.idx.grid, x)
+                    idx.block = self.interp.idx.block
+                    idx.c2p(x)  # This will change the cell attribute
+                    # In-domain check is done in search
+                    if idx.cpoint is None:
+                        self.cpoint = None
+                        self.ppoint = None
+                        return None, None, None
+                    interp = Interpolation(self.interp.flow, idx)
+                    interp.adaptive = self.interp.adaptive
+                    interp.rbf_kernel = self.interp.rbf_kernel
+                    interp.compute(method=self.interp.method)
+                    _J_inv = interp.J_inv
+                    q_interp = Variables(interp)
+                    q_interp.compute_velocity()
+                    p_velocity = q_interp.velocity.reshape(3)
+                    c_velocity = np.matmul(_J_inv, p_velocity)
+                    k = time_step * c_velocity
+                    return k, p_velocity, c_velocity
+
+                x0 = self.interp.idx.cpoint
+                _J_inv = self.interp.J_inv
+                if x0 is None:
+                    return None, None, None
+
+                q_interp = Variables(self.interp)
+                q_interp.compute_velocity()
+                p_velocity = q_interp.velocity.reshape(3)
+                c_velocity = np.matmul(_J_inv, p_velocity)
+                k0 = time_step * c_velocity
+                x1 = x0 + k0
+
+                k1, pv1, cv1 = _rk2_step(self, x1)
+                if k1 is None:
+                    return None, None, None
+
+                x_new = x0 + 1/2 * (k0 + k1)
+                _, pv_new, cv_new = _rk2_step(self, x_new)
+
+                self.cpoint = x_new
+
+                return self.cpoint, pv_new, cv_new
+
+            case 'pRK4':
+                """
+                This is a straight forward RK4 integration. Search for the point,
+                Interpolate the data to the point, Compute required variables,
+                Perform RK4 integration!
+                """
+
+                def _rk4_step(self, x):
+                    """
+
+                    Args:
+                        self:
+                        x: ndarray
+                            point in p-space
+
+                    Returns:
+                        k: ndarray
+                            interim RK4 variables
+
+                    """
+                    idx = Search(self.interp.idx.grid, x)
+                    idx.compute(method='p-space')
+                    # For p-space algos; the point-in-domain check was done in search
+                    if idx.ppoint is None: return None, None
+                    interp = Interpolation(self.interp.flow, idx)
+                    interp.adaptive = self.interp.adaptive
+                    interp.rbf_kernel = self.interp.rbf_kernel
+                    interp.compute(method=self.interp.method)
+                    q_interp = Variables(interp)
+                    q_interp.compute_velocity()
+                    u = q_interp.velocity.reshape(3)
+                    k = time_step * u
+                    return u, k
+
+                # Start RK4 for p-space
+                # For p-space algos; the point-in-domain check was done in search
+                x0 = self.interp.idx.ppoint
+                if x0 is None: return None, None
+                q_interp = Variables(self.interp)
+                q_interp.compute_velocity()
+                u0 = q_interp.velocity.reshape(3)
+                k0 = time_step * u0
+                x1 = x0 + 0.5 * k0
+
+                u1, k1 = _rk4_step(self, x1)
+                if k1 is None: return None, None
+                x2 = x0 + 0.5 * k1
+
+                u2, k2 = _rk4_step(self, x2)
+                if k2 is None: return None, None
+                x3 = x0 + k2
+
+                u3, k3 = _rk4_step(self, x3)
+                if k3 is None: return None, None
+                x_new = x0 + 1/6 * (k0 + 2*k1 + 2*k2 + k3)
+                u_new, _ = _rk4_step(self, x_new)
+
+                self.ppoint = x_new
+
+                return self.ppoint, u_new
+
+            case 'cRK4':
+                '''
+                This is a block-wise integration. Everytime the point gets out
+                a pRK4 is run to find the new block the point is located in.
+                That particular step is done in streamlines algorithm.
+                
+                All the points, x0, x1... are in c-space
+                
+                Point location is known in c-space, avoiding search.
+                Interpolates data to the point
+                RK4 integration is performed!
+                '''
+
+                def _rk4_step(self, x):
+                    """
+
+                    Args:
+                        self:
+                        x: ndarray
+                            point in c-space
+
+                    Returns:
+                        k: ndarray
+                            interim RK4 variables
+
+                    """
+                    idx = Search(self.interp.idx.grid, x)
+                    idx.block = self.interp.idx.block
+                    idx.c2p(x)  # This will change the cell attribute
+                    # In-domain check is done in search
+                    if idx.cpoint is None:
+                        self.cpoint = None
+                        self.ppoint = None
+                        return None, None, None
+                    interp = Interpolation(self.interp.flow, idx)
+                    interp.adaptive = self.interp.adaptive
+                    interp.rbf_kernel = self.interp.rbf_kernel
+                    interp.compute(method=self.interp.method)
+                    _J_inv = interp.J_inv
+                    q_interp = Variables(interp)
+                    q_interp.compute_velocity()
+                    p_velocity = q_interp.velocity.reshape(3)
+                    c_velocity = np.matmul(_J_inv, p_velocity)
+                    k = time_step * c_velocity
+                    return k, p_velocity, c_velocity
+
+                x0 = self.interp.idx.cpoint
+                _J_inv = self.interp.J_inv
+                if x0 is None:
+                    return None, None, None
+
+                q_interp = Variables(self.interp)
+                q_interp.compute_velocity()
+                p_velocity = q_interp.velocity.reshape(3)
+                c_velocity = np.matmul(_J_inv, p_velocity)
+                k0 = time_step * c_velocity
+                x1 = x0 + 0.5 * k0
+
+                k1, pv1, cv1 = _rk4_step(self, x1)
+                if k1 is None:
+                    return None, None, None
+                x2 = x0 + 0.5 * k1
+
+                k2, pv2, cv2 = _rk4_step(self, x2)
+                if k2 is None:
+                    return None, None, None
+                x3 = x0 + k2
+
+                k3, pv3, cv3 = _rk4_step(self, x3)
+                if k3 is None:
+                    return None, None, None
+                x_new = x0 + 1/6 * (k0 + 2*k1 + 2*k2 + k3)
+                _, pv_new, cv_new = _rk4_step(self, x_new)
+
+                self.cpoint = x_new
+
+                return self.cpoint, pv_new, cv_new
+
+    def compute_ppath(self, diameter=1e-6, density=1000, velocity=None,
+                      method='pRK4', time_step=1e-4, drag_model='stokes'):
+
+        def _drag_constant(_re, _q_interp=None, _mach=None, _mu=None, _model=drag_model):
+            """
+            Coefficient of drag for a spherical particle
+
+            Args:
+                _re : Relative Reynolds Number
+                _mach : Relative Mach Number
+                _model : Drag Model Name
+                    Available models are 'sphere', 'stokes', 'oseen', 'schiller_nauman',
+                    'cunningham'
+
+            Returns:
+                coefficient of drag based on local flow/particle properties
+
+            """
+            _gamma = q_interp.gamma
+            match _model:
+                case 'zero-drag':
+                    # zero drag model to simulate fluid
+                    return 0
+
+                case 'sphere':
+                    # ref: Fluid Mechanics, Frank M. White
+                    # This was decided by trail-and-error from VISUAL3 code
+                    if _re <= 1e-9:
+                        return 0
+                    if _re < 1e-3:
+                        return 24 / _re
+                    if 1e-3 <= _re < 0.45:
+                        return 24 / _re * (1 + 3 * _re / 16)
+                    if 0.45 <= _re < 1:
+                        # Same as above due to lack of data
+                        return 24 / _re * (1 + 3 * _re / 16)
+                    if 1 <= _re < 800:
+                        return 24 / _re * (1 + _re ** (2 / 3) / 6)
+                    if 800 <= _re < 3e5:
+                        return 0.44
+                    if 3e5 <= _re < 4e5:
+                        # Same as above due to lack of data
+                        return 0.44
+                    if _re >= 4e5:
+                        return 0.07
+
+                case 'stokes':
+                    # Stokes Drag; for creeping flow regime; Re << 1
+                    if _re <= 1e-9:
+                        return 0
+                    else:
+                        return 24/_re
+
+                case 'melling':
+                    # The popular melling correction
+                    if _re <= 1e-9:
+                        return 0
+                    else:
+                        knd = _mach / _re * np.sqrt(np.pi*_gamma/2)
+                        return 24/_re * (1 + knd)**-1
+
+                case 'melling-2':
+                    # The popular melling correction
+                    if _re <= 1e-9:
+                        return 0
+                    else:
+                        knd = _mach / _re * np.sqrt(np.pi*_gamma/2)
+                        return 24/_re * (1 + 2.7*knd)**-1
+
+                case 'oseen':
+                    # Oseen's model; for creeping flow regime; Re < 1
+                    if _re <= 1e-9:
+                        return 0
+                    else:
+                        return 24/_re * (1 + 3/16 * _re)
+
+                case 'schiller-nauman':
+                    # Schiller and Nauman's model; for Re <~ 200 & M <~ 0.25
+                    if _re <= 1e-9:
+                        return 0
+                    else:
+                        return 24/_re * (1 + 0.15 * _re**0.687)
+
+                case 'cunningham':
+                    # Cunningham model; for Re << 1; M << 1; Kn <~ 0.1
+                    # Knudsen number
+                    # _r = _q_interp.density * _q_interp.velocity_magnitude * diameter / _mu
+                    if _re <= 1e-9:
+                        return 0
+                    if _re <= 1:
+                        _kn = _mach / _re * np.sqrt(_q_interp.gamma * np.pi/2)
+                        return 24/_re * (1 + 4.5*_kn)**-1
+                    if _re > 1:
+                        _kn = _mach / np.sqrt(_re)
+                        return 24/_re * (1 + 4.5*_kn)**-1
+
+                case 'henderson':
+                    # Henderson model; for all flow regimes
+                    # Simplified by ignoring sphere temperature
+                    if _re < 1e-9:
+                        return 0
+
+                    # For Mach < 1
+                    _s = _mach * np.sqrt(_gamma/2)
+                    _f1 = 24 * (_re + _s * (5.89688 * np.exp(-0.247 * _re/_s)))**-1
+                    _f2 = np.exp(-0.5*_mach/np.sqrt(_re)) * \
+                                ((4.5 + 0.38*(0.03*_re + 0.48*np.sqrt(_re))) / (1 + 0.03*_re + 0.48*np.sqrt(_re)) +
+                                 0.1*_mach**2 + 0.2*_mach**8)
+                    _f3 = (1 - np.exp(-_mach/_re))*0.6*_s
+                    _cd1 = _f1 + _f2 + _f3
+                    if _mach < 1:
+                        return _cd1
+
+                    # For Mach >= 1.75
+                    _mach_inf = _mach
+                    _re_inf = _re
+                    _s_inf = _mach_inf * np.sqrt(_gamma/2)
+                    _g1 = 0.9 + 0.34/_mach_inf**2
+                    _g2 = 1.86 * np.sqrt(_mach_inf/_re_inf) * (2 + 2/_s_inf**2 + 1.058/_s_inf - 1/_s_inf**4)
+                    _g3 = 1 + 1.86 * np.sqrt(_mach_inf/_re_inf)
+                    _cd2 = (_g1 + _g2) / _g3
+                    if _mach >= 1.75:
+                        return _cd2
+
+                    # For 1 <= Mach < 1.75; linear interpolation
+                    if 1 <= _mach < 1.75:
+                        return _cd1 + 4/3 * (_mach_inf - 1) * (_cd2 - _cd1)
+
+                case 'subramaniam-balachandar':
+                    # Model from their new book
+                    if _re < 1e-9:
+                        return 0
+
+                    if _re < 0.5:
+                        # Stokes
+                        return 24/_re
+
+                    if _re < 20:
+                        # Clift
+                        return 24/_re * (1 + 0.1315 * _re**(0.82-0.05*np.log10(_re)))
+
+                    if _re < 800:
+                        # Schiller-Naumann
+                        return 24/_re * (1 + 0.15 * _re**0.687)
+
+                    if _re < 3e5:
+                        # Clift-Gauvin
+                        return 24/_re * (1 + 0.15 * _re**0.687 + 0.42/24 * _re * (1 + 4.25e4 * _re**(-1.16))**-1)
+
+                case 'loth':
+                    # Loth's model; for all flow regimes
+                    if _re < 1e-9:
+                        return 0
+
+                    if _re < 45:
+                    # Rarefraction dominated domain
+                        import math
+                        _s = _mach * np.sqrt(_gamma/2)
+                        _cd_fm = (1 + 2 * _s**2) * np.exp(-_s**2) / (_s**3 * np.pi**0.5) + \
+                                 (4*_s**4 + 4*_s**2 - 1) * math.erf(_s) / (2*_s**4) + 2 * np.pi**0.5 / (3 * _s)
+                        _cd_fm_re = _cd_fm / (1 + (_cd_fm/1.63 - 1) * (_re/45)**0.5)
+                        _kn = (np.pi * _gamma / 2)**0.5 * _mach / _re
+                        _f_kn = (1 + _kn * (2.514 + 0.8 * np.exp(-0.55/_kn)))**-1
+                        _cd_kn_re = 24/_re * (1 + 0.15 * _re**0.687) * _f_kn
+                        _cd = (_cd_kn_re + _mach**4 * _cd_fm_re) / (1 + _mach**4)
+                        return _cd
+
+                    if _re == 45:
+                        return 1.63
+
+                    if _re > 45:
+                    # compression-dominated regime
+                        if _mach <= 1.45:
+                            _cm = 5/3 + 2/3 * np.tanh(3 * np.log(_mach + 0.1))
+                        if _mach > 1.45:
+                            _cm = 2.044 + 0.2 * np.exp(-1.8 * (np.log(_mach/1.5))**2)
+                        if _mach <= 0.89:
+                            _gm = 1 - 1.525 * _mach**4
+                        if _mach > 0.89:
+                            _gm = 2e-4 + 8e-4 * np.tanh(12.77 * (_mach - 2.02))
+                        _hm = 1 - 0.258 * _cm / (1 + 514 * _gm)
+                        _cd = 24/_re * (1 + 0.15 * _re**0.687) * _hm + 0.42 * _cm / (1 + 42000 * _gm / _re**1.16)
+                        return _cd
+
+                case 'tedeschi':
+                    # Tedeschi's model; for all flow regimes
+                    if _re < 1e-9:
+                        return 0
+                    if _re <= 1:
+                        _kn = _mach / _re * np.sqrt(_q_interp.gamma * np.pi/2)
+                    else:
+                        _kn = _mach / np.sqrt(_re)
+
+                    s = _mach * np.sqrt(_gamma/2)
+
+                    def _solve_k(_k):
+                        s_prime = (1 - _k) * s
+                        epsilon_prime = 3/8 * (np.pi**2 / s_prime) * (1 + s_prime**2) * s_prime + np.exp(-s_prime**2) /4
+                        a1 = 9/4 * 0.15 * 2 * _kn / epsilon_prime * (s * np.pi**0.5 / _kn)**0.687
+                        a2 = 1 + 9/4 * 2 * _kn / epsilon_prime
+                        return a1 * _k**1.687 + a2 * _k - 1
+
+                    # solve the equation
+                    k = fsolve(_solve_k, np.array([0.5]))
+
+                    c = 1 + _re**2 / (_re**2 + 100) * np.e**(-0.225/_mach**2.5)
+                    _epsilon_kn = 1.177 + 0.177 * (0.851 * _kn**1.16 - 1) / (0.851 * _kn**1.16 + 1)
+
+                    return 24/_re * k * (1 + 0.15 * (k*_re)**0.687) * c * _epsilon_kn
+
+        def _viscosity(_temperature, law='keyes'):
+            """
+            Viscosity of air as a function of temperature
+            Args:
+                _temperature: in Kelvin provided by default in the integration class
+                law: 'sutherland' or 'keyes' -- defaults to 'keyes'
+
+            Returns:
+                _mu: viscosity of air in kg/m-s
+
+            """
+            match law:
+                case 'sutherland':
+                    # Sutherland's viscosity law
+                    # All temperatures must be in kelvin
+                    # Formula from cfd-online
+                    _c1 = 1.716e-5 * (273.15 + 110.4) / 273.15**1.5
+                    _mu = _c1 * _temperature**1.5 * 0.4 / (_temperature + 110.4)
+                case 'keyes':
+                    # New formula from keyes et al.
+                    a0, a, a1 = 1.488, 122.1, 5.0
+                    _tau = 1/_temperature
+                    _mu = a0 * _temperature**0.5 * 10**-6 / (1 + a * _tau / 10 ** (a1 * _tau))
+            return _mu
+
+        match method:
+            case 'pRK4':
+
+                def _rk4_step(self, vp, x):
+                    """
+
+                    Args:
+                        self:
+
+                    Returns:
+                        k: ndarray
+                            interim RK4 variables
+
+                    """
+                    idx = Search(self.interp.idx.grid, x)
+                    idx.compute(method='p-space')
+                    # For p-space algos; the point-in-domain check was done in search
+                    if idx.ppoint is None:
+                        return None, None, None
+                    interp = Interpolation(self.interp.flow, idx)
+                    interp.adaptive = self.interp.adaptive
+                    interp.rbf_kernel = self.interp.rbf_kernel
+                    interp.compute(method=self.interp.method)
+                    q_interp = Variables(interp)
+                    # Compute all variables
+                    q_interp.compute_mach()
+                    uf = q_interp.velocity.reshape(-1)
+                    # particle dynamics
+                    _rhof = q_interp.density.reshape(-1)
+                    dp = diameter
+                    rhop = density
+                    mu = _viscosity(q_interp.temperature.reshape(-1))
+                    # Relative Reynolds Number
+                    re = _rhof * np.linalg.norm(vp - uf) * dp / mu
+                    _mach = np.linalg.norm(vp - uf) * q_interp.mach.reshape(-1) /\
+                            q_interp.velocity_magnitude.reshape(-1)
+                    _cd = _drag_constant(re, _q_interp=q_interp, _mach=_mach, _mu=mu, _model=drag_model)
+                    _k = -0.75 * _rhof / (rhop * dp)
+                    try:
+                        _vk = _cd * _k * (vp - uf) * np.linalg.norm(vp - uf) * time_step
+                    except TypeError:
+                        return None, None, None
+                    return _vk, uf, None
+
+                # Start RK4 for p-space
+                # For p-space algos; the point-in-domain check was done in search
+                x0 = self.interp.idx.ppoint
+                if x0 is None:
+                    return None, None, None
+                q_interp = Variables(self.interp)
+                q_interp.compute_velocity()
+                u0 = q_interp.velocity.reshape(3)
+                # Assign velocity to start Rk4 step
+                if velocity is None:
+                    v0 = u0.copy()
+                else:
+                    v0 = velocity.copy()
+                vk0, uf0, temp = _rk4_step(self, v0, x0)
+                xk0 = v0 * time_step
+                # Assign fluid velocity when vk is zero
+                # Theory: When zero drag particle is massless, hence fluid velocity
+                if np.linalg.norm(vk0) == 0:
+                    v0 = uf0.copy()
+                v1 = v0 + 0.5 * vk0
+                x1 = x0 + 0.5 * xk0
+
+                vk1, uf1, temp = _rk4_step(self, v1, x1)
+                xk1 = v1 * time_step
+                if vk1 is None:
+                    return None, None, None
+                if np.linalg.norm(vk1) == 0:
+                    v0 = uf1.copy()
+                v2 = v0 + 0.5 * vk1
+                x2 = x0 + 0.5 * xk1
+                # Check for mid-RK4 blow-up issue. Happens when Cd and time-step are high
+                if np.linalg.norm(x2 - x0) >= 10 * np.linalg.norm(x1-x0) and np.linalg.norm(x2 - x0) >= 1e-12:
+                    self.rk4_bool = True
+                    return x0, v0, u0
+
+                vk2, uf2, temp = _rk4_step(self, v2, x2)
+                xk2 = v2 * time_step
+                if vk2 is None:
+                    return None, None, None
+                if np.linalg.norm(vk2) == 0:
+                    v0 = uf2.copy()
+                v3 = v0 + vk2
+                x3 = x0 + xk2
+                # Check for mid-RK4 blow-up issue. Happens when Cd and time-step are high
+                if np.linalg.norm(x3 - x0) >= 10 * np.linalg.norm(x1 - x0) and np.linalg.norm(x3 - x0) >= 1e-12:
+                    self.rk4_bool = True
+                    return x0, v0, u0
+
+                vk3, uf3, temp = _rk4_step(self, v3, x3)
+                xk3 = v3 * time_step
+                if vk3 is None:
+                    return None, None, None
+                if np.linalg.norm(vk3) == 0:
+                    v0 = uf3.copy()
+                v_new = v0 + 1 / 6 * (vk0 + 2 * vk1 + 2 * vk2 + vk3)
+                x_new = x0 + 1 / 6 * (xk0 + 2 * xk1 + 2 * xk2 + xk3)
+                # Check for mid-RK4 blow-up issue. Happens when Cd and time-step are high
+                if np.linalg.norm(x_new - x0) >= 10 * np.linalg.norm(x1 - x0) and np.linalg.norm(x_new - x0) >= 1e-12:
+                    self.rk4_bool = True
+                    return x0, v0, u0
+
+                vk_new, uf_new, temp = _rk4_step(self, v_new, x_new)
+                # make sure the velocity is going down in a compression case
+                # This is done to remove the oscillations in the post-shock region
+                if vk_new is None:
+                    return None, None, None
+                if self.interp.method == 'simple_oblique_shock' and np.dot(v_new - v0, uf_new - v_new) < 0:
+                    self.rk4_bool = True
+                    return x0, v0, u0
+
+                self.ppoint = x_new
+
+                return x_new, v_new, uf_new
+
+            case 'cRK4':
+
+                def _rk4_step(self, c_vp, x):
+                    """
+                    Returns required data for the RK4 step
+
+                    Args:
+                        self:
+                        c_vp: ndarray
+                            particle velocity in c-space
+                        x: ndarray
+                            point in c-space
+
+                    Returns:
+                        k: ndarray
+                            interim RK4 variables
+
+                    """
+                    if np.any(x < 0):
+                        return None, None, None, None
+                    idx = Search(self.interp.idx.grid, x)
+                    idx.block = self.interp.idx.block
+                    idx.c2p(x)  # This will change the cell attribute
+                    # In-domain check is done in search
+                    if idx.cpoint is None:
+                        self.cpoint = None
+                        self.ppoint = None
+                        return None, None, None, None
+                    interp = Interpolation(self.interp.flow, idx)
+                    interp.adaptive = self.interp.adaptive
+                    interp.rbf_kernel = self.interp.rbf_kernel
+                    interp.compute(method=self.interp.method)
+                    _J_inv = interp.J_inv
+                    _J = interp.J
+                    q_interp = Variables(interp)
+                    # Computing mach get all the necessary variables
+                    q_interp.compute_mach()
+                    p_uf = q_interp.velocity.reshape(-1)
+                    c_uf = np.matmul(_J_inv, p_uf)
+                    # particle dynamics
+                    _rhof = q_interp.density.reshape(-1)
+                    dp = diameter
+                    rhop = density
+                    # Transform particle velocity to p-space
+                    p_vp = np.matmul(_J, c_vp)
+                    mu = _viscosity(q_interp.temperature.reshape(-1))
+                    # Relative Reynolds Number
+                    re = _rhof * np.linalg.norm(p_vp - p_uf) * dp / mu
+                    _mach = np.linalg.norm(p_vp - p_uf) * q_interp.mach.reshape(-1) /\
+                            q_interp.velocity_magnitude.reshape(-1)
+                    _cd = _drag_constant(re, _q_interp=q_interp, _mach=_mach, _mu=mu, _model=drag_model)
+                    _k = -0.75 * _rhof / (rhop * dp)
+                    p_vk = _cd * _k * (p_vp - p_uf) * np.linalg.norm(p_vp - p_uf) * time_step
+                    c_vk = np.matmul(_J_inv, p_vk)
+                    return c_vk, p_uf, c_uf, p_vp
+
+                # Start RK4 for c-space
+                x0 = self.interp.idx.cpoint
+                if x0 is None:
+                    return None, None, None
+                q_interp = Variables(self.interp)
+                q_interp.compute_velocity()
+                p_u0 = q_interp.velocity.reshape(-1)
+                c_u0 = np.matmul(self.interp.J_inv, p_u0)
+                # Assign velocity to start Rk4 step
+                if velocity is None:
+                    c_v0 = c_u0.copy()
+                else:
+                    c_v0 = np.matmul(self.interp.J_inv, velocity)
+                vk0, p_u0, c_u0, p_v0 = _rk4_step(self, c_v0, x0)
+                # Assign fluid velocity when vk is zero
+                # Theory: When zero drag particle is massless, hence fluid velocity
+                if np.linalg.norm(vk0) == 0:
+                    c_v0 = c_u0.copy()
+                c_v1 = c_v0 + 0.5 * vk0
+                xk0 = c_v0 * time_step
+                x1 = x0 + 0.5 * xk0
+
+                # Integration starts
+                vk1, p_u1, c_u1, p_v1 = _rk4_step(self, c_v1, x1)
+                # if the residual is none return; exited the domain
+                if vk1 is None:
+                    return None, None, None
+                # if zero; particle is acting like massless particle; low relative reynolds number cases
+                if np.linalg.norm(vk1) == 0:
+                    c_v0 = c_u1.copy()
+                c_v2 = c_v0 + 0.5 * vk1
+                xk1 = c_v1 * time_step
+                x2 = x0 + 0.5 * xk1
+                # Check for mid-RK4 blow up due to residuals
+                if np.linalg.norm(x2 - x0) >= 10 * np.linalg.norm(x1-x0):
+                    self.rk4_bool = True
+                    return x0, p_v0, p_u0
+
+                # Repeat three more times; RK4
+                vk2, p_u2, c_u2, p_v2 = _rk4_step(self, c_v2, x2)
+                if vk2 is None:
+                    return None, None, None
+                if np.linalg.norm(vk2) == 0:
+                    c_v0 = c_u2.copy()
+                c_v3 = c_v0 + vk2
+                xk2 = c_v2 * time_step
+                x3 = x0 + xk2
+                if np.linalg.norm(x3 - x0) >= 10 * np.linalg.norm(x1-x0):
+                    self.rk4_bool = True
+                    return x0, p_v0, p_u0
+
+                vk3, p_u3, c_u3, p_v3 = _rk4_step(self, c_v3, x3)
+                if vk3 is None:
+                    return None, None, None
+                if np.linalg.norm(vk3) == 0:
+                    c_v0 = c_u3.copy()
+                c_v_new = c_v0 + 1 / 6 * (vk0 + 2 * vk1 + 2 * vk2 + vk3)
+                xk3 = c_v3 * time_step
+                x_new = x0 + 1 / 6 * (xk0 + 2 * xk1 + 2 * xk2 + xk3)
+                if np.linalg.norm(x_new - x0) >= 10 * np.linalg.norm(x1-x0):
+                    self.rk4_bool = True
+                    return x0, p_v0, p_u0
+
+                _, p_u_new, c_u_new, p_v_new = _rk4_step(self, c_v_new, x_new)
+
+                self.cpoint = x_new
+
+                return x_new, p_u_new, p_v_new
```

### Comparing `project-arrakis-0.1/src/streamlines/search.py` & `project_arrakis-0.1.1/src/streamlines/search.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,357 +1,363 @@
-# This file searches for the cell in which the given point is present in the grid
-
-import numpy as np
-
-
-# noinspection SpellCheckingInspection
-class Search:
-    """Module to search for the cell in which the given point is present
-
-    ...
-
-    Attributes
-    ----------
-    Input :
-        grid : src.io.plot3dio.GridIO
-            Grid object created from GridIO
-        ppoint: list
-            A float list of shape 3 -- Representing x, y, z of a point
-    Output :
-        cpoint: numpy.ndarray
-            ppoint location in c-space. Will be computed if calculating in c-space
-        index: numpy.ndarray
-            Indices of closest node to the given point
-        cell: numpy.ndarray
-            Indices of the cell in which the given point is present
-        info: str
-            Information about the point location
-
-    Methods
-    -------
-    compute()
-        Finds the location of given point in the grid using the given search-method
-        search-methods:
-            distance, block-distance, p-space, c-space
-
-    p2c()
-        Method to convert location of point in physical space to computational space
-        Rarely used
-
-    c2p()
-        Method to convert from c-space to p-space
-        Used in integration algorithms to get new cell
-
-    author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
-    date: 10-24/2021
-        """
-
-    def __init__(self, grid, ppoint):
-        self.grid = grid
-        self.ppoint = ppoint
-        self.cpoint = None
-        self.index = None
-        self.cell = None
-        self.info = None
-        self.block = None
-
-    def __str__(self):
-        doc = "This instance takes in the grid of shape " + self.grid.grd.shape + \
-              "\nand the searches for the point " + self.ppoint + " in the grid.\n" \
-              "Use method 'compute' to find (attributes) the closest 'index' and the nodes of the 'cell'.\n"
-        return doc
-
-    @staticmethod
-    def _cell_nodes(_i, _j, _k):
-        # _Internal method to get the nodes of a cell
-        _cell = np.array([[_i, _j, _k],
-                          [_i + 1, _j, _k],
-                          [_i + 1, _j + 1, _k],
-                          [_i, _j + 1, _k],
-                          [_i, _j, _k + 1],
-                          [_i + 1, _j, _k + 1],
-                          [_i + 1, _j + 1, _k + 1],
-                          [_i, _j + 1, _k + 1]], dtype=int)
-        return _cell
-
-    @staticmethod
-    def _cell_index(self, i, j, k):
-        # _Internal method to obtain the nodes of the cell in which the given point is present
-
-        # Transform to found node to find the location of point
-        # Basically looking at which quadrant the point is located
-        # to find the nodes of the respective cell
-        _node = self.grid.grd[i, j, k, :, self.block]
-        _point_transform = self.ppoint - _node
-
-        # Check if point is a node in the domain
-        if np.all(abs(_point_transform) <= 1e-6):
-            self.cell = self._cell_nodes(i, j, k)
-            self.info = 'Given point is a node in the domain with a tol of 1e-6.\n' \
-                        'Interpolation will assign node properties for integration.\n' \
-                        'Index of the node will be returned by cell attribute\n'
-            # print(self.info)
-            return
-
-        # ON BOUNDARY FOR A GENERALIZED HEXA IS SAME AS DEFAULT SEARCH
-        # Removed the code for on the boundary case
-        # Start the main cell nodes code
-        if np.all(_point_transform >= 1e-6):
-            self.cell = self._cell_nodes(i, j, k)
-            return
-        if _point_transform[0] <= 1e-6 and _point_transform[1] >= 1e-6 and _point_transform[2] >= 1e-6:
-            self.cell = self._cell_nodes(i - 1, j, k)
-            return
-        if _point_transform[0] <= 1e-6 and _point_transform[1] <= 1e-6 and _point_transform[2] >= 1e-6:
-            self.cell = self._cell_nodes(i - 1, j - 1, k)
-            return
-        if _point_transform[0] >= 1e-6 and _point_transform[1] <= 1e-6 and _point_transform[2] >= 1e-6:
-            self.cell = self._cell_nodes(i, j - 1, k)
-            return
-        if _point_transform[0] >= 1e-6 and _point_transform[1] >= 1e-6 and _point_transform[2] <= 1e-6:
-            self.cell = self._cell_nodes(i, j, k - 1)
-            return
-        if _point_transform[0] <= 1e-6 and _point_transform[1] >= 1e-6 and _point_transform[2] <= 1e-6:
-            self.cell = self._cell_nodes(i - 1, j, k - 1)
-            return
-        if np.all(_point_transform <= 1e-6):
-            self.cell = self._cell_nodes(i - 1, j - 1, k - 1)
-            return
-        if _point_transform[0] >= 1e-6 and _point_transform[1] <= 1e-6 and _point_transform[2] <= 1e-6:
-            self.cell = self._cell_nodes(i, j - 1, k - 1)
-            return
-
-        return
-
-    @staticmethod
-    def _find_block(self):
-        # _Internal method to find the block
-        # Setup to compute block number in which the point is present
-        _bool_min = self.grid.grd_min <= self.ppoint
-        _bool_max = self.grid.grd_max >= self.ppoint
-        _bool = _bool_max == _bool_min
-
-        # Test if the given point is in domain or not
-        if np.all(_bool.all(axis=1) == False) or np.all(_bool_min == False) or np.all(_bool_max == False):
-            self.info = 'Given point is not in the domain. The cell attribute will return "None" in search algorithm\n'
-            self.cell = None
-            self.ppoint = None
-            self.cpoint = None
-            self.block = None
-            # print(self.info)
-            return
-        # Assign the block number to the attribute
-        self.block = int(np.where(_bool.all(axis=1))[0][0])
-
-        return self.block
-
-    def compute(self, method='block_distance'):
-        """
-        Use the method to compute index and cell attributes
-
-        parameter:
-            method: str
-                Currently distance or block_distance
-
-        return:
-        None
-
-        author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
-        date: 10-24/2021
-        """
-
-        # Find the block number
-        self.block = self._find_block(self)
-        # To check for point out-of-domain case
-        if self.block is None:
-            return
-
-        match method:
-
-            case 'distance':
-                # Compute the distance from all nodes in the grid
-                _dist = np.sqrt((self.grid.grd[..., 0, :] - self.ppoint[0]) ** 2 +
-                                (self.grid.grd[..., 1, :] - self.ppoint[1]) ** 2 +
-                                (self.grid.grd[..., 2, :] - self.ppoint[2]) ** 2)
-
-                # Find the closest node to the point --> index.ndim = 4
-                self.index = np.array(np.unravel_index(_dist.argmin(), _dist.shape))
-                i, j, k, self.block = self.index[0], self.index[1], self.index[2], self.index[3]
-                self._cell_index(self, i, j, k)
-                # Check for the end of the domain case
-                if max(self.cell[:, 0]) > self.grid.ni[self.block] - 1 or \
-                        max(self.cell[:, 1]) > self.grid.nj[self.block] - 1 or \
-                        max(self.cell[:, 2]) > self.grid.nk[self.block] - 1:
-                    self.cpoint = None
-                    self.ppoint = None
-                    return
-
-            case 'block_distance':
-                # Compute distance inside the block to get the nearest node
-                _i, _j, _k = self.grid.ni[self.block], self.grid.nj[self.block], self.grid.nk[self.block]
-                _dist = np.sqrt((self.grid.grd[:_i, :_j, :_k, 0, self.block] - self.ppoint[0]) ** 2 +
-                                (self.grid.grd[:_i, :_j, :_k, 1, self.block] - self.ppoint[1]) ** 2 +
-                                (self.grid.grd[:_i, :_j, :_k, 2, self.block] - self.ppoint[2]) ** 2)
-
-                # Other methods to calculate distance. The above method is faster
-                # _grd_min_point = self.grid.grd[:_i, :_j, :_k, :, self.block] - self.point
-                # _dist = np.linalg.norm(_grd_min_point, axis=-1)
-                # _dist = np.sqrt(np.einsum("ijkl,ijkl->ijk", _grd_min_point, _grd_min_point))
-
-                self.index = np.array(np.unravel_index(_dist.argmin(), _dist.shape))
-                i, j, k = self.index
-                self._cell_index(self, i, j, k)
-                # Check for the end of the domain case
-                if max(self.cell[:, 0]) > self.grid.ni[self.block] - 1 or \
-                        max(self.cell[:, 1]) > self.grid.nj[self.block] - 1 or \
-                        max(self.cell[:, 2]) > self.grid.nk[self.block] - 1 or np.any(self.cell < 0):
-                    print('Block search returned wrong cell! Point position lost.\n')
-                    self.cpoint = None
-                    self.ppoint = None
-                    return
-
-            case 'p-space':
-                # Search for given point using newton-raphson
-                # credit: Sadarjoen et al.
-                # title: Particle tracing algorithms for 3D Curvilinear grids
-                # This search is performed every single time to find the given point
-                self.cpoint = self.p2c(self.ppoint)
-
-            case 'c-space':
-                # To run c-space global point location is needed
-                # credit: Sadarjoen et al.
-                # title: Particle tracing algorithms for 3D Curvilinear grids
-
-                # Transform given point from p-space to c-space using newton-raphson
-                # This is only performed once to get the initial c-space point
-                self.cpoint = self.p2c(self.ppoint)
-
-    def c2p(self, _cpoint):
-        """
-        Method to convert c-space point to p-space
-        self.block is kept constant through the c-space algos
-        self.block is checked and switched in streamlines algo
-        This method is commonly used to test point location as well
-        in different algorithms
-
-        Args:
-            _cpoint: c-space co-ordinates
-
-        Returns:
-            _ppoint: p-space co-ordinates
-
-        """
-        self.cpoint = _cpoint
-        _eps0, _eps1, _eps2 = _cpoint.astype(int)
-        _alpha, _beta, _gamma = np.modf(_cpoint)[0]  # same as eps % 1.0
-
-        # Check if the given point is in the domain
-        if _eps0 >= self.grid.ni[self.block]-1 or _eps1 >= self.grid.nj[self.block]-1 or \
-                _eps2 >= self.grid.nk[self.block]-1:
-            self.cpoint = None
-            self.ppoint = None
-            return self.ppoint
-
-        # Determine in which cell the current point is present
-        self.cell = self._cell_nodes(_eps0, _eps1, _eps2)
-        _cell_grd = self.grid.grd[self.cell[:, 0], self.cell[:, 1], self.cell[:, 2], :, self.block]
-
-        # Calculate the location in p-space
-        self.ppoint = (1 - _alpha) * (1 - _beta) * (1 - _gamma) * _cell_grd[0] + \
-                _alpha  * (1 - _beta) * (1 - _gamma) * _cell_grd[1] + \
-                _alpha  *      _beta  * (1 - _gamma) * _cell_grd[2] + \
-                (1 - _alpha) *      _beta  * (1 - _gamma) * _cell_grd[3] + \
-                (1 - _alpha) * (1 - _beta) *      _gamma  * _cell_grd[4] + \
-                _alpha  * (1 - _beta) *      _gamma  * _cell_grd[5] + \
-                _alpha  *      _beta *       _gamma  * _cell_grd[6] + \
-                (1 - _alpha) *      _beta  *      _gamma  * _cell_grd[7]
-
-        return self.ppoint
-
-    def p2c(self, _ppoint):
-        """
-        Method to convert p-space point to c-space
-        As there is no direct analytical equation. We use Newton-Raphson
-        Args:
-            _ppoint: p-space co-ordinates
-
-        Returns:
-            eps: c-space co-ordinates
-        """
-        global _cpoint
-        self.ppoint = _ppoint
-
-        if self.block is None:
-            self.block = self._find_block(self)
-
-        # Start Newton-Raphson
-        _iter = 0
-        # Initial guess
-        try:
-            _cpoint is not None
-        except:
-            _cpoint = np.array([self.grid.ni[self.block], self.grid.nj[self.block], self.grid.nk[self.block]]) / 2 + \
-                np.random.randn(3)
-
-        while True:
-            # Check if taking too long
-            if _iter >= 1e3:
-                # print('Newton-Raphson did not converge. Try again!\n'
-                #       'Possible reason might be the point might be too close to the end of a domain')
-                self.ppoint, self.cpoint = None, None
-                return
-
-            # Check for out-of-domain case and reset the point to in-domain
-            _eps0, _eps1, _eps2 = _cpoint.astype(int)
-            _alpha, _beta, _gamma = np.modf(_cpoint)[0]
-            if _eps0 + 1 >= self.grid.ni[self.block]:
-                _cpoint[0] = self.grid.ni[self.block] - 1 - _alpha
-            if _eps1 + 1 >= self.grid.nj[self.block]:
-                _cpoint[1] = self.grid.nj[self.block] - 1 - _beta
-            if _eps2 + 1 >= self.grid.nk[self.block]:
-                _cpoint[2] = self.grid.nk[self.block] - 1 - _gamma
-
-            # Compute eps after the point is reset
-            _eps0, _eps1, _eps2 = _cpoint.astype(int)
-            self.cell = self._cell_nodes(_eps0, _eps1, _eps2)
-
-            # Calculate J_inv for the point --> Uses tri-linear interpolation
-            _cell_J_inv = self.grid.m2[self.cell[:, 0], self.cell[:, 1], self.cell[:, 2], :, :, self.block]
-            _J_inv = (1 - _alpha) * (1 - _beta) * (1 - _gamma) * _cell_J_inv[0] + \
-                     _alpha * (1 - _beta) * (1 - _gamma) * _cell_J_inv[1] + \
-                     _alpha * _beta * (1 - _gamma) * _cell_J_inv[2] + \
-                     (1 - _alpha) * _beta * (1 - _gamma) * _cell_J_inv[3] + \
-                     (1 - _alpha) * (1 - _beta) * _gamma * _cell_J_inv[4] + \
-                     _alpha * (1 - _beta) * _gamma * _cell_J_inv[5] + \
-                     _alpha * _beta * _gamma * _cell_J_inv[6] + \
-                     (1 - _alpha) * _beta * _gamma * _cell_J_inv[7]
-
-            # Transform from c to p-space
-            _pred_ppoint = self.c2p(_cpoint)
-
-            # Difference b/w predicted point to given point
-            _delta_ppoint = _ppoint - _pred_ppoint
-
-            # End newton-raphson if condition is met
-            if sum(abs(_delta_ppoint)) <= 1e-12:
-                _eps0, _eps1, _eps2 = _cpoint.astype(int)
-                self.cell = self._cell_nodes(_eps0, _eps1, _eps2)
-                self.cpoint = _cpoint
-                self.ppoint = _pred_ppoint
-                return _cpoint
-
-            # Transform from p to c-space
-            _delta_cpoint = np.matmul(_J_inv, _delta_ppoint)
-
-            # Save old point
-            _cpoint_old = _cpoint.copy()
-
-            # Update point
-            _cpoint += _delta_cpoint
-            # Update the point to zero if less than zero
-            _cpoint[_cpoint < 0] = 0
-            _cpoint = abs(_cpoint)
-            _iter += 1
-
-            pass
-
-
+# This file searches for the cell in which the given point is present in the grid
+
+import numpy as np
+
+
+# noinspection SpellCheckingInspection
+class Search:
+    """Module to search for the cell in which the given point is present
+
+    ...
+
+    Attributes
+    ----------
+    Input :
+        grid : src.io.plot3dio.GridIO
+            Grid object created from GridIO
+        ppoint: list
+            A float list of shape 3 -- Representing x, y, z of a point
+    Output :
+        cpoint: numpy.ndarray
+            ppoint location in c-space. Will be computed if calculating in c-space
+        index: numpy.ndarray
+            Indices of closest node to the given point
+        cell: numpy.ndarray
+            Indices of the cell in which the given point is present
+        info: str
+            Information about the point location
+
+    Methods
+    -------
+    compute()
+        Finds the location of given point in the grid using the given search-method
+        search-methods:
+            distance, block-distance, p-space, c-space
+
+    p2c()
+        Method to convert location of point in physical space to computational space
+        Rarely used
+
+    c2p()
+        Method to convert from c-space to p-space
+        Used in integration algorithms to get new cell
+
+    author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
+    date: 10-24/2021
+        """
+
+    def __init__(self, grid, ppoint):
+        self.grid = grid
+        self.ppoint = ppoint
+        self.cpoint = None
+        self.index = None
+        self.cell = None
+        self.info = None
+        self.block = None
+
+    def __str__(self):
+        doc = "This instance takes in the grid of shape " + self.grid.grd.shape + \
+              "\nand the searches for the point " + self.ppoint + " in the grid.\n" \
+              "Use method 'compute' to find (attributes) the closest 'index' and the nodes of the 'cell'.\n"
+        return doc
+
+    @staticmethod
+    def _cell_nodes(_i, _j, _k):
+        # _Internal method to get the nodes of a cell
+        _cell = np.array([[_i, _j, _k],
+                          [_i + 1, _j, _k],
+                          [_i + 1, _j + 1, _k],
+                          [_i, _j + 1, _k],
+                          [_i, _j, _k + 1],
+                          [_i + 1, _j, _k + 1],
+                          [_i + 1, _j + 1, _k + 1],
+                          [_i, _j + 1, _k + 1]], dtype=int)
+        return _cell
+
+    @staticmethod
+    def _cell_index(self, i, j, k):
+        # _Internal method to obtain the nodes of the cell in which the given point is present
+
+        # Transform to found node to find the location of point
+        # Basically looking at which quadrant the point is located
+        # to find the nodes of the respective cell
+        _node = self.grid.grd[i, j, k, :, self.block]
+        _point_transform = self.ppoint - _node
+
+        # Check if point is a node in the domain
+        if np.all(abs(_point_transform) <= 1e-12):
+            self.cell = self._cell_nodes(i, j, k)
+            self.info = 'Given point is a node in the domain with a tol of 1e-12.\n' \
+                        'Interpolation will assign node properties for integration.\n' \
+                        'Index of the node will be returned by cell attribute\n'
+            # print(self.info)
+            return
+
+        # ON BOUNDARY FOR A GENERALIZED HEXA IS SAME AS DEFAULT SEARCH
+        # Removed the code for on the boundary case
+        # Start the main cell nodes code
+        if np.all(_point_transform >= 1e-6):
+            self.cell = self._cell_nodes(i, j, k)
+            return
+        if _point_transform[0] <= 1e-6 and _point_transform[1] >= 1e-6 and _point_transform[2] >= 1e-6:
+            self.cell = self._cell_nodes(i - 1, j, k)
+            return
+        if _point_transform[0] <= 1e-6 and _point_transform[1] <= 1e-6 and _point_transform[2] >= 1e-6:
+            self.cell = self._cell_nodes(i - 1, j - 1, k)
+            return
+        if _point_transform[0] >= 1e-6 and _point_transform[1] <= 1e-6 and _point_transform[2] >= 1e-6:
+            self.cell = self._cell_nodes(i, j - 1, k)
+            return
+        if _point_transform[0] >= 1e-6 and _point_transform[1] >= 1e-6 and _point_transform[2] <= 1e-6:
+            self.cell = self._cell_nodes(i, j, k - 1)
+            return
+        if _point_transform[0] <= 1e-6 and _point_transform[1] >= 1e-6 and _point_transform[2] <= 1e-6:
+            self.cell = self._cell_nodes(i - 1, j, k - 1)
+            return
+        if np.all(_point_transform <= 1e-6):
+            self.cell = self._cell_nodes(i - 1, j - 1, k - 1)
+            return
+        if _point_transform[0] >= 1e-6 and _point_transform[1] <= 1e-6 and _point_transform[2] <= 1e-6:
+            self.cell = self._cell_nodes(i, j - 1, k - 1)
+            return
+
+        return
+
+    @staticmethod
+    def _find_block(self):
+        # _Internal method to find the block
+        # Setup to compute block number in which the point is present
+        _bool_min = self.grid.grd_min <= self.ppoint
+        _bool_max = self.grid.grd_max >= self.ppoint
+        _bool = _bool_max == _bool_min
+
+        # Test if the given point is in domain or not
+        if np.all(_bool.all(axis=1) == False) or np.all(_bool_min == False) or np.all(_bool_max == False):
+            self.info = 'Given point is not in the domain. The cell attribute will return "None" in search algorithm\n'
+            self.cell = None
+            self.ppoint = None
+            self.cpoint = None
+            self.block = None
+            # print(self.info)
+            return
+        # Assign the block number to the attribute
+        self.block = int(np.where(_bool.all(axis=1))[0][0])
+
+        return self.block
+
+    def compute(self, method='block_distance'):
+        """
+        Use the method to compute index and cell attributes
+
+        parameter:
+            method: str
+                Currently distance or block_distance
+
+        return:
+        None
+
+        author: Dilip Kalagotla @ kal ~ dilip.kalagotla@gmail.com
+        date: 10-24/2021
+        """
+
+        # Find the block number
+        self.block = self._find_block(self)
+        # To check for point out-of-domain case
+        if self.block is None:
+            return
+
+        match method:
+
+            case 'distance':
+                # Compute the distance from all nodes in the grid
+                _dist = np.sqrt((self.grid.grd[..., 0, :] - self.ppoint[0]) ** 2 +
+                                (self.grid.grd[..., 1, :] - self.ppoint[1]) ** 2 +
+                                (self.grid.grd[..., 2, :] - self.ppoint[2]) ** 2)
+
+                # Find the closest node to the point --> index.ndim = 4
+                self.index = np.array(np.unravel_index(_dist.argmin(), _dist.shape))
+                i, j, k, self.block = self.index[0], self.index[1], self.index[2], self.index[3]
+                self._cell_index(self, i, j, k)
+                # Check for the end of the domain case
+                if max(self.cell[:, 0]) > self.grid.ni[self.block] - 1 or \
+                        max(self.cell[:, 1]) > self.grid.nj[self.block] - 1 or \
+                        max(self.cell[:, 2]) > self.grid.nk[self.block] - 1:
+                    self.cpoint = None
+                    self.ppoint = None
+                    return
+
+            case 'block_distance':
+                # Compute distance inside the block to get the nearest node
+                _i, _j, _k = self.grid.ni[self.block], self.grid.nj[self.block], self.grid.nk[self.block]
+                _dist = np.sqrt((self.grid.grd[:_i, :_j, :_k, 0, self.block] - self.ppoint[0]) ** 2 +
+                                (self.grid.grd[:_i, :_j, :_k, 1, self.block] - self.ppoint[1]) ** 2 +
+                                (self.grid.grd[:_i, :_j, :_k, 2, self.block] - self.ppoint[2]) ** 2)
+
+                # Other methods to calculate distance. The above method is faster
+                # _grd_min_point = self.grid.grd[:_i, :_j, :_k, :, self.block] - self.point
+                # _dist = np.linalg.norm(_grd_min_point, axis=-1)
+                # _dist = np.sqrt(np.einsum("ijkl,ijkl->ijk", _grd_min_point, _grd_min_point))
+
+                self.index = np.array(np.unravel_index(_dist.argmin(), _dist.shape))
+                i, j, k = self.index
+                self._cell_index(self, i, j, k)
+                # Check for the end of the domain case
+                if max(self.cell[:, 0]) > self.grid.ni[self.block] - 1 or \
+                        max(self.cell[:, 1]) > self.grid.nj[self.block] - 1 or \
+                        max(self.cell[:, 2]) > self.grid.nk[self.block] - 1 or np.any(self.cell < 0):
+                    print('Block search returned wrong cell! Point position lost.\n')
+                    self.cpoint = None
+                    self.ppoint = None
+                    return
+
+            case 'p-space':
+                # Search for given point using newton-raphson
+                # credit: Sadarjoen et al.
+                # title: Particle tracing algorithms for 3D Curvilinear grids
+                # This search is performed every single time to find the given point
+                self.cpoint = self.p2c(self.ppoint)
+
+            case 'c-space':
+                # To run c-space global point location is needed
+                # credit: Sadarjoen et al.
+                # title: Particle tracing algorithms for 3D Curvilinear grids
+
+                # Transform given point from p-space to c-space using newton-raphson
+                # This is only performed once to get the initial c-space point
+                self.cpoint = self.p2c(self.ppoint)
+
+    def c2p(self, _cpoint):
+        """
+        Method to convert c-space point to p-space
+        self.block is kept constant through the c-space algos
+        self.block is checked and switched in streamlines algo
+        This method is commonly used to test point location as well
+        in different algorithms
+
+        Args:
+            _cpoint: c-space co-ordinates
+
+        Returns:
+            _ppoint: p-space co-ordinates
+
+        """
+        self.cpoint = _cpoint
+        _eps0, _eps1, _eps2 = _cpoint.astype(int)
+        _alpha, _beta, _gamma = np.modf(_cpoint)[0]  # same as eps % 1.0
+
+        # Check if the given point is in the domain
+        if _eps0 >= self.grid.ni[self.block]-1 or _eps1 >= self.grid.nj[self.block]-1 or \
+                _eps2 >= self.grid.nk[self.block]-1:
+            self.cpoint = None
+            self.ppoint = None
+            return self.ppoint
+
+        # Determine in which cell the current point is present
+        self.cell = self._cell_nodes(_eps0, _eps1, _eps2)
+        _cell_grd = self.grid.grd[self.cell[:, 0], self.cell[:, 1], self.cell[:, 2], :, self.block]
+
+        # Calculate the location in p-space
+        self.ppoint = (1 - _alpha) * (1 - _beta) * (1 - _gamma) * _cell_grd[0] + \
+                _alpha  * (1 - _beta) * (1 - _gamma) * _cell_grd[1] + \
+                _alpha  *      _beta  * (1 - _gamma) * _cell_grd[2] + \
+                (1 - _alpha) *      _beta  * (1 - _gamma) * _cell_grd[3] + \
+                (1 - _alpha) * (1 - _beta) *      _gamma  * _cell_grd[4] + \
+                _alpha  * (1 - _beta) *      _gamma  * _cell_grd[5] + \
+                _alpha  *      _beta *       _gamma  * _cell_grd[6] + \
+                (1 - _alpha) *      _beta  *      _gamma  * _cell_grd[7]
+
+        return self.ppoint
+
+    def p2c(self, _ppoint):
+        """
+        Method to convert p-space point to c-space
+        As there is no direct analytical equation. We use Newton-Raphson
+        Args:
+            _ppoint: p-space co-ordinates
+
+        Returns:
+            eps: c-space co-ordinates
+        """
+        global _cpoint
+        self.ppoint = _ppoint
+
+        if self.block is None:
+            self.block = self._find_block(self)
+
+        # Start Newton-Raphson
+        _iter = 0
+        # Initial guess
+        try:
+            _cpoint is not None
+        except:
+            _cpoint = np.array([self.grid.ni[self.block], self.grid.nj[self.block], self.grid.nk[self.block]]) / 2 + \
+                np.random.randn(3)
+
+        while True:
+            # Check if taking too long
+            if _iter >= 1e3:
+                print('**ERROR** Newton-Raphson did not converge. Try again!\n'
+                      'Possible reason might be the point might be too close to the end of a domain')
+                self.ppoint, self.cpoint = None, None
+                return
+
+            # Check for out-of-domain case and reset the point to in-domain
+            _eps0, _eps1, _eps2 = _cpoint.astype(int)
+            _alpha, _beta, _gamma = np.modf(_cpoint)[0]
+            if _eps0 + 1 >= self.grid.ni[self.block]:
+                _cpoint[0] = self.grid.ni[self.block] - 1 - _alpha
+            if _eps1 + 1 >= self.grid.nj[self.block]:
+                _cpoint[1] = self.grid.nj[self.block] - 1 - _beta
+            if _eps2 + 1 >= self.grid.nk[self.block]:
+                _cpoint[2] = self.grid.nk[self.block] - 1 - _gamma
+
+            # Compute eps after the point is reset
+            _eps0, _eps1, _eps2 = _cpoint.astype(int)
+            self.cell = self._cell_nodes(_eps0, _eps1, _eps2)
+
+            # Calculate J_inv for the point --> Uses tri-linear interpolation
+            _cell_J_inv = self.grid.m2[self.cell[:, 0], self.cell[:, 1], self.cell[:, 2], :, :, self.block]
+            _J_inv = (1 - _alpha) * (1 - _beta) * (1 - _gamma) * _cell_J_inv[0] + \
+                     _alpha * (1 - _beta) * (1 - _gamma) * _cell_J_inv[1] + \
+                     _alpha * _beta * (1 - _gamma) * _cell_J_inv[2] + \
+                     (1 - _alpha) * _beta * (1 - _gamma) * _cell_J_inv[3] + \
+                     (1 - _alpha) * (1 - _beta) * _gamma * _cell_J_inv[4] + \
+                     _alpha * (1 - _beta) * _gamma * _cell_J_inv[5] + \
+                     _alpha * _beta * _gamma * _cell_J_inv[6] + \
+                     (1 - _alpha) * _beta * _gamma * _cell_J_inv[7]
+
+            # Transform from c to p-space
+            _pred_ppoint = self.c2p(_cpoint)
+
+            # Difference b/w predicted point to given point
+            _delta_ppoint = _ppoint - _pred_ppoint
+
+            # End newton-raphson if condition is met
+            # TODO: Condition needs to be adapted based on Jacobian
+            # TODO: Need to improve by normalizing the data
+            _tol = 1e-12 * self.grid.J[self.cell[0, 0], self.cell[0, 1], self.cell[0, 2], self.block]
+            if _tol <= 1e-12:
+                _tol = 1e-12
+            if sum(abs(_delta_ppoint)) <= _tol:
+                _eps0, _eps1, _eps2 = _cpoint.astype(int)
+                # same as self.cell = self._cell_nodes(_eps0, _eps1, _eps2)
+                self._cell_index(self, _eps0, _eps1, _eps2)
+                self.cpoint = _cpoint
+                self.ppoint = _pred_ppoint
+                return _cpoint
+
+            # Transform from p to c-space
+            _delta_cpoint = np.matmul(_J_inv, _delta_ppoint)
+
+            # Save old point
+            _cpoint_old = _cpoint.copy()
+
+            # Update point
+            _cpoint += _delta_cpoint
+            # Update the point to zero if less than zero
+            _cpoint[_cpoint < 0] = 0
+            _cpoint = abs(_cpoint)
+            _iter += 1
+
+            pass
+
+
```

### Comparing `project-arrakis-0.1/src/streamlines/streamlines.py` & `project_arrakis-0.1.1/src/streamlines/streamlines.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,756 +1,793 @@
-# Uses the program API to extract streamlines
-import numpy as np
-from src.function.timer import Timer
-from src.io.plot3dio import GridIO
-from src.io.plot3dio import FlowIO
-from src.streamlines.search import Search
-from src.streamlines.interpolation import Interpolation
-from src.streamlines.integration import Integration
-from src.function.variables import Variables
-
-
-class Streamlines:
-    """
-    Module to extract particle path information
-
-    ...
-
-    Attributes
-    ----------
-    Input:
-        grid_file : str
-            Path to the plot3d grid data file
-        flow_file : str
-            Path to the plot3d flow data file
-        point : list
-            Starting point for integration
-        search : str
-            Default is p-space; can specify c-space
-        interpolation : str
-            Default is p-space; can specify c-space
-        integration : str
-            Default is p-space; can specify c-space
-        time_step : float
-            Default is 1e-3
-        magnitude_adaptivity : float
-            Set to override the adaptivity value
-
-    Output:
-        streamline : numpy.ndarray
-            shape is nx3; each column represents x, y, z
-        fvelocity : list
-            shape is nx3; each column represents ufx, ufy, ufz
-        svelocity: list
-            shape is nx3; each column represents vpx, vpy, vpz
-
-    Methods
-    -------
-    compute()
-        integrates and returns the streamline ndarray
-    ...
-
-    Example:
-        sl = Streamlines('../../data/vortex/vortex.sb.sp.x', '../../data/vortex/vortex.sb.sp.q', [-0.05, 0.05, 5])
-        sl.compute()
-    -------
-
-
-    """
-
-    def __init__(self, grid_file=None, flow_file=None, point=None,
-                 search='p-space', interpolation='p-space', integration='pRK4',
-                 diameter=1e-7, density=1000,
-                 time_step=1e-3, max_time_step=1, drag_model='stokes', adaptivity=0.001,
-                 magnitude_adaptivity=None, filepath=None, task=None):
-        self.grid_file = grid_file
-        self.flow_file = flow_file
-        self.point = np.array(point)
-        self.search = search
-        self.interpolation = interpolation
-        self.integration = integration
-        self.diameter = diameter
-        self.density = density
-        self.time_step = time_step
-        self.max_time_step = max_time_step
-        self.drag_model = drag_model
-        self.streamline = []
-        self.fvelocity = []
-        self.svelocity = []
-        self.time = []
-        self.adaptivity = adaptivity
-        self.magnitude_adaptivity = magnitude_adaptivity
-        self.filepath = filepath
-        self.task = task
-
-    # TODO: Need to add doc for streamlines
-
-    @staticmethod
-    def angle_btw(v1, v2):
-        # If vectors are tiny return for handling tiny time steps
-        # A lot of trail and error decided 1e-9 would work fast
-        if np.linalg.norm(v1) <= 1e-9 or np.linalg.norm(v2) <= 1e-9:
-            return None
-
-        u1 = v1 / np.linalg.norm(v1)
-        u2 = v2 / np.linalg.norm(v2)
-
-        y = u1 - u2
-        x = u1 + u2
-
-        a0 = 2 * np.arctan(np.linalg.norm(y) / np.linalg.norm(x))
-
-        if (not np.signbit(a0)) or np.signbit(np.pi - a0):
-            return np.rad2deg(a0)
-        elif np.signbit(a0):
-            return 0.0
-        else:
-            return 180
-
-    @staticmethod
-    def _save_data(self):
-        """
-        Pass self object to save data if the filepath is provided
-        Args:
-            self: self object of the class
-
-        Returns:
-            None
-        """
-        if self.filepath is not None:
-            p_xdata = np.array(self.streamline)
-            vdata = np.array(self.svelocity)
-            udata = np.array(self.fvelocity)
-            tdata = np.array(self.time).reshape(-1, 1)
-            f_xdata = p_xdata.copy()
-            for _i in range(1, len(f_xdata)):
-                f_xdata[_i] = f_xdata[_i - 1] + udata[_i - 1] * tdata[_i - 1]
-            # Data is added towards the end because of the development cycle. Mostly to work with dataio
-            _data_save = np.hstack((p_xdata, vdata, udata, tdata, f_xdata))
-
-            np.save(self.filepath + 'ppath_' + str(self.task), _data_save)
-            print('** SUCCESS ** Done writing file for particle number - ' + str(self.task) + ' ** SUCCESS **')
-            # set self to None to clear up memory after saving required data
-            self.streamline = []
-            self.svelocity = []
-            self.fvelocity = []
-            self.time = []
-        return
-
-    @staticmethod
-    def _magnitude(self, v1, v2):
-        # return the magnitude of the vector
-        _r = np.linalg.norm(v1 - v2) / min(np.linalg.norm(v1), np.linalg.norm(v2))
-        if _r < 1e-6 * self.magnitude_adaptivity:
-            _r = 1e-6 * self.magnitude_adaptivity
-        return _r
-
-    def compute(self, method='p-space', grid=None, flow=None):
-        """
-        Method to compute particle paths. Contains multiple algorithms
-        Args:
-            method:
-            grid:
-            flow:
-
-        Returns:
-
-        """
-        if grid is None or flow is None:
-            grid = GridIO(self.grid_file)
-            flow = FlowIO(self.flow_file)
-
-            # Read in the grid and flow data
-            grid.read_grid()
-            flow.read_flow()
-            grid.compute_metrics()
-
-        if self.magnitude_adaptivity is None:
-            self.magnitude_adaptivity = abs(np.min(np.gradient(grid.grd[..., 0])))
-        # Add data to output at the given point
-        # This is the assumption where particle velocity is same as the fluid
-        self.streamline.append(self.point)
-        idx = Search(grid, self.point)
-        interp = Interpolation(flow, idx)
-        idx.compute(method=self.search)
-        interp.compute(method=self.interpolation)
-        q_interp = Variables(interp)
-        q_interp.compute_velocity()
-        uf = q_interp.velocity.reshape(3)
-        self.fvelocity.append(uf)
-        self.svelocity.append(uf)
-        self.time.append(self.time_step)
-        loop_check = 0
-
-        if method == 'p-space':
-            t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
-            t.start()
-            while True:
-                idx = Search(grid, self.point)
-                interp = Interpolation(flow, idx)
-                intg = Integration(interp)
-                idx.compute(method=self.search)
-                interp.compute(method=self.interpolation)
-                new_point, new_vel = intg.compute(method=self.integration, time_step=self.time_step)
-                if new_point is None:
-                    print('Integration complete!')
-                    break
-                self.streamline.append(new_point)
-                self.fvelocity.append(new_vel)
-                self.svelocity.append(new_vel)
-                self.time.append(self.time_step)
-                self.point = new_point
-
-            # Save files for each particle; can be used for multiprocessing large number of particles
-            self._save_data(self)
-            t.stop()
-
-        if method == 'adaptive-p-space':
-            t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
-            t.start()
-            vel = None
-            while True:
-                idx = Search(grid, self.point)
-                interp = Interpolation(flow, idx)
-                intg = Integration(interp)
-                idx.compute(method=self.search)
-                interp.compute(method=self.interpolation)
-                new_point, new_vel = intg.compute(method=self.integration, time_step=self.time_step)
-                if new_point is None:
-                    print('Checking if the end of the domain is reached...')
-                    self.time_step = 1e-9 * self.time_step
-                    new_point, new_vel = intg.compute(method=self.integration, time_step=self.time_step)
-                    if new_point is not None:
-                        print('Continuing integration by decreasing time-step!')
-                        continue
-                    elif new_point is None:
-                        print('Integration complete!')
-                        break
-
-                # Adaptive algorithm starts
-                # Save results and adjust time-step
-                # Details for the algorithm are provided in adaptive-ppath
-                if vel is None:
-                    # For the first step in the loop
-                    self.streamline.append(new_point)
-                    self.fvelocity.append(new_vel)
-                    self.svelocity.append(new_vel)
-                    self.time.append(self.time_step)
-                    self.point = new_point
-                    vel = new_vel.copy()
-                elif self.angle_btw(new_point - self.point, vel) is None:
-                    print('Increasing time step. Successive points are same')
-                    self.time_step = 10 * self.time_step
-                    loop_check += 1
-                    if loop_check == 70:
-                        print('Stuck in the same loop for too long. Integration ends!')
-                        break
-                elif self.angle_btw(new_point - self.point, vel) <= 0.001 \
-                        and self.time_step <= self.max_time_step:
-                    self.streamline.append(new_point)
-                    self.fvelocity.append(new_vel)
-                    self.svelocity.append(new_vel)
-                    self.time.append(self.time_step)
-                    self.point = new_point
-                    vel = new_vel.copy()
-                    self.time_step = 2 * self.time_step
-                    loop_check = 0
-                elif self.angle_btw(new_point - self.point, vel) >= 0.01 and self.time_step >= 1e-12:
-                    self.time_step = 0.5 * self.time_step
-                else:
-                    self.streamline.append(new_point)
-                    self.fvelocity.append(new_vel)
-                    self.svelocity.append(new_vel)
-                    self.time.append(self.time_step)
-                    self.point = new_point
-                    vel = new_vel.copy()
-                    loop_check = 0
-
-            # Save files for each particle; can be used for multiprocessing large number of particles
-            self._save_data(self)
-            t.stop()
-
-        if method == 'c-space':
-            # Use c-space search to convert and find the location of given point
-            # All the idx attributes are converted to c-space -- point, cell, block
-            t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
-            t.start()
-            save_point = self.point
-            idx = Search(grid, self.point)
-            idx.compute(method='c-space')
-            while True:
-                interp = Interpolation(flow, idx)
-                interp.compute(method='c-space')
-                intg = Integration(interp)
-                new_point, new_pvel, new_cvel = intg.compute(method='cRK4', time_step=self.time_step)
-                if new_point is None:
-                    # For multi-block case if the point is out-of-block
-                    # Use previous point and run one-step of p-space algo
-                    print('Point exited the block! Searching for new position...')
-                    idx = Search(grid, save_point)
-                    interp = Interpolation(flow, idx)
-                    intg = Integration(interp)
-                    idx.compute(method='block_distance')
-                    interp.compute()
-                    new_point, new_pvel = intg.compute(method='pRK4', time_step=self.time_step)
-                    if new_point is None:
-                        print('Point out-of-domain. Integration complete!')
-                        break
-                    else:
-                        # Update the block in idx
-                        # new_point is in p-space for this else block
-
-                        idx = Search(grid, new_point)
-                        idx.compute(method='c-space')
-                        self.streamline.append(new_point)
-                        self.fvelocity.append(new_pvel)
-                        self.svelocity.append(new_pvel)
-                        self.time.append(self.time_step)
-                        self.point = save_point
-                        save_point = new_point
-                        pvel = new_pvel.copy()
-                else:
-                    save_point = idx.c2p(new_point)
-                    self.streamline.append(save_point)
-                    self.fvelocity.append(new_pvel)
-                    self.svelocity.append(new_pvel)
-                    self.time.append(self.time_step)
-                    idx.point = new_point
-
-            # Save files for each particle; can be used for multiprocessing large number of particles
-            self._save_data(self)
-            t.stop()
-
-        if method == 'adaptive-c-space':
-            # Use c-space search to convert and find the location of given point
-            # All the idx attributes are converted to c-space -- point, cell, block
-            # pvel signifies physical-space velocity
-            t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
-            t.start()
-            save_point = self.point
-            idx = Search(grid, self.point)
-            idx.compute(method='c-space')
-            pvel = None
-            while True:
-                interp = Interpolation(flow, idx)
-                interp.compute(method='c-space')
-                intg = Integration(interp)
-                new_point, new_pvel, new_cvel = intg.compute(method='cRK4', time_step=self.time_step)
-
-                # Check for large time-step in the last loop
-                if new_point is None:
-                    # Checking by decreasing time-step
-                    print('Checking if the end of the domain is reached...')
-                    self.time_step = 1e-9 * self.time_step
-                    new_point, new_pvel, new_cvel = intg.compute(method='cRK4', time_step=self.time_step)
-                    if new_point is not None:
-                        print('Continuing integration by decreasing time-step!')
-                        continue
-                    # Check for block switch
-                    elif new_point is None:
-                        # For multi-block case if the point is out-of-block
-                        # Use previous point and run one-step of p-space algo
-                        print('Point exited the block! Searching for new position...')
-                        idx = Search(grid, save_point)
-                        interp = Interpolation(flow, idx)
-                        intg = Integration(interp)
-                        idx.compute(method='block_distance')
-                        interp.compute()
-                        new_point, new_pvel = intg.compute(method='pRK4', time_step=self.time_step)
-                        # Even after pRK4 if the point is None; End integration
-                        if new_point is None:
-                            print('End of the domain. Integration Ends!')
-                            break
-                        # If not none; update to c-space and run
-                        else:
-                            # Update the block in idx
-                            idx = Search(grid, new_point)
-                            idx.compute(method='c-space')
-                            self.streamline.append(new_point)
-                            self.fvelocity.append(new_pvel)
-                            self.svelocity.append(new_pvel)
-                            self.time.append(self.time_step)
-                            self.point = save_point
-                            save_point = new_point
-                            pvel = new_pvel.copy()
-                            # new_point = idx.p2c(new_point)  # Move point obtained to c-space
-                # If the point is not none; continue c-space
-                else:
-                    self.point = save_point
-                    save_point = idx.c2p(new_point)
-
-                    # Adaptive algorithm starts
-                    # Save results and adjust time-step
-                    # Details for the algorithm are provided in adaptive-ppath
-                    # Decided to use new_pvel for adaptivity because of the in-shock cell RK4 integration
-                    # RK4 depends on future points for integration and this adjustment moves it forward
-                    if self.angle_btw(save_point - self.point, new_pvel) is None:
-                        print('Increasing time step. Successive points are same')
-                        self.time_step = 2 * self.time_step
-                        loop_check += 1
-                        if loop_check == 70:
-                            print('Stuck in the same loop for too long. Integration ends!')
-                            break
-                    elif self.angle_btw(save_point - self.point, new_pvel) <= 0.1 * self.adaptivity \
-                            and self.time_step <= self.max_time_step:
-                        self.point = save_point
-                        save_point = idx.c2p(new_point)
-                        self.streamline.append(save_point)
-                        self.fvelocity.append(new_pvel)
-                        self.svelocity.append(new_pvel)
-                        self.time.append(self.time_step)
-                        idx.point = new_point
-                        pvel = new_pvel.copy()
-                        self.time_step = 2 * self.time_step
-                        loop_check = 0
-                    elif self.angle_btw(save_point - self.point, new_pvel) >= self.adaptivity and\
-                            self.time_step >= 1e-12:
-                        self.time_step = 0.5 * self.time_step
-                    else:
-                        self.point = save_point
-                        save_point = idx.c2p(new_point)
-                        self.streamline.append(save_point)
-                        self.fvelocity.append(new_pvel)
-                        self.svelocity.append(new_pvel)
-                        self.time.append(self.time_step)
-                        idx.point = new_point
-                        pvel = new_pvel.copy()
-                        loop_check = 0
-            # Save files for each particle; can be used for multiprocessing large number of particles
-            self._save_data(self)
-            t.stop()
-
-        if method == 'ppath':
-            t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
-            t.start()
-            vel = None
-            fvel = None
-            while True:
-                idx = Search(grid, self.point)
-                interp = Interpolation(flow, idx)
-                intg = Integration(interp)
-                idx.compute(method=self.search)
-                interp.compute(method=self.interpolation)
-                new_point, new_vel, new_fvel = intg.compute_ppath(diameter=self.diameter,
-                                                                  density=self.density,
-                                                                  velocity=vel, method='pRK4',
-                                                                  time_step=self.time_step,
-                                                                  drag_model=self.drag_model)
-                if new_point is None:
-                    print('Integration complete!')
-                    break
-
-                # Save results and continue the loop
-                self.streamline.append(new_point)
-                self.svelocity.append(new_vel)
-                self.fvelocity.append(new_fvel)
-                self.time.append(self.time_step)
-                self.point = new_point
-                vel = new_vel.copy()
-                fvel = new_fvel.copy()
-
-            # Save files for each particle; can be used for multiprocessing large number of particles
-            self._save_data(self)
-            t.stop()
-
-        if method == 'adaptive-ppath':
-            t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
-            t.start()
-            # particle velocity
-            vel = None
-            # fluid velocity
-            fvel = None
-            while True:
-                idx = Search(grid, self.point)
-                interp = Interpolation(flow, idx)
-                intg = Integration(interp)
-                idx.compute(method=self.search)
-                interp.compute(method=self.interpolation)
-                new_point, new_vel, new_fvel = intg.compute_ppath(diameter=self.diameter, density=self.density,
-                                                                  velocity=vel,
-                                                                  method='pRK4', time_step=self.time_step,
-                                                                  drag_model=self.drag_model)
-                if new_point is None:
-                    # print('Checking if the end of the domain is reached...')
-                    self.time_step = 1e-9 * self.time_step
-                    new_point, new_vel, new_fvel = intg.compute_ppath(diameter=self.diameter, density=self.density,
-                                                                      velocity=vel,
-                                                                      method='pRK4', time_step=self.time_step,
-                                                                      drag_model=self.drag_model)
-                    if new_point is not None:
-                        # print('Continuing integration by decreasing time-step!')
-                        continue
-                    elif new_point is None:
-                        print('Integration complete!')
-                        break
-
-                # Check for mid-rk4 blowup
-                if intg.rk4_bool is True:
-                    print(f'**WARNING** Large residual. Mid-RK4 blow up! Reducing time-step for particle number'
-                          f' - {self.task}')
-                    intg.rk4_bool = False
-                    self.time_step = 0.5 * self.time_step
-                    loop_check += 1
-                    if loop_check == 70:
-                        print('Stuck in the same loop for too long. Integration ends!')
-                        break
-
-                # Adaptive algorithm starts
-                # Save results and continue the loop
-                elif vel is None:
-                    # For the first step in the loop
-                    self.streamline.append(new_point)
-                    self.svelocity.append(new_vel)
-                    self.fvelocity.append(new_fvel)
-                    self.time.append(self.time_step)
-                    self.point = new_point
-                    vel = new_vel.copy()
-                    fvel = new_fvel.copy()
-                # Check for if the points are identical because of tiny time step and deflection
-                elif self.angle_btw(new_vel, vel) is None:
-                    # print('Increasing time step. Successive points are same')
-                    self.time_step = 2 * self.time_step
-                    loop_check += 1
-                    if loop_check == 70:
-                        print(f'Successive points did not change for too long. Integration ends! for particle '
-                              f'{self.task}')
-                        break
-                # Check for strong acceleration and reduce time-step
-                # Increase time step when angle is below 0.05 degrees
-                elif self.angle_btw(new_vel, vel) <= 0.1 * self.adaptivity and self.time_step <= self.max_time_step \
-                        and self._magnitude(self, new_vel, vel) <= 0.01 * self.magnitude_adaptivity:
-                    # print('Increasing time step. Low deflection wrt velocity')
-                    self.streamline.append(new_point)
-                    self.svelocity.append(new_vel)
-                    self.fvelocity.append(new_fvel)
-                    self.time.append(self.time_step)
-                    self.point = new_point
-                    vel = new_vel.copy()
-                    fvel = new_fvel.copy()
-                    self.time_step = 2 * self.time_step
-                    loop_check = 0
-                # Decrease time step when angle is above 1.4 degrees
-                # Make sure time step does not go to zero; 1 pico-second
-                elif self.angle_btw(new_vel, vel) >= self.adaptivity and self.time_step >= 1e-12 \
-                        and self._magnitude(self, new_vel, vel) >= 0.1 * self.magnitude_adaptivity:
-                    # print('Decreasing time step. High deflection wrt velocity')
-                    self.time_step = 0.5 * self.time_step
-                # Save if none of the above conditions meet
-                else:
-                    self.streamline.append(new_point)
-                    self.svelocity.append(new_vel)
-                    self.fvelocity.append(new_fvel)
-                    self.time.append(self.time_step)
-                    self.point = new_point
-                    vel = new_vel.copy()
-                    fvel = new_fvel.copy()
-                    loop_check = 0
-
-            # Save files for each particle; can be used for multiprocessing large number of particles
-            self._save_data(self)
-            t.stop()
-
-        if method == 'ppath-c-space':
-            t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
-            t.start()
-            pvel = None
-            fvel = None
-            save_point = self.point
-            idx = Search(grid, self.point)
-            idx.compute(method='c-space')
-            while True:
-                interp = Interpolation(flow, idx)
-                interp.compute(method='c-space')
-                intg = Integration(interp)
-                new_point, new_fvel, new_pvel = intg.compute_ppath(diameter=self.diameter,
-                                                                   density=self.density,
-                                                                   velocity=pvel, method='cRK4',
-                                                                   time_step=self.time_step,
-                                                                   drag_model=self.drag_model)
-                if new_point is None:
-                    # For multi-block case if the point is out-of-block
-                    # Use previous point and run one-step of p-space algo
-                    print('Point exited the block! Searching for new position...')
-                    idx = Search(grid, save_point)
-                    interp = Interpolation(flow, idx)
-                    intg = Integration(interp)
-                    idx.compute(method='p-space')
-                    interp.compute()
-                    new_point, new_fvel, new_pvel = intg.compute_ppath(diameter=self.diameter,
-                                                                       density=self.density,
-                                                                       velocity=pvel, method='pRK4',
-                                                                       time_step=self.time_step,
-                                                                       drag_model=self.drag_model)
-                    if new_point is None:
-                        print('Point out-of-domain. Integration complete!')
-                        break
-                    else:
-                        # Update the block in idx
-                        idx = Search(grid, new_point)
-                        idx.compute(method='c-space')
-                        self.streamline.append(new_point)
-                        self.fvelocity.append(new_fvel)
-                        self.svelocity.append(new_pvel)
-                        self.time.append(self.time_step)
-                        pvel = new_pvel.copy()
-                        fvel = new_fvel.copy()
-                        self.point = save_point
-                        save_point = new_point
-                else:
-
-                    # Check for mid-rk4 blowup
-                    if intg.rk4_bool is True:
-                        print('Mid-RK4 blow up! Reducing time-step')
-                        intg.rk4_bool = False
-                        self.time_step = 0.5 * self.time_step
-                        loop_check += 1
-                        if loop_check == 70:
-                            print('Stuck in the same loop for too long. Integration ends!')
-                            break
-
-                    else:
-                        self.point = save_point
-                        save_point = idx.c2p(new_point)
-                        self.streamline.append(save_point)
-                        self.fvelocity.append(new_fvel)
-                        self.svelocity.append(new_pvel)
-                        self.time.append(self.time_step)
-                        pvel = new_pvel.copy()
-                        fvel = new_fvel.copy()
-                        idx.point = new_point
-                        if loop_check > 0:
-                            print('Resetting time step')
-                            self.time_step = self.time_step / 0.5 ** loop_check
-                            loop_check = 0
-
-            # Save files for each particle; can be used for multiprocessing large number of particles
-            self._save_data(self)
-            t.stop()
-
-        if method == 'adaptive-ppath-c-space':
-            t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
-            t.start()
-            pvel = None
-            fvel = None
-            save_point = self.point
-            idx = Search(grid, self.point)
-            idx.compute(method='c-space')
-            while True:
-                interp = Interpolation(flow, idx)
-                interp.compute(method='c-space')
-                intg = Integration(interp)
-                new_point, new_fvel, new_pvel = intg.compute_ppath(diameter=self.diameter,
-                                                                   density=self.density,
-                                                                   velocity=pvel, method='cRK4',
-                                                                   time_step=self.time_step,
-                                                                   drag_model=self.drag_model)
-                # Check if the point is out-of-block
-                if new_point is None:
-                    # Check for large time-step
-                    print('Checking if the end of the domain is reached...')
-                    self.time_step = 1e-9 * self.time_step
-                    new_point, new_fvel, new_pvel = intg.compute_ppath(diameter=self.diameter,
-                                                                       density=self.density,
-                                                                       velocity=pvel, method='cRK4',
-                                                                       time_step=self.time_step,
-                                                                       drag_model=self.drag_model)
-                    if new_point is not None:
-                        print('Continuing integration by decreasing time-step!')
-                        continue
-                    # Check for out-of-block situation
-                    # For multi-block case if the point is out-of-block
-                    # Use previous point and run one-step of p-space algo
-                    elif new_point is None:
-                        print('Point exited the block! Searching for new position...')
-                        idx = Search(grid, save_point)
-                        interp = Interpolation(flow, idx)
-                        intg = Integration(interp)
-                        idx.compute(method='p-space')
-                        interp.compute()
-                        new_point, new_fvel, new_pvel = intg.compute_ppath(diameter=self.diameter,
-                                                                           density=self.density,
-                                                                           velocity=pvel, method='pRK4',
-                                                                           time_step=self.time_step,
-                                                                           drag_model=self.drag_model)
-                        if new_point is None:
-                            print('Point out-of-domain. Integration complete!')
-                            break
-                        else:
-                            # Update the block in idx
-                            idx = Search(grid, new_point)
-                            idx.compute(method='c-space')
-                            # new_point found is in p-space; so, append
-                            self.streamline.append(new_point)
-                            self.fvelocity.append(new_fvel)
-                            self.svelocity.append(new_pvel)
-                            self.time.append(self.time_step)
-                            pvel = new_pvel.copy()
-                            fvel = new_fvel.copy()
-                            self.point = save_point
-                            save_point = new_point
-                else:
-                    self.point = save_point
-                    save_point = idx.c2p(new_point)
-
-                    # Check for mid-rk4 blowup
-                    if intg.rk4_bool is True:
-                        print(f'**WARNING** Large residual. Mid-RK4 blow up! Reducing time-step for particle number'
-                              f' - {self.task}')
-                        intg.rk4_bool = False
-                        self.time_step = 0.5 * self.time_step
-                        loop_check += 1
-                        if loop_check == 70:
-                            print('Stuck in the same loop for too long. Integration ends!')
-                            break
-
-                    # Adaptive algorithm starts
-                    # Save results and adjust time-step
-                    # Details for the algorithm are provided in adaptive-ppath
-                    elif pvel is None:
-                        # For the first step in the loop
-                        self.streamline.append(save_point)
-                        self.svelocity.append(new_pvel)
-                        self.fvelocity.append(new_fvel)
-                        self.time.append(self.time_step)
-                        self.point = new_point
-                        pvel = new_pvel.copy()
-                        fvel = new_fvel.copy()
-                    elif self.angle_btw(new_fvel, fvel) is None:
-                        print('Increasing time step. Successive points are same')
-                        self.time_step = 2 * self.time_step
-                        loop_check += 1
-                        if loop_check == 70:
-                            print(f'Successive points did not change for too long. Integration ends! for particle '
-                                  f'{self.task}')
-                            break
-                    elif self.angle_btw(new_fvel,
-                                        fvel) <= 0.1 * self.adaptivity and self.time_step <= self.max_time_step:
-                        self.point = save_point
-                        save_point = idx.c2p(new_point)
-                        self.streamline.append(save_point)
-                        self.fvelocity.append(new_fvel)
-                        self.svelocity.append(new_pvel)
-                        self.time.append(self.time_step)
-                        idx.point = new_point.copy()
-                        pvel = new_pvel.copy()
-                        fvel = new_fvel.copy()
-                        self.time_step = 2 * self.time_step
-                        loop_check = 0
-                    elif self.angle_btw(new_fvel, fvel) >= self.adaptivity and self.time_step >= 1e-12:
-                        self.time_step = 0.5 * self.time_step
-                    else:
-                        self.point = save_point
-                        save_point = idx.c2p(new_point)
-                        self.streamline.append(save_point)
-                        self.fvelocity.append(new_fvel)
-                        self.svelocity.append(new_pvel)
-                        self.time.append(self.time_step)
-                        idx.point = new_point.copy()
-                        pvel = new_pvel.copy()
-                        fvel = new_fvel.copy()
-                        loop_check = 0
-
-            # Save files for each particle; can be used for multiprocessing large number of particles
-            self._save_data(self)
-            t.stop()
-
-        return
+# Uses the program API to extract streamlines
+import numpy as np
+from src.function.timer import Timer
+from src.io.plot3dio import GridIO
+from src.io.plot3dio import FlowIO
+from src.streamlines.search import Search
+from src.streamlines.interpolation import Interpolation
+from src.streamlines.integration import Integration
+from src.function.variables import Variables
+import matplotlib.pyplot as plt
+import functools
+
+
+class Streamlines:
+    """
+    Module to extract particle path information
+
+    ...
+
+    Attributes
+    ----------
+    Input:
+        grid_file : str
+            Path to the plot3d grid data file
+        flow_file : str
+            Path to the plot3d flow data file
+        point : list
+            Starting point for integration
+        search : str
+            Default is p-space; can specify c-space
+        interpolation : str
+            Default is p-space; can specify c-space
+        integration : str
+            Default is p-space; can specify c-space
+        time_step : float
+            Default is 1e-3
+        magnitude_adaptivity : float
+            Set to override the adaptivity value
+
+    Output:
+        streamline : numpy.ndarray
+            shape is nx3; each column represents x, y, z
+        fvelocity : list
+            shape is nx3; each column represents ufx, ufy, ufz
+        svelocity: list
+            shape is nx3; each column represents vpx, vpy, vpz
+
+    Methods
+    -------
+    compute()
+        integrates and returns the streamline ndarray
+    ...
+
+    Example:
+        sl = Streamlines('../../data/vortex/vortex.sb.sp.x', '../../data/vortex/vortex.sb.sp.q', [-0.05, 0.05, 5])
+        sl.compute()
+    -------
+
+
+    """
+
+    def __init__(self, grid_file=None, flow_file=None, point=None,
+                 search='p-space', interpolation='p-space', integration='pRK4',
+                 diameter=1e-7, density=1000,
+                 time_step=1e-3, max_time_step=1, drag_model='stokes', adaptivity=0.001,
+                 magnitude_adaptivity=0.001, filepath=None, task=None, debug=False):
+        self.grid_file = grid_file
+        self.flow_file = flow_file
+        self.point = np.array(point)
+        self.search = search
+        self.interpolation = interpolation
+        self.adaptive_interpolation = None
+        self.integration = integration
+        self.diameter = diameter
+        self.density = density
+        self.time_step = time_step
+        self.max_time_step = max_time_step
+        self.drag_model = drag_model
+        self.streamline = []
+        self.fvelocity = []
+        self.svelocity = []
+        self.time = []
+        self.adaptivity = adaptivity
+        self.magnitude_adaptivity = magnitude_adaptivity
+        self.filepath = filepath
+        self.task = task
+        self.debug = debug
+
+    # TODO: Need to add doc for streamlines
+
+    @staticmethod
+    def angle_btw(v1, v2):
+        # If vectors are tiny return for handling tiny time steps
+        # A lot of trail and error decided 1e-9 would work fast
+        if np.linalg.norm(v1) <= 1e-9 or np.linalg.norm(v2) <= 1e-9:
+            return None
+
+        u1 = v1 / np.linalg.norm(v1)
+        u2 = v2 / np.linalg.norm(v2)
+
+        y = u1 - u2
+        x = u1 + u2
+
+        a0 = 2 * np.arctan(np.linalg.norm(y) / np.linalg.norm(x))
+
+        if (not np.signbit(a0)) or np.signbit(np.pi - a0):
+            return np.rad2deg(a0)
+        elif np.signbit(a0):
+            return 0.0
+        else:
+            return 180
+
+    @staticmethod
+    def _save_data(self):
+        """
+        Pass self object to save data if the filepath is provided
+        Args:
+            self: self object of the class
+
+        Returns:
+            None
+        """
+        if self.filepath is not None:
+            p_xdata = np.array(self.streamline)
+            vdata = np.array(self.svelocity)
+            udata = np.array(self.fvelocity)
+            tdata = np.array(self.time).reshape(-1, 1)
+            f_xdata = p_xdata.copy()
+            for _i in range(1, len(f_xdata)):
+                f_xdata[_i] = f_xdata[_i - 1] + udata[_i - 1] * tdata[_i - 1]
+            # Data is added towards the end because of the development cycle. Mostly to work with dataio
+            _data_save = np.hstack((p_xdata, vdata, udata, tdata, f_xdata,
+                                    np.ones(tdata.shape) * self.diameter,
+                                    np.ones(tdata.shape) * self.density))
+
+            np.save(self.filepath + 'ppath_' + str(self.task), _data_save)
+            self.print_debug(self, '** SUCCESS ** Done writing file for particle number - ' + str(self.task) + ' ** SUCCESS **')
+            # set self to None to clear up memory after saving required data
+            self.streamline = []
+            self.svelocity = []
+            self.fvelocity = []
+            self.time = []
+        return
+
+    @staticmethod
+    def _magnitude(self, v1, v2):
+        # return the magnitude of the vector
+        _r = np.linalg.norm(v1 - v2) / min(np.linalg.norm(v1), np.linalg.norm(v2))
+        if _r < 1e-6 * self.magnitude_adaptivity:
+            _r = 1e-6 * self.magnitude_adaptivity
+        return _r
+
+    @staticmethod
+    def plot_live(func):
+        # Interactive mode for jupyter notebook
+        # plt.ion()
+        @functools.wraps(func)
+        def new_func(*args, **kwargs):
+            # Clear all axes in the current figure.
+            axes = plt.gcf().get_axes()
+            for axis in axes:
+                axis.cla()
+
+            # Call func to plot something
+            result = func(*args, **kwargs)
+
+            # Draw the plot
+            plt.draw()
+            plt.pause(0.001)
+
+            return result
+
+        return new_func
+
+    @plot_live
+    def plot_update(self, ax, *args, **kwargs):
+        colors = ['b', 'g', 'c', 'm', 'y', 'k']
+        for i, (x, y) in enumerate(zip(args[::2], args[1::2])):
+            color = colors[i % len(colors)]
+            ax.plot(x, y, color)
+            ax.plot(x[-5:], y[-5:], 'r-')
+            ax.plot(x[-1], y[-1], 'ro')
+        ax.set_title(kwargs.get('title', ''))
+
+        return
+
+    @staticmethod
+    def print_debug(self, statement):
+        if self.debug is True:
+            print(statement)
+        return
+
+    def compute(self, method='p-space', grid=None, flow=None):
+        """
+        Method to compute particle paths. Contains multiple algorithms
+        Args:
+            method:
+            grid:
+            flow:
+
+        Returns:
+
+        """
+        if grid is None or flow is None:
+            grid = GridIO(self.grid_file)
+            flow = FlowIO(self.flow_file)
+
+            # Read in the grid and flow data
+            grid.read_grid()
+            flow.read_flow()
+            grid.compute_metrics()
+
+        if self.magnitude_adaptivity is None:
+            self.magnitude_adaptivity = abs(np.min(np.gradient(grid.grd[..., 0])))
+        # Add data to output at the given point
+        # This is the assumption where particle velocity is same as the fluid
+        self.streamline.append(self.point)
+        idx = Search(grid, self.point)
+        interp = Interpolation(flow, idx)
+        interp.adaptive = self.adaptive_interpolation
+        idx.compute(method=self.search)
+        interp.compute(method=self.interpolation)
+        q_interp = Variables(interp)
+        q_interp.compute_velocity()
+        uf = q_interp.velocity.reshape(3)
+        vel = uf.copy()
+        pvel = uf.copy()
+        fvel = uf.copy()
+        self.fvelocity.append(uf)
+        self.svelocity.append(uf)
+        self.time.append(self.time_step)
+        loop_check = 0
+
+        if method == 'p-space':
+            # t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
+            # t.start()
+            while True:
+                idx = Search(grid, self.point)
+                interp = Interpolation(flow, idx)
+                interp.adaptive = self.adaptive_interpolation
+                intg = Integration(interp)
+                idx.compute(method=self.search)
+                interp.compute(method=self.interpolation)
+                new_point, new_vel = intg.compute(method=self.integration, time_step=self.time_step)
+                if new_point is None:
+                    self.print_debug(self, 'Integration complete!')
+                    break
+                self.streamline.append(new_point)
+                self.fvelocity.append(new_vel)
+                self.svelocity.append(new_vel)
+                self.time.append(self.time_step)
+                self.point = new_point
+
+            # Save files for each particle; can be used for multiprocessing large number of particles
+            self._save_data(self)
+            # t.stop()
+
+        if method == 'adaptive-p-space':
+            # t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
+            # t.start()
+            while True:
+                idx = Search(grid, self.point)
+                interp = Interpolation(flow, idx)
+                interp.adaptive = self.adaptive_interpolation
+                intg = Integration(interp)
+                idx.compute(method=self.search)
+                interp.compute(method=self.interpolation)
+                new_point, new_vel = intg.compute(method=self.integration, time_step=self.time_step)
+                if new_point is None:
+                    self.print_debug(self, 'Checking if the end of the domain is reached...')
+                    self.time_step = 1e-9 * self.time_step
+                    new_point, new_vel = intg.compute(method=self.integration, time_step=self.time_step)
+                    if new_point is not None:
+                        self.print_debug(self, 'Continuing integration by decreasing time-step!')
+                        continue
+                    elif new_point is None:
+                        self.print_debug(self, 'Integration complete!')
+                        break
+
+                # Adaptive algorithm starts
+                # Save results and adjust time-step
+                # Details for the algorithm are provided in adaptive-ppath
+                if self.angle_btw(new_point - self.point, vel) is None:
+                    self.print_debug(self, 'Increasing time step. Successive points are same')
+                    self.time_step = 10 * self.time_step
+                    loop_check += 1
+                    if loop_check == 70:
+                        self.print_debug(self, 'Stuck in the same loop for too long. Integration ends!')
+                        break
+                elif self.angle_btw(new_point - self.point, vel) <= 0.001 \
+                        and self.time_step <= self.max_time_step:
+                    self.streamline.append(new_point)
+                    self.fvelocity.append(new_vel)
+                    self.svelocity.append(new_vel)
+                    self.time.append(self.time_step)
+                    self.point = new_point
+                    vel = new_vel.copy()
+                    self.time_step = 2 * self.time_step
+                    loop_check = 0
+                elif self.angle_btw(new_point - self.point, vel) >= 0.01 and self.time_step >= 1e-12:
+                    self.time_step = 0.5 * self.time_step
+                else:
+                    self.streamline.append(new_point)
+                    self.fvelocity.append(new_vel)
+                    self.svelocity.append(new_vel)
+                    self.time.append(self.time_step)
+                    self.point = new_point
+                    vel = new_vel.copy()
+                    loop_check = 0
+
+            # Save files for each particle; can be used for multiprocessing large number of particles
+            self._save_data(self)
+            # t.stop()
+
+        if method == 'c-space':
+            # Use c-space search to convert and find the location of given point
+            # All the idx attributes are converted to c-space -- point, cell, block
+            # t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
+            # t.start()
+            save_point = self.point
+            idx = Search(grid, self.point)
+            idx.compute(method='c-space')
+            while True:
+                interp = Interpolation(flow, idx)
+                interp.adaptive = self.adaptive_interpolation
+                interp.compute(method='c-space')
+                intg = Integration(interp)
+                new_point, new_pvel, new_cvel = intg.compute(method='cRK4', time_step=self.time_step)
+                if new_point is None:
+                    # For multi-block case if the point is out-of-block
+                    # Use previous point and run one-step of p-space algo
+                    self.print_debug(self, 'Point exited the block! Searching for new position...')
+                    idx = Search(grid, save_point)
+                    interp = Interpolation(flow, idx)
+                    interp.adaptive = self.adaptive_interpolation
+                    intg = Integration(interp)
+                    idx.compute(method='block_distance')
+                    interp.compute()
+                    new_point, new_pvel = intg.compute(method='pRK4', time_step=self.time_step)
+                    if new_point is None:
+                        self.print_debug(self, 'Point out-of-domain. Integration complete!')
+                        break
+                    else:
+                        # Update the block in idx
+                        # new_point is in p-space for this else block
+
+                        idx = Search(grid, new_point)
+                        idx.compute(method='c-space')
+                        self.streamline.append(new_point)
+                        self.fvelocity.append(new_pvel)
+                        self.svelocity.append(new_pvel)
+                        self.time.append(self.time_step)
+                        self.point = save_point
+                        save_point = new_point
+                        pvel = new_pvel.copy()
+                else:
+                    save_point = idx.c2p(new_point)
+                    self.streamline.append(save_point)
+                    self.fvelocity.append(new_pvel)
+                    self.svelocity.append(new_pvel)
+                    self.time.append(self.time_step)
+                    idx.point = new_point
+
+            # Save files for each particle; can be used for multiprocessing large number of particles
+            self._save_data(self)
+            # t.stop()
+
+        if method == 'adaptive-c-space':
+            # Use c-space search to convert and find the location of given point
+            # All the idx attributes are converted to c-space -- point, cell, block
+            # pvel signifies physical-space velocity
+            # t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
+            # t.start()
+            save_point = self.point
+            idx = Search(grid, self.point)
+            idx.compute(method='c-space')
+            while True:
+                interp = Interpolation(flow, idx)
+                interp.compute(method='c-space')
+                interp.adaptive = self.adaptive_interpolation
+                intg = Integration(interp)
+                new_point, new_pvel, new_cvel = intg.compute(method='cRK4', time_step=self.time_step)
+
+                # Check for large time-step in the last loop
+                if new_point is None:
+                    # Checking by decreasing time-step
+                    self.print_debug(self, 'Checking if the end of the domain is reached...')
+                    self.time_step = 1e-9 * self.time_step
+                    new_point, new_pvel, new_cvel = intg.compute(method='cRK4', time_step=self.time_step)
+                    if new_point is not None:
+                        self.print_debug(self, 'Continuing integration by decreasing time-step!')
+                        continue
+                    # Check for block switch
+                    elif new_point is None:
+                        # For multi-block case if the point is out-of-block
+                        # Use previous point and run one-step of p-space algo
+                        self.print_debug(self, 'Point exited the block! Searching for new position...')
+                        idx = Search(grid, save_point)
+                        interp = Interpolation(flow, idx)
+                        interp.adaptive = self.adaptive_interpolation
+                        intg = Integration(interp)
+                        idx.compute(method='block_distance')
+                        interp.compute(method='p-space')
+                        new_point, new_pvel = intg.compute(method='pRK4', time_step=self.time_step)
+                        # Even after pRK4 if the point is None; End integration
+                        if new_point is None:
+                            self.print_debug(self, 'End of the domain. Integration Ends!')
+                            break
+                        # If not none; update to c-space and run
+                        else:
+                            # Update the block in idx
+                            idx = Search(grid, new_point)
+                            idx.compute(method='c-space')
+                            self.streamline.append(new_point)
+                            self.fvelocity.append(new_pvel)
+                            self.svelocity.append(new_pvel)
+                            self.time.append(self.time_step)
+                            save_point = new_point
+                            pvel = new_pvel.copy()
+                            # new_point = idx.p2c(new_point)  # Move point obtained to c-space
+                # If the point is not none; continue c-space
+                else:
+                    old_ppoint = save_point
+                    # This changes the cell attribute in idx, used for interp
+                    new_ppoint = idx.c2p(new_point)
+
+                    # Adaptive algorithm starts
+                    # Save results and adjust time-step
+                    # Details for the algorithm are provided in adaptive-ppath
+                    if self.angle_btw(new_ppoint - old_ppoint, pvel) is None:
+                        self.print_debug(self, 'Increasing time step. Successive points are same')
+                        self.time_step = 2 * self.time_step
+                        loop_check += 1
+                        if loop_check == 70:
+                            self.print_debug(self, 'Stuck in the same loop for too long. Integration ends!')
+                            break
+                    elif self.angle_btw(new_ppoint - old_ppoint, pvel) <= 0.1 * self.adaptivity \
+                            and self.time_step <= self.max_time_step:
+                        save_point = new_ppoint
+                        self.streamline.append(save_point)
+                        self.fvelocity.append(new_pvel)
+                        self.svelocity.append(new_pvel)
+                        self.time.append(self.time_step)
+                        idx.point = new_point
+                        pvel = new_pvel.copy()
+                        self.time_step = 2 * self.time_step
+                        loop_check = 0
+                    elif self.angle_btw(new_ppoint - old_ppoint, pvel) >= self.adaptivity and \
+                            self.time_step >= 1e-12:
+                        self.time_step = 0.5 * self.time_step
+                    else:
+                        save_point = new_ppoint
+                        self.streamline.append(save_point)
+                        self.fvelocity.append(new_pvel)
+                        self.svelocity.append(new_pvel)
+                        self.time.append(self.time_step)
+                        idx.point = new_point
+                        pvel = new_pvel.copy()
+                        loop_check = 0
+            # Save files for each particle; can be used for multiprocessing large number of particles
+            self._save_data(self)
+            # t.stop()
+
+        if method == 'ppath':
+            # t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
+            # t.start()
+            vel = None
+            fvel = None
+            while True:
+                idx = Search(grid, self.point)
+                interp = Interpolation(flow, idx)
+                intg = Integration(interp)
+                interp.adaptive = self.adaptive_interpolation
+                idx.compute(method=self.search)
+                interp.compute(method=self.interpolation)
+                new_point, new_vel, new_fvel = intg.compute_ppath(diameter=self.diameter,
+                                                                  density=self.density,
+                                                                  velocity=vel, method='pRK4',
+                                                                  time_step=self.time_step,
+                                                                  drag_model=self.drag_model)
+                if new_point is None:
+                    self.print_debug(self, 'Integration complete!')
+                    break
+
+                # Save results and continue the loop
+                self.streamline.append(new_point)
+                self.svelocity.append(new_vel)
+                self.fvelocity.append(new_fvel)
+                self.time.append(self.time_step)
+                self.point = new_point
+                vel = new_vel.copy()
+                fvel = new_fvel.copy()
+
+            # Save files for each particle; can be used for multiprocessing large number of particles
+            self._save_data(self)
+            # t.stop()
+
+        if method == 'adaptive-ppath':
+            # t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
+            # t.start()
+            if self.debug:
+                fig, ax = plt.subplots()
+            while True:
+                idx = Search(grid, self.point)
+                interp = Interpolation(flow, idx)
+                interp.adaptive = self.adaptive_interpolation
+                intg = Integration(interp)
+                idx.compute(method=self.search)
+                interp.compute(method=self.interpolation)
+                new_point, new_vel, new_fvel = intg.compute_ppath(diameter=self.diameter, density=self.density,
+                                                                  velocity=vel,
+                                                                  method='pRK4', time_step=self.time_step,
+                                                                  drag_model=self.drag_model)
+                if new_point is None:
+                    self.print_debug(self, 'Checking if the end of the domain is reached...')
+                    if self.time_step <= 1e-12:
+                        self.time_step = self.time_step
+                    else:
+                        self.time_step = 1e-2 * self.time_step
+                    new_point, new_vel, new_fvel = intg.compute_ppath(diameter=self.diameter, density=self.density,
+                                                                      velocity=vel,
+                                                                      method='pRK4', time_step=self.time_step,
+                                                                      drag_model=self.drag_model)
+                    if new_point is not None:
+                        self.print_debug(self, 'Continuing integration by decreasing time-step!')
+                        continue
+                    elif new_point is None:
+                        self.print_debug(self, 'Integration complete!')
+                        break
+
+                # Check for mid-rk4 blowup
+                if intg.rk4_bool is True:
+                    self.print_debug(self, f'**WARNING** Large residual. Mid-RK4 blow up! Reducing time-step for particle number'
+                          f' - {self.task}')
+                    intg.rk4_bool = False
+                    self.time_step = 0.5 * self.time_step
+                    loop_check += 1
+                    if loop_check == 70:
+                        self.print_debug(self, 'Stuck in the same loop for too long. Integration ends!')
+                        break
+
+                # Adaptive algorithm starts
+                # Save results and continue the loop
+                # Check for if the points are identical because of tiny time step and deflection
+                elif self.angle_btw(new_vel, vel) is None:
+                    self.print_debug(self, 'Increasing time step. Successive points are same')
+                    self.time_step = 2 * self.time_step
+                    loop_check += 1
+                    if loop_check == 70:
+                        self.print_debug(self, f'Successive points did not change for too long. Integration ends! for particle '
+                              f'{self.task}')
+                        break
+                # Check for strong acceleration and reduce time-step
+                # Increase time step when angle is below 0.05 degrees
+                elif self.angle_btw(new_vel, vel) <= 0.1 * self.adaptivity and self.time_step <= self.max_time_step \
+                        and self._magnitude(self, new_vel, vel) <= 0.1 * self.magnitude_adaptivity:
+                    self.print_debug(self, 'Increasing time step. Low deflection wrt velocity')
+                    self.streamline.append(new_point)
+                    self.svelocity.append(new_vel)
+                    self.fvelocity.append(new_fvel)
+                    self.time.append(self.time_step)
+                    self.point = new_point
+                    vel = new_vel.copy()
+                    fvel = new_fvel.copy()
+                    self.time_step = 2 * self.time_step
+                    loop_check = 0  # This check might lead to slower integration for some edge cases
+                # Decrease time step when angle is above 1.4 degrees
+                # Make sure time step does not go to zero; 1 pico-second
+                elif self.angle_btw(new_vel, vel) >= self.adaptivity and self.time_step >= 1e-12 \
+                        and self._magnitude(self, new_vel, vel) >= self.magnitude_adaptivity:
+                    self.print_debug(self, 'Decreasing time step. High deflection wrt velocity')
+                    self.time_step = 0.5 * self.time_step
+                # Save if none of the above conditions meet
+                else:
+                    self.streamline.append(new_point)
+                    self.svelocity.append(new_vel)
+                    self.fvelocity.append(new_fvel)
+                    self.time.append(self.time_step)
+                    self.point = new_point
+                    vel = new_vel.copy()
+                    fvel = new_fvel.copy()
+                    loop_check = 0
+
+                # Plot the streamline for debugging
+                # add levels to debug; multiple ways of showing plots etc...
+                # This will help when working with varying flow fields
+                if self.debug:
+                    self.plot_update(ax,
+                                    [i[0] for i in self.streamline], [i[0] for i in self.svelocity],
+                                    [i[0] for i in self.streamline], [i[0] for i in self.fvelocity],
+                                    title=f'Particle number - {self.task} and diameter - {self.diameter},\n'
+                                          f' density - {self.density} and time-step - {self.time_step}')
+
+            # Save files for each particle; can be used for multiprocessing large number of particles
+            self._save_data(self)
+            # t.stop()
+
+        if method == 'ppath-c-space':
+            t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
+            t.start()
+            save_point = self.point
+            idx = Search(grid, self.point)
+            idx.compute(method='c-space')
+            while True:
+                interp = Interpolation(flow, idx)
+                interp.adaptive = self.adaptive_interpolation
+                interp.compute(method='c-space')
+                intg = Integration(interp)
+                new_point, new_fvel, new_pvel = intg.compute_ppath(diameter=self.diameter,
+                                                                   density=self.density,
+                                                                   velocity=pvel, method='cRK4',
+                                                                   time_step=self.time_step,
+                                                                   drag_model=self.drag_model)
+                if new_point is None:
+                    # For multi-block case if the point is out-of-block
+                    # Use previous point and run one-step of p-space algo
+                    self.print_debug(self, 'Point exited the block! Searching for new position...')
+                    idx = Search(grid, save_point)
+                    interp = Interpolation(flow, idx)
+                    interp.adaptive = self.adaptive_interpolation
+                    intg = Integration(interp)
+                    idx.compute(method='p-space')
+                    interp.compute(method='p-space')
+                    new_point, new_fvel, new_pvel = intg.compute_ppath(diameter=self.diameter,
+                                                                       density=self.density,
+                                                                       velocity=pvel, method='pRK4',
+                                                                       time_step=self.time_step,
+                                                                       drag_model=self.drag_model)
+                    if new_point is None:
+                        self.print_debug(self, 'Point out-of-domain. Integration complete!')
+                        break
+                    else:
+                        # Update the block in idx
+                        idx = Search(grid, new_point)
+                        idx.compute(method='c-space')
+                        self.streamline.append(new_point)
+                        self.fvelocity.append(new_fvel)
+                        self.svelocity.append(new_pvel)
+                        self.time.append(self.time_step)
+                        pvel = new_pvel.copy()
+                        fvel = new_fvel.copy()
+                        self.point = save_point
+                        save_point = new_point
+                else:
+
+                    # Check for mid-rk4 blowup
+                    if intg.rk4_bool is True:
+                        self.print_debug(self, 'Mid-RK4 blow up! Reducing time-step')
+                        intg.rk4_bool = False
+                        self.time_step = 0.5 * self.time_step
+                        loop_check += 1
+                        if loop_check == 70:
+                            self.print_debug(self, 'Stuck in the same loop for too long. Integration ends!')
+                            break
+
+                    else:
+                        self.point = save_point
+                        save_point = idx.c2p(new_point)
+                        self.streamline.append(save_point)
+                        self.fvelocity.append(new_fvel)
+                        self.svelocity.append(new_pvel)
+                        self.time.append(self.time_step)
+                        pvel = new_pvel.copy()
+                        fvel = new_fvel.copy()
+                        idx.point = new_point
+                        if loop_check > 0:
+                            self.print_debug(self, 'Resetting time step')
+                            self.time_step = self.time_step / (0.5 * loop_check)
+                            loop_check = 0
+
+            # Save files for each particle; can be used for multiprocessing large number of particles
+            self._save_data(self)
+            # t.stop()
+
+        if method == 'adaptive-ppath-c-space':
+            # t = Timer(text="Time taken for particle " + str(self.task) + " is {:.2f} seconds")
+            # t.start()
+            save_point = self.point
+            idx = Search(grid, self.point)
+            idx.compute(method='c-space')
+            while True:
+                interp = Interpolation(flow, idx)
+                interp.adaptive = self.adaptive_interpolation
+                interp.compute(method='c-space')
+                intg = Integration(interp)
+                new_point, new_fvel, new_pvel = intg.compute_ppath(diameter=self.diameter,
+                                                                   density=self.density,
+                                                                   velocity=pvel, method='cRK4',
+                                                                   time_step=self.time_step,
+                                                                   drag_model=self.drag_model)
+                # Check if the point is out-of-block
+                if new_point is None:
+                    # Check for large time-step
+                    self.print_debug(self, 'Checking if the end of the domain is reached...')
+                    self.time_step = 1e-9 * self.time_step
+                    new_point, new_fvel, new_pvel = intg.compute_ppath(diameter=self.diameter,
+                                                                       density=self.density,
+                                                                       velocity=pvel, method='cRK4',
+                                                                       time_step=self.time_step,
+                                                                       drag_model=self.drag_model)
+                    if new_point is not None:
+                        self.print_debug(self, 'Continuing integration by decreasing time-step!')
+                        continue
+                    # Check for out-of-block situation
+                    # For multi-block case if the point is out-of-block
+                    # Use previous point and run one-step of p-space algo
+                    elif new_point is None:
+                        self.print_debug(self, 'Point exited the block! Searching for new position...')
+                        idx = Search(grid, save_point)
+                        interp = Interpolation(flow, idx)
+                        interp.adaptive = self.adaptive_interpolation
+                        intg = Integration(interp)
+                        idx.compute(method='p-space')
+                        interp.compute()
+                        new_point, new_fvel, new_pvel = intg.compute_ppath(diameter=self.diameter,
+                                                                           density=self.density,
+                                                                           velocity=pvel, method='pRK4',
+                                                                           time_step=self.time_step,
+                                                                           drag_model=self.drag_model)
+                        if new_point is None:
+                            self.print_debug(self, 'Point out-of-domain. Integration complete!')
+                            break
+                        else:
+                            # Update the block in idx
+                            idx = Search(grid, new_point)
+                            idx.compute(method='c-space')
+                            # new_point found is in p-space; so, append
+                            self.streamline.append(new_point)
+                            self.fvelocity.append(new_fvel)
+                            self.svelocity.append(new_pvel)
+                            self.time.append(self.time_step)
+                            pvel = new_pvel.copy()
+                            fvel = new_fvel.copy()
+                            self.point = save_point
+                            save_point = new_point
+                else:
+                    self.point = save_point
+                    save_point = idx.c2p(new_point)
+
+                    # Check for mid-rk4 blowup
+                    if intg.rk4_bool is True:
+                        self.print_debug(self, f'**WARNING** Large residual. Mid-RK4 blow up! Reducing time-step for particle number'
+                              f' - {self.task}')
+                        intg.rk4_bool = False
+                        self.time_step = 0.5 * self.time_step
+                        loop_check += 1
+                        if loop_check == 70:
+                            self.print_debug(self, 'Stuck in the same loop for too long. Integration ends!')
+                            break
+
+                    # Adaptive algorithm starts
+                    # Save results and adjust time-step
+                    # Details for the algorithm are provided in adaptive-ppath
+                    elif self.angle_btw(new_fvel, fvel) is None:
+                        self.print_debug(self, 'Increasing time step. Successive points are same')
+                        self.time_step = 2 * self.time_step
+                        loop_check += 1
+                        if loop_check == 70:
+                            self.print_debug(self, f'Successive points did not change for too long. Integration ends! for particle '
+                                  f'{self.task}')
+                            break
+                    elif self.angle_btw(new_fvel,
+                                        fvel) <= 0.1 * self.adaptivity and self.time_step <= self.max_time_step:
+                        self.point = save_point
+                        save_point = idx.c2p(new_point)
+                        self.streamline.append(save_point)
+                        self.fvelocity.append(new_fvel)
+                        self.svelocity.append(new_pvel)
+                        self.time.append(self.time_step)
+                        idx.point = new_point.copy()
+                        pvel = new_pvel.copy()
+                        fvel = new_fvel.copy()
+                        self.time_step = 2 * self.time_step
+                        loop_check = 0
+                    elif self.angle_btw(new_fvel, fvel) >= self.adaptivity and self.time_step >= 1e-12:
+                        self.time_step = 0.5 * self.time_step
+                    else:
+                        self.point = save_point
+                        save_point = idx.c2p(new_point)
+                        self.streamline.append(save_point)
+                        self.fvelocity.append(new_fvel)
+                        self.svelocity.append(new_pvel)
+                        self.time.append(self.time_step)
+                        idx.point = new_point.copy()
+                        pvel = new_pvel.copy()
+                        fvel = new_fvel.copy()
+                        loop_check = 0
+
+            # Save files for each particle; can be used for multiprocessing large number of particles
+            self._save_data(self)
+            # t.stop()
+
+        return
```

### Comparing `project-arrakis-0.1/src/test_cases/oblique_shock_data.py` & `project_arrakis-0.1.1/src/test_cases/oblique_shock_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,252 +1,219 @@
-# Class to calculate particle response across an oblique shock
-
-import numpy as np
-from scipy.optimize import newton
-from src.streamlines.stochastic_model import StochasticModel, Particle, SpawnLocations
-import matplotlib.pyplot as plt
-import os
-import glob
-
-
-# Create a class to calculate oblique shock properties from given mach and deflection angle
-class ObliqueShock:
-    """
-    Class to calculate oblique shock properties from given mach and deflection angle
-
-    ...
-
-    Attributes
-    ----------
-    Input :
-        mach : float
-            Mach number
-        deflection : float
-            Deflection angle in degrees
-        shock_angle : float
-            Shock angle in degrees
-    Output :
-        pressure_ratio : float
-            Pressure ratio across the shock
-        density_ratio : float
-            Density ratio across the shock
-        temperature_ratio : float
-            Temperature ratio across the shock
-
-
-    Methods
-    -------
-    oblique_shock_relation(_mach, _deflection, _shock_angle)
-        Oblique shock relations for given mach, deflection and theta
-    derivative(f, method='central', h=1e-7) -- static method
-        Compute the difference formula for f with step size h.
-    compute()
-        Calculate the oblique shock properties
-
-    Example:
-    >>> os = ObliqueShock()
-    >>> os.mach = 2.3
-    >>> os.deflection = 10
-    >>> os.compute()
-    >>> print(os.shock_angle)
-    [34.32642717 85.02615188]
-
-    """
-
-    def __init__(self, mach=None, deflection=None, shock_angle=None):
-        self.mach = mach
-        self.deflection = deflection
-        self.shock_angle = shock_angle
-        self.pressure_ratio = None
-        self.density_ratio = None
-        self.temperature_ratio = None
-        self.mach_ratio = None
-        self.gamma = 1.4
-        self.gas_constant = 287.058
-
-    def oblique_shock_relation(self, _mach, _deflection, _shock_angle):
-        """
-        Oblique shock relations for given mach, deflection and theta
-        Args:
-
-        Returns:
-            delta-theta-mach relation
-        """
-        return (_mach ** 2 * (self.gamma + np.cos(2 * _shock_angle)) + 2) * np.tan(_deflection) * \
-            np.tan(_shock_angle) - 2 * (_mach ** 2 * np.sin(_shock_angle) ** 2 - 1)
-
-    @staticmethod
-    def derivative(f, method='central', h=1e-7):
-        """Compute the difference formula for f with step size h.
-
-        Parameters
-        ----------
-        f : function
-            Vectorized function of one variable
-        method : string
-            Difference formula: 'forward', 'backward' or 'central'
-        h : number
-            Step size in difference formula
-
-        Returns
-        -------
-        function
-            Difference formula:
-                central: f(x+h) - f(x-h))/2h
-                forward: f(x+h) - f(x))/h
-                backward: f(x) - f(x-h))/h
-        """
-
-        if method == 'central':
-            return lambda x: (f(x + h) - f(x - h)) / (2 * h)
-        elif method == 'forward':
-            return lambda x: (f(x + h) - f(x)) / h
-        elif method == 'backward':
-            return lambda x: (f(x) - f(x - h)) / h
-        else:
-            raise ValueError("Method must be 'central', 'forward' or 'backward'.")
-
-    def compute(self):
-        # Use Newton-Raphson method to calculate the shock angle
-        # Compute the shock angle if mach and deflection are given
-        if self.mach is not None and self.deflection is not None:
-            self.deflection = np.radians(self.deflection)
-
-            f_shock_angle = lambda shock_angle: self.oblique_shock_relation(self.mach, self.deflection, shock_angle)
-            df_shock_angle = self.derivative(f_shock_angle)
-
-            self.shock_angle = newton(f_shock_angle, (0.5, 1.57), fprime=df_shock_angle)
-
-        # Calculate the pressure ratio
-        self.pressure_ratio = 1 + 2 * self.gamma / (self.gamma + 1) * (
-                self.mach ** 2 * np.sin(self.shock_angle) ** 2 - 1)
-
-        # Calculate the density ratio
-        self.density_ratio = (self.gamma + 1) * self.mach ** 2 * np.sin(self.shock_angle) ** 2 / \
-                             (2 + (self.gamma - 1) * self.mach ** 2 * np.sin(self.shock_angle) ** 2)
-
-        # Calculate the temperature ratio
-        self.temperature_ratio = self.pressure_ratio / self.density_ratio
-
-        # Calculate the mach ratio
-        self.mach_ratio = 1/self.mach * np.sqrt(
-            (1 + (self.gamma - 1) / 2 * self.mach ** 2 * np.sin(self.shock_angle) ** 2) /
-            (self.gamma * self.mach ** 2 * np.sin(self.shock_angle) ** 2 -
-             (self.gamma - 1) / 2)) / np.sin(self.shock_angle - self.deflection)
-
-        # Change the shock angle to degrees
-        self.shock_angle = np.degrees(self.shock_angle)
-        self.deflection = np.degrees(self.deflection)
-
-        return
-
-
-# class to create a grid and flow based on oblique shock properties
-class ObliqueShockData:
-    """
-    Class to create a grid and flow based on oblique shock properties
-    """
-    def __init__(self, oblique_shock=ObliqueShock()):
-        from src.io.plot3dio import GridIO
-        from src.io.plot3dio import FlowIO
-        self.oblique_shock = oblique_shock
-        self.nx_max = None
-        self.ny_max = None
-        self.nz_max = None
-        self.points = None
-        self.grid = GridIO('dummy')
-        self.flow = FlowIO('dummy')
-        self.shock_strength = 'weak'
-        self.inlet_temperature = None
-        self.inlet_density = None
-        self.inlet_pressure = None
-
-    def create_grid(self):
-        # create a structured grid from -nx_max to nx_max, 0 to ny_max, 0 to nz_max
-        # spacing is the grid spacing
-        _xx, _yy, _zz = np.meshgrid(np.linspace(-self.nx_max, self.nx_max, 2*self.points),
-                                    np.linspace(0, self.ny_max, self.points),
-                                    np.linspace(0, self.nz_max, 2), indexing='ij')
-        # Create a plot3dio similar object
-        # n-blocks - one for the current case
-        self.grid.nb = 1
-        # ni, nj, nk
-        self.grid.ni = np.array([2*self.points], dtype='i4')
-        self.grid.nj = np.array([self.points], dtype='i4')
-        self.grid.nk = np.array([2], dtype='i4')
-        # grd
-        # expand dimensions and stack along the last axis
-        self.grid.grd = np.stack((_xx[..., None], _yy[..., None], _zz[..., None]), axis=3)
-        # grd_min and grd_max - 2d array to match the rest of the code
-        self.grid.grd_min = np.array([[-self.nx_max, 0, 0]])
-        self.grid.grd_max = np.array([[self.nx_max, self.ny_max, self.nz_max]])
-
-        # compute metrics
-        from src.io.plot3dio import GridIO
-        GridIO.compute_metrics(self.grid)
-        return
-
-    def create_flow(self):
-        # Create a vector with density, shock-normal, shock-tangential, zero velocities, and energy
-        # Have pre-shock before x=0 and post-shock after
-        if self.shock_strength == 'weak':
-            self.oblique_shock.shock_angle = self.oblique_shock.shock_angle[0]
-            self.oblique_shock.density_ratio = self.oblique_shock.density_ratio[0]
-            self.oblique_shock.pressure_ratio = self.oblique_shock.pressure_ratio[0]
-            self.oblique_shock.temperature_ratio = self.oblique_shock.temperature_ratio[0]
-            self.oblique_shock.mach_ratio = self.oblique_shock.mach_ratio[0]
-        elif self.shock_strength == 'strong':
-            self.oblique_shock.shock_angle = self.oblique_shock.shock_angle[1]
-            self.oblique_shock.density_ratio = self.oblique_shock.density_ratio[1]
-            self.oblique_shock.pressure_ratio = self.oblique_shock.pressure_ratio[1]
-            self.oblique_shock.temperature_ratio = self.oblique_shock.temperature_ratio[1]
-            self.oblique_shock.mach_ratio = self.oblique_shock.mach_ratio[1]
-        # Compute inlet flow properties -- pre-shock
-        _density = self.inlet_density
-        _velocity = self.oblique_shock.mach * np.sqrt(self.oblique_shock.gamma * self.oblique_shock.gas_constant *
-                                                      self.inlet_temperature)
-        _x_velocity = _velocity * np.sin(np.radians(self.oblique_shock.shock_angle))
-        _y_velocity = _velocity * np.cos(np.radians(self.oblique_shock.shock_angle))
-        _z_velocity = 0
-        _energy = _density * (self.oblique_shock.gamma * self.inlet_temperature / (self.oblique_shock.gamma - 1)
-                              + 0.5 * (_x_velocity ** 2 + _y_velocity ** 2 + _z_velocity ** 2))
-        # _pre_shock properties
-        _pre_shock = np.array([_density, _x_velocity * _density, _y_velocity * _density, _z_velocity * _density,
-                               _energy])
-
-        # post-shock properties
-        _density_post = _density * self.oblique_shock.density_ratio
-        _velocity_post = self.oblique_shock.mach * self.oblique_shock.mach_ratio * np.sqrt(
-            self.oblique_shock.gamma * self.oblique_shock.gas_constant
-            * self.inlet_temperature * self.oblique_shock.temperature_ratio)
-        _x_velocity_post = _velocity_post * np.sin(np.radians(self.oblique_shock.shock_angle
-                                                              - self.oblique_shock.deflection))
-        _y_velocity_post = _velocity_post * np.cos(np.radians(self.oblique_shock.shock_angle
-                                                              - self.oblique_shock.deflection))
-        _z_velocity_post = 0
-        _energy_post = _density_post * (self.oblique_shock.gamma * self.inlet_temperature *
-                                        self.oblique_shock.temperature_ratio / (self.oblique_shock.gamma - 1)
-                                        + 0.5 * (_x_velocity_post ** 2 + _y_velocity_post ** 2 + _z_velocity_post ** 2))
-        _post_shock = np.array([_density_post, _x_velocity_post * _density_post, _y_velocity_post * _density_post,
-                                _z_velocity_post * _density_post, _energy_post])
-
-        # Create a vector with density, shock-normal, shock-tangential, zero velocities, and energy
-        # Have pre-shock before x=0 and post-shock after
-
-        # create plot3dio flow similar object
-        self.flow.nb = 1
-        # ni, nj, nk
-        self.flow.ni = np.array([2*self.points], dtype='i4')
-        self.flow.nj = np.array([self.points], dtype='i4')
-        self.flow.nk = np.array([2], dtype='i4')
-        # mach, aoa/alpha, re, t
-        self.flow.mach = self.oblique_shock.mach
-        self.flow.alpha = 0.0
-        self.flow.rey = (_density * _velocity * (self.grid.grd[1, 0, 0, 0, 0] - self.grid.grd[0, 0, 0, 0, 0])) / 1.8e-5
-        self.flow.t = 1.0
-        # flow
-        self.flow.q = np.zeros((self.flow.ni[0], self.flow.nj[0], self.flow.nk[0], 5, self.flow.nb), dtype='f8')
-        self.flow.q[:self.points, ...] = _pre_shock[..., None]
-        self.flow.q[self.points:, ...] = _post_shock[..., None]
-        return
-
-
+# Class to calculate particle response across an oblique shock
+
+import numpy as np
+from scipy.optimize import newton
+from src.streamlines.stochastic_model import StochasticModel, Particle, SpawnLocations
+import matplotlib.pyplot as plt
+import os
+import glob
+
+
+# Create a class to calculate oblique shock properties from given mach and deflection angle
+class ObliqueShock:
+    """
+    Class to calculate oblique shock properties from given mach and deflection angle
+
+    ...
+
+    Attributes
+    ----------
+    Input :
+        mach : float
+            Mach number
+        deflection : float
+            Deflection angle in degrees
+        shock_angle : float
+            Shock angle in degrees
+    Output :
+        pressure_ratio : float
+            Pressure ratio across the shock
+        density_ratio : float
+            Density ratio across the shock
+        temperature_ratio : float
+            Temperature ratio across the shock
+
+
+    Methods
+    -------
+    oblique_shock_relation(_mach, _deflection, _shock_angle)
+        Oblique shock relations for given mach, deflection and theta
+    derivative(f, method='central', h=1e-7) -- static method
+        Compute the difference formula for f with step size h.
+    compute()
+        Calculate the oblique shock properties
+
+    Example:
+    >>> os = ObliqueShock()
+    >>> os.mach = 2.3
+    >>> os.deflection = 10
+    >>> os.compute()
+    >>> print(os.shock_angle)
+    [34.32642717 85.02615188]
+
+    """
+
+    def __init__(self, mach=None, deflection=None, shock_angle=None):
+        self.mach = mach
+        self.deflection = deflection
+        self.shock_angle = shock_angle
+        self.pressure_ratio = None
+        self.density_ratio = None
+        self.temperature_ratio = None
+        self.mach_ratio = None
+        self.gamma = 1.4
+        self.gas_constant = 287.058
+
+    def compute(self):
+        # Use the cubic equation solver to find the shock angle
+        # Compute the shock angle if mach and deflection are given
+        if self.mach is not None and self.deflection is not None:
+            self.deflection = np.radians(self.deflection)
+
+            # calculate coefficients
+            A = self.mach ** 2 - 1
+            B = 0.5 * (self.gamma + 1) * self.mach ** 4 * np.tan(self.deflection)
+            C = (1 + 0.5 * (self.gamma + 1) * self.mach ** 2) * np.tan(self.deflection)
+            coeffs = [1, C, -A, (B - A * C)]
+
+            # roots of a cubic equation, two positive solutions
+            # (disregard the negative)
+            roots = np.array([r for r in np.roots(coeffs) if r > 0])
+
+            thetas = np.arctan(1 / roots)
+            self.shock_angle = np.array([np.min(thetas), np.max(thetas)])
+
+        # Calculate the pressure ratio
+        self.pressure_ratio = 1 + 2 * self.gamma / (self.gamma + 1) * (
+                self.mach ** 2 * np.sin(self.shock_angle) ** 2 - 1)
+
+        # Calculate the density ratio
+        self.density_ratio = (self.gamma + 1) * self.mach ** 2 * np.sin(self.shock_angle) ** 2 / \
+                             (2 + (self.gamma - 1) * self.mach ** 2 * np.sin(self.shock_angle) ** 2)
+
+        # Calculate the temperature ratio
+        self.temperature_ratio = self.pressure_ratio / self.density_ratio
+
+        # Calculate the mach ratio
+        self.mach_ratio = 1/self.mach * np.sqrt(
+            (1 + (self.gamma - 1) / 2 * self.mach ** 2 * np.sin(self.shock_angle) ** 2) /
+            (self.gamma * self.mach ** 2 * np.sin(self.shock_angle) ** 2 -
+             (self.gamma - 1) / 2)) / np.sin(self.shock_angle - self.deflection)
+
+        # Change the shock angle to degrees
+        self.shock_angle = np.degrees(self.shock_angle)
+        self.deflection = np.degrees(self.deflection)
+
+        return
+
+
+# class to create a grid and flow based on oblique shock properties
+class ObliqueShockData:
+    """
+    Class to create a grid and flow based on oblique shock properties
+    """
+    def __init__(self, oblique_shock=ObliqueShock()):
+        from src.io.plot3dio import GridIO
+        from src.io.plot3dio import FlowIO
+        self.oblique_shock = oblique_shock
+        self.nx_max = None
+        self.ny_max = None
+        self.nz_max = None
+        self.xpoints = None
+        self.ypoints = None
+        self.zpoints = None
+        self.grid = GridIO('dummy')
+        self.flow = FlowIO('dummy')
+        self.shock_strength = 'weak'
+        self.inlet_temperature = None
+        self.inlet_density = None
+
+    def create_grid(self):
+        # create a structured grid from -nx_max to nx_max, 0 to ny_max, 0 to nz_max
+        # spacing is the grid spacing
+        _xx, _yy, _zz = np.meshgrid(np.linspace(-self.nx_max, self.nx_max, 2*self.xpoints),
+                                    np.linspace(0, self.ny_max, self.ypoints),
+                                    np.linspace(0, self.nz_max, self.zpoints), indexing='ij')
+        # Create a plot3dio similar object
+        # n-blocks - one for the current case
+        self.grid.nb = 1
+        # ni, nj, nk
+        self.grid.ni = np.array([2*self.xpoints], dtype='i4')
+        self.grid.nj = np.array([self.ypoints], dtype='i4')
+        self.grid.nk = np.array([self.zpoints], dtype='i4')
+        # grd
+        # expand dimensions and stack along the last axis
+        self.grid.grd = np.stack((_xx[..., None], _yy[..., None], _zz[..., None]), axis=3)
+        # grd_min and grd_max - 2d array to match the rest of the code
+        self.grid.grd_min = np.array([[-self.nx_max, 0, 0]])
+        self.grid.grd_max = np.array([[self.nx_max, self.ny_max, self.nz_max]])
+
+        # compute metrics
+        from src.io.plot3dio import GridIO
+        GridIO.compute_metrics(self.grid)
+        return
+
+    def create_flow(self):
+        # Create a vector with density, shock-normal, shock-tangential, zero velocities, and energy
+        # Have pre-shock before x=0 and post-shock after
+        if self.shock_strength == 'weak':
+            self.oblique_shock.shock_angle = self.oblique_shock.shock_angle[0]
+            self.oblique_shock.density_ratio = self.oblique_shock.density_ratio[0]
+            self.oblique_shock.pressure_ratio = self.oblique_shock.pressure_ratio[0]
+            self.oblique_shock.temperature_ratio = self.oblique_shock.temperature_ratio[0]
+            self.oblique_shock.mach_ratio = self.oblique_shock.mach_ratio[0]
+        elif self.shock_strength == 'strong':
+            self.oblique_shock.shock_angle = self.oblique_shock.shock_angle[1]
+            self.oblique_shock.density_ratio = self.oblique_shock.density_ratio[1]
+            self.oblique_shock.pressure_ratio = self.oblique_shock.pressure_ratio[1]
+            self.oblique_shock.temperature_ratio = self.oblique_shock.temperature_ratio[1]
+            self.oblique_shock.mach_ratio = self.oblique_shock.mach_ratio[1]
+        # Compute inlet flow properties -- pre-shock
+        _density = self.inlet_density
+        _velocity = self.oblique_shock.mach * np.sqrt(self.oblique_shock.gamma * self.oblique_shock.gas_constant *
+                                                      self.inlet_temperature)
+        _x_velocity = _velocity * np.sin(np.radians(self.oblique_shock.shock_angle))
+        _y_velocity = _velocity * np.cos(np.radians(self.oblique_shock.shock_angle))
+        _z_velocity = 0
+        _energy = _density * (self.oblique_shock.gas_constant * self.inlet_temperature / (self.oblique_shock.gamma - 1)
+                              + 0.5 * _velocity**2)
+        # _pre_shock properties
+        _pre_shock = np.array([_density, _x_velocity * _density, _y_velocity * _density, _z_velocity * _density,
+                               _energy])
+
+        # post-shock properties
+        _density_post = _density * self.oblique_shock.density_ratio
+        _velocity_post = self.oblique_shock.mach * self.oblique_shock.mach_ratio * np.sqrt(
+            self.oblique_shock.gamma * self.oblique_shock.gas_constant
+            * self.inlet_temperature * self.oblique_shock.temperature_ratio)
+        _x_velocity_post = _velocity_post * np.sin(np.radians(self.oblique_shock.shock_angle
+                                                              - self.oblique_shock.deflection))
+        _y_velocity_post = _velocity_post * np.cos(np.radians(self.oblique_shock.shock_angle
+                                                              - self.oblique_shock.deflection))
+        _z_velocity_post = 0
+        _energy_post = _density_post * (self.oblique_shock.gas_constant * self.inlet_temperature *
+                                        self.oblique_shock.temperature_ratio / (self.oblique_shock.gamma - 1)
+                                        + 0.5 * _velocity_post**2)
+        _post_shock = np.array([_density_post, _x_velocity_post * _density_post, _y_velocity_post * _density_post,
+                                _z_velocity_post * _density_post, _energy_post])
+
+        # Create a vector with density, shock-normal, shock-tangential, zero velocities, and energy
+        # Have pre-shock before x=0 and post-shock after
+
+        # create plot3dio flow similar object
+        self.flow.nb = 1
+        # ni, nj, nk
+        self.flow.ni = np.array([2*self.xpoints], dtype='i4')
+        self.flow.nj = np.array([self.ypoints], dtype='i4')
+        self.flow.nk = np.array([self.zpoints], dtype='i4')
+        # mach, aoa/alpha, re, t
+        self.flow.mach = self.oblique_shock.mach
+        self.flow.alpha = 0.0
+        self.flow.rey = (_density * _velocity * (self.grid.grd[1, 0, 0, 0, 0] - self.grid.grd[0, 0, 0, 0, 0])) / 1.8e-5
+        self.flow.time = 1.0
+        # flow
+        self.flow.q = np.zeros((self.flow.ni[0], self.flow.nj[0], self.flow.nk[0], 5, self.flow.nb), dtype='f8')
+        self.flow.q[:self.xpoints, ...] = _pre_shock[..., None]
+        self.flow.q[self.xpoints:, ...] = _post_shock[..., None]
+        return
+
+
```

### Comparing `project-arrakis-0.1/test/test_dataio.py` & `project_arrakis-0.1.1/test/test_dataio.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-import unittest
-
-
-class TestDataIO(unittest.TestCase):
-    def test_dataio(self):
-        from src.io.dataio import DataIO
-        from src.io.plot3dio import GridIO, FlowIO
-        # grid object
-        grid = GridIO('../data/shocks/shock_test.sb.sp.x')
-        grid.read_grid()
-        grid.compute_metrics()
-
-        # flow object
-        flow = FlowIO('../data/shocks/shock_test.sb.sp.q')
-        flow.read_flow()
-
-        # data module test
-        # data = DataIO(grid, flow, location='../data/shocks/particle_data/multi_process_test/')
-        data = DataIO(grid, flow, location='../data/shocks/particle_data/281nm_time_step_adaptive/',
-                      read_file='../data/shocks/particle_data/281nm_time_step_adaptive/combined_file.npy')
-        # Increased refinement for better resolution
-        data.x_refinement = 500
-        data.y_refinement = 400
-        data.compute()
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+
+
+class TestDataIO(unittest.TestCase):
+    def test_dataio(self):
+        from src.io.dataio import DataIO
+        from src.io.plot3dio import GridIO, FlowIO
+        # grid object
+        grid = GridIO('../data/shocks/shock_test.sb.sp.x')
+        grid.read_grid()
+        grid.compute_metrics()
+
+        # flow object
+        flow = FlowIO('../data/shocks/shock_test.sb.sp.q')
+        flow.read_flow()
+
+        # data module test
+        # data = DataIO(grid, flow, location='../data/shocks/particle_data/multi_process_test/')
+        data = DataIO(grid, flow, location='../data/shocks/particle_data/281nm_time_step_adaptive/old_data/',
+                      read_file='../data/shocks/particle_data/281nm_time_step_adaptive/old_data/combined_file.npy')
+        data.percent_data = 0.1
+        # Increased refinement for better resolution
+        data.x_refinement = 500
+        data.y_refinement = 400
+        data.compute()
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `project-arrakis-0.1/test/test_import.py` & `project_arrakis-0.1.1/test/test_import.py`

 * *Files identical despite different names*

### Comparing `project-arrakis-0.1/test/test_integration.py` & `project_arrakis-0.1.1/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `project-arrakis-0.1/test/test_plot.py` & `project_arrakis-0.1.1/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `project-arrakis-0.1/test/test_plot3dio.py` & `project_arrakis-0.1.1/test/test_plot3dio.py`

 * *Files identical despite different names*

### Comparing `project-arrakis-0.1/test/test_stochastic_model.py` & `project_arrakis-0.1.1/test/test_stochastic_model.py`

 * *Files identical despite different names*

### Comparing `project-arrakis-0.1/test/test_terminal_run.py` & `project_arrakis-0.1.1/test/test_terminal_run.py`

 * *Files identical despite different names*

### Comparing `project-arrakis-0.1/test/test_variables.py` & `project_arrakis-0.1.1/test/test_variables.py`

 * *Files identical despite different names*

