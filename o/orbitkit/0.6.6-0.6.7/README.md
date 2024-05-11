# Comparing `tmp/orbitkit-0.6.6.tar.gz` & `tmp/orbitkit-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orbitkit-0.6.6.tar", last modified: Fri May 10 08:29:50 2024, max compression
+gzip compressed data, was "dist/orbitkit-0.6.7.tar", last modified: Sat May 11 09:01:42 2024, max compression
```

## Comparing `orbitkit-0.6.6.tar` & `orbitkit-0.6.7.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 08:29:50.000000 orbitkit-0.6.6/
--rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.6.6/LICENSE
--rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.6.6/MANIFEST.in
--rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-10 08:29:50.000000 orbitkit-0.6.6/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.6.6/README.md
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit/
--rw-r--r--   0 crown      (501) staff       (20)        6 2024-05-10 08:28:59.000000 orbitkit-0.6.6/orbitkit/VERSION
--rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.6.6/orbitkit/__init__.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit/id_srv/
--rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.6.6/orbitkit/id_srv/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     3598 2023-12-06 02:14:34.000000 orbitkit-0.6.6/orbitkit/id_srv/id_gen.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit/lark_send/
--rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.6.6/orbitkit/lark_send/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     6886 2023-09-11 08:05:37.000000 orbitkit-0.6.6/orbitkit/lark_send/lark.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit/pdf_embedding/
--rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.6/orbitkit/pdf_embedding/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)    10265 2024-01-31 06:10:24.000000 orbitkit-0.6.6/orbitkit/pdf_embedding/pdf_txt_embedding.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit/pdf_extractor/
--rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.6/orbitkit/pdf_extractor/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      898 2023-08-07 08:25:29.000000 orbitkit-0.6.6/orbitkit/pdf_extractor/exceptions.py
--rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.6.6/orbitkit/pdf_extractor/pdf_block_extractor_base.py
--rw-r--r--   0 crown      (501) staff       (20)     6340 2024-01-31 05:10:37.000000 orbitkit-0.6.6/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
--rw-r--r--   0 crown      (501) staff       (20)    13790 2024-01-31 05:10:37.000000 orbitkit-0.6.6/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
--rw-r--r--   0 crown      (501) staff       (20)    12635 2024-01-31 06:10:24.000000 orbitkit-0.6.6/orbitkit/pdf_extractor/pdf_extractor_azure.py
--rw-r--r--   0 crown      (501) staff       (20)    10724 2024-01-31 06:28:50.000000 orbitkit-0.6.6/orbitkit/pdf_extractor/pdf_extractor_orbit.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit/pdf_extractor_simple/
--rw-r--r--   0 crown      (501) staff       (20)     3362 2024-05-10 08:28:59.000000 orbitkit-0.6.6/orbitkit/pdf_extractor_simple/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      785 2024-04-23 09:31:55.000000 orbitkit-0.6.6/orbitkit/pdf_extractor_simple/base.py
--rw-r--r--   0 crown      (501) staff       (20)     4279 2024-05-10 08:28:59.000000 orbitkit-0.6.6/orbitkit/pdf_extractor_simple/cloud_provider.py
--rw-r--r--   0 crown      (501) staff       (20)       59 2024-04-23 05:22:52.000000 orbitkit-0.6.6/orbitkit/pdf_extractor_simple/exceptions.py
--rw-r--r--   0 crown      (501) staff       (20)     8078 2024-05-10 08:28:59.000000 orbitkit-0.6.6/orbitkit/pdf_extractor_simple/extractors.py
--rw-r--r--   0 crown      (501) staff       (20)      687 2024-05-10 07:36:30.000000 orbitkit-0.6.6/orbitkit/pdf_extractor_simple/utils.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit/util/
--rw-r--r--   0 crown      (501) staff       (20)      997 2024-04-25 01:40:35.000000 orbitkit-0.6.6/orbitkit/util/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     2137 2024-04-25 01:41:05.000000 orbitkit-0.6.6/orbitkit/util/common.py
--rw-r--r--   0 crown      (501) staff       (20)      365 2024-04-25 01:29:34.000000 orbitkit-0.6.6/orbitkit/util/util_aliyun.py
--rw-r--r--   0 crown      (501) staff       (20)     1078 2024-05-10 07:19:16.000000 orbitkit-0.6.6/orbitkit/util/util_aliyun_oss_simple.py
--rw-r--r--   0 crown      (501) staff       (20)     2122 2024-01-31 06:27:51.000000 orbitkit-0.6.6/orbitkit/util/util_aws.py
--rw-r--r--   0 crown      (501) staff       (20)     5837 2024-02-21 06:49:24.000000 orbitkit-0.6.6/orbitkit/util/util_aws_s3_wrapper.py
--rw-r--r--   0 crown      (501) staff       (20)     4698 2023-11-24 05:44:22.000000 orbitkit-0.6.6/orbitkit/util/util_date.py
--rw-r--r--   0 crown      (501) staff       (20)      189 2024-01-24 10:42:04.000000 orbitkit-0.6.6/orbitkit/util/util_html.py
--rw-r--r--   0 crown      (501) staff       (20)      751 2023-11-13 08:39:24.000000 orbitkit-0.6.6/orbitkit/util/util_md5.py
--rw-r--r--   0 crown      (501) staff       (20)     2023 2024-04-25 01:40:35.000000 orbitkit-0.6.6/orbitkit/util/util_selenium.py
--rw-r--r--   0 crown      (501) staff       (20)      336 2023-11-13 08:30:33.000000 orbitkit-0.6.6/orbitkit/util/util_simple_timer.py
--rw-r--r--   0 crown      (501) staff       (20)      723 2024-04-25 01:43:47.000000 orbitkit-0.6.6/orbitkit/util/util_str.py
--rw-r--r--   0 crown      (501) staff       (20)    22822 2024-04-29 03:18:06.000000 orbitkit-0.6.6/orbitkit/util/util_type_mapping.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit.egg-info/
--rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit.egg-info/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     1414 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit.egg-info/SOURCES.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit.egg-info/dependency_links.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit.egg-info/not-zip-safe
--rw-r--r--   0 crown      (501) staff       (20)       74 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit.egg-info/requires.txt
--rw-r--r--   0 crown      (501) staff       (20)        9 2024-05-10 08:29:50.000000 orbitkit-0.6.6/orbitkit.egg-info/top_level.txt
--rw-r--r--   0 crown      (501) staff       (20)       38 2024-05-10 08:29:50.000000 orbitkit-0.6.6/setup.cfg
--rw-r--r--   0 crown      (501) staff       (20)     1530 2024-01-24 09:21:31.000000 orbitkit-0.6.6/setup.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/
+-rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.6.7/LICENSE
+-rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.6.7/MANIFEST.in
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-11 09:01:42.000000 orbitkit-0.6.7/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.6.7/README.md
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/
+-rw-r--r--   0 crown      (501) staff       (20)        6 2024-05-11 05:38:59.000000 orbitkit-0.6.7/orbitkit/VERSION
+-rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.6.7/orbitkit/__init__.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/id_srv/
+-rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.6.7/orbitkit/id_srv/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     3598 2023-12-06 02:14:34.000000 orbitkit-0.6.7/orbitkit/id_srv/id_gen.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/lark_send/
+-rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.6.7/orbitkit/lark_send/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     6886 2023-09-11 08:05:37.000000 orbitkit-0.6.7/orbitkit/lark_send/lark.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/pdf_embedding/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.7/orbitkit/pdf_embedding/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)    10265 2024-01-31 06:10:24.000000 orbitkit-0.6.7/orbitkit/pdf_embedding/pdf_txt_embedding.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      898 2023-08-07 08:25:29.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/exceptions.py
+-rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_block_extractor_base.py
+-rw-r--r--   0 crown      (501) staff       (20)     6340 2024-01-31 05:10:37.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
+-rw-r--r--   0 crown      (501) staff       (20)    13790 2024-01-31 05:10:37.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
+-rw-r--r--   0 crown      (501) staff       (20)    12635 2024-01-31 06:10:24.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_extractor_azure.py
+-rw-r--r--   0 crown      (501) staff       (20)    10724 2024-01-31 06:28:50.000000 orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_extractor_orbit.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/
+-rw-r--r--   0 crown      (501) staff       (20)     1231 2024-05-11 05:36:15.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      785 2024-04-23 09:31:55.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/base.py
+-rw-r--r--   0 crown      (501) staff       (20)     4593 2024-05-11 05:36:15.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/cloud_provider.py
+-rw-r--r--   0 crown      (501) staff       (20)     4078 2024-05-11 07:46:00.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/core.py
+-rw-r--r--   0 crown      (501) staff       (20)       59 2024-04-23 05:22:52.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/exceptions.py
+-rw-r--r--   0 crown      (501) staff       (20)     8078 2024-05-10 08:28:59.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/extractors.py
+-rw-r--r--   0 crown      (501) staff       (20)      687 2024-05-10 07:36:30.000000 orbitkit-0.6.7/orbitkit/pdf_extractor_simple/utils.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit/util/
+-rw-r--r--   0 crown      (501) staff       (20)      997 2024-04-25 01:40:35.000000 orbitkit-0.6.7/orbitkit/util/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     2137 2024-04-25 01:41:05.000000 orbitkit-0.6.7/orbitkit/util/common.py
+-rw-r--r--   0 crown      (501) staff       (20)      365 2024-04-25 01:29:34.000000 orbitkit-0.6.7/orbitkit/util/util_aliyun.py
+-rw-r--r--   0 crown      (501) staff       (20)     1000 2024-05-11 08:50:16.000000 orbitkit-0.6.7/orbitkit/util/util_aliyun_oss_simple.py
+-rw-r--r--   0 crown      (501) staff       (20)     2122 2024-01-31 06:27:51.000000 orbitkit-0.6.7/orbitkit/util/util_aws.py
+-rw-r--r--   0 crown      (501) staff       (20)     5837 2024-02-21 06:49:24.000000 orbitkit-0.6.7/orbitkit/util/util_aws_s3_wrapper.py
+-rw-r--r--   0 crown      (501) staff       (20)     4698 2023-11-24 05:44:22.000000 orbitkit-0.6.7/orbitkit/util/util_date.py
+-rw-r--r--   0 crown      (501) staff       (20)      189 2024-01-24 10:42:04.000000 orbitkit-0.6.7/orbitkit/util/util_html.py
+-rw-r--r--   0 crown      (501) staff       (20)      751 2023-11-13 08:39:24.000000 orbitkit-0.6.7/orbitkit/util/util_md5.py
+-rw-r--r--   0 crown      (501) staff       (20)     2023 2024-04-25 01:40:35.000000 orbitkit-0.6.7/orbitkit/util/util_selenium.py
+-rw-r--r--   0 crown      (501) staff       (20)      336 2023-11-13 08:30:33.000000 orbitkit-0.6.7/orbitkit/util/util_simple_timer.py
+-rw-r--r--   0 crown      (501) staff       (20)      723 2024-04-25 01:43:47.000000 orbitkit-0.6.7/orbitkit/util/util_str.py
+-rw-r--r--   0 crown      (501) staff       (20)    22822 2024-04-29 03:18:06.000000 orbitkit-0.6.7/orbitkit/util/util_type_mapping.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1452 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/SOURCES.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/dependency_links.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/not-zip-safe
+-rw-r--r--   0 crown      (501) staff       (20)       74 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/requires.txt
+-rw-r--r--   0 crown      (501) staff       (20)        9 2024-05-11 09:01:42.000000 orbitkit-0.6.7/orbitkit.egg-info/top_level.txt
+-rw-r--r--   0 crown      (501) staff       (20)       38 2024-05-11 09:01:42.000000 orbitkit-0.6.7/setup.cfg
+-rw-r--r--   0 crown      (501) staff       (20)     1530 2024-01-24 09:21:31.000000 orbitkit-0.6.7/setup.py
```

### Comparing `orbitkit-0.6.6/LICENSE` & `orbitkit-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/PKG-INFO` & `orbitkit-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.6.6
+Version: 0.6.7
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.6.6/README.md` & `orbitkit-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/id_srv/id_gen.py` & `orbitkit-0.6.7/orbitkit/id_srv/id_gen.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/lark_send/lark.py` & `orbitkit-0.6.7/orbitkit/lark_send/lark.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/pdf_embedding/pdf_txt_embedding.py` & `orbitkit-0.6.7/orbitkit/pdf_embedding/pdf_txt_embedding.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/pdf_extractor/exceptions.py` & `orbitkit-0.6.7/orbitkit/pdf_extractor/exceptions.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/pdf_extractor/pdf_block_extractor_base.py` & `orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_block_extractor_base.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/pdf_extractor/pdf_block_extractor_v1.py` & `orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_block_extractor_v1.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/pdf_extractor/pdf_block_extractor_v2.py` & `orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_block_extractor_v2.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/pdf_extractor/pdf_extractor_azure.py` & `orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_extractor_azure.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/pdf_extractor/pdf_extractor_orbit.py` & `orbitkit-0.6.7/orbitkit/pdf_extractor/pdf_extractor_orbit.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/pdf_extractor_simple/__init__.py` & `orbitkit-0.6.7/orbitkit/pdf_extractor_simple/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,42 +2,51 @@
 import shutil
 import tempfile
 from typing import List, Optional
 from orbitkit.pdf_extractor_simple.base import CloudObjectProvider, PdfExtractor
 from orbitkit.pdf_extractor_simple.cloud_provider import AwsCloudObjectProvider, OssCloudObjectProvider
 
 
