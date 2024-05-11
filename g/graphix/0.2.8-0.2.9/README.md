# Comparing `tmp/graphix-0.2.8.tar.gz` & `tmp/graphix-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphix-0.2.8.tar", last modified: Sun Nov  5 06:47:31 2023, max compression
+gzip compressed data, was "graphix-0.2.9.tar", last modified: Wed Nov 29 13:56:35 2023, max compression
```

## Comparing `graphix-0.2.8.tar` & `graphix-0.2.9.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-11-05 06:47:31.078952 graphix-0.2.8/
--rw-r--r--   0 sunami     (501) staff       (20)    10761 2023-09-04 10:04:40.000000 graphix-0.2.8/LICENSE
--rw-r--r--   0 sunami     (501) staff       (20)      119 2023-09-29 12:52:52.000000 graphix-0.2.8/MANIFEST.in
--rw-r--r--   0 sunami     (501) staff       (20)     6446 2023-11-05 06:47:31.078686 graphix-0.2.8/PKG-INFO
--rw-r--r--   0 sunami     (501) staff       (20)     5089 2023-09-04 10:07:15.000000 graphix-0.2.8/README.md
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-11-05 06:47:31.073888 graphix-0.2.8/graphix/
--rw-r--r--   0 sunami     (501) staff       (20)      247 2023-09-04 10:04:40.000000 graphix-0.2.8/graphix/__init__.py
--rw-r--r--   0 sunami     (501) staff       (20)     7451 2023-09-04 10:04:40.000000 graphix-0.2.8/graphix/clifford.py
--rw-r--r--   0 sunami     (501) staff       (20)     3747 2023-11-05 06:08:41.000000 graphix-0.2.8/graphix/device_interface.py
--rw-r--r--   0 sunami     (501) staff       (20)     6304 2023-10-17 06:11:39.000000 graphix-0.2.8/graphix/extraction.py
--rw-r--r--   0 sunami     (501) staff       (20)     4187 2023-09-29 12:52:52.000000 graphix-0.2.8/graphix/generator.py
--rw-r--r--   0 sunami     (501) staff       (20)    13034 2023-09-04 10:07:15.000000 graphix-0.2.8/graphix/gflow.py
--rw-r--r--   0 sunami     (501) staff       (20)    14059 2023-10-04 01:55:38.000000 graphix-0.2.8/graphix/graphsim.py
--rw-r--r--   0 sunami     (501) staff       (20)     2463 2023-09-04 10:04:40.000000 graphix-0.2.8/graphix/ops.py
--rw-r--r--   0 sunami     (501) staff       (20)    72204 2023-10-17 06:11:39.000000 graphix-0.2.8/graphix/pattern.py
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-11-05 06:47:31.075217 graphix-0.2.8/graphix/sim/
--rw-r--r--   0 sunami     (501) staff       (20)        0 2023-09-04 10:04:40.000000 graphix-0.2.8/graphix/sim/__init__.py
--rw-r--r--   0 sunami     (501) staff       (20)    14254 2023-11-05 06:08:41.000000 graphix-0.2.8/graphix/sim/statevec.py
--rw-r--r--   0 sunami     (501) staff       (20)    26314 2023-09-04 10:04:40.000000 graphix-0.2.8/graphix/sim/tensornet.py
--rw-r--r--   0 sunami     (501) staff       (20)     2269 2023-09-20 05:37:02.000000 graphix-0.2.8/graphix/simulator.py
--rw-r--r--   0 sunami     (501) staff       (20)    37418 2023-09-29 12:52:52.000000 graphix-0.2.8/graphix/transpiler.py
--rw-r--r--   0 sunami     (501) staff       (20)       22 2023-11-05 06:09:26.000000 graphix-0.2.8/graphix/version.py
--rw-r--r--   0 sunami     (501) staff       (20)    22116 2023-10-17 06:11:39.000000 graphix-0.2.8/graphix/visualization.py
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-11-05 06:47:31.074675 graphix-0.2.8/graphix.egg-info/
--rw-r--r--   0 sunami     (501) staff       (20)     6446 2023-11-05 06:47:31.000000 graphix-0.2.8/graphix.egg-info/PKG-INFO
--rw-r--r--   0 sunami     (501) staff       (20)      842 2023-11-05 06:47:31.000000 graphix-0.2.8/graphix.egg-info/SOURCES.txt
--rw-r--r--   0 sunami     (501) staff       (20)        1 2023-11-05 06:47:31.000000 graphix-0.2.8/graphix.egg-info/dependency_links.txt
--rw-r--r--   0 sunami     (501) staff       (20)      144 2023-11-05 06:47:31.000000 graphix-0.2.8/graphix.egg-info/requires.txt
--rw-r--r--   0 sunami     (501) staff       (20)       14 2023-11-05 06:47:31.000000 graphix-0.2.8/graphix.egg-info/top_level.txt
--rw-r--r--   0 sunami     (501) staff       (20)       81 2023-09-04 10:04:40.000000 graphix-0.2.8/pyproject.toml
--rw-r--r--   0 sunami     (501) staff       (20)       96 2023-11-05 06:08:41.000000 graphix-0.2.8/requirements.txt
--rw-r--r--   0 sunami     (501) staff       (20)       38 2023-11-05 06:47:31.079003 graphix-0.2.8/setup.cfg
--rw-r--r--   0 sunami     (501) staff       (20)     1623 2023-11-05 06:08:41.000000 graphix-0.2.8/setup.py
-drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-11-05 06:47:31.078083 graphix-0.2.8/tests/
--rw-r--r--   0 sunami     (501) staff       (20)        0 2023-09-04 10:04:40.000000 graphix-0.2.8/tests/__init__.py
--rw-r--r--   0 sunami     (501) staff       (20)     2431 2023-09-04 10:04:40.000000 graphix-0.2.8/tests/random_circuit.py
--rw-r--r--   0 sunami     (501) staff       (20)     2904 2023-09-04 10:04:40.000000 graphix-0.2.8/tests/test_clifford.py
--rw-r--r--   0 sunami     (501) staff       (20)     4836 2023-10-17 06:11:39.000000 graphix-0.2.8/tests/test_extraction.py
--rw-r--r--   0 sunami     (501) staff       (20)     2986 2023-09-04 10:04:40.000000 graphix-0.2.8/tests/test_generator.py
--rw-r--r--   0 sunami     (501) staff       (20)     2479 2023-09-04 10:04:40.000000 graphix-0.2.8/tests/test_gflow.py
--rw-r--r--   0 sunami     (501) staff       (20)     3988 2023-09-04 10:07:15.000000 graphix-0.2.8/tests/test_graphsim.py
--rw-r--r--   0 sunami     (501) staff       (20)    16935 2023-09-29 12:52:52.000000 graphix-0.2.8/tests/test_pattern.py
--rw-r--r--   0 sunami     (501) staff       (20)     2104 2023-11-05 06:08:41.000000 graphix-0.2.8/tests/test_runner.py
--rw-r--r--   0 sunami     (501) staff       (20)     1509 2023-09-04 10:07:15.000000 graphix-0.2.8/tests/test_statevec_backend.py
--rw-r--r--   0 sunami     (501) staff       (20)    15771 2023-09-04 10:04:40.000000 graphix-0.2.8/tests/test_tnsim.py
--rw-r--r--   0 sunami     (501) staff       (20)     5102 2023-09-04 10:04:40.000000 graphix-0.2.8/tests/test_transpiler.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-11-29 13:56:35.308327 graphix-0.2.9/
+-rw-r--r--   0 sunami     (501) staff       (20)    10761 2023-11-29 10:28:14.000000 graphix-0.2.9/LICENSE
+-rw-r--r--   0 sunami     (501) staff       (20)      119 2023-09-29 12:52:52.000000 graphix-0.2.9/MANIFEST.in
+-rw-r--r--   0 sunami     (501) staff       (20)     6625 2023-11-29 13:56:35.308052 graphix-0.2.9/PKG-INFO
+-rw-r--r--   0 sunami     (501) staff       (20)     5188 2023-11-29 13:54:09.000000 graphix-0.2.9/README.md
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-11-29 13:56:35.303339 graphix-0.2.9/graphix/
+-rw-r--r--   0 sunami     (501) staff       (20)      247 2023-09-04 10:04:40.000000 graphix-0.2.9/graphix/__init__.py
+-rw-r--r--   0 sunami     (501) staff       (20)     7451 2023-09-04 10:04:40.000000 graphix-0.2.9/graphix/clifford.py
+-rw-r--r--   0 sunami     (501) staff       (20)     3746 2023-11-29 10:25:23.000000 graphix-0.2.9/graphix/device_interface.py
+-rw-r--r--   0 sunami     (501) staff       (20)     6304 2023-11-10 03:38:53.000000 graphix-0.2.9/graphix/extraction.py
+-rw-r--r--   0 sunami     (501) staff       (20)     4327 2023-11-25 06:11:19.000000 graphix-0.2.9/graphix/generator.py
+-rw-r--r--   0 sunami     (501) staff       (20)    14721 2023-11-29 10:25:23.000000 graphix-0.2.9/graphix/gflow.py
+-rw-r--r--   0 sunami     (501) staff       (20)    14059 2023-10-04 01:55:38.000000 graphix-0.2.9/graphix/graphsim.py
+-rw-r--r--   0 sunami     (501) staff       (20)     7895 2023-11-25 06:11:19.000000 graphix-0.2.9/graphix/linalg.py
+-rw-r--r--   0 sunami     (501) staff       (20)     2463 2023-09-04 10:04:40.000000 graphix-0.2.9/graphix/ops.py
+-rw-r--r--   0 sunami     (501) staff       (20)    72330 2023-11-25 06:11:19.000000 graphix-0.2.9/graphix/pattern.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-11-29 13:56:35.305022 graphix-0.2.9/graphix/sim/
+-rw-r--r--   0 sunami     (501) staff       (20)        0 2023-09-04 10:04:40.000000 graphix-0.2.9/graphix/sim/__init__.py
+-rw-r--r--   0 sunami     (501) staff       (20)    14325 2023-11-29 10:25:23.000000 graphix-0.2.9/graphix/sim/statevec.py
+-rw-r--r--   0 sunami     (501) staff       (20)    26314 2023-09-04 10:04:40.000000 graphix-0.2.9/graphix/sim/tensornet.py
+-rw-r--r--   0 sunami     (501) staff       (20)     2268 2023-11-28 01:07:43.000000 graphix-0.2.9/graphix/simulator.py
+-rw-r--r--   0 sunami     (501) staff       (20)    37429 2023-11-29 10:25:23.000000 graphix-0.2.9/graphix/transpiler.py
+-rw-r--r--   0 sunami     (501) staff       (20)       22 2023-11-29 13:47:07.000000 graphix-0.2.9/graphix/version.py
+-rw-r--r--   0 sunami     (501) staff       (20)    22530 2023-11-28 01:07:43.000000 graphix-0.2.9/graphix/visualization.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-11-29 13:56:35.307437 graphix-0.2.9/graphix.egg-info/
+-rw-r--r--   0 sunami     (501) staff       (20)     6625 2023-11-29 13:56:35.000000 graphix-0.2.9/graphix.egg-info/PKG-INFO
+-rw-r--r--   0 sunami     (501) staff       (20)      881 2023-11-29 13:56:35.000000 graphix-0.2.9/graphix.egg-info/SOURCES.txt
+-rw-r--r--   0 sunami     (501) staff       (20)        1 2023-11-29 13:56:35.000000 graphix-0.2.9/graphix.egg-info/dependency_links.txt
+-rw-r--r--   0 sunami     (501) staff       (20)      176 2023-11-29 13:56:35.000000 graphix-0.2.9/graphix.egg-info/requires.txt
+-rw-r--r--   0 sunami     (501) staff       (20)       14 2023-11-29 13:56:35.000000 graphix-0.2.9/graphix.egg-info/top_level.txt
+-rw-r--r--   0 sunami     (501) staff       (20)       81 2023-09-04 10:04:40.000000 graphix-0.2.9/pyproject.toml
+-rw-r--r--   0 sunami     (501) staff       (20)      111 2023-11-25 06:11:19.000000 graphix-0.2.9/requirements.txt
+-rw-r--r--   0 sunami     (501) staff       (20)       38 2023-11-29 13:56:35.308380 graphix-0.2.9/setup.cfg
+-rw-r--r--   0 sunami     (501) staff       (20)     1643 2023-11-29 10:26:29.000000 graphix-0.2.9/setup.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-11-29 13:56:35.307191 graphix-0.2.9/tests/
+-rw-r--r--   0 sunami     (501) staff       (20)        0 2023-09-04 10:04:40.000000 graphix-0.2.9/tests/__init__.py
+-rw-r--r--   0 sunami     (501) staff       (20)     2431 2023-09-04 10:04:40.000000 graphix-0.2.9/tests/random_circuit.py
+-rw-r--r--   0 sunami     (501) staff       (20)     2904 2023-09-04 10:04:40.000000 graphix-0.2.9/tests/test_clifford.py
+-rw-r--r--   0 sunami     (501) staff       (20)     4836 2023-11-10 03:38:53.000000 graphix-0.2.9/tests/test_extraction.py
+-rw-r--r--   0 sunami     (501) staff       (20)     3199 2023-11-25 06:11:19.000000 graphix-0.2.9/tests/test_generator.py
+-rw-r--r--   0 sunami     (501) staff       (20)     3950 2023-11-25 06:11:19.000000 graphix-0.2.9/tests/test_gflow.py
+-rw-r--r--   0 sunami     (501) staff       (20)     3988 2023-09-04 10:07:15.000000 graphix-0.2.9/tests/test_graphsim.py
+-rw-r--r--   0 sunami     (501) staff       (20)     7559 2023-11-25 06:11:19.000000 graphix-0.2.9/tests/test_linalg.py
+-rw-r--r--   0 sunami     (501) staff       (20)    16935 2023-09-29 12:52:52.000000 graphix-0.2.9/tests/test_pattern.py
+-rw-r--r--   0 sunami     (501) staff       (20)     2104 2023-11-25 06:11:19.000000 graphix-0.2.9/tests/test_runner.py
+-rw-r--r--   0 sunami     (501) staff       (20)     1509 2023-09-04 10:07:15.000000 graphix-0.2.9/tests/test_statevec_backend.py
+-rw-r--r--   0 sunami     (501) staff       (20)    15771 2023-09-04 10:04:40.000000 graphix-0.2.9/tests/test_tnsim.py
+-rw-r--r--   0 sunami     (501) staff       (20)     5102 2023-09-04 10:04:40.000000 graphix-0.2.9/tests/test_transpiler.py
```

### Comparing `graphix-0.2.8/LICENSE` & `graphix-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/PKG-INFO` & `graphix-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphix
-Version: 0.2.8
+Version: 0.2.9
 Summary: Optimize and simulate measurement-based quantum computation
 Home-page: https://graphix.readthedocs.io
 Author: Shinichi Sunami
 Author-email: shinichi.sunami@gmail.com
 Maintainer: Shinichi Sunami
 Maintainer-email: shinichi.sunami@gmail.com
 License: Apache License 2.0
