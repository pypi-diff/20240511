# Comparing `tmp/flops_utils-0.3.7.tar.gz` & `tmp/flops_utils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flops_utils-0.3.7.tar", max compression
+gzip compressed data, was "flops_utils-0.4.0.tar", max compression
```

## Comparing `flops_utils-0.3.7.tar` & `flops_utils-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.3.7/README.md
--rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.3.7/flops_utils/logging.py
--rw-r--r--   0        0        0      782 2024-05-05 12:55:14.703088 flops_utils-0.3.7/flops_utils/ml_model_flavor_wrapper.py
--rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.3.7/flops_utils/ml_repo_files_wrapper.py
--rw-r--r--   0        0        0     2632 2024-05-05 10:09:52.795212 flops_utils-0.3.7/flops_utils/ml_repo_templates.py
--rw-r--r--   0        0        0     1441 2024-05-11 09:55:30.969946 flops_utils-0.3.7/flops_utils/notifications.py
--rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.3.7/flops_utils/types.py
--rw-r--r--   0        0        0      435 2024-05-11 09:55:37.385946 flops_utils-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 flops_utils-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0        5 2024-04-24 16:17:22.069103 flops_utils-0.4.0/README.md
+-rw-r--r--   0        0        0     1700 2024-04-25 13:42:32.054488 flops_utils-0.4.0/flops_utils/logging.py
+-rw-r--r--   0        0        0      782 2024-05-05 12:55:14.703088 flops_utils-0.4.0/flops_utils/ml_model_flavor_wrapper.py
+-rw-r--r--   0        0        0      500 2024-05-04 14:02:04.855413 flops_utils-0.4.0/flops_utils/ml_repo_files_wrapper.py
+-rw-r--r--   0        0        0     2632 2024-05-05 10:09:52.795212 flops_utils-0.4.0/flops_utils/ml_repo_templates.py
+-rw-r--r--   0        0        0     1441 2024-05-11 09:55:30.969946 flops_utils-0.4.0/flops_utils/notifications.py
+-rw-r--r--   0        0        0     2180 2024-05-11 18:03:51.996035 flops_utils-0.4.0/flops_utils/timer.py
+-rw-r--r--   0        0        0      395 2024-05-03 14:36:34.589614 flops_utils-0.4.0/flops_utils/types.py
+-rw-r--r--   0        0        0      455 2024-05-11 18:06:16.740038 flops_utils-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 flops_utils-0.4.0/PKG-INFO
```

### Comparing `flops_utils-0.3.7/flops_utils/logging.py` & `flops_utils-0.4.0/flops_utils/logging.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.3.7/flops_utils/ml_model_flavor_wrapper.py` & `flops_utils-0.4.0/flops_utils/ml_model_flavor_wrapper.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.3.7/flops_utils/ml_repo_templates.py` & `flops_utils-0.4.0/flops_utils/ml_repo_templates.py`

 * *Files identical despite different names*

### Comparing `flops_utils-0.3.7/flops_utils/notifications.py` & `flops_utils-0.4.0/flops_utils/notifications.py`

 * *Files identical despite different names*