-class ExtractPdfSimpleTxtByCloud:
+class CorePdfExtract:
     cloud_object_provider: CloudObjectProvider = None
     pdf_extractor_list: List[PdfExtractor] = []
 
-    def __init__(self, cloud_path: str, cloud_txt_path: Optional[str] = None, *args, **kwargs):
-        if cloud_txt_path is None:
-            self.cloud_txt_path = cloud_path + ".txt"
-        self.cloud_path = cloud_path
-
-        # FIXME: need to add param validation
-        pass
+    def __init__(self, *args, **kwargs):
+        self.args = args
+        self.kwargs = kwargs
 
-        # Select CloudObjectProvider by protocol
-        self._setup_cloud_object_provider(cloud_path, *args, **kwargs)
-
-    def _setup_cloud_object_provider(self, cloud_path: str, *args, **kwargs):
+    def _setup_cloud_object_provider(self, cloud_path: str):
+        # FIXME: Specific cloud provider could be new() delayed.
         if cloud_path.startswith("s3://"):
-            self.cloud_object_provider = AwsCloudObjectProvider(*args, **kwargs)
+            self.cloud_object_provider = AwsCloudObjectProvider(*self.args, **self.kwargs)
             return
         if cloud_path.startswith("oss://"):
-            self.cloud_object_provider = OssCloudObjectProvider()
+            self.cloud_object_provider = OssCloudObjectProvider(*self.args, **self.kwargs)
             return
         raise Exception("No specific CloudObjectProvider err!")
 
     def add_pdf_extractor(self, pdf_extractor: PdfExtractor):
         self.pdf_extractor_list.append(pdf_extractor)
 
