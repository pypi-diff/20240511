# Comparing `tmp/HiYaPyCo-0.5.5.tar.gz` & `tmp/HiYaPyCo-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HiYaPyCo-0.5.5.tar", last modified: Sat Apr 13 09:12:19 2024, max compression
+gzip compressed data, was "HiYaPyCo-0.5.6.tar", last modified: Sat May 11 05:03:28 2024, max compression
```

## Comparing `HiYaPyCo-0.5.5.tar` & `HiYaPyCo-0.5.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-04-13 09:12:19.201440 HiYaPyCo-0.5.5/
-drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-04-13 09:12:19.197439 HiYaPyCo-0.5.5/HiYaPyCo.egg-info/
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    11195 2024-04-13 09:12:19.000000 HiYaPyCo-0.5.5/HiYaPyCo.egg-info/PKG-INFO
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)      489 2024-04-13 09:12:19.000000 HiYaPyCo-0.5.5/HiYaPyCo.egg-info/SOURCES.txt
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)        1 2024-04-13 09:12:19.000000 HiYaPyCo-0.5.5/HiYaPyCo.egg-info/dependency_links.txt
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)       34 2024-04-13 09:12:19.000000 HiYaPyCo-0.5.5/HiYaPyCo.egg-info/requires.txt
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)        9 2024-04-13 09:12:19.000000 HiYaPyCo-0.5.5/HiYaPyCo.egg-info/top_level.txt
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    35141 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/LICENSE
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)       36 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/MANIFEST.in
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    11195 2024-04-13 09:12:19.201440 HiYaPyCo-0.5.5/PKG-INFO
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    10404 2024-04-13 08:55:30.000000 HiYaPyCo-0.5.5/README.rst
-drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-04-13 09:12:19.197439 HiYaPyCo-0.5.5/hiyapyco/
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)    21689 2024-04-13 08:37:16.000000 HiYaPyCo-0.5.5/hiyapyco/__init__.py
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)     2604 2024-04-13 08:37:32.000000 HiYaPyCo-0.5.5/hiyapyco/odyldo.py
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)       16 2024-04-13 08:39:01.000000 HiYaPyCo-0.5.5/hiyapyco/version.py
--rw-r--r--   0 zerwes    (1000) zerwes    (1000)      109 2024-04-13 09:12:19.201440 HiYaPyCo-0.5.5/setup.cfg
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1357 2024-04-13 08:39:36.000000 HiYaPyCo-0.5.5/setup.py
-drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-04-13 09:12:19.201440 HiYaPyCo-0.5.5/test/
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1739 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_castinterpolated.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     3021 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_interpolation.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1734 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_interpolationunicode.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     4905 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_invocation.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     5075 2023-11-29 07:36:03.000000 HiYaPyCo-0.5.5/test/test_merge.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     4313 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_missingfiles.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1753 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_multiple.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     2836 2022-05-04 08:47:46.000000 HiYaPyCo-0.5.5/test/test_odict.py
--rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1913 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.5/test/test_simple.py
+drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-05-11 05:03:28.522827 HiYaPyCo-0.5.6/
+drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-05-11 05:03:28.518827 HiYaPyCo-0.5.6/HiYaPyCo.egg-info/
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    11283 2024-05-11 05:03:28.000000 HiYaPyCo-0.5.6/HiYaPyCo.egg-info/PKG-INFO
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)      489 2024-05-11 05:03:28.000000 HiYaPyCo-0.5.6/HiYaPyCo.egg-info/SOURCES.txt
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)        1 2024-05-11 05:03:28.000000 HiYaPyCo-0.5.6/HiYaPyCo.egg-info/dependency_links.txt
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)       34 2024-05-11 05:03:28.000000 HiYaPyCo-0.5.6/HiYaPyCo.egg-info/requires.txt
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)        9 2024-05-11 05:03:28.000000 HiYaPyCo-0.5.6/HiYaPyCo.egg-info/top_level.txt
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    35141 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/LICENSE
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)       36 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/MANIFEST.in
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    11283 2024-05-11 05:03:28.522827 HiYaPyCo-0.5.6/PKG-INFO
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    10492 2024-05-11 04:56:25.000000 HiYaPyCo-0.5.6/README.rst
+drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-05-11 05:03:28.518827 HiYaPyCo-0.5.6/hiyapyco/
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)    21991 2024-05-10 18:45:35.000000 HiYaPyCo-0.5.6/hiyapyco/__init__.py
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)     2604 2024-04-13 08:37:32.000000 HiYaPyCo-0.5.6/hiyapyco/odyldo.py
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)       16 2024-05-11 04:43:26.000000 HiYaPyCo-0.5.6/hiyapyco/version.py
+-rw-r--r--   0 zerwes    (1000) zerwes    (1000)      109 2024-05-11 05:03:28.522827 HiYaPyCo-0.5.6/setup.cfg
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1357 2024-05-11 04:53:17.000000 HiYaPyCo-0.5.6/setup.py
+drwxr-xr-x   0 zerwes    (1000) zerwes    (1000)        0 2024-05-11 05:03:28.518827 HiYaPyCo-0.5.6/test/
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1739 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_castinterpolated.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     3021 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_interpolation.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1734 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_interpolationunicode.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     4905 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_invocation.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     5075 2023-11-29 07:36:03.000000 HiYaPyCo-0.5.6/test/test_merge.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     4313 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_missingfiles.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1753 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_multiple.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     2836 2022-05-04 08:47:46.000000 HiYaPyCo-0.5.6/test/test_odict.py
+-rwxr-xr-x   0 zerwes    (1000) zerwes    (1000)     1913 2020-06-18 09:22:15.000000 HiYaPyCo-0.5.6/test/test_simple.py
```

### Comparing `HiYaPyCo-0.5.5/HiYaPyCo.egg-info/PKG-INFO` & `HiYaPyCo-0.5.6/HiYaPyCo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiYaPyCo
-Version: 0.5.5
+Version: 0.5.6
 Summary: Hierarchical Yaml Python Config
 Home-page: https://github.com/zerwes/hiyapyco
 Author: Klaus Zerwes zero-sys.net
 Author-email: zerwes@users.noreply.github.com
 License: GPLv3
 Keywords: configuration parser yaml
 Platform: any
