# Comparing `tmp/pysqa-0.1.8.tar.gz` & `tmp/pysqa-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqa-0.1.8.tar", last modified: Mon Dec 11 21:27:29 2023, max compression
+gzip compressed data, was "pysqa-0.1.9.tar", last modified: Mon Jan  1 17:32:49 2024, max compression
```

## Comparing `pysqa-0.1.8.tar` & `pysqa-0.1.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:27:29.768107 pysqa-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-12-11 21:26:22.000000 pysqa-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-11 21:26:22.000000 pysqa-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2023-12-11 21:27:29.768107 pysqa-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2023-12-11 21:26:22.000000 pysqa-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2023-12-11 21:27:27.000000 pysqa-0.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:27:29.760107 pysqa-0.1.8/pysqa/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-12-11 21:27:29.768107 pysqa-0.1.8/pysqa/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:27:29.760107 pysqa-0.1.8/pysqa/executor/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/executor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/executor/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/executor/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/executor/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:27:29.764107 pysqa-0.1.8/pysqa/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/ext/modular.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/ext/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/queueadapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:27:29.764107 pysqa-0.1.8/pysqa/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17823 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/utils/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/utils/queues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:27:29.764107 pysqa-0.1.8/pysqa/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/wrapper/flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/wrapper/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/wrapper/gent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/wrapper/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/wrapper/moab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/wrapper/sge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/wrapper/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2023-12-11 21:26:22.000000 pysqa-0.1.8/pysqa/wrapper/torque.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:27:29.760107 pysqa-0.1.8/pysqa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2023-12-11 21:27:29.000000 pysqa-0.1.8/pysqa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-12-11 21:27:29.000000 pysqa-0.1.8/pysqa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 21:27:29.000000 pysqa-0.1.8/pysqa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-11 21:27:29.000000 pysqa-0.1.8/pysqa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-12-11 21:27:29.000000 pysqa-0.1.8/pysqa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-11 21:27:29.000000 pysqa-0.1.8/pysqa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 21:27:29.768107 pysqa-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-11 21:26:22.000000 pysqa-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 21:27:29.768107 pysqa-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_execute_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_gent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_moab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_scheduler_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_sge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-12-11 21:26:22.000000 pysqa-0.1.8/tests/test_torque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 17:32:49.673530 pysqa-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-01-01 17:31:43.000000 pysqa-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-01 17:31:43.000000 pysqa-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-01-01 17:32:49.673530 pysqa-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-01-01 17:31:43.000000 pysqa-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-01-01 17:32:47.000000 pysqa-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 17:32:49.665530 pysqa-0.1.9/pysqa/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-01 17:32:49.673530 pysqa-0.1.9/pysqa/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 17:32:49.665530 pysqa-0.1.9/pysqa/executor/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/executor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/executor/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/executor/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 17:32:49.665530 pysqa-0.1.9/pysqa/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/ext/modular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/ext/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/queueadapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 17:32:49.669530 pysqa-0.1.9/pysqa/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/utils/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/utils/queues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 17:32:49.669530 pysqa-0.1.9/pysqa/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/wrapper/flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/wrapper/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/wrapper/gent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/wrapper/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/wrapper/moab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/wrapper/sge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/wrapper/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-01-01 17:31:43.000000 pysqa-0.1.9/pysqa/wrapper/torque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 17:32:49.665530 pysqa-0.1.9/pysqa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-01-01 17:32:49.000000 pysqa-0.1.9/pysqa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-01 17:32:49.000000 pysqa-0.1.9/pysqa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-01 17:32:49.000000 pysqa-0.1.9/pysqa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-01 17:32:49.000000 pysqa-0.1.9/pysqa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-01 17:32:49.000000 pysqa-0.1.9/pysqa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-01 17:32:49.000000 pysqa-0.1.9/pysqa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-01 17:32:49.673530 pysqa-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-01 17:31:43.000000 pysqa-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 17:32:49.673530 pysqa-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_execute_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_gent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_moab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_scheduler_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_sge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-01-01 17:31:43.000000 pysqa-0.1.9/tests/test_torque.py
```

### Comparing `pysqa-0.1.8/LICENSE` & `pysqa-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/PKG-INFO` & `pysqa-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqa
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple HPC queuing system adapter for Python on based jinja templates to automate the submission script creation.
 Author-email: Jan Janssen <janssen@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Jan Janssen
         All rights reserved.
         
@@ -52,15 +52,15 @@
 License-File: LICENSE
 Requires-Dist: jinja2<=3.1.2,>=2.11.3
 Requires-Dist: pandas<=2.1.4,>=1.5.3
 Requires-Dist: pyyaml<=6.0.1,>=5.3.1
 Provides-Extra: sge
 Requires-Dist: defusedxml<=0.7.1,>=0.7.0; extra == "sge"
 Provides-Extra: remote
-Requires-Dist: paramiko<=3.3.1,>=2.7.1; extra == "remote"
+Requires-Dist: paramiko<=3.4.0,>=2.7.1; extra == "remote"
 Requires-Dist: tqdm==4.66.1; extra == "remote"
 Provides-Extra: executor
 Requires-Dist: pympipool<=0.7.9,>=0.7.0; extra == "executor"
 Requires-Dist: cloudpickle<=3.0.0,>=2.2.1; extra == "executor"
 
 # pysqa - a simple queue adapter for python
