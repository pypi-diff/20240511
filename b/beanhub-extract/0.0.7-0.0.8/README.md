# Comparing `tmp/beanhub_extract-0.0.7.tar.gz` & `tmp/beanhub_extract-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_extract-0.0.7.tar", max compression
+gzip compressed data, was "beanhub_extract-0.0.8.tar", max compression
```

## Comparing `beanhub_extract-0.0.7.tar` & `beanhub_extract-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-09 18:30:16.708548 beanhub_extract-0.0.7/LICENSE
--rw-r--r--   0        0        0     2725 2024-05-09 18:30:16.708548 beanhub_extract-0.0.7/README.md
--rw-r--r--   0        0        0        0 2024-05-09 18:30:16.708548 beanhub_extract-0.0.7/beanhub_extract/__init__.py
--rw-r--r--   0        0        0     1996 2024-05-09 18:30:16.708548 beanhub_extract-0.0.7/beanhub_extract/data_types.py
--rw-r--r--   0        0        0      115 2024-05-09 18:30:16.708548 beanhub_extract-0.0.7/beanhub_extract/extractors/__init__.py
--rw-r--r--   0        0        0     2423 2024-05-09 18:30:16.708548 beanhub_extract-0.0.7/beanhub_extract/extractors/mercury.py
--rw-r--r--   0        0        0      977 2024-05-09 18:30:16.708548 beanhub_extract-0.0.7/beanhub_extract/utils.py
--rw-r--r--   0        0        0      578 2024-05-09 18:30:16.708548 beanhub_extract-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 beanhub_extract-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-11 07:51:15.529460 beanhub_extract-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2934 2024-05-11 07:51:15.529460 beanhub_extract-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 07:51:15.533460 beanhub_extract-0.0.8/beanhub_extract/__init__.py
+-rw-r--r--   0        0        0     1996 2024-05-11 07:51:15.533460 beanhub_extract-0.0.8/beanhub_extract/data_types.py
+-rw-r--r--   0        0        0      115 2024-05-11 07:51:15.533460 beanhub_extract-0.0.8/beanhub_extract/extractors/__init__.py
+-rw-r--r--   0        0        0     2423 2024-05-11 07:51:15.533460 beanhub_extract-0.0.8/beanhub_extract/extractors/mercury.py
+-rw-r--r--   0        0        0      977 2024-05-11 07:51:15.533460 beanhub_extract-0.0.8/beanhub_extract/utils.py
+-rw-r--r--   0        0        0      587 2024-05-11 07:51:15.533460 beanhub_extract-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3582 1970-01-01 00:00:00.000000 beanhub_extract-0.0.8/PKG-INFO
```

### Comparing `beanhub_extract-0.0.7/LICENSE` & `beanhub_extract-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.7/README.md` & `beanhub_extract-0.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# beanhub-extract
+# beanhub-extract [![CircleCI](https://dl.circleci.com/status-badge/img/gh/LaunchPlatform/beanhub-extract/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/LaunchPlatform/beanhub-extract/tree/master)
 The simple library for extracting all kind of bank account transaction export files, mostly for [beanhub-import](https://github.com/LaunchPlatform/beanhub-import) to ingest and generate transactions
 
 **Note**: This project is still in early stage, still subject to rapid major changes
 
 ## Why?
 
 Have you ever wondered why each of us has to write our own different Beancount importers for the same bank again and again?
```

#### html2text {}

```diff
@@ -1,17 +1,20 @@
-# beanhub-extract The simple library for extracting all kind of bank account
-transaction export files, mostly for [beanhub-import](https://github.com/
-LaunchPlatform/beanhub-import) to ingest and generate transactions **Note**:
-This project is still in early stage, still subject to rapid major changes ##
-Why? Have you ever wondered why each of us has to write our own different
-Beancount importers for the same bank again and again? Why we cannot use the
-same exporter for the same bank CSV file? One of the biggest problems of the
-original Beancount importer design is that the transaction generation logic is
-coupled with the extract logic, making it hard to reuse. We are addressing the
-problem by creating a library only for extracting bank-exported CSV files into
+# beanhub-extract [![CircleCI](https://dl.circleci.com/status-badge/img/gh/
+LaunchPlatform/beanhub-extract/tree/master.svg?style=svg)](https://
+dl.circleci.com/status-badge/redirect/gh/LaunchPlatform/beanhub-extract/tree/
+master) The simple library for extracting all kind of bank account transaction
+export files, mostly for [beanhub-import](https://github.com/LaunchPlatform/
+beanhub-import) to ingest and generate transactions **Note**: This project is
+still in early stage, still subject to rapid major changes ## Why? Have you
+ever wondered why each of us has to write our own different Beancount importers
+for the same bank again and again? Why we cannot use the same exporter for the
+same bank CSV file? One of the biggest problems of the original Beancount
+importer design is that the transaction generation logic is coupled with the
+extract logic, making it hard to reuse. We are addressing the problem by
+creating a library only for extracting bank-exported CSV files into
 standardized transaction structures to be processed later. Ideally, you should
 be able to import this library and use it to import standardized transactions
 from CSV files exported from any bank in the world. ## Install ```bash pip
 install beanhub-extract ``` ## Example Extracting transactions from the CSV
 file is easy. Simply create the extractor class and make a function call on the
 instance object, which will return a transaction object generator. Like this:
 ```python from beanhub_extract.extractors.mercury import MercuryExtractor with
