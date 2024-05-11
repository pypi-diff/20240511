# Comparing `tmp/pylogg-0.3.2.tar.gz` & `tmp/pylogg-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogg-0.3.2.tar", last modified: Wed Apr 17 18:07:07 2024, max compression
+gzip compressed data, was "pylogg-0.3.3.tar", last modified: Sat May 11 17:18:07 2024, max compression
```

## Comparing `pylogg-0.3.2.tar` & `pylogg-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:07:07.128898 pylogg-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-17 18:06:58.000000 pylogg-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-17 18:07:07.128898 pylogg-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-17 18:06:58.000000 pylogg-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:07:07.124897 pylogg-0.3.2/pylogg/
--rw-r--r--   0 runner    (1001) docker     (127)    17574 2024-04-17 18:06:58.000000 pylogg-0.3.2/pylogg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-17 18:06:58.000000 pylogg-0.3.2/pylogg/jsonfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-17 18:06:58.000000 pylogg-0.3.2/pylogg/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-04-17 18:06:58.000000 pylogg-0.3.2/pylogg/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:07:07.124897 pylogg-0.3.2/pylogg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-17 18:07:07.000000 pylogg-0.3.2/pylogg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-17 18:07:07.000000 pylogg-0.3.2/pylogg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 18:07:07.000000 pylogg-0.3.2/pylogg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-17 18:07:07.000000 pylogg-0.3.2/pylogg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 18:07:07.000000 pylogg-0.3.2/pylogg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-17 18:06:58.000000 pylogg-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 18:07:07.128898 pylogg-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 18:07:07.124897 pylogg-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-17 18:06:58.000000 pylogg-0.3.2/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:18:07.961746 pylogg-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-11 17:18:03.000000 pylogg-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-11 17:18:07.961746 pylogg-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-11 17:18:03.000000 pylogg-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:18:07.957746 pylogg-0.3.3/pylogg/
+-rw-r--r--   0 runner    (1001) docker     (127)    17674 2024-05-11 17:18:03.000000 pylogg-0.3.3/pylogg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-11 17:18:03.000000 pylogg-0.3.3/pylogg/jsonfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-11 17:18:03.000000 pylogg-0.3.3/pylogg/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-05-11 17:18:03.000000 pylogg-0.3.3/pylogg/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:18:07.961746 pylogg-0.3.3/pylogg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-11 17:18:07.000000 pylogg-0.3.3/pylogg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-11 17:18:07.000000 pylogg-0.3.3/pylogg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 17:18:07.000000 pylogg-0.3.3/pylogg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-11 17:18:07.000000 pylogg-0.3.3/pylogg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 17:18:07.000000 pylogg-0.3.3/pylogg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-11 17:18:03.000000 pylogg-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 17:18:07.961746 pylogg-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 17:18:07.961746 pylogg-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-11 17:18:03.000000 pylogg-0.3.3/tests/test_settings.py
```

### Comparing `pylogg-0.3.2/LICENSE` & `pylogg-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylogg-0.3.2/PKG-INFO` & `pylogg-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogg
-Version: 0.3.2
+Version: 0.3.3
 Summary: Logging and YAML-based configuration modules in Python.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/python-logg
 Project-URL: Bug Tracker, https://github.com/akhlakm/python-logg/issues
 Keywords: logging,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pylogg-0.3.2/README.md` & `pylogg-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pylogg-0.3.2/pylogg/__init__.py` & `pylogg-0.3.3/pylogg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A personally opinionated logging package.
 LICENSE MIT Copyright 2024 Akhlak Mahmood
 
 """
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 __author__ = "Akhlak Mahmood"
 
 import os
 import sys
 import textwrap
 import time
 from datetime import datetime, timezone
@@ -212,16 +212,15 @@
 def _colorize(conf, level, msg):
     if not conf.color:
         return msg
     else:
         return f"{_color_seqs[level]}{msg}{_reset_seq}"
 
 def _save(conf : _config, level, fmtmsg, timestr, caller):
-    if conf.fileh is None:
-        return
+    """ Log to file or callback """
 
     if not conf.file_times:
         timestr = ""
 
     extra = ""
     if conf.file_stack or level in [Level.FATAL, Level.ERROR, Level.DEBUG]:
         extra += caller
@@ -231,22 +230,28 @@
         prefix = _prefixes[level]
         fmtlogger = f"{conf.logger}_ " if conf.logger else ""
         line = f"{timestr}{prefix} {fmtlogger}{fmtmsg} {extra}"
         line = _indent(conf, line)
     else:
         line = fmtmsg
 
-    conf.fileh.write(line + "\n")
-    conf.fileh.flush()
-    os.fsync(conf.fileh.fileno())
+    if conf.fileh:
+        conf.fileh.write(line + "\n")
+        conf.fileh.flush()
+        os.fsync(conf.fileh.fileno())
 
     if conf.callback:
-        conf.callback(line)
+        try:
+            conf.callback(line)
+        except Exception as err:
+            print(err)
+
     return line
 
+
 def _print(conf : _config, level, fmtmsg, timestr, caller):
     if not conf.console_times:
         timestr = ""
 
     extra = ""
     if conf.console_stack or level in [Level.FATAL, Level.ERROR, Level.DEBUG]:
         extra += caller
```

### Comparing `pylogg-0.3.2/pylogg/jsonfs.py` & `pylogg-0.3.3/pylogg/jsonfs.py`

 * *Files identical despite different names*

### Comparing `pylogg-0.3.2/pylogg/postgres.py` & `pylogg-0.3.3/pylogg/postgres.py`

 * *Files identical despite different names*

### Comparing `pylogg-0.3.2/pylogg/settings.py` & `pylogg-0.3.3/pylogg/settings.py`

 * *Files identical despite different names*

### Comparing `pylogg-0.3.2/pylogg.egg-info/PKG-INFO` & `pylogg-0.3.3/pylogg.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogg
-Version: 0.3.2
+Version: 0.3.3
 Summary: Logging and YAML-based configuration modules in Python.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/python-logg
 Project-URL: Bug Tracker, https://github.com/akhlakm/python-logg/issues
 Keywords: logging,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pylogg-0.3.2/pyproject.toml` & `pylogg-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylogg-0.3.2/tests/test_settings.py` & `pylogg-0.3.3/tests/test_settings.py`

 * *Files identical despite different names*

