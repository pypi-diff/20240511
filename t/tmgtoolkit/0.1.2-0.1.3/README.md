# Comparing `tmp/tmgtoolkit-0.1.2.tar.gz` & `tmp/tmgtoolkit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmgtoolkit-0.1.2.tar", last modified: Wed Apr 17 09:41:06 2024, max compression
+gzip compressed data, was "tmgtoolkit-0.1.3.tar", last modified: Sat May 11 19:40:47 2024, max compression
```

## Comparing `tmgtoolkit-0.1.2.tar` & `tmgtoolkit-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-17 09:41:06.606380 tmgtoolkit-0.1.2/
--rw-r--r--   0 ej        (1000) wheel      (998)    34916 2024-04-10 06:55:31.000000 tmgtoolkit-0.1.2/LICENSE.md
--rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-04-17 09:41:06.606380 tmgtoolkit-0.1.2/PKG-INFO
--rw-r--r--   0 ej        (1000) wheel      (998)      563 2024-04-10 07:01:19.000000 tmgtoolkit-0.1.2/README.md
--rw-r--r--   0 ej        (1000) wheel      (998)      103 2024-04-10 07:09:13.000000 tmgtoolkit-0.1.2/pyproject.toml
--rw-r--r--   0 ej        (1000) wheel      (998)      754 2024-04-17 09:41:06.606380 tmgtoolkit-0.1.2/setup.cfg
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-17 09:41:06.603046 tmgtoolkit-0.1.2/src/
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-17 09:41:06.603046 tmgtoolkit-0.1.2/src/tmgtoolkit/
--rw-r--r--   0 ej        (1000) wheel      (998)        0 2024-04-09 14:32:51.000000 tmgtoolkit-0.1.2/src/tmgtoolkit/__init__.py
--rw-r--r--   0 ej        (1000) wheel      (998)     3298 2024-04-17 08:36:30.000000 tmgtoolkit-0.1.2/src/tmgtoolkit/constants.py
--rw-r--r--   0 ej        (1000) wheel      (998)    16033 2024-04-10 20:05:19.000000 tmgtoolkit-0.1.2/src/tmgtoolkit/plotting.py
--rw-r--r--   0 ej        (1000) wheel      (998)    14809 2024-04-17 08:36:20.000000 tmgtoolkit-0.1.2/src/tmgtoolkit/spm.py
--rw-r--r--   0 ej        (1000) wheel      (998)    18630 2024-04-12 13:27:22.000000 tmgtoolkit-0.1.2/src/tmgtoolkit/time_series.py
--rw-r--r--   0 ej        (1000) wheel      (998)     3283 2024-04-13 07:30:15.000000 tmgtoolkit-0.1.2/src/tmgtoolkit/tmgio.py
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-17 09:41:06.606380 tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/
--rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-04-17 09:41:06.000000 tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 ej        (1000) wheel      (998)      410 2024-04-17 09:41:06.000000 tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 ej        (1000) wheel      (998)        1 2024-04-17 09:41:06.000000 tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 ej        (1000) wheel      (998)       50 2024-04-17 09:41:06.000000 tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/requires.txt
--rw-r--r--   0 ej        (1000) wheel      (998)       11 2024-04-17 09:41:06.000000 tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-04-17 09:41:06.606380 tmgtoolkit-0.1.2/tests/
--rw-r--r--   0 ej        (1000) wheel      (998)       85 2024-04-17 09:39:29.000000 tmgtoolkit-0.1.2/tests/test_mwe.py
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-11 19:40:47.958154 tmgtoolkit-0.1.3/
+-rw-r--r--   0 ej        (1000) wheel      (998)    34916 2024-04-10 06:55:31.000000 tmgtoolkit-0.1.3/LICENSE.md
+-rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-05-11 19:40:47.958154 tmgtoolkit-0.1.3/PKG-INFO
+-rw-r--r--   0 ej        (1000) wheel      (998)      563 2024-04-10 07:01:19.000000 tmgtoolkit-0.1.3/README.md
+-rw-r--r--   0 ej        (1000) wheel      (998)      103 2024-04-10 07:09:13.000000 tmgtoolkit-0.1.3/pyproject.toml
+-rw-r--r--   0 ej        (1000) wheel      (998)      754 2024-05-11 19:40:47.958154 tmgtoolkit-0.1.3/setup.cfg
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-11 19:40:47.951487 tmgtoolkit-0.1.3/src/
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-11 19:40:47.954821 tmgtoolkit-0.1.3/src/tmgtoolkit/
+-rw-r--r--   0 ej        (1000) wheel      (998)        0 2024-04-09 14:32:51.000000 tmgtoolkit-0.1.3/src/tmgtoolkit/__init__.py
+-rw-r--r--   0 ej        (1000) wheel      (998)     5159 2024-05-11 14:14:37.000000 tmgtoolkit-0.1.3/src/tmgtoolkit/constants.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    16033 2024-05-10 15:04:33.000000 tmgtoolkit-0.1.3/src/tmgtoolkit/plotting.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    13745 2024-05-10 15:04:51.000000 tmgtoolkit-0.1.3/src/tmgtoolkit/spm.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    18630 2024-04-28 11:37:20.000000 tmgtoolkit-0.1.3/src/tmgtoolkit/time_series.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    11910 2024-05-11 14:13:54.000000 tmgtoolkit-0.1.3/src/tmgtoolkit/tmgio.py
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-11 19:40:47.954821 tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/
+-rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-05-11 19:40:47.000000 tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 ej        (1000) wheel      (998)      410 2024-05-11 19:40:47.000000 tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 ej        (1000) wheel      (998)        1 2024-05-11 19:40:47.000000 tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 ej        (1000) wheel      (998)       50 2024-05-11 19:40:47.000000 tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/requires.txt
+-rw-r--r--   0 ej        (1000) wheel      (998)       11 2024-05-11 19:40:47.000000 tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-11 19:40:47.954821 tmgtoolkit-0.1.3/tests/
+-rw-r--r--   0 ej        (1000) wheel      (998)       85 2024-04-17 09:39:29.000000 tmgtoolkit-0.1.3/tests/test_mwe.py
```

### Comparing `tmgtoolkit-0.1.2/LICENSE.md` & `tmgtoolkit-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.2/PKG-INFO` & `tmgtoolkit-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmgtoolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: Time series analysis of tensiomyography (TMG) data
 Home-page: https://github.com/ejmastnak/tmgtoolkit
 Author: Elijan Mastnak
 Author-email: admin@ejmastnak.com
 Project-URL: Bug Tracker, https://github.com/ejmastnak/tmgtoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tmgtoolkit-0.1.2/README.md` & `tmgtoolkit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.2/setup.cfg` & `tmgtoolkit-0.1.3/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tmgtoolkit
