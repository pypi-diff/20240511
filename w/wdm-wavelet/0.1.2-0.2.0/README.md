# Comparing `tmp/wdm_wavelet-0.1.2.tar.gz` & `tmp/wdm_wavelet-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wdm_wavelet-0.1.2.tar", last modified: Sat May 11 08:51:14 2024, max compression
+gzip compressed data, was "wdm_wavelet-0.2.0.tar", last modified: Sat May 11 08:51:14 2024, max compression
```

## Comparing `wdm_wavelet-0.1.2.tar` & `wdm_wavelet-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.017217 wdm_wavelet-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    35065 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/Makefile
--rw-r--r--   0 root         (0) root         (0)      642 2024-05-11 08:51:14.017217 wdm_wavelet-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.014217 wdm_wavelet-0.1.2/notebook/
--rw-rw-rw-   0 root         (0) root         (0)   164420 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/notebook/transform_GW.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      566 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 08:51:14.017217 wdm_wavelet-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1622 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.015217 wdm_wavelet-0.1.2/test/
--rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/test/test_wdm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.015217 wdm_wavelet-0.1.2/wdm_wavelet/
--rw-rw-rw-   0 root         (0) root         (0)      133 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/wdm_wavelet/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-05-11 08:51:13.000000 wdm_wavelet-0.1.2/wdm_wavelet/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.016217 wdm_wavelet-0.1.2/wdm_wavelet/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/wdm_wavelet/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/wdm_wavelet/core/get_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2444 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/wdm_wavelet/core/t2w.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/wdm_wavelet/core/w2t.py
--rw-rw-rw-   0 root         (0) root         (0)   106583 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/wdm_wavelet/fourier_coeff.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.017217 wdm_wavelet-0.1.2/wdm_wavelet/types/
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/wdm_wavelet/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2656 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/wdm_wavelet/types/time_frequency_map.py
--rw-rw-rw-   0 root         (0) root         (0)     2928 2024-05-11 08:51:08.000000 wdm_wavelet-0.1.2/wdm_wavelet/wdm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.017217 wdm_wavelet-0.1.2/wdm_wavelet.egg-info/
--rw-r--r--   0 root         (0) root         (0)      642 2024-05-11 08:51:13.000000 wdm_wavelet-0.1.2/wdm_wavelet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      569 2024-05-11 08:51:14.000000 wdm_wavelet-0.1.2/wdm_wavelet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 08:51:13.000000 wdm_wavelet-0.1.2/wdm_wavelet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-11 08:51:13.000000 wdm_wavelet-0.1.2/wdm_wavelet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-11 08:51:13.000000 wdm_wavelet-0.1.2/wdm_wavelet.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.428219 wdm_wavelet-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    35065 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)      642 2024-05-11 08:51:14.428219 wdm_wavelet-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.425219 wdm_wavelet-0.2.0/notebook/
+-rw-rw-rw-   0 root         (0) root         (0)   164420 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/notebook/transform_GW.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      566 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 08:51:14.428219 wdm_wavelet-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.425219 wdm_wavelet-0.2.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/test/test_wdm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.426219 wdm_wavelet-0.2.0/wdm_wavelet/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/wdm_wavelet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-11 08:51:14.000000 wdm_wavelet-0.2.0/wdm_wavelet/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.427219 wdm_wavelet-0.2.0/wdm_wavelet/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/wdm_wavelet/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/wdm_wavelet/core/get_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/wdm_wavelet/core/t2w.py
+-rw-rw-rw-   0 root         (0) root         (0)     2021 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/wdm_wavelet/core/w2t.py
+-rw-rw-rw-   0 root         (0) root         (0)   106583 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/wdm_wavelet/fourier_coeff.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.427219 wdm_wavelet-0.2.0/wdm_wavelet/types/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/wdm_wavelet/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2813 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/wdm_wavelet/types/time_frequency_map.py
+-rw-rw-rw-   0 root         (0) root         (0)     3494 2024-05-11 08:51:08.000000 wdm_wavelet-0.2.0/wdm_wavelet/wdm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 08:51:14.427219 wdm_wavelet-0.2.0/wdm_wavelet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      642 2024-05-11 08:51:14.000000 wdm_wavelet-0.2.0/wdm_wavelet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      569 2024-05-11 08:51:14.000000 wdm_wavelet-0.2.0/wdm_wavelet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 08:51:14.000000 wdm_wavelet-0.2.0/wdm_wavelet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-11 08:51:14.000000 wdm_wavelet-0.2.0/wdm_wavelet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-11 08:51:14.000000 wdm_wavelet-0.2.0/wdm_wavelet.egg-info/top_level.txt
```

### Comparing `wdm_wavelet-0.1.2/.gitlab-ci.yml` & `wdm_wavelet-0.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `wdm_wavelet-0.1.2/LICENSE` & `wdm_wavelet-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wdm_wavelet-0.1.2/PKG-INFO` & `wdm_wavelet-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wdm-wavelet
-Version: 0.1.2
+Version: 0.2.0
 Summary: A Python package for Wilson-Daubechies-Meyer (WDM) wavelet from coherentWaveBurst
 Home-page: https://git.ligo.org/yumeng.xu/setup.py
 Author: Yumeng Xu
 Author-email: The PycWB team <yumeng.xu@ligo.org>
 Keywords: ligo,wavelet,gravitational waves,burst,DWT,WDM,Wilson-Daubechies-Meyer,cWB
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `wdm_wavelet-0.1.2/notebook/transform_GW.ipynb` & `wdm_wavelet-0.2.0/notebook/transform_GW.ipynb`

 * *Files identical despite different names*

### Comparing `wdm_wavelet-0.1.2/pyproject.toml` & `wdm_wavelet-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wdm_wavelet-0.1.2/setup.py` & `wdm_wavelet-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `wdm_wavelet-0.1.2/wdm_wavelet/core/get_filter.py` & `wdm_wavelet-0.2.0/wdm_wavelet/core/get_filter.py`

 * *Files identical despite different names*

