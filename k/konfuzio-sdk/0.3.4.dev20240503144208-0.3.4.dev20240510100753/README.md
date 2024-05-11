# Comparing `tmp/konfuzio_sdk-0.3.4.dev20240503144208.tar.gz` & `tmp/konfuzio_sdk-0.3.4.dev20240510100753.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konfuzio_sdk-0.3.4.dev20240503144208.tar", last modified: Sat May  4 03:27:47 2024, max compression
+gzip compressed data, was "konfuzio_sdk-0.3.4.dev20240510100753.tar", last modified: Sat May 11 03:27:43 2024, max compression
```

## Comparing `konfuzio_sdk-0.3.4.dev20240503144208.tar` & `konfuzio_sdk-0.3.4.dev20240510100753.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:27:47.015671 konfuzio_sdk-0.3.4.dev20240503144208/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-04 03:27:47.011671 konfuzio_sdk-0.3.4.dev20240503144208/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:27:47.003671 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   207592 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/settings_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:27:47.007670 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:27:47.007670 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/document_categorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/file_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/image.py
--rw-r--r--   0 runner    (1001) docker     (127)   102313 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/information_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:27:47.011671 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-04 03:27:46.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-04 03:27:46.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 03:27:46.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-04 03:27:46.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-04 03:27:46.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 03:27:46.000000 konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 03:27:47.015671 konfuzio_sdk-0.3.4.dev20240503144208/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:27:47.011671 konfuzio_sdk-0.3.4.dev20240503144208/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    23504 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   168877 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-05-04 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240503144208/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:27:43.970110 konfuzio_sdk-0.3.4.dev20240510100753/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-11 03:27:43.970110 konfuzio_sdk-0.3.4.dev20240510100753/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:27:43.962109 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33566 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   207592 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44747 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27029 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/settings_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:27:43.962109 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13180 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15231 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/paragraph_and_sentence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:27:43.962109 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75617 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/document_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51309 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/file_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102313 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/information_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37377 2024-05-11 03:27:35.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:27:43.966109 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-11 03:27:43.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-11 03:27:43.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:27:43.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-11 03:27:43.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-11 03:27:43.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 03:27:43.000000 konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 03:27:43.970110 konfuzio_sdk-0.3.4.dev20240510100753/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:27:43.966109 konfuzio_sdk-0.3.4.dev20240510100753/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23531 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   169232 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80271 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41449 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9505 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-05-11 03:27:36.000000 konfuzio_sdk-0.3.4.dev20240510100753/tests/test_utils.py
```

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/LICENSE.md` & `konfuzio_sdk-0.3.4.dev20240510100753/LICENSE.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/PKG-INFO` & `konfuzio_sdk-0.3.4.dev20240510100753/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.4.dev20240503144208
+Version: 0.3.4.dev20240510100753
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/README.md` & `konfuzio_sdk-0.3.4.dev20240510100753/README.md`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/api.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/api.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/cli.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/data.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/data.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/evaluate.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/extras.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/normalize.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/regex.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/samples.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/settings_importer.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/settings_importer.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/base.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/paragraph_and_sentence.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/paragraph_and_sentence.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/tokenizer/regex.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/tokenizer/regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/base.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/base.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/document_categorization.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/document_categorization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/file_splitting.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/file_splitting.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/image.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/image.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/information_extraction.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/information_extraction.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/tokenization.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/tokenization.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/trainer/utils.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/urls.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk/utils.py` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/PKG-INFO` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konfuzio_sdk
-Version: 0.3.4.dev20240503144208
+Version: 0.3.4.dev20240510100753
 Summary: Konfuzio Software Development Kit
 Home-page: https://github.com/konfuzio-ai/konfuzio-sdk/
 Author: Helm & Nagel GmbH
 Author-email: info@helm-nagel.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: certifi==2023.7.22
```

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/SOURCES.txt` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/konfuzio_sdk.egg-info/requires.txt` & `konfuzio_sdk-0.3.4.dev20240510100753/konfuzio_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/setup.py` & `konfuzio_sdk-0.3.4.dev20240510100753/setup.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_api.py` & `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,15 @@
             revised=False,
             is_correct=True,
             spans=spans,
         )
 
         assert response.status_code == 201
         annotation = json.loads(response.text)
-        assert delete_document_annotation(annotation['id'])
+        assert delete_document_annotation(annotation['id'], delete_from_database=True)
 
     @unittest.skip(reason='Not supported by Server: https://gitlab.com/konfuzio/objectives/-/issues/8663')
     def test_post_document_annotation_multiline_as_offsets(self):
         """Create a multiline Annotation via API."""
         label_id = 862  # just for testing
         label_set_id = 64  # just for testing
```

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_cli.py` & `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_data.py` & `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -445,14 +445,22 @@
     def test_get_image_jpeg(self):
         """Test that a JPEG image file can be obtained via page.get_image() method."""
         document = Document.from_file(path='tests/test_data/jpg.jpg', project=self.project)
         image = document.pages()[0].get_image()
         assert isinstance(image, PIL.PngImagePlugin.PngImageFile)
         document.delete(delete_online=True)
 
+    @classmethod
+    def tearDownClass(cls) -> None:
+        """Remove any files that might have been left from the test pipeline."""
+        project = Project(id_=TEST_PROJECT_ID, update=True)
+        for document in project._documents:
+            if document.name in os.listdir('tests/test_data/'):
+                document.delete(delete_online=True)
+
 
 class TestOfflineExampleData(unittest.TestCase):
     """Test data features without real data."""
 
     @classmethod
     def setUpClass(cls) -> None:
         """Initialize the test Project."""
```

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_evaluate.py` & `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_extras.py` & `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_extras.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_normalize.py` & `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_normalize.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_regex.py` & `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_samples.py` & `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_urls.py` & `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `konfuzio_sdk-0.3.4.dev20240503144208/tests/test_utils.py` & `konfuzio_sdk-0.3.4.dev20240510100753/tests/test_utils.py`

 * *Files identical despite different names*

