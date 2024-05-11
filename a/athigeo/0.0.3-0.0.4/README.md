# Comparing `tmp/athigeo-0.0.3.tar.gz` & `tmp/athigeo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athigeo-0.0.3.tar", last modified: Wed Apr 24 19:59:50 2024, max compression
+gzip compressed data, was "athigeo-0.0.4.tar", last modified: Sat May 11 12:48:39 2024, max compression
```

## Comparing `athigeo-0.0.3.tar` & `athigeo-0.0.4.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.217353 athigeo-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 19:59:38.000000 athigeo-0.0.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.205354 athigeo-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.209354 athigeo-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.209354 athigeo-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-24 19:59:38.000000 athigeo-0.0.3/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-24 19:59:38.000000 athigeo-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:59:38.000000 athigeo-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 19:59:38.000000 athigeo-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-24 19:59:50.213353 athigeo-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-24 19:59:38.000000 athigeo-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.209354 athigeo-0.0.3/athigeo/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-24 19:59:38.000000 athigeo-0.0.3/athigeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 19:59:38.000000 athigeo-0.0.3/athigeo/athigeo.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-24 19:59:38.000000 athigeo-0.0.3/athigeo/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.213353 athigeo-0.0.3/athigeo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-24 19:59:50.000000 athigeo-0.0.3/athigeo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-24 19:59:50.000000 athigeo-0.0.3/athigeo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:59:50.000000 athigeo-0.0.3/athigeo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 19:59:50.000000 athigeo-0.0.3/athigeo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 19:59:50.000000 athigeo-0.0.3/athigeo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 19:59:50.000000 athigeo-0.0.3/athigeo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.213353 athigeo-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/athigeo.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.213353 athigeo-0.0.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.213353 athigeo-0.0.3/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 19:59:38.000000 athigeo-0.0.3/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-24 19:59:38.000000 athigeo-0.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-24 19:59:38.000000 athigeo-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 19:59:38.000000 athigeo-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-24 19:59:38.000000 athigeo-0.0.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:59:50.217353 athigeo-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:59:50.213353 athigeo-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 19:59:38.000000 athigeo-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-24 19:59:38.000000 athigeo-0.0.3/tests/test_athigeo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.597303 athigeo-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-11 12:48:28.000000 athigeo-0.0.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.589303 athigeo-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.593303 athigeo-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.593303 athigeo-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-11 12:48:28.000000 athigeo-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:48:28.000000 athigeo-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-11 12:48:28.000000 athigeo-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-11 12:48:39.597303 athigeo-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-11 12:48:28.000000 athigeo-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.593303 athigeo-0.0.4/athigeo/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-11 12:48:28.000000 athigeo-0.0.4/athigeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-11 12:48:28.000000 athigeo-0.0.4/athigeo/athigeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-11 12:48:28.000000 athigeo-0.0.4/athigeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-11 12:48:28.000000 athigeo-0.0.4/athigeo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.597303 athigeo-0.0.4/athigeo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-11 12:48:39.000000 athigeo-0.0.4/athigeo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-11 12:48:39.000000 athigeo-0.0.4/athigeo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:48:39.000000 athigeo-0.0.4/athigeo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-11 12:48:39.000000 athigeo-0.0.4/athigeo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-11 12:48:39.000000 athigeo-0.0.4/athigeo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-11 12:48:39.000000 athigeo-0.0.4/athigeo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.597303 athigeo-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/athigeo.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.597303 athigeo-0.0.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/examples/csv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.597303 athigeo-0.0.4/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-11 12:48:28.000000 athigeo-0.0.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-11 12:48:28.000000 athigeo-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 12:48:28.000000 athigeo-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-11 12:48:28.000000 athigeo-0.0.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:48:39.597303 athigeo-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.597303 athigeo-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-11 12:48:28.000000 athigeo-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-11 12:48:28.000000 athigeo-0.0.4/tests/test_athigeo.py
```

### Comparing `athigeo-0.0.3/.github/workflows/docs-build.yml` & `athigeo-0.0.4/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.3/.github/workflows/docs.yml` & `athigeo-0.0.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.3/.github/workflows/installation.yml` & `athigeo-0.0.4/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.3/.github/workflows/macos.yml` & `athigeo-0.0.4/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.3/.github/workflows/pypi.yml` & `athigeo-0.0.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.3/.github/workflows/ubuntu.yml` & `athigeo-0.0.4/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.3/.github/workflows/windows.yml` & `athigeo-0.0.4/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.3/.gitignore` & `athigeo-0.0.4/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 private/
 *.py[cod]
 *$py.class
+*.json
+*.shx
+*.shp
+*.prj
+*.geojson
+*.csv
+*.cpg
+*.dbf
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 env/
```

### Comparing `athigeo-0.0.3/PKG-INFO` & `athigeo-0.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athigeo
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package intro
 Author-email: Dennis Mutai <dennis.mutaigeo@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Dmutai/athigeo
 Keywords: athigeo
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ipyleaflet
+Requires-Dist: pandas
 Provides-Extra: all
 Requires-Dist: athigeo[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # athigeo
```

### Comparing `athigeo-0.0.3/athigeo.egg-info/PKG-INFO` & `athigeo-0.0.4/athigeo.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athigeo
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package intro
 Author-email: Dennis Mutai <dennis.mutaigeo@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Dmutai/athigeo
 Keywords: athigeo
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ipyleaflet
+Requires-Dist: pandas
 Provides-Extra: all
 Requires-Dist: athigeo[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # athigeo
```

### Comparing `athigeo-0.0.3/athigeo.egg-info/SOURCES.txt` & `athigeo-0.0.4/athigeo.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 .github/workflows/macos.yml
 .github/workflows/pypi.yml
 .github/workflows/ubuntu.yml
 .github/workflows/windows.yml
 athigeo/__init__.py
 athigeo/athigeo.py
 athigeo/common.py
+athigeo/utils.py
 athigeo.egg-info/PKG-INFO
 athigeo.egg-info/SOURCES.txt
 athigeo.egg-info/dependency_links.txt
 athigeo.egg-info/entry_points.txt
 athigeo.egg-info/requires.txt
 athigeo.egg-info/top_level.txt
 docs/CNAME
@@ -31,11 +32,13 @@
 docs/changelog.md
 docs/common.md
 docs/contributing.md
 docs/faq.md
 docs/index.md
 docs/installation.md
 docs/usage.md
+docs/utils.md
+docs/examples/csv.ipynb
 docs/examples/intro.ipynb
 docs/overrides/main.html
 tests/__init__.py
 tests/test_athigeo.py
```

### Comparing `athigeo-0.0.3/docs/contributing.md` & `athigeo-0.0.4/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.3/docs/installation.md` & `athigeo-0.0.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.3/mkdocs.yml` & `athigeo-0.0.4/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -77,10 +77,12 @@
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/Dmutai/athigeo/issues
     - Examples:
         - examples/intro.ipynb
+        - examples/csv.ipynb
     - API Reference:
           - athigeo module: athigeo.md
           - common module: common.md
+          - utils module: utils.md
```

### Comparing `athigeo-0.0.3/pyproject.toml` & `athigeo-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "athigeo"
-version = "0.0.3"
+version = "0.0.4"
 dynamic = [
     "dependencies",
 ]
 description = "A python package intro"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.3"
+current_version = "0.0.4"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