@@ -20,21 +20,23 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy<1.26,>=1.22
 Requires-Dist: networkx>3.0
-Requires-Dist: z3-solver
 Requires-Dist: quimb>=1.4.0
 Requires-Dist: autoray>=0.6.0
 Requires-Dist: opt_einsum>=3.2
+Requires-Dist: galois>=0.3.0
+Requires-Dist: sympy>=1.9
 Requires-Dist: matplotlib
 Provides-Extra: extra
 Requires-Dist: graphix-ibmq; extra == "extra"
+Requires-Dist: graphix-perceval; extra == "extra"
 Provides-Extra: test
 Requires-Dist: qiskit; extra == "test"
 Requires-Dist: qiskit-aer; extra == "test"
 
 <img src="https://github.com/TeamGraphix/graphix/raw/master/docs/logo/black_with_name.png" alt="logo" width="550">
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graphix)
@@ -60,18 +62,18 @@
 $ pip install graphix
 ```
 
 Install together with device interface:
 ```bash
 $ pip install graphix[extra]
 ```
-this will install `graphix` and [IBMQ interface](https://github.com/TeamGraphix/graphix-ibmq) to run MBQC patterns on IBM devices and Aer simulator.
+this will install `graphix` and inteface for [IBMQ](https://github.com/TeamGraphix/graphix-ibmq) and [Perceval](https://github.com/TeamGraphix/graphix-perceval) to run MBQC patterns on superconducting and optical QPUs and their simulators.
 
-We are currently adding more quantum device interfaces.
-Please suggest in [issues](https://github.com/TeamGraphix/graphix/issues) if you have any particular device in mind!
+<!-- We are currently adding more quantum device interface.
+Please suggest in [issues](https://github.com/TeamGraphix/graphix/issues) if you have any particular device in mind! -->
 
 
 ## Next Steps
 
 - We have a few [demos](https://graphix.readthedocs.io/en/latest/gallery/index.html) showing basic usages of `Graphix`.
 - You can run demos on your browser:
   - Preprocessing Clifford gates: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=deutsch-jozsa.ipynb)
```

