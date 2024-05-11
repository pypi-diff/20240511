# Comparing `tmp/symclosestwannier-1.1.8.tar.gz` & `tmp/symclosestwannier-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symclosestwannier-1.1.8.tar", last modified: Thu Feb  1 04:44:21 2024, max compression
+gzip compressed data, was "symclosestwannier-1.1.9.tar", last modified: Sun Feb  4 15:55:13 2024, max compression
```

## Comparing `symclosestwannier-1.1.8.tar` & `symclosestwannier-1.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-01 04:44:21.327378 symclosestwannier-1.1.8/
--rw-r--r--   0 ro         (501) staff       (20)    18092 2023-12-19 03:50:00.000000 symclosestwannier-1.1.8/LICENSE
--rw-r--r--   0 ro         (501) staff       (20)       57 2023-12-19 03:46:59.000000 symclosestwannier-1.1.8/MANIFEST.in
--rw-r--r--   0 ro         (501) staff       (20)     2542 2024-02-01 04:44:21.327290 symclosestwannier-1.1.8/PKG-INFO
--rw-r--r--   0 ro         (501) staff       (20)     1805 2023-12-19 03:54:41.000000 symclosestwannier-1.1.8/README.md
--rw-r--r--   0 ro         (501) staff       (20)      887 2024-02-01 04:44:21.327817 symclosestwannier-1.1.8/setup.cfg
--rw-r--r--   0 ro         (501) staff       (20)       38 2023-12-19 03:47:00.000000 symclosestwannier-1.1.8/setup.py
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-01 04:44:21.316014 symclosestwannier-1.1.8/symclosestwannier/
--rw-r--r--   0 ro         (501) staff       (20)      106 2024-02-01 04:44:14.000000 symclosestwannier-1.1.8/symclosestwannier/__init__.py
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-01 04:44:21.320351 symclosestwannier-1.1.8/symclosestwannier/analyzer/
--rw-r--r--   0 ro         (501) staff       (20)     3455 2024-01-22 00:23:53.000000 symclosestwannier-1.1.8/symclosestwannier/analyzer/analyzer.py
--rw-r--r--   0 ro         (501) staff       (20)     4715 2023-12-19 03:50:00.000000 symclosestwannier-1.1.8/symclosestwannier/analyzer/band.py
--rw-r--r--   0 ro         (501) staff       (20)     1779 2023-12-19 03:50:00.000000 symclosestwannier-1.1.8/symclosestwannier/analyzer/get_band.py
--rw-r--r--   0 ro         (501) staff       (20)    19167 2024-01-31 10:51:59.000000 symclosestwannier-1.1.8/symclosestwannier/analyzer/get_response.py
--rw-r--r--   0 ro         (501) staff       (20)     9472 2024-02-01 04:44:14.000000 symclosestwannier-1.1.8/symclosestwannier/analyzer/response.py
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-01 04:44:21.324104 symclosestwannier-1.1.8/symclosestwannier/cw/
--rw-r--r--   0 ro         (501) staff       (20)     2807 2024-01-24 13:49:38.000000 symclosestwannier-1.1.8/symclosestwannier/cw/amn.py
--rw-r--r--   0 ro         (501) staff       (20)     8519 2024-01-31 15:04:58.000000 symclosestwannier-1.1.8/symclosestwannier/cw/cw_creator.py
--rw-r--r--   0 ro         (501) staff       (20)     7135 2024-01-16 01:16:37.000000 symclosestwannier-1.1.8/symclosestwannier/cw/cw_info.py
--rw-r--r--   0 ro         (501) staff       (20)     5529 2023-12-19 03:50:00.000000 symclosestwannier-1.1.8/symclosestwannier/cw/cw_manager.py
--rw-r--r--   0 ro         (501) staff       (20)    39644 2024-02-01 04:44:14.000000 symclosestwannier-1.1.8/symclosestwannier/cw/cw_model.py
--rw-r--r--   0 ro         (501) staff       (20)     7628 2024-01-22 00:23:53.000000 symclosestwannier-1.1.8/symclosestwannier/cw/cwin.py
--rw-r--r--   0 ro         (501) staff       (20)     3336 2024-01-31 04:41:33.000000 symclosestwannier-1.1.8/symclosestwannier/cw/eig.py
--rw-r--r--   0 ro         (501) staff       (20)     5161 2024-01-31 04:41:33.000000 symclosestwannier-1.1.8/symclosestwannier/cw/mmn.py
--rw-r--r--   0 ro         (501) staff       (20)    11004 2024-01-31 04:41:33.000000 symclosestwannier-1.1.8/symclosestwannier/cw/nnkp.py
--rw-r--r--   0 ro         (501) staff       (20)     5985 2023-12-19 03:50:00.000000 symclosestwannier-1.1.8/symclosestwannier/cw/spn.py
--rw-r--r--   0 ro         (501) staff       (20)     9558 2024-02-01 04:44:14.000000 symclosestwannier-1.1.8/symclosestwannier/cw/umat.py
--rw-r--r--   0 ro         (501) staff       (20)    18360 2024-02-01 04:44:14.000000 symclosestwannier-1.1.8/symclosestwannier/cw/win.py
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-01 04:44:21.324932 symclosestwannier-1.1.8/symclosestwannier/scripts/
--rw-r--r--   0 ro         (501) staff       (20)     2420 2024-01-23 05:22:29.000000 symclosestwannier-1.1.8/symclosestwannier/scripts/postcw.py
--rw-r--r--   0 ro         (501) staff       (20)     2462 2024-01-23 05:22:29.000000 symclosestwannier-1.1.8/symclosestwannier/scripts/pw2cw.py
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-01 04:44:21.326259 symclosestwannier-1.1.8/symclosestwannier/util/
--rw-r--r--   0 ro         (501) staff       (20)    22494 2024-02-01 04:44:14.000000 symclosestwannier-1.1.8/symclosestwannier/util/_utility.py
--rw-r--r--   0 ro         (501) staff       (20)     4222 2023-12-19 03:47:00.000000 symclosestwannier-1.1.8/symclosestwannier/util/band.py
--rw-r--r--   0 ro         (501) staff       (20)     3357 2023-12-19 03:50:00.000000 symclosestwannier-1.1.8/symclosestwannier/util/constants.py
--rw-r--r--   0 ro         (501) staff       (20)     8538 2024-01-31 11:24:33.000000 symclosestwannier-1.1.8/symclosestwannier/util/get_oper_R.py
--rw-r--r--   0 ro         (501) staff       (20)    15932 2024-01-31 04:41:33.000000 symclosestwannier-1.1.8/symclosestwannier/util/header.py
--rw-r--r--   0 ro         (501) staff       (20)    10854 2024-02-01 04:44:14.000000 symclosestwannier-1.1.8/symclosestwannier/util/message.py
-drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-01 04:44:21.318510 symclosestwannier-1.1.8/symclosestwannier.egg-info/
--rw-r--r--   0 ro         (501) staff       (20)     2542 2024-02-01 04:44:21.000000 symclosestwannier-1.1.8/symclosestwannier.egg-info/PKG-INFO
--rw-r--r--   0 ro         (501) staff       (20)     1160 2024-02-01 04:44:21.000000 symclosestwannier-1.1.8/symclosestwannier.egg-info/SOURCES.txt
--rw-r--r--   0 ro         (501) staff       (20)        1 2024-02-01 04:44:21.000000 symclosestwannier-1.1.8/symclosestwannier.egg-info/dependency_links.txt
--rw-r--r--   0 ro         (501) staff       (20)      108 2024-02-01 04:44:21.000000 symclosestwannier-1.1.8/symclosestwannier.egg-info/entry_points.txt
--rw-r--r--   0 ro         (501) staff       (20)       81 2024-02-01 04:44:21.000000 symclosestwannier-1.1.8/symclosestwannier.egg-info/requires.txt
--rw-r--r--   0 ro         (501) staff       (20)       18 2024-02-01 04:44:21.000000 symclosestwannier-1.1.8/symclosestwannier.egg-info/top_level.txt
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.292865 symclosestwannier-1.1.9/
+-rw-r--r--   0 ro         (501) staff       (20)    18092 2023-12-19 03:50:00.000000 symclosestwannier-1.1.9/LICENSE
+-rw-r--r--   0 ro         (501) staff       (20)       57 2023-12-19 03:46:59.000000 symclosestwannier-1.1.9/MANIFEST.in
+-rw-r--r--   0 ro         (501) staff       (20)     2542 2024-02-04 15:55:13.292788 symclosestwannier-1.1.9/PKG-INFO
+-rw-r--r--   0 ro         (501) staff       (20)     1805 2023-12-19 03:54:41.000000 symclosestwannier-1.1.9/README.md
+-rw-r--r--   0 ro         (501) staff       (20)      887 2024-02-04 15:55:13.293142 symclosestwannier-1.1.9/setup.cfg
+-rw-r--r--   0 ro         (501) staff       (20)       38 2023-12-19 03:47:00.000000 symclosestwannier-1.1.9/setup.py
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.283915 symclosestwannier-1.1.9/symclosestwannier/
+-rw-r--r--   0 ro         (501) staff       (20)      106 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/__init__.py
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.287405 symclosestwannier-1.1.9/symclosestwannier/analyzer/
+-rw-r--r--   0 ro         (501) staff       (20)     3455 2024-01-22 00:23:53.000000 symclosestwannier-1.1.9/symclosestwannier/analyzer/analyzer.py
+-rw-r--r--   0 ro         (501) staff       (20)     4715 2023-12-19 03:50:00.000000 symclosestwannier-1.1.9/symclosestwannier/analyzer/band.py
+-rw-r--r--   0 ro         (501) staff       (20)     1779 2023-12-19 03:50:00.000000 symclosestwannier-1.1.9/symclosestwannier/analyzer/get_band.py
+-rw-r--r--   0 ro         (501) staff       (20)    18822 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/analyzer/get_response.py
+-rw-r--r--   0 ro         (501) staff       (20)     9136 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/analyzer/response.py
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.290222 symclosestwannier-1.1.9/symclosestwannier/cw/
+-rw-r--r--   0 ro         (501) staff       (20)     2807 2024-01-24 13:49:38.000000 symclosestwannier-1.1.9/symclosestwannier/cw/amn.py
+-rw-r--r--   0 ro         (501) staff       (20)     8487 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/cw/cw_creator.py
+-rw-r--r--   0 ro         (501) staff       (20)     7116 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/cw/cw_info.py
+-rw-r--r--   0 ro         (501) staff       (20)     5529 2023-12-19 03:50:00.000000 symclosestwannier-1.1.9/symclosestwannier/cw/cw_manager.py
+-rw-r--r--   0 ro         (501) staff       (20)    40198 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/cw/cw_model.py
+-rw-r--r--   0 ro         (501) staff       (20)     8123 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/cw/cwin.py
+-rw-r--r--   0 ro         (501) staff       (20)     3336 2024-01-31 04:41:33.000000 symclosestwannier-1.1.9/symclosestwannier/cw/eig.py
+-rw-r--r--   0 ro         (501) staff       (20)     5137 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/cw/mmn.py
+-rw-r--r--   0 ro         (501) staff       (20)    11484 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/cw/nnkp.py
+-rw-r--r--   0 ro         (501) staff       (20)     5985 2023-12-19 03:50:00.000000 symclosestwannier-1.1.9/symclosestwannier/cw/spn.py
+-rw-r--r--   0 ro         (501) staff       (20)     9558 2024-02-01 04:44:14.000000 symclosestwannier-1.1.9/symclosestwannier/cw/umat.py
+-rw-r--r--   0 ro         (501) staff       (20)    18360 2024-02-04 08:23:06.000000 symclosestwannier-1.1.9/symclosestwannier/cw/win.py
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.290920 symclosestwannier-1.1.9/symclosestwannier/scripts/
+-rw-r--r--   0 ro         (501) staff       (20)     2420 2024-01-23 05:22:29.000000 symclosestwannier-1.1.9/symclosestwannier/scripts/postcw.py
+-rw-r--r--   0 ro         (501) staff       (20)     2462 2024-01-23 05:22:29.000000 symclosestwannier-1.1.9/symclosestwannier/scripts/pw2cw.py
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.292301 symclosestwannier-1.1.9/symclosestwannier/util/
+-rw-r--r--   0 ro         (501) staff       (20)    22461 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/util/_utility.py
+-rw-r--r--   0 ro         (501) staff       (20)     4222 2023-12-19 03:47:00.000000 symclosestwannier-1.1.9/symclosestwannier/util/band.py
+-rw-r--r--   0 ro         (501) staff       (20)     3357 2023-12-19 03:50:00.000000 symclosestwannier-1.1.9/symclosestwannier/util/constants.py
+-rw-r--r--   0 ro         (501) staff       (20)     8296 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/util/get_oper_R.py
+-rw-r--r--   0 ro         (501) staff       (20)    16238 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/util/header.py
+-rw-r--r--   0 ro         (501) staff       (20)    10854 2024-02-04 15:54:44.000000 symclosestwannier-1.1.9/symclosestwannier/util/message.py
+drwxr-xr-x   0 ro         (501) staff       (20)        0 2024-02-04 15:55:13.285825 symclosestwannier-1.1.9/symclosestwannier.egg-info/
+-rw-r--r--   0 ro         (501) staff       (20)     2542 2024-02-04 15:55:13.000000 symclosestwannier-1.1.9/symclosestwannier.egg-info/PKG-INFO
+-rw-r--r--   0 ro         (501) staff       (20)     1160 2024-02-04 15:55:13.000000 symclosestwannier-1.1.9/symclosestwannier.egg-info/SOURCES.txt
+-rw-r--r--   0 ro         (501) staff       (20)        1 2024-02-04 15:55:13.000000 symclosestwannier-1.1.9/symclosestwannier.egg-info/dependency_links.txt
+-rw-r--r--   0 ro         (501) staff       (20)      108 2024-02-04 15:55:13.000000 symclosestwannier-1.1.9/symclosestwannier.egg-info/entry_points.txt
+-rw-r--r--   0 ro         (501) staff       (20)       81 2024-02-04 15:55:13.000000 symclosestwannier-1.1.9/symclosestwannier.egg-info/requires.txt
+-rw-r--r--   0 ro         (501) staff       (20)       18 2024-02-04 15:55:13.000000 symclosestwannier-1.1.9/symclosestwannier.egg-info/top_level.txt
```

### Comparing `symclosestwannier-1.1.8/LICENSE` & `symclosestwannier-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/PKG-INFO` & `symclosestwannier-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symclosestwannier
-Version: 1.1.8
+Version: 1.1.9
 Summary: A Python library for Symmetry-Adapted Closest Wannier (SymCW) Tight-Binding model based on Plane-Wave DFT calculation.
 Home-page: https://github.com/CMT-MU/SymClosestWannier
 Author: Rikuto Oiwa
 Author-email: ro.qp.07@gmail.com
 License: MIT
 Keywords: dft,wannier function,tight-binding model,symmetry,materials science
 Requires-Python: >=3.9
