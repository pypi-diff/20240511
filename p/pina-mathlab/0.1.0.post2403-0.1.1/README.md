# Comparing `tmp/pina-mathlab-0.1.0.post2403.tar.gz` & `tmp/pina-mathlab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PINA/PINA/dist/.tmp-ziwo8_cb/pina-mathlab-0.1.0.post2403.tar", last modified: Fri Mar  1 02:42:04 2024, max compression
+gzip compressed data, was "/home/runner/work/PINA/PINA/dist/.tmp-kby7lo90/pina-mathlab-0.1.1.tar", last modified: Sat May 11 08:02:16 2024, max compression
```

## Comparing `pina-mathlab-0.1.0.post2403.tar` & `pina-mathlab-0.1.1.tar`

### file list

```diff
@@ -1,98 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina/adaptive_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/adaptive_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/adaptive_functions/adaptive_cos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/adaptive_functions/adaptive_exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/adaptive_functions/adaptive_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/adaptive_functions/adaptive_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/adaptive_functions/adaptive_sin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/adaptive_functions/adaptive_softplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/adaptive_functions/adaptive_square.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/adaptive_functions/adaptive_tanh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/callbacks/adaptive_refinment_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/callbacks/optimizer_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/callbacks/processing_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina/equation/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/equation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/equation/equation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/equation/equation_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/equation/equation_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/equation/system_equation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/geometry/cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/geometry/difference_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/geometry/ellipsoid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/geometry/exclusion_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/geometry/intersection_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/geometry/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/geometry/operation_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/geometry/simplex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/geometry/union_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     9673 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/label_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina/model/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/base_no.py
--rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/deeponet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9299 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/feed_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/fno.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina/model/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/layers/convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    21470 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/layers/convolution_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/layers/fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/layers/integral.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/layers/pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/layers/residual.py
--rw-r--r--   0 runner    (1001) docker     (127)    13966 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/layers/spectral.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/layers/stride.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/layers/utils_convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/multi_feed_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/model/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina/problem/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9845 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/problem/abstract_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/problem/inverse_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/problem/parametric_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/problem/spatial_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/problem/timedep_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/solvers/garom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/solvers/pinn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/solvers/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/solvers/supervised.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/pina/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina_mathlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina_mathlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina_mathlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina_mathlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina_mathlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina_mathlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/pina_mathlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 02:42:04.000000 pina-mathlab-0.1.0.post2403/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/tests/test_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/tests/test_label_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/tests/test_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/tests/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-01 02:41:58.000000 pina-mathlab-0.1.0.post2403/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina/adaptive_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/adaptive_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19631 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/adaptive_functions/adaptive_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/adaptive_functions/adaptive_func_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/callbacks/adaptive_refinment_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/callbacks/optimizer_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/callbacks/processing_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina/equation/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/equation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/equation/equation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/equation/equation_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/equation/equation_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/equation/system_equation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/geometry/cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/geometry/difference_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/geometry/ellipsoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/geometry/exclusion_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/geometry/intersection_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/geometry/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/geometry/operation_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/geometry/simplex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/geometry/union_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/label_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/avno.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/base_no.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/deeponet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9299 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/feed_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/fno.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina/model/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/layers/avno_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/layers/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21470 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/layers/convolution_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6409 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/layers/fourier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/layers/integral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/layers/lowrank_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/layers/pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/layers/residual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13966 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/layers/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/layers/stride.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/layers/utils_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/lno.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/multi_feed_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/model/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina/problem/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/problem/abstract_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/problem/inverse_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/problem/parametric_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/problem/spatial_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/problem/timedep_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/solvers/garom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina/solvers/pinns/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/solvers/pinns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9439 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/solvers/pinns/basepinn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/solvers/pinns/causalpinn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/solvers/pinns/competitive_pinn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/solvers/pinns/gpinn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/solvers/pinns/pinn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/solvers/pinns/sapinn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/solvers/rom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/solvers/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/solvers/supervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/pina/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina_mathlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina_mathlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina_mathlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina_mathlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina_mathlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina_mathlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/pina_mathlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 08:02:16.000000 pina-mathlab-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/tests/test_adaptive_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/tests/test_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/tests/test_label_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/tests/test_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/tests/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-11 08:02:09.000000 pina-mathlab-0.1.1/tests/test_utils.py
```

### Comparing `pina-mathlab-0.1.0.post2403/LICENSE.rst` & `pina-mathlab-0.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/PKG-INFO` & `pina-mathlab-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pina-mathlab
-Version: 0.1.0.post2403
+Version: 0.1.1
 Summary: Physic Informed Neural networks for Advance modeling.
 Home-page: https://github.com/mathLab/PINA
 Author: PINA Contributors
 Author-email: demo.nicola@gmail.com, dario.coscia@sissa.it
 License: MIT
 Keywords: physics-informed neural-network
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pina-mathlab-0.1.0.post2403/README.md` & `pina-mathlab-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/callbacks/adaptive_refinment_callbacks.py` & `pina-mathlab-0.1.1/pina/callbacks/adaptive_refinment_callbacks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 """PINA Callbacks Implementations"""
 
