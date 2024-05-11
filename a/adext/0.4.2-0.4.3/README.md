# Comparing `tmp/adext-0.4.2.tar.gz` & `tmp/adext-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adext-0.4.2.tar", last modified: Tue Jun  1 00:13:31 2021, max compression
+gzip compressed data, was "adext-0.4.3.tar", last modified: Sat May 11 17:15:05 2024, max compression
```

## Comparing `adext-0.4.2.tar` & `adext-0.4.3.tar`

### file list

```diff
@@ -1,29 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 00:13:31.567460 adext-0.4.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 00:13:31.559460 adext-0.4.2/.devcontainer/
--rw-r--r--   0 root         (0) root         (0)     1042 2021-06-01 00:13:21.000000 adext-0.4.2/.devcontainer/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1501 2021-06-01 00:13:21.000000 adext-0.4.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 00:13:31.559460 adext-0.4.2/.github/
--rw-r--r--   0 root         (0) root         (0)      322 2021-06-01 00:13:21.000000 adext-0.4.2/.github/release-drafter.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 00:13:31.567460 adext-0.4.2/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      307 2021-06-01 00:13:21.000000 adext-0.4.2/.github/workflows/pulls.yaml
--rw-r--r--   0 root         (0) root         (0)      583 2021-06-01 00:13:21.000000 adext-0.4.2/.github/workflows/pypi-upload.yaml
--rw-r--r--   0 root         (0) root         (0)      321 2021-06-01 00:13:21.000000 adext-0.4.2/.github/workflows/release-drafter.yml
--rw-r--r--   0 root         (0) root         (0)     2156 2021-06-01 00:13:21.000000 adext-0.4.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)       79 2021-06-01 00:13:21.000000 adext-0.4.2/.pylintrc
--rw-r--r--   0 root         (0) root         (0)     1054 2021-06-01 00:13:21.000000 adext-0.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2021-06-01 00:13:21.000000 adext-0.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4813 2021-06-01 00:13:31.567460 adext-0.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4238 2021-06-01 00:13:21.000000 adext-0.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 00:13:31.567460 adext-0.4.2/adext/
--rw-r--r--   0 root         (0) root         (0)       67 2021-06-01 00:13:21.000000 adext-0.4.2/adext/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3176 2021-06-01 00:13:21.000000 adext-0.4.2/adext/adext.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 00:13:31.567460 adext-0.4.2/adext.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4813 2021-06-01 00:13:31.000000 adext-0.4.2/adext.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2021-06-01 00:13:31.000000 adext-0.4.2/adext.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-06-01 00:13:31.000000 adext-0.4.2/adext.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2021-06-01 00:13:31.000000 adext-0.4.2/adext.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2021-06-01 00:13:31.000000 adext-0.4.2/adext.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-06-01 00:13:31.567460 adext-0.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      975 2021-06-01 00:13:21.000000 adext-0.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-01 00:13:31.567460 adext-0.4.2/tests/
--rw-r--r--   0 root         (0) root         (0)     5277 2021-06-01 00:13:21.000000 adext-0.4.2/tests/test_adext.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 17:15:05.209942 adext-0.4.3/
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-05-11 17:15:00.000000 adext-0.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-11 17:15:00.000000 adext-0.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4830 2024-05-11 17:15:05.209942 adext-0.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4238 2024-05-11 17:15:00.000000 adext-0.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 17:15:05.209942 adext-0.4.3/adext/
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-11 17:15:00.000000 adext-0.4.3/adext/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2024-05-11 17:15:00.000000 adext-0.4.3/adext/adext.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 17:15:05.209942 adext-0.4.3/adext.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4830 2024-05-11 17:15:05.000000 adext-0.4.3/adext.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      235 2024-05-11 17:15:05.000000 adext-0.4.3/adext.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 17:15:05.000000 adext-0.4.3/adext.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-11 17:15:05.000000 adext-0.4.3/adext.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-11 17:15:05.000000 adext-0.4.3/adext.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 17:15:05.209942 adext-0.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      975 2024-05-11 17:15:00.000000 adext-0.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 17:15:05.209942 adext-0.4.3/tests/
+-rw-r--r--   0 root         (0) root         (0)     5277 2024-05-11 17:15:00.000000 adext-0.4.3/tests/test_adext.py
```

### Comparing `adext-0.4.2/LICENSE` & `adext-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adext-0.4.2/PKG-INFO` & `adext-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: adext
-Version: 0.4.2
+Version: 0.4.3
 Summary: AlarmDecoder extended
 Home-page: https://github.com/ajschmidt8/adext
 Author: AJ Schmidt
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Security
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: alarmdecoder==1.13.11
 
 # adext
 
 `adext` is a small package that extends [alarmdecoder](https://github.com/nutechsoftware/alarmdecoder/) to include some additional methods for [Home Assistant](https://github.com/home-assistant/core).
 
 Specifically, the following methods have been added:
 
@@ -81,9 +81,7 @@
 
 | Mode                                                    | Key Sequence                    |
 | ------------------------------------------------------- | ------------------------------- |
 | `alarm_arm_home`                                        | `chr(4)` + `chr(4)` + `chr(4)`  |
 | `alarm_arm_away`                                        | `chr(5)` + `chr(5)` + `chr(5)`  |
 | `alarm_arm_night` (`alt_night_mode` = `false`, default) | `chr(4)` + `chr(4)` + `chr(4)`  |
 | `alarm_arm_night` (`alt_night_mode` = `true`)           | `*9` + `code`                   |
-
-
```

### Comparing `adext-0.4.2/README.md` & `adext-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `adext-0.4.2/adext/adext.py` & `adext-0.4.3/adext/adext.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 """
 Extends the AlarmDecoder class to include helper methods for HomeAssistant
 """
 
+import asyncio
+
 from alarmdecoder.decoder import AlarmDecoder
 from alarmdecoder.panels import DSC, ADEMCO as HONEYWELL
 
 ARM_HOME = "arm_home"
 ARM_AWAY = "arm_away"
 ARM_NIGHT = "arm_night"
 
 
 class AdExt(AlarmDecoder):
     """
     Extended AlarmDecoder class
     """
 
+    def __init__(self, device, ignore_message_states=False, ignore_lrr_states=True):
+        super().__init__(device, ignore_message_states, ignore_lrr_states)
+        self._event = asyncio.Event()
+
+    def _handle_version(self, data):
+        super()._handle_version(data)
+        self._event.set()
+
+    async def is_init(self):
+        return (await self._event.wait())
+
     def _get_arm_sequence(
         self, arm_mode, code, code_arm_required, auto_bypass, alt_night_mode=False,
     ):
         """
         Returns arming sequences based on panel brand & config settings
         """
```

### Comparing `adext-0.4.2/adext.egg-info/PKG-INFO` & `adext-0.4.3/adext.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: adext
-Version: 0.4.2
+Version: 0.4.3
 Summary: AlarmDecoder extended
 Home-page: https://github.com/ajschmidt8/adext
 Author: AJ Schmidt
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Communications
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Security
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: alarmdecoder==1.13.11
 
 # adext
 
 `adext` is a small package that extends [alarmdecoder](https://github.com/nutechsoftware/alarmdecoder/) to include some additional methods for [Home Assistant](https://github.com/home-assistant/core).
 
 Specifically, the following methods have been added:
 
@@ -81,9 +81,7 @@
 
 | Mode                                                    | Key Sequence                    |
 | ------------------------------------------------------- | ------------------------------- |
 | `alarm_arm_home`                                        | `chr(4)` + `chr(4)` + `chr(4)`  |
 | `alarm_arm_away`                                        | `chr(5)` + `chr(5)` + `chr(5)`  |
 | `alarm_arm_night` (`alt_night_mode` = `false`, default) | `chr(4)` + `chr(4)` + `chr(4)`  |
 | `alarm_arm_night` (`alt_night_mode` = `true`)           | `*9` + `code`                   |
-
-
```

### Comparing `adext-0.4.2/setup.py` & `adext-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `adext-0.4.2/tests/test_adext.py` & `adext-0.4.3/tests/test_adext.py`

 * *Files identical despite different names*

