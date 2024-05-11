# Comparing `tmp/pygformula-1.1.0.tar.gz` & `tmp/pygformula-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygformula-1.1.0.tar", last modified: Wed May  1 03:35:10 2024, max compression
+gzip compressed data, was "pygformula-1.1.1.tar", last modified: Sat May 11 00:34:09 2024, max compression
```

## Comparing `pygformula-1.1.0.tar` & `pygformula-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 03:35:10.857942 pygformula-1.1.0/
--rw-rw-rw-   0        0        0     1122 2024-04-18 20:33:45.000000 pygformula-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1451 2024-05-01 03:35:10.856943 pygformula-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2024-05-01 03:32:18.000000 pygformula-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 03:35:10.818853 pygformula-1.1.0/pygformula/
--rw-rw-rw-   0        0        0       53 2024-04-18 18:44:20.000000 pygformula-1.1.0/pygformula/__init__.py
--rw-rw-rw-   0        0        0    14167 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/comparisons.py
--rw-rw-rw-   0        0        0     9610 2024-04-18 20:32:39.000000 pygformula-1.1.0/pygformula/data.py
--rw-rw-rw-   0        0        0    12355 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/interventions.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:35:10.844169 pygformula-1.1.0/pygformula/parametric_gformula/
--rw-rw-rw-   0        0        0       55 2024-02-09 07:11:15.000000 pygformula-1.1.0/pygformula/parametric_gformula/__init__.py
--rw-rw-rw-   0        0        0    17447 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/parametric_gformula/bootstrap.py
--rw-rw-rw-   0        0        0    21378 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/parametric_gformula/fit.py
--rw-rw-rw-   0        0        0     8385 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/parametric_gformula/histories.py
--rw-rw-rw-   0        0        0    44696 2024-05-01 02:34:23.000000 pygformula-1.1.0/pygformula/parametric_gformula/parametric_gformula.py
--rw-rw-rw-   0        0        0    25089 2024-05-01 02:34:15.000000 pygformula-1.1.0/pygformula/parametric_gformula/simulate.py
--rw-rw-rw-   0        0        0    19939 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/plot.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:35:10.850931 pygformula-1.1.0/pygformula/utils/
--rw-rw-rw-   0        0        0        0 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/utils/__init__.py
--rw-rw-rw-   0        0        0     7677 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/utils/helper.py
--rw-rw-rw-   0        0        0    39587 2024-04-24 19:56:21.000000 pygformula-1.1.0/pygformula/utils/util.py
-drwxrwxrwx   0        0        0        0 2024-05-01 03:35:10.828166 pygformula-1.1.0/pygformula.egg-info/
--rw-rw-rw-   0        0        0     1451 2024-05-01 03:35:10.000000 pygformula-1.1.0/pygformula.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      624 2024-05-01 03:35:10.000000 pygformula-1.1.0/pygformula.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 03:35:10.000000 pygformula-1.1.0/pygformula.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-01 03:35:10.000000 pygformula-1.1.0/pygformula.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 03:35:10.858942 pygformula-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      421 2024-05-01 03:32:18.000000 pygformula-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:34:09.144175 pygformula-1.1.1/
+-rw-rw-rw-   0        0        0     1122 2024-04-18 20:33:45.000000 pygformula-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2032 2024-05-11 00:34:09.143335 pygformula-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1768 2024-05-11 00:11:03.000000 pygformula-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 00:34:09.106414 pygformula-1.1.1/pygformula/
+-rw-rw-rw-   0        0        0       87 2024-05-11 00:15:57.000000 pygformula-1.1.1/pygformula/__init__.py
+-rw-rw-rw-   0        0        0    14167 2024-04-18 20:33:45.000000 pygformula-1.1.1/pygformula/comparisons.py
+-rw-rw-rw-   0        0        0     9610 2024-04-18 20:32:39.000000 pygformula-1.1.1/pygformula/data.py
+-rw-rw-rw-   0        0        0    12355 2024-05-01 03:39:34.000000 pygformula-1.1.1/pygformula/interventions.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:34:09.131331 pygformula-1.1.1/pygformula/parametric_gformula/
+-rw-rw-rw-   0        0        0       55 2024-02-09 07:11:15.000000 pygformula-1.1.1/pygformula/parametric_gformula/__init__.py
+-rw-rw-rw-   0        0        0    17447 2024-04-18 20:33:45.000000 pygformula-1.1.1/pygformula/parametric_gformula/bootstrap.py
+-rw-rw-rw-   0        0        0    21378 2024-04-18 20:33:45.000000 pygformula-1.1.1/pygformula/parametric_gformula/fit.py
+-rw-rw-rw-   0        0        0     8385 2024-04-18 20:33:45.000000 pygformula-1.1.1/pygformula/parametric_gformula/histories.py
+-rw-rw-rw-   0        0        0    44696 2024-05-01 03:39:34.000000 pygformula-1.1.1/pygformula/parametric_gformula/parametric_gformula.py
+-rw-rw-rw-   0        0        0    25089 2024-05-01 03:39:34.000000 pygformula-1.1.1/pygformula/parametric_gformula/simulate.py
+-rw-rw-rw-   0        0        0    19939 2024-04-18 20:33:45.000000 pygformula-1.1.1/pygformula/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:34:09.139768 pygformula-1.1.1/pygformula/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-18 20:33:45.000000 pygformula-1.1.1/pygformula/utils/__init__.py
+-rw-rw-rw-   0        0        0     7677 2024-04-18 20:33:45.000000 pygformula-1.1.1/pygformula/utils/helper.py
+-rw-rw-rw-   0        0        0    39587 2024-04-24 19:56:21.000000 pygformula-1.1.1/pygformula/utils/util.py
+-rw-rw-rw-   0        0        0     1415 2024-05-11 00:30:39.000000 pygformula-1.1.1/pygformula/version.py
+drwxrwxrwx   0        0        0        0 2024-05-11 00:34:09.114028 pygformula-1.1.1/pygformula.egg-info/
+-rw-rw-rw-   0        0        0     2032 2024-05-11 00:34:08.000000 pygformula-1.1.1/pygformula.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      646 2024-05-11 00:34:08.000000 pygformula-1.1.1/pygformula.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 00:34:08.000000 pygformula-1.1.1/pygformula.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-11 00:34:08.000000 pygformula-1.1.1/pygformula.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 00:34:09.144175 pygformula-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      469 2024-05-11 00:17:58.000000 pygformula-1.1.1/setup.py
```

### Comparing `pygformula-1.1.0/LICENSE` & `pygformula-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygformula-1.1.0/PKG-INFO` & `pygformula-1.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-Metadata-Version: 2.1
-Name: pygformula
-Version: 1.1.0
-Summary: A python implementation of the parametric g-formula
-Maintainer: Jing Li
-Maintainer-email: jing_li@hsph.harvard.edu
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pygformula: a python implementation of the parametric g-formula
 
