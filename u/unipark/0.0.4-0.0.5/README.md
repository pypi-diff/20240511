# Comparing `tmp/unipark-0.0.4.tar.gz` & `tmp/unipark-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipark-0.0.4.tar", last modified: Wed May  8 16:41:32 2024, max compression
+gzip compressed data, was "unipark-0.0.5.tar", last modified: Sat May 11 04:44:46 2024, max compression
```

## Comparing `unipark-0.0.4.tar` & `unipark-0.0.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.039103 unipark-0.0.4/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      131 2023-10-12 11:57:58.000000 unipark-0.0.4/MANIFEST.in
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      334 2024-05-08 16:41:32.035103 unipark-0.0.4/PKG-INFO
--rw-rw-r--   0 parklam   (1000) parklam   (1000)       83 2023-10-07 03:22:37.000000 unipark-0.0.4/README.md
--rw-rw-r--   0 parklam   (1000) parklam   (1000)        6 2024-05-08 14:10:40.000000 unipark-0.0.4/VERSION
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      138 2023-10-17 06:13:44.000000 unipark-0.0.4/pyproject.toml
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.027103 unipark-0.0.4/requirements/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      113 2023-10-11 19:05:16.000000 unipark-0.0.4/requirements/runtime.txt
--rw-rw-r--   0 parklam   (1000) parklam   (1000)       38 2024-05-08 16:41:32.039103 unipark-0.0.4/setup.cfg
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     1722 2023-10-13 05:37:26.000000 unipark-0.0.4/setup.py
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.031103 unipark-0.0.4/tests/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      144 2023-10-31 19:27:19.000000 unipark-0.0.4/tests/__init__.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      609 2023-10-16 05:05:16.000000 unipark-0.0.4/tests/test_cli.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     2796 2024-05-08 14:04:13.000000 unipark-0.0.4/tests/test_config.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     9632 2023-10-30 12:15:00.000000 unipark-0.0.4/tests/test_mvc.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      630 2023-10-13 05:15:16.000000 unipark-0.0.4/tests/test_requests.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     1093 2023-10-13 05:34:55.000000 unipark-0.0.4/tests/test_utils.py
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.031103 unipark-0.0.4/unipark/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      795 2023-10-17 06:21:08.000000 unipark-0.0.4/unipark/__init__.py
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.035103 unipark-0.0.4/unipark/cli/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      545 2023-10-13 07:10:19.000000 unipark-0.0.4/unipark/cli/__init__.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     1334 2024-05-08 14:01:37.000000 unipark-0.0.4/unipark/config.py
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.035103 unipark-0.0.4/unipark/mvc/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     5808 2023-10-31 05:02:40.000000 unipark-0.0.4/unipark/mvc/__init__.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      824 2023-10-31 19:27:19.000000 unipark-0.0.4/unipark/mvc/command.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     2329 2023-10-16 03:57:36.000000 unipark-0.0.4/unipark/mvc/facade.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     1237 2023-10-31 19:29:36.000000 unipark-0.0.4/unipark/mvc/mediator.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     1672 2023-10-31 19:27:19.000000 unipark-0.0.4/unipark/mvc/observer.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      737 2023-10-31 19:27:19.000000 unipark-0.0.4/unipark/mvc/proxy.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     4363 2023-10-13 05:13:35.000000 unipark-0.0.4/unipark/requests.py
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.035103 unipark-0.0.4/unipark/utils/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     2863 2023-10-31 19:27:19.000000 unipark-0.0.4/unipark/utils/__init__.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     6364 2023-10-07 10:19:42.000000 unipark-0.0.4/unipark/utils/log.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)     1381 2023-12-03 06:41:23.000000 unipark-0.0.4/unipark/utils/translation.py
--rw-rw-r--   0 parklam   (1000) parklam   (1000)       47 2024-05-08 16:41:29.000000 unipark-0.0.4/unipark/version.py
-drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-08 16:41:32.035103 unipark-0.0.4/unipark.egg-info/
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      334 2024-05-08 16:41:30.000000 unipark-0.0.4/unipark.egg-info/PKG-INFO
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      699 2024-05-08 16:41:32.000000 unipark-0.0.4/unipark.egg-info/SOURCES.txt
--rw-rw-r--   0 parklam   (1000) parklam   (1000)        1 2024-05-08 16:41:30.000000 unipark-0.0.4/unipark.egg-info/dependency_links.txt
--rw-rw-r--   0 parklam   (1000) parklam   (1000)       41 2024-05-08 16:41:31.000000 unipark-0.0.4/unipark.egg-info/entry_points.txt
--rw-rw-r--   0 parklam   (1000) parklam   (1000)      113 2024-05-08 16:41:31.000000 unipark-0.0.4/unipark.egg-info/requires.txt
--rw-rw-r--   0 parklam   (1000) parklam   (1000)        8 2024-05-08 16:41:31.000000 unipark-0.0.4/unipark.egg-info/top_level.txt
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-11 04:44:46.112726 unipark-0.0.5/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      131 2023-10-12 11:57:58.000000 unipark-0.0.5/MANIFEST.in
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      334 2024-05-11 04:44:46.112726 unipark-0.0.5/PKG-INFO
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)       83 2023-10-07 03:22:37.000000 unipark-0.0.5/README.md
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)        6 2024-05-11 04:44:25.000000 unipark-0.0.5/VERSION
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      138 2023-10-17 06:13:44.000000 unipark-0.0.5/pyproject.toml
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-11 04:44:46.104725 unipark-0.0.5/requirements/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      113 2023-10-11 19:05:16.000000 unipark-0.0.5/requirements/runtime.txt
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)       38 2024-05-11 04:44:46.112726 unipark-0.0.5/setup.cfg
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     1722 2023-10-13 05:37:26.000000 unipark-0.0.5/setup.py
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-11 04:44:46.104725 unipark-0.0.5/tests/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      144 2023-10-31 19:27:19.000000 unipark-0.0.5/tests/__init__.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      609 2023-10-16 05:05:16.000000 unipark-0.0.5/tests/test_cli.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     2796 2024-05-08 14:04:13.000000 unipark-0.0.5/tests/test_config.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     9632 2023-10-30 12:15:00.000000 unipark-0.0.5/tests/test_mvc.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      630 2023-10-13 05:15:16.000000 unipark-0.0.5/tests/test_requests.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     1093 2023-10-13 05:34:55.000000 unipark-0.0.5/tests/test_utils.py
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-11 04:44:46.108726 unipark-0.0.5/unipark/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      795 2023-10-17 06:21:08.000000 unipark-0.0.5/unipark/__init__.py
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-11 04:44:46.108726 unipark-0.0.5/unipark/cli/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      545 2023-10-13 07:10:19.000000 unipark-0.0.5/unipark/cli/__init__.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     1415 2024-05-11 04:42:58.000000 unipark-0.0.5/unipark/config.py
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-11 04:44:46.108726 unipark-0.0.5/unipark/mvc/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     5808 2023-10-31 05:02:40.000000 unipark-0.0.5/unipark/mvc/__init__.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      824 2023-10-31 19:27:19.000000 unipark-0.0.5/unipark/mvc/command.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     2329 2023-10-16 03:57:36.000000 unipark-0.0.5/unipark/mvc/facade.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     1237 2023-10-31 19:29:36.000000 unipark-0.0.5/unipark/mvc/mediator.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     1672 2023-10-31 19:27:19.000000 unipark-0.0.5/unipark/mvc/observer.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      737 2023-10-31 19:27:19.000000 unipark-0.0.5/unipark/mvc/proxy.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     4363 2023-10-13 05:13:35.000000 unipark-0.0.5/unipark/requests.py
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-11 04:44:46.112726 unipark-0.0.5/unipark/utils/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     2863 2023-10-31 19:27:19.000000 unipark-0.0.5/unipark/utils/__init__.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     6364 2023-10-07 10:19:42.000000 unipark-0.0.5/unipark/utils/log.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)     1381 2023-12-03 06:41:23.000000 unipark-0.0.5/unipark/utils/translation.py
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)       47 2024-05-11 04:44:43.000000 unipark-0.0.5/unipark/version.py
+drwxrwxr-x   0 parklam   (1000) parklam   (1000)        0 2024-05-11 04:44:46.108726 unipark-0.0.5/unipark.egg-info/
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      334 2024-05-11 04:44:44.000000 unipark-0.0.5/unipark.egg-info/PKG-INFO
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      699 2024-05-11 04:44:46.000000 unipark-0.0.5/unipark.egg-info/SOURCES.txt
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)        1 2024-05-11 04:44:44.000000 unipark-0.0.5/unipark.egg-info/dependency_links.txt
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)       41 2024-05-11 04:44:45.000000 unipark-0.0.5/unipark.egg-info/entry_points.txt
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)      113 2024-05-11 04:44:45.000000 unipark-0.0.5/unipark.egg-info/requires.txt
+-rw-rw-r--   0 parklam   (1000) parklam   (1000)        8 2024-05-11 04:44:45.000000 unipark-0.0.5/unipark.egg-info/top_level.txt
```

### Comparing `unipark-0.0.4/setup.py` & `unipark-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/tests/test_cli.py` & `unipark-0.0.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/tests/test_config.py` & `unipark-0.0.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/tests/test_mvc.py` & `unipark-0.0.5/tests/test_mvc.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/tests/test_requests.py` & `unipark-0.0.5/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/tests/test_utils.py` & `unipark-0.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/unipark/__init__.py` & `unipark-0.0.5/unipark/__init__.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/unipark/cli/__init__.py` & `unipark-0.0.5/unipark/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/unipark/config.py` & `unipark-0.0.5/unipark/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,17 @@
             except decouple.UndefinedValueError as e:
                 raise AttributeError(str(e))
 
     def _retrieve_option_from_config(self, *args, **kwargs):
         option = decouple.config(*args, **kwargs)
         if self.auto_cast and \
                 isinstance(option, str):