-# from lightning.pytorch.callbacks import Callback
-from pytorch_lightning.callbacks import Callback
 import torch
+from pytorch_lightning.callbacks import Callback
+from ..label_tensor import LabelTensor
 from ..utils import check_consistency
 
 
 class R3Refinement(Callback):
 
     def __init__(self, sample_every):
         """
         PINA Implementation of an R3 Refinement Callback.
 
-        This callback implements the R3 (Retain-Resample-Release) routine for sampling new points based on adaptive search.
-        The algorithm incrementally accumulates collocation points in regions of high PDE residuals, and releases those
-        with low residuals. Points are sampled uniformly in all regions where sampling is needed.
+        This callback implements the R3 (Retain-Resample-Release) routine for
+        sampling new points based on adaptive search.
+        The algorithm incrementally accumulates collocation points in regions
+        of high PDE residuals, and releases those
+        with low residuals. Points are sampled uniformly in all regions
+        where sampling is needed.
 
         .. seealso::
 
-            Original Reference: Daw, Arka, et al. *Mitigating Propagation Failures in Physics-informed Neural Networks
+            Original Reference: Daw, Arka, et al. *Mitigating Propagation
+            Failures in Physics-informed Neural Networks
             using Retain-Resample-Release (R3) Sampling. (2023)*.
             DOI: `10.48550/arXiv.2207.02338
             <https://doi.org/10.48550/arXiv.2207.02338>`_
 
         :param int sample_every: Frequency for sampling.
-
         :raises ValueError: If `sample_every` is not an integer.
 
         Example:
             >>> r3_callback = R3Refinement(sample_every=5)
         """
         super().__init__()
 
@@ -43,26 +46,38 @@
         :return: the total loss, and pointwise loss.
         :rtype: tuple
         """
 
         # extract the solver and device from trainer
         solver = trainer._model
         device = trainer._accelerator_connector._accelerator_flag
+        precision = trainer.precision
+        if precision == "64-true":
+            precision = torch.float64
+        elif precision == "32-true":
+            precision = torch.float32
+        else:
+            raise RuntimeError(
+                "Currently R3Refinement is only implemented "
+                "for precision '32-true' and '64-true', set "
+                "Trainer precision to match one of the "
+                "available precisions."
+            )
 
         # compute residual
         res_loss = {}
         tot_loss = []
         for location in self._sampling_locations:
             condition = solver.problem.conditions[location]
             pts = solver.problem.input_pts[location]
             # send points to correct device
-            pts = pts.to(device)
+            pts = pts.to(device=device, dtype=precision)
             pts = pts.requires_grad_(True)
             pts.retain_grad()
-            # PINN loss: equation evaluated only on locations where sampling is needed
+            # PINN loss: equation evaluated only for sampling locations
             target = condition.equation.residual(pts, solver.forward(pts))
             res_loss[location] = torch.abs(target).as_subclass(torch.Tensor)
             tot_loss.append(torch.abs(target))
 
         return torch.vstack(tot_loss), res_loss
 
     def _r3_routine(self, trainer):
@@ -82,21 +97,22 @@
 
         # points to keep
         old_pts = {}
         tot_points = 0
         for location in self._sampling_locations:
             pts = trainer._model.problem.input_pts[location]
             labels = pts.labels
-            pts = pts.cpu().detach()
+            pts = pts.cpu().detach().as_subclass(torch.Tensor)
             residuals = res_loss[location].cpu()
             mask = (residuals > avg).flatten()
             if any(
                 mask
             ):  # if there are residuals greater than averge we append them
-                pts = pts[mask]  # TODO masking remove labels
+                # Fix the issue, masking remove labels
+                pts = (pts[mask]).as_subclass(LabelTensor)
                 pts.labels = labels
                 old_pts[location] = pts
                 tot_points += len(pts)
 
         # extract new points to sample uniformally for each location
         n_points = (self._tot_pop_numb - tot_points) // len(
             self._sampling_locations
@@ -118,15 +134,16 @@
         # update dataloader
         trainer._create_or_update_loader()
 
     def on_train_start(self, trainer, _):
         """
         Callback function called at the start of training.
 