### Comparing `graphix-0.2.8/README.md` & `graphix-0.2.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 $ pip install graphix
 ```
 
 Install together with device interface:
 ```bash
 $ pip install graphix[extra]
 ```
-this will install `graphix` and [IBMQ interface](https://github.com/TeamGraphix/graphix-ibmq) to run MBQC patterns on IBM devices and Aer simulator.
+this will install `graphix` and inteface for [IBMQ](https://github.com/TeamGraphix/graphix-ibmq) and [Perceval](https://github.com/TeamGraphix/graphix-perceval) to run MBQC patterns on superconducting and optical QPUs and their simulators.
 
-We are currently adding more quantum device interfaces.
-Please suggest in [issues](https://github.com/TeamGraphix/graphix/issues) if you have any particular device in mind!
+<!-- We are currently adding more quantum device interface.
+Please suggest in [issues](https://github.com/TeamGraphix/graphix/issues) if you have any particular device in mind! -->
 
 
 ## Next Steps
 
 - We have a few [demos](https://graphix.readthedocs.io/en/latest/gallery/index.html) showing basic usages of `Graphix`.
 - You can run demos on your browser:
   - Preprocessing Clifford gates: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=deutsch-jozsa.ipynb)
```

### Comparing `graphix-0.2.8/graphix/clifford.py` & `graphix-0.2.9/graphix/clifford.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/graphix/device_interface.py` & `graphix-0.2.9/graphix/device_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     Executes the measurement pattern.
     """
 
     def __init__(self, pattern, backend="ibmq", **kwargs):
         """
 
-        Parameteres
+        Parameters
         -----------
         pattern: :class:`graphix.pattern.Pattern` object
             MBQC pattern to be executed.
         backend_name: str, optional
             execution backend, default is 'ibmq'.
         kwargs: dict
             keyword args for specified backend.
```

### Comparing `graphix-0.2.8/graphix/extraction.py` & `graphix-0.2.9/graphix/extraction.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/graphix/generator.py` & `graphix-0.2.9/graphix/generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 import numpy as np
 from graphix.pattern import Pattern
 from graphix.gflow import flow, gflow, get_layers, find_odd_neighbor
 
 
-def generate_from_graph(graph, angles, inputs, outputs, timeout=100):
+def generate_from_graph(graph, angles, inputs, outputs, meas_planes=None):
     r"""Generate the measurement pattern from open graph and measurement angles.
 
     This function takes an open graph G = (nodes, edges, input, outputs),
     specified by networks.Graph and two lists specifying input and output nodes.
     Currently we support XY-plane measurements.
 
     Searches for the flow in the open graph using :func:`flow` and if found,
@@ -40,27 +40,30 @@
         graph on which MBQC should be performed
     angles : dict
         measurement angles for each nodes on the graph (unit of pi), except output nodes
     inputs : list
         list of node indices for input nodes
     outputs : list
         list of node indices for output nodes
-    timeout : int
-        optional argument for flow and gflow search depth
+    meas_planes : dict(optional)
+        measurement planes for each nodes on the graph, except output nodes
 
     Returns
     -------
     pattern : graphix.pattern.Pattern object
         constructed pattern.
     """
     assert len(inputs) == len(outputs)
     measuring_nodes = list(set(graph.nodes) - set(outputs) - set(inputs))
 
+    if meas_planes is None:
+        meas_planes = {i: "XY" for i in measuring_nodes}
+
     # search for flow first
-    f, l_k = flow(graph, set(inputs), set(outputs), timeout=timeout)
+    f, l_k = flow(graph, set(inputs), set(outputs), meas_planes=meas_planes)
     if f:
         # flow found
         depth, layers = get_layers(l_k)
         pattern = Pattern(input_nodes=inputs, output_nodes=outputs, width=len(inputs))
         pattern.seq = [["N", i] for i in inputs]
         for i in set(graph.nodes) - set(inputs):
             pattern.seq.append(["N", i])
@@ -74,15 +77,15 @@
                 for k in set(graph.neighbors(f[j])) - set([j]):
                     if k not in measured:
                         pattern.seq.append(["Z", k, [j]])
                 pattern.seq.append(["X", f[j], [j]])
         pattern.Nnode = len(graph.nodes)
     else:
         # no flow found - we try gflow
-        g, l_k = gflow(graph, set(inputs), set(outputs), timeout=timeout)
+        g, l_k = gflow(graph, set(inputs), set(outputs), meas_planes=meas_planes)
         if g:
             # gflow found
             depth, layers = get_layers(l_k)
             pattern = Pattern(input_nodes=inputs, output_nodes=outputs, width=len(inputs))
             pattern.seq = [["N", i] for i in inputs]
             for i in set(graph.nodes) - set(inputs):
                 pattern.seq.append(["N", i])
```

### Comparing `graphix-0.2.8/graphix/gflow.py` & `graphix-0.2.9/graphix/gflow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,354 +1,324 @@
-"""Optimum generalized flow finding algorithm
+"""flow finding algorithm
 
-For a given open graph (G, I, O), this iterative method
-finds a generalized flow (gflow) [NJP 9, 250 (2007)] in polynomial time.
-In particular, this outputs gflow with minimum depth.
-We implemented a modification according to definition of
-Pauli flow (NJP 9, 250 (2007)).
+For a given underlying graph (G, I, O, meas_plane), this method finds a (generalized) flow [NJP 9, 250 (2007)]
+in polynomincal time.
+In particular, this outputs gflow with minimum depth, maximally delayed gflow.
 
 Ref: Mhalla and Perdrix, International Colloquium on Automata,
 Languages, and Programming (Springer, 2008), pp. 857-868.
