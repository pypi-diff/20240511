# Comparing `tmp/mov_cli_test-1.1.4.tar.gz` & `tmp/mov_cli_test-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli_test-1.1.4.tar", last modified: Thu Apr 25 01:49:59 2024, max compression
+gzip compressed data, was "mov_cli_test-1.1.5.tar", last modified: Sat May 11 19:41:16 2024, max compression
```

## Comparing `mov_cli_test-1.1.4.tar` & `mov_cli_test-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 01:49:59.291343 mov_cli_test-1.1.4/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1062 2024-03-02 20:16:40.000000 mov_cli_test-1.1.4/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2959 2024-04-25 01:49:59.291343 mov_cli_test-1.1.4/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      532 2024-03-26 18:16:37.000000 mov_cli_test-1.1.4/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 01:49:59.288010 mov_cli_test-1.1.4/mov_cli_test/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      350 2024-04-25 01:49:27.000000 mov_cli_test-1.1.4/mov_cli_test/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4732 2024-04-25 01:49:23.000000 mov_cli_test-1.1.4/mov_cli_test/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-25 01:49:59.291343 mov_cli_test-1.1.4/mov_cli_test.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2959 2024-04-25 01:49:59.000000 mov_cli_test-1.1.4/mov_cli_test.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      260 2024-04-25 01:49:59.000000 mov_cli_test-1.1.4/mov_cli_test.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-25 01:49:59.000000 mov_cli_test-1.1.4/mov_cli_test.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)      114 2024-04-25 01:49:59.000000 mov_cli_test-1.1.4/mov_cli_test.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       13 2024-04-25 01:49:59.000000 mov_cli_test-1.1.4/mov_cli_test.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1395 2024-03-26 17:26:10.000000 mov_cli_test-1.1.4/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-25 01:49:59.291343 mov_cli_test-1.1.4/setup.cfg
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-11 19:41:16.897625 mov_cli_test-1.1.5/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1062 2024-05-11 19:41:05.000000 mov_cli_test-1.1.5/LICENSE
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2962 2024-05-11 19:41:16.897625 mov_cli_test-1.1.5/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      532 2024-05-11 19:41:05.000000 mov_cli_test-1.1.5/README.md
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-11 19:41:16.894291 mov_cli_test-1.1.5/mov_cli_test/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      350 2024-05-11 19:41:05.000000 mov_cli_test-1.1.5/mov_cli_test/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     4735 2024-05-11 19:41:05.000000 mov_cli_test-1.1.5/mov_cli_test/scraper.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-11 19:41:16.894291 mov_cli_test-1.1.5/mov_cli_test.egg-info/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2962 2024-05-11 19:41:16.000000 mov_cli_test-1.1.5/mov_cli_test.egg-info/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      260 2024-05-11 19:41:16.000000 mov_cli_test-1.1.5/mov_cli_test.egg-info/SOURCES.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-05-11 19:41:16.000000 mov_cli_test-1.1.5/mov_cli_test.egg-info/dependency_links.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      117 2024-05-11 19:41:16.000000 mov_cli_test-1.1.5/mov_cli_test.egg-info/requires.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       13 2024-05-11 19:41:16.000000 mov_cli_test-1.1.5/mov_cli_test.egg-info/top_level.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1398 2024-05-11 19:41:05.000000 mov_cli_test-1.1.5/pyproject.toml
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-05-11 19:41:16.897625 mov_cli_test-1.1.5/setup.cfg
```

### Comparing `mov_cli_test-1.1.4/LICENSE` & `mov_cli_test-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli_test-1.1.4/PKG-INFO` & `mov_cli_test-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-test
-Version: 1.1.4
+Version: 1.1.5
 Summary: A mov-cli plugin that let's you test mov-cli's capabilities by watching free films and animations in the creative commons.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 Goldy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,15 +38,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: mov-cli>=4.2
-Requires-Dist: pytube
+Requires-Dist: pytubefix
 Requires-Dist: devgoldyutils>=2.5.8
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
```

### Comparing `mov_cli_test-1.1.4/README.md` & `mov_cli_test-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli_test-1.1.4/mov_cli_test/scraper.py` & `mov_cli_test-1.1.5/mov_cli_test/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 if TYPE_CHECKING:
     from typing import Iterable, Optional, Dict
 
     from mov_cli import Config
     from mov_cli.http_client import HTTPClient
     from mov_cli.scraper import ScraperOptionsT
 
-from pytube import YouTube
+from pytubefix import YouTube
 from devgoldyutils import Colours
 
 from mov_cli.utils import EpisodeSelector
 from mov_cli import Scraper, Multi, Single, Metadata, MetadataType
 
 __all__ = ("TestScraper",)
```

### Comparing `mov_cli_test-1.1.4/mov_cli_test.egg-info/PKG-INFO` & `mov_cli_test-1.1.5/mov_cli_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-test
-Version: 1.1.4
+Version: 1.1.5
 Summary: A mov-cli plugin that let's you test mov-cli's capabilities by watching free films and animations in the creative commons.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 Goldy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,15 +38,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: mov-cli>=4.2
-Requires-Dist: pytube
+Requires-Dist: pytubefix
 Requires-Dist: devgoldyutils>=2.5.8
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
```

### Comparing `mov_cli_test-1.1.4/pyproject.toml` & `mov_cli_test-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 	'Programming Language :: Python :: 3.11'
 ]
 dependencies = [
     "requests",
     "importlib-metadata; python_version<'3.8'",
 
     "mov-cli>=4.2",
-    "pytube",
+    "pytubefix",
     "devgoldyutils>=2.5.8"
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
```

