# Comparing `tmp/beanhub_import-0.1.5.tar.gz` & `tmp/beanhub_import-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_import-0.1.5.tar", max compression
+gzip compressed data, was "beanhub_import-0.1.6.tar", max compression
```

## Comparing `beanhub_import-0.1.5.tar` & `beanhub_import-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-05-10 05:32:31.216346 beanhub_import-0.1.5/LICENSE
--rw-r--r--   0        0        0    24309 2024-05-10 05:32:31.216346 beanhub_import-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-05-10 05:32:31.224346 beanhub_import-0.1.5/beanhub_import/__init__.py
--rw-r--r--   0        0        0      231 2024-05-10 05:32:31.224346 beanhub_import-0.1.5/beanhub_import/constants.py
--rw-r--r--   0        0        0     4617 2024-05-10 05:32:31.224346 beanhub_import-0.1.5/beanhub_import/data_types.py
--rw-r--r--   0        0        0     7958 2024-05-10 05:32:31.224346 beanhub_import-0.1.5/beanhub_import/post_processor.py
--rw-r--r--   0        0        0    10490 2024-05-10 05:32:31.224346 beanhub_import-0.1.5/beanhub_import/processor.py
--rw-r--r--   0        0        0      276 2024-05-10 05:32:31.224346 beanhub_import-0.1.5/beanhub_import/templates.py
--rw-r--r--   0        0        0      767 2024-05-10 05:32:31.224346 beanhub_import-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    25232 1970-01-01 00:00:00.000000 beanhub_import-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-11 07:46:53.301742 beanhub_import-0.1.6/LICENSE
+-rw-r--r--   0        0        0    24362 2024-05-11 07:46:53.301742 beanhub_import-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/beanhub_import/__init__.py
+-rw-r--r--   0        0        0      231 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/beanhub_import/constants.py
+-rw-r--r--   0        0        0     4617 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/beanhub_import/data_types.py
+-rw-r--r--   0        0        0     7958 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/beanhub_import/post_processor.py
+-rw-r--r--   0        0        0    10490 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/beanhub_import/processor.py
+-rw-r--r--   0        0        0      276 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/beanhub_import/templates.py
+-rw-r--r--   0        0        0      774 2024-05-11 07:46:53.309742 beanhub_import-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    25283 1970-01-01 00:00:00.000000 beanhub_import-0.1.6/PKG-INFO
```

### Comparing `beanhub_import-0.1.5/LICENSE` & `beanhub_import-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.5/README.md` & `beanhub_import-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # beanhub-import [![CircleCI](https://dl.circleci.com/status-badge/img/gh/LaunchPlatform/beanhub-import/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/LaunchPlatform/beanhub-import/tree/master)
 
-Beanhub-import is a simple, declarative, smart, and easy-to-use library for importing extracted transactions from beanhub-extract.
+Beanhub-import is a simple, declarative, smart, and easy-to-use library for importing extracted transactions from [beanhub-extract](https://github.com/LaunchPlatform/beanhub-extract).
 It generates Beancount transactions based on predefined rules.
 
 **Note**: This project is still in early stage, still subject to rapid major changes
 
 ## Features
 
 - **Easy-to-use** - you only need to know a little bit about YAML and Jinja2 template syntax.
@@ -405,15 +405,15 @@
 - name: Ignore unused entries
   match:
     extractor:
       equals: "mercury"
     desc:
       one_of:
       - Mercury Credit
-      - Mercury Checking xx1462
+      - Mercury Checking xx1234
   actions:
     - type: ignore
 ```
 
 ## Sponsor
 
 <p align="center">
```

### Comparing `beanhub_import-0.1.5/beanhub_import/data_types.py` & `beanhub_import-0.1.6/beanhub_import/data_types.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.5/beanhub_import/post_processor.py` & `beanhub_import-0.1.6/beanhub_import/post_processor.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.5/beanhub_import/processor.py` & `beanhub_import-0.1.6/beanhub_import/processor.py`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.5/pyproject.toml` & `beanhub_import-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "beanhub-import"
-version = "0.1.5"
+version = "0.1.6"
 description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pytz = "^2024.1"
+pytz = ">=2023.1,<2025"
 pydantic = ">= 2.0.0, <3.0.0"
 pyyaml = "^6.0.1"
 jinja2 = "^3.1.3"
 beanhub-extract = ">= 0.0.7, <0.1.0"
 beancount-black = ">= 1.0.2, < 1.1.0"
 beancount-parser = ">= 1.2.3, < 1.3.0"
```

### Comparing `beanhub_import-0.1.5/PKG-INFO` & `beanhub_import-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanhub-import
-Version: 0.1.5
+Version: 0.1.6
 Summary: The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,21 +12,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beancount-black (>=1.0.2,<1.1.0)
 Requires-Dist: beancount-parser (>=1.2.3,<1.3.0)
 Requires-Dist: beanhub-extract (>=0.0.7,<0.1.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: pydantic (>=2.0.0,<3.0.0)
-Requires-Dist: pytz (>=2024.1,<2025.0)
+Requires-Dist: pytz (>=2023.1,<2025)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 # beanhub-import [![CircleCI](https://dl.circleci.com/status-badge/img/gh/LaunchPlatform/beanhub-import/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/LaunchPlatform/beanhub-import/tree/master)
 
-Beanhub-import is a simple, declarative, smart, and easy-to-use library for importing extracted transactions from beanhub-extract.
+Beanhub-import is a simple, declarative, smart, and easy-to-use library for importing extracted transactions from [beanhub-extract](https://github.com/LaunchPlatform/beanhub-extract).
 It generates Beancount transactions based on predefined rules.
 
 **Note**: This project is still in early stage, still subject to rapid major changes
 
 ## Features
 
 - **Easy-to-use** - you only need to know a little bit about YAML and Jinja2 template syntax.
@@ -427,15 +427,15 @@
 - name: Ignore unused entries
   match:
     extractor:
       equals: "mercury"
     desc:
       one_of:
       - Mercury Credit
-      - Mercury Checking xx1462
+      - Mercury Checking xx1234
   actions:
     - type: ignore
 ```
 
 ## Sponsor
 
 <p align="center">
```