+[![PyPI version](https://badge.fury.io/py/pygformula.svg)](https://pypi.org/project/pygformula)
+[![Documentation Status](https://readthedocs.org/projects/pygformula/badge/?version=latest)](https://pygformula.readthedocs.io)
+
+**Authors: Jing Li, Sophia Rein, Sean McGrath, Roger Logan, Ryan O’Dea, Miguel Hernán**
+
 
 ## Overview
 The pygformula package implements the non-iterative conditional expectation (NICE) algorithm of the g-formula algorithm
-(Robins, 1986). The g-formula can estimate the counterfactual mean or risk of an outcome under hypothetical treatment strategies
+(Robins, 1986). The g-formula can estimate an outcome’s counterfactual mean or risk under hypothetical treatment strategies
 (interventions) when there is sufficient information on time-varying treatments and confounders.
 
 
 ### Features
 
 * Treatments: discrete or continuous time-varying treatments.
 * Outcomes: failure time outcomes or continuous/binary end of follow-up outcomes.
@@ -44,7 +40,12 @@
 - statsmodels
 - tqdm
 
 
 ## Documentation
 
 The online documentation is available at [pygformula documentation](https://pygformula.readthedocs.io).
+
+## Issues
+
+If you have any issues, please open an [issue](https://github.com/CausalInference/pygformula/issues) on github, we will 
+regularly check the questions. For any additional questions or comments, please email jing_li@hsph.harvard.edu.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygformula-1.1.0/pygformula/comparisons.py` & `pygformula-1.1.1/pygformula/comparisons.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.1.0/pygformula/data.py` & `pygformula-1.1.1/pygformula/data.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.1.0/pygformula/interventions.py` & `pygformula-1.1.1/pygformula/interventions.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.1.0/pygformula/parametric_gformula/bootstrap.py` & `pygformula-1.1.1/pygformula/parametric_gformula/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.1.0/pygformula/parametric_gformula/fit.py` & `pygformula-1.1.1/pygformula/parametric_gformula/fit.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.1.0/pygformula/parametric_gformula/histories.py` & `pygformula-1.1.1/pygformula/parametric_gformula/histories.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.1.0/pygformula/parametric_gformula/parametric_gformula.py` & `pygformula-1.1.1/pygformula/parametric_gformula/parametric_gformula.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.1.0/pygformula/parametric_gformula/simulate.py` & `pygformula-1.1.1/pygformula/parametric_gformula/simulate.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.1.0/pygformula/plot.py` & `pygformula-1.1.1/pygformula/plot.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.1.0/pygformula/utils/helper.py` & `pygformula-1.1.1/pygformula/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.1.0/pygformula/utils/util.py` & `pygformula-1.1.1/pygformula/utils/util.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.1.0/pygformula.egg-info/PKG-INFO` & `pygformula-1.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: pygformula
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python implementation of the parametric g-formula
 Maintainer: Jing Li
 Maintainer-email: jing_li@hsph.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pygformula: a python implementation of the parametric g-formula
 
+[![PyPI version](https://badge.fury.io/py/pygformula.svg)](https://pypi.org/project/pygformula)
+[![Documentation Status](https://readthedocs.org/projects/pygformula/badge/?version=latest)](https://pygformula.readthedocs.io)
+
+**Authors: Jing Li, Sophia Rein, Sean McGrath, Roger Logan, Ryan Oâ€™Dea, Miguel HernÃ¡n**
+
 
 ## Overview
 The pygformula package implements the non-iterative conditional expectation (NICE) algorithm of the g-formula algorithm
-(Robins, 1986). The g-formula can estimate the counterfactual mean or risk of an outcome under hypothetical treatment strategies
+(Robins, 1986). The g-formula can estimate an outcomeâ€™s counterfactual mean or risk under hypothetical treatment strategies
 (interventions) when there is sufficient information on time-varying treatments and confounders.
 
 
 ### Features
 
 * Treatments: discrete or continuous time-varying treatments.
 * Outcomes: failure time outcomes or continuous/binary end of follow-up outcomes.
@@ -44,7 +49,12 @@
 - statsmodels
 - tqdm
 
 
 ## Documentation
 
 The online documentation is available at [pygformula documentation](https://pygformula.readthedocs.io).
+
+## Issues
+
+If you have any issues, please open an [issue](https://github.com/CausalInference/pygformula/issues) on github, we will 
+regularly check the questions. For any additional questions or comments, please email jing_li@hsph.harvard.edu.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygformula-1.1.0/pygformula.egg-info/SOURCES.txt` & `pygformula-1.1.1/pygformula.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 pygformula/__init__.py
 pygformula/comparisons.py
 pygformula/data.py
 pygformula/interventions.py
 pygformula/plot.py
+pygformula/version.py
 pygformula.egg-info/PKG-INFO
 pygformula.egg-info/SOURCES.txt
 pygformula.egg-info/dependency_links.txt
 pygformula.egg-info/top_level.txt
 pygformula/parametric_gformula/__init__.py
 pygformula/parametric_gformula/bootstrap.py
 pygformula/parametric_gformula/fit.py
```