-    def pdf_extract(self, copy_path: str, auto_upload: bool = True):
+    def pdf_extract(self, cloud_path: str,
+                    cloud_txt_path: Optional[str] = None,
+                    copy_path: Optional[str] = None,
+                    auto_upload: bool = True,
+                    return_txt_list: bool = False) -> Optional[list]:
+
+        # Supply cloud_path & cloud_txt_path
+        self.cloud_path = cloud_path
+        if cloud_txt_path is None:
+            self.cloud_txt_path = cloud_path + ".txt"
+        else:
+            self.cloud_txt_path = cloud_txt_path
+
+        # Select CloudObjectProvider by protocol
+        self._setup_cloud_object_provider(cloud_path)
+
         # Create a tmp folder
         with tempfile.TemporaryDirectory() as tmp_dir:
             # Check if the target .txt file exist in cloud
             if self.cloud_object_provider.check_file_exist(self.cloud_txt_path):
                 # Exist then download directly: local_path = tmp_dir + '/' + self.cloud_txt_path.split("/")[-1]
                 self.cloud_object_provider.download_file(cloud_path=self.cloud_txt_path,
                                                          local_path=tmp_dir,
@@ -59,8 +68,19 @@
                         if auto_upload:
                             self.cloud_object_provider.upload_file(self.cloud_txt_path, final_txt_path)
                         break
                 if is_extract_success is False:
                     raise Exception("Failed to extract pdf with given pdf extractor!")
 
             # export copy path
-            shutil.move(final_txt_path, copy_path)
+            if copy_path:
+                shutil.copy(final_txt_path, copy_path)
+
+            # Return list
+            txt_content_list = None
+            if return_txt_list:
+                txt_content_list = []
+                with open(final_txt_path, encoding="utf-8") as ft:
+                    for line in ft.readlines():
+                        txt_content_list.append(line)
+                    return txt_content_list
+            return txt_content_list
```

### Comparing `orbitkit-0.6.6/orbitkit/pdf_extractor_simple/base.py` & `orbitkit-0.6.7/orbitkit/pdf_extractor_simple/base.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/pdf_extractor_simple/cloud_provider.py` & `orbitkit-0.6.7/orbitkit/pdf_extractor_simple/cloud_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import logging
+import threading
 from orbitkit.util import s3_split_path, get_from_dict_or_env, get_content_type_4_filename, oss_split_path
 from orbitkit.pdf_extractor_simple.base import CloudObjectProvider
 
 logger = logging.getLogger(__name__)
 
 try:
     import oss2
@@ -14,15 +15,30 @@
     raise ValueError(
         "Please install below packages before using PDF Extractor function.\n"
         "- boto3\n"
         "- oss2\n"
     )
 
 
+def singleton(cls):
+    instances = {}
+    lock = threading.Lock()
+
+    def get_instance(*args, **kwargs):
+        with lock:
+            if cls not in instances:
+                instances[cls] = cls(*args, **kwargs)
+            return instances[cls]
+
+    return get_instance
+
+
+@singleton
 class AwsCloudObjectProvider(CloudObjectProvider):
+
     def __init__(self, *args, **kwargs):
         aws_access_key_id = get_from_dict_or_env(
             kwargs, "aws_access_key_id", "AWS_ACCESS_KEY_ID",
         )
 
         aws_secret_access_key = get_from_dict_or_env(
             kwargs, "aws_secret_access_key", "AWS_SECRET_ACCESS_KEY",
@@ -62,26 +78,27 @@
 
         self.s3_client.upload_file(local_path,
                                    s3_path_obj["bucket"],
                                    s3_path_obj["store_path"],
                                    ExtraArgs={'ContentType': content_type})
 
 
+@singleton
 class OssCloudObjectProvider(CloudObjectProvider):
     def __init__(self, *args, **kwargs):
         oss_app_id = get_from_dict_or_env(
-            kwargs, "oss_app_id", "OSSAPPID",
+            kwargs, "ossappid", "OSSAPPID",
         )
 
         oss_pwd = get_from_dict_or_env(
-            kwargs, "oss_pwd", "OSSPWD",
+            kwargs, "osspwd", "OSSPWD",
         )
 
         self.oss_endpoint = get_from_dict_or_env(
-            kwargs, "oss_endpoint", "OSSENDPOINT",
+            kwargs, "ossendpoint", "OSSENDPOINT",
         )
 
         self.auth = oss2.Auth(oss_app_id, oss_pwd)
 
     def check_file_exist(self, cloud_path: str) -> bool:
         oss_path_obj = oss_split_path(cloud_path)
         oss_bucket = oss2.Bucket(self.auth, self.oss_endpoint, oss_path_obj["bucket"])
```

### Comparing `orbitkit-0.6.6/orbitkit/pdf_extractor_simple/extractors.py` & `orbitkit-0.6.7/orbitkit/pdf_extractor_simple/extractors.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/pdf_extractor_simple/utils.py` & `orbitkit-0.6.7/orbitkit/pdf_extractor_simple/utils.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/util/__init__.py` & `orbitkit-0.6.7/orbitkit/util/__init__.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/util/common.py` & `orbitkit-0.6.7/orbitkit/util/common.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/util/util_aliyun_oss_simple.py` & `orbitkit-0.6.7/orbitkit/util/util_aliyun_oss_simple.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,11 +32,8 @@
     result = bucket.put_object_from_file(oos_path, local_path)
     if result.status == 200:
         return oos_path
     return None
 
 
 def down_oss(bucket, local_path, oos_path):
-    result = bucket.get_object_to_file(oos_path, local_path)
-    if result.status == 200:
-        return oos_path
-    return None
+    bucket.get_object_to_file(oos_path, local_path)
```

### Comparing `orbitkit-0.6.6/orbitkit/util/util_aws.py` & `orbitkit-0.6.7/orbitkit/util/util_aws.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/util/util_aws_s3_wrapper.py` & `orbitkit-0.6.7/orbitkit/util/util_aws_s3_wrapper.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/util/util_date.py` & `orbitkit-0.6.7/orbitkit/util/util_date.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/util/util_md5.py` & `orbitkit-0.6.7/orbitkit/util/util_md5.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/util/util_selenium.py` & `orbitkit-0.6.7/orbitkit/util/util_selenium.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/util/util_str.py` & `orbitkit-0.6.7/orbitkit/util/util_str.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit/util/util_type_mapping.py` & `orbitkit-0.6.7/orbitkit/util/util_type_mapping.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.6.6/orbitkit.egg-info/PKG-INFO` & `orbitkit-0.6.7/orbitkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.6.6
+Version: 0.6.7
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.6.6/orbitkit.egg-info/SOURCES.txt` & `orbitkit-0.6.7/orbitkit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 orbitkit/pdf_extractor/pdf_block_extractor_v1.py
 orbitkit/pdf_extractor/pdf_block_extractor_v2.py
 orbitkit/pdf_extractor/pdf_extractor_azure.py
 orbitkit/pdf_extractor/pdf_extractor_orbit.py
 orbitkit/pdf_extractor_simple/__init__.py
 orbitkit/pdf_extractor_simple/base.py
 orbitkit/pdf_extractor_simple/cloud_provider.py
+orbitkit/pdf_extractor_simple/core.py
 orbitkit/pdf_extractor_simple/exceptions.py
 orbitkit/pdf_extractor_simple/extractors.py
 orbitkit/pdf_extractor_simple/utils.py
 orbitkit/util/__init__.py
 orbitkit/util/common.py
 orbitkit/util/util_aliyun.py
 orbitkit/util/util_aliyun_oss_simple.py
```

### Comparing `orbitkit-0.6.6/setup.py` & `orbitkit-0.6.7/setup.py`

 * *Files identical despite different names*

