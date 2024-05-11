# Comparing `tmp/sgex-0.7.3.tar.gz` & `tmp/sgex-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgex-0.7.3.tar", last modified: Thu Feb  8 11:05:10 2024, max compression
+gzip compressed data, was "sgex-0.7.4.tar", last modified: Sat May 11 21:05:55 2024, max compression
```

## Comparing `sgex-0.7.3.tar` & `sgex-0.7.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-08 11:05:10.038496 sgex-0.7.3/
--rw-r--r--   0 user      (1000) user      (1000)     1520 2022-01-17 07:52:33.000000 sgex-0.7.3/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     5449 2024-02-08 11:05:10.037496 sgex-0.7.3/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)    17536 2024-02-08 11:01:32.000000 sgex-0.7.3/README.md
--rw-r--r--   0 user      (1000) user      (1000)     2837 2023-11-21 20:07:37.000000 sgex-0.7.3/README_pypi.md
--rw-r--r--   0 user      (1000) user      (1000)     1082 2024-02-08 11:04:14.000000 sgex-0.7.3/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2024-02-08 11:05:10.038496 sgex-0.7.3/setup.cfg
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-08 11:05:10.034496 sgex-0.7.3/sgex/
--rw-r--r--   0 user      (1000) user      (1000)       96 2024-02-08 11:04:14.000000 sgex-0.7.3/sgex/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)    22798 2023-11-21 20:07:37.000000 sgex-0.7.3/sgex/call.py
--rw-r--r--   0 user      (1000) user      (1000)    13749 2023-11-21 20:07:37.000000 sgex-0.7.3/sgex/job.py
--rw-r--r--   0 user      (1000) user      (1000)    10199 2023-11-21 18:31:48.000000 sgex-0.7.3/sgex/query.py
--rw-r--r--   0 user      (1000) user      (1000)     3027 2024-02-08 11:01:32.000000 sgex-0.7.3/sgex/util.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-08 11:05:10.037496 sgex-0.7.3/sgex.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     5449 2024-02-08 11:05:10.000000 sgex-0.7.3/sgex.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      368 2024-02-08 11:05:10.000000 sgex-0.7.3/sgex.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-02-08 11:05:10.000000 sgex-0.7.3/sgex.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       31 2024-02-08 11:05:10.000000 sgex-0.7.3/sgex.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        5 2024-02-08 11:05:10.000000 sgex-0.7.3/sgex.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-02-08 11:05:10.036496 sgex-0.7.3/test/
--rw-r--r--   0 user      (1000) user      (1000)     7889 2023-11-21 20:07:37.000000 sgex-0.7.3/test/test_call_integration.py
--rw-r--r--   0 user      (1000) user      (1000)     6935 2023-11-21 20:07:37.000000 sgex-0.7.3/test/test_job.py
--rw-r--r--   0 user      (1000) user      (1000)    11029 2023-11-21 20:07:37.000000 sgex-0.7.3/test/test_job_integration.py
--rw-r--r--   0 user      (1000) user      (1000)     7531 2023-10-10 15:08:25.000000 sgex-0.7.3/test/test_query.py
--rw-r--r--   0 user      (1000) user      (1000)     1874 2024-02-08 11:01:32.000000 sgex-0.7.3/test/test_util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-11 21:05:55.632025 sgex-0.7.4/
+-rw-r--r--   0 user      (1000) user      (1000)     1520 2022-01-17 07:52:33.000000 sgex-0.7.4/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     5449 2024-05-11 21:05:55.632025 sgex-0.7.4/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)    19841 2024-05-11 21:01:21.000000 sgex-0.7.4/README.md
+-rw-r--r--   0 user      (1000) user      (1000)     2837 2023-11-21 20:07:37.000000 sgex-0.7.4/README_pypi.md
+-rw-r--r--   0 user      (1000) user      (1000)     1082 2024-05-11 21:05:19.000000 sgex-0.7.4/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-05-11 21:05:55.632025 sgex-0.7.4/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-11 21:05:55.630025 sgex-0.7.4/sgex/
+-rw-r--r--   0 user      (1000) user      (1000)       96 2024-05-11 21:05:19.000000 sgex-0.7.4/sgex/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    22798 2023-11-21 20:07:37.000000 sgex-0.7.4/sgex/call.py
+-rw-r--r--   0 user      (1000) user      (1000)    13749 2024-05-11 09:50:38.000000 sgex-0.7.4/sgex/job.py
+-rw-r--r--   0 user      (1000) user      (1000)    10199 2023-11-21 18:31:48.000000 sgex-0.7.4/sgex/query.py
+-rw-r--r--   0 user      (1000) user      (1000)     3027 2024-02-08 11:01:32.000000 sgex-0.7.4/sgex/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-11 21:05:55.631025 sgex-0.7.4/sgex.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     5449 2024-05-11 21:05:55.000000 sgex-0.7.4/sgex.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      368 2024-05-11 21:05:55.000000 sgex-0.7.4/sgex.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-05-11 21:05:55.000000 sgex-0.7.4/sgex.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       31 2024-05-11 21:05:55.000000 sgex-0.7.4/sgex.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        5 2024-05-11 21:05:55.000000 sgex-0.7.4/sgex.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-05-11 21:05:55.631025 sgex-0.7.4/test/
+-rw-r--r--   0 user      (1000) user      (1000)     7889 2023-11-21 20:07:37.000000 sgex-0.7.4/test/test_call_integration.py
+-rw-r--r--   0 user      (1000) user      (1000)     6935 2023-11-21 20:07:37.000000 sgex-0.7.4/test/test_job.py
+-rw-r--r--   0 user      (1000) user      (1000)    11029 2023-11-21 20:07:37.000000 sgex-0.7.4/test/test_job_integration.py
+-rw-r--r--   0 user      (1000) user      (1000)     7531 2023-10-10 15:08:25.000000 sgex-0.7.4/test/test_query.py
+-rw-r--r--   0 user      (1000) user      (1000)     1874 2024-02-08 11:01:32.000000 sgex-0.7.4/test/test_util.py
```

### Comparing `sgex-0.7.3/LICENSE` & `sgex-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sgex-0.7.3/PKG-INFO` & `sgex-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgex
-Version: 0.7.3
+Version: 0.7.4
 Summary: Sketch Grammar Explorer (Sketch Engine API wrapper)
 Author-email: Loryn Isaacs <50170623+engisalor@users.noreply.github.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Loryn Isaacs
         All rights reserved.