+Ref: Backens et al., Quantum 5, 421 (2021).
 
 """
 
+from itertools import product
+
 import networkx as nx
 import numpy as np
-import z3
-import copy
-
-
-def solvebool(A, b):
-    """solves linear equations of booleans
-
-    Solves Ax=b, where A is n*m matrix and b is 1*m array, both of booleans.
-    for example, for A=[[0,1,1],[1,0,1]] and b=[1,0], we solve:
-        XOR(x1,x2) = 1
-
-        XOR(x0,x2) = 0
-    for which (one of) the solution is [x0,x1,x2]=[1,0,1]
-
-    Uses Z3, a theorem prover from Microsoft Research.
-
-    Parameters
-    ----------
-    A: np.array
-        n*m array of 1s and 0s, or booleans
-    b: np.array
-        length m array of 1s and 0s, or booleans
-
-    Returns
-    --------
-    x: np.array
-        length n array of 1s and 0s satisfying Ax=b.
-        if no solution is found, returns False.
-    """
+import sympy as sp
 
-    def xor_n(a):
-        if len(a) == 1:
-            return a[0]
-        elif len(a) > 1:
-            return z3.Xor(a[0], xor_n(a[1:]))
-
-    # create list of params
-    p = []
-    for i in range(A.shape[1]):
-        p.append(z3.Bool(i))
-    p = np.array(p)
-
-    # add constraints
-    s = z3.Solver()
-    for i in range(len(b)):
-        arr = np.asarray(A[i, :]).flatten().astype(np.bool8)
-        if arr.any():
-            if b[i] == 0:
-                s.add(z3.Not(xor_n(p[arr])))
-            else:
-                s.add(xor_n(p[arr]))
-
-    # solve
-    if s.check() == z3.sat:  # there's solution
-        ans = s.model()
-        return np.array([ans[p[i]] for i in range(A.shape[1])])
-    else:  # no solution found
-        return False
+from graphix.linalg import MatGF2
 
 
-def gflow(g, v_in, v_out, meas_plane=None, timeout=1000):
-    """Optimum generalized flow finding algorithm
+def gflow(graph, input, output, meas_planes, mode="single"):
+    """Maximally delayed gflow finding algorithm
 
-    For open graph g with input and output, this returns optimum gflow.
+    For open graph g with input, output, and measurement planes, this returns maximally delayed gflow.
 
     gflow consist of function g(i) where i is the qubit labels,
     and strict partial ordering < or layers labels l_k where each element
     specify the order of qubits to be measured to maintain determinism in MBQC.
     In practice, we must measure qubits in order specified in array l_k (increasing order
     of l_k from 1), and for each measurements of qubit i we must perform corrections on
     qubits in g(i), depending on the measurement outcome.
 
     For more details of gflow, see Browne et al., NJP 9, 250 (2007).
-
-    Original algorithm by Mhalla and Perdrix,
-    International Colloquium on Automata, Languages, and Programming (Springer, 2008),
-    pp. 857-868.
+    We use the extended gflow finding algorithm in Backens et al., Quantum 5, 421 (2021).
 
     Parameters
     ----------
-    g: nx.Graph
+    graph: nx.Graph
         graph (incl. in and out)
-    v_in: set
+    input: set
         set of node labels for input
-    v_out: set
+    output: set
         set of node labels for output
-    timeout: int
-        number of iterations allowed before timeout
+    meas_planes: dict
+        measurement planes for each qubits. meas_planes[i] is the measurement plane for qubit i.
+    mode: str(optional)
+        The gflow finding algorithm can yield multiple equivalent solutions. So there are three options
+            - "single": Returrns a single solution
+            - "all": Returns all possible solutions
+            - "abstract": Returns an abstract solution. Uncertainty is represented with sympy.Symbol objects,
+              requiring user substitution to get a concrete answer.
+
+        Default is "single".
 
     Returns
     -------
-    g: list of sets
-        list of length |g| where each set is the correcting nodes for
-        the measurements of each qubits. function g() in gflow.
-    l_k: np.array
-        1D array of length |g|, where elements are layer of each qubits
-        corresponds to the strict partial ordering < in gflow.
-        Measurements must proceed in decreasing order of layer numbers.
+    g: dict
+        gflow function. g[i] is the set of qubits to be corrected for the measurement of qubit i.
+    l_k: dict
+        layers obtained by gflow algorithm. l_k[d] is a node set of depth d.
     """
-    v = set(g.nodes)
-    if meas_plane is None:
-        meas_plane = {u: "XY" for u in v}
-
-    gamma = nx.to_numpy_array(g)  # adjacency matrix
-    index_list = list(g.nodes)  # match g.nodes with gamma's index
-    l_k = {i: 0 for i in v}  # contains k, layer number initialized to default (0).
-    g = dict()  # contains the correction set g(i) for i\in V.
-    k = 1
-    vo = copy.deepcopy(v_out)
-    finished = False
-    count = 0
-    while not finished:
-        count += 1
-        vo, g, l_k, finished, exist = gflowaux(v, gamma, index_list, v_in, vo, g, l_k, k, meas_plane)
-        k = k + 1
-        if not exist:
-            return None, None
-        if count > timeout:
-            raise TimeoutError("max iteration number n={} reached".format(timeout))
-    return g, l_k
-
-
-def gflowaux(v, gamma, index_list, v_in, v_out, g, l_k, k, meas_plane):
+    l_k = dict()
+    g = dict()
+    for node in graph.nodes:
+        l_k[node] = 0
+    return gflowaux(graph, input, output, meas_planes, 1, l_k, g, mode=mode)
+
+
+def gflowaux(
+    graph,
+    input: set,
+    output: set,
+    meas_planes: dict,
+    k: int,
+    l_k: dict,
+    g: dict,
+    mode,
+):
     """Function to find one layer of the gflow.
 
-    Ref: Mhalla and Perdrix, International Colloquium on Automata,
-    Languages, and Programming (Springer, 2008), pp. 857-868.
+    Ref: Backens et al., Quantum 5, 421 (2021).
 
     Parameters
     ----------
-    v: set
-        labels of all qubits (nodes)
-    gamma: np.array
-        adjacency matrix of graph
-    index_list: list of ints
-        this list connects between index of gamma and node number of Graph.
-    v_in: set
-        input qubit set
-    v_out: set
-        output qubit set U set of qubits in layers 0...k-1.
-    g: list of sets
-        g(i) for all qubits i
-    l_k: np.array
-        1D array for all qubits labeling layer number
-    k: current layer number.
-    meas_plane: array of length |v| containing 'X','Y','Z','XY','YZ','XZ'.
-        measurement planes xy, yz, xz or Pauli measurement x,y,z.
+    graph: nx.Graph
+        graph (incl. in and out)
+    input: set
+        set of node labels for input
+    output: set
+        set of node labels for output
+    meas_planes: dict
+        measurement planes for each qubits. meas_planes[i] is the measurement plane for qubit i.
+    k: int
+        current layer number.
+    l_k: dict
+        layers obtained by gflow algorithm. l_k[d] is a node set of depth d.
+    g: dict
+        gflow function. g[i] is the set of qubits to be corrected for the measurement of qubit i.
+    mode: str(optional)
+        The gflow finding algorithm can yield multiple equivalent solutions. So there are three options
+            - "single": Returrns a single solution
+            - "all": Returns all possible solutions
+            - "abstract": Returns an abstract solution. Uncertainty is represented with sympy.Symbol objects,
+              requiring user substitution to get a concrete answer.
 
-    Outputs
+    Returns
     -------
-    v_out: set
-        output qubit set U set of qubits in layers 0...k+1.
-    g: list of sets
-        updated g(i) for all qubits i
-    l_k: np.array
-        updated 1D array for all qubits labeling layer number
-    finished: bool
-        whether iteration ends or not
-    exist: bool
-        whether gflow exists or not
+    g: dict
+        gflow function. g[i] is the set of qubits to be corrected for the measurement of qubit i.
+    l_k: dict
+        layers obtained by gflow algorithm. l_k[d] is a node set of depth d.
     """
 
