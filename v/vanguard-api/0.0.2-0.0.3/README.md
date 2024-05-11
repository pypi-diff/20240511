# Comparing `tmp/vanguard_api-0.0.2.tar.gz` & `tmp/vanguard_api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanguard_api-0.0.2.tar", last modified: Sat May 11 01:19:30 2024, max compression
+gzip compressed data, was "vanguard_api-0.0.3.tar", last modified: Sat May 11 01:26:34 2024, max compression
```

## Comparing `vanguard_api-0.0.2.tar` & `vanguard_api-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:19:30.526579 vanguard_api-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-11 01:19:30.526579 vanguard_api-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 01:19:30.526579 vanguard_api-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:19:30.526579 vanguard_api-0.0.2/vanguard/
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/vanguard/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/vanguard/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/vanguard/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-11 01:19:26.000000 vanguard_api-0.0.2/vanguard/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:19:30.526579 vanguard_api-0.0.2/vanguard_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-11 01:19:30.000000 vanguard_api-0.0.2/vanguard_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-11 01:19:30.000000 vanguard_api-0.0.2/vanguard_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:19:30.000000 vanguard_api-0.0.2/vanguard_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 01:19:30.000000 vanguard_api-0.0.2/vanguard_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 01:19:30.000000 vanguard_api-0.0.2/vanguard_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:26:34.664524 vanguard_api-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-11 01:26:30.000000 vanguard_api-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-11 01:26:34.664524 vanguard_api-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-11 01:26:30.000000 vanguard_api-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 01:26:34.664524 vanguard_api-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-11 01:26:30.000000 vanguard_api-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:26:34.660524 vanguard_api-0.0.3/vanguard/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-11 01:26:30.000000 vanguard_api-0.0.3/vanguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-11 01:26:30.000000 vanguard_api-0.0.3/vanguard/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-05-11 01:26:30.000000 vanguard_api-0.0.3/vanguard/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-05-11 01:26:30.000000 vanguard_api-0.0.3/vanguard/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-11 01:26:30.000000 vanguard_api-0.0.3/vanguard/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:26:34.664524 vanguard_api-0.0.3/vanguard_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-11 01:26:34.000000 vanguard_api-0.0.3/vanguard_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-11 01:26:34.000000 vanguard_api-0.0.3/vanguard_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:26:34.000000 vanguard_api-0.0.3/vanguard_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 01:26:34.000000 vanguard_api-0.0.3/vanguard_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 01:26:34.000000 vanguard_api-0.0.3/vanguard_api.egg-info/top_level.txt
```

### Comparing `vanguard_api-0.0.2/LICENSE` & `vanguard_api-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.2/PKG-INFO` & `vanguard_api-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.2.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.3.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

### Comparing `vanguard_api-0.0.2/README.md` & `vanguard_api-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.2/setup.py` & `vanguard_api-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="vanguard-api",
-    version="0.0.2",
+    version="0.0.3",
     author="MaxxRK",
     author_email="maxxrk@pm.me",
     description="An unofficial API for Vanguard Invest",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/MaxxRK/vanguard-api",
-    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.2.tar.gz",
+    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.3.tar.gz",
     keywords=["VANGUARD", "API"],
     install_requires=["playwright", "playwright-stealth"],
     packages=["vanguard"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP :: Session",
```

### Comparing `vanguard_api-0.0.2/vanguard/account.py` & `vanguard_api-0.0.3/vanguard/account.py`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.2/vanguard/order.py` & `vanguard_api-0.0.3/vanguard/order.py`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.2/vanguard/session.py` & `vanguard_api-0.0.3/vanguard/session.py`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.0.2/vanguard_api.egg-info/PKG-INFO` & `vanguard_api-0.0.3/vanguard_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.2.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.0.3.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

