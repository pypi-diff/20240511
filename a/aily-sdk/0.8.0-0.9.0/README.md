# Comparing `tmp/aily_sdk-0.8.0.tar.gz` & `tmp/aily_sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aily_sdk-0.8.0.tar", max compression
+gzip compressed data, was "aily_sdk-0.9.0.tar", max compression
```

## Comparing `aily_sdk-0.8.0.tar` & `aily_sdk-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-01-18 06:26:34.312573 aily_sdk-0.8.0/LICENSE
--rw-r--r--   0        0        0       10 2024-01-18 06:26:34.313383 aily_sdk-0.8.0/README.md
--rw-r--r--   0        0        0        0 2024-01-16 09:55:54.646999 aily_sdk-0.8.0/aily_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-01-15 05:28:16.396456 aily_sdk-0.8.0/aily_sdk/message/__init__.py
--rw-r--r--   0        0        0     1038 2024-01-22 09:16:54.538590 aily_sdk-0.8.0/aily_sdk/message/button.py
--rw-r--r--   0        0        0     5157 2024-01-19 10:22:18.255702 aily_sdk-0.8.0/aily_sdk/message/chart.py
--rw-r--r--   0        0        0     2738 2024-01-22 06:02:02.774816 aily_sdk-0.8.0/aily_sdk/message/field.py
--rw-r--r--   0        0        0     1173 2024-01-22 06:04:43.276430 aily_sdk-0.8.0/aily_sdk/message/record.py
--rw-r--r--   0        0        0      823 2024-01-22 05:54:45.177013 aily_sdk-0.8.0/aily_sdk/message/table.py
--rw-r--r--   0        0        0      191 2024-01-18 09:27:34.885530 aily_sdk-0.8.0/aily_sdk/message/utils.py
--rw-r--r--   0        0        0        0 2024-01-18 08:23:28.467796 aily_sdk-0.8.0/aily_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-01-18 08:48:12.866557 aily_sdk-0.8.0/aily_sdk/util/channel_context.py
--rw-r--r--   0        0        0      279 2024-01-22 09:18:36.241576 aily_sdk-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      408 1970-01-01 00:00:00.000000 aily_sdk-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-18 06:26:34.312573 aily_sdk-0.9.0/LICENSE
+-rw-r--r--   0        0        0       10 2024-01-18 06:26:34.313383 aily_sdk-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2024-01-16 09:55:54.646999 aily_sdk-0.9.0/aily_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-15 05:28:16.396456 aily_sdk-0.9.0/aily_sdk/message/__init__.py
+-rw-r--r--   0        0        0     1038 2024-01-22 09:16:54.538590 aily_sdk-0.9.0/aily_sdk/message/button.py
+-rw-r--r--   0        0        0     5157 2024-01-19 10:22:18.255702 aily_sdk-0.9.0/aily_sdk/message/chart.py
+-rw-r--r--   0        0        0     2738 2024-01-22 06:02:02.774816 aily_sdk-0.9.0/aily_sdk/message/field.py
+-rw-r--r--   0        0        0     1173 2024-01-22 06:04:43.276430 aily_sdk-0.9.0/aily_sdk/message/record.py
+-rw-r--r--   0        0        0      823 2024-01-22 05:54:45.177013 aily_sdk-0.9.0/aily_sdk/message/table.py
+-rw-r--r--   0        0        0      191 2024-01-18 09:27:34.885530 aily_sdk-0.9.0/aily_sdk/message/utils.py
+-rw-r--r--   0        0        0      870 2024-01-29 10:29:20.031304 aily_sdk-0.9.0/aily_sdk/openapi/__init__.py
+-rw-r--r--   0        0        0     3265 2024-01-29 07:40:41.715663 aily_sdk-0.9.0/aily_sdk/openapi/data.py
+-rw-r--r--   0        0        0        0 2024-01-24 09:57:06.915228 aily_sdk-0.9.0/aily_sdk/openapi/intent.py
+-rw-r--r--   0        0        0     1940 2024-01-30 08:23:24.048824 aily_sdk-0.9.0/aily_sdk/openapi/meta.py
+-rw-r--r--   0        0        0        0 2024-01-24 06:38:51.480726 aily_sdk-0.9.0/aily_sdk/openapi/skill.py
+-rw-r--r--   0        0        0        0 2024-01-18 08:23:28.467796 aily_sdk-0.9.0/aily_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-01-18 08:48:12.866557 aily_sdk-0.9.0/aily_sdk/util/channel_context.py
+-rw-r--r--   0        0        0      300 2024-01-30 08:27:42.177451 aily_sdk-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 aily_sdk-0.9.0/PKG-INFO
```

### Comparing `aily_sdk-0.8.0/LICENSE` & `aily_sdk-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aily_sdk-0.8.0/aily_sdk/message/button.py` & `aily_sdk-0.9.0/aily_sdk/message/button.py`

 * *Files identical despite different names*

### Comparing `aily_sdk-0.8.0/aily_sdk/message/chart.py` & `aily_sdk-0.9.0/aily_sdk/message/chart.py`

 * *Files identical despite different names*

### Comparing `aily_sdk-0.8.0/aily_sdk/message/field.py` & `aily_sdk-0.9.0/aily_sdk/message/field.py`

 * *Files identical despite different names*

### Comparing `aily_sdk-0.8.0/aily_sdk/message/record.py` & `aily_sdk-0.9.0/aily_sdk/message/record.py`

 * *Files identical despite different names*

### Comparing `aily_sdk-0.8.0/aily_sdk/message/table.py` & `aily_sdk-0.9.0/aily_sdk/message/table.py`

 * *Files identical despite different names*

