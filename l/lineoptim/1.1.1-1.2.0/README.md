# Comparing `tmp/lineoptim-1.1.1.tar.gz` & `tmp/lineoptim-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineoptim-1.1.1.tar", last modified: Wed Apr 17 07:27:14 2024, max compression
+gzip compressed data, was "lineoptim-1.2.0.tar", last modified: Sat May 11 15:44:23 2024, max compression
```

## Comparing `lineoptim-1.1.1.tar` & `lineoptim-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 07:27:14.393663 lineoptim-1.1.1/
--rw-rw-rw-   0        0        0     1094 2024-02-25 15:16:35.000000 lineoptim-1.1.1/LICENCE
--rw-rw-rw-   0        0        0     3323 2024-04-17 07:27:14.381695 lineoptim-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2571 2024-04-17 07:17:15.000000 lineoptim-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 07:27:14.254035 lineoptim-1.1.1/lineoptim/
--rw-rw-rw-   0        0        0      140 2024-04-17 07:12:27.000000 lineoptim-1.1.1/lineoptim/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:27:14.359753 lineoptim-1.1.1/lineoptim/components/
--rw-rw-rw-   0        0        0      142 2024-04-10 05:13:14.000000 lineoptim-1.1.1/lineoptim/components/__init__.py
--rw-rw-rw-   0        0        0    11226 2024-04-12 05:13:19.000000 lineoptim-1.1.1/lineoptim/components/line.py
--rw-rw-rw-   0        0        0     4171 2024-04-12 05:00:58.000000 lineoptim-1.1.1/lineoptim/components/network.py
--rw-rw-rw-   0        0        0     3589 2024-04-17 04:57:28.000000 lineoptim-1.1.1/lineoptim/main.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:27:14.372720 lineoptim-1.1.1/lineoptim.egg-info/
--rw-rw-rw-   0        0        0     3323 2024-04-17 07:27:14.000000 lineoptim-1.1.1/lineoptim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2024-04-17 07:27:14.000000 lineoptim-1.1.1/lineoptim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 07:27:14.000000 lineoptim-1.1.1/lineoptim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-17 07:27:14.000000 lineoptim-1.1.1/lineoptim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-17 07:27:14.000000 lineoptim-1.1.1/lineoptim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 07:27:14.393663 lineoptim-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1208 2024-04-17 07:26:59.000000 lineoptim-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 15:44:23.093720 lineoptim-1.2.0/
+-rw-rw-rw-   0        0        0     1094 2024-02-25 15:16:35.000000 lineoptim-1.2.0/LICENCE
+-rw-rw-rw-   0        0        0     6012 2024-05-11 15:44:23.056817 lineoptim-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5235 2024-05-11 15:41:07.000000 lineoptim-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 15:44:22.760609 lineoptim-1.2.0/lineoptim/
+-rw-rw-rw-   0        0        0      180 2024-05-10 05:49:42.000000 lineoptim-1.2.0/lineoptim/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 15:44:22.917191 lineoptim-1.2.0/lineoptim/components/
+-rw-rw-rw-   0        0        0      142 2024-04-10 05:13:14.000000 lineoptim-1.2.0/lineoptim/components/__init__.py
+-rw-rw-rw-   0        0        0    13414 2024-05-10 05:30:18.000000 lineoptim-1.2.0/lineoptim/components/line.py
+-rw-rw-rw-   0        0        0     4236 2024-05-10 05:41:53.000000 lineoptim-1.2.0/lineoptim/components/network.py
+drwxrwxrwx   0        0        0        0 2024-05-11 15:44:23.004956 lineoptim-1.2.0/lineoptim/plot/
+-rw-rw-rw-   0        0        0      261 2024-05-10 04:49:32.000000 lineoptim-1.2.0/lineoptim/plot/__init__.py
+-rw-rw-rw-   0        0        0     4535 2024-04-27 05:52:45.000000 lineoptim-1.2.0/lineoptim/plot/graph.py
+-rw-rw-rw-   0        0        0    18183 2024-05-10 05:17:57.000000 lineoptim-1.2.0/lineoptim/plot/plotter.py
+drwxrwxrwx   0        0        0        0 2024-05-11 15:44:23.036872 lineoptim-1.2.0/lineoptim.egg-info/
+-rw-rw-rw-   0        0        0     6012 2024-05-11 15:44:22.000000 lineoptim-1.2.0/lineoptim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-05-11 15:44:22.000000 lineoptim-1.2.0/lineoptim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 15:44:22.000000 lineoptim-1.2.0/lineoptim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-11 15:44:22.000000 lineoptim-1.2.0/lineoptim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-11 15:44:22.000000 lineoptim-1.2.0/lineoptim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 15:44:23.094720 lineoptim-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1229 2024-05-10 05:55:52.000000 lineoptim-1.2.0/setup.py
```

### Comparing `lineoptim-1.1.1/LICENCE` & `lineoptim-1.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `lineoptim-1.1.1/lineoptim/components/network.py` & `lineoptim-1.2.0/lineoptim/components/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import json
+import numpy as np
 import logging
 import torch
 from torch import nn
 from torch.optim import Adam
-from torch import tensor
 import matplotlib.pyplot as plt
 
 from lineoptim.components import Line, compute_partial_voltages
 
 logger = logging.getLogger(__name__)
 
 logging.basicConfig(
@@ -33,15 +32,15 @@
         self.resistivity = nn.Parameter(line.get_resistivity_tensor(), requires_grad=True)
 
         print(f"Initial resistivity: {self.resistivity}")
 
     def forward(self):
         self.line.set_resistivity_tensor(self.resistivity)  # update resistivity
 
-        compute_partial_voltages(self.line, iterations=5)
+        self.line.recompute()  # recompute partial voltages
 
         dux = self.line.get_residual_voltage_tensor()  # compute residual voltage
 
         voltage_drop_percent = (1 - (dux / self.line['v_nominal'])) * 100  # convert to %
 
         return voltage_drop_percent
 
@@ -130,11 +129,13 @@
                 break
 
         # print results
         print(f'Predictions: {predictions}')
         print(f'Resulting resistivity: {model.resistivity}')
 
         # plot the loss
-        plt.plot(losses)
-        plt.xlabel('Epoch')
-        plt.ylabel('Loss')
-        plt.show()
+        fig, ax = plt.subplots()
+        fig.suptitle('Optimization loss')
+        ax.plot(losses)
+        ax.set_xlabel('Epoch')
+        ax.set_ylabel('Loss')
+        fig.show()
```

### Comparing `lineoptim-1.1.1/setup.py` & `lineoptim-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
       The lines in the README file.
   """
     with open("README.md", encoding="utf-8") as f:
         return f.read()
 
 setup(
     name='lineoptim',
-    version='1.1.1',
+    version='1.2.0',
     description='A line optimization package for electrical conductors.',
     author='David Senoner',
     author_email='david.senoner@gmail.com',
     long_description=fetch_readme(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
@@ -30,13 +30,14 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     install_requires=[
         "matplotlib",
         "numpy",
         "pandas",
-        "torch"
+        "torch",
+        "networkx"
     ],
     project_urls={
         "Github": "https://github.com/davidsenoner/lineoptim",
     },
 )
```