```

### Comparing `symclosestwannier-1.1.8/README.md` & `symclosestwannier-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/setup.cfg` & `symclosestwannier-1.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/analyzer/analyzer.py` & `symclosestwannier-1.1.9/symclosestwannier/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/analyzer/band.py` & `symclosestwannier-1.1.9/symclosestwannier/analyzer/band.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/analyzer/get_band.py` & `symclosestwannier-1.1.9/symclosestwannier/analyzer/get_band.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/analyzer/get_response.py` & `symclosestwannier-1.1.9/symclosestwannier/analyzer/get_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,46 +27,50 @@
 # *  LVTS12 = PRB 85, 014435 (2012)  (orbital magnetization and AHC)
 # *  CTVR06 = PRB 74, 024408 (2006)  (  "          "       )
 # *  IATS18 = PRB 97, 245143 (2018)  (nonlinear shift current)
 # *  QZYZ18 = PRB 98, 214402 (2018)  (spin Hall conductivity - SHC)
 # *  RPS19  = PRB 99, 235113 (2019)  (spin Hall conductivity - SHC)
 # *  IAdJS19 = arXiv:1910.06172 (2019) (quasi-degenerate k.p)
 # ---------------------------------------------------------------
-#
-# * Undocumented, works for limited purposes only:
-#                                 reading k-points and weights from file
 
 import numpy as np
+import multiprocessing
+from joblib import Parallel, delayed
 
 from symclosestwannier.util._utility import (
     fourier_transform_r_to_k,
     fourier_transform_r_to_k_new,
     fourier_transform_r_to_k_vec,
 )
 
+# ==================================================
+# number of cpu cores
+_cpu_num = multiprocessing.cpu_count()
+
 
 # ==================================================
-def wham_get_D_h(delH, E, U):
+def wham_get_D_h(delHH, E, U):
     """
     Compute D^H_a=UU^dag.del_a UU (a=x,y,z)
     using Eq.(24) of WYSV06
     """
     num_k = E.shape[0]
     num_wann = E.shape[1]
 
-    D_h = 1.0j * np.zeros((3, num_k, num_wann, num_wann))
-    for k in range(num_k):
-        ek = E[k]
-        for i in range(3):
-            delH_i = U[k].transpose().conjugate() @ delH[i, k] @ U[k]
-            for m in range(num_wann):
-                for n in range(num_wann):
-                    if n == m or abs(ek[m] - ek[n]) < 1e-7:
-                        continue
-                    D_h[i, k, n, m] = delH_i[n, m] / (ek[m] - ek[n])
+    delHH_Band = U.transpose(0, 2, 1).conjugate()[np.newaxis, :, :, :] @ delHH @ U[np.newaxis, :, :, :]
+    fac = np.array(
+        [
+            [
+                [0.0 if n == m or abs(E[k, m] - E[k, n]) < 1e-7 else 1.0 / (E[k, n] - E[k, m]) for n in range(num_wann)]
+                for m in range(num_wann)
+            ]
+            for k in range(num_k)
+        ]
+    )
+    D_h = delHH_Band * fac[np.newaxis, :, :, :]
 
     return D_h
 
 
 # ==================================================
 def utility_w0gauss(x, n):
     """
@@ -85,15 +89,15 @@
 
     # cold smearing  (Marzari-Vanderbilt)
     if n == -1:
         arg = min(200, (x - 1.0 / np.sqrt(2)) ** 2)
         utility_w0gauss = sqrtpm1 * np.exp(-arg) * (2.0 - np.sqrt(2.0) * x)
     # Fermi-Dirac smearing
     elif n == -99:
-        if abs(x) <= 36.0:
+        if np.abs(x) <= 36.0:
             utility_w0gauss = 1.0 / (2.0 + np.exp(-x) + np.exp(+x))
         else:
             utility_w0gauss = 0.0
     # Gaussian
     elif n == 0:
         arg = min(200, x**2)
         utility_w0gauss = np.exp(-arg) * sqrtpm1
@@ -144,17 +148,19 @@
         "kubo_H_spn": 0.0,
         "kubo_AH_spn": 0.0,
         # sc
         # shc
         # kdotp
     }
 
-    # atoms_list = list(cwi["atoms_frac"].values())
-    # atoms_frac = np.array([atoms_list[i] for i in cwi["nw2n"]])
-    atoms_frac = None
+    if cwi["tb_gauge"]:
+        atoms_list = list(cwi["atoms_frac"].values())
+        atoms_frac = np.array([atoms_list[i] for i in cwi["nw2n"]])
+    else:
+        atoms_frac = None
 
     N1, N2, N3 = cwi["berry_kmesh"]
     kpoints = np.array(
         [[i / float(N1), j / float(N2), k / float(N3)] for i in range(N1) for j in range(N2) for k in range(N3)]
     )
 
     HH, delHH = fourier_transform_r_to_k_new(
@@ -162,18 +168,16 @@
     )
 
     E, U = np.linalg.eigh(HH)
 
     D_h = wham_get_D_h(delHH, E, U)
 
     AA = fourier_transform_r_to_k_vec(operators["AA_R"], kpoints, cwi["irvec"], cwi["ndegen"], atoms_frac)
-    Ax = U.transpose(0, 2, 1).conjugate() @ AA[0] @ U
-    Ay = U.transpose(0, 2, 1).conjugate() @ AA[1] @ U
-    Az = U.transpose(0, 2, 1).conjugate() @ AA[2] @ U
-    Avec = np.array([Ax, Ay, Az])
+
+    Avec = np.array([U.transpose(0, 2, 1).conjugate() @ AA[i] @ U for i in range(3)])
 
     A = Avec + 1.0j * D_h  # Eq.(25) WYSV06
 
     # (ahc)  Anomalous Hall conductivity (from Berry curvature)
     if cwi["berry_task"] == "ahc":
         pass
 
@@ -233,125 +237,126 @@
 
     Args:
 
     Returns:
     """
     ef = cwi["fermi_energy"]
     berry_kmesh = cwi["berry_kmesh"]