```

### Comparing `pysqa-0.1.8/README.md` & `pysqa-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pyproject.toml` & `pysqa-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 Homepage = "https://github.com/pyiron/pysqa"
 Documentation = "https://pysqa.readthedocs.io"
 Repository = "https://github.com/pyiron/pysqa"
 
 [project.optional-dependencies]
 sge = ["defusedxml>=0.7.0,<=0.7.1"]
 remote = [
-    "paramiko>=2.7.1,<=3.3.1",
+    "paramiko>=2.7.1,<=3.4.0",
     "tqdm==4.66.1",
 ]
 executor = [
     "pympipool>=0.7.0,<=0.7.9",
     "cloudpickle>=2.2.1,<=3.0.0",
 ]
```

### Comparing `pysqa-0.1.8/pysqa/cmd.py` & `pysqa-0.1.9/pysqa/cmd.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/executor/backend.py` & `pysqa-0.1.9/pysqa/executor/backend.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/executor/executor.py` & `pysqa-0.1.9/pysqa/executor/executor.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/executor/helper.py` & `pysqa-0.1.9/pysqa/executor/helper.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/ext/modular.py` & `pysqa-0.1.9/pysqa/ext/modular.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/ext/remote.py` & `pysqa-0.1.9/pysqa/ext/remote.py`

 * *Files 11% similar despite different names*

```diff
@@ -172,14 +172,18 @@
                 ssh = self._open_ssh_connection()
             sftp_client = ssh.open_sftp()
         else:
             sftp_client = sftp
         for file_src, file_dst in tqdm(file_dict.items()):
             if transfer_back:
                 try:
+                    # Check remote file existence.
+                    # If the remote file does not exist, sftp_client.get() will make the local file empty
+                    # sftp_client.stat() can throw an exception early to prevent the execution of sftp_client.get().
+                    sftp_client.stat(file_dst)
                     sftp_client.get(file_dst, file_src)
                 except FileNotFoundError:
                     pass
             else:
                 sftp_client.put(file_src, file_dst)
         if sftp is None:
             sftp_client.close()
```

### Comparing `pysqa-0.1.8/pysqa/queueadapter.py` & `pysqa-0.1.9/pysqa/queueadapter.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/utils/basic.py` & `pysqa-0.1.9/pysqa/utils/basic.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/utils/execute.py` & `pysqa-0.1.9/pysqa/utils/execute.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/utils/queues.py` & `pysqa-0.1.9/pysqa/utils/queues.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/wrapper/flux.py` & `pysqa-0.1.9/pysqa/wrapper/flux.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/wrapper/generic.py` & `pysqa-0.1.9/pysqa/wrapper/generic.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/wrapper/gent.py` & `pysqa-0.1.9/pysqa/wrapper/gent.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/wrapper/lsf.py` & `pysqa-0.1.9/pysqa/wrapper/lsf.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/wrapper/moab.py` & `pysqa-0.1.9/pysqa/wrapper/moab.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/wrapper/sge.py` & `pysqa-0.1.9/pysqa/wrapper/sge.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/wrapper/slurm.py` & `pysqa-0.1.9/pysqa/wrapper/slurm.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa/wrapper/torque.py` & `pysqa-0.1.9/pysqa/wrapper/torque.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/pysqa.egg-info/PKG-INFO` & `pysqa-0.1.9/pysqa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqa
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple HPC queuing system adapter for Python on based jinja templates to automate the submission script creation.
 Author-email: Jan Janssen <janssen@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Jan Janssen
         All rights reserved.
         
@@ -52,15 +52,15 @@
 License-File: LICENSE
 Requires-Dist: jinja2<=3.1.2,>=2.11.3
 Requires-Dist: pandas<=2.1.4,>=1.5.3
 Requires-Dist: pyyaml<=6.0.1,>=5.3.1
 Provides-Extra: sge
 Requires-Dist: defusedxml<=0.7.1,>=0.7.0; extra == "sge"
 Provides-Extra: remote
-Requires-Dist: paramiko<=3.3.1,>=2.7.1; extra == "remote"
+Requires-Dist: paramiko<=3.4.0,>=2.7.1; extra == "remote"
 Requires-Dist: tqdm==4.66.1; extra == "remote"
 Provides-Extra: executor
 Requires-Dist: pympipool<=0.7.9,>=0.7.0; extra == "executor"
 Requires-Dist: cloudpickle<=3.0.0,>=2.2.1; extra == "executor"
 
 # pysqa - a simple queue adapter for python
```

### Comparing `pysqa-0.1.8/pysqa.egg-info/SOURCES.txt` & `pysqa-0.1.9/pysqa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_basic.py` & `pysqa-0.1.9/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_cmd.py` & `pysqa-0.1.9/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_execute_command.py` & `pysqa-0.1.9/tests/test_execute_command.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_executor.py` & `pysqa-0.1.9/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_flux.py` & `pysqa-0.1.9/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_gent.py` & `pysqa-0.1.9/tests/test_gent.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_lsf.py` & `pysqa-0.1.9/tests/test_lsf.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_moab.py` & `pysqa-0.1.9/tests/test_moab.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_multi.py` & `pysqa-0.1.9/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_remote.py` & `pysqa-0.1.9/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_scheduler_commands.py` & `pysqa-0.1.9/tests/test_scheduler_commands.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_sge.py` & `pysqa-0.1.9/tests/test_sge.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_slurm.py` & `pysqa-0.1.9/tests/test_slurm.py`

 * *Files identical despite different names*

### Comparing `pysqa-0.1.8/tests/test_torque.py` & `pysqa-0.1.9/tests/test_torque.py`

 * *Files identical despite different names*

