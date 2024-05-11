# Comparing `tmp/event-external-local-0.0.8.tar.gz` & `tmp/event-external-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event-external-local-0.0.8.tar", last modified: Mon Dec 11 11:51:48 2023, max compression
+gzip compressed data, was "event-external-local-0.0.9.tar", last modified: Mon Dec 11 14:03:44 2023, max compression
```

## Comparing `event-external-local-0.0.8.tar` & `event-external-local-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 11:51:48.848183 event-external-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-12-11 11:51:48.848183 event-external-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-12-11 11:51:31.000000 event-external-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 11:51:48.844183 event-external-local-0.0.8/event-external-local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 11:51:48.844183 event-external-local-0.0.8/event-external-local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 11:51:31.000000 event-external-local-0.0.8/event-external-local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-12-11 11:51:31.000000 event-external-local-0.0.8/event-external-local/src/external_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2023-12-11 11:51:31.000000 event-external-local-0.0.8/event-external-local/src/external_event_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2023-12-11 11:51:31.000000 event-external-local-0.0.8/event-external-local/src/external_event_local_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 11:51:48.848183 event-external-local-0.0.8/event_external_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-12-11 11:51:48.000000 event-external-local-0.0.8/event_external_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-11 11:51:48.000000 event-external-local-0.0.8/event_external_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 11:51:48.000000 event-external-local-0.0.8/event_external_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-11 11:51:48.000000 event-external-local-0.0.8/event_external_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-11 11:51:48.000000 event-external-local-0.0.8/event_external_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-11 11:51:31.000000 event-external-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 11:51:48.848183 event-external-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-11 11:51:31.000000 event-external-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:03:44.241195 event-external-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2023-12-11 14:03:44.237195 event-external-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-12-11 14:03:21.000000 event-external-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:03:44.233195 event-external-local-0.0.9/event_external_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:03:44.237195 event-external-local-0.0.9/event_external_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 14:03:21.000000 event-external-local-0.0.9/event_external_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-12-11 14:03:21.000000 event-external-local-0.0.9/event_external_local/src/external_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2023-12-11 14:03:21.000000 event-external-local-0.0.9/event_external_local/src/external_event_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2023-12-11 14:03:21.000000 event-external-local-0.0.9/event_external_local/src/external_event_local_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 14:03:44.237195 event-external-local-0.0.9/event_external_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2023-12-11 14:03:44.000000 event-external-local-0.0.9/event_external_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2023-12-11 14:03:44.000000 event-external-local-0.0.9/event_external_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 14:03:44.000000 event-external-local-0.0.9/event_external_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-11 14:03:44.000000 event-external-local-0.0.9/event_external_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-11 14:03:44.000000 event-external-local-0.0.9/event_external_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-11 14:03:21.000000 event-external-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 14:03:44.241195 event-external-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2023-12-11 14:03:21.000000 event-external-local-0.0.9/setup.py
```

### Comparing `event-external-local-0.0.8/PKG-INFO` & `event-external-local-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-external-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles event-external-local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `event-external-local-0.0.8/README.md` & `event-external-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `event-external-local-0.0.8/event-external-local/src/external_event.py` & `event-external-local-0.0.9/event_external_local/src/external_event.py`

 * *Files identical despite different names*

### Comparing `event-external-local-0.0.8/event-external-local/src/external_event_constants.py` & `event-external-local-0.0.9/event_external_local/src/external_event_constants.py`

 * *Files identical despite different names*

### Comparing `event-external-local-0.0.8/event-external-local/src/external_event_local_class.py` & `event-external-local-0.0.9/event_external_local/src/external_event_local_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sys
 import os
 import copy
 from dotenv import load_dotenv
+load_dotenv()
 script_directory = os.path.dirname(os.path.abspath(__file__))
 sys.path.append(os.path.join(script_directory, '..'))
-load_dotenv()
 from circles_local_database_python.generic_crud import GenericCRUD  # noqa
 from logger_local.Logger import Logger  # noqa
-from .external_event_constants import ExternalEventLocalConstants  # noqa
-from .external_event import EventExternal  # noqa
+from external_event_constants import ExternalEventLocalConstants  # noqa
+from external_event import EventExternal  # noqa
 
 
 object1 = ExternalEventLocalConstants.EXTERNAL_EVENT_LOCAL_CODE_LOGGER_OBJECT
 logger = Logger.create_logger(object=object1)
 
 
 class ExternalEventsLocal(GenericCRUD):
```

### Comparing `event-external-local-0.0.8/event_external_local.egg-info/PKG-INFO` & `event-external-local-0.0.9/event_external_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-external-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles event-external-local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `event-external-local-0.0.8/pyproject.toml` & `event-external-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `event-external-local-0.0.8/setup.py` & `event-external-local-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 PACKAGE_NAME = "event-external-local"
-package_dir = PACKAGE_NAME  # .replace("-", "_")
+package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # update only the minor version each time
+    version='0.0.9',  # update only the minor version each time
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles event-external-local Python",
     long_description="PyPI Package for Circles event-external-local Python",
     long_description_content_type='text/markdown',
     # TODO: Please update the URL below
     url="https://github.com/circles",
```