```

### Comparing `sgex-0.7.3/README.md` & `sgex-0.7.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,14 @@
 [![License](https://img.shields.io/pypi/l/sgex.svg)](https://github.com/pandas-dev/sgex/blob/main/LICENSE)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6812334.svg)](https://doi.org/10.5281/zenodo.6812334)
 
 ## Introduction
 
 Sketch Grammar Explorer is an API wrapper for [Sketch Engine](https://www.sketchengine.eu/), a corpus management software useful for linguistic research. The goal is to build a flexible scaffold for any kind of programmatic work with Sketch Engine and [NoSketch Engine](https://nlp.fi.muni.cz/trac/noske).
 
-**UPDATE**
-
-SGEX `0.7.0+` is another redesign of the package meant to facilitate enhancements. The workflow is improved and it's streamlined for adapting to SkE's updated API schema. Old methods are deprecated and unavailable in new releases.
-
 ## Installation
 
 Clone SGEX or install it with `pip install sgex` (main dependencies are `pandas pyyaml aiohttp aiofiles`).
 
 Get a [Sketch Engine API key](https://www.sketchengine.eu/documentation/api-documentation/#toggle-id-1). Be sure to reference SkE's documentation and schema:
 
 `wget https://www.sketchengine.eu/apidoc/openapi.yaml -O .openapi.yaml`
@@ -344,14 +340,87 @@
 >>> type(j.errors[0][0])
 <class 'aiohttp.client_exceptions.ServerTimeoutError'>
 
 ```
 
 >Even if a request is timed-out by the client, a server may still try to compute results (and continue taking up resources on a local machine, causing unexpected exceptions).
 
+### Example: make a stratified random sample with a series of API calls
+
+Data from different call types can be utilized together to construct more complex queries and custom operations. For example, the `random sample` feature in Sketch Engine's interface uses simple randomization, yet some analyses might require a stratified sampling technique (taking a separate random sample for each category in a text type). This can be done with the code below.
+
+This includes three API call types:
+
+1. a `CorpInfo` call
+2. a `AttrVals` call
+3. a series of `View` calls (64, requested concurrently)
+
+It retrieves 5 random concordances for each `doc.file` text type in the `susanne` corpus for cases of "the" and a following token.
+
+```py
+>>> from sgex.job import Job
+
+# 1. check the corpus's attributes
+>>> j = Job(params={"call_type": "CorpInfo", "corpname": "susanne", "struct_attr_stats": 1})
+>>> j.run()
+>>> j.data.corpinfo[0].structures_from_json()
+  structure  attribute  size
+0      font       type     2
+0      head       type     2
+0       doc       file    64
+1       doc          n    12
+2       doc  wordcount     1
+
+# 2. get values for one text type
+# (make sure avmaxitems is >= the size of the text type)
+>>> j0 = Job(params={"call_type": "AttrVals", "corpname": "susanne", "avattr": "doc.file", "avmaxitems": 1000000})
+>>> j0.run()
+>>> values = j0.data.attrvals[0].response.json()["suggestions"]
+
+# the query ['a<default_attribute>,"<cql_rule>"', "r<sample_size>"]
+>>> q = [f'alemma,"the" []', "r5"]
+>>> call_template = {
+...    "call_type": "View",
+...    "corpname": "susanne",
+...    "viewmode": "sen",
+...    "pagesize": 1000, # make greater than "r<int>"" to get everything in one request
+...    "attrs": "word,tag,lemma",
+...    "attr_allpos": "all"}
+
+# generate list of calls
+>>> calls = []
+>>> for value in values:
+...    within = f' within <doc file="{value}" />'
+...    calls.append(call_template | {"q": [q[0] + within, q[1]]})
+
+# 3. execute job
+>>> j1 = Job(params=calls, thread=True)
+>>> j1.run()
+
+# process data as needed
+# (print the query for the first sample)
+>>> print(j1.data.view[0].response.json()["request"]["q"])
+['alemma,"the" [] within <doc file="A01" />', 'r5']
+
+# (print the KWICs for the first sample)
+>>> for x in range(5):
+...    kwic = j1.data.view[0].response.json()["Lines"][x]["Kwic"]
+...    tokens = []
+...    for dt in kwic:
+...        if dt["class"] != "attr":
+...            tokens.append(dt["str"].strip())
+...    print(" ".join(tokens))
+the jury
+the Fulton
+the state
+the recommendations
+the jury
+
+```
+
 ## Running as a script
 
 If the repo is cloned and is the current working directory, SGEX can be run as a script as such:
 
 ```sh
 # gets collocation data from the Susanne corpus for the lemma "bird"
 python sgex/job.py -p '{"call_type": "Collx", "corpname": "susanne","q": "alemma,\"bird\""}'
```

### Comparing `sgex-0.7.3/README_pypi.md` & `sgex-0.7.4/README_pypi.md`

 * *Files identical despite different names*

### Comparing `sgex-0.7.3/pyproject.toml` & `sgex-0.7.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sgex"
-version = "0.7.3"  # x-release-please-version
+version = "0.7.4"  # x-release-please-version
 requires-python = ">=3.11"
 authors = [{name="Loryn Isaacs", email="50170623+engisalor@users.noreply.github.com"}]
 description = "Sketch Grammar Explorer (Sketch Engine API wrapper)"
 keywords = [
     "sketch engine",
     "api wrapper",
     "corpus linguistics",
```

### Comparing `sgex-0.7.3/sgex/call.py` & `sgex-0.7.4/sgex/call.py`

 * *Files identical despite different names*

### Comparing `sgex-0.7.3/sgex/job.py` & `sgex-0.7.4/sgex/job.py`

 * *Files identical despite different names*

### Comparing `sgex-0.7.3/sgex/query.py` & `sgex-0.7.4/sgex/query.py`

 * *Files identical despite different names*

### Comparing `sgex-0.7.3/sgex/util.py` & `sgex-0.7.4/sgex/util.py`

 * *Files identical despite different names*

### Comparing `sgex-0.7.3/sgex.egg-info/PKG-INFO` & `sgex-0.7.4/sgex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgex
-Version: 0.7.3
+Version: 0.7.4
 Summary: Sketch Grammar Explorer (Sketch Engine API wrapper)
 Author-email: Loryn Isaacs <50170623+engisalor@users.noreply.github.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Loryn Isaacs
         All rights reserved.
```

### Comparing `sgex-0.7.3/test/test_call_integration.py` & `sgex-0.7.4/test/test_call_integration.py`

 * *Files identical despite different names*

### Comparing `sgex-0.7.3/test/test_job.py` & `sgex-0.7.4/test/test_job.py`

 * *Files identical despite different names*

### Comparing `sgex-0.7.3/test/test_job_integration.py` & `sgex-0.7.4/test/test_job_integration.py`

 * *Files identical despite different names*

### Comparing `sgex-0.7.3/test/test_query.py` & `sgex-0.7.4/test/test_query.py`

 * *Files identical despite different names*

### Comparing `sgex-0.7.3/test/test_util.py` & `sgex-0.7.4/test/test_util.py`

 * *Files identical despite different names*

