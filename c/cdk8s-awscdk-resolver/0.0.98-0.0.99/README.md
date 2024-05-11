# Comparing `tmp/cdk8s-awscdk-resolver-0.0.98.tar.gz` & `tmp/cdk8s-awscdk-resolver-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-awscdk-resolver-0.0.98.tar", last modified: Thu May  9 06:13:44 2024, max compression
+gzip compressed data, was "cdk8s-awscdk-resolver-0.0.99.tar", last modified: Sat May 11 06:12:35 2024, max compression
```

## Comparing `cdk8s-awscdk-resolver-0.0.98.tar` & `cdk8s-awscdk-resolver-0.0.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:13:44.467697 cdk8s-awscdk-resolver-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-09 06:13:44.467697 cdk8s-awscdk-resolver-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:13:44.467697 cdk8s-awscdk-resolver-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:13:44.463698 cdk8s-awscdk-resolver-0.0.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:13:44.463698 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:13:44.463698 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   981048 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:13:44.463698 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-09 06:13:44.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-09 06:13:44.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:13:44.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-09 06:13:44.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 06:13:44.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:12:35.728141 cdk8s-awscdk-resolver-0.0.99/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-11 06:12:23.000000 cdk8s-awscdk-resolver-0.0.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 06:12:23.000000 cdk8s-awscdk-resolver-0.0.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-11 06:12:35.728141 cdk8s-awscdk-resolver-0.0.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-11 06:12:23.000000 cdk8s-awscdk-resolver-0.0.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-11 06:12:23.000000 cdk8s-awscdk-resolver-0.0.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 06:12:35.728141 cdk8s-awscdk-resolver-0.0.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-11 06:12:23.000000 cdk8s-awscdk-resolver-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:12:35.724141 cdk8s-awscdk-resolver-0.0.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:12:35.724141 cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-11 06:12:23.000000 cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:12:35.724141 cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-11 06:12:23.000000 cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   981797 2024-05-11 06:12:23.000000 cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 06:12:23.000000 cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 06:12:35.724141 cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-11 06:12:35.000000 cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-11 06:12:35.000000 cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 06:12:35.000000 cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-11 06:12:35.000000 cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 06:12:35.000000 cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver.egg-info/top_level.txt
```

### Comparing `cdk8s-awscdk-resolver-0.0.98/LICENSE` & `cdk8s-awscdk-resolver-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.98/PKG-INFO` & `cdk8s-awscdk-resolver-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-awscdk-resolver
-Version: 0.0.98
+Version: 0.0.99
 Summary: @cdk8s/awscdk-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-awscdk-resolver-0.0.98/README.md` & `cdk8s-awscdk-resolver-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.98/setup.py` & `cdk8s-awscdk-resolver-0.0.99/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-awscdk-resolver",
-    "version": "0.0.98",
+    "version": "0.0.99",
     "description": "@cdk8s/awscdk-resolver",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk8s_awscdk_resolver",
         "cdk8s_awscdk_resolver._jsii"
     ],
     "package_data": {
         "cdk8s_awscdk_resolver._jsii": [
-            "awscdk-resolver@0.0.98.jsii.tgz"
+            "awscdk-resolver@0.0.99.jsii.tgz"
         ],
         "cdk8s_awscdk_resolver": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/__init__.py` & `cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/_jsii/__init__.py` & `cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import cdk8s._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdk8s/awscdk-resolver",
-    "0.0.98",
+    "0.0.99",
     __name__[0:-6],
-    "awscdk-resolver@0.0.98.jsii.tgz",
+    "awscdk-resolver@0.0.99.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO` & `cdk8s-awscdk-resolver-0.0.99/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-awscdk-resolver
-Version: 0.0.98
+Version: 0.0.99
 Summary: @cdk8s/awscdk-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

