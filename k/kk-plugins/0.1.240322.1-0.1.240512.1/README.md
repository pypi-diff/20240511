# Comparing `tmp/kk-plugins-0.1.240322.1.tar.gz` & `tmp/kk_plugins-0.1.240512.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kk-plugins-0.1.240322.1.tar", last modified: Fri Mar 22 10:15:39 2024, max compression
+gzip compressed data, was "kk_plugins-0.1.240512.1.tar", last modified: Sat May 11 19:15:16 2024, max compression
```

## Comparing `kk-plugins-0.1.240322.1.tar` & `kk_plugins-0.1.240512.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:15:39.912847 kk-plugins-0.1.240322.1/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-22 10:15:39.912847 kk-plugins-0.1.240322.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-22 10:15:29.000000 kk-plugins-0.1.240322.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 10:15:39.912847 kk-plugins-0.1.240322.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-22 10:15:29.000000 kk-plugins-0.1.240322.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:15:39.908847 kk-plugins-0.1.240322.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:15:39.912847 kk-plugins-0.1.240322.1/src/kk_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-22 10:15:29.000000 kk-plugins-0.1.240322.1/src/kk_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-22 10:15:29.000000 kk-plugins-0.1.240322.1/src/kk_plugins/account.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-22 10:15:29.000000 kk-plugins-0.1.240322.1/src/kk_plugins/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-03-22 10:15:29.000000 kk-plugins-0.1.240322.1/src/kk_plugins/compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-03-22 10:15:29.000000 kk-plugins-0.1.240322.1/src/kk_plugins/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-03-22 10:15:29.000000 kk-plugins-0.1.240322.1/src/kk_plugins/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-03-22 10:15:29.000000 kk-plugins-0.1.240322.1/src/kk_plugins/split_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 10:15:39.912847 kk-plugins-0.1.240322.1/src/kk_plugins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-22 10:15:39.000000 kk-plugins-0.1.240322.1/src/kk_plugins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-22 10:15:39.000000 kk-plugins-0.1.240322.1/src/kk_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 10:15:39.000000 kk-plugins-0.1.240322.1/src/kk_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-22 10:15:39.000000 kk-plugins-0.1.240322.1/src/kk_plugins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-22 10:15:39.000000 kk-plugins-0.1.240322.1/src/kk_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:15:16.836480 kk_plugins-0.1.240512.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-11 19:15:16.836480 kk_plugins-0.1.240512.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-11 19:15:08.000000 kk_plugins-0.1.240512.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 19:15:16.836480 kk_plugins-0.1.240512.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-11 19:15:08.000000 kk_plugins-0.1.240512.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:15:16.832480 kk_plugins-0.1.240512.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:15:16.836480 kk_plugins-0.1.240512.1/src/kk_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-11 19:15:08.000000 kk_plugins-0.1.240512.1/src/kk_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-11 19:15:08.000000 kk_plugins-0.1.240512.1/src/kk_plugins/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-11 19:15:08.000000 kk_plugins-0.1.240512.1/src/kk_plugins/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-11 19:15:08.000000 kk_plugins-0.1.240512.1/src/kk_plugins/compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-05-11 19:15:08.000000 kk_plugins-0.1.240512.1/src/kk_plugins/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-11 19:15:08.000000 kk_plugins-0.1.240512.1/src/kk_plugins/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-11 19:15:08.000000 kk_plugins-0.1.240512.1/src/kk_plugins/split_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:15:16.836480 kk_plugins-0.1.240512.1/src/kk_plugins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-11 19:15:16.000000 kk_plugins-0.1.240512.1/src/kk_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-11 19:15:16.000000 kk_plugins-0.1.240512.1/src/kk_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 19:15:16.000000 kk_plugins-0.1.240512.1/src/kk_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-11 19:15:16.000000 kk_plugins-0.1.240512.1/src/kk_plugins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 19:15:16.000000 kk_plugins-0.1.240512.1/src/kk_plugins.egg-info/top_level.txt
```

### Comparing `kk-plugins-0.1.240322.1/PKG-INFO` & `kk_plugins-0.1.240512.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk-plugins
-Version: 0.1.240322.1
+Version: 0.1.240512.1
 Summary: kk plugins
 Home-page: https://github.com/kk-plugins
 License: MIT
 Keywords: kk-plugins
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,12 +17,13 @@
 Requires-Dist: redis~=4.5.4
 Requires-Dist: requests~=2.28.1
 Requires-Dist: pandas~=1.5.3
 Requires-Dist: prettytable~=3.8.0
 Requires-Dist: Jinja2~=3.1.2
 Requires-Dist: setuptools~=60.2.0
 Requires-Dist: xlwings
+Requires-Dist: PyPDF2
 
 # kk plugins
 
 # v0.0.1
 init project
```

### Comparing `kk-plugins-0.1.240322.1/setup.py` & `kk_plugins-0.1.240512.1/setup.py`

 * *Files identical despite different names*

### Comparing `kk-plugins-0.1.240322.1/src/kk_plugins/account.py` & `kk_plugins-0.1.240512.1/src/kk_plugins/account.py`

 * *Files identical despite different names*

### Comparing `kk-plugins-0.1.240322.1/src/kk_plugins/compress.py` & `kk_plugins-0.1.240512.1/src/kk_plugins/compress.py`

 * *Files identical despite different names*

### Comparing `kk-plugins-0.1.240322.1/src/kk_plugins/excel.py` & `kk_plugins-0.1.240512.1/src/kk_plugins/excel.py`

 * *Files identical despite different names*

### Comparing `kk-plugins-0.1.240322.1/src/kk_plugins/project.py` & `kk_plugins-0.1.240512.1/src/kk_plugins/project.py`

 * *Files identical despite different names*

### Comparing `kk-plugins-0.1.240322.1/src/kk_plugins.egg-info/PKG-INFO` & `kk_plugins-0.1.240512.1/src/kk_plugins.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk-plugins
-Version: 0.1.240322.1
+Version: 0.1.240512.1
 Summary: kk plugins
 Home-page: https://github.com/kk-plugins
 License: MIT
 Keywords: kk-plugins
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,12 +17,13 @@
 Requires-Dist: redis~=4.5.4
 Requires-Dist: requests~=2.28.1
 Requires-Dist: pandas~=1.5.3
 Requires-Dist: prettytable~=3.8.0
 Requires-Dist: Jinja2~=3.1.2
 Requires-Dist: setuptools~=60.2.0
 Requires-Dist: xlwings
+Requires-Dist: PyPDF2
 
 # kk plugins
 
 # v0.0.1
 init project
```