-version = 0.1.2
+version = 0.1.3
 author = Elijan Mastnak
 author_email = admin@ejmastnak.com
 description = Time series analysis of tensiomyography (TMG) data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejmastnak/tmgtoolkit
 project_urls =
```

### Comparing `tmgtoolkit-0.1.2/src/tmgtoolkit/plotting.py` & `tmgtoolkit-0.1.3/src/tmgtoolkit/plotting.py`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.2/src/tmgtoolkit/spm.py` & `tmgtoolkit-0.1.3/src/tmgtoolkit/spm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections import namedtuple
 import numpy as np
 import spm1d
 
 from .constants import SpmConstants, NamedTupleTypes
 from .time_series import _idx_to_time, _interpolate_extremum
 
-def get_spm_t_statistic(group1, group2, mitigate_iir_filter_artefact=True):
+def get_spm_t_statistic(group1, group2, mitigate_iir_filter_artefact=True, swap_groups=False):
     """Computes SPM t-test statistic for the inputted data.
 
     Returns an SpmTStatistic namedtuple containing the 1D SPM t-test statistic
     resulting from a paired SPM t-test comparing the time series data in the
     inputted arrays `group1` and `group2`. The returned SPM t-statistic is
     implicitly defined on the same time (or other independent variable) grid as
     the time series in `group1` and `group2`, but it is up to the calling code
@@ -24,24 +24,31 @@
         (points_per_series, number_of_series).
     group2 : ndarray
         2D Numpy array holding at least two time series, to be compared to the
         set of time series in `group1`. The number of time series in `group2`
         may be different from the number of time series in `group1`, but the
         length of the time series in `group1` and `group2` should be equal
         (i.e. `group1` and `group2` should have the same number of rows).
-    mitigate_iir_filter_artefact : bool
+    mitigate_iir_filter_artefact : bool, optional
         If True, passes data through `_mitigate_iir_filter_artefact` before
         computing the SPM t-statistic. See `_mitigate_iir_filter_artefact` for
         details.
+    swap_groups : bool, optional
+        Controls the order in which `group1` and `group2` are passed to spm1d's
+        paired t-test function. This can be useful e.g. if client wants to
+        manipulate which group is treated as "potentiated".
 
     Pre-Conditions
     --------------
-    No row in `group1` or in `group2` can have all equal values—this is to
-    ensure there are no rows in the inputted data with zero variance, which
-    would cause a divide by zero error when computing the SPM t-statistic.
+    1. `group1` and `group2` must have the same shape—this is a requirement for
+       further analysis by spm1d.
+    2. No row in `group1` or in `group2` can have all equal values—this is to
+       ensure there are no rows in the inputted data with zero variance, which
+       would cause a divide by zero error when computing the SPM t-statistic.
+       This is again a requirement for further analysis by spm1d.
 
     Note on time values: although the time (or other independent variable)
     values on which `group1` and `group2` are defined are not needed to compute
     the SPM t-statistic, `group1` and `group2` should conceptually be defined
     on the same time grid; this becomes relevant when performing inference on
     the t-statistic returned by this function.
 
@@ -60,18 +67,23 @@
               `group1` and `group2` have different lengths).
         - `spm_t` (spm1d._spm.SPM_T): wrapper object for the t-statistic used
             by the spm1d library. Meant for internal use only and subject to
             change in future versions.
         Access fields with e.g. `spm_ts.t_statistic`.
 
     """
+    if group1.shape != group2.shape:
+        raise ValueError("Group 1 and Group 2 must have the same shape, but have shapes {} and {}.".format(group1.shape, group2.shape))
+
     if mitigate_iir_filter_artefact:
         group1, group2 = _mitigate_iir_filter_artefact(group1, group2)
-    group1, group2 = _equalize_columns(group1, group2)
-    spm_t = spm1d.stats.ttest_paired(group1.T, group2.T)
+    if swap_groups:
+        spm_t = spm1d.stats.ttest_paired(group2.T, group1.T)
+    else:
+        spm_t = spm1d.stats.ttest_paired(group1.T, group2.T)
     return NamedTupleTypes.SpmTStatistic(t_statistic=spm_t.z, spm_t=spm_t)
 
 
 def get_spm_t_inference(spm_ts, t=None, alpha=0.05, two_tailed=True):
     """Performs SPM inference on the inputted SPM t-statistic data.
 
     Returns an SpmTInference namedtuple holding the results of performing
@@ -190,64 +202,14 @@
     if mean2 > mean1:
         group2 = group2 - np.mean(mean2 - mean1)
     else:
         group1 = group1 - np.mean(mean1 - mean2)
     return (group1, group2)
 
 
-def _equalize_columns(group1, group2):
-    """Ensures inputted 2D arrays have the same number of columns.
-
-    Context: 2D arrays inputted to `spm1d`'s analysis functions require that
-    the arrays have the same number of rows and columns. This function
-    equalizes the number of columns in the inputted data, if necessary, so that
-    the data can be analyzed with `spm1d`.
-
-    The function works by computing the mean of the array with fewer columns,
-    and repeatedly appending this mean column to the array with fewer columns
-    until the number of columns in `group1` and `group2` are equal.
-
-    Parameters
-    ----------
-    group1 : ndarray
-        2D Numpy array holding at least two time series, as for
-        `get_spm_t_statistic`.
-    group2 : ndarray
-        2D Numpy array holding at least two time series, as for
-        `get_spm_t_statistic`.
-
-    Returns
-    -------
-    group_tuple : tuple
-        Tuple holding equalized versions of `group1` and `group2`; fields are
-        0. `group1` (ndarray)
-        1. `group2` (ndarray)
-    """
-    rows = group1.shape[0]
-    cols1 = group1.shape[1]
-    cols2 = group2.shape[1]
-    if cols1 == cols2:
-        return (group1, group2)
-
-    elif cols1 < cols2:
-        padded_group1 = np.zeros((rows, cols2))
-        padded_group1[:, 0:cols1] = group1
-        mean1 = np.mean(group1, axis=1)
-        for c in range(cols1, cols2):
-            padded_group1[:, c] = mean1
-        return (padded_group1, group2)
-    elif cols2 < cols1:
-        padded_group2 = np.zeros((rows, cols1))
-        padded_group2[:, 0:cols2] = group2
-        mean2 = np.mean(group2, axis=1)
-        for c in range(cols2, cols1):
-            padded_group2[:, c] = mean2
-        return (group1, padded_group2)
-
-
 def _get_spm_clusters(spm_ti, t):
     """Returns information describing an SPM inference object's clusters.
 
     Returns a list of SpmCluster namedtuples summarizing the supra-threshold
     clusters in the SPM inference object `spm_ti`.
 
     Parameters
```

### Comparing `tmgtoolkit-0.1.2/src/tmgtoolkit/time_series.py` & `tmgtoolkit-0.1.3/src/tmgtoolkit/time_series.py`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.2/src/tmgtoolkit.egg-info/PKG-INFO` & `tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmgtoolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: Time series analysis of tensiomyography (TMG) data
 Home-page: https://github.com/ejmastnak/tmgtoolkit
 Author: Elijan Mastnak
 Author-email: admin@ejmastnak.com
 Project-URL: Bug Tracker, https://github.com/ejmastnak/tmgtoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