-
-    if cwi["kubo_eigval_max"] < +100000:
-        kubo_eigval_max = cwi["kubo_eigval_max"]
-    elif cwi["dis_froz_max"] < +100000:
-        kubo_eigval_max = cwi["dis_froz_max"] + 0.6667
-    else:
-        kubo_eigval_max = np.max(E) + 0.6667
-
     num_k = np.prod(berry_kmesh)
     num_wann = cwi["num_wann"]
 
     spin_decomp = cwi["spin_decomp"]
     spn_nk = np.zeros(num_wann)
 
     kubo_adpt_smr = cwi["kubo_adpt_smr"]
     kubo_adpt_smr_fac = cwi["kubo_adpt_smr_fac"]
     kubo_adpt_smr_max = cwi["kubo_adpt_smr_max"]
 
     kubo_smr_fixed_en_width = cwi["kubo_smr_fixed_en_width"]
     eta_smr = kubo_smr_fixed_en_width
 
     kubo_freq_list = np.arange(cwi["kubo_freq_min"], cwi["kubo_freq_max"], cwi["kubo_freq_step"])
-
     if not kubo_adpt_smr and kubo_smr_fixed_en_width != 0.0:
         kubo_freq_list = kubo_freq_list + 1.0j * kubo_smr_fixed_en_width
 
     kubo_nfreq = len(kubo_freq_list)
     if cwi["kubo_smr_type"] == "gauss":
         kubo_smr_type_idx = 0
     elif "m-p" in cwi["kubo_smr_type"]:
         m_pN = cwi["kubo_smr_type"]
         kubo_smr_type_idx = m_pN[2:]
     elif cwi["kubo_smr_type"] == "m-v" or cwi["kubo_smr_type"] == "cold":
         kubo_smr_type_idx = -1
     elif cwi["kubo_smr_type"] == "f-d":
         kubo_smr_type_idx = -99
 
-    occ = np.array([[1.0 if E[k, m] < ef else 0.0 for m in range(num_wann)] for k in range(num_k)])
+    if cwi["kubo_eigval_max"] < +100000:
+        kubo_eigval_max = cwi["kubo_eigval_max"]
+    elif cwi["dis_froz_max"] < +100000:
+        kubo_eigval_max = cwi["dis_froz_max"] + 0.6667
+    else:
+        kubo_eigval_max = np.max(E) + 0.6667
 
     kubo_H = 1.0j * np.zeros((kubo_nfreq, 3, 3))
     kubo_AH = 1.0j * np.zeros((kubo_nfreq, 3, 3))
 
     if spin_decomp:
         kubo_H_spn = 1.0j * np.zeros((kubo_nfreq, 3, 3, 3))
         kubo_AH_spn = 1.0j * np.zeros((kubo_nfreq, 3, 3, 3))
     else:
         kubo_H_spn = 0.0
         kubo_AH_spn = 0.0
 
-    for k in range(num_k):
-        # print(f"{k+1}/{num_k}")
-        ek = E[k]
-        fk = occ[k]
-        ak = A[:, k, :, :]
-
-        for m in range(num_wann):
-            for n in range(num_wann):
-                if n == m:
-                    continue
-                if ek[m] > kubo_eigval_max or ek[n] > kubo_eigval_max:
-                    continue
-                if spin_decomp:
-                    if spn_nk[n] >= 0 and spn_nk[m] >= 0:
-                        ispn = 0  # up --> up transition
-                    elif spn_nk[n] < 0 and spn_nk[m] < 0:
-                        ispn = 1  # down --> down
-                    else:
-                        ispn = 2  # spin-flip
-                if kubo_adpt_smr:  # Eq.(35) YWVS07
-                    # vdum[:] = del_ek[m, :] - del_ek[n, :]
-                    # joint_level_spacing = np.sqrt(np.dot(vdum, vdum))*Delta_k
-                    # eta_smr = min(joint_level_spacing*kubo_adpt_smr_fac, kubo_adpt_smr_max)
-                    eta_smr = kubo_smr_fixed_en_width
-                else:
-                    eta_smr = kubo_smr_fixed_en_width
-
-                rfac1 = (fk[m] - fk[n]) * (ek[m] - ek[n])
-
-                for ifreq in range(kubo_nfreq):
-                    #
-                    # Complex frequency for the anti-Hermitian conductivity
-                    #
-                    if kubo_adpt_smr:
-                        omega = np.real(kubo_freq_list[ifreq]) + 1.0j * eta_smr
-                    else:
-                        omega = kubo_freq_list[ifreq]
-                    #
-                    # Broadened delta function for the Hermitian conductivity and JDOS
-                    #
-                    arg = (ek[m] - ek[n] - np.real(omega)) / eta_smr
-                    # If only Hermitean part were computed, could speed up
-                    # by inserting here 'if(abs(arg)>10.0_dp) cycle'
-                    delta = utility_w0gauss(arg, kubo_smr_type_idx) / eta_smr
-
-                    #
-                    # Lorentzian shape (for testing purposes)
-                    # delta = 1.0 / (1.0 + arg * arg) / np.pi
-                    # delta = delta / eta_smr
-                    #
-                    cfac = 1.0j * rfac1 / (ek[m] - ek[n] - omega)
-                    rfac2 = -np.pi * rfac1 * delta
-
-                    for j in range(3):
-                        for i in range(3):
-                            ak_inm_ak_jmn = ak[i, n, m] * ak[j, m, n]
-                            kubo_H[ifreq, i, j] += rfac2 * ak_inm_ak_jmn
-                            kubo_AH[ifreq, i, j] += cfac * ak_inm_ak_jmn
-
-                            if spin_decomp:
-                                kubo_H_spn[ifreq, i, j, ispn] += rfac2 * ak_inm_ak_jmn
-                                kubo_AH_spn[ifreq, i, j, ispn] += cfac * ak_inm_ak_jmn
+    k_m_n_list = [
+        (k, m, n)
+        for k in range(num_k)
+        for m in range(num_wann)
+        for n in range(num_wann)
+        if m != n and E[k, m] < kubo_eigval_max and E[k, n] < kubo_eigval_max
+    ]
+
+    def proc(k, m, n):
+        ekm = E[k, m]
+        ekn = E[k, n]
+        fkm = 1.0 if E[k, m] < ef else 0.0
+        fkn = 1.0 if E[k, n] < ef else 0.0
+
+        if spin_decomp:
+            if spn_nk[n] >= 0 and spn_nk[m] >= 0:
+                ispn = 0  # up --> up transition
+            elif spn_nk[n] < 0 and spn_nk[m] < 0:
+                ispn = 1  # down --> down
+            else:
+                ispn = 2  # spin-flip
+
+        if kubo_adpt_smr:  # Eq.(35) YWVS07
+            # vdum[:] = del_ek[m, :] - del_ek[n, :]
+            # joint_level_spacing = np.sqrt(np.dot(vdum, vdum))*Delta_k
+            # eta_smr = min(joint_level_spacing*kubo_adpt_smr_fac, kubo_adpt_smr_max)
+            eta_smr = kubo_smr_fixed_en_width
+        else:
+            eta_smr = kubo_smr_fixed_en_width
+
+        # Complex frequency for the anti-Hermitian conductivity
+        if kubo_adpt_smr:
+            omega_list = np.real(kubo_freq_list) + 1.0j * eta_smr
+        else:
+            omega_list = kubo_freq_list
+
+        # Broadened delta function for the Hermitian conductivity and JDOS
+        arg = (ekm - ekn - np.real(omega_list)) / eta_smr
+        delta = np.array([utility_w0gauss(arg[ifreq], kubo_smr_type_idx) for ifreq in range(kubo_nfreq)]) / eta_smr
+
+        rfac1 = (fkm - fkn) * (ekm - ekn)
+        rfac2 = -np.pi * rfac1 * delta
+        cfac = 1.0j * rfac1 / (ekm - ekn - omega_list)
+
+        aiknm_ajkmn = np.array([[A[i, k, n, m] * A[j, k, m, n] for j in range(3)] for i in range(3)])
+
+        kubo_H_ = rfac2[:, np.newaxis, np.newaxis] * aiknm_ajkmn[np.newaxis, :, :]
+        kubo_AH_ = cfac[:, np.newaxis, np.newaxis] * aiknm_ajkmn[np.newaxis, :, :]
+
+        if spin_decomp:
+            kubo_H_spn_ = rfac2[:, np.newaxis, np.newaxis] * aiknm_ajkmn[np.newaxis, :, :]
+            kubo_AH_spn_ = cfac[:, np.newaxis, np.newaxis] * aiknm_ajkmn[np.newaxis, :, :]
+        else:
+            kubo_H_spn_ = 0
+            kubo_AH_spn_ = 0
+
+        return kubo_H_, kubo_AH_, kubo_H_spn_, kubo_AH_spn_
+
+    n_jobs = _cpu_num - 2  # if self._mpm.parallel else 1
+    print(len(k_m_n_list))
+    res_lst = Parallel(n_jobs=n_jobs, verbose=10)(delayed(proc)(k, m, n) for k, m, n in k_m_n_list)
+
+    for kubo_H_, kubo_AH_, kubo_H_spn_, kubo_AH_spn_ in res_lst:
+        kubo_H += kubo_H_
+        kubo_AH += kubo_AH_
+        kubo_H_spn += kubo_H_spn_
+        kubo_AH_spn += kubo_AH_spn_
 
     # Convert to S/cm
     # ==================================================
     # fac = e^2/(hbar.V_c*10^-8)
     # ==================================================
     #
     # with 'V_c' in Angstroms^3, and 'e', 'hbar' in SI units
@@ -360,14 +365,15 @@
     cell_volume = cwi["unit_cell_volume"]
     hbar_SI = 1.054571726e-34  # wannier90
     elem_charge_SI = 1.602176565e-19  # wannier90
 
     fac = 1.0e8 * elem_charge_SI**2 / (hbar_SI * cell_volume) / num_k
     kubo_H *= fac
     kubo_AH *= fac
+
     if spin_decomp:
         kubo_H_spn *= fac
         kubo_AH_spn *= fac
 
     return kubo_H, kubo_AH, kubo_H_spn, kubo_AH_spn
