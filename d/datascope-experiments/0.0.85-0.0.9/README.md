# Comparing `tmp/datascope-experiments-0.0.85.tar.gz` & `tmp/datascope-experiments-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascope-experiments-0.0.85.tar", last modified: Fri May 10 22:06:25 2024, max compression
+gzip compressed data, was "datascope-experiments-0.0.9.tar", last modified: Sat Jan  7 11:55:37 2023, max compression
```

## Comparing `datascope-experiments-0.0.85.tar` & `datascope-experiments-0.0.9.tar`

### file list

```diff
@@ -1,65 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:06:25.565373 datascope-experiments-0.0.85/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-10 22:06:25.565373 datascope-experiments-0.0.85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:06:25.557373 datascope-experiments-0.0.85/datascope/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:06:25.557373 datascope-experiments-0.0.85/datascope/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:06:25.557373 datascope-experiments-0.0.85/datascope/experiments/baselines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:06:25.557373 datascope-experiments-0.0.85/datascope/experiments/baselines/influence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/influence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/influence/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    33529 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/influence/genericNeuralNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/influence/hessians.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/influence/importance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/influence/logisticRegressionWithLBFGS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:06:25.561373 datascope-experiments-0.0.85/datascope/experiments/baselines/matchingnet/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/matchingnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/matchingnet/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/matchingnet/few_shot_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/matchingnet/matchingnet_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/matchingnet/predesigned_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/matchingnet/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/baselines/matchingnet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:06:25.561373 datascope-experiments-0.0.85/datascope/experiments/bench/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64286 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/bench/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/bench/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     9493 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/bench/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:06:25.561373 datascope-experiments-0.0.85/datascope/experiments/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76711 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/datasets/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:06:25.561373 datascope-experiments-0.0.85/datascope/experiments/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23485 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/pipelines/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    22471 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/pipelines/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/pipelines/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/pipelines/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:06:25.561373 datascope-experiments-0.0.85/datascope/experiments/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48488 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/reports/aggregate_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:06:25.561373 datascope-experiments-0.0.85/datascope/experiments/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/scenarios/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5297 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/scenarios/compute_time.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23625 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/scenarios/data_discard.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13941 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/scenarios/datascope_scenario.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20983 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/scenarios/label_repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/scenarios/marginal_contribution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:06:25.565373 datascope-experiments-0.0.85/datascope/experiments/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/utility/files.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/datascope/experiments/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:06:25.565373 datascope-experiments-0.0.85/datascope_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-10 22:06:25.000000 datascope-experiments-0.0.85/datascope_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-10 22:06:25.000000 datascope-experiments-0.0.85/datascope_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:06:25.000000 datascope-experiments-0.0.85/datascope_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 22:06:25.000000 datascope-experiments-0.0.85/datascope_experiments.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-10 22:06:25.000000 datascope-experiments-0.0.85/datascope_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 22:06:25.000000 datascope-experiments-0.0.85/datascope_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 22:06:25.565373 datascope-experiments-0.0.85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-10 22:05:08.000000 datascope-experiments-0.0.85/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.112194 datascope-experiments-0.0.9/datascope/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.112194 datascope-experiments-0.0.9/datascope/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope/experiments/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42998 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope/experiments/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/pipelines/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/pipelines/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope/experiments/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36299 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/reports/aggregate_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope/experiments/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46851 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6636 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/compute_time.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17443 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/data_discard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11559 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/datascope_scenario.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18395 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/label_repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/setup.py
```

### Comparing `datascope-experiments-0.0.85/PKG-INFO` & `datascope-experiments-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascope-experiments
-Version: 0.0.85
+Version: 0.0.9
 Summary: Module for running experiments on top of datascope.
 Home-page: https://ease.ml/datascope/
 Author-email: easeml@ds3lab.com
 License: MIT
 Description: # Experimental toolkit for ease.ml/datascope
         
         [![PyPI version](https://badge.fury.io/py/datascope-experiments.svg)](https://badge.fury.io/py/datascope-experiments)
```

### Comparing `datascope-experiments-0.0.85/datascope/experiments/bench/__init__.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 from .base import (
-    Configurable,
     Scenario,
     Study,
     Report,
     Backend,
     Queue as QueueProtocol,
     attribute,
     result,
     get_scenario_runner,
-    add_dynamic_arguments,
     DEFAULT_RESULTS_PATH,
     DEFAULT_RESULTS_SCENARIOS_PATH,
     DEFAULT_REPORTS_PATH,
     DEFAULT_STUDY_PATH,
     DEFAULT_BACKEND,
     DEFAULT_SLURM_JOBTIME,
     DEFAULT_SLURM_JOBMEMORY,
 )
-
-from .main import main
+from .label_repair import LabelRepairScenario
+from .data_discard import DataDiscardScenario
+from .compute_time import ComputeTimeScenario
 
 __all__ = [
-    "Configurable",
     "Scenario",
     "Study",
     "Report",
     "Backend",
     "QueueProtocol",
     "attribute",
     "result",
     "get_scenario_runner",
-    "add_dynamic_arguments",
     "DEFAULT_RESULTS_PATH",
     "DEFAULT_RESULTS_SCENARIOS_PATH",
     "DEFAULT_REPORTS_PATH",
     "DEFAULT_STUDY_PATH",
     "DEFAULT_BACKEND",
     "DEFAULT_SLURM_JOBTIME",
     "DEFAULT_SLURM_JOBMEMORY",
-    "main",
+    "LabelRepairScenario",
+    "DataDiscardScenario",
+    "ComputeTimeScenario",
 ]
```

### Comparing `datascope-experiments-0.0.85/datascope/experiments/bench/base.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import argparse
 import collections.abc
 import datetime
-import gc
 import gevent
 import gevent.signal
 import logging
 import logging.handlers
 import numpy as np
 import os
 import pandas as pd
@@ -20,38 +18,34 @@
 import threading
 import time
 import traceback
 import warnings
 import yaml
 import zerorpc
 
-from abc import abstractmethod
-from dataclasses import dataclass
+from abc import ABC, abstractmethod
 from enum import Enum
-from functools import cached_property
 from glob import glob
 from inspect import signature
 from io import TextIOBase, StringIO, SEEK_END
 from itertools import product
 from logging import Logger
 from matplotlib.figure import Figure
-from methodtools import lru_cache
 from multiprocessing import Process, Queue as MultiprocessingQueue
 from numpy import ndarray
 from pandas import DataFrame
 from ray.util.multiprocessing import Pool
 from ray.util.queue import Queue as RayQueue
 from shutil import copyfileobj
 from tqdm.auto import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 from typing import (
     Any,
     Callable,
     Dict,
-    Generic,
     Iterable,
     List,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
@@ -60,44 +54,29 @@
     get_args,
     overload,
     Union,
     Protocol,
 )
 
 
-def represent(x: Any):
-    if isinstance(x, Enum):
-        return repr(x.value)
-    else:
-        return repr(x)
-
-
-def stringify(x: Any):
-    if isinstance(x, Enum):
-        return str(x.value)
-    else:
-        return str(x)
-
-
 class Queue(Protocol):
-    def get(self, block: bool = True, timeout: Optional[float] = None) -> Any: ...
-
-    def put(self, item: Any, block: bool = True, timeout: Optional[float] = None) -> None: ...
+    def get(self, block: bool = True, timeout: Optional[float] = None) -> Any:
+        ...
 
-
-C = TypeVar("C")
+    def put(self, item: Any, block: bool = True, timeout: Optional[float] = None) -> None:
+        ...
 
 
 class PropertyTag(property):
+
     domain: Optional[Iterable] = None
-    inherit: bool = False
 
     @classmethod
-    def get_properties(cls: Type[C], target: object) -> Dict[str, C]:
-        res: Dict[str, C] = {}
+    def get_properties(cls: Type[property], target: object) -> Dict[str, property]:
+        res: Dict[str, property] = {}
         for name in dir(target):
             if hasattr(target, name):
                 member = getattr(target, name)
                 if isinstance(member, cls):
                     res[name] = member
         return res
 
@@ -105,20 +84,18 @@
 class attribute(PropertyTag):
     def __init__(
         self,
         fget: Optional[Callable[[Any], Any]] = None,
         fset: Optional[Callable[[Any, Any], None]] = None,
         fdel: Optional[Callable[[Any], None]] = None,
         doc: Optional[str] = None,
-        domain: Optional[Union[Iterable, Dict]] = None,
-        inherit: bool = False,
+        domain: Optional[Iterable] = None,
     ) -> None:
         super().__init__(fget, fset, fdel, doc)
         self.domain = domain
-        self.inherit = inherit
 
     def __call__(
         self,
         fget: Optional[Callable[[Any], Any]] = None,
         fset: Optional[Callable[[Any, Any], None]] = None,
         fdel: Optional[Callable[[Any], None]] = None,
         doc: Optional[str] = None,
@@ -127,49 +104,25 @@
             fget = self.fget
         if fset is None:
             fset = self.fset
         if fdel is None:
             fdel = self.fdel
         if doc is None:
             doc = self.__doc__
-        return type(self)(fget, fset, fdel, doc, domain=self.domain, inherit=self.inherit)
+        return type(self)(fget, fset, fdel, doc, self.domain)
 
     __isattribute__ = True
 
 
 class result(PropertyTag):
-    def __init__(
-        self,
-        fget: Optional[Callable[[Any], Any]] = None,
-        fset: Optional[Callable[[Any, Any], None]] = None,
-        fdel: Optional[Callable[[Any], None]] = None,
-        doc: Optional[str] = None,
-        lazy: bool = False,
-    ) -> None:
-        super().__init__(fget, fset, fdel, doc)
-        self.lazy = lazy
+    __isresult__ = True
 
-    def __call__(
-        self,
-        fget: Optional[Callable[[Any], Any]] = None,
-        fset: Optional[Callable[[Any, Any], None]] = None,
-        fdel: Optional[Callable[[Any], None]] = None,
-        doc: Optional[str] = None,
-    ) -> "result":
-        if fget is None:
-            fget = self.fget
-        if fset is None:
-            fset = self.fset
-        if fdel is None:
-            fdel = self.fdel
-        if doc is None:
-            doc = self.__doc__
-        return type(self)(fget, fset, fdel, doc, lazy=self.lazy)
 
-    __isresult__ = True
+# def extract_simpletype(target: object) -> type:
+#     pass
 
 
 def extract_enumtype(target: object) -> Optional[Type[Enum]]:
     if isinstance(target, type) and issubclass(target, Enum):
         return target
     else:
         origin = get_origin(target)
@@ -202,17 +155,17 @@
 
 
 def get_property_domain(target: object, name: str) -> List[Any]:
     prop, getter = get_property_and_getter(target, name)
     sign = signature(getter)
     enum = extract_enumtype(sign.return_annotation)
     if isinstance(prop, PropertyTag) and prop.domain is not None:
-        return list(prop.domain.keys()) if isinstance(prop.domain, dict) else list(prop.domain)
+        return list(prop.domain)
     elif sign.return_annotation is bool:
-        return [None]
+        return [False, True]
     elif enum is None:
         return [None]
     else:
         return list(enum.__members__.values())
 
 
 def get_property_helpstring(target: object, name: str) -> Optional[str]:
@@ -244,124 +197,24 @@
 def get_property_isiterable(target: object, name: str) -> bool:
     _, getter = get_property_and_getter(target, name)
     sign = signature(getter)
     a = sign.return_annotation
     return get_origin(a) in [collections.abc.Sequence, collections.abc.Iterable, list, set]
 
 
-def get_property_is_inheritable(target: object, name: str) -> bool:
-    member = getattr(target, name)
-    if isinstance(member, attribute):
-        return member.inherit
-    else:
-        return False
-
-
 def has_attribute_value(target: object, name: str, value: Any, ignore_none: bool = True) -> bool:
     target_value = get_property_value(target, name)
     if not isinstance(value, Iterable):
         value = [value]
     if ignore_none:
         return target_value is None or value == [None] or target_value in value
     else:
         return target_value in value
 
 
-def make_type_parser(target: Optional[type]) -> Callable[[str], Any]:
-    def parser(source: str) -> Any:
-        if target is None:
-            return source
-        result: Any = source
-        if issubclass(target, bool):
-            result = result in ["True", "true", "T", "t", "Yes", "yes", "y"]
-        elif issubclass(target, int):
-            result = int(result)
-        elif issubclass(target, float):
-            result = float(result)
-        elif issubclass(target, Enum):
-            result = target(result)
-        return result
-
-    return parser
-
-
-# TODO: Delete this function.
-def add_dynamic_arguments(
-    parser: argparse.ArgumentParser,
-    targets: Iterable[type],
-    all_iterable: bool = False,
-    single_instance: bool = False,
-) -> None:
-    attribute_domains: Dict[str, Set[Any]] = {}
-    attribute_helpstrings: Dict[str, Optional[str]] = {}
-    attribute_types: Dict[str, Optional[type]] = {}
-    attribute_defaults: Dict[str, Optional[Any]] = {}
-    attribute_isiterable: Dict[str, bool] = {}
-
-    for cls in targets:
-        # Extract domain of scenario.
-        props = attribute.get_properties(cls)
-        domain = dict((name, set(get_property_domain(cls, name))) for name in props.keys())
-
-        # Include the new domain into the total domain.
-        for name, values in domain.items():
-            attribute_domains.setdefault(name, set()).update(values)
-
-        # Extract types of the scenario attributes.
-        types = dict((name, get_property_type(cls, name)) for name in props.keys())
-        attribute_types.update(types)
-
-        # Extract helpstrings of the scenario attributes.
-        helpstrings = dict((name, get_property_helpstring(cls, name)) for name in props.keys())
-        attribute_helpstrings.update(helpstrings)
-
-        # Extract types of the scenario attributes.
-        defaults = dict((name, get_property_default(cls, name)) for name in props.keys())
-        attribute_defaults.update(defaults)
-
-        # Set all attributes to be iterable when passed to get_instances.
-        isiterable = dict((name, True if all_iterable else get_property_isiterable(cls, name)) for name in props.keys())
-        attribute_isiterable.update(isiterable)
-
-    for name in attribute_domains:
-        default = attribute_defaults[name]
-        attribute_domain: Optional[List] = [x.value if isinstance(x, Enum) else x for x in attribute_domains[name]]
-        if attribute_domain == [None]:
-            attribute_domain = None
-        helpstring = attribute_helpstrings[name] or ("Scenario " + name + ".")
-        if default is None:
-            helpstring += " Default: [all]" if not single_instance else ""
-        else:
-            helpstring += " Default: %s" % str(default)
-        parser.add_argument(
-            "--%s" % name.replace("_", "-"),
-            help=helpstring,
-            type=make_type_parser(attribute_types[name]),
-            choices=attribute_domain,
-            nargs=(1 if single_instance else "+") if attribute_isiterable[name] else None,  # type: ignore
-        )
-
-
-T = TypeVar("T")
-
-
-class LazyLoader(Generic[T]):
-    loader: Callable[[], T]
-    value: Optional[T]
-
-    def __init__(self, loader: Callable[[], T]) -> None:
-        self.loader = loader
-        self.value: Optional[T] = None
-
-    def __call__(self) -> T:
-        if self.value is None:
-            self.value = self.loader()
-        return self.value
-
-
 def save_dict(source: Dict[str, Any], dirpath: str, basename: str, saveonly: Optional[Sequence[str]] = None) -> None:
     basedict: Dict[str, Any] = dict((k, v) for (k, v) in source.items() if type(v) in [int, float, bool, str])
     basedict.update(dict((k, v.value) for (k, v) in source.items() if isinstance(v, Enum)))
     if len(basedict) > 0:
         with open(os.path.join(dirpath, ".".join([basename, "yaml"])), "w") as f:
             yaml.safe_dump(basedict, f)
 
@@ -388,20 +241,19 @@
                 data.savefig(fname=filename, bbox_extra_artists=extra_artists, bbox_inches="tight")
                 filename = os.path.join(dirpath, ".".join([basename, name, "png"]))
                 data.savefig(fname=filename, bbox_extra_artists=extra_artists, bbox_inches="tight")
             else:
                 raise ValueError("Key '%s' has unsupported type '%s'." % (name, str(type(data))))
 
 
-def load_dict(dirpath: str, basename: str, lazy: Optional[Sequence[str]] = None) -> Dict[str, Any]:
+def load_dict(dirpath: str, basename: str) -> Dict[str, Any]:
     if not os.path.isdir(dirpath):
         raise ValueError("The provided path '%s' does not point to a directory." % dirpath)
 
     res: Dict[str, Any] = {}
-    lazy = [] if lazy is None else lazy
 
     filename = os.path.join(dirpath, ".".join([basename, "yaml"]))
     if os.path.isfile(filename):
         with open(filename, "r") as f:
             res.update(yaml.safe_load(f))
 
     for path in glob(os.path.join(dirpath, basename) + "*"):
@@ -409,23 +261,17 @@
         base, ext = os.path.splitext(filename)
         name = base[len(basename) + 1 :]  # noqa: E203
 
         if name == "":
             continue
 
         if ext == ".npy":
-            if name in lazy:
-                res[name] = LazyLoader(lambda: np.load(path))
-            else:
-                res[name] = np.load(path)
+            res[name] = np.load(path)
         elif ext == ".csv":
-            if name in lazy:
-                res[name] = LazyLoader(lambda: pd.read_csv(path, index_col=0))
-            else:
-                res[name] = pd.read_csv(path, index_col=0)
+            res[name] = pd.read_csv(path)
         elif ext == ".yaml":
             with open(path) as f:
                 res[name] = yaml.safe_load(f)
         else:
             warnings.warn("File '%s' with unsupported extension '%s' will be ignored." % (path, ext))
 
     return res
@@ -507,303 +353,67 @@
         elif event.type == Progress.Event.Type.CLOSE:
             cls.pbars[event.id].close()
             del cls.pbars[event.id]
             # Ensure that bars get redrawn properly after they reshuffle due to closure of one of them.
             cls.refresh()
 
 
-@dataclass
-class AttributeDescriptor:
-    attr_type: Optional[type]
-    helpstring: Optional[str]
-    is_iterable: bool
-    domain: Iterable
-    default: Any
-    inherit: bool = False
-
-
-def get_all_subclasses(cls):
-    all_subclasses = []
-    for subclass in cls.__subclasses__():
-        all_subclasses.append(subclass)
-        all_subclasses.extend(get_all_subclasses(subclass))
-    return all_subclasses
-
-
-def get_class(class_id: str) -> Optional[type]:
-    import importlib
-
-    module_name, class_name = class_id.rsplit(".", 1)
-    try:
-        module = importlib.import_module(module_name)
-        return getattr(module, class_name)
-    except (ModuleNotFoundError, AttributeError):
-        return None
-
-
-class Configurable:
-    NESTING_SEPARATOR = "_"
-    _class_id: str
-    _class_longname: Optional[str] = None
-    _class_argname: str = "class"
-    _class_abstract: bool = True
-
-    def __init_subclass__(
-        cls: Type["Configurable"],
-        id: Optional[str] = None,
-        longname: Optional[str] = None,
-        argname: Optional[str] = None,
-        abstract: bool = False,
-    ) -> None:
-        cls._class_id = id if id is not None else "%s.%s" % (cls.__module__, cls.__name__)
-        cls._class_longname = longname if longname is not None else cls.__name__
-        if argname is not None:
-            cls._class_argname = argname
-        cls._class_abstract = abstract
-
-    @lru_cache(maxsize=2)
-    @classmethod
-    def get_subclasses(cls: Type["Configurable"], include_abstract: bool = False) -> Dict[str, Type["Configurable"]]:
-        subclasses = {c.get_class_identifier(): c for c in cls.__subclasses__()}
-        subsubclasses: Dict[str, Type["Configurable"]] = {}
-        for c in subclasses.values():
-            subsubclasses.update(**c.get_subclasses())
-        subclasses.update(subsubclasses)
-        if include_abstract:
-            return subclasses
-        else:
-            return {k: v for k, v in subclasses.items() if not v._class_abstract}
-
-    @classmethod
-    def get_class_identifier(cls: Type["Configurable"]) -> str:
-        return cls._class_id
-
-    @lru_cache(maxsize=8)
-    @classmethod
-    def _get_attribute_descriptors(
-        cls: Type["Configurable"],
-        flattened: bool = False,
-        include_subclasses: bool = False,
-        include_classarg: bool = False,
-    ) -> Dict[str, AttributeDescriptor]:
-        attribute_descriptors = {}
-        if include_classarg:
-            attribute_descriptors[cls._class_argname] = AttributeDescriptor(
-                attr_type=str,
-                helpstring="Identifier of the specific %s instance." % cls.__name__.lower(),
-                is_iterable=False,
-                domain=list(cls.get_subclasses().keys()),
-                default=None,
-                inherit=False,
-            )
-        properties = attribute.get_properties(cls)
-        for name, prop in properties.items():
-            attr_type = get_property_type(cls, name)
-            helpstring = get_property_helpstring(cls, name)
-            is_iterable = get_property_isiterable(cls, name)
-            inherit = get_property_is_inheritable(cls, name)
-            default = get_property_default(cls, name)
-            if attr_type is not None and issubclass(attr_type, Configurable) and flattened:
-                domain = list(attr_type.get_subclasses().keys())
-                attribute_descriptors[name] = AttributeDescriptor(
-                    attr_type=str,
-                    helpstring=helpstring,
-                    is_iterable=is_iterable,
-                    domain=domain,
-                    default=default,
-                    inherit=inherit,
-                )
-                nested_attribute_descriptors = attr_type._get_attribute_descriptors(
-                    flattened=True, include_subclasses=True
-                )
-                for nested_name, nested_descriptor in nested_attribute_descriptors.items():
-                    attribute_descriptors[name + cls.NESTING_SEPARATOR + nested_name] = nested_descriptor
-            else:
-                domain = get_property_domain(cls, name)
-                attribute_descriptors[name] = AttributeDescriptor(
-                    attr_type=attr_type,
-                    helpstring=helpstring,
-                    is_iterable=is_iterable,
-                    domain=domain,
-                    default=default,
-                    inherit=inherit,
-                )
-
-        if include_subclasses:
-            for subclass in cls.get_subclasses().values():
-                subclass_descriptors = subclass._get_attribute_descriptors(
-                    flattened=flattened, include_subclasses=False
-                )
-                attribute_descriptors.update(subclass_descriptors)
-
-        return attribute_descriptors
-
-    @cached_property
-    def attributes(self) -> Dict[str, Any]:
-        props = attribute.get_properties(type(self))
-        attributes = dict((name, get_property_value(self, name)) for name in props.keys())
-        attributes[self._class_argname] = self.get_class_identifier()
-        return attributes
-
-    def __repr__(self) -> str:
-        full_class_id = "%s.%s" % (type(self).__module__, type(self).__name__)
-        class_id = self.get_class_identifier()
-        result = str(self)
-        if result.startswith(class_id) and class_id != full_class_id:
-            result = result.replace(class_id, full_class_id, 1)
-        return result
+class Scenario(ABC):
 
-    def __str__(self) -> str:
-        result = self.get_class_identifier()
-        attributes = self.attributes
-        attribute_string = ", ".join(
-            ["%s=%s" % (str(k), stringify(attributes[k])) for k in sorted(attributes) if k != self._class_argname]
-        )
-        if len(attribute_string) > 0:
-            result += "(%s)" % attribute_string
-        return result
+    scenarios: Dict[str, Type["Scenario"]] = {}
+    scenario_domains: Dict[str, Dict[str, Set[Any]]] = {}
+    attribute_domains: Dict[str, Set[Any]] = {}
+    attribute_helpstrings: Dict[str, Optional[str]] = {}
+    attribute_types: Dict[str, Optional[type]] = {}
+    attribute_defaults: Dict[str, Optional[Any]] = {}
+    attribute_isiterable: Dict[str, bool] = {}
+    _scenario: Optional[str] = None
 
-    @classmethod
-    def _compose_attributes(cls: Type["Configurable"], attributes: Dict[str, Any]) -> Dict[str, Any]:
-        attribute_descriptors: Dict[str, AttributeDescriptor] = cls._get_attribute_descriptors()
-        result: Dict[str, Any] = {}
-        skip_prefixes: Set[str] = set()
-        for k in sorted(attributes.keys()):
-            if any(k.startswith(prefix) for prefix in skip_prefixes):
-                continue
-            v = attributes[k]
-            result[k] = v
-            if isinstance(v, str) or isinstance(v, dict):
-                target_base_descriptor = attribute_descriptors.get(k, None)
-                if target_base_descriptor is not None:
-                    target_base_cls = target_base_descriptor.attr_type
-                    if target_base_cls is not None and issubclass(target_base_cls, Configurable):
-                        target_cls_id = v if isinstance(v, str) else v.get(target_base_cls._class_argname, None)
-                        if target_cls_id is None:
-                            raise ValueError(
-                                "If the key '%s' contains a nested dictionary, it must have a "
-                                "key '%s' corresponding to the class identifier." % (k, target_base_cls._class_argname)
-                            )
-
-                        target_cls = target_base_cls.get_subclasses().get(target_cls_id, None)
-                        if target_cls is None:
-                            target_cls = get_class(target_cls_id)
-                            if target_cls is not None:
-                                if not issubclass(target_cls, target_base_cls) or not issubclass(
-                                    target_cls, Configurable
-                                ):
-                                    target_cls = None
-
-                        if target_cls is not None:
-                            target_attributes = {}
-
-                            # If any attributes are inheritable, pass them down.
-                            target_attribute_descriptors: Dict[str, AttributeDescriptor] = (
-                                target_cls._get_attribute_descriptors()
-                            )
-                            for kk, vd in target_attribute_descriptors.items():
-                                if vd.inherit:
-                                    target_attributes[kk] = attributes[kk]
-
-                            # Pass down all attributes that are prefixed with the current key.
-                            target_attributes.update(
-                                {
-                                    kk.removeprefix(k + cls.NESTING_SEPARATOR): vv
-                                    for kk, vv in attributes.items()
-                                    if kk.startswith(k + cls.NESTING_SEPARATOR)
-                                }
-                            )
-
-                            # If the value is a nested dictionary, then we reuse its attributes.
-                            if isinstance(v, dict):
-                                target_attributes.update(
-                                    {kk: vv for kk, vv in v.items() if kk != target_base_cls._class_argname}
-                                )
-
-                            # Recursively compose target attributes and instantiate the configurable object.
-                            target_attributes = target_cls._compose_attributes(target_attributes)
-                            result[k] = target_cls(**target_attributes)
+    def __init__(self, id: Optional[str] = None, logstream: Optional[TextIOBase] = None, **kwargs: Any) -> None:
+        super().__init__()
+        self._id = id if id is not None else "".join(random.choices(string.ascii_lowercase + string.digits, k=10))
+        self._logstream = logstream if logstream is not None else StringIO()
+        self._progress = Progress(id=self._id)
+        self._attributes: Optional[Dict[str, Any]] = None
 
-                            # Ensure that the nested attributes are not passed to the parent object constructor.
-                            skip_prefixes.add(k + cls.NESTING_SEPARATOR)
-        return result
+    def __init_subclass__(cls: Type["Scenario"], id: Optional[str] = None, abstract: bool = False) -> None:
+        if abstract or id is None:
+            return
+
+        # Register scenario under the given name.
+        cls._scenario = id
+        Scenario.scenarios[id] = cls
+        assert isinstance(Scenario.scenario, PropertyTag)
+        assert isinstance(Scenario.scenario.domain, set)
+        Scenario.scenario.domain.add(id)
 
-    @classmethod
-    def _flatten_attributes(cls: Type["Configurable"], attributes: Dict[str, Any]) -> Dict[str, Any]:
-        result: Dict[str, Any] = {}
-        for k, v in attributes.items():
-            if isinstance(v, Configurable):
-                result[k] = v.get_class_identifier()
-                ejected_attributes = v._flatten_attributes(v.attributes)
-                for kk, vv in ejected_attributes.items():
-                    result[k + cls.NESTING_SEPARATOR + kk] = vv
-            else:
-                result[k] = v
-        return result
+        # Extract domain of scenario.
+        props = attribute.get_properties(cls)
+        domain = dict((name, set(get_property_domain(cls, name))) for name in props.keys())
+        Scenario.scenario_domains[id] = domain
 
-    @classmethod
-    def from_dict(cls: Type["Configurable"], attributes: Dict[str, Any]) -> "Configurable":
-        class_id = attributes.get(cls._class_argname, None)
-        target_class = cls
-        if class_id is not None and class_id != cls.get_class_identifier():
-            # If class_id is provided, then we need to find the corresponding subclass.
-            target_class = cls.get_subclasses().get(class_id, None)
-            if target_class is None:
-                target_cls = get_class(class_id)
-                if target_cls is not None:
-                    if not issubclass(target_cls, Configurable):
-                        target_cls = None
-            if target_class is None:
-                raise ValueError("The provided class ID '%s' does not correspond to any valid class." % class_id)
-        elif cls._class_abstract:
-            # If class_id is not provided, then we need to ensure that cls is not abstract.
-            raise ValueError(
-                "Function called on abstract class '%s' but argument '%s' specifying subclass is missing."
-                % (cls._class_id, cls._class_argname)
-            )
-        attributes = target_class._compose_attributes(attributes)
-        return target_class(**attributes)
+        # Include the new domain into the total domain.
+        for name, values in domain.items():
+            Scenario.attribute_domains.setdefault(name, set()).update(values)
 
-    @classmethod
-    def add_dynamic_arguments(
-        cls: Type["Configurable"],
-        parser: argparse.ArgumentParser,
-        all_iterable: bool = False,
-        single_instance: bool = False,
-    ) -> None:
-        attribute_descriptors: Dict[str, AttributeDescriptor] = cls._get_attribute_descriptors(
-            flattened=True, include_subclasses=True, include_classarg=True
-        )
-        for name, descriptor in attribute_descriptors.items():
-            attribute_domain: Optional[List] = [x.value if isinstance(x, Enum) else x for x in descriptor.domain]
-            if attribute_domain == [None]:
-                attribute_domain = None
-            helpstring = descriptor.helpstring or ("Scenario " + name + ".")
-            if descriptor.default is None:
-                helpstring += " Default: [all]" if not single_instance else ""
-            else:
-                helpstring += " Default: %s" % str(descriptor.default)
-            nargs = (1 if single_instance else "+") if (descriptor.is_iterable or all_iterable) else None
-            parser.add_argument(
-                "--%s" % name.replace("_", "-"),
-                help=helpstring,
-                type=make_type_parser(descriptor.attr_type),
-                choices=attribute_domain,
-                nargs=nargs,  # type: ignore
-            )
+        # Extract types of the scenario attributes.
+        types = dict((name, get_property_type(cls, name)) for name in props.keys())
+        Scenario.attribute_types.update(types)
 
+        # Extract helpstrings of the scenario attributes.
+        helpstrings = dict((name, get_property_helpstring(cls, name)) for name in props.keys())
+        Scenario.attribute_helpstrings.update(helpstrings)
 
-class Scenario(Configurable, argname="scenario"):
+        # Extract types of the scenario attributes.
+        defaults = dict((name, get_property_default(cls, name)) for name in props.keys())
+        Scenario.attribute_defaults.update(defaults)
 
-    def __init__(self, id: Optional[str] = None, logstream: Optional[TextIOBase] = None, **kwargs: Any) -> None:
-        super().__init__()
-        self._id = id if id is not None else "".join(random.choices(string.ascii_lowercase + string.digits, k=10))
-        self._logstream = logstream if logstream is not None else StringIO()
-        self._progress = Progress(id=self._id)
-        self._attributes: Optional[Dict[str, Any]] = None
+        # Set all attributes to be iterable when passed to get_instances.
+        isiterable = dict((k, True) for k in props.keys())
+        Scenario.attribute_isiterable.update(isiterable)
 
     def run(self, progress_bar: bool = True, console_log: bool = True) -> None:
         # Set up logging.
         formatter = logging.Formatter("[%(asctime)s] [%(levelname)s] %(message)s")
         fh = logging.StreamHandler(self._logstream)
         fh.setFormatter(formatter)
         self.logger.addHandler(fh)
@@ -837,14 +447,21 @@
         raise NotImplementedError()
 
     @property
     @abstractmethod
     def dataframe(self) -> DataFrame:
         raise NotImplementedError()
 
+    @attribute(domain=set())
+    def scenario(self) -> str:
+        """Type of scenario."""
+        if self._scenario is None:
+            raise ValueError("Cannot call this on an abstract class instance.")
+        return self._scenario
+
     @attribute
     def id(self) -> str:
         """A unique identifier of the scenario."""
         return self._id
 
     @property
     def progress(self) -> Progress:
@@ -862,48 +479,47 @@
     def log(self) -> str:
         result = ""
         self._logstream.seek(0)
         result = "\n".join(self._logstream.readlines())
         self._logstream.seek(0, SEEK_END)
         return result
 
-    @lru_cache(maxsize=1)
-    @classmethod
-    def get_keyword_replacements(cls: Type["Scenario"]) -> Dict[str, str]:
+    @property
+    def attributes(self) -> Dict[str, Any]:
+        if self._attributes is None:
+            props = attribute.get_properties(self.__class__)
+            self._attributes = dict((name, get_property_value(self, name)) for name in props.keys())
+        return self._attributes
+
+    @property
+    def keyword_replacements(self) -> Dict[str, str]:
         return {}
 
     @classmethod
-    def get_instances(cls: Type["Scenario"], **kwargs: Any) -> Iterable["Scenario"]:
+    def get_instances(cls, **kwargs: Any) -> Iterable["Scenario"]:
         if cls == Scenario:
-            # for id, scenario in Scenario.scenarios.items():
-            for id, subclass in Scenario.get_subclasses().items():
+            for id, scenario in Scenario.scenarios.items():
                 if kwargs.get("scenario", None) is None or id in kwargs["scenario"]:
-                    assert issubclass(subclass, Scenario)
-                    for instance in subclass.get_instances(**kwargs):
+                    for instance in scenario.get_instances(**kwargs):
                         yield instance
         else:
-            attribute_descriptors: Dict[str, AttributeDescriptor] = cls._get_attribute_descriptors(flattened=True)
             domains = []
-            names = list(attribute_descriptors.keys())
+            names = Scenario.attribute_domains.keys()
             for name in names:
                 if name in kwargs and kwargs[name] is not None:
                     domain = kwargs[name]
-                    if not isinstance(domain, Iterable) or isinstance(domain, str):
+                    if not isinstance(domain, Iterable):
                         domain = [domain]
                     domains.append(list(domain))
                 else:
-                    domains.append(list(attribute_descriptors[name].domain))
-            print("len(list(product(*domains)))", len(list(product(*domains))))
+                    domains.append(list(Scenario.attribute_domains[name]))
             for values in product(*domains):
                 attributes = dict((name, value) for (name, value) in zip(names, values) if value is not None)
-                composed_attributes = cls._compose_attributes(attributes)
-                if cls.is_valid_config(**composed_attributes):
-                    scenario = cls(**composed_attributes)
-                    # assert isinstance(scenario, Scenario)
-                    yield scenario
+                if cls.is_valid_config(**attributes):
+                    yield cls(**attributes)
 
     @classmethod
     def is_valid_config(cls, **attributes: Any) -> bool:
         return True
 
     def save(self, path: str) -> None:
         if os.path.splitext(path)[1] != "":
@@ -914,42 +530,53 @@
         logpath = os.path.join(path, "scenario.log")
         with open(logpath, "w") as f:
             self._logstream.seek(0)
             copyfileobj(self._logstream, f)
             self._logstream.seek(0, SEEK_END)
 
         # Save attributes as a single yaml file.
-        attributes = self._flatten_attributes(self.attributes)
+        props = attribute.get_properties(type(self))
+        attributes = dict((name, prop.fget(self) if prop.fget is not None else None) for (name, prop) in props.items())
         save_dict(attributes, path, "attributes")
 
         # Save results as separate files.
-        props: Dict[str, result] = result.get_properties(type(self))
+        props = result.get_properties(type(self))
         results = dict((name, prop.fget(self) if prop.fget is not None else None) for (name, prop) in props.items())
         save_dict(results, path, "results")
 
+    def __str__(self) -> str:
+        props = attribute.get_properties(type(self))
+        attributes = dict((name, prop.fget(self) if prop.fget is not None else None) for (name, prop) in props.items())
+        for k, v in attributes.items():
+            if isinstance(v, Enum):
+                attributes[k] = v.value
+        return "(%s)" % ", ".join(["%s=%s" % (str(k), str(v)) for (k, v) in attributes.items()])
+
+    @classmethod
+    def from_dict(cls, source: Dict[str, Any]) -> "Scenario":
+        scenario_id = source["scenario"]
+        scenario_cls = cls.scenarios[scenario_id]
+        return scenario_cls(**source)
+
     @classmethod
     def load(cls, path: str) -> "Scenario":
         if not os.path.isdir(path):
             raise ValueError("The provided path '%s' does not point to a directory." % path)
 
         # Load the log file.
         logpath = os.path.join(path, "scenario.log")
         logstream: Optional[TextIOBase] = None
         if os.path.isfile(logpath):
             with open(logpath, "r") as f:
                 logstream = StringIO(f.read())
 
         attributes = load_dict(path, "attributes")
-        attributes = cls._compose_attributes(attributes)
-        lazy = [k for k, v in result.get_properties(cls).items() if v.lazy]
-        results = load_dict(path, "results", lazy=lazy)
+        results = load_dict(path, "results")
         kwargs = {"logstream": logstream}
-        scenario = cls.from_dict({**attributes, **results, **kwargs})
-        assert isinstance(scenario, Scenario)
-        return scenario
+        return cls.from_dict({**attributes, **results, **kwargs})
 
     @classmethod
     def isscenario(cls, path: str) -> bool:
         attributes_filename = os.path.join(path, ".".join(["attributes", "yaml"]))
         return os.path.isdir(path) and os.path.isfile(attributes_filename)  # TODO: Refine this check.
 
     def is_match(self, other: "Scenario") -> bool:
@@ -996,23 +623,15 @@
         return self._data.__getitem__(index)
 
     def __len__(self) -> int:
         return self._data.__len__()
 
     @property
     def df(self):
-        data = [
-            (
-                x._flatten_attributes(x.attributes)
-                if isinstance(x, Configurable)
-                else {a: get_value(x, a) for a in self._attributes}
-            )
-            for x in self._data
-        ]
-        df = pd.DataFrame.from_dict({a: [x.get(a, None) for x in data] for a in self._attributes})
+        df = pd.DataFrame.from_dict({a: [get_value(x, a) for x in self._data] for a in self._attributes})
         if self._key is not None:
             df.set_index(self._key, inplace=True)
         return df
 
     def __repr__(self) -> str:
         return self.df.__repr__()
 
@@ -1034,15 +653,14 @@
 def get_scenario_runner(
     queue: Optional[Queue] = None,
     catch_exceptions: bool = True,
     progress_bar: bool = True,
     console_log: bool = True,
     rerun: bool = False,
     pickled_queue: bool = False,
-    job_memory: Optional[str] = None,
 ) -> Callable[[Scenario], Scenario]:
     def _scenario_runner(scenario: Scenario) -> Scenario:
         try:
             scenario.progress.queue = queue
             scenario.progress.pickled = pickled_queue
             scenario.logger.setLevel(logging.DEBUG)
             qh: Optional[logging.Handler] = None
@@ -1056,23 +674,14 @@
                 queue.put(payload)
             elif console_log:
                 formatter = logging.Formatter("[%(asctime)s] [%(levelname)s] [%(name)s] %(message)s")
                 ch = logging.StreamHandler(sys.stdout)
                 ch.setFormatter(formatter)
                 scenario.logger.addHandler(ch)
 
-            # Quickly consume a 70% of the given amount of memory for 10 seconds.
-            if job_memory is not None:
-                suffixes = {"G": 1024**3, "M": 1024**2, "K": 1024}
-                size = int(float(job_memory[:-1]) * suffixes[job_memory[-1]] * np.random.uniform(0.55, 0.7))
-                data = bytearray(size)  # noqa: F841
-                time.sleep(10)
-                del data
-                gc.collect()
-
             if rerun or not scenario.completed:
                 if queue is not None:
                     scenario.run(progress_bar=progress_bar, console_log=False)
                 else:
                     with logging_redirect_tqdm(loggers=[scenario.logger]):
                         scenario.run(progress_bar=progress_bar, console_log=False)
             else:
@@ -1122,33 +731,14 @@
             sock.close()
             return port
         except OSError:
             port += 1
     raise IOError("Cannot find a free port.")
 
 
-def update_keyword_prefixes(
-    keyword_replacements: Dict[str, str],
-    prefix_mappings: Optional[Dict[str, str]] = None,
-    key_separator: str = Configurable.NESTING_SEPARATOR,
-    value_separator: str = " ",
-) -> Dict[str, str]:
-    result = keyword_replacements
-    if prefix_mappings is not None:
-        result = {}
-        for key_prefix, value_prefix in prefix_mappings.items():
-            result.update(
-                {
-                    key_prefix + key_separator + k: value_prefix + value_separator + v
-                    for k, v in keyword_replacements.items()
-                }
-            )
-    return result
-
-
 DEFAULT_RESULTS_PATH = os.path.join("var", "results")
 DEFAULT_RESULTS_SCENARIOS_PATH = os.path.join("var", "results", "scenarios")
 DEFAULT_REPORTS_PATH = os.path.join("var", "reports")
 ALL_STUDY_PATHS = glob(os.path.join(DEFAULT_RESULTS_PATH, "*"))
 DEFAULT_STUDY_PATH = max(ALL_STUDY_PATHS, key=lambda x: os.path.getmtime(x)) if len(ALL_STUDY_PATHS) > 0 else None
 DEFAULT_SCENARIO_PATH_FORMAT = "{id}"
 DEFAULT_BACKEND = Backend.LOCAL
@@ -1168,15 +758,14 @@
     ) -> None:
         self._scenarios = scenarios
         self._id = id if id is not None else datetime.datetime.now().strftime("Study-%Y-%m-%d-%H-%M-%S")
         self._outpath = outpath
         self._scenario_path_format = scenario_path_format
         self._logstream = logstream if logstream is not None else StringIO()
         self._logger = logging.getLogger(self._id)
-        self._logger.setLevel(logging.DEBUG)
         self._verify_scenario_path(scenario_path_format, scenarios)
 
     @staticmethod
     def _status_monitor(
         queue: Queue,
         logger: Logger,
         study_queue: Optional[Queue] = None,
@@ -1209,80 +798,92 @@
         console_log: bool = True,
         backend: Backend = DEFAULT_BACKEND,
         ray_address: Optional[str] = None,
         ray_numprocs: Optional[int] = None,
         slurm_jobtime: Optional[str] = DEFAULT_SLURM_JOBTIME,
         slurm_jobmemory: Optional[str] = DEFAULT_SLURM_JOBMEMORY,
         slurm_constraint: Optional[str] = None,
-        slurm_partition: Optional[str] = None,
-        slurm_maxjobs: Optional[int] = None,
-        slurm_args: Optional[str] = None,
         eventstream_host_ip: Optional[str] = None,
         eventstream_host_port: Optional[int] = None,
         eagersave: bool = True,
-        **kwargs: Any,
+        **kwargs: Any
     ) -> None:
+
         # Set up logging.
         formatter = logging.Formatter("[%(asctime)s] [%(levelname)s] [%(name)s] %(message)s")
         fh = logging.StreamHandler(self._logstream)
         fh.setFormatter(formatter)
         self.logger.addHandler(fh)
         ch: Optional[logging.Handler] = None
         if console_log:
             ch = logging.StreamHandler(sys.stdout)
             ch.setFormatter(formatter)
             self.logger.addHandler(ch)
 
         # Set up progress bar.
+        # pbar = None if not progress_bar else tqdm(total=len(self.scenarios), desc="Scenarios", position=0)
         queue: Optional[Queue] = None
         process: Optional[Process] = None
         pickled_queue = backend == Backend.SLURM
         if backend == Backend.RAY:
             queue = RayQueue()
         elif backend == Backend.SLURM:
             queue = MultiprocessingQueue()
 
         pbar = None if not progress_bar else Progress(queue, id=self.id, pickled=pickled_queue)
         if pbar is not None:
             pbar.start(total=len(self.scenarios), desc="Scenarios")
 
         with logging_redirect_tqdm(loggers=[self.logger]):
+            # for scenario in self.scenarios:
+            #     try:
+            #         scenario.run(logger=self._logger, progress_bar=progress_bar, **kwargs)
+            #     except Exception as e:
+            #         if catch_exceptions:
+            #             trace_output = traceback.format_exc()
+            #             print(trace_output)
+            #         else:
+            #             raise e
+            #     finally:
+            #         if pbar is not None:
+            #             pbar.update(1)
 
             scenarios = []
             runner = get_scenario_runner(
                 queue, catch_exceptions, progress_bar, console_log, pickled_queue=pickled_queue
             )
-            if backend == Backend.LOCAL:
-                for scenario in map(runner, self.scenarios):
+            if backend == Backend.RAY:
+                monitor = threading.Thread(target=Study._status_monitor, args=(queue, self.logger))
+                monitor.start()
+                pool = Pool(processes=ray_numprocs, ray_address=ray_address)
+                for scenario in pool.imap_unordered(runner, self.scenarios):
                     scenarios.append(scenario)
                     if pbar is not None:
                         pbar.update(1)
                     if eagersave:
                         self.save_scenario(scenario)
 
-            elif backend == Backend.RAY:
-                monitor = threading.Thread(target=Study._status_monitor, args=(queue, self.logger))
-                monitor.start()
-                pool = Pool(processes=ray_numprocs, ray_address=ray_address)
-                for scenario in pool.imap_unordered(runner, self.scenarios):
+            elif backend == Backend.LOCAL:
+                for scenario in map(runner, self.scenarios):
                     scenarios.append(scenario)
                     if pbar is not None:
                         pbar.update(1)
                     if eagersave:
                         self.save_scenario(scenario)
 
             elif backend == Backend.SLURM:
+
                 # If the host port was not specified, we look for the first free port.
                 if eventstream_host_port is None:
                     eventstream_host_port = get_free_port(DEFAULT_EVENTSTREAM_HOST_PORT)
 
                 # Set up the process that will host the queue RPC server.
                 # Reference: https://stackoverflow.com/a/21146917
                 def serve(queue: Queue) -> None:
-                    server = zerorpc.Server(queue, heartbeat=45)
+                    server = zerorpc.Server(queue, heartbeat=5)
                     assert eventstream_host_port is not None
                     server.bind("tcp://0.0.0.0:%d" % eventstream_host_port)
 
                     def stop_routine():
                         server.stop()
 
                     def stop_handler(number, frame):
@@ -1303,68 +904,45 @@
                 monitor.start()
 
                 if eventstream_host_ip is None:
                     eventstream_host_ip = get_ip()
                 address = "tcp://%s:%d" % (eventstream_host_ip, eventstream_host_port)
                 self.logger.info("Status event monitor listening on " + address)
 
-                try:
-                    # Create a batch job on slurm for every scenario.
-                    scenarios_pending = len(self.scenarios)
-                    scenarios_running = 0
-                    for scenario in self.scenarios:
-                        scenarios_pending -= 1
-                        if scenario.completed:
-                            if pbar is not None:
-                                pbar.update(1)
-                        else:
-                            path = self.save_scenario(scenario)
-                            logpath = os.path.join(path, "slurm.log")
-                            run_command = "python -m datascope.experiments run-scenario -o %s -e %s -m %s" % (
-                                path,
-                                address,
-                                slurm_jobmemory,
-                            )
-                            slurm_command = "sbatch --job-name=%s" % self.id
-                            slurm_command += " --time=%s" % slurm_jobtime
-                            slurm_command += " --mem-per-cpu=%s" % slurm_jobmemory
-                            if slurm_constraint is not None:
-                                slurm_command += " --constraint=%s" % slurm_constraint
-                            if slurm_partition is not None:
-                                slurm_command += " --partition=%s" % slurm_partition
-                            if slurm_args is not None:
-                                slurm_command += " %s " % slurm_args
-                            slurm_command += " --output=%s" % logpath
-                            slurm_command += ' --wrap="%s"' % run_command
-                            result = subprocess.run(slurm_command, capture_output=True, shell=True)
-                            if result.returncode != 0:
-                                raise RuntimeError(
-                                    "Slurm sbatch command gave a non-zero return code. \nstdout:\n%r\nstderr:\n%r\n"
-                                    % (result.stdout, result.stderr)
-                                )
-                            scenarios_running += 1
-
-                        # Check if we need to wait for jobs to finish. We do that either when
-                        # the maximum number of allowed jobs has been reached
-                        # or if all jobs have been submitted but not all have finished yet.
-                        while (slurm_maxjobs is not None and scenarios_running > slurm_maxjobs) or (
-                            scenarios_pending <= 0 and scenarios_running > 0
-                        ):
-                            scenario_event: ScenarioEvent = study_queue.get()
-                            if scenario_event.type == ScenarioEvent.Type.COMPLETED:
-                                scenarios_running -= 1
-                                if pbar is not None:
-                                    pbar.update(1)
-
-                except (Exception, KeyboardInterrupt) as e:
-                    # Make sure to cancel all submitted slurm jobs in case of an exception or keyboard interrupt.
-                    self.logger.info("Running: scancel --name=%s" % self.id)
-                    subprocess.run(["scancel", "--name=%s" % self.id])
-                    self.logger.info("Slurm jobs canceled.")
-                    raise e
+                # Create a batch job on slurm for every scenario.
+                scenarios_running = len(self.scenarios)
+                for scenario in self.scenarios:
+                    if scenario.completed:
+                        scenarios_running -= 1
+                        if pbar is not None:
+                            pbar.update(1)
+                        continue
+                    path = self.save_scenario(scenario)
+                    logpath = os.path.join(path, "slurm.log")
+                    run_command = "python -m datascope.experiments run-scenario -o %s -e %s" % (path, address)
+                    slurm_command = "sbatch --job-name=datascope-experiment"
+                    slurm_command += " --time=%s" % slurm_jobtime
+                    slurm_command += " --mem-per-cpu=%s" % slurm_jobmemory
+                    if slurm_constraint is not None:
+                        slurm_command += " --constraint=%s" % slurm_constraint
+                    slurm_command += " --output=%s" % logpath
+                    slurm_command += ' --wrap="%s"' % run_command
+                    result = subprocess.run(slurm_command, capture_output=True, shell=True)
+                    if result.returncode != 0:
+                        raise RuntimeError(
+                            "Slurm sbatch command resulted in non-zero return code. \nstdout:\n%r\nstderr:\n%r\n"
+                            % (result.stdout, result.stderr)
+                        )
+
+                while scenarios_running > 0:
+                    scenario_event: ScenarioEvent = study_queue.get()
+                    if scenario_event.type == ScenarioEvent.Type.COMPLETED:
+                        scenarios_running -= 1
+                        if pbar is not None:
+                            pbar.update(1)
 
                 scenarios = Study.load_scenarios(self.path)
 
             self._scenarios = scenarios
 
             if pbar is not None:
                 pbar.close()
@@ -1401,14 +979,15 @@
         replacements = dict((name, get_property_value(scenario, name)) for name in attributes)
         exppath = self._scenario_path_format.format_map(replacements)
         full_exppath = os.path.join(self.path, "scenarios", exppath)
         scenario.save(full_exppath)
         return full_exppath
 
     def save(self, save_scenarios: bool = True) -> None:
+
         # Make directory that will contain the study.
         os.makedirs(self.path, exist_ok=True)
 
         # Write a marker file.
         markerpath = os.path.join(self.path, "study.yml")
         with open(markerpath, "w") as f:
             yaml.safe_dump({"id": self.id, "scenario_path_format": self.scenario_path_format}, f)
@@ -1416,18 +995,33 @@
         # Write a log file.
         logpath = os.path.join(self.path, "study.log")
         with open(logpath, "w") as f:
             self._logstream.seek(0)
             copyfileobj(self._logstream, f)
             self._logstream.seek(0, SEEK_END)
 
-        # Save all scenarios.
+        # Verify that the provided scenario path is unique enough.
+        # self._verify_scenario_path(self._scenario_path_format, self.scenarios)
+
+        # Iterate over all scenarios and compute their target paths.
+        # attributes = re.findall(r"\{(.*?)\}", scenario_path)
+        # scenario_paths: Set[str] = set()
         if save_scenarios:
             for scenario in self.scenarios:
                 self.save_scenario(scenario)
+                # replacements = dict((name, get_property_value(scenario, name)) for name in attributes)
+                # exppath = scenario_path.format_map(replacements)
+                # if exppath in scenario_paths:
+                #     raise ValueError(
+                #         "Provided scenario_path does not produce unique paths. The path '%s' caused a conflict."
+                #         % exppath
+                #     )
+                # scenario_paths.add(exppath)
+                # full_exppath = os.path.join(self.path, "scenarios", exppath)
+                # scenario.save(full_exppath)
 
     @classmethod
     def load_scenarios(cls, path: str) -> List[Scenario]:
         # Load all scenarios.
         scenarios: List[Scenario] = []
         for attpath in glob(os.path.join(path, "**/attributes.yaml"), recursive=True):
             exppath = os.path.dirname(attpath)
@@ -1507,183 +1101,172 @@
 
     @property
     def completed(self) -> bool:
         return all(exp.completed for exp in self.scenarios if isinstance(exp, Scenario))
 
     @property
     def scenarios(self) -> Table[Scenario]:
-        attributes = sorted(Scenario._get_attribute_descriptors(flattened=True, include_subclasses=True).keys())
+        attributes = list(Scenario.attribute_domains.keys())
         return Table[Scenario](self._scenarios, attributes, "id")
 
-    def get_keyword_replacements(self) -> Dict[str, str]:
-        scenario_types: Set[Type[Scenario]] = set([type(scenario) for scenario in self.scenarios])
-        result: Dict[str, str] = {}
-        for scenario_type in scenario_types:
-            result.update(scenario_type.get_keyword_replacements())
-        return result
-
     @property
     def dataframe(self) -> DataFrame:
-        df = pd.concat(
-            [s.dataframe.assign(scenario=s.get_class_identifier(), id=s.id) for s in self.scenarios], ignore_index=True
-        )
+        df = pd.concat([scenario.dataframe for scenario in self.scenarios], ignore_index=True)
         df.sort_index(inplace=True)
         return df
 
     def get_scenarios(self, **attributes: Dict[str, Any]) -> Sequence[Scenario]:
         res: List[Scenario] = []
         for exp in self.scenarios:
             if all(has_attribute_value(exp, name, value) for (name, value) in attributes.items() if hasattr(exp, name)):
                 res.append(exp)
         return res
 
-    @classmethod
-    def union(
-        cls: Type["Study"],
-        *studies: "Study",
-        id: Optional[str] = None,
-        outpath: str = DEFAULT_RESULTS_PATH,
-        scenario_path_format: str = DEFAULT_SCENARIO_PATH_FORMAT,
-        logstream: Optional[TextIOBase] = None,
-    ) -> "Study":
-        scenarios: List[Scenario] = []
-        for study in studies:
-            scenarios.extend(study.scenarios)
-        return Study(scenarios, id=id, outpath=outpath, scenario_path_format=scenario_path_format, logstream=logstream)
 
-    def __add__(self, other: "Study") -> "Study":
-        return Study.union(self, other)
+def represent(x: Any):
+    if isinstance(x, Enum):
+        return repr(x.value)
+    else:
+        return repr(x)
+
+
+def stringify(x: Any):
+    if isinstance(x, Enum):
+        return str(x.value)
+    else:
+        return str(x)
 
-    def __radd__(self, other: "Study") -> "Study":
-        return Study.union(other, self)
 
+class Report(ABC):
 
-class Report(Configurable):
+    reports: Dict[str, Type["Report"]] = {}
+    report_domains: Dict[str, Dict[str, Set[Any]]] = {}
+    attribute_domains: Dict[str, Set[Any]] = {}
+    attribute_helpstrings: Dict[str, Optional[str]] = {}
+    attribute_types: Dict[str, Optional[type]] = {}
+    attribute_defaults: Dict[str, Optional[Any]] = {}
+    attribute_isiterable: Dict[str, bool] = {}
+    _report: Optional[str] = None
 
     def __init__(
-        self,
-        dataframe: DataFrame,
-        id: Optional[str] = None,
-        study: Optional[Study] = None,
-        partvals: Optional[Dict[str, Any]] = None,
-        keyword_replacements: Optional[Dict[str, str]] = None,
-        **kwargs: Any,
+        self, study: Study, id: Optional[str] = None, groupby: Optional[Dict[str, Any]] = None, **kwargs: Any
     ) -> None:
         super().__init__()
-        self._dataframe = dataframe
-        self._id = id if id is not None else "".join(random.choices(string.ascii_lowercase + string.digits, k=10))
         self._study = study
-        self._partvals: Dict[str, Any] = {} if partvals is None else partvals
-        self._keyword_replacements: Dict[str, str] = {} if keyword_replacements is None else keyword_replacements
+        self._id = id if id is not None else "".join(random.choices(string.ascii_lowercase + string.digits, k=10))
+        self._groupby: Dict[str, Any] = {} if groupby is None else groupby
+
+    def __init_subclass__(cls: Type["Report"], id: str) -> None:
+        cls._report = id
+        cls.reports[id] = cls
+
+        # Extract domain of scenario.
+        props = attribute.get_properties(cls)
+        domain = dict((name, set(get_property_domain(cls, name))) for name in props.keys())
+        Report.report_domains[id] = domain
+
+        # Include the new domain into the total domain.
+        for name, values in domain.items():
+            Report.attribute_domains.setdefault(name, set()).update(values)
+
+        # Extract types of the scenario attributes.
+        types = dict((name, get_property_type(cls, name)) for name in props.keys())
+        Report.attribute_types.update(types)
+
+        # Extract helpstrings of the scenario attributes.
+        helpstrings = dict((name, get_property_helpstring(cls, name)) for name in props.keys())
+        Report.attribute_helpstrings.update(helpstrings)
+
+        # Extract types of the scenario attributes.
+        defaults = dict((name, get_property_default(cls, name)) for name in props.keys())
+        Report.attribute_defaults.update(defaults)
+
+        # Specify if attributes should be iterable when passed to get_instances.
+        Report.attribute_isiterable = dict((name, get_property_isiterable(cls, name)) for name in props.keys())
+        Report.attribute_isiterable["report"] = True  # We hard code that we allow multiple report argument values.
+
+    @attribute
+    def report(self) -> str:
+        if self._report is None:
+            raise ValueError("Cannot call this on an abstract class instance.")
+        return self._report
 
     @attribute
     def id(self) -> str:
         """A unique identifier of the report."""
         return self._id
 
     @property
-    def partvals(self) -> Dict[str, Any]:
-        return self._partvals
+    def groupby(self) -> Dict[str, Any]:
+        return self._groupby
 
     @property
-    def study(self) -> Optional[Study]:
+    def study(self) -> Study:
         return self._study
 
-    @property
-    def dataframe(self) -> DataFrame:
-        return self._dataframe
-
-    @property
-    def keyword_replacements(self) -> Dict[str, str]:
-        return self._keyword_replacements
-
     @classmethod
     def is_valid_config(cls, **attributes: Any) -> bool:
         return True
 
     @abstractmethod
     def generate(self) -> None:
         raise NotImplementedError()
 
     def save(
         self,
         path: Optional[str] = None,
-        use_partvals: bool = True,
+        use_groupby: bool = True,
         use_id: bool = False,
         use_subdirs: bool = False,
         saveonly: Optional[Sequence[str]] = None,
     ) -> None:
         if path is None:
-            if self._study is not None:
-                path = os.path.join(self._study.path, "reports")
-            else:
-                path = os.path.join(DEFAULT_REPORTS_PATH, self._id)
+            path = os.path.join(self._study.path, "reports")
         basename = "report"
         if use_subdirs:
-            if use_partvals:
-                partvals = ["%s=%s" % (str(key), str(self._partvals[key])) for key in sorted(self.partvals.keys())]
-                path = os.path.join(path, *partvals)
+            if use_groupby:
+                groupby = ["%s=%s" % (str(key), str(self._groupby[key])) for key in sorted(self.groupby.keys())]
+                path = os.path.join(path, *groupby)
             if use_id:
                 path = os.path.join(path, self._id)
             if os.path.splitext(path)[1] != "":
                 raise ValueError("The provided path '%s' is not a valid directory path." % path)
         else:
-            if use_partvals:
-                partvals = [self._partvals[key] for key in sorted(self.partvals.keys())]
+            if use_groupby:
+                groupby = [self._groupby[key] for key in sorted(self.groupby.keys())]
                 basename = "_".join(
                     [basename]
-                    + ["%s=%s" % (str(key), stringify(self._partvals[key])) for key in sorted(self.partvals.keys())]
+                    + ["%s=%s" % (str(key), stringify(self._groupby[key])) for key in sorted(self.groupby.keys())]
                 )
             if use_id:
                 basename = basename + "_id=" + self._id
 
         os.makedirs(path, exist_ok=True)
 
         # Save results as separate files.
         props = result.get_properties(type(self))
         results = dict((name, prop.fget(self) if prop.fget is not None else None) for (name, prop) in props.items())
         save_dict(results, path, basename, saveonly=saveonly)
 
     @classmethod
     def get_instances(
-        cls: Type["Report"],
-        study: Study,
-        partby: Optional[Sequence[str]],
-        keyword_replacements: Optional[Dict[str, str]] = None,
-        **kwargs: Any,
+        cls: Type["Report"], study: Study, groupby: Optional[Sequence[str]], **kwargs: Any
     ) -> Iterable["Report"]:
-        keyword_replacements = {} if keyword_replacements is None else keyword_replacements
-        keyword_replacements = {
-            **keyword_replacements,
-            **study.get_keyword_replacements(),
-        }
-
         if cls == Report:
-            for id, report_class in Report.get_subclasses().items():
+            for id, report in Report.reports.items():
                 if kwargs.get("report", None) is None or id in kwargs["report"]:
-                    for instance in report_class.get_instances(
-                        study=study, partby=partby, keyword_replacements=keyword_replacements, **kwargs
-                    ):
+                    for instance in report.get_instances(study=study, groupby=groupby, **kwargs):
                         yield instance
         else:
             # If grouping attributes were not specified, then we return only a single instance.
-            if partby is None or len(partby) == 0:
-                yield cls(study=study, dataframe=study.dataframe, **kwargs)
+            if groupby is None or len(groupby) == 0:
+                yield cls(study=study, **kwargs)
 
             else:
                 # Find distinct grouping attribute assignments.
                 all_values: List[Tuple] = []
-                partitioned = study.dataframe.groupby(partby)  # type: ignore
                 if len(study.scenarios) > 0:
-                    all_values = list(partitioned.groups.keys())
+                    all_values = list(study.dataframe.groupby(groupby).groups.keys())
 
                 for values in all_values:
-                    dataframe = partitioned.get_group(values)
-                    partvals = dict((k, v) for (k, v) in zip(partby, values))
-
-                    yield cls(
-                        study=study,
-                        dataframe=dataframe,
-                        partvals=partvals,
-                        keyword_replacements=keyword_replacements,
-                        **kwargs,
-                    )
+                    groupby_values = dict((k, v) for (k, v) in zip(groupby, values))
+                    yield cls(study=study, groupby=groupby_values, **kwargs)
```

### Comparing `datascope-experiments-0.0.85/datascope/experiments/reports/aggregate_plot.py` & `datascope-experiments-0.0.9/datascope/experiments/reports/aggregate_plot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import re
 
 from enum import Enum
 from functools import partial
-from itertools import combinations, product
 from matplotlib.figure import Figure
 from matplotlib.ticker import EngFormatter, PercentFormatter
-from matplotlib.transforms import Bbox
-from numpy.typing import NDArray
-from scipy.sparse import lil_matrix
-from scipy.sparse.csgraph import connected_components
 from typing import Callable, Optional, Dict, Any, List, Union, TypeVar, Tuple
 
-from pandas import DataFrame, MultiIndex
-from pandas.core.groupby.generic import DataFrameGroupBy
+from pandas import DataFrame
 from pandas.core.groupby.groupby import GroupBy
 
-from ..bench import Report, Study, result, attribute
+from ..scenarios import Report, Study, result, attribute
 
 COLOR_NAMES = ["blue", "red", "yellow", "green", "purple", "brown", "cyan", "pink"]
-COLORS = ["#2BBFD9", "#DF362A", "#FAC802", "#8AB365", "#C670D2", "#AE7E1E", "#008F6B", "#6839CC"]
+COLORS = ["#2BBFD9", "#DF362A", "#FAC802", "#8AB365", "#C670D2", "#C58F21", "#00AC9B", "#DB006A"]
 LABELS = {
     "random": "Random",
     "shapley-tmc": "Shapley TMC",
     "shapley-knn-single": "Shapley KNN Single",
     "shapley-knn-interactive": "Shapley KNN Interactive",
     "shapley-tmc-10": "Shapley TMC x10",
     "shapley-tmc-50": "Shapley TMC x50",
@@ -55,61 +49,46 @@
 class AggregationMode(str, Enum):
     MEDIAN_PERC_90 = "median-perc-90"
     MEDIAN_PERC_95 = "median-perc-95"
     MEDIAN_PERC_99 = "median-perc-99"
     MEAN_STD = "mean-std"
 
 
-VALUE_MEASURES: Dict[AggregationMode, Dict[str, Union[Callable, str]]] = {
+VALUE_MEASURES: Dict[AggregationMode, Dict[str, Callable]] = {
     AggregationMode.MEAN_STD: {
-        "mean": "mean",
-        "std": "std",
+        "mean": np.mean,
+        "std": np.std,
         "std-l": lambda x: np.mean(x) - np.std(x),
         "std-h": lambda x: np.mean(x) + np.std(x),
     },
     AggregationMode.MEDIAN_PERC_90: {
-        "median": "median",
+        "median": np.median,
         "95perc-l": partial(np.percentile, q=5),
         "95perc-h": partial(np.percentile, q=95),
     },
     AggregationMode.MEDIAN_PERC_95: {
-        "median": "median",
+        "median": np.median,
         "95perc-l": partial(np.percentile, q=2.5),
         "95perc-h": partial(np.percentile, q=97.5),
     },
     AggregationMode.MEDIAN_PERC_99: {
-        "median": "median",
+        "median": np.median,
         "95perc-l": partial(np.percentile, q=0.5),
         "95perc-h": partial(np.percentile, q=99.5),
     },
 }
 
 VALUE_MEASURE_C: Dict[AggregationMode, str] = {
     AggregationMode.MEAN_STD: "mean",
     AggregationMode.MEDIAN_PERC_90: "median",
     AggregationMode.MEDIAN_PERC_95: "median",
     AggregationMode.MEDIAN_PERC_99: "median",
 }
 
 
-class CrossAggregationMode(str, Enum):
-    MEAN_SQUARE_ERROR = "mse"
-    ROOT_MEAN_SQUARE_ERROR = "rmse"
-    MEAN_ABSOLUTE_ERROR = "mae"
-    MEAN_ABSOLUTE_PERCENTAGE_ERROR = "mape"
-
-
-CROSS_AGGREGATION_FUNCTIONS: Dict[CrossAggregationMode, Callable[[NDArray, NDArray], float]] = {
-    CrossAggregationMode.MEAN_SQUARE_ERROR: lambda x1, x2: np.square(x1 - x2).mean(),
-    CrossAggregationMode.ROOT_MEAN_SQUARE_ERROR: lambda x1, x2: np.sqrt(np.square(x1 - x2).mean()),
-    CrossAggregationMode.MEAN_ABSOLUTE_ERROR: lambda x1, x2: np.abs(x1 - x2).mean(),
-    CrossAggregationMode.MEAN_ABSOLUTE_PERCENTAGE_ERROR: lambda x1, x2: np.abs((x1 - x2) / (x1 + 1e-6)).mean(),
-}
-
-
 class SliceOp(str, Enum):
     COUNT = "count"
     FIRST = "first"
     LAST = "last"
     MAX = "max"
     MIN = "min"
     MEAN = "mean"
@@ -126,15 +105,14 @@
     SliceOp.MEAN: GroupBy.mean,
     SliceOp.STD: GroupBy.std,
     SliceOp.MEDIAN: GroupBy.median,
 }
 
 DEFAULT_LABEL_FORMAT = "{compare}"
 DEFAULT_FONTSIZE = 16
-DEFAULT_LINEWIDTH = 2.5
 
 
 def represent(x: Any):
     if isinstance(x, Enum):
         return repr(x.value)
     if isinstance(x, float):
         return "%.2f" % x
@@ -163,105 +141,47 @@
     aggmode: AggregationMode = AggregationMode.MEDIAN_PERC_95,
 ) -> DataFrame:
     if compare is None:
         compare = []
     value_measures = VALUE_MEASURES[aggmode]
 
     groupbycols = [index] + list(compare)
-    dataframe = dataframe[[index] + targetval + compare].dropna()
     values = [dataframe.groupby(groupbycols)[targetval].agg(f).add_suffix(":" + k) for (k, f) in value_measures.items()]
     dataframe = pd.concat(values, axis=1)
     dataframe.sort_index(inplace=True)
     if len(compare) > 0:
-        unstacked = dataframe.unstack()
-        dataframe = unstacked if isinstance(unstacked, DataFrame) else unstacked.to_frame()
-        assert isinstance(dataframe.columns, MultiIndex)
-        dataframe.columns = dataframe.columns.swaplevel().map(lambda x: tuple(str(xx) for xx in x)).map(">".join)
+        dataframe = dataframe.unstack()
+        dataframe.columns = dataframe.columns.swaplevel().map(">".join)
     return dataframe
 
 
 def summarize(
     dataframe: DataFrame,
     summarize: List[str],
     compare: Optional[List[str]] = None,
     summode: Optional[AggregationMode] = None,
 ) -> dict:
     if summode is None:
         summode = AggregationMode.MEAN_STD
     if compare is None:
         compare = []
     value_measures = VALUE_MEASURES[summode]
-    dataframe = dataframe[summarize + compare].dropna()
-    if len(compare) > 0:
-        summary_frames = [
-            dataframe.groupby(compare)[summarize].agg(f).add_suffix(":" + k) for (k, f) in value_measures.items()
-        ]
-        return pd.concat(summary_frames, axis=1).to_dict(orient="index")
-    else:
-        summary_series = [dataframe[summarize].agg(f).add_suffix(":" + k) for (k, f) in value_measures.items()]
-        return pd.concat(summary_series, axis=0).to_dict()
-
-
-def cross_aggregate(
-    dataframe: pd.DataFrame,
-    index: Optional[List[str]],
-    compare: List[str],
-    targetval: List[str],
-    crossaggover: List[str],
-    crossaggpairs: Optional[List[str]] = None,
-    crossaggmode: CrossAggregationMode = CrossAggregationMode.MEAN_ABSOLUTE_ERROR,
-):
-    # Pivot the table so that target values from different comparison values appear side by side.
-    index = [] if index is None else index
-    crossaggover = [x for x in crossaggover if x not in index]
-    assert index is not None
-    indexlen = len(index)
-    dataframe = dataframe.pivot(index=index + crossaggover, columns=compare, values=targetval)
-
-    # Produce a series of pairwise comparisons for each target value and then concatdaenate them into one dataframe.
-    method = CROSS_AGGREGATION_FUNCTIONS[crossaggmode]
-    correlation_parts = []
-    for val in targetval:
-        target: Union[DataFrame, DataFrameGroupBy] = dataframe[[val]]
-        if len(index) > 0:
-            assert isinstance(target, DataFrame)
-            target = target.groupby(index)
-        target = target.corr(method=method)  # type: ignore
-        target = target.stack(dropna=False, level=compare)  # type: ignore
-        target = target.droplevel(axis=0, level=1 if len(index) > 0 else 0)  # type: ignore
-        correlation_parts.append(target)
-    dataframe = pd.concat(correlation_parts, axis=1)
-
-    # Keep only a single instance of each pair.
-    if crossaggpairs is None or len(crossaggpairs) == 0:
-        comparevals = [sorted(dataframe[col].unique()) for col in compare]
-        crossaggpairs = [x[0] + x[1] for x in combinations(product(*comparevals), r=2)]
-    pairs = [tuple(x.replace("&", ",").split(",")) for x in crossaggpairs]
-    dataframe = dataframe[dataframe.index.map(lambda x: x[indexlen:] in pairs)]
-
-    # Move values from the index into regular columns.
-    n = len(compare)
-
-    def column_mapper(x: Tuple) -> Tuple:
-        result = tuple(x[:indexlen])
-        result += (",".join(str(x[i]) for i in range(-2 * n, -n)) + "&" + ",".join(str(x[i]) for i in range(-n, 0)),)
-        result += tuple([None for _ in range(2 * n - 1)])
-        return result
-
-    dataframe.index = dataframe.index.map(column_mapper)
-    dataframe.index = dataframe.index.droplevel(list(range(-2 * n + 1, 0)))
-    dataframe.index = dataframe.index.set_names(">".join(compare), level=-1 if len(index) > 0 else None)
-    dataframe = dataframe.reset_index()
-    return dataframe
+    groups = dataframe.groupby(compare) if len(compare) > 0 else dataframe
+    values = [groups[summarize].agg(f).add_suffix(":" + k) for (k, f) in value_measures.items()]
+    axis = 0 if len(compare) == 0 else 1
+    dataframe = pd.concat(values, axis=axis)
+    dataframe.sort_index(inplace=True)
+    return dataframe.to_dict(orient="index") if isinstance(dataframe, DataFrame) else dataframe.to_dict()
 
 
 def replace_keywords(source: str, keyword_replacements: Dict[str, str]) -> str:
-    for k, v in sorted(keyword_replacements.items(), key=lambda x: len(x[0]), reverse=True):
+    for k, v in sorted(keyword_replacements.items(), key=lambda x: len(x[1]), reverse=True):
         source = re.sub("(?<![a-zA-Z])%s(?![a-z-Z])" % k, v, source)
-    return source.replace("_", " ").title()
+        # source = source.replace(k, v)
+    return source
 
 
 def get_colors(keys: List[Tuple[str, ...]], colors: Optional[Dict[Tuple[str, ...], str]]) -> List[str]:
     available_default_colors = [
         COLORS[i]
         for i in range(len(COLORS))
         if colors is None or (COLORS[i] not in colors.values() and COLOR_NAMES[i] not in colors.values())
@@ -274,77 +194,14 @@
                 color = COLORS[COLOR_NAMES.index(color)]
             result_colors.append(color)
         else:
             result_colors.append(available_default_colors.pop(0))
     return result_colors
 
 
-def fix_text_positioning(texts: Union[List[plt.Text], List[plt.Annotation]], axes: plt.Axes) -> None:
-
-    # Get renderer from axes.
-    renderer = axes.figure.canvas.renderer  # type: ignore
-
-    # Extract bounding boxes of all text objects.
-    transforms = [text.get_transform() for text in texts]
-    bboxes = [text.get_window_extent(renderer) for text in texts]
-    # bboxes = [axes.transData.inverted().transform_bbox(bbox) for bbox in bboxes]
-    heights = np.array([bbox.y1 - bbox.y0 for bbox in bboxes])
-    vertical_positions = np.array([bbox.y0 for bbox in bboxes])
-
-    # # Draw a bounding rectangle of all objects using bboxes.
-    # for bbox in bboxes:
-    #     rect_bbox = axes.transData.inverted().transform_bbox(bbox)
-    #     axes.add_patch(
-    #         Rectangle(
-    #             (rect_bbox.xmin, rect_bbox.ymin),
-    #             rect_bbox.width,
-    #             rect_bbox.height,
-    #             fill=False,
-    #             edgecolor="red",
-    #             # transform=axes.transAxes,
-    #         )
-    #     )
-
-    # Find groups of texts that overlap.
-    overlaps = lil_matrix((len(bboxes), len(bboxes)), dtype=bool)
-    for i in range(len(bboxes)):
-        for j in range(i + 1, len(bboxes)):
-            if bboxes[i].overlaps(bboxes[j]):
-                overlaps[i, j] = True
-    n_components, labels = connected_components(csgraph=overlaps, directed=False, return_labels=True)
-    for i in range(n_components):
-        group = np.where(labels == i)[0]
-        if len(group) > 1:
-            # Reorder the group by vertical position.
-            group = group[np.argsort(vertical_positions[group])]
-
-            # Find the bounding box that covers the group and use it to adjust the position of the texts.
-            bbox = Bbox.union([bboxes[i] for i in group])
-            y_cur = (bbox.ymin + bbox.ymax) / 2 - np.sum(heights[group]) / 2 + heights[group[0]] / 2
-            for i in group:
-                text = texts[i]
-                _, y = transforms[i].inverted().transform((0, y_cur))
-                text.set_y(y)
-                y_cur += heights[i]
-
-    # Expand the axes to fit the new text positions.
-    bboxes = [text.get_window_extent(renderer) for text in texts]
-    bbox_union = Bbox.union(bboxes)
-    bbox_data_coords = axes.transData.inverted().transform_bbox(bbox_union)
-    # axes.update_datalim(bbox_union)
-    if bbox_data_coords.xmin < axes.get_xlim()[0]:
-        axes.set_xlim(xmin=bbox_data_coords.xmin)
-    if bbox_data_coords.xmax > axes.get_xlim()[1]:
-        axes.set_xlim(xmax=bbox_data_coords.xmax)
-    if bbox_data_coords.ymin < axes.get_ylim()[0]:
-        axes.set_ylim(ymin=bbox_data_coords.ymin)
-    if bbox_data_coords.ymax > axes.get_ylim()[1]:
-        axes.set_ylim(ymax=bbox_data_coords.ymax)
-
-
 def lineplot(
     dataframe: DataFrame,
     index: str,
     targetval: str,
     compare: Optional[List[str]] = None,
     compareorder: List[str] = [],
     colors: Optional[Dict[str, str]] = None,
@@ -353,15 +210,14 @@
     labelformat: Optional[str] = None,
     summary: Optional[dict] = None,
     keyword_replacements: Optional[Dict[str, str]] = None,
     axes: Optional[plt.Axes] = None,
     fontsize: int = DEFAULT_FONTSIZE,
     annotations: bool = False,
     dontcompare: Optional[str] = None,
-    linemarker: Optional[str] = None,
 ) -> Optional[Figure]:
     if compare is None:
         compare = []
     if labelformat is None:
         if len(compare) > 0:
             labelformat = "; ".join("%%(%s)s" % c for c in compare)
         else:
@@ -380,129 +236,79 @@
     else:
         comparison = [(targetval,)]
         dataframe.columns = dataframe.columns.map(lambda x: (targetval,) + tuple(x.split(":")))
     compareorder_unpacked = [tuple(x.split(",")) for x in compareorder]
     if len(compareorder_unpacked) > 0:
         comparison = sorted(
             comparison,
-            key=lambda x: (
-                compareorder_unpacked.index(x)
-                if compareorder_unpacked is not None and x in compareorder_unpacked
-                else len(comparison)
-            ),
+            key=lambda x: compareorder_unpacked.index(x)
+            if compareorder_unpacked is not None and x in compareorder_unpacked
+            else len(comparison),
         )
 
     figure: Optional[Figure] = None
     if axes is None:
         figure = plt.figure(figsize=(10, 8))
-        subplots = figure.subplots()
-        assert isinstance(subplots, plt.Axes)
-        axes = subplots
-    else:
-        figure = axes.get_figure()
-    assert figure is not None
+        axes = figure.subplots()
 
     labels: List[str] = []
     for i, comp in enumerate(comparison):
+        if ",".join(str(c) for c in comp) in dontcompare:
+            continue
         formatdict = dict(zip(compare, comp))
         if summary is not None:
             comp_summary = summary
             for c in comp:
                 comp_summary = comp_summary.get(c, comp_summary)
             formatdict.update(comp_summary)
         label = labelformat % formatdict
         label = replace_keywords(label, keyword_replacements)
         labels.append(label)
 
     centercol = VALUE_MEASURE_C[aggmode]
     split_colors = dict((tuple(k.split(",")), v) for (k, v) in colors.items()) if colors is not None else None
     comp_colors = get_colors(comparison, colors=split_colors)
-    texts = []
-    ymin, ymax = np.inf, -np.inf
     for i, comp in enumerate(comparison):
         if ",".join(str(c) for c in comp) in dontcompare:
             continue
         cols: List[str] = dataframe[comp][targetval].columns.to_list()
         uppercol = next(c for c in cols if c.endswith("-h"))
         lowercol = next(c for c in cols if c.endswith("-l"))
         upper = dataframe[comp][targetval][uppercol].to_numpy()
         lower = dataframe[comp][targetval][lowercol].to_numpy()
-        ymax, ymin = max(ymax, np.max(upper)), min(ymin, np.min(lower))
         if errdisplay == ErrorDisplay.SHADE:
             axes.fill_between(dataframe.index.values, upper, lower, color=comp_colors[i], alpha=0.2)
         elif errdisplay == ErrorDisplay.BAR:
             center = dataframe[comp][targetval][centercol]
             xval = dataframe.index.values
             yval = center.to_numpy()
             yerr = np.abs(np.stack([lower, upper]) - yval)
-            axes.errorbar(
-                xval,
-                yval,
-                yerr=yerr,
-                fmt="o",
-                linewidth=DEFAULT_LINEWIDTH,
-                capsize=6,
-                color=comp_colors[i],
-                label=labels[i],
-            )
+            axes.errorbar(xval, yval, yerr=yerr, fmt="o", linewidth=2, capsize=6, color=comp_colors[i], label=labels[i])
             if annotations:
                 for x, y in zip(xval, yval):
-                    text = axes.annotate(
+                    axes.annotate(
                         "%.2f" % y,
                         xy=(x, y),
                         xytext=(fontsize * 0.5, 0),
                         textcoords="offset points",
                         fontsize=fontsize,
                         horizontalalignment="left",
                         verticalalignment="center",
-                        # arrowprops=dict(arrowstyle="-", color=comp_colors[i]),
                     )
-                    texts.append(text)
-
-    linedesc = list(zip(comparison, comp_colors, labels))
-    for comp, c, l in linedesc:
-        if ",".join(str(c) for c in comp) in dontcompare:
-            continue
-        ll = l if errdisplay != ErrorDisplay.BAR else None
-        axes.plot(
-            dataframe[comp][targetval][centercol],
-            color=c,
-            label=ll,
-            marker=linemarker,
-            markersize=4 * DEFAULT_LINEWIDTH,
-            linewidth=DEFAULT_LINEWIDTH,
-        )
 
-    # Plot a dashed line over the current lines to improve visibility of overlapping lines.
-    for comp, c, l in reversed(linedesc):
+    for i, comp in enumerate(comparison):
         if ",".join(str(c) for c in comp) in dontcompare:
             continue
-        axes.plot(dataframe[comp][targetval][centercol], color=c, linestyle=(0, (3, 3)), linewidth=DEFAULT_LINEWIDTH)
+        axes.plot(dataframe[comp][targetval][centercol], color=comp_colors[i], label=labels[i])
 
     # axes.set_xlim([dataframe.index.values[0], (dataframe.index.values[-1] - dataframe.index.values[0]) * 1.2])
     # axes.set_ylim([-0.2, 1])
     axes.set_ylabel(replace_keywords(targetval, keyword_replacements), fontsize=fontsize, wrap=True)
     axes.set_xlabel(replace_keywords(index, keyword_replacements), fontsize=fontsize, wrap=True)
     # axes.legend(loc="lower right", fontsize=fontsize, borderaxespad=0, edgecolor="black", fancybox=False)
-
-    axes.relim()
-
-    if len(texts) > 0:
-        figure.canvas.draw()
-        fix_text_positioning(texts, axes)
-
-    axes.autoscale_view(tight=True)
-
-    # Readjust the y-axis limits to include the error bars.
-    ymin = min(ymin - 0.1 * (ymax - ymin), axes.get_ylim()[0])
-    ymax = max(ymax + 0.1 * (ymax - ymin), axes.get_ylim()[1])
-    axes.set_ylim(ymin, ymax)
-
-    figure.canvas.draw()
-
     return figure
 
 
 T = TypeVar("T")
 
 
 def dictpivot(d: Dict, compare: List[str], prefix: Tuple[str, ...] = tuple()) -> Dict[Tuple[str, ...], Dict]:
@@ -553,106 +359,69 @@
     if keyword_replacements is None:
         keyword_replacements = {}
     if dontcompare is None:
         dontcompare = ""
     figure: Optional[Figure] = None
     if axes is None:
         figure = plt.figure(figsize=(10, 8))
-        subplots = figure.subplots()
-        assert isinstance(subplots, plt.Axes)
-        axes = subplots
-    else:
-        figure = axes.get_figure()
-    assert figure is not None
+        axes = figure.subplots()
 
     # x, y, yerr = [], [], []
     summary = dictpivot(summary, compare=compare)
     summary_items = list(summary.items())
 
+    comparison = [item[0] for item in summary_items]
+    split_colors = dict((tuple(k.split(",")), v) for (k, v) in colors.items()) if colors is not None else None
+    comp_colors = get_colors(comparison, colors=split_colors)
     compareorder_unpacked = [tuple(x.split(",")) for x in compareorder]
     if len(compareorder_unpacked) > 0:
         summary_items = sorted(
             summary_items,
-            key=lambda x: (
-                compareorder_unpacked.index(x[0])
-                if compareorder_unpacked is not None and x[0] in compareorder_unpacked
-                else len(summary_items)
-            ),
+            key=lambda x: compareorder_unpacked.index(x[0])
+            if compareorder_unpacked is not None and x[0] in compareorder_unpacked
+            else len(comparison),
         )
-
-    comparison = [item[0] for item in summary_items]
-    split_colors = dict((tuple(k.split(",")), v) for (k, v) in colors.items()) if colors is not None else None
-    comp_colors = get_colors(comparison, colors=split_colors)
-    texts = []
-    ymin, ymax = np.inf, -np.inf
-
     for i, (comp, values) in enumerate(summary_items):
         if ",".join(str(c) for c in comp) in dontcompare:
             continue
         centercol = VALUE_MEASURE_C[aggmode]
         formatdict = dict(zip(compare, comp))
         label = labelformat % formatdict
         label = replace_keywords(label, keyword_replacements)
-        # xval = "; ".join(str(x) for x in comp)
+        xval = "; ".join(str(x) for x in comp)
         col = targetval + ":" + centercol
         yval = values[col]
 
-        uppercol = next(c for c in values.keys() if c.startswith(targetval) and c.endswith("-h"))
-        lowercol = next(c for c in values.keys() if c.startswith(targetval) and c.endswith("-l"))
+        uppercol = next(c for c in values.keys() if c.endswith("-h"))
+        lowercol = next(c for c in values.keys() if c.endswith("-l"))
         yerr = np.abs(np.array([[values[col] - values[lowercol]], [values[col] - values[uppercol]]]))
-        ymax, ymin = max(ymax, np.max(yerr)), min(ymin, np.min(yerr))
-        axes.errorbar(
-            [i],
-            [yval],
-            yerr=yerr,
-            fmt="o",
-            linewidth=DEFAULT_LINEWIDTH,
-            capsize=6,
-            color=comp_colors[i],
-            label=label,
-        )
+        axes.errorbar([xval], [yval], yerr=yerr, fmt="o", linewidth=2, capsize=6, color=comp_colors[i], label=label)
 
         if annotations:
-            text = axes.annotate(
+            axes.annotate(
                 "%.2f" % yval,
-                xy=(i, yval),
+                xy=(xval, yval),
                 xytext=(fontsize * 0.5, 0),
                 textcoords="offset points",
                 fontsize=fontsize,
                 horizontalalignment="left",
                 verticalalignment="center",
             )
-            texts.append(text)
 
     axes.set_ylabel(replace_keywords(targetval, keyword_replacements), fontsize=fontsize, wrap=True)
     axes.get_xaxis().set_ticks([])
-    axes.relim()
 
     # Squeeze xlimit.
     xlim = axes.get_xlim()
     xlim_delta = xlim[1] - xlim[0]
     axes.set_xlim((xlim[0] - xlim_delta * 0.1, xlim[1] + xlim_delta * 0.3))
     # axes.legend(
     #     loc="upper right", fontsize=fontsize, borderaxespad=0, edgecolor="black", fancybox=False, ncol=len(summary)
     # )
 
-    axes.relim()
-
-    if len(texts) > 0:
-        figure.canvas.draw()
-        fix_text_positioning(texts, axes)
-
-    axes.autoscale_view(tight=True)
-    figure.canvas.draw()
-
-    # Readjust the y-axis limits to include the error bars.
-    ymin = min(ymin - 0.1 * (ymax - ymin), axes.get_ylim()[0])
-    ymax = max(ymax + 0.1 * (ymax - ymin), axes.get_ylim()[1])
-    axes.set_ylim(ymin, ymax)
-
     return figure
 
 
 def dotplot(
     summary: dict,
     xtargetval: str,
     ytargetval: str,
@@ -681,113 +450,99 @@
     if keyword_replacements is None:
         keyword_replacements = {}
     if dontcompare is None:
         dontcompare = ""
     figure: Optional[Figure] = None
     if axes is None:
         figure = plt.figure(figsize=(10, 8))
-        subplots = figure.subplots()
-        assert isinstance(subplots, plt.Axes)
-        axes = subplots
-    else:
-        figure = axes.get_figure()
-    assert figure is not None
+        axes = figure.subplots()
 
     # x, y, yerr = [], [], []
     summary = dictpivot(summary, compare=compare)
     summary_items = list(summary.items())
 
+    comparison = [item[0] for item in summary_items]
+    split_colors = dict((tuple(k.split(",")), v) for (k, v) in colors.items()) if colors is not None else None
+    comp_colors = get_colors(comparison, colors=split_colors)
     compareorder_unpacked = [tuple(x.split(",")) for x in compareorder]
     if len(compareorder_unpacked) > 0:
         summary_items = sorted(
             summary_items,
-            key=lambda x: (
-                compareorder_unpacked.index(x[0])
-                if compareorder_unpacked is not None and x[0] in compareorder_unpacked
-                else len(summary_items)
-            ),
+            key=lambda x: compareorder_unpacked.index(x[0])
+            if compareorder_unpacked is not None and x[0] in compareorder_unpacked
+            else len(comparison),
         )
-
-    comparison = [item[0] for item in summary_items]
-    split_colors = dict((tuple(k.split(",")), v) for (k, v) in colors.items()) if colors is not None else None
-    comp_colors = get_colors(comparison, colors=split_colors)
-    texts = []
-
     for i, (comp, values) in enumerate(summary_items):
         if ",".join(str(c) for c in comp) in dontcompare:
             continue
         centercol = VALUE_MEASURE_C[aggmode]
         formatdict = dict(zip(compare, comp))
         label = labelformat % formatdict
         label = replace_keywords(label, keyword_replacements)
-        # xval = "; ".join(str(x) for x in comp)
+        xval = "; ".join(str(x) for x in comp)
         xcol = xtargetval + ":" + centercol
         xval = values[xcol]
         ycol = ytargetval + ":" + centercol
         yval = values[ycol]
 
         xuppercol = next(c for c in values.keys() if c.startswith(xtargetval) and c.endswith("-h"))
         xlowercol = next(c for c in values.keys() if c.startswith(xtargetval) and c.endswith("-l"))
         xerr = np.abs(np.array([[values[xcol] - values[xlowercol]], [values[xcol] - values[xuppercol]]]))
 
         yuppercol = next(c for c in values.keys() if c.startswith(ytargetval) and c.endswith("-h"))
         ylowercol = next(c for c in values.keys() if c.startswith(ytargetval) and c.endswith("-l"))
         yerr = np.abs(np.array([[values[ycol] - values[ylowercol]], [values[ycol] - values[yuppercol]]]))
         axes.errorbar(
-            [xval],
-            [yval],
-            xerr=xerr,
-            yerr=yerr,
-            fmt="o",
-            linewidth=DEFAULT_LINEWIDTH,
-            capsize=6,
-            color=comp_colors[i],
-            label=label,
+            [xval], [yval], xerr=xerr, yerr=yerr, fmt="o", linewidth=2, capsize=6, color=comp_colors[i], label=label
         )
 
         if annotations:
-            text = axes.annotate(
+            axes.annotate(
                 "%.2f" % yval,
                 xy=(xval, yval),
                 xytext=(fontsize * 0.5, 0),
                 textcoords="offset points",
                 fontsize=fontsize,
                 horizontalalignment="left",
                 verticalalignment="center",
             )
-            texts.append(text)
 
     axes.set_ylabel(replace_keywords(ytargetval, keyword_replacements), fontsize=fontsize, wrap=True)
     axes.set_xlabel(replace_keywords(xtargetval, keyword_replacements), fontsize=fontsize, wrap=True)
-    axes.relim()
 
     # Squeeze xlimit.
     # xlim = axes.get_xlim()
     # xlim_delta = xlim[1] - xlim[0]
     # axes.set_xlim((xlim[0] - xlim_delta * 0.1, xlim[1] + xlim_delta * 0.3))
     # axes.legend(
     #     loc="upper right", fontsize=fontsize, borderaxespad=0, edgecolor="black", fancybox=False, ncol=len(summary)
     # )
 
-    axes.relim()
-
-    if len(texts) > 0:
-        figure.canvas.draw()
-        fix_text_positioning(texts, axes)
-
-    axes.autoscale_view(tight=True)
-    figure.canvas.draw()
-
     return figure
 
 
 NONE_SYMBOL = "-"
 DEFAULT_PLOTSIZE = [10, 8]
 
 
+# def ensurelist(
+#     x: Optional[Union[List[T], T]],
+#     default: Optional[T] = None,
+#     length: Optional[int] = None,
+# ) -> List[T]:
+#     result = [default] if x is None else x if isinstance(x, list) else [x]
+#     if length is not None and len(result) != length:
+#         if len(result) > 1:
+#             raise ValueError("Expected length to be %d but encountered %d." % (length, len(result)))
+#         else:
+#             result = [result[0] for _ in range(length)]
+#     return result
+#     # return [x if x != NONE_SYMBOL else None for x in result]
+
+
 def ensurelist(
     x: Optional[Union[List[T], T]],
     default: Optional[T] = None,
     length: Optional[int] = None,
 ) -> List[T]:
     result: List[T] = ([default] if default is not None else []) if x is None else x if isinstance(x, list) else [x]
     if length is not None and len(result) != length:
@@ -809,90 +564,76 @@
     return spec
 
 
 def unpackdict(target: Dict[str, Union[Dict, Any]], prefix: str = "") -> Dict[str, Any]:
     result: Dict[str, Any] = {}
     for k, v in target.items():
         if isinstance(v, dict):
-            for kk, vv in unpackdict(v, prefix=str(k)).items():
+            for kk, vv in unpackdict(v, prefix=k).items():
                 key = ".".join(([] if prefix == "" else [prefix]) + [kk])
                 result[key] = vv
         else:
             key = ".".join(([] if prefix == "" else [prefix]) + [k])
             result[key] = v
     return result
 
 
 class AggregatePlot(Report, id="aggplot"):
     def __init__(
         self,
-        dataframe: DataFrame,
-        partvals: Optional[Dict[str, Any]] = None,
-        id: Optional[str] = None,
-        study: Optional[Study] = None,
-        keyword_replacements: Optional[Dict[str, str]] = None,
+        study: Study,
         plot: Optional[Union[List[str], str]] = None,
         index: Optional[str] = None,
         targetval: Optional[Union[List[str], str]] = None,
         compare: Optional[Union[List[str], str]] = None,
         compareorder: Optional[List[str]] = None,
         colors: Optional[List[str]] = None,
         summarize: Optional[Union[List[str], str]] = None,
-        crossaggover: Optional[Union[List[str], str]] = None,
         sliceby: Optional[Union[List[str], str]] = None,
         sliceop: Optional[SliceOp] = None,
         resultfilter: Optional[str] = None,
         errdisplay: Optional[ErrorDisplay] = None,
         aggmode: Optional[AggregationMode] = None,
         summode: Optional[AggregationMode] = None,
-        crossaggmode: Optional[CrossAggregationMode] = None,
         xlogscale: Optional[Union[List[bool], bool]] = None,
         ylogscale: Optional[Union[List[bool], bool]] = None,
         xtickfmt: Optional[Union[List[TickFormat], TickFormat]] = None,
         ytickfmt: Optional[Union[List[TickFormat], TickFormat]] = None,
-        linemarker: Optional[Union[List[str], str]] = None,
         annotations: Optional[Union[List[bool], bool]] = None,
         dontcompare: Optional[Union[List[str], str]] = None,
+        groupby: Optional[Dict[str, Any]] = None,
         labelformat: Optional[str] = None,
         plotsize: Optional[List[int]] = None,
         fontsize: Optional[int] = None,
         usetex: Optional[bool] = True,
         legend: Optional[bool] = True,
         titleformat: Optional[List[str]] = None,
+        id: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
-        super().__init__(
-            dataframe=dataframe,
-            id=id,
-            study=study,
-            partvals=partvals,
-            keyword_replacements=keyword_replacements,
-            **kwargs,
-        )
+        super().__init__(study, id=id, groupby=groupby, **kwargs)
         self._plot = ensurelist(plot, default=None)
         n_plots = len(self._plot)
         self._index = index
         self._targetval: List[str] = ensurelist(targetval, default=None)
         self._compare: List[str] = ensurelist(compare, default=None)
         self._compareorder: List[str] = compareorder if compareorder is not None else []
         self._colors: List[str] = colors if colors is not None else []
         self._summarize: List[str] = ensurelist(summarize, default=None)
-        self._crossaggover: List[str] = ensurelist(crossaggover, default=None)
+        self._filter = filter
         self._sliceby: List[str] = ensurelist(sliceby, default=None)
         self._sliceop = sliceop if sliceop is not None else SliceOp.FIRST
         self._resultfilter: Optional[str] = resultfilter
         self._errdisplay = errdisplay if errdisplay is not None else ErrorDisplay.SHADE
         self._aggmode = aggmode if aggmode is not None else AggregationMode.MEDIAN_PERC_95
         self._summode = summode if summode is not None else AggregationMode.MEDIAN_PERC_95
-        self._crossaggmode = crossaggmode if crossaggmode is not None else CrossAggregationMode.MEAN_ABSOLUTE_ERROR
         self._xlogscale: List[bool] = ensurelist(xlogscale, default=False, length=n_plots)
         self._ylogscale: List[bool] = ensurelist(ylogscale, default=False, length=n_plots)
         self._xtickfmt: List[TickFormat] = ensurelist(xtickfmt, default=TickFormat.DEFAULT, length=n_plots)
         self._ytickfmt: List[TickFormat] = ensurelist(ytickfmt, default=TickFormat.DEFAULT, length=n_plots)
-        self._linemarker: List[str] = ensurelist(linemarker, default="", length=n_plots)
         self._annotations: List[bool] = ensurelist(annotations, default=False, length=n_plots)
         self._dontcompare: List[str] = ensurelist(dontcompare, default=NONE_SYMBOL, length=n_plots)
 
         self._labelformat = (
             labelformat
             if labelformat is not None
             else (
@@ -905,15 +646,15 @@
         self._plotsize = plotsize if plotsize is not None else DEFAULT_PLOTSIZE
         if len(self._plotsize) != 2:
             raise ValueError("The plotsize must have two parameters: width and height.")
         self._fontsize = fontsize if fontsize is not None else DEFAULT_FONTSIZE
         self._usetex = usetex if usetex is not None else True
         self._legend = legend if legend is not None else True
         if titleformat is None:
-            titleformat = ["; ".join("%s=%%(%s)s" % (str(k).title(), str(k)) for k in self._partvals.keys())]
+            titleformat = [" ".join("%s=%%(%s)s" % (str(k).title(), str(k)) for k in self._groupby.keys())]
         self._titleformat = titleformat
 
         self._view: Optional[DataFrame] = None
         self._figure: Optional[Figure] = None
         self._summary: Optional[dict] = None
 
     @attribute
@@ -948,19 +689,14 @@
 
     @attribute
     def summarize(self) -> List[str]:
         """The attribute aggregate over the entire dataframe."""
         return self._summarize
 
     @attribute
-    def crossaggover(self) -> List[str]:
-        """The attributes that we use for joining the cross aggregation."""
-        return self._crossaggover
-
-    @attribute
     def sliceby(self) -> List[str]:
         """Slice along the index attribute by taking the first value in each slice plane.
         We use the given set of attributes to define a slice plane."""
         return self._sliceby
 
     @attribute
     def sliceop(self) -> SliceOp:
@@ -979,19 +715,14 @@
 
     @attribute
     def summode(self) -> AggregationMode:
         """The mode of summarization to apply."""
         return self._summode
 
     @attribute
-    def crossaggmode(self) -> CrossAggregationMode:
-        """The mode of cross aggregation to apply."""
-        return self._crossaggmode
-
-    @attribute
     def errdisplay(self) -> ErrorDisplay:
         """The method of displaying error bars."""
         return self._errdisplay
 
     @attribute
     def xlogscale(self) -> List[bool]:
         """Whether to represent the x-axis in the logarithmic scale."""
@@ -1009,19 +740,14 @@
 
     @attribute
     def ytickfmt(self) -> List[TickFormat]:
         """The tick formatting to use for the y-axis."""
         return self._ytickfmt
 
     @attribute
-    def linemarker(self) -> List[str]:
-        """The type of marker to use when plotting lines."""
-        return self._linemarker
-
-    @attribute
     def annotations(self) -> List[bool]:
         """Whether to add annotations to all points displayed."""
         return self._annotations
 
     @attribute
     def dontcompare(self) -> List[str]:
         """Space-separated list of comma separated lists of values that should not be compared."""
@@ -1057,129 +783,77 @@
 
     @attribute
     def titleformat(self) -> List[str]:
         """The formatted text to use in the title."""
         return self._titleformat
 
     def generate(self) -> None:
-        dataframe = self.dataframe
-        if self.resultfilter is not None:
-            dataframe = dataframe.query(self.resultfilter)
+        dataframe = filter(self.study.dataframe, attributes=self.groupby, resultfilter=self.resultfilter)
 
-        keyword_replacements: Dict[str, str] = {**self.keyword_replacements}
+        keyword_replacements: Dict[str, str] = {}
         summarydict: Dict[str, str] = {}
-        if self.study is not None:
-            keyword_replacements.update(self.study.get_keyword_replacements())
+        for scenario in self.study.scenarios:
+            keyword_replacements.update(scenario.keyword_replacements)
 
         if self.index is not None and len(self.targetval) > 0:
             if self._view is None:
-                agg_dataframe = dataframe
-
-                # If slicing was specified, then we slice the dataframe first.
-                if len(self.sliceby) > 0:
-                    groupattrs = self.sliceby + self.compare + [self.index]
-                    groupby = agg_dataframe.groupby(groupattrs)
-                    sliceop = SLICE_OPS[self.sliceop]
-                    agg_dataframe = sliceop(groupby)
-                    agg_dataframe.reset_index(inplace=True)
-
-                if len(self._crossaggover) > 0:
-                    agg_dataframe = cross_aggregate(
-                        dataframe=dataframe,
-                        index=[self.index],
-                        compare=self.compare,
-                        targetval=self.targetval,
-                        crossaggover=self._crossaggover,
-                        crossaggpairs=self._compareorder,
-                        crossaggmode=self._crossaggmode,
-                    )
-
                 self._view = aggregate(
-                    dataframe=agg_dataframe,
+                    dataframe=dataframe,
                     compare=self.compare,
                     index=self.index,
                     targetval=self.targetval,
                     aggmode=self.aggmode,
                 )
 
         if len(self.summarize) > 0:
-            if self._summary is None:
-                summ_dataframe = dataframe
 
-                # If slicing was specified, then we slice the dataframe first.
-                if len(self.sliceby) > 0:
-                    groupattrs = self.sliceby + self.compare
-                    groupby = summ_dataframe.groupby(groupattrs)
-                    sliceop = SLICE_OPS[self.sliceop]
-                    summ_dataframe = sliceop(groupby)
-                    summ_dataframe.reset_index(inplace=True)
-
-                if len(self._crossaggover) > 0:
-                    summ_dataframe = cross_aggregate(
-                        dataframe=summ_dataframe,
-                        index=None,
-                        compare=self.compare,
-                        targetval=self.targetval,
-                        crossaggover=self._crossaggover,
-                        crossaggpairs=self._compareorder,
-                        crossaggmode=self._crossaggmode,
-                    )
+            # If slicing was specified, then we slice the dataframe first.
+            if len(self.sliceby) > 0:
+                groupattrs = self.sliceby + self.compare
+                groupby = dataframe.groupby(groupattrs)
+                sliceop = SLICE_OPS[self.sliceop]
+                dataframe = sliceop(groupby)
+                dataframe.reset_index()
 
+            if self._summary is None:
                 self._summary = summarize(
-                    dataframe=summ_dataframe,
+                    dataframe=dataframe,
                     summarize=self.summarize,
                     compare=self.compare,
                     summode=self.summode,
                 )
             summarydict = dict((k, represent(v)) for (k, v) in unpackdict(self._summary).items())
 
         if len(self.plot) > 0:
             figsize = (len(self.plot) * self.plotsize[0], self.plotsize[1])
             self._figure = plt.figure(figsize=figsize)
-            formatdict = dict(**self.partvals)
+            formatdict = dict(**self.groupby)
             formatdict.update(summarydict)
             title = "\n".join(self.titleformat) % formatdict
             title = replace_keywords(title, keyword_replacements)
             plt.rc("text", usetex=self.usetex)
-            if not title.isspace():
-                self._figure.suptitle(title, fontsize=self.fontsize * 0.9)
-            subplots = self._figure.subplots(nrows=1, ncols=len(self.plot))
-            assert isinstance(subplots, np.ndarray) or isinstance(subplots, plt.Axes)
-            axes: NDArray = np.array([subplots]) if isinstance(subplots, plt.Axes) else subplots.flatten()
+            self._figure.suptitle(title, fontsize=self.fontsize * 1.2)
+            axes: plt.Axes = self._figure.subplots(nrows=1, ncols=len(self.plot))
+            if len(self.plot) == 1:
+                axes = np.array([axes])
+            axes = axes.flatten()
             colors = dict((x.split(":")[0], x.split(":")[1]) for x in self._colors) if len(self._colors) > 0 else None
 
             for i, plotspec in enumerate(self.plot):
                 plottype, target = parseplotspec(plotspec)
 
                 # Axes style.
                 axes[i].spines["top"].set_visible(False)
                 axes[i].spines["right"].set_visible(False)
                 axes[i].tick_params(axis="both", which="major", labelsize=self.fontsize)
 
-                if self.xlogscale[i]:
-                    axes[i].set_xscale("log")
-                if self.ylogscale[i]:
-                    axes[i].set_yscale("log")
-
-                if self.xtickfmt[i] == TickFormat.PERCENT:
-                    axes[i].xaxis.set_major_formatter(PercentFormatter(xmax=1.0, decimals=0))
-                elif self.xtickfmt[i] == TickFormat.ENG:
-                    axes[i].xaxis.set_major_formatter(EngFormatter(places=0, sep=""))
-                if self.ytickfmt[i] == TickFormat.PERCENT:
-                    axes[i].yaxis.set_major_formatter(PercentFormatter(xmax=1.0, decimals=0))
-                elif self.ytickfmt[i] == TickFormat.ENG:
-                    axes[i].yaxis.set_major_formatter(EngFormatter(places=0, sep=""))
-
                 if plottype == PlotType.LINE:
+
                     if self._index is None:
                         raise ValueError("An index must be specified when plotting line plots.")
-                    if self._view is None:
-                        raise ValueError(
-                            "An aggregate view must be generated for a line plot by specifying a targetval and index."
-                        )
 
                     lineplot(
                         self._view,
                         index=self._index,
                         targetval=target[0],
                         summary=self._summary,
                         compare=self._compare,
@@ -1189,17 +863,17 @@
                         labelformat=self._labelformat,
                         aggmode=self._aggmode,
                         keyword_replacements=keyword_replacements,
                         axes=axes[i],
                         fontsize=self.fontsize,
                         annotations=self._annotations[i],
                         dontcompare=self._dontcompare[i],
-                        linemarker=self._linemarker[i],
                     )
                 elif plottype == PlotType.BAR:
+
                     if self._summary is None:
                         raise ValueError("A bar plot can only be generated from a summary.")
 
                     barplot(
                         summary=self._summary,
                         targetval=target[0],
                         compare=self.compare,
@@ -1211,14 +885,15 @@
                         axes=axes[i],
                         fontsize=self.fontsize,
                         annotations=self._annotations[i],
                         dontcompare=self._dontcompare[i],
                     )
 
                 else:
+
                     if self._summary is None:
                         raise ValueError("A dot plot can only be generated from a summary.")
 
                     if len(target) != 2:
                         raise ValueError(
                             "A dot plot must be specified with two targets. One for the x-axis and one for the y-axis."
                         )
@@ -1235,14 +910,28 @@
                         keyword_replacements=keyword_replacements,
                         axes=axes[i],
                         fontsize=self.fontsize,
                         annotations=self._annotations[i],
                         dontcompare=self._dontcompare[i],
                     )
 
+                if self.xlogscale[i]:
+                    axes[i].set_xscale("log")
+                if self.ylogscale[i]:
+                    axes[i].set_yscale("log")
+
+                if self.xtickfmt[i] == TickFormat.PERCENT:
+                    axes[i].xaxis.set_major_formatter(PercentFormatter(xmax=1.0))
+                elif self.xtickfmt[i] == TickFormat.ENG:
+                    axes[i].xaxis.set_major_formatter(EngFormatter(places=0, sep=""))
+                if self.ytickfmt[i] == TickFormat.PERCENT:
+                    axes[i].yaxis.set_major_formatter(PercentFormatter(xmax=1.0))
+                elif self.ytickfmt[i] == TickFormat.ENG:
+                    axes[i].yaxis.set_major_formatter(EngFormatter(places=0, sep=""))
+
             if self._legend:
                 self._figure.subplots_adjust(bottom=0.25)
                 lines, labels = self._figure.axes[0].get_legend_handles_labels()
                 self._figure.legend(
                     lines,
                     labels,
                     loc="upper center",
```

### Comparing `datascope-experiments-0.0.85/datascope/experiments/scenarios/compute_time.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/compute_time.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,114 @@
 import numpy as np
 
 from datascope.importance.common import SklearnModelAccuracy
 from datascope.importance.shapley import ShapleyImportance
 from datetime import timedelta
-from methodtools import lru_cache
 from pandas import DataFrame
 from time import process_time_ns
-from typing import Any, Optional, Dict, Type
+from typing import Any, Optional, Dict
 
-from ..bench import Scenario, attribute, result
+from .base import Scenario, attribute, result
 from .datascope_scenario import (
     RepairMethod,
     IMPORTANCE_METHODS,
     MC_ITERATIONS,
     DEFAULT_SEED,
     DEFAULT_MODEL,
     DEFAULT_MC_TIMEOUT,
     KEYWORD_REPLACEMENTS,
     UtilityType,
 )
-from ..datasets import Dataset, RandomDataset
-from ..pipelines import Pipeline, Model
+from ..datasets import Dataset, DEFAULT_TRAINSIZE, DEFAULT_VALSIZE, DEFAULT_NUMFEATURES
+from ..pipelines import Pipeline, ModelType, get_model
 
-DEFAULT_DATASET = RandomDataset()
+DEFAULT_DATASET = "random"
+KEYWORD_REPLACEMENTS = {
+    **KEYWORD_REPLACEMENTS,
+    **{"trainsize": "Training Set Size", "valsize": "Validation Set Size", "numfeatures": "Number of Features"},
+}
 
 
 class ComputeTimeScenario(Scenario, id="compute-time"):
     def __init__(
         self,
-        pipeline: Pipeline,
+        pipeline: str,
         method: RepairMethod,
-        dataset: Dataset = DEFAULT_DATASET,
-        model: Model = DEFAULT_MODEL,
+        iteration: int,
+        dataset: str = DEFAULT_DATASET,
+        model: ModelType = DEFAULT_MODEL,
         seed: int = DEFAULT_SEED,
+        trainsize: int = DEFAULT_TRAINSIZE,
+        valsize: int = DEFAULT_VALSIZE,
+        numfeatures: int = DEFAULT_NUMFEATURES,
         mc_timeout: int = DEFAULT_MC_TIMEOUT,
         importance_cputime: Optional[float] = None,
-        iteration: Optional[int] = None,  # Iteration became seed. Keeping this for back compatibility reasons.
         **kwargs: Any
     ) -> None:
         super().__init__(**kwargs)
         self._dataset = dataset
         self._pipeline = pipeline
         self._method = method
         self._iteration = iteration
         self._model = model
         self._seed = seed
-        if iteration is not None:
-            self._seed += iteration
+        self._trainsize = trainsize
+        self._valsize = valsize
+        self._numfeatures = numfeatures
         self._mc_timeout = mc_timeout
         self._importance_cputime: Optional[float] = importance_cputime
 
     @classmethod
     def is_valid_config(cls, **attributes: Any) -> bool:
         result = True
         if "utility" in attributes:
             result = attributes["utility"] == UtilityType.ACCURACY
         if "method" in attributes:
             result = result and not RepairMethod.is_tmc_nonpipe(attributes["method"])
         return result and super().is_valid_config(**attributes)
 
-    @attribute
-    def dataset(self) -> Dataset:
+    @attribute(domain=[DEFAULT_DATASET])
+    def dataset(self) -> str:
         """Dataset to use for training and validation."""
         return self._dataset
 
-    @attribute
-    def pipeline(self) -> Pipeline:
+    @attribute(domain=Pipeline.pipelines.keys())
+    def pipeline(self) -> str:
         """Pipeline to use for feature extraction."""
         return self._pipeline
 
     @attribute
     def method(self) -> RepairMethod:
         """Method used to perform data repairs."""
         return self._method
 
-    @attribute
-    def model(self) -> Model:
+    @attribute(domain=[None])
+    def model(self) -> ModelType:
         """Model used to make predictions."""
         return self._model
 
     @attribute(domain=range(10))
-    def seed(self) -> int:
-        """The random seed that applies to all pseudo-random processes in the scenario."""
-        return self._seed
+    def iteration(self) -> int:
+        """The ordinal number of the experiment repetition. Also serves as the random seed."""
+        return self._iteration
+
+    @attribute
+    def trainsize(self) -> int:
+        """The size of the training dataset to use. The value 0 means maximal value."""
+        return self._trainsize
+
+    @attribute
+    def valsize(self) -> int:
+        """The size of the validation dataset to use. The value 0 means maximal value."""
+        return self._valsize
+
+    @attribute
+    def numfeatures(self) -> int:
+        """The number of features to have in the dataset when it is generated."""
+        return self._numfeatures
 
     @attribute
     def mc_timeout(self) -> int:
         """The maximum time in seconds that a Monte-Carlo importance method is allowed to run."""
         return self._mc_timeout
 
     @result
@@ -96,57 +118,69 @@
 
     @property
     def completed(self) -> bool:
         return self.importance_cputime is not None
 
     @property
     def dataframe(self) -> DataFrame:
-        attributes = self._flatten_attributes(self.attributes)
-        return DataFrame(attributes)
+        return DataFrame(
+            dict(
+                dataset=[self.dataset],
+                pipeline=[self.pipeline],
+                model=[self.model],
+                method=[self.method],
+                iteration=[self.iteration],
+                trainsize=[self.trainsize],
+                valsize=[self.valsize],
+                numfeatures=[self.numfeatures],
+                timeout=[self.mc_timeout],
+                importance_cputime=[self.importance_cputime],
+            )
+        )
 
-    @lru_cache(maxsize=1)
-    @classmethod
-    def get_keyword_replacements(cls: Type["Scenario"]) -> Dict[str, str]:
-        return {
-            **KEYWORD_REPLACEMENTS,
-            **Dataset.get_keyword_replacements(),
-            **Pipeline.get_keyword_replacements(),
-            **Model.get_keyword_replacements(),
-        }
+    @property
+    def keyword_replacements(self) -> Dict[str, str]:
+        return {**KEYWORD_REPLACEMENTS, **Pipeline.summaries}
 
     def _run(self, progress_bar: bool = True, **kwargs: Any) -> None:
+
         # Load dataset.
-        dataset = self.dataset.load()
-        self.logger.debug("Loaded dataset %s.", dataset)
+        seed = self._seed + self._iteration
+        dataset = Dataset.datasets[self.dataset](
+            trainsize=self.trainsize, valsize=self.valsize, numfeatures=self.numfeatures, seed=seed
+        )
+        dataset.load()
+        self.logger.debug(
+            "Dataset '%s' loaded (trainsize=%d, valsize=%d).", self.dataset, dataset.trainsize, dataset.valsize
+        )
 
         # Load the pipeline and process the data.
-        pipeline = self.pipeline.construct(dataset)
+        pipeline = Pipeline.pipelines[self.pipeline].construct(dataset)
 
         # Initialize the model and utility.
-        model = self.model.construct(dataset)
+        model = get_model(self.model)
         utility = SklearnModelAccuracy(model)
 
         # Compute importance scores and time it.
         importance_time_start = process_time_ns()
-        n_units = self.dataset.provenance.num_units
+        n_units = dataset.units.shape[0]
         importance: Optional[ShapleyImportance] = None
-        random = np.random.RandomState(seed=self.seed + self._iteration)
+        random = np.random.RandomState(seed=self._seed + self._iteration)
         if self.method == RepairMethod.RANDOM:
             list(random.rand(n_units))
         else:
             method = IMPORTANCE_METHODS[self.method]
             mc_iterations = MC_ITERATIONS[self.method]
             mc_preextract = RepairMethod.is_tmc_nonpipe(self.method)
+            provenance = np.array(np.nan)  # TODO: Remove this hack.
             importance = ShapleyImportance(
                 method=method,
                 utility=utility,
                 pipeline=pipeline,
                 mc_iterations=mc_iterations,
                 mc_timeout=self.mc_timeout,
                 mc_preextract=mc_preextract,
             )
-            importance.fit(dataset.X_train, dataset.y_train, dataset.metadata_train).score(
-                dataset.X_val, dataset.y_val, dataset.metadata_val
-            )
+            importance.fit(dataset.X_train, dataset.y_train, provenance=provenance).score(dataset.X_val, dataset.y_val)
         importance_time_end = process_time_ns()
         self._importance_cputime = (importance_time_end - importance_time_start) / 1e9
         self.logger.debug("Importance computed in: %s", str(timedelta(seconds=self._importance_cputime)))
```

### Comparing `datascope-experiments-0.0.85/datascope/experiments/scenarios/datascope_scenario.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/datascope_scenario.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,282 +1,235 @@
 import pandas as pd
 
 from datascope.importance.shapley import ImportanceMethod, DEFAULT_MC_TIMEOUT, DEFAULT_MC_TOLERANCE, DEFAULT_NN_K
 from enum import Enum
-from methodtools import lru_cache
 from pandas import DataFrame
-from typing import Any, Optional, Dict, Type
+from typing import Any, Optional, Dict
 
-from ..bench import Scenario, attribute, result
+from .base import Scenario, attribute, result
 from ..datasets import (
     Dataset,
     BiasMethod,
-    AugmentableMixin,
+    DEFAULT_TRAINSIZE,
+    DEFAULT_VALSIZE,
+    DEFAULT_TESTSIZE,
     DEFAULT_BIAS_METHOD,
-    DEFAULT_CACHE_DIR,
+    KEYWORD_REPLACEMENTS as DATASET_KEYWORD_REPLACEMENTS,
 )
-from ..pipelines import Pipeline, Model, Postprocessor, LogisticRegressionModel
+from ..pipelines import Pipeline, ModelType
 
 
 class RepairMethod(str, Enum):
     KNN_Single = "shapley-knn-single"
     KNN_Interactive = "shapley-knn-interactive"
-    KNN_Raw = "shapley-knn-raw"
     TMC_1 = "shapley-tmc-001"
     TMC_5 = "shapley-tmc-005"
     TMC_10 = "shapley-tmc-010"
     TMC_50 = "shapley-tmc-050"
     TMC_100 = "shapley-tmc-100"
     TMC_500 = "shapley-tmc-500"
-    TMC_1000 = "shapley-tmc-1000"
     TMC_PIPE_1 = "shapley-tmc-pipe-001"
     TMC_PIPE_5 = "shapley-tmc-pipe-005"
     TMC_PIPE_10 = "shapley-tmc-pipe-010"
     TMC_PIPE_50 = "shapley-tmc-pipe-050"
     TMC_PIPE_100 = "shapley-tmc-pipe-100"
     TMC_PIPE_500 = "shapley-tmc-pipe-500"
-    TMC_PIPE_1000 = "shapley-tmc-pipe-1000"
     RANDOM = "random"
-    INFLUENCE = "influence"
 
     @staticmethod
     def is_pipe(method: "RepairMethod") -> bool:
         return method in [
             RepairMethod.TMC_PIPE_1,
             RepairMethod.TMC_PIPE_5,
             RepairMethod.TMC_PIPE_10,
             RepairMethod.TMC_PIPE_50,
             RepairMethod.TMC_PIPE_100,
             RepairMethod.TMC_PIPE_500,
-            RepairMethod.TMC_PIPE_1000,
         ]
 
     @staticmethod
     def is_tmc(method: "RepairMethod") -> bool:
         return method in [
             RepairMethod.TMC_1,
             RepairMethod.TMC_5,
             RepairMethod.TMC_10,
             RepairMethod.TMC_50,
             RepairMethod.TMC_100,
             RepairMethod.TMC_500,
-            RepairMethod.TMC_1000,
             RepairMethod.TMC_PIPE_1,
             RepairMethod.TMC_PIPE_5,
             RepairMethod.TMC_PIPE_10,
             RepairMethod.TMC_PIPE_50,
             RepairMethod.TMC_PIPE_100,
             RepairMethod.TMC_PIPE_500,
-            RepairMethod.TMC_PIPE_1000,
         ]
 
     @staticmethod
     def is_tmc_nonpipe(method: "RepairMethod") -> bool:
         return method in [
             RepairMethod.TMC_1,
             RepairMethod.TMC_5,
             RepairMethod.TMC_10,
             RepairMethod.TMC_50,
             RepairMethod.TMC_100,
             RepairMethod.TMC_500,
-            RepairMethod.TMC_1000,
         ]
 
 
 class RepairGoal(str, Enum):
     FAIRNESS = "fairness"
     ACCURACY = "accuracy"
 
 
 class UtilityType(str, Enum):
     ACCURACY = "acc"
     EQODDS = "eqodds"
     EQODDS_AND_ACCURACY = "eqodds-acc"
-    ROC_AUC = "rocauc"
 
 
 IMPORTANCE_METHODS = {
     RepairMethod.KNN_Single: ImportanceMethod.NEIGHBOR,
     RepairMethod.KNN_Interactive: ImportanceMethod.NEIGHBOR,
-    RepairMethod.KNN_Raw: ImportanceMethod.NEIGHBOR,
     RepairMethod.TMC_1: ImportanceMethod.MONTECARLO,
     RepairMethod.TMC_5: ImportanceMethod.MONTECARLO,
     RepairMethod.TMC_10: ImportanceMethod.MONTECARLO,
     RepairMethod.TMC_50: ImportanceMethod.MONTECARLO,
     RepairMethod.TMC_100: ImportanceMethod.MONTECARLO,
     RepairMethod.TMC_500: ImportanceMethod.MONTECARLO,
-    RepairMethod.TMC_1000: ImportanceMethod.MONTECARLO,
     RepairMethod.TMC_PIPE_1: ImportanceMethod.MONTECARLO,
     RepairMethod.TMC_PIPE_5: ImportanceMethod.MONTECARLO,
     RepairMethod.TMC_PIPE_10: ImportanceMethod.MONTECARLO,
     RepairMethod.TMC_PIPE_50: ImportanceMethod.MONTECARLO,
     RepairMethod.TMC_PIPE_100: ImportanceMethod.MONTECARLO,
     RepairMethod.TMC_PIPE_500: ImportanceMethod.MONTECARLO,
-    RepairMethod.TMC_PIPE_1000: ImportanceMethod.MONTECARLO,
 }
 
+
 MC_ITERATIONS = {
     RepairMethod.KNN_Single: 0,
     RepairMethod.KNN_Interactive: 0,
-    RepairMethod.KNN_Raw: 0,
     RepairMethod.TMC_1: 1,
     RepairMethod.TMC_5: 5,
     RepairMethod.TMC_10: 10,
     RepairMethod.TMC_50: 50,
     RepairMethod.TMC_100: 100,
     RepairMethod.TMC_500: 500,
-    RepairMethod.TMC_1000: 1000,
     RepairMethod.TMC_PIPE_1: 1,
     RepairMethod.TMC_PIPE_5: 5,
     RepairMethod.TMC_PIPE_10: 10,
     RepairMethod.TMC_PIPE_50: 50,
     RepairMethod.TMC_PIPE_100: 100,
     RepairMethod.TMC_PIPE_500: 500,
-    RepairMethod.TMC_PIPE_1000: 1000,
 }
 
 KEYWORD_REPLACEMENTS = {
     "random": "Random",
-    "influence": "Influence Function",
     "shapley-tmc": "Shapley TMC",
     "shapley-knn-single": "Shapley KNN Single",
     "shapley-knn-interactive": "Shapley KNN Interactive",
-    "shapley-knn-raw": "Shapley KNN over Raw Features",
-    "shapley-tmc-001": "Shapley TMC+PP x1",
-    "shapley-tmc-005": "Shapley TMC+PP x5",
-    "shapley-tmc-010": "Shapley TMC+PP x10",
-    "shapley-tmc-050": "Shapley TMC+PP x50",
-    "shapley-tmc-100": "Shapley TMC+PP x100",
-    "shapley-tmc-500": "Shapley TMC+PP x500",
-    "shapley-tmc-1000": "Shapley TMC+PP x1000",
-    "shapley-tmc-pipe-001": "Shapley TMC x1",
-    "shapley-tmc-pipe-005": "Shapley TMC x5",
-    "shapley-tmc-pipe-010": "Shapley TMC x10",
-    "shapley-tmc-pipe-050": "Shapley TMC x50",
-    "shapley-tmc-pipe-100": "Shapley TMC x100",
-    "shapley-tmc-pipe-500": "Shapley TMC x500",
-    "shapley-tmc-pipe-1000": "Shapley TMC x1000",
+    "shapley-tmc-001": "Shapley TMC x1",
+    "shapley-tmc-005": "Shapley TMC x5",
+    "shapley-tmc-010": "Shapley TMC x10",
+    "shapley-tmc-050": "Shapley TMC x50",
+    "shapley-tmc-100": "Shapley TMC x100",
+    "shapley-tmc-500": "Shapley TMC x500",
+    "shapley-tmc-pipe-001": "Shapley TMC Pipe x1",
+    "shapley-tmc-pipe-005": "Shapley TMC Pipe x5",
+    "shapley-tmc-pipe-010": "Shapley TMC Pipe x10",
+    "shapley-tmc-pipe-050": "Shapley TMC Pipe x50",
+    "shapley-tmc-pipe-100": "Shapley TMC Pipe x100",
+    "shapley-tmc-pipe-500": "Shapley TMC Pipe x500",
     "eqodds": "Equalized Odds Difference",
     "importance_cputime": "Compute Time [s]",
     "steps": "Repair Steps Taken",
     "steps_rel": "Relative Repair Steps Taken",
     "acc": "Accuracy",
     "eqodds-acc": "Accuracy + Equalized Odds Difference",
-    "accuracy": "Accuracy",
-    "accuracy_rel": "Relative Accuracy",
-    "roc_auc": "ROC AUC",
-    "roc_auc_rel": "Relative ROC AUC",
-    "train_eqodds": "Equalized Odds Difference",
-    "train_eqodds_rel": "Relative Equalized Odds Difference",
-    "train_accuracy": "Accuracy",
-    "train_accuracy_rel": "Relative Accuracy",
-    "train_roc_auc": "ROC AUC",
-    "train_roc_auc_rel": "Relative ROC AUC",
-    "val_eqodds": "Validation Equalized Odds Difference",
-    "val_eqodds_rel": "Validation Relative Equalized Odds Difference",
-    "val_accuracy": "Validation Accuracy",
-    "val_accuracy_rel": "Validation Relative Accuracy",
-    "val_roc_auc": "Validation ROC AUC",
-    "val_roc_auc_rel": "Validation Relative ROC AUC",
-    "test_eqodds": "Test Equalized Odds Difference",
-    "test_eqodds_rel": "Test Relative Equalized Odds Difference",
-    "test_accuracy": "Test Accuracy",
-    "test_accuracy_rel": "Test Relative Accuracy",
-    "test_roc_auc": "Test ROC AUC",
-    "test_roc_auc_rel": "Test Relative ROC AUC",
 }
+KEYWORD_REPLACEMENTS.update(DATASET_KEYWORD_REPLACEMENTS)
 
 DEFAULT_SEED = 1
 DEFAULT_CHECKPOINTS = 100
 DEFAULT_PROVIDERS = 0
-DEFAULT_MODEL = LogisticRegressionModel()
+DEFAULT_MODEL = ModelType.LogisticRegression
 DEFAULT_REPAIR_GOAL = RepairGoal.ACCURACY
 DEFAULT_TRAIN_BIAS = 0.0
 DEFAULT_VAL_BIAS = 0.0
-DEFAULT_AUGMENT_FACTOR = 0
 
 
 class DatascopeScenario(Scenario, abstract=True):
     def __init__(
         self,
-        dataset: Dataset,
-        pipeline: Pipeline,
+        dataset: str,
+        pipeline: str,
         method: RepairMethod,
         utility: UtilityType,
-        model: Model = DEFAULT_MODEL,
-        postprocessor: Optional[Postprocessor] = None,
+        iteration: int,
+        model: ModelType = DEFAULT_MODEL,
         trainbias: float = DEFAULT_TRAIN_BIAS,
         valbias: float = DEFAULT_VAL_BIAS,
         biasmethod: BiasMethod = DEFAULT_BIAS_METHOD,
         seed: int = DEFAULT_SEED,
-        augment_factor: int = DEFAULT_AUGMENT_FACTOR,
-        eager_preprocessing: bool = False,
-        pipeline_cache_dir: str = DEFAULT_CACHE_DIR,
+        trainsize: int = DEFAULT_TRAINSIZE,
+        valsize: int = DEFAULT_VALSIZE,
+        testsize: int = DEFAULT_TESTSIZE,
         mc_timeout: int = DEFAULT_MC_TIMEOUT,
         mc_tolerance: float = DEFAULT_MC_TOLERANCE,
         nn_k: int = DEFAULT_NN_K,
-        numcheckpoints: int = DEFAULT_CHECKPOINTS,
+        checkpoints: int = DEFAULT_CHECKPOINTS,
         providers: int = DEFAULT_PROVIDERS,
         repairgoal: RepairGoal = DEFAULT_REPAIR_GOAL,
         evolution: Optional[pd.DataFrame] = None,
         importance_cputime: Optional[float] = None,
-        iteration: Optional[int] = None,  # Iteration became seed. Keeping this for back compatibility reasons.
         **kwargs: Any
     ) -> None:
         super().__init__(**kwargs)
         self._dataset = dataset
         self._pipeline = pipeline
         self._method = method
         self._utility = utility
+        self._iteration = iteration
         self._model = model
-        self._postprocessor = postprocessor
         self._trainbias = trainbias
         self._valbias = valbias
         self._biasmethod = biasmethod
         self._seed = seed
-        if iteration is not None:
-            self._seed += iteration
-        self._augment_factor = augment_factor
-        self._eager_preprocessing = eager_preprocessing
-        self._pipeline_cache_dir = pipeline_cache_dir
+        self._trainsize = trainsize
+        self._valsize = valsize
+        self._testsize = testsize
         self._mc_timeout = mc_timeout
         self._mc_tolerance = mc_tolerance
         self._nn_k = nn_k
-        self._numcheckpoints = numcheckpoints
+        self._checkpoints = checkpoints
         self._providers = providers
         self._repairgoal = repairgoal
         self._evolution = pd.DataFrame() if evolution is None else evolution
         self._importance_cputime: Optional[float] = importance_cputime
 
-    @attribute
-    def dataset(self) -> Dataset:
+    @attribute(domain=Dataset.datasets.keys())
+    def dataset(self) -> str:
         """Dataset to use for training and validation."""
         return self._dataset
 
-    @attribute
-    def pipeline(self) -> Pipeline:
+    @attribute(domain=Pipeline.pipelines.keys())
+    def pipeline(self) -> str:
         """Pipeline to use for feature extraction."""
         return self._pipeline
 
     @attribute
     def method(self) -> RepairMethod:
         """Method used to perform data repairs."""
         return self._method
 
-    @attribute
-    def model(self) -> Model:
+    @attribute(domain=[None])
+    def model(self) -> ModelType:
         """Model used to make predictions."""
         return self._model
 
     @attribute
-    def postprocessor(self) -> Optional[Postprocessor]:
-        """Postprocessor used to perform final processing of model predictions."""
-        return self._postprocessor
-
-    @attribute
     def trainbias(self) -> float:
         """The bias of the training dataset used in fairness experiments."""
         return self._trainbias
 
     @attribute
     def valbias(self) -> float:
         """The bias of the validation dataset used in fairness experiments."""
@@ -289,32 +242,32 @@
 
     @attribute
     def utility(self) -> UtilityType:
         """The utility to use for importance computation."""
         return self._utility
 
     @attribute(domain=range(10))
-    def seed(self) -> int:
-        """The random seed that applies to all pseudo-random processes in the scenario."""
-        return self._seed
+    def iteration(self) -> int:
+        """The ordinal number of the experiment repetition. Also serves as the random seed."""
+        return self._iteration
 
     @attribute
-    def augment_factor(self) -> int:
-        """The augmentation factor to apply to the dataset after loading it (if applicable)."""
-        return self._augment_factor
+    def trainsize(self) -> int:
+        """The size of the training dataset to use for model training. The value 0 means maximal value."""
+        return self._trainsize
 
-    @attribute(domain=[None])
-    def eager_preprocessing(self) -> bool:
-        """Training data is passed through the preprocessing pipeline before being passed to importance computation."""
-        return self._eager_preprocessing
+    @attribute
+    def valsize(self) -> int:
+        """The size of the validation dataset to use for importance computation. The value 0 means maximal value."""
+        return self._valsize
 
     @attribute
-    def pipeline_cache_dir(self) -> str:
-        """The directory where the pipeline cache is stored."""
-        return self._pipeline_cache_dir
+    def testsize(self) -> int:
+        """The size of the test dataset to use for final evaluation. The value 0 means maximal value."""
+        return self._testsize
 
     @attribute
     def mc_timeout(self) -> int:
         """The maximum time in seconds that a Monte-Carlo importance method is allowed to run. Zero means no timeout."""
         return self._mc_timeout
 
     @attribute
@@ -324,20 +277,20 @@
 
     @attribute
     def nn_k(self) -> int:
         """The size of the K-neighborhood of the Shapley KNN model."""
         return self._nn_k
 
     @attribute
-    def numcheckpoints(self) -> int:
+    def checkpoints(self) -> int:
         """
         The number of checkpoints to record in the workflow.
         The value 0 means that a checkpoint will be recorded for each training data example.
         """
-        return self._numcheckpoints
+        return self._checkpoints
 
     @attribute
     def providers(self) -> int:
         """
         The number of data providers. Each provider is treated as one unit.
         The value 0 means that each data example is provided independently.
         """
@@ -351,39 +304,40 @@
     @result
     def evolution(self) -> DataFrame:
         """The evolution of the experimental parameters."""
         return self._evolution
 
     @property
     def completed(self) -> bool:
-        return len(self._evolution) == self.numcheckpoints + 1
+        return len(self._evolution) == self.checkpoints + 1
 
     @property
     def dataframe(self) -> DataFrame:
-        attributes = self._flatten_attributes(self.attributes)
-        result = self._evolution.assign(**attributes)
+        result = self._evolution.assign(
+            id=self.id,
+            dataset=self.dataset,
+            pipeline=self.pipeline,
+            model=self.model,
+            providers=self.providers,
+            mc_timeout=self.mc_timeout,
+            mc_tolerance=self.mc_tolerance,
+            nn_k=self.nn_k,
+            method=self.method,
+            utility=self.utility,
+            iteration=self.iteration,
+        )
         if "importance_cputime" not in result.columns and self._importance_cputime is not None:
             result = result.assign(importance_cputime=self._importance_cputime)
         return result
 
-    @lru_cache(maxsize=1)
-    @classmethod
-    def get_keyword_replacements(cls: Type["Scenario"]) -> Dict[str, str]:
-        return {
-            **KEYWORD_REPLACEMENTS,
-            **Dataset.get_keyword_replacements(),
-            **Pipeline.get_keyword_replacements(),
-            **Postprocessor.get_keyword_replacements(),
-            **Model.get_keyword_replacements(),
-        }
+    @property
+    def keyword_replacements(self) -> Dict[str, str]:
+        return {**KEYWORD_REPLACEMENTS, **Pipeline.summaries}
 
     @classmethod
     def is_valid_config(cls, **attributes: Any) -> bool:
         result = True
-        dataset: Optional[Dataset] = attributes.get("dataset", None)
-        pipeline: Optional[Pipeline] = attributes.get("pipeline", None)
-        augment_factor: Optional[int] = attributes.get("augment_factor", None)
-        if pipeline is not None and dataset is not None:
-            result = result and any(isinstance(dataset, modality) for modality in pipeline.modalities)
-        if augment_factor is not None and augment_factor > 0 and dataset is not None:
-            result = result and isinstance(dataset, AugmentableMixin)
+        if "pipeline" in attributes and "dataset" in attributes:
+            dataset = Dataset.datasets[attributes["dataset"]]()
+            pipeline = Pipeline.pipelines[attributes["pipeline"]].construct(dataset)
+            result = result and dataset.modality in pipeline.modalities
         return result and super().is_valid_config(**attributes)
```

### Comparing `datascope-experiments-0.0.85/datascope/experiments/scenarios/label_repair.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/label_repair.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,441 +1,382 @@
 from copy import deepcopy
 import numpy as np
 import pandas as pd
 
 from datascope.importance.common import (
-    JointUtility,
     SklearnModelAccuracy,
+    JointUtility,
     SklearnModelEqualizedOddsDifference,
-    SklearnModelRocAuc,
     Utility,
-    UtilityResult,
     compute_groupings,
 )
-from datascope.importance.importance import Importance
 from datascope.importance.shapley import ShapleyImportance
 from datetime import timedelta
-from methodtools import lru_cache
-from numpy.typing import NDArray
 from time import process_time_ns
-from typing import Any, Iterable, List, Optional, Union, Dict, Type
+from typing import Any, Iterable, List, Optional, Union, Dict
 
-from ..bench import attribute
+from .base import attribute
 from .datascope_scenario import (
     DatascopeScenario,
     RepairMethod,
     IMPORTANCE_METHODS,
     MC_ITERATIONS,
     DEFAULT_SEED,
     DEFAULT_CHECKPOINTS,
     DEFAULT_PROVIDERS,
     DEFAULT_MODEL,
-    DEFAULT_TRAIN_BIAS,
-    DEFAULT_VAL_BIAS,
-    DEFAULT_AUGMENT_FACTOR,
     DEFAULT_REPAIR_GOAL,
     DEFAULT_MC_TIMEOUT,
     DEFAULT_MC_TOLERANCE,
     DEFAULT_NN_K,
     UtilityType,
     RepairGoal,
 )
 from ..datasets import (
     Dataset,
     BiasMethod,
-    BiasedNoisyLabelDataset,
-    NoisyLabelDataset,
-    AugmentableMixin,
-    TabularDatasetMixin,
-    ImageDatasetMixin,
-    RandomDataset,
-    DEFAULT_BIAS_METHOD,
-    DEFAULT_CACHE_DIR,
+    BiasedDirtyLabelDataset,
+    DirtyLabelDataset,
+    DEFAULT_TRAINSIZE,
+    DEFAULT_VALSIZE,
+    DEFAULT_TESTSIZE,
 )
-from ..pipelines import Pipeline, FlattenPipeline, Model, DistanceModelMixin, Postprocessor, LogisticRegressionModel
+from ..pipelines import Pipeline, ModelType, get_model
 
 
 DEFAULT_DIRTY_RATIO = 0.5
 DEFAULT_DIRTY_BIAS = 0.0
 KEYWORD_REPLACEMENTS = {
+    "accuracy": "Accuracy",
+    "accuracy_rel": "Relative Accuracy",
     "repaired": "Number of Labels Examined",
     "repaired_rel": "Portion of Labels Examined",
     "discovered": "Number of Dirty Labels Found",
     "discovered_rel": "Portion of Dirty Labels Found",
 }
 
 
 class LabelRepairScenario(DatascopeScenario, id="label-repair"):
     def __init__(
         self,
-        dataset: Dataset,
-        pipeline: Pipeline,
+        dataset: str,
+        pipeline: str,
         method: RepairMethod,
-        utility: UtilityType,
-        model: Model = DEFAULT_MODEL,
-        postprocessor: Optional[Postprocessor] = None,
-        trainbias: float = DEFAULT_TRAIN_BIAS,
-        valbias: float = DEFAULT_VAL_BIAS,
-        biasmethod: BiasMethod = DEFAULT_BIAS_METHOD,
+        iteration: int,
+        utility: UtilityType = UtilityType.ACCURACY,
+        model: ModelType = DEFAULT_MODEL,
+        dirtyratio: float = DEFAULT_DIRTY_RATIO,
+        dirtybias: float = DEFAULT_DIRTY_BIAS,
         seed: int = DEFAULT_SEED,
-        augment_factor: int = DEFAULT_AUGMENT_FACTOR,
-        eager_preprocessing: bool = False,
-        pipeline_cache_dir: str = DEFAULT_CACHE_DIR,
+        trainsize: int = DEFAULT_TRAINSIZE,
+        valsize: int = DEFAULT_VALSIZE,
+        testsize: int = DEFAULT_TESTSIZE,
         mc_timeout: int = DEFAULT_MC_TIMEOUT,
         mc_tolerance: float = DEFAULT_MC_TOLERANCE,
         nn_k: int = DEFAULT_NN_K,
         checkpoints: int = DEFAULT_CHECKPOINTS,
         providers: int = DEFAULT_PROVIDERS,
         repairgoal: RepairGoal = DEFAULT_REPAIR_GOAL,
         evolution: Optional[pd.DataFrame] = None,
         importance_cputime: Optional[float] = None,
-        iteration: Optional[int] = None,  # Iteration became seed. Keeping this for back compatibility reasons.
-        dirtyratio: float = DEFAULT_DIRTY_RATIO,
-        dirtybias: float = DEFAULT_DIRTY_BIAS,
         **kwargs: Any
     ) -> None:
         kwargs.pop("biasmethod", None)
         super().__init__(
             dataset=dataset,
             pipeline=pipeline,
             method=method,
             utility=utility,
+            iteration=iteration,
             model=model,
-            postprocessor=postprocessor,
-            trainbias=trainbias,
-            valbias=valbias,
             seed=seed,
-            augment_factor=augment_factor,
-            eager_preprocessing=eager_preprocessing,
-            pipeline_cache_dir=pipeline_cache_dir,
+            trainsize=trainsize,
+            valsize=valsize,
+            testsize=testsize,
             mc_timeout=mc_timeout,
             mc_tolerance=mc_tolerance,
             nn_k=nn_k,
             checkpoints=checkpoints,
             providers=providers,
             repairgoal=repairgoal,
+            biasmethod=BiasMethod.Feature,
             evolution=evolution,
             importance_cputime=importance_cputime,
-            iteration=iteration,
             **kwargs
         )
         self._dirtyratio = dirtyratio
         self._dirtybias = dirtybias
 
     @classmethod
     def is_valid_config(cls, **attributes: Any) -> bool:
         result = True
-        dataset: Optional[Dataset] = attributes.get("dataset", None)
-        repairgoal: RepairGoal = attributes.get("repairgoal", None)
-        utility: UtilityType = attributes.get("utility", None)
-        method: RepairMethod = attributes.get("method", None)
-        model: Model = attributes.get("model", None)
-
-        if dataset is not None:
-            result = result and isinstance(dataset, NoisyLabelDataset)
-        if repairgoal is not None or repairgoal == RepairGoal.FAIRNESS:
-            if dataset is not None:
-                result = result and isinstance(dataset, BiasedNoisyLabelDataset)
-        elif repairgoal is not None and repairgoal == RepairGoal.ACCURACY:
-            if dataset is not None:
-                result = result and not isinstance(dataset, RandomDataset)
-            if utility is not None:
-                result = result and utility in [UtilityType.ACCURACY, UtilityType.ROC_AUC]
-        if method is not None and method == RepairMethod.KNN_Raw:
-            result = result and any(
-                isinstance(dataset, modality) for modality in [TabularDatasetMixin, ImageDatasetMixin]
-            )
-        elif method is not None and method == RepairMethod.INFLUENCE:
-            result = result and isinstance(model, LogisticRegressionModel)
+        # if "method" in attributes:
+        #     result = result and not RepairMethod.is_tmc_nonpipe(attributes["method"])
+        if "dataset" in attributes:
+            dataset_class = Dataset.datasets[attributes["dataset"]]
+            result = result and issubclass(dataset_class, DirtyLabelDataset)
+
+        if "repairgoal" not in attributes or attributes["repairgoal"] == RepairGoal.FAIRNESS:
+            if "dataset" in attributes:
+                dataset = Dataset.datasets[attributes["dataset"]]()
+                result = result and isinstance(dataset, BiasedDirtyLabelDataset)
+        elif "repairgoal" in attributes and attributes["repairgoal"] == RepairGoal.ACCURACY:
+            if "dataset" in attributes:
+                result = result and (attributes["dataset"] != "random")
+            if "utility" in attributes:
+                result = result and attributes["utility"] == UtilityType.ACCURACY
         return result and super().is_valid_config(**attributes)
 
     @attribute
     def dirtyratio(self) -> float:
         """The proportion of examples that will have corrupted labels in label repair experiments."""
         return self._dirtyratio
 
     @attribute
     def dirtybias(self) -> float:
         """The bias of dirty ratio between the sensitive data subgroup and the rest."""
         return self._dirtybias
 
-    @lru_cache(maxsize=1)
-    @classmethod
-    def get_keyword_replacements(cls: Type["LabelRepairScenario"]) -> Dict[str, str]:
-        result = super().get_keyword_replacements()
+    @property
+    def keyword_replacements(self) -> Dict[str, str]:
+        result = super().keyword_replacements
         return {**result, **KEYWORD_REPLACEMENTS}
 
     def _run(self, progress_bar: bool = True, **kwargs: Any) -> None:
+
         # Load dataset.
-        dataset = self.dataset.load()
-        assert isinstance(dataset, NoisyLabelDataset)
-        self.logger.debug("Loaded dataset %s.", dataset)
+        seed = self._seed + self._iteration
+        dataset = Dataset.datasets[self.dataset](
+            trainsize=self.trainsize, valsize=self.valsize, testsize=self.testsize, seed=seed
+        )
+        assert isinstance(dataset, DirtyLabelDataset)
+        dataset.load()
+        self.logger.debug(
+            "Dataset '%s' loaded (trainsize=%d, valsize=%d, testsize=%d).",
+            self.dataset,
+            dataset.trainsize,
+            dataset.valsize,
+            dataset.testsize,
+        )
 
         # Compute sensitive feature groupings.
-        groupings_val: Optional[NDArray] = None
-        groupings_test: Optional[NDArray] = None
-        if isinstance(dataset, BiasedNoisyLabelDataset):
+        groupings_val: Optional[np.ndarray] = None
+        groupings_test: Optional[np.ndarray] = None
+        if isinstance(dataset, BiasedDirtyLabelDataset):
             groupings_val = compute_groupings(dataset.X_val, dataset.sensitive_feature)
             groupings_test = compute_groupings(dataset.X_test, dataset.sensitive_feature)
 
         # Create the dirty dataset and apply the data corruption.
+        # dataset_dirty = deepcopy(dataset)
+        # random = np.random.RandomState(seed=self._seed + self._iteration)
+        # dirty_probs = [1 - self._dirtyratio, self._dirtyratio]
+        # dirty_idx = random.choice(a=[False, True], size=(dataset_dirty.trainsize), p=dirty_probs)
+        # dataset_dirty.y_train[dirty_idx] = 1 - dataset_dirty.y_train[dirty_idx]
         probabilities: Union[float, List[float]] = self._dirtyratio
         if self.providers > 1:
             dirty_providers = round(self.providers * self._dirtyratio)
             clean_providers = self.providers - dirty_providers
             probabilities = [float(i + 1) / dirty_providers for i in range(dirty_providers)]
             probabilities += [0.0 for _ in range(clean_providers)]
 
         if self.repairgoal == RepairGoal.ACCURACY:
             dataset_dirty = dataset.corrupt_labels(probabilities=probabilities)
             units_dirty = deepcopy(dataset_dirty.units_dirty)
         if self.repairgoal == RepairGoal.FAIRNESS:
-            assert isinstance(dataset, BiasedNoisyLabelDataset)
+            assert isinstance(dataset, BiasedDirtyLabelDataset)
             dataset_dirty = dataset.corrupt_labels_with_bias(probabilities=probabilities, groupbias=self.dirtybias)
             units_dirty = deepcopy(dataset_dirty.units_dirty)
 
-        if self.augment_factor > 0 and self.method != RepairMethod.KNN_Raw:
-            assert isinstance(dataset, AugmentableMixin) and isinstance(dataset_dirty, AugmentableMixin)
-            dataset.augment(factor=self.augment_factor, inplace=True)
-            dataset_dirty.augment(factor=self.augment_factor, inplace=True)
-
-        # Load the pipeline and process the data if eager preprocessing was specified.
-        pipeline = self.pipeline.construct(dataset)
-        if self.eager_preprocessing:
-            dataset.apply(pipeline, cache_dir=self.pipeline_cache_dir, inplace=True)
-            dataset_dirty.apply(pipeline, cache_dir=self.pipeline_cache_dir, inplace=True)
-
-        # Initialize the model, postprocessor and utility.
-        model = self.model.construct(dataset)
-        postprocessor = None if self.postprocessor is None else self.postprocessor.construct(dataset)
-        accuracy_utility = SklearnModelAccuracy(model, postprocessor=postprocessor)
-        roc_auc_utility = SklearnModelRocAuc(model, postprocessor=postprocessor)
+        # Load the pipeline and process the data.
+        pipeline = Pipeline.pipelines[self.pipeline].construct(dataset)
+        # X_train, y_train = dataset.X_train, dataset.y_train
+        # X_val, y_val = dataset.X_val, dataset.y_val
+        # X_train_dirty, y_train_dirty = dataset_dirty.X_train, dataset_dirty.y_train
+        # assert X_train is not None and y_train is not None
+        # assert X_train_dirty is not None and y_train_dirty is not None
+        # assert X_val is not None and y_val is not None
+        # if RepairMethod.is_tmc_nonpipe(self.method):
+        #     raise ValueError("This is not supported at the moment.")
+        #     self.logger.debug("Shape of X_train before feature extraction: %s", str(X_train.shape))
+        #     X_train = pipeline.fit_transform(X_train, y_train)  # TODO: Fit the pipeline with dirty data.
+        #     assert isinstance(X_train, ndarray)
+        #     X_train_dirty = pipeline.transform(X_train_dirty)
+        #     assert isinstance(X_train_dirty, ndarray)
+        #     X_val = pipeline.transform(X_val)
+        #     assert isinstance(X_val, ndarray)
+        #     self.logger.debug("Shape of X_train after feature extraction: %s", str(X_train.shape))
+
+        # Reshape datasets if needed.
+        # if X_train.ndim > 2:
+        #     X_train = X_train.reshape(X_train.shape[0], -1)
+        #     X_train_dirty = X_train_dirty.reshape(X_train_dirty.shape[0], -1)
+        #     X_val = X_val.reshape(X_val.shape[0], -1)
+        #     self.logger.debug("Need to reshape. New shape: %s", str(X_train.shape))
+
+        # Construct binarized provenance matrix.
+        # provenance = np.expand_dims(np.arange(dataset.trainsize, dtype=int), axis=(1, 2, 3))
+        # provenance = np.pad(provenance, pad_width=((0, 0), (0, 0), (0, 0), (0, 1)))
+        # provenance = binarize(provenance)
+
+        # Initialize the model and utility.
+        model = get_model(self.model)
+        # model_pipeline = deepcopy(pipeline)
+        # pipeline.steps.append(("model", model))
+        # if RepairMethod.is_pipe(self.method):
+        #     model = model_pipeline
+        accuracy_utility = SklearnModelAccuracy(model)
         eqodds_utility: Optional[SklearnModelEqualizedOddsDifference] = None
         if self.repairgoal == RepairGoal.FAIRNESS:
-            assert isinstance(dataset, BiasedNoisyLabelDataset)
+            assert isinstance(dataset, BiasedDirtyLabelDataset)
             eqodds_utility = SklearnModelEqualizedOddsDifference(
-                model,
-                sensitive_features=dataset.sensitive_feature,
-                groupings=groupings_test,
-                postprocessor=postprocessor,
+                model, sensitive_features=dataset.sensitive_feature, groupings=groupings_test
             )
 
+        # target_model = model if RepairMethod.is_tmc_nonpipe(self.method) else pipeline
         target_utility: Utility
         if self.utility == UtilityType.ACCURACY:
-            target_utility = JointUtility(SklearnModelAccuracy(model, postprocessor=postprocessor), weights=[-1.0])
+            target_utility = JointUtility(SklearnModelAccuracy(model), weights=[-1.0])
+            # target_utility = SklearnModelAccuracy(model)
         elif self.utility == UtilityType.EQODDS:
-            assert self.repairgoal == RepairGoal.FAIRNESS and isinstance(dataset, BiasedNoisyLabelDataset)
+            assert self.repairgoal == RepairGoal.FAIRNESS and isinstance(dataset, BiasedDirtyLabelDataset)
             target_utility = SklearnModelEqualizedOddsDifference(
-                model,
-                sensitive_features=dataset.sensitive_feature,
-                groupings=groupings_val,
-                postprocessor=postprocessor,
+                model, sensitive_features=dataset.sensitive_feature, groupings=groupings_val
             )
         elif self.utility == UtilityType.EQODDS_AND_ACCURACY:
-            assert self.repairgoal == RepairGoal.FAIRNESS and isinstance(dataset, BiasedNoisyLabelDataset)
+            assert self.repairgoal == RepairGoal.FAIRNESS and isinstance(dataset, BiasedDirtyLabelDataset)
             target_utility = JointUtility(
-                SklearnModelAccuracy(model, postprocessor=postprocessor),
+                SklearnModelAccuracy(model),
                 SklearnModelEqualizedOddsDifference(
-                    model,
-                    sensitive_features=dataset.sensitive_feature,
-                    groupings=groupings_val,
-                    postprocessor=postprocessor,
+                    model, sensitive_features=dataset.sensitive_feature, groupings=groupings_val
                 ),
                 weights=[-0.5, 0.5],
             )
-        elif self.utility == UtilityType.ROC_AUC:
-            target_utility = JointUtility(SklearnModelRocAuc(model, postprocessor=postprocessor), weights=[-1.0])
         else:
             raise ValueError("Unknown utility type '%s'." % repr(self.utility))
 
         # Compute importance scores and time it.
         importance_time_start = process_time_ns()
-        n_units = dataset.provenance.num_units
-        importance: Optional[Importance] = None
+        n_units = dataset_dirty.units.shape[0]
+        importance: Optional[ShapleyImportance] = None
         importances: Optional[Iterable[float]] = None
-        random = np.random.RandomState(seed=self.seed + 1)
+        random = np.random.RandomState(seed=self._seed + self._iteration + 1)
         if self.method == RepairMethod.RANDOM:
             importances = list(random.rand(n_units))
-        elif self.method == RepairMethod.INFLUENCE:
-            from ..baselines.influence.importance import InfluenceImportance
-
-            dataset_f = dataset.apply(pipeline)
-            dataset_dirty_f = dataset_dirty.apply(pipeline)
-            importance = InfluenceImportance()
-            importances = importance.fit(
-                dataset_dirty_f.X_train, dataset_dirty_f.y_train, provenance=dataset_dirty_f.provenance
-            ).score(dataset_f.X_val, dataset_f.y_val)
-            importances = [-x for x in importances]
         else:
-            shapley_pipeline = pipeline if self.method != RepairMethod.KNN_Raw else FlattenPipeline()
             method = IMPORTANCE_METHODS[self.method]
             mc_iterations = MC_ITERATIONS[self.method]
             mc_preextract = RepairMethod.is_tmc_nonpipe(self.method)
             importance = ShapleyImportance(
                 method=method,
                 utility=target_utility,
-                pipeline=None if self.eager_preprocessing else shapley_pipeline,
+                pipeline=pipeline,
                 mc_iterations=mc_iterations,
                 mc_timeout=self.mc_timeout,
                 mc_tolerance=self.mc_tolerance,
                 mc_preextract=mc_preextract,
                 nn_k=self.nn_k,
                 logger=self.logger,
             )
-            if isinstance(model, DistanceModelMixin):
-                importance.nn_distance = model.distance
             importances = importance.fit(
-                dataset_dirty.X_train,
-                dataset_dirty.y_train,
-                dataset_dirty.metadata_train,
-                provenance=dataset_dirty.provenance,
-            ).score(dataset.X_val, dataset.y_val, dataset.metadata_val)
+                dataset_dirty.X_train, dataset_dirty.y_train, provenance=dataset_dirty.provenance
+            ).score(dataset.X_val, dataset.y_val)
         importance_time_end = process_time_ns()
         importance_cputime = (importance_time_end - importance_time_start) / 1e9
         self.logger.debug("Importance computed in: %s", str(timedelta(seconds=importance_cputime)))
         visited_units = np.zeros(n_units, dtype=bool)
         argsorted_importances = (-np.array(importances)).argsort()
-
-        if self.augment_factor > 0 and self.method == RepairMethod.KNN_Raw:
-            assert isinstance(dataset, AugmentableMixin) and isinstance(dataset_dirty, AugmentableMixin)
-            dataset.augment(factor=self.augment_factor, inplace=True)
-            dataset_dirty.augment(factor=self.augment_factor, inplace=True)
+        # argsorted_importances = np.ma.array(importances, mask=visited_units).argsort()
 
         # Run the model to get initial score.
-        dataset_f = dataset if self.eager_preprocessing else dataset.apply(pipeline, cache_dir=self.pipeline_cache_dir)
-        dataset_dirty_f = (
-            dataset_dirty
-            if self.eager_preprocessing
-            else dataset_dirty.apply(pipeline, cache_dir=self.pipeline_cache_dir)
-        )
-        eqodds_utility_result = UtilityResult()
+        # assert y_val is not None
+        dataset_f = dataset.apply(pipeline)
+        dataset_dirty_f = dataset_dirty.apply(pipeline)
+        eqodds: Optional[float] = None
         if eqodds_utility is not None:
-            eqodds_utility_result = eqodds_utility(
-                dataset_dirty_f.X_train,
-                dataset_dirty_f.y_train,
-                dataset_f.X_test,
-                dataset_f.y_test,
-                metadata_train=dataset_dirty_f.metadata_train,
-                metadata_test=dataset_f.metadata_test,
+            eqodds = eqodds_utility(
+                dataset_dirty_f.X_train, dataset_dirty_f.y_train, dataset_f.X_test, dataset_f.y_test
             )
-        accuracy_utility_result = accuracy_utility(
-            dataset_dirty_f.X_train,
-            dataset_dirty_f.y_train,
-            dataset_f.X_test,
-            dataset_f.y_test,
-            metadata_train=dataset_dirty_f.metadata_train,
-            metadata_test=dataset_f.metadata_test,
-        )
-        roc_auc_utility_result = roc_auc_utility(
-            dataset_dirty_f.X_train,
-            dataset_dirty_f.y_train,
-            dataset_f.X_test,
-            dataset_f.y_test,
-            metadata_train=dataset_dirty_f.metadata_train,
-            metadata_test=dataset_f.metadata_test,
+        accuracy = accuracy_utility(
+            dataset_dirty_f.X_train, dataset_dirty_f.y_train, dataset_f.X_test, dataset_f.y_test
         )
 
         # Update result table.
-        evolution = [
-            [
-                0.0,
-                eqodds_utility_result.score,
-                eqodds_utility_result.score,
-                accuracy_utility_result.score,
-                accuracy_utility_result.score,
-                roc_auc_utility_result.score,
-                roc_auc_utility_result.score,
-                0,
-                0.0,
-                0,
-                0.0,
-                0.0,
-            ]
-        ]
-        eqodds_start = eqodds_utility_result.score
-        accuracy_start = accuracy_utility_result.score
-        roc_auc_start = roc_auc_utility_result.score
+        evolution = [[0.0, eqodds, eqodds, accuracy, accuracy, 0, 0.0, 0, 0.0, 0.0]]
+        eqodds_start = eqodds
+        accuracy_start = accuracy
 
         # Set up progress bar.
-        n_checkpoints = self.numcheckpoints if self.numcheckpoints > 0 and self.numcheckpoints < n_units else n_units
-        n_units_per_checkpoint = round(n_units / n_checkpoints)
+        checkpoints = self.checkpoints if self.checkpoints > 0 and self.checkpoints < n_units else n_units
+        n_units_per_checkpoint = round(n_units / checkpoints)
         if progress_bar:
-            self.progress.start(total=n_checkpoints, desc="(id=%s) Repairs" % self.id)
+            self.progress.start(total=checkpoints, desc="(id=%s) Repairs" % self.id)
+        # pbar = None if not progress_bar else tqdm(total=dataset.trainsize, desc="%s Repairs" % str(self))
 
         # Iterate over the repair process.
-        for i in range(n_checkpoints):
+        # visited_units = np.zeros(dataset.trainsize, dtype=bool)
+        for i in range(checkpoints):
+
             # Determine indices of data examples that should be repaired given the unit with the highest importance.
             unvisited_units = np.invert(visited_units)
             target_units = argsorted_importances[unvisited_units[argsorted_importances]]
-            if i + 1 < n_checkpoints:
+            if i + 1 < checkpoints:
                 target_units = target_units[:n_units_per_checkpoint]
+            # target_query = np.zeros(n_units, dtype=int)
+            # target_query[target_units] = 1
+            # target_unit = np.ma.array(importances, mask=visited_units).argmin()
+            # target_query = np.eye(1, visited_units.shape[0], target_unit, dtype=int).flatten()
+            # target_idx = get_indices(dataset_dirty.provenance, target_query)
 
             # Repair the data example.
+            # dataset_dirty.y_train[target_idx] = dataset.y_train[target_idx]
             visited_units[target_units] = True
             dataset_dirty.units_dirty[target_units] = False
 
             # Run the model.
             if eqodds_utility is not None:
-                eqodds_utility_result = eqodds_utility(
+                eqodds = eqodds_utility(
                     dataset_dirty_f.X_train,
                     dataset_dirty.y_train,
                     dataset_dirty_f.X_test,
                     dataset_dirty_f.y_test,
-                    metadata_train=dataset_dirty_f.metadata_train,
-                    metadata_test=dataset_dirty_f.metadata_test,
                 )
-            accuracy_utility_result = accuracy_utility(
-                dataset_dirty_f.X_train,
-                dataset_dirty.y_train,
-                dataset_dirty_f.X_test,
-                dataset_dirty_f.y_test,
-                metadata_train=dataset_dirty_f.metadata_train,
-                metadata_test=dataset_dirty_f.metadata_test,
-            )
-            roc_auc_utility_result = roc_auc_utility(
-                dataset_dirty_f.X_train,
-                dataset_dirty.y_train,
-                dataset_dirty_f.X_test,
-                dataset_dirty_f.y_test,
-                metadata_train=dataset_dirty_f.metadata_train,
-                metadata_test=dataset_dirty_f.metadata_test,
+            accuracy = accuracy_utility(
+                dataset_dirty_f.X_train, dataset_dirty.y_train, dataset_dirty_f.X_test, dataset_dirty_f.y_test
             )
 
+            # self.logger.debug("Dirty units: %.2f", np.sum(dataset_dirty.units_dirty))
+            # self.logger.debug("Same labels: %.2f", np.sum(dataset_dirty.y_train == dataset.y_train))
+
             # Update result table.
-            steps_rel = (i + 1) / float(n_checkpoints)
+            steps_rel = (i + 1) / float(checkpoints)
             repaired = visited_units.sum(dtype=int)
             repaired_rel = repaired / float(n_units)
             discovered = np.logical_and(visited_units, units_dirty).sum(dtype=int)
             discovered_rel = discovered / units_dirty.sum(dtype=float)
             evolution.append(
                 [
                     steps_rel,
-                    eqodds_utility_result.score,
-                    eqodds_utility_result.score,
-                    accuracy_utility_result.score,
-                    accuracy_utility_result.score,
-                    roc_auc_utility_result.score,
-                    roc_auc_utility_result.score,
+                    eqodds,
+                    eqodds,
+                    accuracy,
+                    accuracy,
                     repaired,
                     repaired_rel,
                     discovered,
                     discovered_rel,
                     importance_cputime,
                 ]
             )
 
             # Recompute if needed.
             if importance is not None and self.method == RepairMethod.KNN_Interactive:
                 importance_time_start = process_time_ns()
                 importances = importance.fit(
-                    dataset_dirty.X_train,
-                    dataset_dirty.y_train,
-                    dataset_dirty.metadata_train,
-                    provenance=dataset_dirty.provenance,
-                ).score(dataset.X_val, dataset.y_val, dataset.metadata_val)
+                    dataset_dirty.X_train, dataset_dirty.y_train, provenance=dataset_dirty.provenance
+                ).score(dataset.X_val, dataset.y_val)
                 importance_time_end = process_time_ns()
                 importance_cputime += (importance_time_end - importance_time_start) / 1e9
                 argsorted_importances = (-np.array(importances)).argsort()
                 # argsorted_importances = np.ma.array(importances, mask=visited_units).argsort()
 
             # Update progress bar.
             if progress_bar:
@@ -446,46 +387,39 @@
             evolution,
             columns=[
                 "steps_rel",
                 "eqodds",
                 "eqodds_rel",
                 "accuracy",
                 "accuracy_rel",
-                "roc_auc",
-                "roc_auc_rel",
                 "repaired",
                 "repaired_rel",
                 "discovered",
                 "discovered_rel",
                 "importance_cputime",
             ],
         )
         self._evolution.index.name = "steps"
 
         # Recompute relative equalized odds (if we were keeping track of it).
         if eqodds_utility is not None:
-            eqodds_end = eqodds_utility_result.score
+            assert eqodds is not None and eqodds_start is not None
+            eqodds_end = eqodds
             eqqods_min = min(eqodds_start, eqodds_end)
             eqodds_delta = abs(eqodds_end - eqodds_start)
             self._evolution["eqodds_rel"] = self._evolution["eqodds_rel"].apply(
                 lambda x: (x - eqqods_min) / eqodds_delta
             )
         else:
             # Otherwise drop those columns.
             self._evolution.drop(["eqodds", "eqodds_rel"], axis=1, inplace=True)
 
-        # Recompute relative accuracy and ROC AUC.
-        accuracy_end = accuracy_utility_result.score
+        # Recompute relative accuracy.
+        accuracy_end = accuracy
         accuracy_delta = accuracy_end - accuracy_start
         self._evolution["accuracy_rel"] = self._evolution["accuracy_rel"].apply(
             lambda x: (x - accuracy_start) / accuracy_delta
         )
-        roc_auc_end = roc_auc_utility_result.score
-        roc_auc_min = min(roc_auc_start, roc_auc_end)
-        roc_auc_delta = abs(roc_auc_end - roc_auc_start)
-        self._evolution["roc_auc_rel"] = self._evolution["roc_auc_rel"].apply(
-            lambda x: (x - roc_auc_min) / roc_auc_delta
-        )
 
         # Close progress bar.
         if progress_bar:
             self.progress.close()
```

### Comparing `datascope-experiments-0.0.85/datascope_experiments.egg-info/PKG-INFO` & `datascope-experiments-0.0.9/datascope_experiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascope-experiments
-Version: 0.0.85
+Version: 0.0.9
 Summary: Module for running experiments on top of datascope.
 Home-page: https://ease.ml/datascope/
 Author-email: easeml@ds3lab.com
 License: MIT
 Description: # Experimental toolkit for ease.ml/datascope
         
         [![PyPI version](https://badge.fury.io/py/datascope-experiments.svg)](https://badge.fury.io/py/datascope-experiments)
```

### Comparing `datascope-experiments-0.0.85/setup.py` & `datascope-experiments-0.0.9/setup.py`

 * *Files identical despite different names*