-        This method extracts the locations for sampling from the problem conditions and calculates the total population.
+        This method extracts the locations for sampling from the problem
+        conditions and calculates the total population.
 
         :param trainer: The trainer object managing the training process.
         :type trainer: pytorch_lightning.Trainer
         :param _: Placeholder argument (not used).
 
         :return: None
         :rtype: None
@@ -147,15 +164,16 @@
             total_population += len(pts)
         self._tot_pop_numb = total_population
 
     def on_train_epoch_end(self, trainer, __):
         """
         Callback function called at the end of each training epoch.
 
-        This method triggers the R3 routine for refinement if the current epoch is a multiple of `_sample_every`.
+        This method triggers the R3 routine for refinement if the current
+        epoch is a multiple of `_sample_every`.
 
         :param trainer: The trainer object managing the training process.
         :type trainer: pytorch_lightning.Trainer
         :param __: Placeholder argument (not used).
 
         :return: None
         :rtype: None
```

### Comparing `pina-mathlab-0.1.0.post2403/pina/callbacks/optimizer_callbacks.py` & `pina-mathlab-0.1.1/pina/callbacks/optimizer_callbacks.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/callbacks/processing_callbacks.py` & `pina-mathlab-0.1.1/pina/callbacks/processing_callbacks.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/condition.py` & `pina-mathlab-0.1.1/pina/condition.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/dataset.py` & `pina-mathlab-0.1.1/pina/dataset.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/equation/equation.py` & `pina-mathlab-0.1.1/pina/equation/equation.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/equation/equation_factory.py` & `pina-mathlab-0.1.1/pina/equation/equation_factory.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/equation/equation_interface.py` & `pina-mathlab-0.1.1/pina/equation/equation_interface.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/equation/system_equation.py` & `pina-mathlab-0.1.1/pina/equation/system_equation.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/geometry/__init__.py` & `pina-mathlab-0.1.1/pina/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/geometry/cartesian.py` & `pina-mathlab-0.1.1/pina/geometry/cartesian.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/geometry/difference_domain.py` & `pina-mathlab-0.1.1/pina/geometry/difference_domain.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/geometry/ellipsoid.py` & `pina-mathlab-0.1.1/pina/geometry/ellipsoid.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/geometry/exclusion_domain.py` & `pina-mathlab-0.1.1/pina/geometry/exclusion_domain.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/geometry/intersection_domain.py` & `pina-mathlab-0.1.1/pina/geometry/intersection_domain.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/geometry/location.py` & `pina-mathlab-0.1.1/pina/geometry/location.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/geometry/operation_interface.py` & `pina-mathlab-0.1.1/pina/geometry/operation_interface.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/geometry/simplex.py` & `pina-mathlab-0.1.1/pina/geometry/simplex.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/geometry/union_domain.py` & `pina-mathlab-0.1.1/pina/geometry/union_domain.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/label_tensor.py` & `pina-mathlab-0.1.1/pina/label_tensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Module for LabelTensor """
 
