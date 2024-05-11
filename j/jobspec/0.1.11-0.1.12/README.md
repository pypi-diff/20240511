# Comparing `tmp/jobspec-0.1.11.tar.gz` & `tmp/jobspec-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobspec-0.1.11.tar", last modified: Fri May 10 06:00:37 2024, max compression
+gzip compressed data, was "jobspec-0.1.12.tar", last modified: Sat May 11 17:25:02 2024, max compression
```

## Comparing `jobspec-0.1.11.tar` & `jobspec-0.1.12.tar`

### file list

```diff
@@ -1,49 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.473936 jobspec-0.1.11/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-10 06:00:21.000000 jobspec-0.1.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 06:00:21.000000 jobspec-0.1.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-10 06:00:21.000000 jobspec-0.1.11/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-10 06:00:37.473936 jobspec-0.1.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-10 06:00:21.000000 jobspec-0.1.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.469936 jobspec-0.1.11/jobspec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.469936 jobspec-0.1.11/jobspec/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.469936 jobspec-0.1.11/jobspec/core/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/core/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/core/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.469936 jobspec-0.1.11/jobspec/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/plugin/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.469936 jobspec-0.1.11/jobspec/steps/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/steps/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/steps/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/steps/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/steps/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.473936 jobspec-0.1.11/jobspec/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.473936 jobspec-0.1.11/jobspec/transformer/flux/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/transformer/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/transformer/flux/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/transformer/flux/workload.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/transformer/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-10 06:00:21.000000 jobspec-0.1.11/jobspec/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:00:37.473936 jobspec-0.1.11/jobspec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 06:00:37.000000 jobspec-0.1.11/jobspec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-10 06:00:21.000000 jobspec-0.1.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 06:00:37.473936 jobspec-0.1.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-10 06:00:21.000000 jobspec-0.1.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:25:02.989083 jobspec-0.1.12/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-11 17:24:46.000000 jobspec-0.1.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-11 17:24:46.000000 jobspec-0.1.12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-11 17:24:46.000000 jobspec-0.1.12/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-11 17:25:02.989083 jobspec-0.1.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-11 17:24:46.000000 jobspec-0.1.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:25:02.985083 jobspec-0.1.12/jobspec/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:25:02.985083 jobspec-0.1.12/jobspec/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:25:02.985083 jobspec-0.1.12/jobspec/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/core/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:25:02.989083 jobspec-0.1.12/jobspec/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/logger/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:25:02.989083 jobspec-0.1.12/jobspec/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/plugin/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:25:02.989083 jobspec-0.1.12/jobspec/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/steps/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/steps/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/steps/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/steps/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:25:02.989083 jobspec-0.1.12/jobspec/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:25:02.989083 jobspec-0.1.12/jobspec/transformer/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/transformer/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/transformer/flux/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/transformer/flux/workload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/transformer/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-11 17:24:46.000000 jobspec-0.1.12/jobspec/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:25:02.989083 jobspec-0.1.12/jobspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-11 17:25:02.000000 jobspec-0.1.12/jobspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-11 17:25:02.000000 jobspec-0.1.12/jobspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 17:25:02.000000 jobspec-0.1.12/jobspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-11 17:25:02.000000 jobspec-0.1.12/jobspec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 17:25:02.000000 jobspec-0.1.12/jobspec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-11 17:25:02.000000 jobspec-0.1.12/jobspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-11 17:25:02.000000 jobspec-0.1.12/jobspec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-11 17:24:46.000000 jobspec-0.1.12/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-11 17:25:02.989083 jobspec-0.1.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-11 17:24:46.000000 jobspec-0.1.12/setup.py
```

### Comparing `jobspec-0.1.11/LICENSE` & `jobspec-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/NOTICE` & `jobspec-0.1.12/NOTICE`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/PKG-INFO` & `jobspec-0.1.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobspec
-Version: 0.1.11
+Version: 0.1.12
 Summary: Jobspec specification and translation layer for cluster work
 Home-page: https://github.com/compspec/jobspec
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cluster,orchestration,transformer,jobspec,flux
```

### Comparing `jobspec-0.1.11/README.md` & `jobspec-0.1.12/README.md`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/jobspec/cli/__init__.py` & `jobspec-0.1.12/jobspec/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/jobspec/cli/run.py` & `jobspec-0.1.12/jobspec/cli/run.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/jobspec/core/base.py` & `jobspec-0.1.12/jobspec/core/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,28 +39,31 @@
         """
         if not attrs:
             return
         self.data.update(attrs)
 
     def load(self, filename):
         """