-    c_set = set()
-    v_rem = v - v_out  # remaining vertices
-    v_rem_list = list(v_rem)
-    n = len(v_rem)
-    v_correct = v_out - v_in
-    v_correct_list = list(v_correct)
-
-    index_0 = [[index_list.index(i)] for i in iter(v_rem)]  # for slicing rows
-    index_1 = [index_list.index(i) for i in iter(v_correct)]  # for slicing columns
-
-    # if index_0 or index_1 is blank, skip the calculation below
-    if len(index_0) * len(index_1):
-        gamma_sub = gamma[index_0, index_1]
-
-        for u in iter(v_rem):
-            if meas_plane[u] == "Z":
-                c_set = c_set | {u}
-                g[u] = set()
-                l_k[u] = k
-                continue
-            elif meas_plane[u] in ["XY", "XZ", "X", "Y"]:
-                Iu = np.zeros(n, dtype=np.int8)
-                Iu[v_rem_list.index(u)] = 1
-            elif meas_plane[u] == "YZ":
-                Iu = np.ones(n, dtype=np.int8)
-                Iu[v_rem_list.index(u)] = 0
-
-            Ix = solvebool(gamma_sub.astype(np.int8), Iu.astype(np.int8))
-            inds = np.where(Ix)[0]
-
-            if len(inds) > 0:  # has solution
-                c_set = c_set | {u}
-                g[u] = set(v_correct_list[ind_] for ind_ in inds)
-                l_k[u] = k
-    if not c_set:
-        finished = True
-        if v_out == v:
-            exist = True
+    nodes = set(graph.nodes)
+    if output == nodes:
+        return g, l_k
+    non_output = nodes - output
+    correction_candidate = output - input
+    adj_mat, node_order_list = get_adjacency_matrix(graph)
+    node_order_row = node_order_list.copy()
+    node_order_row.sort()
+    node_order_col = node_order_list.copy()
+    node_order_col.sort()
+    for out in output:
+        adj_mat.remove_row(node_order_row.index(out))
+        node_order_row.remove(out)
+    adj_mat_row_reduced = adj_mat.copy()  # later use for construct RHS
+    for node in nodes - correction_candidate:
+        adj_mat.remove_col(node_order_col.index(node))
+        node_order_col.remove(node)
+
+    b = MatGF2(np.zeros((adj_mat.data.shape[0], len(non_output)), dtype=int))
+    for i_row in range(len(node_order_row)):
+        node = node_order_row[i_row]
+        vec = MatGF2(np.zeros(len(node_order_row), dtype=int))
+        if meas_planes[node] == "XY":
+            vec.data[i_row] = 1
+        elif meas_planes[node] == "XZ":
+            vec.data[i_row] = 1
+            vec_add = adj_mat_row_reduced.data[:, node_order_list.index(node)]
+            vec = vec + vec_add
+        elif meas_planes[node] == "YZ":
+            vec.data = adj_mat_row_reduced.data[:, i_row].reshape(vec.data.shape)
+        b.data[:, i_row] = vec.data
+
+    adj_mat, b, _, col_pertumutation = adj_mat.forward_eliminate(b)
+    x, kernels = adj_mat.backward_substitute(b)
+
+    corrected_nodes = set()
+    for i_row in range(len(node_order_row)):
+        non_out_node = node_order_row[i_row]
+        x_col = x[:, i_row]
+        if x_col[0] == sp.nan:  # no solution
+            continue
+        if mode == "single":
+            sol_list = [x_col[i].subs(zip(kernels, [sp.false] * len(kernels))) for i in range(len(x_col))]
+            sol = np.array(sol_list)
+            sol_index = sol.nonzero()[0]
+            g[non_out_node] = set(node_order_col[col_pertumutation[i]] for i in sol_index)
+            if meas_planes[non_out_node] in ["XZ", "YZ"]:
+                g[non_out_node] |= {non_out_node}
+
+        elif mode == "all":
+            g[non_out_node] = set()
+            binary_combinations = product([0, 1], repeat=len(kernels))
+            for binary_combination in binary_combinations:
+                sol_list = [x_col[i].subs(zip(kernels, binary_combination)) for i in range(len(x_col))]
+                kernel_list = [True if i == 1 else False for i in binary_combination]
+                sol_list.extend(kernel_list)
+                sol = np.array(sol_list)
+                sol_index = sol.nonzero()[0]
+                g_i = set(node_order_col[col_pertumutation[i]] for i in sol_index)
+                if meas_planes[non_out_node] in ["XZ", "YZ"]:
+                    g_i |= {non_out_node}
+
+                g[non_out_node] |= {frozenset(g_i)}
+
+        elif mode == "abstract":
+            g[non_out_node] = dict()
+            for i in range(len(x_col)):
+                node = node_order_col[col_pertumutation[i]]
+                g[non_out_node][node] = x_col[i]
+            for i in range(len(kernels)):
+                g[non_out_node][node_order_col[col_pertumutation[len(x_col) + i]]] = kernels[i]
+            if meas_planes[non_out_node] in ["XZ", "YZ"]:
+                g[non_out_node][non_out_node] = sp.true
+
+        l_k[non_out_node] = k
+        corrected_nodes |= {non_out_node}
+
+    if len(corrected_nodes) == 0:
+        if output == nodes:
+            return g, l_k
         else:
-            exist = False
+            return None, None
     else:
-        finished = False
-        exist = True
-
-    return v_out | c_set, g, l_k, finished, exist
+        return gflowaux(
+            graph,
+            input,
+            output | corrected_nodes,
+            meas_planes,
+            k + 1,
+            l_k,
+            g,
+            mode=mode,
+        )
 
 
-def flow(g, v_in, v_out, meas_plane=None, timeout=10000):
+def flow(graph, input, output, meas_planes=None):
     """Causal flow finding algorithm
 
-    For open graph g with input and output, this returns causal flow.
-
+    For open graph g with input, output, and measurement planes, this returns causal flow.
     For more detail of causal flow, see Danos and Kashefi, PRA 74, 052310 (2006).
 
     Original algorithm by Mhalla and Perdrix,
     International Colloquium on Automata, Languages, and Programming (2008),
     pp. 857-868.
 
     Parameters
     ----------
-    g: nx.Graph
+    graph: nx.Graph
         graph (incl. in and out)
-    v_in: set
+    input: set
         set of node labels for input
-    v_out: set
+    output: set
         set of node labels for output
-    timeout: int
-        number of iterations allowed before timeout
+    meas_planes: int(optional)
+        measurement planes for each qubits. meas_planes[i] is the measurement plane for qubit i.
+        Note that an underlying graph has a causal flow only if all measurement planes are "XY".
+        If not specified, all measurement planes are interpreted as "XY".
 
     Returns
     -------
     f: list of nodes
-        list of length |g| where each node corrects the measurements of each qubits. function f() in flow.
-    l_k: np.array
-        1D array of length |g|, where elements are layer of each qubits
-        corresponds to the strict partial ordering < in flow.
-        Measurements must proceed in decreasing order of layer numbers.
+        causal flow function. f[i] is the qubit to be measured after qubit i.
+    l_k: dict
+        layers obtained by gflow algorithm. l_k[d] is a node set of depth d.
     """
-    v = set(g.nodes)
-    e = set(g.edges)
+    nodes = set(graph.nodes)
+    edges = set(graph.edges)
 
-    l_k = {i: 0 for i in v}
+    if meas_planes is None:
+        meas_planes = {i: "XY" for i in (nodes - output)}
+
+    for plane in meas_planes.values():
+        if plane not in ["X", "Y", "XY"]:
+            return None, None
+
+    l_k = {i: 0 for i in nodes}
     f = dict()
     k = 1
-    vo = copy.deepcopy(v_out)
-    finished = False
-    exist = True
-    count = 0
-    v_c = v_out - v_in
-    while not finished:
-        count += 1
-        vo, v_c, f, l_k, finished, exist = flowaux(v, e, v_in, vo, v_c, f, l_k, k)
-        k += 1
-        if not exist:
-            return None, None
-        if count > timeout:
-            raise TimeoutError("max iteration number n={} reached".format(timeout))
-    return f, l_k
+    v_c = output - input
+    return flowaux(nodes, edges, input, output, v_c, f, l_k, k)
 
 
-def flowaux(v, e, v_in, v_out, v_c, f, l_k, k):
+def flowaux(nodes, edges, input, output, v_c, f, l_k, k):
     """Function to find one layer of the flow.
 
     Ref: Mhalla and Perdrix, International Colloquium on Automata,
     Languages, and Programming (Springer, 2008), pp. 857-868.
 
     Parameters
     ----------
-    v: set
+    nodes: set
         labels of all qubits (nodes)
-    e: set
+    edges: set
         edges
-    v_in: set
-        input qubit set
-    v_out: set
-        output qubit set U set of qubits in layers 0...k-1.
+    input: set
+        set of node labels for input
+    output: set
+        set of node labels for output
     v_c: set
-        correction qubit set in layer k
-    f: list of sets
-        f(i) for all qubits i
-    l_k: np.array
-        1D array for all qubits labeling layer number
-    k: current layer number.
-    meas_plane: array of length |v| containing 'x','y','z','xy','yz',xz'.
-        measurement planes xy, yz, xz or Pauli measurement x,y,z.
+        correction candidate qubits
+    f: dict
+        flow function. f[i] is the qubit to be measured after qubit i.
+    l_k: dict
+        layers obtained by flow algorithm. l_k[d] is a node set of depth d.
+    k: int
+        current layer number.
+    meas_planes: dict
+        measurement planes for each qubits. meas_planes[i] is the measurement plane for qubit i.
 
     Outputs
     -------
-    v_out: set
-        output qubit set U set of qubits in layers 0...k+1.
-    v_c: set
-        correction qubit set updated in the k-th layer.
-    f: list of sets
-        updated f(i) for all qubits i
-    l_k: np.array
-        updated 1D array for all qubits labeling layer number
-    finished: bool
-        whether iteration ends or not
-    exist: bool
-        whether gflow exists or not
+    f: list of nodes
+        causal flow function. f[i] is the qubit to be measured after qubit i.
+    l_k: dict
+        layers obtained by gflow algorithm. l_k[d] is a node set of depth d.
     """
     v_out_prime = set()
     c_prime = set()
 
     for q in v_c:
-        N = search_neighbor(q, e)
-        p_set = N & (v - v_out)
+        N = search_neighbor(q, edges)
+        p_set = N & (nodes - output)
         if len(p_set) == 1:
             p = list(p_set)[0]
             f[p] = q
             l_k[p] = k
             v_out_prime = v_out_prime | {p}
             c_prime = c_prime | {q}
     # determine whether there exists flow
     if not v_out_prime:
-        finished = True
-        if v_out == v:
-            exist = True
+        if output == nodes:
+            return f, l_k
         else:
-            exist = False
-    else:
-        finished = False
-        exist = True
-    return (
-        v_out | v_out_prime,
-        (v_c - c_prime) | (v_out_prime & (v - v_in)),
+            return None, None
+    return flowaux(
+        nodes,
+        edges,
+        input,
+        output | v_out_prime,
+        (v_c - c_prime) | (v_out_prime & (nodes - input)),
         f,
         l_k,
-        finished,
-        exist,
+        k + 1,
     )
 
 
 def search_neighbor(node, edges):
     """Function to find neighborhood of node in edges. This is an ancillary method for `flowaux()`.
 
     Parameter
@@ -368,42 +338,51 @@
         if node == edge[0]:
             N = N | {edge[1]}
         elif node == edge[1]:
             N = N | {edge[0]}
     return N
 
 
-def find_flow(g, v_in, v_out, meas_plane=None, timeout=100):
+def find_flow(graph, input, output, meas_planes=None, mode="single"):
     """Function to determine whether there exists flow or gflow
 
     Parameters
     ---------
-    g: nx.Graph
+    graph: nx.Graph
         graph (incl. in and out)
-    v_in: set
+    input: set
         set of node labels for input
-    v_out: set
+    output: set
         set of node labels for output
-    timeout: int
-        number of iterations allowed before timeout
+    meas_planes: dict(optional)
+        measurement planes for each qubits. meas_planes[i] is the measurement plane for qubit i.
+    mode: str(optional)
+        This is the option for gflow.
+        The gflow finding algorithm can yield multiple equivalent solutions. so there are three options
+            - "single": Returrns a single solution
+            - "all": Returns all possible solutions
+            - "abstract": Returns an abstract solution. Uncertainty is represented with sympy.Symbol objects,
+            requiring user substitution to get a concrete answer.
     """
-    f, l_k = gflow(g, v_in, v_out, meas_plane, timeout)
-    if f:
-        print("gflow found")
-        print("g is ", f)
-        print("l_k is ", l_k)
-    else:
-        print("no gflow found, finding flow")
-    f, l_k = flow(g, v_in, v_out, timeout=timeout)
+    if meas_planes is None:
+        meas_planes = {i: "XY" for i in (set(graph.nodes) - output)}
+    f, l_k = flow(graph, input, output, meas_planes)
     if f:
         print("flow found")
         print("f is ", f)
         print("l_k is ", l_k)
     else:
-        print("no flow found")
+        print("no flow found, finding gflow")
+    g, l_k = gflow(graph, input, output, meas_planes, mode=mode)
+    if g:
+        print("gflow found")
+        print("g is ", g)
+        print("l_k is ", l_k)
+    else:
+        print("no gflow found")
 
 
 def get_min_depth(l_k):
     """get minimum depth of graph.
 
     Parameters
     ----------
@@ -457,7 +436,25 @@
         components of each layer
     """
     d = get_min_depth(l_k)
     layers = {k: [] for k in range(d + 1)}
     for i in l_k.keys():
         layers[l_k[i]].append(i)
     return d, layers
+
+
+def get_adjacency_matrix(graph):
+    """Get adjacency matrix of the graph
+
+    Returns
+    -------
+    adjacency_matrix: graphix.linalg.MatGF2
+        adjacency matrix of the graph. the matrix is defined on GF(2) field.
+    node_list: list
+        ordered list of nodes. node_list[i] is the node label of i-th row/column of the adjacency matrix.
+
+    """
+    node_list = list(graph.nodes)
+    node_list.sort()
+    adjacency_matrix = nx.to_numpy_array(graph, nodelist=node_list)
+    adjacency_matrix = MatGF2(adjacency_matrix.astype(int))
+    return adjacency_matrix, node_list
```

### Comparing `graphix-0.2.8/graphix/graphsim.py` & `graphix-0.2.9/graphix/graphsim.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/graphix/ops.py` & `graphix-0.2.9/graphix/ops.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/graphix/pattern.py` & `graphix-0.2.9/graphix/pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -778,15 +778,16 @@
         """
         nodes, edges = self.get_graph()
         G = nx.Graph()
         G.add_nodes_from(nodes)
         G.add_edges_from(edges)
         vin = set(self.input_nodes) if self.input_nodes is not None else set()
         vout = set(self.output_nodes)
-        f, l_k = flow(G, vin, vout)
+        meas_planes = self.get_meas_plane()
+        f, l_k = flow(G, vin, vout, meas_planes=meas_planes)
         if f is None:
             return None
         depth, layer = get_layers(l_k)
         meas_order = []
         for i in range(depth):
             k = depth - i
             nodes = layer[k]
@@ -1246,15 +1247,16 @@
 
         nodes, edges = self.get_graph()
         g = nx.Graph()
         g.add_nodes_from(nodes)
         g.add_edges_from(edges)
         vin = self.input_nodes if self.input_nodes is not None else []
         vout = self.output_nodes
-        vis = GraphVisualizer(g, vin, vout)
+        meas_planes = self.get_meas_plane()
+        vis = GraphVisualizer(g, vin, vout, meas_planes)
         if pauli_indicator:
             angles = self.get_angles()
         else:
             angles = None
         if local_clifford_indicator:
             local_clifford = self.get_vops()
         else:
```

### Comparing `graphix-0.2.8/graphix/sim/statevec.py` & `graphix-0.2.9/graphix/sim/statevec.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class StatevectorBackend:
     """MBQC simulator with statevector method."""
 
     def __init__(self, pattern, max_qubit_num=20):
         """
-        Parameteres
+        Parameters
         -----------
         pattern : :class:`graphix.pattern.Pattern` object
             MBQC pattern to be simulated.
         backend : str, 'statevector'
             optional argument for simulation.
         max_qubit_num : int
             optional argument specifying the maximum number of qubits
@@ -254,16 +254,16 @@
     def ptrace(self, qargs):
         """Perform partial trace of the selected qubits.
 
         .. warning::
             This method currently assumes qubits in qargs to be separable from the rest
             (checks not implemented for speed).
             Otherwise, the state returned will be forced to be pure which will result in incorrect output.
-            Correct behaviour will be implemented as soon as the densitymatrix class, currently under development (PR #64),
-            is merged.
+            Correct behaviour will be implemented as soon as the densitymatrix class, currently under development
+            (PR #64), is merged.
 
         Parameters
         ----------
         qargs : list of int
             qubit indices to trace over
         """
         nqubit_after = len(self.psi.shape) - len(qargs)
@@ -272,39 +272,44 @@
         rho = np.reshape(rho, (2**nqubit_after, 2**nqubit_after))
         evals, evecs = np.linalg.eig(rho)  # back to statevector
         self.psi = np.reshape(evecs[:, np.argmax(evals)], (2,) * nqubit_after)
 
     def remove_qubit(self, qarg):
         r"""Remove a separable qubit from the system and assemble a statevector for remaining qubits.
         This results in the same result as partial trace, if the qubit `qarg` is separable from the rest.
-        
-        For a statevector :math:`\ket{\psi} = \sum c_i \ket{i}` with sum taken over :math:`i \in [ 0 \dots 00,\ 0\dots 01,\ \dots,\
+
+        For a statevector :math:`\ket{\psi} = \sum c_i \ket{i}` with sum taken over
+        :math:`i \in [ 0 \dots 00,\ 0\dots 01,\ \dots,\
         1 \dots 11 ]`, this method returns
 
         .. math::
             \begin{align}
                 \ket{\psi}' =&
-                    c_{0 \dots 0_{\mathrm{k-1}}0_{\mathrm{k}}0_{\mathrm{k+1}} \dots 00} \ket{0 \dots 0_{\mathrm{k-1}}0_{\mathrm{k+1}} \dots 00} \\
-                    & + c_{0 \dots 0_{\mathrm{k-1}}0_{\mathrm{k}}0_{\mathrm{k+1}} \dots 01} \ket{0 \dots 0_{\mathrm{k-1}}0_{\mathrm{k+1}} \dots 01} \\
-                    & + c_{0 \dots 0_{\mathrm{k-1}}0_{\mathrm{k}}0_{\mathrm{k+1}} \dots 10} \ket{0 \dots 0_{\mathrm{k-1}}0_{\mathrm{k+1}} \dots 10} \\
+                    c_{0 \dots 0_{\mathrm{k-1}}0_{\mathrm{k}}0_{\mathrm{k+1}} \dots 00}
+                    \ket{0 \dots 0_{\mathrm{k-1}}0_{\mathrm{k+1}} \dots 00} \\
+                    & + c_{0 \dots 0_{\mathrm{k-1}}0_{\mathrm{k}}0_{\mathrm{k+1}} \dots 01}
+                    \ket{0 \dots 0_{\mathrm{k-1}}0_{\mathrm{k+1}} \dots 01} \\
+                    & + c_{0 \dots 0_{\mathrm{k-1}}0_{\mathrm{k}}0_{\mathrm{k+1}} \dots 10}
+                    \ket{0 \dots 0_{\mathrm{k-1}}0_{\mathrm{k+1}} \dots 10} \\
                     & + \dots \\
-                    & + c_{1 \dots 1_{\mathrm{k-1}}0_{\mathrm{k}}1_{\mathrm{k+1}} \dots 11} \ket{1 \dots 1_{\mathrm{k-1}}1_{\mathrm{k+1}} \dots 11},
+                    & + c_{1 \dots 1_{\mathrm{k-1}}0_{\mathrm{k}}1_{\mathrm{k+1}} \dots 11}
+                    \ket{1 \dots 1_{\mathrm{k-1}}1_{\mathrm{k+1}} \dots 11},
            \end{align}
 
         (after normalization) for :math:`k =` qarg. If the :math:`k` th qubit is in :math:`\ket{1}` state,
-        above will return zero amplitudes; in such a case the returned state will be the one above with :math:`0_{\mathrm{k}}`
-        replaced with :math:`1_{\mathrm{k}}` .
+        above will return zero amplitudes; in such a case the returned state will be the one above with
+        :math:`0_{\mathrm{k}}` replaced with :math:`1_{\mathrm{k}}` .
 
         .. warning::
             This method assumes the qubit with index `qarg` to be separable from the rest,
             and is implemented as a significantly faster alternative for partial trace to
             be used after single-qubit measurements.
             Care needs to be taken when using this method.
             Checks for separability will be implemented soon as an option.
-        
+
         .. seealso::
             :meth:`graphix.sim.statevec.Statevec.ptrace` and warning therein.
 
         Parameters
         ----------
         qarg : int
             qubit index
```

### Comparing `graphix-0.2.8/graphix/sim/tensornet.py` & `graphix-0.2.9/graphix/sim/tensornet.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/graphix/simulator.py` & `graphix-0.2.9/graphix/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """MBQC simulator
 
     Executes the measurement pattern.
     """
 
     def __init__(self, pattern, backend="statevector", **kwargs):
         """
-        Parameteres
+        Parameters
         -----------
         pattern: :class:`graphix.pattern.Pattern` object
             MBQC pattern to be simulated.
         backend: str, 'statevector' or 'tensornetwork'
             simulation backend (optional), default is 'statevector'.
         kwargs: keyword args for specified backend.
```

### Comparing `graphix-0.2.8/graphix/transpiler.py` & `graphix-0.2.9/graphix/transpiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,111 +32,111 @@
         """
         self.width = width
         self.instruction = []
 
     def cnot(self, control, target):
         """CNOT gate
 
-        Prameters
+        Parameters
         ---------
         control : int
             control qubit
         target : int
             target qubit
         """
         assert control in np.arange(self.width)
         assert target in np.arange(self.width)
         assert control != target
         self.instruction.append(["CNOT", [control, target]])
 
     def h(self, qubit):
         """Hadamard gate
 
-        Prameters
+        Parameters
         ---------
         qubit : int
             target qubit
         """
         assert qubit in np.arange(self.width)
         self.instruction.append(["H", qubit])
 
     def s(self, qubit):
         """S gate
 
-        Prameters
+        Parameters
         ---------
         qubit : int
             target qubit
         """
         assert qubit in np.arange(self.width)
         self.instruction.append(["S", qubit])
 
     def x(self, qubit):
         """Pauli X gate
 
-        Prameters
+        Parameters
         ---------
         qubit : int
             target qubit
         """
         assert qubit in np.arange(self.width)
         self.instruction.append(["X", qubit])
 
     def y(self, qubit):
         """Pauli Y gate
 
-        Prameters
+        Parameters
         ---------
         qubit : int
             target qubit
         """
         assert qubit in np.arange(self.width)
         self.instruction.append(["Y", qubit])
 
     def z(self, qubit):
         """Pauli Z gate
 
-        Prameters
+        Parameters
         ---------
         qubit : int
             target qubit
         """
         assert qubit in np.arange(self.width)
         self.instruction.append(["Z", qubit])
 
     def rx(self, qubit, angle):
         """X rotation gate
 
-        Prameters
+        Parameters
         ---------
         qubit : int
             target qubit
         angle : float
             rotation angle in radian
         """
         assert qubit in np.arange(self.width)
         self.instruction.append(["Rx", qubit, angle])
 
     def ry(self, qubit, angle):
         """Y rotation gate
 
-        Prameters
+        Parameters
         ---------
         qubit : int
             target qubit
         angle : float
             angle in radian
         """
         assert qubit in np.arange(self.width)
         self.instruction.append(["Ry", qubit, angle])
 
     def rz(self, qubit, angle):
         """Z rotation gate
 
-        Prameters
+        Parameters
         ---------
         qubit : int
             target qubit
         angle : float
             rotation angle in radian
         """
         assert qubit in np.arange(self.width)
@@ -148,29 +148,29 @@
         CNOT(control, target),
         Rz(target, angle),
         CNOT(control, target)
 
         and realizes rotation expressed by
         :math:`e^{-i \frac{\theta}{2} Z_c Z_t}`.
 
-        Prameters
+        Parameters
         ---------
         qubit : int
             target qubit
         angle : float
             rotation angle in radian
         """
         assert control in np.arange(self.width)
         assert target in np.arange(self.width)
         self.instruction.append(["Rzz", [control, target], angle])
 
     def i(self, qubit):
         """identity (teleportation) gate
 
-        Prameters
+        Parameters
         ---------
         qubit : int
             target qubit
         """
         assert qubit in np.arange(self.width)
         self.instruction.append(["I", qubit])
```

### Comparing `graphix-0.2.8/graphix/visualization.py` & `graphix-0.2.9/graphix/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,31 @@
         the graph to be visualized
     v_in : list
         list of input nodes
     v_out : list
         list of output nodes
     """
 
-    def __init__(self, G, v_in, v_out):
+    def __init__(self, G, v_in, v_out, meas_plane=None):
         """
+        Parameters
+        ----------
         G: networkx graph
         v_in: list of input nodes
         v_out: list of output nodes
+        meas_plane: dict specifying the measurement planes for each node, except output nodes.
+            if None, all measurements are assumed to be in XY-plane.
         """
         self.G = G
         self.v_in = v_in
         self.v_out = v_out
+        if meas_plane is None:
+            self.meas_plane = {i: "XY" for i in iter(G.nodes)}
+        else:
+            self.meas_plane = meas_plane
 
     def visualize(self, angles=None, local_clifford=None, figsize=None, save=False, filename=None):
         """
         Visualizes the graph with flow or gflow structure.
         If there exists a flow structure, then the graph is visualized with the flow structure.
         If flow structure is not found and there exists a gflow structure, then the graph is visualized
         with the gflow structure.
@@ -49,20 +57,20 @@
             Figure size of the plot.
         save : bool
             If True, the plot is saved as a png file.
         filename : str
             Filename of the saved plot.
         """
 
-        f, l_k = gflow.flow(self.G, set(self.v_in), set(self.v_out))
+        f, l_k = gflow.flow(self.G, set(self.v_in), set(self.v_out), meas_planes=self.meas_plane)
         if f:
             print("Flow found.")
             self.visualize_w_flow(f, l_k, angles, local_clifford, figsize, save, filename)
         else:
-            g, l_k = gflow.gflow(self.G, set(self.v_in), set(self.v_out))
+            g, l_k = gflow.gflow(self.G, set(self.v_in), set(self.v_out), self.meas_plane)
             if g:
                 print("No flow found. Gflow found.")
                 self.visualize_w_gflow(g, l_k, angles, local_clifford, figsize, save, filename)
             else:
                 print("No flow or gflow found.")
                 self.visualize_wo_structure(angles, local_clifford, save, filename)
```

### Comparing `graphix-0.2.8/graphix.egg-info/PKG-INFO` & `graphix-0.2.9/graphix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphix
-Version: 0.2.8
+Version: 0.2.9
 Summary: Optimize and simulate measurement-based quantum computation
 Home-page: https://graphix.readthedocs.io
 Author: Shinichi Sunami
 Author-email: shinichi.sunami@gmail.com
 Maintainer: Shinichi Sunami
 Maintainer-email: shinichi.sunami@gmail.com
 License: Apache License 2.0
@@ -20,21 +20,23 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy<1.26,>=1.22
 Requires-Dist: networkx>3.0
-Requires-Dist: z3-solver
 Requires-Dist: quimb>=1.4.0
 Requires-Dist: autoray>=0.6.0
 Requires-Dist: opt_einsum>=3.2
+Requires-Dist: galois>=0.3.0
+Requires-Dist: sympy>=1.9
 Requires-Dist: matplotlib
 Provides-Extra: extra
 Requires-Dist: graphix-ibmq; extra == "extra"
+Requires-Dist: graphix-perceval; extra == "extra"
 Provides-Extra: test
 Requires-Dist: qiskit; extra == "test"
 Requires-Dist: qiskit-aer; extra == "test"
 
 <img src="https://github.com/TeamGraphix/graphix/raw/master/docs/logo/black_with_name.png" alt="logo" width="550">
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/graphix)
@@ -60,18 +62,18 @@
 $ pip install graphix
 ```
 
 Install together with device interface:
 ```bash
 $ pip install graphix[extra]
 ```
-this will install `graphix` and [IBMQ interface](https://github.com/TeamGraphix/graphix-ibmq) to run MBQC patterns on IBM devices and Aer simulator.
+this will install `graphix` and inteface for [IBMQ](https://github.com/TeamGraphix/graphix-ibmq) and [Perceval](https://github.com/TeamGraphix/graphix-perceval) to run MBQC patterns on superconducting and optical QPUs and their simulators.
 
-We are currently adding more quantum device interfaces.
-Please suggest in [issues](https://github.com/TeamGraphix/graphix/issues) if you have any particular device in mind!
+<!-- We are currently adding more quantum device interface.
+Please suggest in [issues](https://github.com/TeamGraphix/graphix/issues) if you have any particular device in mind! -->
 
 
 ## Next Steps
 
 - We have a few [demos](https://graphix.readthedocs.io/en/latest/gallery/index.html) showing basic usages of `Graphix`.
 - You can run demos on your browser:
   - Preprocessing Clifford gates: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TeamGraphix/graphix-examples/HEAD?labpath=deutsch-jozsa.ipynb)
```

### Comparing `graphix-0.2.8/graphix.egg-info/SOURCES.txt` & `graphix-0.2.9/graphix.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 graphix/__init__.py
 graphix/clifford.py
 graphix/device_interface.py
 graphix/extraction.py
 graphix/generator.py
 graphix/gflow.py
 graphix/graphsim.py
+graphix/linalg.py
 graphix/ops.py
 graphix/pattern.py
 graphix/simulator.py
 graphix/transpiler.py
 graphix/version.py
 graphix/visualization.py
 graphix.egg-info/PKG-INFO
@@ -28,12 +29,13 @@
 tests/__init__.py
 tests/random_circuit.py
 tests/test_clifford.py
 tests/test_extraction.py
 tests/test_generator.py
 tests/test_gflow.py
 tests/test_graphsim.py
+tests/test_linalg.py
 tests/test_pattern.py
 tests/test_runner.py
 tests/test_statevec_backend.py
 tests/test_tnsim.py
 tests/test_transpiler.py
```

### Comparing `graphix-0.2.8/setup.py` & `graphix-0.2.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,11 +33,11 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Physics",
     ],
     "python_requires": ">=3.8,<3.12",
     "install_requires": requirements,
-    "extras_require": {"extra": ["graphix-ibmq"], "test": ["qiskit", "qiskit-aer"]},
+    "extras_require": {"extra": ["graphix-ibmq", "graphix-perceval"], "test": ["qiskit", "qiskit-aer"]},
 }
 
 setup(**(info))
```

### Comparing `graphix-0.2.8/tests/random_circuit.py` & `graphix-0.2.9/tests/random_circuit.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/tests/test_clifford.py` & `graphix-0.2.9/tests/test_clifford.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/tests/test_extraction.py` & `graphix-0.2.9/tests/test_extraction.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/tests/test_generator.py` & `graphix-0.2.9/tests/test_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,34 +9,36 @@
     def test_pattern_generation_determinism_flow(self):
         graph = nx.Graph([(0, 3), (1, 4), (2, 5), (1, 3), (2, 4), (3, 6), (4, 7), (5, 8)])
         inputs = {0, 1, 2}
         outputs = {6, 7, 8}
         angles = np.random.randn(6)
         results = []
         repeats = 3  # for testing the determinism of a pattern
+        meas_planes = {i: "XY" for i in range(6)}
         for _ in range(repeats):
-            pattern = generate_from_graph(graph, angles, list(inputs), list(outputs))
+            pattern = generate_from_graph(graph, angles, list(inputs), list(outputs), meas_planes=meas_planes)
             pattern.standardize()
             pattern.minimize_space()
             state = pattern.simulate_pattern()
             results.append(state)
         combinations = [(0, 1), (0, 2), (1, 2)]
         for i, j in combinations:
             inner_product = np.dot(results[i].flatten(), results[j].flatten().conjugate())
             np.testing.assert_almost_equal(abs(inner_product), 1)
 
     def test_pattern_generation_determinism_gflow(self):
         graph = nx.Graph([(1, 2), (2, 3), (3, 4), (4, 5), (5, 6), (3, 6), (1, 6)])
         inputs = {1, 3, 5}
         outputs = {2, 4, 6}
         angles = np.random.randn(6)
+        meas_planes = {i: "XY" for i in range(1, 6)}
         results = []
         repeats = 3  # for testing the determinism of a pattern
         for _ in range(repeats):
-            pattern = generate_from_graph(graph, angles, list(inputs), list(outputs))
+            pattern = generate_from_graph(graph, angles, list(inputs), list(outputs), meas_planes=meas_planes)
             pattern.standardize()
             pattern.minimize_space()
             state = pattern.simulate_pattern()
             results.append(state)
         combinations = [(0, 1), (0, 2), (1, 2)]
         for i, j in combinations:
             inner_product = np.dot(results[i].flatten(), results[j].flatten().conjugate())
@@ -56,15 +58,16 @@
         g = nx.Graph()
         g.add_nodes_from(nodes)
         g.add_edges_from(edges)
         input = [0, 1, 2]
         angles = dict()
         for cmd in pattern.get_measurement_commands():
             angles[cmd[1]] = cmd[3]
-        pattern2 = generate_from_graph(g, angles, input, pattern.output_nodes)
+        meas_planes = pattern.get_meas_plane()
+        pattern2 = generate_from_graph(g, angles, input, pattern.output_nodes, meas_planes)
         # check that the new one runs and returns correct result
         pattern2.standardize()
         pattern2.shift_signals()
         pattern2.minimize_space()
         state = circuit.simulate_statevector()
         state_mbqc = pattern2.simulate_pattern()
         np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
```

### Comparing `graphix-0.2.8/tests/test_graphsim.py` & `graphix-0.2.9/tests/test_graphsim.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/tests/test_pattern.py` & `graphix-0.2.9/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/tests/test_runner.py` & `graphix-0.2.9/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/tests/test_statevec_backend.py` & `graphix-0.2.9/tests/test_statevec_backend.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/tests/test_tnsim.py` & `graphix-0.2.9/tests/test_tnsim.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.8/tests/test_transpiler.py` & `graphix-0.2.9/tests/test_transpiler.py`

 * *Files identical despite different names*