### Comparing `wdm_wavelet-0.1.2/wdm_wavelet/core/t2w.py` & `wdm_wavelet-0.2.0/wdm_wavelet/core/t2w.py`

 * *Files identical despite different names*

### Comparing `wdm_wavelet-0.1.2/wdm_wavelet/fourier_coeff.py` & `wdm_wavelet-0.2.0/wdm_wavelet/fourier_coeff.py`

 * *Files identical despite different names*

### Comparing `wdm_wavelet-0.1.2/wdm_wavelet/types/time_frequency_map.py` & `wdm_wavelet-0.2.0/wdm_wavelet/types/time_frequency_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,25 @@
         Complex Time-frequency map data
     df: float
         Frequency resolution
     dt: float
         Time resolution
     t0: float
         Start time
+    len_timeseries: int
+        Length of the converted time series
+    wdm_params: dict
+        WDM parameters
     """
     data: np.ndarray
     df: float
     dt: float
     t0: float
+    len_timeseries: int
+    wdm_params: dict
 
     @property
     def n_freq(self):
         """
         Number of frequency bins
 
         Returns
```

### Comparing `wdm_wavelet-0.1.2/wdm_wavelet/wdm.py` & `wdm_wavelet-0.2.0/wdm_wavelet/wdm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import numpy as np
+
 from .core.get_filter import get_filter
 from .core.t2w import t2w
+from .core.w2t import w2t
 from .fourier_coeff import load_fourier_coeff
 from gwpy.timeseries import TimeSeries
 from wdm_wavelet.types import TimeFrequencyMap
 
 
 class WDM:
     """
@@ -68,23 +71,36 @@
                                  "but the sample_rate or start_time cannot be extracted")
         else:
             if sample_rate is None:
                 raise ValueError("sample_rate must be provided if strain is not"
                                  " a gwpy.TimeSeries object or a pycbc.TimeSeries object")
 
         # calculate the time frequency map
-        _, _, time_frequency_map = t2w(self.M, self.m_H, strain, self.filter, MM)
+        _, len_timeseries, time_frequency_map = t2w(self.M, self.m_H, strain, self.filter, MM)
 
         # calculate the df and dt
         max_f_layer = time_frequency_map.shape[2] - 1
         max_t_layer = time_frequency_map.shape[1]
         df = sample_rate/max_f_layer/2.
 
         t_len = len(strain) / sample_rate
         dt = t_len/max_t_layer
 
-        time_frequency_map = time_frequency_map[0] - 1j * time_frequency_map[1]
+        time_frequency_map = time_frequency_map[0] + 1j * time_frequency_map[1]
 
-        return TimeFrequencyMap(time_frequency_map.T, df, dt, t0)
+        return TimeFrequencyMap(time_frequency_map.T, df, dt, t0, len_timeseries, self.params)
 
-    def w2t(self):
-        raise NotImplementedError("w2t is not implemented yet")
+    def w2t(self, time_frequency_map):
+        data = np.array([time_frequency_map.data.real.T, time_frequency_map.data.imag.T]).flatten()
+        t = w2t(data, time_frequency_map.n_freq, self.filter)
+
+        sample_rate = 2 * time_frequency_map.df * (time_frequency_map.n_freq - 1)
+        return TimeSeries(t, sample_rate=sample_rate, t0=time_frequency_map.t0)
+
+    @property
+    def params(self):
+        return {
+            "M": self.M,
+            "K": self.K,
+            "beta_order": self.beta_order,
+            "precision": self.precision
+        }
```

### Comparing `wdm_wavelet-0.1.2/wdm_wavelet.egg-info/PKG-INFO` & `wdm_wavelet-0.2.0/wdm_wavelet.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wdm-wavelet
-Version: 0.1.2
+Version: 0.2.0
 Summary: A Python package for Wilson-Daubechies-Meyer (WDM) wavelet from coherentWaveBurst
 Home-page: https://git.ligo.org/yumeng.xu/setup.py
 Author: Yumeng Xu
 Author-email: The PycWB team <yumeng.xu@ligo.org>
 Keywords: ligo,wavelet,gravitational waves,burst,DWT,WDM,Wilson-Daubechies-Meyer,cWB
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `wdm_wavelet-0.1.2/wdm_wavelet.egg-info/SOURCES.txt` & `wdm_wavelet-0.2.0/wdm_wavelet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