```

### Comparing `beanhub_extract-0.0.7/beanhub_extract/data_types.py` & `beanhub_extract-0.0.8/beanhub_extract/data_types.py`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.7/beanhub_extract/extractors/mercury.py` & `beanhub_extract-0.0.8/beanhub_extract/extractors/mercury.py`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.7/beanhub_extract/utils.py` & `beanhub_extract-0.0.8/beanhub_extract/utils.py`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.7/pyproject.toml` & `beanhub_extract-0.0.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "beanhub-extract"
-version = "0.0.7"
+version = "0.0.8"
 description = "The simple library for extracting all kind of bank account transaction export files, mostly for beanhub-import to inject and generate transactions"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pytz = "^2024.1"
+pytz = ">= 2023.1, <2025"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.1"
 pytest-mock = "^3.11.1"
```

### Comparing `beanhub_extract-0.0.7/PKG-INFO` & `beanhub_extract-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: beanhub-extract
-Version: 0.0.7
+Version: 0.0.8
 Summary: The simple library for extracting all kind of bank account transaction export files, mostly for beanhub-import to inject and generate transactions
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pytz (>=2024.1,<2025.0)
+Requires-Dist: pytz (>=2023.1,<2025)
 Description-Content-Type: text/markdown
 
-# beanhub-extract
+# beanhub-extract [![CircleCI](https://dl.circleci.com/status-badge/img/gh/LaunchPlatform/beanhub-extract/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/LaunchPlatform/beanhub-extract/tree/master)
 The simple library for extracting all kind of bank account transaction export files, mostly for [beanhub-import](https://github.com/LaunchPlatform/beanhub-import) to ingest and generate transactions
 
 **Note**: This project is still in early stage, still subject to rapid major changes
 
 ## Why?
 
 Have you ever wondered why each of us has to write our own different Beancount importers for the same bank again and again?
```

#### html2text {}

```diff
@@ -1,35 +1,38 @@
-Metadata-Version: 2.1 Name: beanhub-extract Version: 0.0.7 Summary: The simple
+Metadata-Version: 2.1 Name: beanhub-extract Version: 0.0.8 Summary: The simple
 library for extracting all kind of bank account transaction export files,
 mostly for beanhub-import to inject and generate transactions License: MIT
 Author: Fang-Pen Lin Author-email: fangpen@launchplatform.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: pytz (>=2024.1,<2025.0)
-Description-Content-Type: text/markdown # beanhub-extract The simple library
-for extracting all kind of bank account transaction export files, mostly for
-[beanhub-import](https://github.com/LaunchPlatform/beanhub-import) to ingest
-and generate transactions **Note**: This project is still in early stage, still
-subject to rapid major changes ## Why? Have you ever wondered why each of us
-has to write our own different Beancount importers for the same bank again and
-again? Why we cannot use the same exporter for the same bank CSV file? One of
-the biggest problems of the original Beancount importer design is that the
-transaction generation logic is coupled with the extract logic, making it hard
-to reuse. We are addressing the problem by creating a library only for
-extracting bank-exported CSV files into standardized transaction structures to
-be processed later. Ideally, you should be able to import this library and use
-it to import standardized transactions from CSV files exported from any bank in
-the world. ## Install ```bash pip install beanhub-extract ``` ## Example
-Extracting transactions from the CSV file is easy. Simply create the extractor
-class and make a function call on the instance object, which will return a
-transaction object generator. Like this: ```python from
-beanhub_extract.extractors.mercury import MercuryExtractor with open("/path/to/
-my-mercury.csv", "rt") as fo: extractor = MercuryExtractor(fo) for txn in
-extractor(): print(txn) # process your transaction here ``` ## Sponsor
+Programming Language :: Python :: 3.11 Requires-Dist: pytz (>=2023.1,<2025)
+Description-Content-Type: text/markdown # beanhub-extract [![CircleCI](https://
+dl.circleci.com/status-badge/img/gh/LaunchPlatform/beanhub-extract/tree/
+master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/
+LaunchPlatform/beanhub-extract/tree/master) The simple library for extracting
+all kind of bank account transaction export files, mostly for [beanhub-import]
+(https://github.com/LaunchPlatform/beanhub-import) to ingest and generate
+transactions **Note**: This project is still in early stage, still subject to
+rapid major changes ## Why? Have you ever wondered why each of us has to write
+our own different Beancount importers for the same bank again and again? Why we
+cannot use the same exporter for the same bank CSV file? One of the biggest
+problems of the original Beancount importer design is that the transaction
+generation logic is coupled with the extract logic, making it hard to reuse. We
+are addressing the problem by creating a library only for extracting bank-
+exported CSV files into standardized transaction structures to be processed
+later. Ideally, you should be able to import this library and use it to import
+standardized transactions from CSV files exported from any bank in the world.
+## Install ```bash pip install beanhub-extract ``` ## Example Extracting
+transactions from the CSV file is easy. Simply create the extractor class and
+make a function call on the instance object, which will return a transaction
+object generator. Like this: ```python from beanhub_extract.extractors.mercury
+import MercuryExtractor with open("/path/to/my-mercury.csv", "rt") as fo:
+extractor = MercuryExtractor(fo) for txn in extractor(): print(txn) # process
+your transaction here ``` ## Sponsor
                                 _[_B_e_a_n_H_u_b_ _l_o_g_o_]
 A modern accounting book service based on the most popular open source version
 control system [Git](https://git-scm.com/) and text-based double entry
 accounting book software [Beancount](https://beancount.github.io/docs/
 index.html). ## Transaction data object We defined a standardized transaction
 data object to accommodate a transaction statement's most commonly used
 columns. The data object type is a simple immutable Python
```