@@ -351,14 +351,21 @@
 
 Changelog
 ---------
 
 0.5.5
 ~~~~~~
 
+MERGED: #70 by itachi-cracker
+
+FIXED: #61 (removed deprecated distutils)
+
+0.5.5
+~~~~~~
+
 FIXED: #67 cosmetic changes
 
 0.5.4
 ~~~~~~
 
 FIXED: #60 recursive calls to _substmerge
```

### Comparing `HiYaPyCo-0.5.5/LICENSE` & `HiYaPyCo-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.5/PKG-INFO` & `HiYaPyCo-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiYaPyCo
-Version: 0.5.5
+Version: 0.5.6
 Summary: Hierarchical Yaml Python Config
 Home-page: https://github.com/zerwes/hiyapyco
 Author: Klaus Zerwes zero-sys.net
 Author-email: zerwes@users.noreply.github.com
 License: GPLv3
 Keywords: configuration parser yaml
 Platform: any
@@ -351,14 +351,21 @@
 
 Changelog
 ---------
 
 0.5.5
 ~~~~~~
 
+MERGED: #70 by itachi-cracker
+
+FIXED: #61 (removed deprecated distutils)
+
+0.5.5
+~~~~~~
+
 FIXED: #67 cosmetic changes
 
 0.5.4
 ~~~~~~
 
 FIXED: #60 recursive calls to _substmerge
```

### Comparing `HiYaPyCo-0.5.5/README.rst` & `HiYaPyCo-0.5.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -330,14 +330,21 @@
 
 Changelog
 ---------
 
 0.5.5
 ~~~~~~
 
+MERGED: #70 by itachi-cracker
+
+FIXED: #61 (removed deprecated distutils)
+
+0.5.5
+~~~~~~
+
 FIXED: #67 cosmetic changes
 
 0.5.4
 ~~~~~~
 
 FIXED: #60 recursive calls to _substmerge
```

### Comparing `HiYaPyCo-0.5.5/hiyapyco/__init__.py` & `HiYaPyCo-0.5.6/hiyapyco/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 """
 
 from __future__ import unicode_literals
 
 import sys
 import os
 import logging
-from distutils.util import strtobool
 import re
 import io
 import yaml
 from yaml import parser
 from jinja2 import Environment, Undefined, DebugUndefined, StrictUndefined, TemplateError
 
 from . import odyldo
@@ -517,8 +516,19 @@
     Returns a representation of the merged and (if requested) interpolated config.
     Will mostly be a OrderedDict (dict if usedefaultyamlloader), but can be of any other type,
     depending on the yaml files.
     """
     hiyapyco = HiYaPyCo(*args, **kwargs)
     return hiyapyco.data()
 
+def strtobool(val):
+    """
+    minimal implementation of the strtobool function (replaces deprecated distutils)
+    """
+    val = val.lower()
+    if val in ("y", "yes", "t", "true", "on", "1"):
+        return 1
+    if val in ("n", "no", "f", "false", "off", "0"):
+        return 0
+    raise ValueError("invalid truth value %r" % (val,))
+
 # vim: tabstop=4 expandtab shiftwidth=4 softtabstop=4 smartindent nu
```

### Comparing `HiYaPyCo-0.5.5/hiyapyco/odyldo.py` & `HiYaPyCo-0.5.6/hiyapyco/odyldo.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.5/setup.py` & `HiYaPyCo-0.5.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 from setuptools import setup
 
 basepath = os.path.dirname(os.path.realpath(__file__))
 sys.path.insert(0, os.path.dirname(basepath))
 
-HIYAPYCOVERSION='0.5.5'
+HIYAPYCOVERSION='0.5.6'
 
 long_description = open('README.rst').read()
 
 installrequires = [
     'PyYAML<7',
     'Jinja2>3,<4',
     'MarkupSafe<3'
```

### Comparing `HiYaPyCo-0.5.5/test/test_castinterpolated.py` & `HiYaPyCo-0.5.6/test/test_castinterpolated.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.5/test/test_interpolation.py` & `HiYaPyCo-0.5.6/test/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.5/test/test_interpolationunicode.py` & `HiYaPyCo-0.5.6/test/test_interpolationunicode.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.5/test/test_invocation.py` & `HiYaPyCo-0.5.6/test/test_invocation.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.5/test/test_merge.py` & `HiYaPyCo-0.5.6/test/test_merge.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.5/test/test_missingfiles.py` & `HiYaPyCo-0.5.6/test/test_missingfiles.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.5/test/test_multiple.py` & `HiYaPyCo-0.5.6/test/test_multiple.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.5/test/test_odict.py` & `HiYaPyCo-0.5.6/test/test_odict.py`

 * *Files identical despite different names*

### Comparing `HiYaPyCo-0.5.5/test/test_simple.py` & `HiYaPyCo-0.5.6/test/test_simple.py`

 * *Files identical despite different names*