-        Load the jobspec
+        Load the jobspec (from file or as string)
         """
         # Case 1: given a raw filename
         if isinstance(filename, str) and os.path.exists(filename):
             self.filename = os.path.abspath(filename)
 
             try:
                 self.data = utils.read_json(self.filename)
             except:
                 self.data = utils.read_yaml(self.filename)
 
         # Case 2: jobspec as dict (that we just want to validate)
         elif isinstance(filename, dict):
             self.data = filename
-        # Case 3: jobspec as string
+        # Case 3: jobspec as string for json or yaml
         else:
-            self.data = json.loads(filename)
+            try:
+                self.data = json.loads(filename)
+            except:
+                self.data = yaml.load(filename)
 
         # Case 4: wtf are you giving me? :X
         if not self.data:
             raise ValueError("Unrecognized input format for {self.__class__.__name__}.")
```

### Comparing `jobspec-0.1.11/jobspec/core/core.py` & `jobspec-0.1.12/jobspec/core/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import copy
 
 import jsonschema
 
 import jobspec.schema as schema
+from jobspec.logger.generate import generate_name
 
 from .base import ResourceBase
 from .resources import find_resources, to_jobspec
 
 
 class Jobspec(ResourceBase):
-    def __init__(self, filename, validate=True, schema=schema.jobspec_nextgen):
+    def __init__(self, filename, validate=True, name=None, schema=schema.jobspec_nextgen):
         """
         Load in and validate a Jobspec
         """
+        self.name = name or generate_name()
+
         # This should typically be loaded from jobspec.core
         if not hasattr(self, "schema") or not self.schema:
             self.schema = schema
-        self.filename = filename
         self.data = None
         self.load(filename)
         if validate:
             self.validate()
 
     def validate(self):
         """
```

### Comparing `jobspec-0.1.11/jobspec/core/resources.py` & `jobspec-0.1.12/jobspec/core/resources.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/jobspec/logger.py` & `jobspec-0.1.12/jobspec/logger/logger.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/jobspec/plugin/registry.py` & `jobspec-0.1.12/jobspec/plugin/registry.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/jobspec/runner.py` & `jobspec-0.1.12/jobspec/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,9 +72,8 @@
     def load_jobspec(self, filename):
         """
         Load and transform a jobspec.
 
         This function should be able to load it in some raw format
         and convert into correct directives given the transformer.
         """
-        filename = os.path.abspath(filename)
         return js.Jobspec(filename)
```

### Comparing `jobspec-0.1.11/jobspec/schema.py` & `jobspec-0.1.12/jobspec/schema.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/jobspec/steps/base.py` & `jobspec-0.1.12/jobspec/steps/base.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/jobspec/steps/fileio.py` & `jobspec-0.1.12/jobspec/steps/fileio.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/jobspec/steps/runner.py` & `jobspec-0.1.12/jobspec/steps/runner.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/jobspec/transformer/flux/steps.py` & `jobspec-0.1.12/jobspec/transformer/flux/steps.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/jobspec/transformer/flux/workload.py` & `jobspec-0.1.12/jobspec/transformer/flux/workload.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/jobspec/utils.py` & `jobspec-0.1.12/jobspec/utils.py`

 * *Files identical despite different names*

### Comparing `jobspec-0.1.11/jobspec/version.py` & `jobspec-0.1.12/jobspec/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.11"
+__version__ = "0.1.12"
 AUTHOR = "Vanessa Sochat"
 AUTHOR_EMAIL = "vsoch@users.noreply.github.com"
 NAME = "jobspec"
 PACKAGE_URL = "https://github.com/compspec/jobspec"
 KEYWORDS = "cluster, orchestration, transformer, jobspec, flux"
 DESCRIPTION = "Jobspec specification and translation layer for cluster work"
 LICENSE = "LICENSE"
```

### Comparing `jobspec-0.1.11/jobspec.egg-info/PKG-INFO` & `jobspec-0.1.12/jobspec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobspec
-Version: 0.1.11
+Version: 0.1.12
 Summary: Jobspec specification and translation layer for cluster work
 Home-page: https://github.com/compspec/jobspec
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cluster,orchestration,transformer,jobspec,flux
```

### Comparing `jobspec-0.1.11/jobspec.egg-info/SOURCES.txt` & `jobspec-0.1.12/jobspec.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 NOTICE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 jobspec/__init__.py
 jobspec/defaults.py
-jobspec/logger.py
 jobspec/runner.py
 jobspec/schema.py
 jobspec/utils.py
 jobspec/version.py
 jobspec.egg-info/PKG-INFO
 jobspec.egg-info/SOURCES.txt
 jobspec.egg-info/dependency_links.txt
@@ -19,16 +18,20 @@
 jobspec.egg-info/not-zip-safe
 jobspec.egg-info/requires.txt
 jobspec.egg-info/top_level.txt
 jobspec/cli/__init__.py
 jobspec/cli/run.py
 jobspec/core/__init__.py
 jobspec/core/base.py
+jobspec/core/converter.py
 jobspec/core/core.py
 jobspec/core/resources.py
+jobspec/logger/__init__.py
+jobspec/logger/generate.py
+jobspec/logger/logger.py
 jobspec/plugin/__init__.py
 jobspec/plugin/registry.py
 jobspec/steps/__init__.py
 jobspec/steps/base.py
 jobspec/steps/empty.py
 jobspec/steps/fileio.py
 jobspec/steps/runner.py
```

### Comparing `jobspec-0.1.11/setup.py` & `jobspec-0.1.12/setup.py`

 * *Files identical despite different names*