-from typing import Any
+from copy import deepcopy
 import torch
 from torch import Tensor
 
 
 class LabelTensor(torch.Tensor):
     """Torch tensor with a label for any column."""
 
@@ -75,14 +75,29 @@
         if len(labels) != x.shape[-1]:
             raise ValueError(
                 "the tensor has not the same number of columns of "
                 "the passed labels."
             )
         self._labels = labels
 
+    def __deepcopy__(self, __):
+        """
+        Implements deepcopy for label tensor. By default it stores the
+        current labels and use the :meth:`~torch._tensor.Tensor.__deepcopy__`
+        method for creating a new :class:`pina.label_tensor.LabelTensor`.
+
+        :param __: Placeholder parameter.
+        :type __: None
+        :return: The deep copy of the :class:`pina.label_tensor.LabelTensor`.
+        :rtype: LabelTensor
+        """
+        labels = self.labels
+        copy_tensor = deepcopy(self.tensor)
+        return LabelTensor(copy_tensor, labels)
+
     @property
     def labels(self):
         """Property decorator for labels
 
         :return: labels of self
         :rtype: list
         """
@@ -157,24 +172,24 @@
     def cuda(self, *args, **kwargs):
         """
         Send Tensor to cuda. For more details, see :meth:`torch.Tensor.cuda`.
         """
         tmp = super().cuda(*args, **kwargs)
         new = self.__class__.clone(self)
         new.data = tmp.data
-        return tmp
+        return new
 
     def cpu(self, *args, **kwargs):
         """
         Send Tensor to cpu. For more details, see :meth:`torch.Tensor.cpu`.
         """
         tmp = super().cpu(*args, **kwargs)
         new = self.__class__.clone(self)
         new.data = tmp.data
-        return tmp
+        return new
 
     def extract(self, label_to_extract):
         """
         Extract the subset of the original tensor by returning all the columns
         corresponding to the passed ``label_to_extract``.
 
         :param label_to_extract: The label(s) to extract.
```

### Comparing `pina-mathlab-0.1.0.post2403/pina/loss.py` & `pina-mathlab-0.1.1/pina/loss.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/base_no.py` & `pina-mathlab-0.1.1/pina/model/base_no.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/deeponet.py` & `pina-mathlab-0.1.1/pina/model/deeponet.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/feed_forward.py` & `pina-mathlab-0.1.1/pina/model/feed_forward.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/fno.py` & `pina-mathlab-0.1.1/pina/model/fno.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/layers/convolution.py` & `pina-mathlab-0.1.1/pina/model/layers/convolution.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/layers/convolution_2d.py` & `pina-mathlab-0.1.1/pina/model/layers/convolution_2d.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/layers/fourier.py` & `pina-mathlab-0.1.1/pina/model/layers/fourier.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/layers/integral.py` & `pina-mathlab-0.1.1/pina/model/layers/integral.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/layers/pod.py` & `pina-mathlab-0.1.1/pina/model/layers/pod.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/layers/residual.py` & `pina-mathlab-0.1.1/pina/model/layers/residual.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/layers/spectral.py` & `pina-mathlab-0.1.1/pina/model/layers/spectral.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/layers/stride.py` & `pina-mathlab-0.1.1/pina/model/layers/stride.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/layers/utils_convolution.py` & `pina-mathlab-0.1.1/pina/model/layers/utils_convolution.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/multi_feed_forward.py` & `pina-mathlab-0.1.1/pina/model/multi_feed_forward.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/model/network.py` & `pina-mathlab-0.1.1/pina/model/network.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/operators.py` & `pina-mathlab-0.1.1/pina/operators.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/plotter.py` & `pina-mathlab-0.1.1/pina/plotter.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/problem/abstract_problem.py` & `pina-mathlab-0.1.1/pina/problem/abstract_problem.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Module for AbstractProblem class """
 
 from abc import ABCMeta, abstractmethod
 from ..utils import merge_tensors, check_consistency