```

### Comparing `symclosestwannier-1.1.8/symclosestwannier/analyzer/response.py` & `symclosestwannier-1.1.9/symclosestwannier/analyzer/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,56 +92,56 @@
         Wannier matrix elements, allocations and initializations.
         """
         self._cwm.log(cw_start_set_operators_msg(), stamp=None, end="\n", file=self._outfile, mode="a")
         self._cwm.set_stamp()
 
         # (ahc)  Anomalous Hall conductivity (from Berry curvature)
         if self._cwi["berry_task"] == "ahc":
-            self["HH_R"] = get_oper_R("HH_R", self._cwi, tb_gauge=False) if self["HH_R"] is None else None
-            self["AA_R"] = get_oper_R("AA_R", self._cwi, tb_gauge=False) if self["AA_R"] is None else None
+            self["HH_R"] = get_oper_R("HH_R", self._cwi) if self["HH_R"] is None else None
+            self["AA_R"] = get_oper_R("AA_R", self._cwi) if self["AA_R"] is None else None
 
         # (morb) Orbital magnetization
         if self._cwi["berry_task"] == "morb":
-            self["HH_R"] = get_oper_R("HH_R", self._cwi, tb_gauge=False) if self["HH_R"] is None else None
-            self["AA_R"] = get_oper_R("AA_R", self._cwi, tb_gauge=False) if self["AA_R"] is None else None
-            self["BB_R"] = get_oper_R("BB_R", self._cwi, tb_gauge=False) if self["BB_R"] is None else None
-            self["CC_R"] = get_oper_R("CC_R", self._cwi, tb_gauge=False) if self["CC_R"] is None else None
+            self["HH_R"] = get_oper_R("HH_R", self._cwi) if self["HH_R"] is None else None
+            self["AA_R"] = get_oper_R("AA_R", self._cwi) if self["AA_R"] is None else None
+            self["BB_R"] = get_oper_R("BB_R", self._cwi) if self["BB_R"] is None else None
+            self["CC_R"] = get_oper_R("CC_R", self._cwi) if self["CC_R"] is None else None
 
         # (kubo) Complex optical conductivity (Kubo-Greenwood) & JDOS
         if self._cwi["berry_task"] == "kubo":
-            self["HH_R"] = get_oper_R("HH_R", self._cwi, tb_gauge=False) if self["HH_R"] is None else None
-            self["AA_R"] = get_oper_R("AA_R", self._cwi, tb_gauge=False) if self["AA_R"] is None else None
+            self["HH_R"] = get_oper_R("HH_R", self._cwi) if self["HH_R"] is None else None
+            self["AA_R"] = get_oper_R("AA_R", self._cwi) if self["AA_R"] is None else None
             if self._cwi["spin_decomp"]:
-                self["SS_R"] = get_oper_R("SS_R", self._cwi, tb_gauge=False) if self["SS_R"] is None else None
+                self["SS_R"] = get_oper_R("SS_R", self._cwi) if self["SS_R"] is None else None
 
         # (sc)   Nonlinear shift current
         if self._cwi["berry_task"] == "sc":
-            self["HH_R"] = get_oper_R("HH_R", self._cwi, tb_gauge=False) if self["HH_R"] is None else None
-            self["AA_R"] = get_oper_R("AA_R", self._cwi, tb_gauge=False) if self["AA_R"] is None else None
+            self["HH_R"] = get_oper_R("HH_R", self._cwi) if self["HH_R"] is None else None
+            self["AA_R"] = get_oper_R("AA_R", self._cwi) if self["AA_R"] is None else None
 
         # (shc)  Spin Hall conductivity
         if self._cwi["berry_task"] == "shc":
-            self["HH_R"] = get_oper_R("HH_R", self._cwi, tb_gauge=False) if self["HH_R"] is None else None
-            self["AA_R"] = get_oper_R("AA_R", self._cwi, tb_gauge=False) if self["AA_R"] is None else None
-            self["SS_R"] = get_oper_R("SS_R", self._cwi, tb_gauge=False) if self["SS_R"] is None else None
+            self["HH_R"] = get_oper_R("HH_R", self._cwi) if self["HH_R"] is None else None
+            self["AA_R"] = get_oper_R("AA_R", self._cwi) if self["AA_R"] is None else None
+            self["SS_R"] = get_oper_R("SS_R", self._cwi) if self["SS_R"] is None else None
 
             if self._cwi["shc_method"] == "qiao":
-                self["SHC_R"] = get_oper_R("SHC_R", self._cwi, tb_gauge=False) if self["SHC_R"] is None else None
+                self["SHC_R"] = get_oper_R("SHC_R", self._cwi) if self["SHC_R"] is None else None
             else:  # ryoo
-                self["SAA_R"] = get_oper_R("SAA_R", self._cwi, tb_gauge=False) if self["SAA_R"] is None else None
-                self["SBB_R"] = get_oper_R("SBB_R", self._cwi, tb_gauge=False) if self["SBB_R"] is None else None
+                self["SAA_R"] = get_oper_R("SAA_R", self._cwi) if self["SAA_R"] is None else None
+                self["SBB_R"] = get_oper_R("SBB_R", self._cwi) if self["SBB_R"] is None else None
 
         if self._cwi["berry_task"] == "kdotp":
-            self["HH_R"] = get_oper_R("HH_R", self._cwi, tb_gauge=False) if self["HH_R"] is None else None
+            self["HH_R"] = get_oper_R("HH_R", self._cwi) if self["HH_R"] is None else None
 
         # (me) magnetoelectric tensor
         if self._cwi["berry_task"] == "me":
-            self["HH_R"] = get_oper_R("HH_R", self._cwi, tb_gauge=False) if self["HH_R"] is None else None
-            self["AA_R"] = get_oper_R("AA_R", self._cwi, tb_gauge=False) if self["AA_R"] is None else None
-            self["SS_R"] = get_oper_R("SS_R", self._cwi, tb_gauge=False) if self["SS_R"] is None else None
+            self["HH_R"] = get_oper_R("HH_R", self._cwi) if self["HH_R"] is None else None
+            self["AA_R"] = get_oper_R("AA_R", self._cwi) if self["AA_R"] is None else None
+            self["SS_R"] = get_oper_R("SS_R", self._cwi) if self["SS_R"] is None else None
 
         self._cwm.log(cw_end_set_operators_msg(), stamp=None, end="\n", file=self._outfile, mode="a")
 
     # ==================================================
     def calc_response(self):
         self._cwm.log(cw_start_response_msg(), stamp=None, end="\n", file=self._outfile, mode="a")
         self._cwm.set_stamp()
```

### Comparing `symclosestwannier-1.1.8/symclosestwannier/cw/amn.py` & `symclosestwannier-1.1.9/symclosestwannier/cw/amn.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/cw/cw_creator.py` & `symclosestwannier-1.1.9/symclosestwannier/cw/cw_creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,20 +92,20 @@
         cw_model.write_or(cw_model["Sr"], filename, header=CWModel._sr_header())
 
     if cwi["write_u_matrices"] and cwi["restart"] != "w90":
         file_names = (f"{cwi['seedname']}_u.mat.cw", f"{cwi['seedname']}_u_dis.mat.cw")
         cwi.umat.write(file_names)
 
     if cwi["write_rmn"]:
-        AA_R = get_oper_R("AA_R", cwi, tb_gauge=False)
+        AA_R = get_oper_R("AA_R", cwi)
         filename = f"{cwi['seedname']}_r.dat.cw"
         cw_model.write_or(AA_R, filename, vec=True)
 
     if cwi["write_tb"]:
-        AA_R = get_oper_R("AA_R", cwi, tb_gauge=False)
+        AA_R = get_oper_R("AA_R", cwi)
         filename = f"{cwi['seedname']}_tb.dat.cw"
         cw_model.write_tb(cw_model["Hr"], AA_R, filename)
 
     if cwi["write_vmn"]:
         pass
 
     if cwi["write_spn"]:
```

### Comparing `symclosestwannier-1.1.8/symclosestwannier/cw/cw_info.py` & `symclosestwannier-1.1.9/symclosestwannier/cw/cw_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,27 +85,28 @@
         for name, C in _class_map.items():
             if name == "umat" and (d["restart"] != "w90"):
                 continue
             if name == "mmn":
                 if not np.any([d["write_rmn"], d["write_vmn"], d["write_tb"], d["berry"]]):
                     continue
             if name == "spn":
-                if not np.any([d["write_spn"], d["write_spn"], d["spin_decomp"]]):
+                if not np.any([d["write_spn"], d["spin_decomp"]]):
                     continue
 
             info = C(topdir, seedname)
             for k, v in info.items():
                 for name_, info_ in info_list:
                     if k in info_:
                         v_ = info_[k]
-                        try:
-                            if v != v_:
+
+                        if type(v) == list:
+                            if not np.allclose(v, v_, 1e-6):
                                 raise Exception(f"The value of {k} in {name} and {name_} is inconsistent.")
-                        except:
-                            if not np.sum(np.array(v) - np.array(v_)) < 1e-6:
+                        else:
+                            if v != v_:
                                 raise Exception(f"The value of {k} in {name} and {name_} is inconsistent.")
 
             info_list.append((name, info))
             d.update(info)
 
         # additional information
         A = np.array(d["A"])
```

### Comparing `symclosestwannier-1.1.8/symclosestwannier/cw/cw_manager.py` & `symclosestwannier-1.1.9/symclosestwannier/cw/cw_manager.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/cw/cw_model.py` & `symclosestwannier-1.1.9/symclosestwannier/cw/cw_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -467,20 +467,24 @@
         rpoints_mp = [(n1, n2, n3) for Zj_dict in Zr_dict.values() for (n1, n2, n3, _, _) in Zj_dict.keys()]
         rpoints_mp = sorted(list(set(rpoints_mp)), key=rpoints_mp.index)
 
         Sr_sym = CWModel.construct_Or(list(s.values()), self._cwi["num_wann"], rpoints_mp, mat)
         Hr_sym = CWModel.construct_Or(list(z.values()), self._cwi["num_wann"], rpoints_mp, mat)
         Hr_nonortho_sym = CWModel.construct_Or(list(z_nonortho.values()), self._cwi["num_wann"], rpoints_mp, mat)
 
-        Sk_sym = CWModel.fourier_transform_r_to_k(Sr_sym, self._cwi["kpoints"], rpoints_mp, atoms_frac=atoms_frac_samb)
-        Hk_sym = CWModel.fourier_transform_r_to_k(Hr_sym, self._cwi["kpoints"], rpoints_mp, atoms_frac=atoms_frac_samb)
-        Hk_nonortho_sym = CWModel.fourier_transform_r_to_k(
-            Hr_nonortho_sym, self._cwi["kpoints"], rpoints_mp, atoms_frac=atoms_frac_samb
-        )
-
+        if self._cwi["tb_gauge"]:
+            Sk_sym = CWModel.fourier_transform_r_to_k(Sr_sym, self._cwi["kpoints"], rpoints_mp, atoms_frac=atoms_frac_samb)
+            Hk_sym = CWModel.fourier_transform_r_to_k(Hr_sym, self._cwi["kpoints"], rpoints_mp, atoms_frac=atoms_frac_samb)
+            Hk_nonortho_sym = CWModel.fourier_transform_r_to_k(
+                Hr_nonortho_sym, self._cwi["kpoints"], rpoints_mp, atoms_frac=atoms_frac_samb
+            )
+        else:
+            Sk_sym = CWModel.fourier_transform_r_to_k(Sr_sym, self._cwi["kpoints"], rpoints_mp)
+            Hk_sym = CWModel.fourier_transform_r_to_k(Hr_sym, self._cwi["kpoints"], rpoints_mp)
+            Hk_nonortho_sym = CWModel.fourier_transform_r_to_k(Hr_nonortho_sym, self._cwi["kpoints"], rpoints_mp)
         self._cwm.log("done", file=self._outfile, mode="a")
 
         #####
 
         msg = "    - evaluating fitting accuracy ... "
         self._cwm.log(msg, None, end="\n", file=self._outfile, mode="a")
         self._cwm.set_stamp()
@@ -498,17 +502,21 @@
 
         if not mat["molecule"]:
             Hk_path = CWModel.fourier_transform_r_to_k(
                 self["Hr"], self._cwi["kpoints_path"], self._cwi["irvec"], self._cwi["ndegen"]
             )
             Ek_path, _ = np.linalg.eigh(Hk_path)
 
-            Hk_sym_path = CWModel.fourier_transform_r_to_k(
-                Hr_sym, self._cwi["kpoints_path"], rpoints_mp, atoms_frac=atoms_frac_samb
-            )
+            if self._cwi["tb_gauge"]:
+                Hk_sym_path = CWModel.fourier_transform_r_to_k(
+                    Hr_sym, self._cwi["kpoints_path"], rpoints_mp, atoms_frac=atoms_frac_samb
+                )
+            else:
+                Hk_sym_path = CWModel.fourier_transform_r_to_k(Hr_sym, self._cwi["kpoints_path"], rpoints_mp)
+
             Ek_path_sym, _ = np.linalg.eigh(Hk_sym_path)
 
             num_k, num_wann = Ek_path_sym.shape
             Ek_RMSE_path = np.sum(np.abs(Ek_path_sym - Ek_path)) / num_k / num_wann * 1000  # [meV]
 
             msg = f"     * RMSE of eigen values between CW and Symmetry-Adapted CW models (path) = {'{:.4f}'.format(Ek_RMSE_path)} [meV]"
             self._cwm.log(msg, None, end="\n", file=self._outfile, mode="a")
@@ -563,26 +571,26 @@
         Args:
             Ok (ndarray): arbitrary operator in k-space representation, O_{ab}(k) = <φ_{a}(k)|O|φ_{b}(k)>.
             kpoints (ndarray): k-points used in DFT calculation, [[k1, k2, k3]] (crystal coordinate).
             irvec (ndarray, optional): irreducible R vectors (crystal coordinate, [[n1,n2,n3]], nj: integer).
             atoms_frac (ndarray, optional): atom's position in fractional coordinates.
 
         Returns:
-            (ndarray, ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(R)|O|φ_{b}(0)>, lattice points.
+            (ndarray, ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(0)|O|φ_{b}(R)>, lattice points.
         """
         return fourier_transform_k_to_r(Ok, kpoints, irvec, atoms_frac)
 
     # ==================================================
     @classmethod
     def fourier_transform_r_to_k(cls, Or, kpoints, irvec, ndegen=None, atoms_frac=None):
         """
         fourier transformation of an arbitrary operator from real-space representation into k-space representation.
 
         Args:
-        Or (ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(R)|O|φ_{b}(0)>.
+        Or (ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(0)|O|φ_{b}(R)>.
         kpoints (ndarray): k-points used in DFT calculation, [[k1, k2, k3]] (crystal coordinate).
         irvec (ndarray): irreducible R vectors (crystal coordinate, [[n1,n2,n3]], nj: integer).
         ndegen (ndarray, optional): number of degeneracy at each R.
         atoms_frac (ndarray, optional): atom's position in fractional coordinates.
 
         Returns:
             ndarray: k-space representation of the given operator, O_{ab}(k) = <φ_{a}(k)|O|φ_{b}(k)>.
@@ -612,15 +620,15 @@
     # ==================================================
     @classmethod
     def matrix_dict_r(cls, Or, rpoints, diagonal=False):
         """
         dictionary form of an arbitrary operator matrix in real-space representation.
 
         Args:
-            Or (ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(R)|O|φ_{b}(0)>.
+            Or (ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(0)|O|φ_{b}(R)>.
             rpoints (ndarray): lattice points (crystal coordinate, [[n1,n2,n3]], nj: integer).
             diagonal (bool, optional): diagonal matrix ?
 
         Returns:
             dict: real-space representation of the given operator, {(n2,n2,n3,a,b) = O_{ab}(R)}.
         """
         return matrix_dict_r(Or, rpoints, diagonal)
@@ -912,15 +920,15 @@
 
     # ==================================================
     def write_or(self, Or, filename, rpoints=None, header=None, vec=False):
         """
         write seedname_or.dat.
 
         Args:
-            Or (ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(R)|O|φ_{b}(0)>.
+            Or (ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(0)|O|φ_{b}(R)>.
             filename (str): file name.
             rpoints (ndarray): rpoints.
             header (str, optional): header.
             vec (bool, optional): vector ?
         """
         num_wann = self._cwi["num_wann"]
         unit_cell_cart = np.array(self._cwi["unit_cell_cart"])
@@ -963,16 +971,16 @@
 
     # ==================================================
     def write_tb(self, Hr, Ar, filename, rpoints=None):
         """
         write seedname_or.dat.
 
         Args:
-            Hr (ndarray): real-space representation of the Hamiltonian, H_{ab}(R) = <φ_{a}(R)|H|φ_{b}(0)>.
-            Ar (ndarray): real-space representation of the Hamiltonian, A_{ab}(R) = <φ_{a}(R)|r|φ_{b}(0)>.
+            Hr (ndarray): real-space representation of the Hamiltonian, H_{ab}(R) = <φ_{a}(0)|H|φ_{b}(R)>.
+            Ar (ndarray): real-space representation of the Hamiltonian, A_{ab}(R) = <φ_{a}(0)|r|φ_{b}(R)>.
             filename (str): file name.
             rpoints (ndarray): rpoints.
         """
         num_wann = self._cwi["num_wann"]
         unit_cell_cart = np.array(self._cwi["unit_cell_cart"])
         Hr = np.array(Hr)
         tb_str = "# created by pw2cw \n"
@@ -983,15 +991,15 @@
         tb_str += " {0[0]:15.6f} {0[1]:15.6f} {0[2]:15.6f}\n".format(unit_cell_cart[2, :])
 
         if rpoints is None:
             rpoints = np.array(self._cwi["irvec"])
             ndegen = np.array(self._cwi["ndegen"])
             tb_str += "{:12d}\n{:12d}\n".format(num_wann, len(ndegen))
             tb_str += textwrap.fill("".join(["{:5d}".format(x) for x in ndegen]), 75, drop_whitespace=False)
-            tb_str += "\n"
+            tb_str += "\n\n"
 
         else:
             rpoints = np.array(rpoints)
             ndegen = None
             tb_str += "{:12d}\n".format(num_wann)
 
         # _hr
```

### Comparing `symclosestwannier-1.1.8/symclosestwannier/cw/cwin.py` & `symclosestwannier-1.1.9/symclosestwannier/cw/cwin.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     "delta": 1e-12,
     "svd": False,
     #
     "verbose": False,
     "parallel": False,
     "formatter": False,
     #
+    "transl_inv": True, # use Eq.(31) of Marzari&Vanderbilt PRB 56, 12847 (1997) for band-diagonal position matrix elements.
+    "tb_gauge": False, # tb gauge?
+    #
     "write_hr": False,
     "write_sr": False,
     "write_u_matrices": False,
     "write_rmn": False,
     "write_vmn": False,
     "write_tb": False,
     "write_spn": False,
@@ -94,14 +97,16 @@
                 - smearing_temp_max : smearing temperature for upper window (float), [5.0].
                 - smearing_temp_min : smearing temperature for lower window (float), [0.01].
                 - delta             : small constant to avoid ill-conditioning of overlap matrices (float), [1e-12].
                 - svd               : implement singular value decomposition ? otherwise adopt Lowdin's orthogonalization method (bool), [False].
                 - verbose           : verbose calculation info (bool, optional), [False].
                 - parallel          : use parallel code? (bool), [False].
                 - formatter         : format by using black? (bool), [False].
+                - transl_inv        : use Eq.(31) of Marzari&Vanderbilt PRB 56, 12847 (1997) for band-diagonal position matrix elements? (bool), [True].
+                - tb_gauge          : use tb gauge? (bool), [False].
                 - write_hr          : write seedname_hr.py ? (bool), [False].
                 - write_sr          : write seedname_sr.py ? (bool), [False].
                 - write_u_matrices  : write seedname_u.dat and seedname_u_dis.dat ? (bool), [False].
                 - write_rmn         : write seedname_r.dat ? (bool), [False].
                 - write_vmn         : write seedname_v.dat ? (bool), [False].
                 - write_tb          : write seedname_tb.dat ? (bool), [False].
                 - write_spn         : write seedname.spn.cw ? (bool), [False].
@@ -124,67 +129,70 @@
         else:
             raise Exception("failed to read cwin file: " + file_name)
 
         # default
         d = CWin._default().copy()
 
         for line in cwin_data:
-            line = [vi for vi in line.replace("\n", "").split(" ") if vi != ""]
-            if len(line) == 0:
-                continue
+            line = line.replace("\n", "")
 
-            if "!" in line[0]:
+            if len([vi for vi in line.split(" ") if vi != ""]) == 0:
                 continue
 
-            if "#" in line[0]:
+            key = line.split("=")[0]
+            key = key.replace(" ", "")
+
+            if "!" in key or "#" in key:
                 continue
 
-            k = line[0]
-            if k == "ket_amn":
-                v = "".join(line[2:]) if line[1] == "=" else "".join(line[1:])
-            else:
-                v = line[2] if line[1] == "=" else line[1]
+            if "=" in line:
+                v = (line.split("=")[1].split("!")[0]).replace(" ", "")
+            elif ":" in line:
+                v = (line.split(":")[1].split("!")[0]).replace(" ", "")
+
+            if key == "ket_amn":
+                v = "".join(v)
 
-            d[k] = self._str_to(k, v)
+            d[key] = self._str_to(key, v)
         assert not (
             d["restart"] == "w90" and d["symmetrization"]
         ), "Symmetrization cannot be performed when restart == w90."
 
         return d
 
     # ==================================================
-    def _str_to(self, k, v):
+    def _str_to(self, key, v):
         v = str(v).replace("'", "").replace('"', "")
 
-        if k in ("seedname", "mp_seedname"):
+        if key in ("seedname", "mp_seedname"):
             pass
-        elif k in ("outdir", "mp_outdir"):
+        elif key in ("outdir", "mp_outdir"):
             v = v[:-1] if v[-1] == "/" else v
-        elif k == "restart":
+        elif key == "restart":
             if v not in ("cw", "sym", "w90"):
                 raise Exception(f"invalid restart = {v} was given. choose from 'cw'/'w90'/'sym'.")
-        elif k in (
+        elif key in (
             "proj_min",
             "dis_win_emax",
             "dis_win_emin",
             "smearing_temp_max",
             "smearing_temp_min",
             "delta",
             "a",
             "fermi_energy",
         ):
             v = float(v)
-        elif k == "N1":
+        elif key == "N1":
             v = int(v)
-        elif k == "ket_amn":
+        elif key == "ket_amn":
             if "(" in str(v) and ")" in str(v):
                 v = [str(o) if i == 0 else f"({str(o)}" for i, o in enumerate(v[1:-1].split(",("))]
             else:
                 v = [str(o) for o in v[1:-1].split(",")]
-        elif k == "irreps":
+        elif key == "irreps":
             if "[" in v and "]" in v:
                 v = [str(o) for o in v[1:-1].split(",")]
             else:
                 if v not in ("all", "full"):
                     raise Exception(f"invalid irreps = {v} was given. choose from 'all'/'full'.")
         else:
             if v.lower() in ("true", ".true."):
```

### Comparing `symclosestwannier-1.1.8/symclosestwannier/cw/eig.py` & `symclosestwannier-1.1.9/symclosestwannier/cw/eig.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/cw/mmn.py` & `symclosestwannier-1.1.9/symclosestwannier/cw/mmn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Mmn manages overlap matrix elements in seedname.mmn file, M_{mn}(k,b) = <u^{KS}_{m}(k)|u^{KS}_{n}(k+b)>.
 - ψ^{KS}_{m}(k) = u^{KS}_{m}(k) e^{ik.r}.
 """
+
 import os
 import gzip
 import tarfile
 import itertools
 import datetime
 import multiprocessing
 from itertools import islice
@@ -112,17 +113,15 @@
 
         Mkb_data = [d[:, 0] + 1j * d[:, 1] for d in Mkb_data]
         Mkb = np.array(Mkb_data).reshape(num_k, num_b, num_bands, num_bands).transpose((0, 1, 3, 2))
         nnkpts_data = np.array([s.split() for s in nnkpts_data], dtype=int).reshape(num_k, num_b, 5)
 
         assert np.all(nnkpts_data[:, :, 0] - 1 == np.arange(num_k)[:, None])
 
-        nnkpts = nnkpts_data
-
-        nnkpts = nnkpts.tolist()
+        nnkpts = nnkpts_data.tolist()
         Mkb = Mkb.tolist()
 
         d = {"num_k": num_k, "num_bands": num_bands, "num_b": num_b, "nnkpts": nnkpts, "Mkb": Mkb}
 
         return d
 
     # ==================================================
```

### Comparing `symclosestwannier-1.1.8/symclosestwannier/cw/nnkp.py` & `symclosestwannier-1.1.9/symclosestwannier/cw/nnkp.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "A": [[1, 0, 0], [0, 1, 0], [0, 0, 1]],
     "B": [[2 * np.pi, 0, 0], [0, 2 * np.pi, 0], [0, 0, 2 * np.pi]],
     "num_k": 1,
     "num_wann": 1,
     "num_atom": 1,
     "num_b": 1,
     "kpoints": [[0, 0, 0]],
+    "kpoints_wo_shift": [[0, 0, 0]],
     "nnkpts": None,
     "nw2n": None,
     "nw2l": None,
     "nw2m": None,
     "nw2r": None,
     "atom_orb": None,
     "atom_pos": None,
@@ -69,32 +70,33 @@
         read seedname.nnkp file.
 
         Args:
             file_name (str, optional): file name.
 
         Returns:
             dict:
-                - A          : real lattice vectors, A = [a1,a2,a3] (list), [[[1,0,0], [0,1,0], [0,0,1]]].
-                - B          : reciprocal lattice vectors, B = [b1,b2,b3] (list), [[[2*pi,0,0], [0,2*pi,0], [0,0,2*pi]]].
-                - num_k      : # of k points (int), [1].
-                - num_wann   : # of WFs (int), [1].
-                - num_atom   : # of atoms (int), [1].
-                - num_b      : # of b-vectors (int), [1].
-                - kpoints    : k-points, [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].
-                - nnkpts     : nearest-neighbour k-points (list), [None].
-                - nw2n       : atom position index of each WFs (list), [None].
-                - nw2l       : l specifies the angular part Θlm(θ, φ) (list), [None].
-                - nw2m       : m specifies the angular part Θlm(θ, φ) (list), [None].
-                - nw2r       : r specifies the radial part Rr(r) (list), [None].
-                - atom_orb   : WFs indexes of each atom (list), [None].
-                - atom_pos   : atom position index of each atom (list), [None].
-                - atom_pos_r : atom position of each atom in fractional coordinates with respect to the lattice vectors (list), [None].
-                - bvec_cart  : b-vectors (cartesian coordinate) (list), [None].
-                - bvec_crys  : b-vectors (crystal coordinate) (list), [None].
-                - wb         : weight for each k-points and nearest-neighbour k-points (list), [None].
+                - A                : real lattice vectors, A = [a1,a2,a3] (list), [[[1,0,0], [0,1,0], [0,0,1]]].
+                - B                : reciprocal lattice vectors, B = [b1,b2,b3] (list), [[[2*pi,0,0], [0,2*pi,0], [0,0,2*pi]]].
+                - num_k            : # of k points (int), [1].
+                - num_wann         : # of WFs (int), [1].
+                - num_atom         : # of atoms (int), [1].
+                - num_b            : # of b-vectors (int), [1].
+                - kpoints          : k-points, [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].
+                - kpoints_wo_shift : k-points without shift, [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].
+                - nnkpts           : nearest-neighbour k-points (list), [None].
+                - nw2n             : atom position index of each WFs (list), [None].
+                - nw2l             : l specifies the angular part Θlm(θ, φ) (list), [None].
+                - nw2m             : m specifies the angular part Θlm(θ, φ) (list), [None].
+                - nw2r             : r specifies the radial part Rr(r) (list), [None].
+                - atom_orb         : WFs indexes of each atom (list), [None].
+                - atom_pos         : atom position index of each atom (list), [None].
+                - atom_pos_r       : atom position of each atom in fractional coordinates with respect to the lattice vectors (list), [None].
+                - bvec_cart        : b-vectors (cartesian coordinate) (list), [None].
+                - bvec_crys        : b-vectors (crystal coordinate) (list), [None].
+                - wb               : weight for each k-points and nearest-neighbour k-points (list), [None].
         """
         if os.path.exists(file_name):
             with open(file_name) as fp:
                 nnkp_data = fp.readlines()
         elif os.path.exists(file_name + ".gz"):
             with gzip.open(file_name + ".gz", "rt") as fp:
                 nnkp_data = fp.readlines()
@@ -112,20 +114,22 @@
                     d["A"] = np.genfromtxt(nnkp_data[i + 1 : i + 4], dtype=float).tolist()
 
                 if "begin recip_lattice" in line:
                     d["B"] = np.genfromtxt(nnkp_data[i + 1 : i + 4], dtype=float).tolist()
 
                 if "begin kpoints" in line:
                     d["num_k"] = int(nnkp_data[i + 1])
-                    kpoints = np.genfromtxt(nnkp_data[i + 2 : i + 2 + d["num_k"]], dtype=float)
-                    kpoints = np.mod(kpoints, 1)  # 0 <= kj < 1.0
+                    kpoints_wo_shift = np.genfromtxt(nnkp_data[i + 2 : i + 2 + d["num_k"]], dtype=float)
+                    kpoints = np.mod(kpoints_wo_shift, 1)  # 0 <= kj < 1.0
                     if kpoints.ndim == 1:
                         d["kpoints"] = [kpoints.tolist()]
+                        d["kpoints_wo_shift"] = [kpoints_wo_shift.tolist()]
                     else:
                         d["kpoints"] = kpoints.tolist()
+                        d["kpoints_wo_shift"] = kpoints_wo_shift.tolist()
 
                 if "begin nnkpts" in line:
                     d["num_b"] = int(nnkp_data[i + 1])
                     dat = np.genfromtxt(nnkp_data[i + 2 : i + 2 + d["num_k"] * d["num_b"]], dtype=int)
                     d["nnkpts"] = dat.reshape(d["num_k"], d["num_b"], 5).tolist()
 
                 if "begin projections" in line or "begin spinor_projections" in line:
@@ -177,22 +181,24 @@
                     d["atom_pos"] = atom_pos
                     d["atom_pos_r"] = atom_pos_r
 
             bvec_cart = np.zeros([d["num_b"], 3])
             bvec_crys = np.zeros([d["num_b"], 3])
             bbmat = np.zeros([d["num_b"], 9])
             try:
-                Gp_idx = d["kpoints"].index([0.0, 0.0, 0.0])
+                Gp_idx = d["kpoints_wo_shift"].index([0.0, 0.0, 0.0])
             except:
                 raise Exception("Gamma point must be included.")
+
             for i in range(d["num_b"]):
                 kv = d["nnkpts"][Gp_idx][i]
-                k = d["kpoints"][kv[0] - 1]
-                k_b = d["kpoints"][kv[1] - 1]
+                k = d["kpoints_wo_shift"][kv[0] - 1]
+                k_b = d["kpoints_wo_shift"][kv[1] - 1]
                 b = np.array(k_b) - np.array(k) + np.array(kv[2:5])
+
                 bvec_cart[i, :] = self.k_crys2cart(b, d["B"])
                 bvec_crys[i, :] = self.k_cart2crys(bvec_cart[i, :], d["A"])
                 bbmat[i, :] = [bvec_cart[i, a] * bvec_cart[i, b] for a, b in itertools.product(range(3), range(3))]
 
             delta_ab = np.array([a == b for a, b in itertools.product(range(3), range(3))]).astype(int)
             wb = np.matmul(delta_ab, scipy.linalg.pinv(bbmat))
 
@@ -218,16 +224,16 @@
 
     # ==================================================
     def bvec(self, d, type="cart"):
         """
         d : array of integer [5]
         return : b vector in cartesian/fractional coordinates
         """
-        k = np.array(self["kpoints"][d[0] - 1])
-        kb = np.array(self["kpoints"][d[1] - 1])
+        k = np.array(self["kpoints_wo_shift"][d[0] - 1])
+        kb = np.array(self["kpoints_wo_shift"][d[1] - 1])
         G = np.array(d[2:5])
         b_crys = kb + G - k
 
         if type == "cart":
             return self.k_crys2cart(b_crys, self["B"])
         else:
             return b_crys
```

### Comparing `symclosestwannier-1.1.8/symclosestwannier/cw/spn.py` & `symclosestwannier-1.1.9/symclosestwannier/cw/spn.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/cw/umat.py` & `symclosestwannier-1.1.9/symclosestwannier/cw/umat.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/cw/win.py` & `symclosestwannier-1.1.9/symclosestwannier/cw/win.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/scripts/postcw.py` & `symclosestwannier-1.1.9/symclosestwannier/scripts/postcw.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/scripts/pw2cw.py` & `symclosestwannier-1.1.9/symclosestwannier/scripts/pw2cw.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/util/_utility.py` & `symclosestwannier-1.1.9/symclosestwannier/util/_utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 utility codes.
 """
+
 import numpy as np
 import fortio, scipy.io
 
 from gcoreutils.nsarray import NSArray
 
 M_ZERO = np.finfo(float).eps
 
@@ -116,15 +117,15 @@
     Args:
         Ok (ndarray): arbitrary operator in k-space representation, O_{ab}(k) = <φ_{a}(k)|O|φ_{b}(k)>.
         kpoints (ndarray): k-points used in DFT calculation, [[k1, k2, k3]] (crystal coordinate).
         irvec (ndarray, optional): irreducible R vectors (crystal coordinate, [[n1,n2,n3]], nj: integer).
         atoms_frac (ndarray, optional): atom's position in fractional coordinates.
 
     Returns:
-        (ndarray, ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(R)|O|φ_{b}(0)>, lattice points.
+        (ndarray, ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(0)|O|φ_{b}(R)>, lattice points.
     """
     Ok = np.array(Ok, dtype=complex)
     kpoints = np.array(kpoints, dtype=float)
     irvec = np.array(irvec, dtype=float)
 
     num_k = kpoints.shape[0]
 
@@ -145,15 +146,15 @@
 
 # ==================================================
 def fourier_transform_r_to_k(Or, kpoints, irvec, ndegen=None, atoms_frac=None):
     """
     fourier transformation of an arbitrary operator from real-space representation into k-space representation.
 
     Args:
-        Or (ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(R)|O|φ_{b}(0)>.
+        Or (ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(0)|O|φ_{b}(R)>.
         kpoints (ndarray): k-points used in DFT calculation, [[k1, k2, k3]] (crystal coordinate).
         irvec (ndarray): irreducible R vectors (crystal coordinate, [[n1,n2,n3]], nj: integer).
         ndegen (ndarray, optional): number of degeneracy at each R.
         atoms_frac (ndarray, optional): atom's position in fractional coordinates.
 
     Returns:
         ndarray: k-space representation of the given operator, O_{ab}(k) = <φ_{a}(k)|O|φ_{b}(k)>.
@@ -209,15 +210,15 @@
 
 # ==================================================
 def fourier_transform_r_to_k_new(Or, kpoints, unit_cell_cart, irvec, ndegen=None, atoms_frac=None):
     """
     fourier transformation of an arbitrary operator from real-space representation into k-space representation.
 
     Args:
-        Or (ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(R)|O|φ_{b}(0)>.
+        Or (ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(0)|O|φ_{b}(R)>.
         kpoints (ndarray): k-points used in DFT calculation, [[k1, k2, k3]] (crystal coordinate).
         unit_cell_cart (ndarray): transform matrix, [a1,a2,a3], [None].
         irvec (ndarray): irreducible R vectors (crystal coordinate, [[n1,n2,n3]], nj: integer).
         ndegen (ndarray, optional): number of degeneracy at each R.
         atoms_frac (ndarray, optional): atom's position in fractional coordinates.
 
     Returns:
@@ -241,17 +242,16 @@
 
     if atoms_frac is not None:
         tau = np.array(atoms_frac)
         ktau = np.einsum("ka,ma->km", kpoints, tau, optimize=True)
         eiktau = np.exp(-2 * np.pi * 1j * ktau)
 
         atoms_cart = np.array([np.array(r) @ np.array(A) for r in atoms_frac])
-        print(atoms_cart.shape)
 
-        bond_cart = np.array([[[((R + rm) - rn) for rn in atoms_cart] for rm in atoms_cart] for R in irvec_cart])
+        bond_cart = np.array([[[(R + rn) - rm for rn in atoms_cart] for rm in atoms_cart] for R in irvec_cart])
 
         Ok = np.einsum("R,kR,km,Rmn,kn->kmn", weight, phase_R, eiktau, Or, eiktau.conjugate(), optimize=True)
         Ok_dx, Ok_dy, Ok_dz = 1.0j * np.einsum(
             "R,kR,Rmna,km,Rmn,kn->akmn", weight, phase_R, bond_cart, eiktau, Or, eiktau.conjugate(), optimize=True
         )
     else:
         Ok = np.einsum("R,kR,Rmn->kmn", weight, phase_R, Or, optimize=True)
@@ -287,15 +287,15 @@
 
 # ==================================================
 def matrix_dict_r(Or, rpoints, diagonal=False):
     """
     dictionary form of an arbitrary operator matrix in real-space representation.
 
     Args:
-        Or (ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(R)|O|φ_{b}(0)>.
+        Or (ndarray): real-space representation of the given operator, O_{ab}(R) = <φ_{a}(0)|O|φ_{b}(R)>.
         rpoints (ndarray): lattice points (crystal coordinate, [[n1,n2,n3]], nj: integer).
         diagonal (bool, optional): diagonal matrix ?
 
     Returns:
         dict: real-space representation of the given operator, {(n2,n2,n3,a,b) = O_{ab}(R)}.
     """
     # number of pseudo atomic orbitals
@@ -514,15 +514,15 @@
         z = {
             tag: np.sum(
                 [
                     np.real(v * v_)
                     for m, n in d.keys()
                     for bond, R1, R2, R3, v in d[(m, n)]
                     for bond_, R1_, R2_, R3_, v_ in Or[(n, m)]
-                    if np.allclose(bond, -bond_, rtol=1e-03, atol=1e-03)
+                    if np.allclose(bond, -bond_, rtol=1e-04, atol=1e-04)
                 ]
             )
             for tag, d in Zr_dict_.items()
         }
 
     return z
```

### Comparing `symclosestwannier-1.1.8/symclosestwannier/util/band.py` & `symclosestwannier-1.1.9/symclosestwannier/util/band.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/util/constants.py` & `symclosestwannier-1.1.9/symclosestwannier/util/constants.py`

 * *Files identical despite different names*

### Comparing `symclosestwannier-1.1.8/symclosestwannier/util/get_oper_R.py` & `symclosestwannier-1.1.9/symclosestwannier/util/get_oper_R.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,21 +20,20 @@
 
 import numpy as np
 
 from symclosestwannier.util._utility import fourier_transform_k_to_r
 
 
 # ==================================================
-def get_oper_R(name, cwi, tb_gauge=False):
+def get_oper_R(name, cwi):
     """
     wrapper for getting matrix elements of the operator.
 
     Args:
         cwi (SystemInfo): CWInfo.
-        tb_gauge (bool, optional): tb gauge?
 
     Returns:
         ndarray: matrix elements of the operator.
     """
     d = {
         "HH_R": get_HH_R,  # <0n|H|Rm>
         "AA_R": get_AA_R,  # <0n|r|Rm>
@@ -44,25 +43,24 @@
         "SR_R": get_SR_R,  # <0n|sigma_x,y,z.(r-R)_alpha|Rm>
         "SHR_R": get_SHR_R,  # <0n|sigma_x,y,z.H.(r-R)_alpha|Rm>
         "SH_R": get_SH_R,  # <0n|sigma_x,y,z.H|Rm>
         "SAA_R": get_SAA_R,  # <0n|sigma_x,y,z.(r-R)_alpha|Rm>
         "SBB_R": get_SBB_R,  # <0n|sigma_x,y,z.H.(r-R)_alpha|Rm>
     }
 
-    return d[name](cwi, tb_gauge)
+    return d[name](cwi)
 
 
 # ==================================================
-def get_HH_R(cwi, tb_gauge=False):
+def get_HH_R(cwi):
     """
     matrix elements of real-space Hamiltonian, <0n|H|Rm>.
 
     Args:
         cwi (SystemInfo): CWInfo.
-        tb_gauge (bool, optional): tb gauge?
 
     Returns:
         ndarray: Hamiltonian, HH_R(len(irvec), num_wann, num_wann).
     """
     Ek = np.array(cwi["Ek"])
     Uk = np.array(cwi["Uk"])
     num_k = cwi["num_k"]
@@ -70,33 +68,32 @@
     diag_Ek = np.array([np.diag(Ek[k]) for k in range(num_k)])
     HH_k = Uk.transpose(0, 2, 1).conjugate() @ diag_Ek @ Uk
     HH_k = 0.5 * (HH_k + np.einsum("kmn->knm", HH_k).conj())
 
     kpoints = np.array(cwi["kpoints"])
     irvec = np.array(cwi["irvec"])
 
-    if tb_gauge:
-        atoms_list = list(cwi["atoms_frac"].values())
-        atoms_frac = np.array([atoms_list[i] for i in cwi["nw2n"]])
-    else:
-        atoms_frac = None
+    # if cwi["tb_gauge"]:
+    #     atoms_list = list(cwi["atoms_frac"].values())
+    #     atoms_frac = np.array([atoms_list[i] for i in cwi["nw2n"]])
+    # else:
+    #     atoms_frac = None
 
-    HH_R = fourier_transform_k_to_r(HH_k, kpoints, irvec, atoms_frac)
+    HH_R = fourier_transform_k_to_r(HH_k, kpoints, irvec)
 
     return HH_R
 
 
 # ==================================================
-def get_AA_R(cwi, tb_gauge=False):
+def get_AA_R(cwi):
     """
     matrix elements of real-space position operator, <0n|r|Rm>.
 
     Args:
         cwi (SystemInfo): CWInfo.
-        tb_gauge (bool, optional): tb gauge?
 
     Returns:
         ndarray: position operator, AA_R(3, len(irvec), num_wann, num_wann).
     """
     Mkb = np.array(cwi["Mkb"])
     Uk = np.array(cwi["Uk"])
 
@@ -105,28 +102,30 @@
     wk = cwi.nnkp.wk()
 
     kpoints = np.array(cwi["kpoints"])
     irvec = np.array(cwi["irvec"])
 
     ### Unitary transform Mkb ###
     Mkb_w = np.einsum("klm, kblp, kbpn->kbmn", np.conj(Uk), Mkb, Uk[kb2k[:, :], :, :], optimize=True)  # Eq. (61)
-
     AA_k = 1j * np.einsum("kb,kba,kbmn->akmn", wk, bveck, Mkb_w, optimize=True)
-    AA_k_diag = -1 * np.einsum("kb,kba,kbnn->akn", wk, bveck, np.imag(np.log(Mkb_w)), optimize=True)
-    np.einsum("aknn->akn", AA_k)[:] = AA_k_diag
+
+    # Use Eq.(31) of Marzari&Vanderbilt PRB 56, 12847 (1997) for band-diagonal position matrix.
+    if cwi["transl_inv"]:
+        AA_k_diag = -1 * np.einsum("kb,kba,kbnn->akn", wk, bveck, np.imag(np.log(Mkb_w)), optimize=True)
+        np.einsum("aknn->akn", AA_k)[:] = AA_k_diag
 
     AA_k = 0.5 * (AA_k + np.einsum("akmn->aknm", AA_k).conj())
 
-    if tb_gauge:
-        atoms_list = list(cwi["atoms_frac"].values())
-        atoms_frac = np.array([atoms_list[i] for i in cwi["nw2n"]])
-    else:
-        atoms_frac = None
+    # if cwi["tb_gauge"]:
+    #     atoms_list = list(cwi["atoms_frac"].values())
+    #     atoms_frac = np.array([atoms_list[i] for i in cwi["nw2n"]])
+    # else:
+    #     atoms_frac = None
 
-    AA_R = np.array([fourier_transform_k_to_r(AA_k[i], kpoints, irvec, atoms_frac) for i in range(3)])
+    AA_R = np.array([fourier_transform_k_to_r(AA_k[i], kpoints, irvec) for i in range(3)])
 
     return AA_R
 
 
 # ==================================================
 def get_BB_R():
     """<0|H(r-R)|R>"""
@@ -136,35 +135,34 @@
 # ==================================================
 def get_CC_R():
     """<0|r_alpha.H(r-R)_beta|R>"""
     pass
 
 
 # ==================================================
-def get_SS_R(cwi, tb_gauge=False):
+def get_SS_R(cwi):
     """
     matrix elements of real-space spin operator, <0n|sigma_x,y,z|Rm>.
 
     Args:
         cwi (SystemInfo): CWInfo.
-        tb_gauge (bool, optional): tb gauge?
 
     Returns:
         ndarray: spin operator, SS_R(3, len(irvec), num_wann, num_wann).
     """
     Sk = np.array(cwi["Sk"])
     Uk = np.array(cwi["Uk"])
 
     SS_k = Uk.transpose(0, 2, 1).conjugate() @ Sk @ Uk
     SS_k = 0.5 * (SS_k + np.einsum("akmn->aknm", SS_k).conj())
 
     kpoints = np.array(cwi["kpoints"])
     irvec = np.array(cwi["irvec"])
 
-    if tb_gauge:
+    if cwi["tb_gauge"]:
         atoms_list = list(cwi["atoms_frac"].values())
         atoms_frac = np.array([atoms_list[i] for i in cwi["nw2n"]])
     else:
         atoms_frac = None
 
     SS_R = np.array([fourier_transform_k_to_r(SS_k[i], kpoints, irvec, atoms_frac) for i in range(3)])
 
@@ -203,21 +201,20 @@
 
 # ******************************************************************
 # ******************************************************************
 # ******************************************************************
 
 
 # ==================================================
-def get_berry_phase_R(cwi, tb_gauge=False):
+def get_berry_phase_R(cwi):
     """
     matrix elements of real-space spin operator, <0n|A_x,y,z|Rm>.
 
     Args:
         cwi (SystemInfo): CWInfo.
-        tb_gauge (bool, optional): tb gauge?
 
     Returns:
         ndarray: spin operator, SS_R(3, len(irvec), num_wann, num_wann).
     """
     Mkb = np.array(cwi["Mkb"])
     Uk = np.array(cwi["Uk"])
     num_wann = cwi["num_wann"]
@@ -232,18 +229,17 @@
     # i<wik|∇wjk>
     a_k = 1j * np.einsum("kb,kba,kbmn->akmn", wk, bveck, (Mkb_w - np.eye(num_wann)), optimize=True)
     a_k = 0.5 * (a_k + np.einsum("akmn->aknm", a_k.conj()))
 
     kpoints = np.array(cwi["kpoints"])
     irvec = np.array(cwi["irvec"])
 
-    if tb_gauge:
+    if cwi["tb_gauge"]:
         atoms_list = list(cwi["atoms_frac"].values())
         atoms_frac = np.array([atoms_list[i] for i in cwi["nw2n"]])
-        # atoms_frac = np.array([cwi["atom_pos_r"][idx] for idx in cwi["nw2n"]])
     else:
         atoms_frac = None
 
     a_R = np.array([fourier_transform_k_to_r(a_k[i], kpoints, irvec, atoms_frac) for i in range(3)])
 
     return a_R
```

### Comparing `symclosestwannier-1.1.8/symclosestwannier/util/header.py` & `symclosestwannier-1.1.9/symclosestwannier/util/header.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     "smearing_temp_max": "smearing temperature for upper window (float), [5.0].",
     "smearing_temp_min": "smearing temperature for lower window (float), [0.01].",
     "delta": "small constant to avoid ill-conditioning of overlap matrices (float), [1e-12].",
     "svd": "implement singular value decomposition ? otherwise adopt Lowdin's orthogonalization method (bool), [False].",
     "verbose": "verbose calculation info (bool, optional), [False].",
     "parallel": "use parallel code? (bool), [False].",
     "formatter": "format by using black? (bool), [False].",
+    "transl_inv": "use Eq.(31) of Marzari&Vanderbilt PRB 56, 12847 (1997) for band-diagonal position matrix elements? (bool), [True].",
+    "tb_gauge"          : "use tb gauge? (bool), [False].",
     "write_hr": "write seedname_hr.dat ? (bool), [False].",
     "write_sr": "write seedname_sr.dat ? (bool), [False].",
     "write_u_matrices": "write seedname_u.dat and seedname_u_dis.dat ? (bool), [False].",
     "write_rmn": "write seedname_r.dat ? (bool), [False].",
     "write_vmn": "write seedname_v.dat ? (bool), [False].",
     "write_tb": "write seedname_tb.dat ? (bool), [False].",
     "write_spn": "write seedname.spn.cw ? (bool), [False].",
@@ -89,14 +91,15 @@
     "A": "real lattice vectors, A = [a1,a2,a3] (list), [[[1,0,0], [0,1,0], [0,0,1]]].",
     "B": "reciprocal lattice vectors, B = [b1,b2,b3] (list), [[[2*pi,0,0], [0,2*pi,0], [0,0,2*pi]]].",
     "num_k": "# of k points (int), [1].",
     "num_wann": "# of WFs (int), [1].",
     "num_atom": "# of atoms (int), [1].",
     "num_b": "# of b-vectors (int), [1].",
     "kpoints": "k-points, [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].",
+    "kpoints_wo_shift": "k-points without shift, [[k1, k2, k3]] (crystal coordinate) (list), [[[0, 0, 0]]].",
     "nnkpts": "nearest-neighbour k-points (list), [None].",
     "nw2n": "atom position index of each WFs (list), [None].",
     "nw2l": "l specifies the angular part Θlm(θ, φ) (list), [None].",
     "nw2m": "m specifies the angular part Θlm(θ, φ) (list), [None].",
     "nw2r": "r specifies the radial part Rr(r) (list), [None].",
     "atom_orb": "WFs indexes of each atom (list), [None].",
     "atom_pos": "atom position index of each atom (list), [None].",
@@ -260,23 +263,23 @@
 - k = (k1,k2,k3) : k points (crystal coordinate).
 """
 
 
 hr_header = """
 === Hamiltonian matrix elements in real-space ===
 - n1 n2 n3 a b re(H_{ab}(R)) im(H_{ab}(R))
-    - H_{ab}(R)      : <φ_{a}(R)|H|φ_{b}(0)>.
+    - H_{ab}(R)      : <φ_{a}(0)|H|φ_{b}(R)>.
     - φ_{a}(R)       : orthogonalized pseudo atomic orbital.
     - R = (n1,n2,n3) : lattice points (crystal coordinate, nj: integer).
 """
 
 sr_header = """
 === Overlap matrix elements in real-space ===
 - n1 n2 n3 a b re(S_{ab}(R)) im(S_{ab}(R))
-    - S_{ab}(R)      : <φ_{a}(R)|φ_{b}(0)>.
+    - S_{ab}(R)      : <φ_{a}(0)|φ_{b}(R)>.
     - φ_{a}(R)       : non-orthogonalized pseudo atomic orbital.
     - R = (n1,n2,n3) : lattice points (crystal coordinate, nj: integer).
 """
 
 
 z_header = """
 === The expansion coefficients of the Hamiltonian matrix (orthogonal) H expressed by a linear combination of SAMBs ===
```

### Comparing `symclosestwannier-1.1.8/symclosestwannier/util/message.py` & `symclosestwannier-1.1.9/symclosestwannier/util/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
              |         Phys. Rev. B 107, 195118 (2023)           |
              |                                                   |
              |                                                   |
              | Copyright (c) 2023-                               |
              |     The SymClosestWwannier Developer Group and    |
              |        individual contributors                    |
              |                                                   |
-             |       Release: 1.1.8       22th January 2024      |
+             |       Release: 1.1.9       22th January 2024      |
              |                                                   |
              | This program is free software; you can            |
              | redistribute it and/or modify it under the terms  |
              | of the GNU General Public License as published by |
              | the Free Software Foundation; either version 2 of |
              | the License, or (at your option) any later version|
              |                                                   |
```

### Comparing `symclosestwannier-1.1.8/symclosestwannier.egg-info/PKG-INFO` & `symclosestwannier-1.1.9/symclosestwannier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symclosestwannier
-Version: 1.1.8
+Version: 1.1.9
 Summary: A Python library for Symmetry-Adapted Closest Wannier (SymCW) Tight-Binding model based on Plane-Wave DFT calculation.
 Home-page: https://github.com/CMT-MU/SymClosestWannier
 Author: Rikuto Oiwa
 Author-email: ro.qp.07@gmail.com
 License: MIT
 Keywords: dft,wannier function,tight-binding model,symmetry,materials science
 Requires-Python: >=3.9
```

### Comparing `symclosestwannier-1.1.8/symclosestwannier.egg-info/SOURCES.txt` & `symclosestwannier-1.1.9/symclosestwannier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