-            if option.upper() in ( 'TRUE', 'FALSE', ):
+            if kwargs.get('cast', None) is str: 
+                return option
+            elif option.upper() in ( 'TRUE', 'FALSE', ):
                 return option.upper() == 'TRUE'
             else:
                 try:
                     return int(option)
                 except ValueError as e:
                     pass
                 try:
```

### Comparing `unipark-0.0.4/unipark/mvc/__init__.py` & `unipark-0.0.5/unipark/mvc/__init__.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/unipark/mvc/command.py` & `unipark-0.0.5/unipark/mvc/command.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/unipark/mvc/facade.py` & `unipark-0.0.5/unipark/mvc/facade.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/unipark/mvc/mediator.py` & `unipark-0.0.5/unipark/mvc/mediator.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/unipark/mvc/observer.py` & `unipark-0.0.5/unipark/mvc/observer.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/unipark/mvc/proxy.py` & `unipark-0.0.5/unipark/mvc/proxy.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/unipark/requests.py` & `unipark-0.0.5/unipark/requests.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/unipark/utils/__init__.py` & `unipark-0.0.5/unipark/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/unipark/utils/log.py` & `unipark-0.0.5/unipark/utils/log.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/unipark/utils/translation.py` & `unipark-0.0.5/unipark/utils/translation.py`

 * *Files identical despite different names*

### Comparing `unipark-0.0.4/unipark.egg-info/SOURCES.txt` & `unipark-0.0.5/unipark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