+from copy import deepcopy
 import torch
 
 
 class AbstractProblem(metaclass=ABCMeta):
     """
     The abstract `AbstractProblem` class. All the class defining a PINA Problem
     should be inheritied from this class.
@@ -25,14 +26,31 @@
         self._have_sampled_points = {}
         for condition_name in self.conditions:
             self._have_sampled_points[condition_name] = False
 
         # put in self.input_pts all the points that we don't need to sample
         self._span_condition_points()
 
+    def __deepcopy__(self, memo):
+        """
+        Implements deepcopy for the
+        :class:`~pina.problem.abstract_problem.AbstractProblem` class.
+
+        :param dict memo: Memory dictionary, to avoid excess copy
+        :return: The deep copy of the
+            :class:`~pina.problem.abstract_problem.AbstractProblem` class
+        :rtype: AbstractProblem
+        """
+        cls = self.__class__
+        result = cls.__new__(cls)
+        memo[id(self)] = result
+        for k, v in self.__dict__.items():
+            setattr(result, k, deepcopy(v, memo))
+        return result
+
     @property
     def input_variables(self):
         """
         The input variables of the AbstractProblem, whose type depends on the
         type of domain (spatial, temporal, and parameter).
 
         :return: the input variables of self
```

### Comparing `pina-mathlab-0.1.0.post2403/pina/problem/inverse_problem.py` & `pina-mathlab-0.1.1/pina/problem/inverse_problem.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/problem/parametric_problem.py` & `pina-mathlab-0.1.1/pina/problem/parametric_problem.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/problem/spatial_problem.py` & `pina-mathlab-0.1.1/pina/problem/spatial_problem.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/problem/timedep_problem.py` & `pina-mathlab-0.1.1/pina/problem/timedep_problem.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/solvers/garom.py` & `pina-mathlab-0.1.1/pina/solvers/garom.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,26 +249,19 @@
         :type batch: tuple
         :param batch_idx: The batch index.
         :type batch_idx: int
         :return: The sum of the loss functions.
         :rtype: LabelTensor
         """
 
-        dataloader = self.trainer.train_dataloader
         condition_idx = batch["condition"]
 
         for condition_id in range(condition_idx.min(), condition_idx.max() + 1):
 
-            if sys.version_info >= (3, 8):
-                condition_name = dataloader.condition_names[condition_id]
-            else:
-                condition_name = dataloader.loaders.condition_names[
-                    condition_id
-                ]
-
+            condition_name = self._dataloader.condition_names[condition_id]
             condition = self.problem.conditions[condition_name]
             pts = batch["pts"].detach()
             out = batch["output"]
 
             if condition_name not in self.problem.conditions:
                 raise RuntimeError("Something wrong happened.")
```

### Comparing `pina-mathlab-0.1.0.post2403/pina/solvers/pinn.py` & `pina-mathlab-0.1.1/pina/solvers/supervised.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,78 @@
-""" Module for PINN """
+""" Module for SupervisedSolver """
 
 import torch
 
 try:
     from torch.optim.lr_scheduler import LRScheduler  # torch >= 2.0
 except ImportError:
     from torch.optim.lr_scheduler import (
         _LRScheduler as LRScheduler,
     )  # torch < 2.0
 
-import sys
 from torch.optim.lr_scheduler import ConstantLR
 
 from .solver import SolverInterface
 from ..label_tensor import LabelTensor
 from ..utils import check_consistency
 from ..loss import LossInterface
-from ..problem import InverseProblem
 from torch.nn.modules.loss import _Loss
 
-torch.pi = torch.acos(torch.zeros(1)).item() * 2  # which is 3.1415927410125732
 
-
-class PINN(SolverInterface):
-    """
-    PINN solver class. This class implements Physics Informed Neural
-    Network solvers, using a user specified ``model`` to solve a specific
-    ``problem``. It can be used for solving both forward and inverse problems.
-
-    .. seealso::
-
-        **Original reference**: Karniadakis, G. E., Kevrekidis, I. G., Lu, L.,
-        Perdikaris, P., Wang, S., & Yang, L. (2021).
-        Physics-informed machine learning. Nature Reviews Physics, 3(6), 422-440.
-        <https://doi.org/10.1038/s42254-021-00314-5>`_.
+class SupervisedSolver(SolverInterface):
+    r"""
+    SupervisedSolver solver class. This class implements a SupervisedSolver,
+    using a user specified ``model`` to solve a specific ``problem``.
+
+    The  Supervised Solver class aims to find
+    a map between the input :math:`\mathbf{s}:\Omega\rightarrow\mathbb{R}^m`
+    and the output :math:`\mathbf{u}:\Omega\rightarrow\mathbb{R}^m`. The input
+    can be discretised in space (as in :obj:`~pina.solvers.rom.ROMe2eSolver`),
+    or not (e.g. when training Neural Operators).
+
+    Given a model :math:`\mathcal{M}`, the following loss function is
+    minimized during training:
+
+    .. math::
+        \mathcal{L}_{\rm{problem}} = \frac{1}{N}\sum_{i=1}^N
+        \mathcal{L}(\mathbf{u}_i - \mathcal{M}(\mathbf{v}_i))
+
+    where :math:`\mathcal{L}` is a specific loss function,
+    default Mean Square Error:
+
+    .. math::
+        \mathcal{L}(v) = \| v \|^2_2.
+
+    In this context :math:`\mathbf{u}_i` and :math:`\mathbf{v}_i` means that
+    we are seeking to approximate multiple (discretised) functions given
+    multiple (discretised) input functions.
     """
 
     def __init__(
         self,
         problem,
         model,
         extra_features=None,
         loss=torch.nn.MSELoss(),
         optimizer=torch.optim.Adam,
         optimizer_kwargs={"lr": 0.001},
         scheduler=ConstantLR,
         scheduler_kwargs={"factor": 1, "total_iters": 0},
     ):
         """
-        :param AbstractProblem problem: The formulation of the problem.
+        :param AbstractProblem problem: The formualation of the problem.
         :param torch.nn.Module model: The neural network model to use.
         :param torch.nn.Module loss: The loss function used as minimizer,
             default :class:`torch.nn.MSELoss`.
         :param torch.nn.Module extra_features: The additional input
             features to use as augmented input.
         :param torch.optim.Optimizer optimizer: The neural network optimizer to
             use; default is :class:`torch.optim.Adam`.
         :param dict optimizer_kwargs: Optimizer constructor keyword args.
+        :param float lr: The learning rate; default is 0.001.
         :param torch.optim.LRScheduler scheduler: Learning
             rate scheduler.
         :param dict scheduler_kwargs: LR scheduler constructor keyword args.
         """
         super().__init__(
             models=[model],
             problem=problem,
@@ -75,158 +87,99 @@
         check_consistency(loss, (LossInterface, _Loss), subclass=False)
 
         # assign variables
         self._scheduler = scheduler(self.optimizers[0], **scheduler_kwargs)
         self._loss = loss
         self._neural_net = self.models[0]
 
-        # inverse problem handling
-        if isinstance(self.problem, InverseProblem):
-            self._params = self.problem.unknown_parameters
-        else:
-            self._params = None
-
     def forward(self, x):
-        """
-        Forward pass implementation for the PINN
-        solver.
+        """Forward pass implementation for the solver.
 
         :param torch.Tensor x: Input tensor.
-        :return: PINN solution.
+        :return: Solver solution.
         :rtype: torch.Tensor
         """
         return self.neural_net(x)
 
     def configure_optimizers(self):
-        """
-        Optimizer configuration for the PINN
-        solver.
+        """Optimizer configuration for the solver.
 
         :return: The optimizers and the schedulers
         :rtype: tuple(list, list)
         """
-        # if the problem is an InverseProblem, add the unknown parameters
-        # to the parameters that the optimizer needs to optimize
-        if isinstance(self.problem, InverseProblem):
-            self.optimizers[0].add_param_group(
-                {
-                    "params": [
-                        self._params[var]
-                        for var in self.problem.unknown_variables
-                    ]
-                }
-            )
         return self.optimizers, [self.scheduler]
 
-    def _clamp_inverse_problem_params(self):
-        for v in self._params:
-            self._params[v].data.clamp_(
-                self.problem.unknown_parameter_domain.range_[v][0],
-                self.problem.unknown_parameter_domain.range_[v][1],
-            )
-
-    def _loss_data(self, input, output):
-        return self.loss(self.forward(input), output)
-
-    def _loss_phys(self, samples, equation):
-        try:
-            residual = equation.residual(samples, self.forward(samples))
-        except (
-            TypeError
-        ):  # this occurs when the function has three inputs, i.e. inverse problem
-            residual = equation.residual(
-                samples, self.forward(samples), self._params
-            )
-        return self.loss(
-            torch.zeros_like(residual, requires_grad=True), residual
-        )
-
     def training_step(self, batch, batch_idx):
-        """
-        PINN solver training step.
+        """Solver training step.
 
         :param batch: The batch element in the dataloader.
         :type batch: tuple
         :param batch_idx: The batch index.
         :type batch_idx: int
         :return: The sum of the loss functions.
         :rtype: LabelTensor
         """
 
-        dataloader = self.trainer.train_dataloader
-        condition_losses = []
-
         condition_idx = batch["condition"]
 
         for condition_id in range(condition_idx.min(), condition_idx.max() + 1):
 
-            if sys.version_info >= (3, 8):
-                condition_name = dataloader.condition_names[condition_id]
-            else:
-                condition_name = dataloader.loaders.condition_names[
-                    condition_id
-                ]
+            condition_name = self._dataloader.condition_names[condition_id]
             condition = self.problem.conditions[condition_name]
             pts = batch["pts"]
+            out = batch["output"]
 
-            if len(batch) == 2:
-                samples = pts[condition_idx == condition_id]
-                loss = self._loss_phys(samples, condition.equation)
-            elif len(batch) == 3:
-                samples = pts[condition_idx == condition_id]
-                ground_truth = batch["output"][condition_idx == condition_id]
-                loss = self._loss_data(samples, ground_truth)
-            else:
-                raise ValueError("Batch size not supported")
-
-            # TODO for users this us hard to remember when creating a new solver, to fix in a smarter way
-            loss = loss.as_subclass(torch.Tensor)
+            if condition_name not in self.problem.conditions:
+                raise RuntimeError("Something wrong happened.")
 
-            #            # add condition losses and accumulate logging for each epoch
-            condition_losses.append(loss * condition.data_weight)
-            self.log(
-                condition_name + "_loss",
-                float(loss),
-                prog_bar=True,
-                logger=True,
-                on_epoch=True,
-                on_step=False,
+            # for data driven mode
+            if not hasattr(condition, "output_points"):
+                raise NotImplementedError(
+                    f"{type(self).__name__} works only in data-driven mode."
+                )
+
+            output_pts = out[condition_idx == condition_id]
+            input_pts = pts[condition_idx == condition_id]
+
+            loss = (
+                self.loss_data(input_pts=input_pts, output_pts=output_pts)
+                * condition.data_weight
             )
+            loss = loss.as_subclass(torch.Tensor)
 
-        # clamp unknown parameters of the InverseProblem to their domain ranges (if needed)
-        if isinstance(self.problem, InverseProblem):
-            self._clamp_inverse_problem_params()
-
-        # TODO Fix the bug, tot_loss is a label tensor without labels
-        # we need to pass it as a torch tensor to make everything work
-        total_loss = sum(condition_losses)
-        self.log(
-            "mean_loss",
-            float(total_loss / len(condition_losses)),
-            prog_bar=True,
-            logger=True,
-            on_epoch=True,
-            on_step=False,
-        )
+        self.log("mean_loss", float(loss), prog_bar=True, logger=True)
+        return loss
 
-        return total_loss
+    def loss_data(self, input_pts, output_pts):
+        """
+        The data loss for the Supervised solver. It computes the loss between
+        the network output against the true solution. This function
+        should not be override if not intentionally.
+
+        :param LabelTensor input_tensor: The input to the neural networks.
+        :param LabelTensor output_tensor: The true solution to compare the
+            network solution.
+        :return: The residual loss averaged on the input coordinates
+        :rtype: torch.Tensor
+        """
+        return self.loss(self.forward(input_pts), output_pts)
 
     @property
     def scheduler(self):
         """
-        Scheduler for the PINN training.
+        Scheduler for training.
         """
         return self._scheduler
 
     @property
     def neural_net(self):
         """
-        Neural network for the PINN training.
+        Neural network for training.
         """
         return self._neural_net
 
     @property
     def loss(self):
         """
-        Loss for the PINN training.
+        Loss for training.
         """
         return self._loss
```

### Comparing `pina-mathlab-0.1.0.post2403/pina/solvers/solver.py` & `pina-mathlab-0.1.1/pina/solvers/solver.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from abc import ABCMeta, abstractmethod
 from ..model.network import Network
 import pytorch_lightning
 from ..utils import check_consistency
 from ..problem import AbstractProblem
 import torch
+import sys
 
 
 class SolverInterface(pytorch_lightning.LightningModule, metaclass=ABCMeta):
     """
     Solver base class. This class inherits is a wrapper of
     LightningModule class, inheriting all the
     LightningModule methods.
@@ -138,14 +139,28 @@
 
     @property
     def problem(self):
         """
         The problem formulation."""
         return self._pina_problem
 
+    def on_train_start(self):
+        """
+        On training epoch start this function is call to do global checks for
+        the different solvers.
+        """
+
+        # 1. Check the verison for dataloader
+        dataloader = self.trainer.train_dataloader
+        if sys.version_info < (3, 8):
+            dataloader = dataloader.loaders
+        self._dataloader = dataloader
+
+        return super().on_train_start()
+
     # @model.setter
     # def model(self, new_model):
     #     """
     #     Set the torch."""
     #     check_consistency(new_model, nn.Module, 'torch model')
     #     self._model= new_model
```

### Comparing `pina-mathlab-0.1.0.post2403/pina/trainer.py` & `pina-mathlab-0.1.1/pina/trainer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Trainer module. """
 
+import torch
 import pytorch_lightning
 from .utils import check_consistency
 from .dataset import SamplePointDataset, SamplePointLoader, DataPointDataset
 from .solvers.solver import SolverInterface
 
 
 class Trainer(pytorch_lightning.Trainer):
@@ -59,14 +60,20 @@
 
         device = devices[0]
         dataset_phys = SamplePointDataset(self._model.problem, device)
         dataset_data = DataPointDataset(self._model.problem, device)
         self._loader = SamplePointLoader(
             dataset_phys, dataset_data, batch_size=self.batch_size, shuffle=True
         )
+        pb = self._model.problem
+        if hasattr(pb, "unknown_parameters"):
+            for key in pb.unknown_parameters:
+                pb.unknown_parameters[key] = torch.nn.Parameter(
+                    pb.unknown_parameters[key].data.to(device)
+                )
 
     def train(self, **kwargs):
         """
         Train the solver method.
         """
         return super().fit(
             self._model, train_dataloaders=self._loader, **kwargs
```

### Comparing `pina-mathlab-0.1.0.post2403/pina/utils.py` & `pina-mathlab-0.1.1/pina/utils.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina/writer.py` & `pina-mathlab-0.1.1/pina/writer.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/pina_mathlab.egg-info/PKG-INFO` & `pina-mathlab-0.1.1/pina_mathlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pina-mathlab
-Version: 0.1.0.post2403
+Version: 0.1.1
 Summary: Physic Informed Neural networks for Advance modeling.
 Home-page: https://github.com/mathLab/PINA
 Author: PINA Contributors
 Author-email: demo.nicola@gmail.com, dario.coscia@sissa.it
 License: MIT
 Keywords: physics-informed neural-network
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pina-mathlab-0.1.0.post2403/setup.py` & `pina-mathlab-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/tests/test_condition.py` & `pina-mathlab-0.1.1/tests/test_condition.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/tests/test_dataset.py` & `pina-mathlab-0.1.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/tests/test_label_tensor.py` & `pina-mathlab-0.1.1/tests/test_label_tensor.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/tests/test_operators.py` & `pina-mathlab-0.1.1/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/tests/test_plotter.py` & `pina-mathlab-0.1.1/tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/tests/test_problem.py` & `pina-mathlab-0.1.1/tests/test_problem.py`

 * *Files identical despite different names*

### Comparing `pina-mathlab-0.1.0.post2403/tests/test_utils.py` & `pina-mathlab-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

