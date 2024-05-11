# Comparing `tmp/freezegun-1.4.0.tar.gz` & `tmp/freezegun-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freezegun-1.4.0.tar", last modified: Tue Dec 19 10:46:30 2023, max compression
+gzip compressed data, was "freezegun-1.5.0.tar", last modified: Tue Apr 23 18:33:39 2024, max compression
```

## Comparing `freezegun-1.4.0.tar` & `freezegun-1.5.0.tar`

### file list

```diff
@@ -1,44 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 10:46:30.612686 freezegun-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-19 10:46:15.000000 freezegun-1.4.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2023-12-19 10:46:15.000000 freezegun-1.4.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2023-12-19 10:46:15.000000 freezegun-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-19 10:46:15.000000 freezegun-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2023-12-19 10:46:30.612686 freezegun-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2023-12-19 10:46:15.000000 freezegun-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 10:46:30.608686 freezegun-1.4.0/freezegun/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-12-19 10:46:24.000000 freezegun-1.4.0/freezegun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-19 10:46:15.000000 freezegun-1.4.0/freezegun/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-12-19 10:46:15.000000 freezegun-1.4.0/freezegun/_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    29579 2023-12-19 10:46:15.000000 freezegun-1.4.0/freezegun/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2023-12-19 10:46:15.000000 freezegun-1.4.0/freezegun/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-12-19 10:46:15.000000 freezegun-1.4.0/freezegun/config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 10:46:15.000000 freezegun-1.4.0/freezegun/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 10:46:30.612686 freezegun-1.4.0/freezegun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2023-12-19 10:46:30.000000 freezegun-1.4.0/freezegun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-19 10:46:30.000000 freezegun-1.4.0/freezegun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 10:46:30.000000 freezegun-1.4.0/freezegun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-19 10:46:30.000000 freezegun-1.4.0/freezegun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-19 10:46:30.000000 freezegun-1.4.0/freezegun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-19 10:46:15.000000 freezegun-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-19 10:46:15.000000 freezegun-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-12-19 10:46:30.616685 freezegun-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-19 10:46:15.000000 freezegun-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 10:46:30.612686 freezegun-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/another_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/fake_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_class_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)    27795 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_datetimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_import_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_ticking.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-12-19 10:46:15.000000 freezegun-1.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:33:39.480508 freezegun-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-23 18:33:19.000000 freezegun-1.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-23 18:33:19.000000 freezegun-1.5.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-04-23 18:33:19.000000 freezegun-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-23 18:33:19.000000 freezegun-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-23 18:33:39.480508 freezegun-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-04-23 18:33:19.000000 freezegun-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:33:39.476508 freezegun-1.5.0/freezegun/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-23 18:33:36.000000 freezegun-1.5.0/freezegun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-23 18:33:19.000000 freezegun-1.5.0/freezegun/_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34845 2024-04-23 18:33:19.000000 freezegun-1.5.0/freezegun/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-23 18:33:19.000000 freezegun-1.5.0/freezegun/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:33:19.000000 freezegun-1.5.0/freezegun/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:33:39.480508 freezegun-1.5.0/freezegun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-23 18:33:39.000000 freezegun-1.5.0/freezegun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-23 18:33:39.000000 freezegun-1.5.0/freezegun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:33:39.000000 freezegun-1.5.0/freezegun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 18:33:39.000000 freezegun-1.5.0/freezegun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 18:33:39.000000 freezegun-1.5.0/freezegun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 18:33:19.000000 freezegun-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 18:33:19.000000 freezegun-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-23 18:33:39.480508 freezegun-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 18:33:19.000000 freezegun-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:33:39.480508 freezegun-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/another_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/fake_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/test_class_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/test_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/test_datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/test_import_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/test_sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/test_ticking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/test_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/test_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-23 18:33:19.000000 freezegun-1.5.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-23 18:33:19.000000 freezegun-1.5.0/tox.ini
```

### Comparing `freezegun-1.4.0/AUTHORS.rst` & `freezegun-1.5.0/AUTHORS.rst`

 * *Files 6% similar despite different names*

```diff
@@ -17,7 +17,9 @@
 - `Dan Elkis <github.com/rinslow>`_
 - `Bastien Vallet <github.com/djailla>`_
 - `Julian Mehnle <github.com/jmehnle>`_
 - `Lukasz Balcerzak <https://github.com/lukaszb>`_
 - `Hannes Ljungberg <hannes@5monkeys.se>`_
 - `staticdev <staticdev-support@proton.me>`_
 - `Marcin Sulikowski <https://github.com/marcinsulikowski>`_
+- `Ashish Patil <https://github.com/ashishnitinpatil>`_
+- `Victor Ferrer <https://github.com/vicfergar>`_
```

### Comparing `freezegun-1.4.0/CHANGELOG` & `freezegun-1.5.0/CHANGELOG`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Freezegun Changelog
 ===================
 
+1.5.0
+----
+ * The default ignore list now contains the `queue`-package
+ * Added a missing `move_to`-function when calling `freeze_time(tick=True)`
+ * Fixes a rounding error in `time.time_ns()`
+ * Fixed a bug where the default ignore list could not be empty (`configure(default_ignore_list=[])`)
+ * All `tick()` methods now return the new datetime (instead of None)
+ * Type improvements
+
 1.4.0
 -----
  * `asyncio`-support from 1.3.x introduced quite a few  bugs, so that functionality is now hidden behind a flag:
    `with freeze_time('1970-01-02', real_asyncio=True):`
 
 1.3.1
 -----
```

### Comparing `freezegun-1.4.0/LICENSE` & `freezegun-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freezegun-1.4.0/PKG-INFO` & `freezegun-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freezegun
-Version: 1.4.0
+Version: 1.5.0
 Summary: Let your Python tests travel through time
 Home-page: https://github.com/spulec/freezegun
 Author: Steve Pulec
 Author-email: spulec@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/spulec/freezegun/issues
 Project-URL: Changes, https://github.com/spulec/freezegun/blob/master/CHANGELOG
```

### Comparing `freezegun-1.4.0/README.rst` & `freezegun-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `freezegun-1.4.0/freezegun/_async.py` & `freezegun-1.5.0/freezegun/_async.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.4.0/freezegun/api.py` & `freezegun-1.5.0/freezegun/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,29 +11,41 @@
 import calendar
 import unittest
 import platform
 import warnings
 import types
 import numbers
 import inspect
+from typing import TYPE_CHECKING, overload
+from typing import Any, Awaitable, Callable, Dict, Iterator, List, Optional, Set, Type, TypeVar, Tuple, Union
 
 from dateutil import parser
 from dateutil.tz import tzlocal
 
 try:
-    from maya import MayaDT
+    from maya import MayaDT  # type: ignore
 except ImportError:
     MayaDT = None
 
+if TYPE_CHECKING:
+    from typing_extensions import ParamSpec
+
+    P = ParamSpec("P")
+
+T = TypeVar("T")
+
 _TIME_NS_PRESENT = hasattr(time, 'time_ns')
 _MONOTONIC_NS_PRESENT = hasattr(time, 'monotonic_ns')
 _PERF_COUNTER_NS_PRESENT = hasattr(time, 'perf_counter_ns')
 _EPOCH = datetime.datetime(1970, 1, 1)
 _EPOCHTZ = datetime.datetime(1970, 1, 1, tzinfo=dateutil.tz.UTC)
 
+T2 = TypeVar("T2")
+_Freezable = Union[str, datetime.datetime,  datetime.date,  datetime.timedelta,  types.FunctionType,  Callable[[], Union[str, datetime.datetime, datetime.date, datetime.timedelta]], Iterator[datetime.datetime]]
+
 real_time = time.time
 real_localtime = time.localtime
 real_gmtime = time.gmtime
 real_monotonic = time.monotonic
 real_perf_counter = time.perf_counter
 real_strftime = time.strftime
 real_date = datetime.date
@@ -53,46 +65,48 @@
     real_date_objects.append(real_perf_counter_ns)
 
 _real_time_object_ids = {id(obj) for obj in real_date_objects}
 
 # time.clock is deprecated and was removed in Python 3.8
 real_clock = getattr(time, 'clock', None)
 
-freeze_factories = []
-tz_offsets = []
-ignore_lists = []
-tick_flags = []
+freeze_factories: List[Union["StepTickTimeFactory", "TickingDateTimeFactory", "FrozenDateTimeFactory"]] = []
+tz_offsets: List[datetime.timedelta] = []
+ignore_lists: List[Tuple[str, ...]] = []
+tick_flags: List[bool] = []
 
 try:
     # noinspection PyUnresolvedReferences
-    real_uuid_generate_time = uuid._uuid_generate_time
+    real_uuid_generate_time = uuid._uuid_generate_time  # type: ignore
     uuid_generate_time_attr = '_uuid_generate_time'
 except AttributeError:
     # noinspection PyUnresolvedReferences
-    uuid._load_system_functions()
+    if hasattr(uuid, '_load_system_functions'):
+        # A no-op after Python ~3.9, being removed in 3.13.
+        uuid._load_system_functions()
     # noinspection PyUnresolvedReferences
-    real_uuid_generate_time = uuid._generate_time_safe
+    real_uuid_generate_time = uuid._generate_time_safe  # type: ignore
     uuid_generate_time_attr = '_generate_time_safe'
 except ImportError:
     real_uuid_generate_time = None
-    uuid_generate_time_attr = None
+    uuid_generate_time_attr = None  # type: ignore
 
 try:
     # noinspection PyUnresolvedReferences
-    real_uuid_create = uuid._UuidCreate
+    real_uuid_create = uuid._UuidCreate  # type: ignore
 except (AttributeError, ImportError):
     real_uuid_create = None
 
 
 # keep a cache of module attributes otherwise freezegun will need to analyze too many modules all the time
-_GLOBAL_MODULES_CACHE = {}
+_GLOBAL_MODULES_CACHE: Dict[str, Tuple[str, List[Tuple[str, Any]]]] = {}
 
 
-def _get_module_attributes(module):
-    result = []
+def _get_module_attributes(module: types.ModuleType) -> List[Tuple[str, Any]]:
+    result: List[Tuple[str, Any]] = []
     try:
         module_attributes = dir(module)
     except (ImportError, TypeError):
         return result
     for attribute_name in module_attributes:
         try:
             attribute_value = getattr(module, attribute_name)
@@ -100,32 +114,32 @@
             # For certain libraries, this can result in ImportError(_winreg) or AttributeError (celery)
             continue
         else:
             result.append((attribute_name, attribute_value))
     return result
 
 
-def _setup_module_cache(module):
+def _setup_module_cache(module: types.ModuleType) -> None:
     date_attrs = []
     all_module_attributes = _get_module_attributes(module)
     for attribute_name, attribute_value in all_module_attributes:
         if id(attribute_value) in _real_time_object_ids:
             date_attrs.append((attribute_name, attribute_value))
     _GLOBAL_MODULES_CACHE[module.__name__] = (_get_module_attributes_hash(module), date_attrs)
 
 
-def _get_module_attributes_hash(module):
+def _get_module_attributes_hash(module: types.ModuleType) -> str:
     try:
         module_dir = dir(module)
     except (ImportError, TypeError):
         module_dir = []
     return f'{id(module)}-{hash(frozenset(module_dir))}'
 
 
-def _get_cached_module_attributes(module):
+def _get_cached_module_attributes(module: types.ModuleType) -> List[Tuple[str, Any]]:
     module_hash, cached_attrs = _GLOBAL_MODULES_CACHE.get(module.__name__, ('0', []))
     if _get_module_attributes_hash(module) == module_hash:
         return cached_attrs
 
     # cache miss: update the cache and return the refreshed value
     _setup_module_cache(module)
     # return the newly cached value
@@ -138,481 +152,518 @@
     platform.python_implementation().lower() == "cpython"
 )
 
 
 call_stack_inspection_limit = 5
 
 
-def _should_use_real_time():
+def _should_use_real_time() -> bool:
     if not call_stack_inspection_limit:
         return False
 
     # Means stop() has already been called, so we can now return the real time
     if not ignore_lists:
         return True
 
     if not ignore_lists[-1]:
         return False
 
-    frame = inspect.currentframe().f_back.f_back
+    frame = inspect.currentframe().f_back.f_back  # type: ignore
 
     for _ in range(call_stack_inspection_limit):
-        module_name = frame.f_globals.get('__name__')
+        module_name = frame.f_globals.get('__name__')  # type: ignore
         if module_name and module_name.startswith(ignore_lists[-1]):
             return True
 
-        frame = frame.f_back
+        frame = frame.f_back  # type: ignore
         if frame is None:
             break
 
     return False
 
 
-def get_current_time():
+def get_current_time() -> datetime.datetime:
     return freeze_factories[-1]()
 
 
-def fake_time():
+def fake_time() -> float:
     if _should_use_real_time():
         return real_time()
     current_time = get_current_time()
     return calendar.timegm(current_time.timetuple()) + current_time.microsecond / 1000000.0
 
 if _TIME_NS_PRESENT:
-    def fake_time_ns():
+    def fake_time_ns() -> int:
         if _should_use_real_time():
             return real_time_ns()
-        return int(int(fake_time()) * 1e9)
+        return int(fake_time() * 1e9)
 
 
-def fake_localtime(t=None):
+def fake_localtime(t: Optional[float]=None) -> time.struct_time:
     if t is not None:
         return real_localtime(t)
     if _should_use_real_time():
         return real_localtime()
     shifted_time = get_current_time() - datetime.timedelta(seconds=time.timezone)
     return shifted_time.timetuple()
 
 
-def fake_gmtime(t=None):
+def fake_gmtime(t: Optional[float]=None) -> time.struct_time:
     if t is not None:
         return real_gmtime(t)
     if _should_use_real_time():
         return real_gmtime()
     return get_current_time().timetuple()
 
 
-def _get_fake_monotonic():
+def _get_fake_monotonic() -> float:
     # For monotonic timers like .monotonic(), .perf_counter(), etc
     current_time = get_current_time()
     return (
         calendar.timegm(current_time.timetuple()) +
         current_time.microsecond / 1e6
     )
 
 
-def _get_fake_monotonic_ns():
+def _get_fake_monotonic_ns() -> int:
     # For monotonic timers like .monotonic(), .perf_counter(), etc
     current_time = get_current_time()
     return (
         calendar.timegm(current_time.timetuple()) * 1000000 +
         current_time.microsecond
     ) * 1000
 
 
-def fake_monotonic():
+def fake_monotonic() -> float:
     if _should_use_real_time():
         return real_monotonic()
 
     return _get_fake_monotonic()
 
 
-def fake_perf_counter():
+def fake_perf_counter() -> float:
     if _should_use_real_time():
         return real_perf_counter()
 
     return _get_fake_monotonic()
 
 
 if _MONOTONIC_NS_PRESENT:
-    def fake_monotonic_ns():
+    def fake_monotonic_ns() -> int:
         if _should_use_real_time():
             return real_monotonic_ns()
 
         return _get_fake_monotonic_ns()
 
 
 if _PERF_COUNTER_NS_PRESENT:
-    def fake_perf_counter_ns():
+    def fake_perf_counter_ns() -> int:
         if _should_use_real_time():
             return real_perf_counter_ns()
         return _get_fake_monotonic_ns()
 
 
-def fake_strftime(format, time_to_format=None):
+def fake_strftime(format: Any, time_to_format: Any=None) -> str:
     if time_to_format is None:
         if not _should_use_real_time():
             time_to_format = fake_localtime()
 
     if time_to_format is None:
         return real_strftime(format)
     else:
         return real_strftime(format, time_to_format)
 
 if real_clock is not None:
-    def fake_clock():
+    def fake_clock() -> Any:
         if _should_use_real_time():
-            return real_clock()
+            return real_clock()  # type: ignore
 
         if len(freeze_factories) == 1:
-            return 0.0 if not tick_flags[-1] else real_clock()
+            return 0.0 if not tick_flags[-1] else real_clock()  # type: ignore
 
         first_frozen_time = freeze_factories[0]()
         last_frozen_time = get_current_time()
 
         timedelta = (last_frozen_time - first_frozen_time)
         total_seconds = timedelta.total_seconds()
 
         if tick_flags[-1]:
-            total_seconds += real_clock()
+            total_seconds += real_clock()  # type: ignore
 
         return total_seconds
 
 
 class FakeDateMeta(type):
     @classmethod
-    def __instancecheck__(self, obj):
+    def __instancecheck__(self, obj: Any) -> bool:
         return isinstance(obj, real_date)
 
     @classmethod
-    def __subclasscheck__(cls, subclass):
+    def __subclasscheck__(cls, subclass: Any) -> bool:
         return issubclass(subclass, real_date)
 
 
-def datetime_to_fakedatetime(datetime):
+def datetime_to_fakedatetime(datetime: datetime.datetime) -> "FakeDatetime":
     return FakeDatetime(datetime.year,
                         datetime.month,
                         datetime.day,
                         datetime.hour,
                         datetime.minute,
                         datetime.second,
                         datetime.microsecond,
                         datetime.tzinfo)
 
 
-def date_to_fakedate(date):
+def date_to_fakedate(date: datetime.date) -> "FakeDate":
     return FakeDate(date.year,
                     date.month,
                     date.day)
 
 
 class FakeDate(real_date, metaclass=FakeDateMeta):
-    def __add__(self, other):
+    def __add__(self, other: Any) -> "FakeDate":
         result = real_date.__add__(self, other)
         if result is NotImplemented:
             return result
         return date_to_fakedate(result)
 
-    def __sub__(self, other):
+    def __sub__(self, other: Any) -> "FakeDate":  # type: ignore
         result = real_date.__sub__(self, other)
         if result is NotImplemented:
-            return result
+            return result  # type: ignore
         if isinstance(result, real_date):
             return date_to_fakedate(result)
         else:
-            return result
+            return result  # type: ignore
 
     @classmethod
-    def today(cls):
+    def today(cls: Type["FakeDate"]) -> "FakeDate":
         result = cls._date_to_freeze() + cls._tz_offset()
         return date_to_fakedate(result)
 
     @staticmethod
-    def _date_to_freeze():
+    def _date_to_freeze() -> datetime.datetime:
         return get_current_time()
 
     @classmethod
-    def _tz_offset(cls):
+    def _tz_offset(cls) -> datetime.timedelta:
         return tz_offsets[-1]
 
 FakeDate.min = date_to_fakedate(real_date.min)
 FakeDate.max = date_to_fakedate(real_date.max)
 
 
 class FakeDatetimeMeta(FakeDateMeta):
     @classmethod
-    def __instancecheck__(self, obj):
+    def __instancecheck__(self, obj: Any) -> bool:
         return isinstance(obj, real_datetime)
 
     @classmethod
-    def __subclasscheck__(cls, subclass):
+    def __subclasscheck__(cls, subclass: Any) -> bool:
         return issubclass(subclass, real_datetime)
 
 
 class FakeDatetime(real_datetime, FakeDate, metaclass=FakeDatetimeMeta):
-    def __add__(self, other):
+    def __add__(self, other: Any) -> "FakeDatetime":  # type: ignore
         result = real_datetime.__add__(self, other)
         if result is NotImplemented:
             return result
         return datetime_to_fakedatetime(result)
 
-    def __sub__(self, other):
+    def __sub__(self, other: Any) -> "FakeDatetime":  # type: ignore
         result = real_datetime.__sub__(self, other)
         if result is NotImplemented:
-            return result
+            return result  # type: ignore
         if isinstance(result, real_datetime):
             return datetime_to_fakedatetime(result)
         else:
-            return result
+            return result  # type: ignore
 
-    def astimezone(self, tz=None):
+    def astimezone(self, tz: Optional[datetime.tzinfo]=None) -> "FakeDatetime":
         if tz is None:
             tz = tzlocal()
         return datetime_to_fakedatetime(real_datetime.astimezone(self, tz))
 
     @classmethod
-    def fromtimestamp(cls, t, tz=None):
+    def fromtimestamp(cls, t: float, tz: Optional[datetime.tzinfo]=None) -> "FakeDatetime":
         if tz is None:
-            return real_datetime.fromtimestamp(
-                    t, tz=dateutil.tz.tzoffset("freezegun", cls._tz_offset())
-                ).replace(tzinfo=None)
-        return datetime_to_fakedatetime(real_datetime.fromtimestamp(t, tz))
+            tz = dateutil.tz.tzoffset("freezegun", cls._tz_offset())
+            result = real_datetime.fromtimestamp(t, tz=tz).replace(tzinfo=None)
+        else:
+            result = real_datetime.fromtimestamp(t, tz)
+        return datetime_to_fakedatetime(result)
 
-    def timestamp(self):
+    def timestamp(self) -> float:
         if self.tzinfo is None:
-            return (self - _EPOCH - self._tz_offset()).total_seconds()
-        return (self - _EPOCHTZ).total_seconds()
+            return (self - _EPOCH - self._tz_offset()).total_seconds()  # type: ignore
+        return (self - _EPOCHTZ).total_seconds()  # type: ignore
 
     @classmethod
-    def now(cls, tz=None):
+    def now(cls, tz: Optional[datetime.tzinfo] = None) -> "FakeDatetime":
         now = cls._time_to_freeze() or real_datetime.now()
         if tz:
             result = tz.fromutc(now.replace(tzinfo=tz)) + cls._tz_offset()
         else:
             result = now + cls._tz_offset()
         return datetime_to_fakedatetime(result)
 
-    def date(self):
+    def date(self) -> "FakeDate":
         return date_to_fakedate(self)
 
     @property
-    def nanosecond(self):
+    def nanosecond(self) -> int:
         try:
             # noinspection PyUnresolvedReferences
-            return real_datetime.nanosecond
+            return real_datetime.nanosecond  # type: ignore
         except AttributeError:
             return 0
 
     @classmethod
-    def today(cls):
+    def today(cls) -> "FakeDatetime":
         return cls.now(tz=None)
 
     @classmethod
-    def utcnow(cls):
+    def utcnow(cls) -> "FakeDatetime":
         result = cls._time_to_freeze() or real_datetime.now(datetime.timezone.utc)
         return datetime_to_fakedatetime(result)
 
     @staticmethod
-    def _time_to_freeze():
+    def _time_to_freeze() -> Optional[datetime.datetime]:
         if freeze_factories:
             return get_current_time()
+        return None
 
     @classmethod
-    def _tz_offset(cls):
+    def _tz_offset(cls) -> datetime.timedelta:
         return tz_offsets[-1]
 
 
 FakeDatetime.min = datetime_to_fakedatetime(real_datetime.min)
 FakeDatetime.max = datetime_to_fakedatetime(real_datetime.max)
 
 
-def convert_to_timezone_naive(time_to_freeze):
+def convert_to_timezone_naive(time_to_freeze: datetime.datetime) -> datetime.datetime:
     """
     Converts a potentially timezone-aware datetime to be a naive UTC datetime
     """
     if time_to_freeze.tzinfo:
-        time_to_freeze -= time_to_freeze.utcoffset()
+        time_to_freeze -= time_to_freeze.utcoffset()  # type: ignore
         time_to_freeze = time_to_freeze.replace(tzinfo=None)
     return time_to_freeze
 
 
-def pickle_fake_date(datetime_):
+def pickle_fake_date(datetime_: datetime.date) -> Tuple[Type[FakeDate], Tuple[int, int, int]]:
     # A pickle function for FakeDate
     return FakeDate, (
         datetime_.year,
         datetime_.month,
         datetime_.day,
     )
 
 
-def pickle_fake_datetime(datetime_):
+def pickle_fake_datetime(datetime_: datetime.datetime) -> Tuple[Type[FakeDatetime], Tuple[int, int, int, int, int, int, int, Optional[datetime.tzinfo]]]:
     # A pickle function for FakeDatetime
     return FakeDatetime, (
         datetime_.year,
         datetime_.month,
         datetime_.day,
         datetime_.hour,
         datetime_.minute,
         datetime_.second,
         datetime_.microsecond,
         datetime_.tzinfo,
     )
 
 
-def _parse_time_to_freeze(time_to_freeze_str):
+def _parse_time_to_freeze(time_to_freeze_str: Optional[_Freezable]) -> datetime.datetime:
     """Parses all the possible inputs for freeze_time
     :returns: a naive ``datetime.datetime`` object
     """
     if time_to_freeze_str is None:
         time_to_freeze_str = datetime.datetime.now(datetime.timezone.utc)
 
     if isinstance(time_to_freeze_str, datetime.datetime):
         time_to_freeze = time_to_freeze_str
     elif isinstance(time_to_freeze_str, datetime.date):
         time_to_freeze = datetime.datetime.combine(time_to_freeze_str, datetime.time())
     elif isinstance(time_to_freeze_str, datetime.timedelta):
         time_to_freeze = datetime.datetime.now(datetime.timezone.utc) + time_to_freeze_str
     else:
-        time_to_freeze = parser.parse(time_to_freeze_str)
+        time_to_freeze = parser.parse(time_to_freeze_str)  # type: ignore
 
     return convert_to_timezone_naive(time_to_freeze)
 
 
-def _parse_tz_offset(tz_offset):
+def _parse_tz_offset(tz_offset: Union[datetime.timedelta, float]) -> datetime.timedelta:
     if isinstance(tz_offset, datetime.timedelta):
         return tz_offset
     else:
         return datetime.timedelta(hours=tz_offset)
 
 
 class TickingDateTimeFactory:
 
-    def __init__(self, time_to_freeze, start):
+    def __init__(self, time_to_freeze: datetime.datetime, start: datetime.datetime):
         self.time_to_freeze = time_to_freeze
         self.start = start
 
-    def __call__(self):
+    def __call__(self) -> datetime.datetime:
         return self.time_to_freeze + (real_datetime.now() - self.start)
 
+    def tick(self, delta: Union[datetime.timedelta, int]=datetime.timedelta(seconds=1)) -> datetime.datetime:
+        if isinstance(delta, numbers.Real):
+            # noinspection PyTypeChecker
+            self.move_to(self.time_to_freeze + datetime.timedelta(seconds=delta))
+        else:
+            self.move_to(self.time_to_freeze + delta)  # type: ignore
+        return self.time_to_freeze
+
+    def move_to(self, target_datetime: _Freezable) -> None:
+        """Moves frozen date to the given ``target_datetime``"""
+        self.start = real_datetime.now()
+        self.time_to_freeze = _parse_time_to_freeze(target_datetime)
+
 
 class FrozenDateTimeFactory:
 
-    def __init__(self, time_to_freeze):
+    def __init__(self, time_to_freeze: datetime.datetime):
         self.time_to_freeze = time_to_freeze
 
-    def __call__(self):
+    def __call__(self) -> datetime.datetime:
         return self.time_to_freeze
 
-    def tick(self, delta=datetime.timedelta(seconds=1)):
+    def tick(self, delta: Union[datetime.timedelta, int]=datetime.timedelta(seconds=1)) -> datetime.datetime:
         if isinstance(delta, numbers.Real):
             # noinspection PyTypeChecker
             self.time_to_freeze += datetime.timedelta(seconds=delta)
         else:
-            self.time_to_freeze += delta
+            self.time_to_freeze += delta  # type: ignore
+        return self.time_to_freeze
 
-    def move_to(self, target_datetime):
+    def move_to(self, target_datetime: _Freezable) -> None:
         """Moves frozen date to the given ``target_datetime``"""
         target_datetime = _parse_time_to_freeze(target_datetime)
         delta = target_datetime - self.time_to_freeze
         self.tick(delta=delta)
 
 
 class StepTickTimeFactory:
 
-    def __init__(self, time_to_freeze, step_width):
+    def __init__(self, time_to_freeze: datetime.datetime, step_width: float):
         self.time_to_freeze = time_to_freeze
         self.step_width = step_width
 
-    def __call__(self):
+    def __call__(self) -> datetime.datetime:
         return_time = self.time_to_freeze
         self.tick()
         return return_time
 
-    def tick(self, delta=None):
+    def tick(self, delta: Union[datetime.timedelta, int, None]=None) -> datetime.datetime:
         if not delta:
             delta = datetime.timedelta(seconds=self.step_width)
-        self.time_to_freeze += delta
+        self.time_to_freeze += delta  # type: ignore
+        return self.time_to_freeze
 
-    def update_step_width(self, step_width):
+    def update_step_width(self, step_width: float) -> None:
         self.step_width = step_width
 
-    def move_to(self, target_datetime):
+    def move_to(self, target_datetime: _Freezable) -> None:
         """Moves frozen date to the given ``target_datetime``"""
         target_datetime = _parse_time_to_freeze(target_datetime)
         delta = target_datetime - self.time_to_freeze
         self.tick(delta=delta)
 
 
 class _freeze_time:
 
-    def __init__(self, time_to_freeze_str, tz_offset, ignore, tick, as_arg, as_kwarg, auto_tick_seconds, real_asyncio):
+    def __init__(
+        self,
+        time_to_freeze_str: Optional[_Freezable],
+        tz_offset: Union[int, datetime.timedelta],
+        ignore: List[str],
+        tick: bool,
+        as_arg: bool,
+        as_kwarg: str,
+        auto_tick_seconds: float,
+        real_asyncio: Optional[bool],
+    ):
         self.time_to_freeze = _parse_time_to_freeze(time_to_freeze_str)
         self.tz_offset = _parse_tz_offset(tz_offset)
         self.ignore = tuple(ignore)
         self.tick = tick
         self.auto_tick_seconds = auto_tick_seconds
-        self.undo_changes = []
-        self.modules_at_start = set()
+        self.undo_changes: List[Tuple[types.ModuleType, str, Any]] = []
+        self.modules_at_start: Set[str] = set()
         self.as_arg = as_arg
         self.as_kwarg = as_kwarg
         self.real_asyncio = real_asyncio
 
-    def __call__(self, func):
+    @overload
+    def __call__(self, func: Type[T2]) -> Type[T2]:
+        ...
+
+    @overload
+    def __call__(self, func: "Callable[P, Awaitable[Any]]") -> "Callable[P, Awaitable[Any]]":
+        ...
+
+    @overload
+    def __call__(self, func: "Callable[P, T]") -> "Callable[P, T]":
+        ...
+
+    def __call__(self, func: Union[Type[T2], "Callable[P, Awaitable[Any]]", "Callable[P, T]"]) -> Union[Type[T2], "Callable[P, Awaitable[Any]]", "Callable[P, T]"]:  # type: ignore
         if inspect.isclass(func):
             return self.decorate_class(func)
         elif inspect.iscoroutinefunction(func):
             return self.decorate_coroutine(func)
-        return self.decorate_callable(func)
+        return self.decorate_callable(func)  # type: ignore
 
-    def decorate_class(self, klass):
+    def decorate_class(self, klass: Type[T2]) -> Type[T2]:
         if issubclass(klass, unittest.TestCase):
             # If it's a TestCase, we freeze time around setup and teardown, as well
             # as for every test case. This requires some care to avoid freezing
             # the time pytest sees, as otherwise this would distort the reported
             # timings.
 
             orig_setUpClass = klass.setUpClass
             orig_tearDownClass = klass.tearDownClass
 
             # noinspection PyDecorator
-            @classmethod
-            def setUpClass(cls):
+            @classmethod  # type: ignore
+            def setUpClass(cls: type) -> None:
                 self.start()
                 if orig_setUpClass is not None:
                     orig_setUpClass()
                 self.stop()
 
             # noinspection PyDecorator
-            @classmethod
-            def tearDownClass(cls):
+            @classmethod  # type: ignore
+            def tearDownClass(cls: type) -> None:
                 self.start()
                 if orig_tearDownClass is not None:
                     orig_tearDownClass()
                 self.stop()
 
-            klass.setUpClass = setUpClass
-            klass.tearDownClass = tearDownClass
+            klass.setUpClass = setUpClass  # type: ignore
+            klass.tearDownClass = tearDownClass  # type: ignore
 
             orig_setUp = klass.setUp
             orig_tearDown = klass.tearDown
 
-            def setUp(*args, **kwargs):
+            def setUp(*args: Any, **kwargs: Any) -> None:
                 self.start()
                 if orig_setUp is not None:
                     orig_setUp(*args, **kwargs)
 
-            def tearDown(*args, **kwargs):
+            def tearDown(*args: Any, **kwargs: Any) -> None:
                 if orig_tearDown is not None:
                     orig_tearDown(*args, **kwargs)
                 self.stop()
 
-            klass.setUp = setUp
-            klass.tearDown = tearDown
-
-            return klass
+            klass.setUp = setUp  # type: ignore[method-assign]
+            klass.tearDown = tearDown  # type: ignore[method-assign]
 
         else:
 
             seen = set()
 
             klasses = klass.mro()
             for base_klass in klasses:
@@ -625,26 +676,26 @@
                         continue
 
                     try:
                         setattr(klass, attr, self(attr_value))
                     except (AttributeError, TypeError):
                         # Sometimes we can't set this for built-in types and custom callables
                         continue
-            return klass
+        return klass
 
-    def __enter__(self):
+    def __enter__(self) -> Union[StepTickTimeFactory, TickingDateTimeFactory, FrozenDateTimeFactory]:
         return self.start()
 
-    def __exit__(self, *args):
+    def __exit__(self, *args: Any) -> None:
         self.stop()
 
-    def start(self):
+    def start(self) -> Union[StepTickTimeFactory, TickingDateTimeFactory, FrozenDateTimeFactory]:
 
         if self.auto_tick_seconds:
-            freeze_factory = StepTickTimeFactory(self.time_to_freeze, self.auto_tick_seconds)
+            freeze_factory: Union[StepTickTimeFactory, TickingDateTimeFactory, FrozenDateTimeFactory] = StepTickTimeFactory(self.time_to_freeze, self.auto_tick_seconds)
         elif self.tick:
             freeze_factory = TickingDateTimeFactory(self.time_to_freeze, real_datetime.now())
         else:
             freeze_factory = FrozenDateTimeFactory(self.time_to_freeze)
 
         is_already_started = len(freeze_factories) > 0
         freeze_factories.append(freeze_factory)
@@ -652,27 +703,27 @@
         ignore_lists.append(self.ignore)
         tick_flags.append(self.tick)
 
         if is_already_started:
             return freeze_factory
 
         # Change the modules
-        datetime.datetime = FakeDatetime
-        datetime.date = FakeDate
+        datetime.datetime = FakeDatetime  # type: ignore[misc]
+        datetime.date = FakeDate  # type: ignore[misc]
 
         time.time = fake_time
         time.monotonic = fake_monotonic
         time.perf_counter = fake_perf_counter
-        time.localtime = fake_localtime
-        time.gmtime = fake_gmtime
-        time.strftime = fake_strftime
+        time.localtime = fake_localtime  # type: ignore
+        time.gmtime = fake_gmtime  # type: ignore
+        time.strftime = fake_strftime  # type: ignore
         if uuid_generate_time_attr:
             setattr(uuid, uuid_generate_time_attr, None)
-        uuid._UuidCreate = None
-        uuid._last_timestamp = None
+        uuid._UuidCreate = None  # type: ignore[attr-defined]
+        uuid._last_timestamp = None  # type: ignore[attr-defined]
 
         copyreg.dispatch_table[real_datetime] = pickle_fake_datetime
         copyreg.dispatch_table[real_date] = pickle_fake_date
 
         # Change any place where the module had already been imported
         to_patch = [
             ('real_date', real_date, FakeDate),
@@ -695,18 +746,18 @@
 
         if _PERF_COUNTER_NS_PRESENT:
             time.perf_counter_ns = fake_perf_counter_ns
             to_patch.append(('real_perf_counter_ns', real_perf_counter_ns, fake_perf_counter_ns))
 
         if real_clock is not None:
             # time.clock is deprecated and was removed in Python 3.8
-            time.clock = fake_clock
+            time.clock = fake_clock  # type: ignore[attr-defined]
             to_patch.append(('real_clock', real_clock, fake_clock))
 
-        self.fake_names = tuple(fake.__name__ for real_name, real, fake in to_patch)
+        self.fake_names = tuple(fake.__name__ for real_name, real, fake in to_patch)  # type: ignore
         self.reals = {id(fake): real for real_name, real, fake in to_patch}
         fakes = {id(real): fake for real_name, real, fake in to_patch}
         add_change = self.undo_changes.append
 
         # Save the current loaded modules
         self.modules_at_start = set(sys.modules.keys())
 
@@ -737,28 +788,28 @@
             # Note that we cannot statically tell the class of asyncio event loops
             # because it is not officially documented and can actually be changed
             # at run time using `asyncio.set_event_loop_policy`. That's why we check
             # the type by creating a loop here and destroying it immediately.
             event_loop = asyncio.new_event_loop()
             event_loop.close()
             EventLoopClass = type(event_loop)
-            add_change((EventLoopClass, "time", EventLoopClass.time))
-            EventLoopClass.time = lambda self: real_monotonic()
+            add_change((EventLoopClass, "time", EventLoopClass.time))  # type: ignore
+            EventLoopClass.time = lambda self: real_monotonic()  # type: ignore[method-assign]
 
         return freeze_factory
 
-    def stop(self):
+    def stop(self) -> None:
         freeze_factories.pop()
         ignore_lists.pop()
         tick_flags.pop()
         tz_offsets.pop()
 
         if not freeze_factories:
-            datetime.datetime = real_datetime
-            datetime.date = real_date
+            datetime.datetime = real_datetime  # type: ignore[misc]
+            datetime.date = real_date  # type: ignore[misc]
             copyreg.dispatch_table.pop(real_datetime)
             copyreg.dispatch_table.pop(real_date)
             for module_or_object, attribute, original_value in self.undo_changes:
                 setattr(module_or_object, attribute, original_value)
             self.undo_changes = []
 
             # Restore modules loaded after start()
@@ -790,54 +841,54 @@
 
             time.time = real_time
             time.monotonic = real_monotonic
             time.perf_counter = real_perf_counter
             time.gmtime = real_gmtime
             time.localtime = real_localtime
             time.strftime = real_strftime
-            time.clock = real_clock
+            time.clock = real_clock  # type: ignore[attr-defined]
 
             if _TIME_NS_PRESENT:
                 time.time_ns = real_time_ns
 
             if _MONOTONIC_NS_PRESENT:
                 time.monotonic_ns = real_monotonic_ns
 
             if _PERF_COUNTER_NS_PRESENT:
                 time.perf_counter_ns = real_perf_counter_ns
 
             if uuid_generate_time_attr:
                 setattr(uuid, uuid_generate_time_attr, real_uuid_generate_time)
-            uuid._UuidCreate = real_uuid_create
-            uuid._last_timestamp = None
+            uuid._UuidCreate = real_uuid_create  # type: ignore[attr-defined]
+            uuid._last_timestamp = None  # type: ignore[attr-defined]
 
-    def decorate_coroutine(self, coroutine):
+    def decorate_coroutine(self, coroutine: "Callable[P, Awaitable[T]]") -> "Callable[P, Awaitable[T]]":
         return wrap_coroutine(self, coroutine)
 
-    def decorate_callable(self, func):
-        def wrapper(*args, **kwargs):
+    def decorate_callable(self, func: "Callable[P, T]") -> "Callable[P, T]":
+        @functools.wraps(func)
+        def wrapper(*args: "P.args", **kwargs: "P.kwargs") -> T:
             with self as time_factory:
                 if self.as_arg and self.as_kwarg:
                     assert False, "You can't specify both as_arg and as_kwarg at the same time. Pick one."
                 elif self.as_arg:
-                    result = func(time_factory, *args, **kwargs)
+                    result = func(time_factory, *args, **kwargs)  # type: ignore
                 elif self.as_kwarg:
                     kwargs[self.as_kwarg] = time_factory
                     result = func(*args, **kwargs)
                 else:
                     result = func(*args, **kwargs)
             return result
-        functools.update_wrapper(wrapper, func)
 
         return wrapper
 
 
-def freeze_time(time_to_freeze=None, tz_offset=0, ignore=None, tick=False, as_arg=False, as_kwarg='',
-                auto_tick_seconds=0, real_asyncio=False):
-    acceptable_times = (type(None), str, datetime.date, datetime.timedelta,
+def freeze_time(time_to_freeze: Optional[_Freezable]=None, tz_offset: Union[int, datetime.timedelta]=0, ignore: Optional[List[str]]=None, tick: bool=False, as_arg: bool=False, as_kwarg: str='',
+                auto_tick_seconds: float=0, real_asyncio: bool=False) -> _freeze_time:
+    acceptable_times: Any = (type(None), str, datetime.date, datetime.timedelta,
              types.FunctionType, types.GeneratorType)
 
     if MayaDT is not None:
         acceptable_times += MayaDT,
 
     if not isinstance(time_to_freeze, acceptable_times):
         raise TypeError(('freeze_time() expected None, a string, date instance, datetime '
@@ -879,18 +930,18 @@
     # noinspection PyUnresolvedReferences
     import sqlite3
 except ImportError:
     # Some systems have trouble with this
     pass
 else:
     # These are copied from Python sqlite3.dbapi2
-    def adapt_date(val):
+    def adapt_date(val: datetime.date) -> str:
         return val.isoformat()
 
-    def adapt_datetime(val):
+    def adapt_datetime(val: datetime.datetime) -> str:
         return val.isoformat(" ")
 
     sqlite3.register_adapter(FakeDate, adapt_date)
     sqlite3.register_adapter(FakeDatetime, adapt_datetime)
 
 
 # Setup converters for pymysql
```

### Comparing `freezegun-1.4.0/freezegun/config.py` & `freezegun-1.5.0/freezegun/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 DEFAULT_IGNORE_LIST = [
     'nose.plugins',
     'six.moves',
     'django.utils.six.moves',
     'google.gax',
     'threading',
     'multiprocessing',
-    'Queue',
+    'queue',
     'selenium',
     '_pytest.terminal.',
     '_pytest.runner.',
     'gi',
     'prompt_toolkit',
 ]
 
@@ -28,16 +28,16 @@
 class ConfigurationError(Exception):
     pass
 
 
 def configure(default_ignore_list: Optional[List[str]]=None, extend_ignore_list: Optional[List[str]]=None) -> None:
     if default_ignore_list is not None and extend_ignore_list is not None:
         raise ConfigurationError("Either default_ignore_list or extend_ignore_list might be given, not both")
-    if default_ignore_list:
+    if default_ignore_list is not None:
         settings.default_ignore_list = default_ignore_list
     if extend_ignore_list:
-        settings.default_ignore_list = [*settings.default_ignore_list, *extend_ignore_list]
+        settings.default_ignore_list = list(dict.fromkeys([*settings.default_ignore_list, *extend_ignore_list]))
 
 
 def reset_config() -> None:
     global settings
     settings = Settings()
```

### Comparing `freezegun-1.4.0/freezegun.egg-info/PKG-INFO` & `freezegun-1.5.0/freezegun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freezegun
-Version: 1.4.0
+Version: 1.5.0
 Summary: Let your Python tests travel through time
 Home-page: https://github.com/spulec/freezegun
 Author: Steve Pulec
 Author-email: spulec@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/spulec/freezegun/issues
 Project-URL: Changes, https://github.com/spulec/freezegun/blob/master/CHANGELOG
```

### Comparing `freezegun-1.4.0/freezegun.egg-info/SOURCES.txt` & `freezegun-1.5.0/freezegun.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 README.rst
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 freezegun/__init__.py
-freezegun/__init__.pyi
 freezegun/_async.py
 freezegun/api.py
-freezegun/api.pyi
 freezegun/config.py
 freezegun/py.typed
 freezegun.egg-info/PKG-INFO
 freezegun.egg-info/SOURCES.txt
 freezegun.egg-info/dependency_links.txt
 freezegun.egg-info/requires.txt
 freezegun.egg-info/top_level.txt
```

### Comparing `freezegun-1.4.0/setup.cfg` & `freezegun-1.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `freezegun-1.4.0/tests/another_module.py` & `freezegun-1.5.0/tests/another_module.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,64 @@
 from datetime import date, datetime
 from time import time, localtime, gmtime, strftime
+from typing import Any
 
 from freezegun.api import (
     FakeDatetime,
     FakeDate,
     fake_time,
     fake_localtime,
     fake_gmtime,
     fake_strftime,
 )
 
 
 # Reals
 
-def get_datetime():
+def get_datetime() -> Any:
     return datetime
 
 
-def get_date():
+def get_date() -> Any:
     return date
 
 
-def get_time():
+def get_time() -> Any:
     return time
 
 
-def get_localtime():
+def get_localtime() -> Any:
     return localtime
 
 
-def get_gmtime():
+def get_gmtime() -> Any:
     return gmtime
 
 
-def get_strftime():
+def get_strftime() -> Any:
     return strftime
 
 
 # Fakes
 
-def get_fake_datetime():
+def get_fake_datetime() -> Any:
     return FakeDatetime
 
 
-def get_fake_date():
+def get_fake_date() -> Any:
     return FakeDate
 
 
-def get_fake_time():
+def get_fake_time() -> Any:
     return fake_time
 
 
-def get_fake_localtime():
+def get_fake_localtime() -> Any:
     return fake_localtime
 
 
-def get_fake_gmtime():
+def get_fake_gmtime() -> Any:
     return fake_gmtime
 
 
-def get_fake_strftime():
+def get_fake_strftime() -> Any:
     return fake_strftime
```

### Comparing `freezegun-1.4.0/tests/test_asyncio.py` & `freezegun-1.5.0/tests/test_asyncio.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 import asyncio
 import datetime
 import time
+from typing import Any
 
 from freezegun import freeze_time
 
 
-def test_datetime_in_coroutine():
+def test_datetime_in_coroutine() -> None:
     @freeze_time('1970-01-01')
-    async def frozen_coroutine():
+    async def frozen_coroutine() -> Any:
         assert datetime.date.today() == datetime.date(1970, 1, 1)
 
-    asyncio.run(frozen_coroutine())
+    asyncio.run(frozen_coroutine())  # type: ignore
 
 
-def test_freezing_time_in_coroutine():
+def test_freezing_time_in_coroutine() -> None:
     """Test calling freeze_time while executing asyncio loop."""
-    async def coroutine():
+    async def coroutine() -> None:
         with freeze_time('1970-01-02'):
             assert time.time() == 86400
         with freeze_time('1970-01-03'):
             assert time.time() == 86400 * 2
 
     asyncio.run(coroutine())
 
 
-def test_freezing_time_before_running_coroutine():
+def test_freezing_time_before_running_coroutine() -> None:
     """Test calling freeze_time before executing asyncio loop."""
-    async def coroutine():
+    async def coroutine() -> None:
         assert time.time() == 86400
     with freeze_time('1970-01-02'):
         asyncio.run(coroutine())
 
 
-def test_asyncio_sleeping_not_affected_by_freeze_time():
+def test_asyncio_sleeping_not_affected_by_freeze_time() -> None:
     """Test that asyncio.sleep() is not affected by `freeze_time`.
 
     This test ensures that despite freezing time using `freeze_time`,
     the asyncio event loop can see real monotonic time, which is required
     to make things like `asyncio.sleep()` work.
     """
 
-    async def coroutine():
+    async def coroutine() -> None:
         # Sleeping with time frozen should sleep the expected duration.
         before_sleep = time.time()
         with freeze_time('1970-01-02', real_asyncio=True):
             await asyncio.sleep(0.05)
         assert 0.02 <= time.time() - before_sleep < 0.3
 
         # Exiting `freeze_time` the time should not break asyncio sleeping.
         before_sleep = time.time()
         await asyncio.sleep(0.05)
         assert 0.02 <= time.time() - before_sleep < 0.3
 
     asyncio.run(coroutine())
 
 
-def test_asyncio_to_call_later_with_frozen_time():
+def test_asyncio_to_call_later_with_frozen_time() -> None:
     """Test that asyncio `loop.call_later` works with frozen time."""
     # `to_call_later` will be called by asyncio event loop and should add
     # the Unix timestamp of 1970-01-02 00:00 to the `timestamps` list.
     timestamps = []
-    def to_call_later():
+    def to_call_later() -> None:
         timestamps.append(time.time())
 
-    async def coroutine():
+    async def coroutine() -> None:
         # Schedule calling `to_call_later` in 100 ms.
         asyncio.get_running_loop().call_later(0.1, to_call_later)
 
         # Sleeping for 10 ms should not result in calling `to_call_later`.
         await asyncio.sleep(0.01)
         assert timestamps == []
```

### Comparing `freezegun-1.4.0/tests/test_class_import.py` & `freezegun-1.5.0/tests/test_class_import.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,32 +18,32 @@
     fake_gmtime,
     fake_strftime,
 )
 import datetime
 
 
 @freeze_time("2012-01-14")
-def test_import_datetime_works():
+def test_import_datetime_works() -> None:
     assert fake_datetime_function().day == 14
 
 
 @freeze_time("2012-01-14")
-def test_import_date_works():
+def test_import_date_works() -> None:
     assert fake_date_function().day == 14
 
 
 @freeze_time("2012-01-14")
-def test_import_time():
+def test_import_time() -> None:
     local_time = datetime.datetime(2012, 1, 14)
     utc_time = local_time - datetime.timedelta(seconds=time.timezone)
     expected_timestamp = time.mktime(utc_time.timetuple())
     assert fake_time_function() == expected_timestamp
 
 
-def test_start_and_stop_works():
+def test_start_and_stop_works() -> None:
     freezer = freeze_time("2012-01-14")
 
     result = fake_datetime_function()
     assert result.__class__ == datetime.datetime
     assert result.__class__ != FakeDatetime
 
     freezer.start()
@@ -53,88 +53,88 @@
 
     freezer.stop()
     result = fake_datetime_function()
     assert result.__class__ == datetime.datetime
     assert result.__class__ != FakeDatetime
 
 
-def test_isinstance_works():
+def test_isinstance_works() -> None:
     date = datetime.date.today()
     now = datetime.datetime.now()
 
     freezer = freeze_time('2011-01-01')
     freezer.start()
     assert isinstance(date, datetime.date)
     assert not isinstance(date, datetime.datetime)
     assert isinstance(now, datetime.datetime)
     assert isinstance(now, datetime.date)
     freezer.stop()
 
 
-def test_issubclass_works():
+def test_issubclass_works() -> None:
     real_date = datetime.date
     real_datetime = datetime.datetime
 
     freezer = freeze_time('2011-01-01')
     freezer.start()
     assert issubclass(real_date, datetime.date)
     assert issubclass(real_datetime, datetime.datetime)
     freezer.stop()
 
 
-def test_fake_uses_real_when_ignored():
+def test_fake_uses_real_when_ignored() -> None:
     real_time_before = time.time()
     with freeze_time('2012-01-14', ignore=['tests.fake_module']):
         real_time = fake_time_function()
     real_time_after = time.time()
     assert real_time_before <= real_time <= real_time_after
 
 
-def test_can_ignore_email_module():
+def test_can_ignore_email_module() -> None:
     from email.utils import formatdate
     with freeze_time('2012-01-14'):
         faked_date_str = formatdate()
 
     before_date_str = formatdate()
     with freeze_time('2012-01-14', ignore=['email']):
         date_str = formatdate()
 
     after_date_str = formatdate()
     assert date_str != faked_date_str
     assert before_date_str <= date_str <= after_date_str
 
 
 @freeze_time('2011-01-01')
-def test_avoid_replacing_equal_to_anything():
+def test_avoid_replacing_equal_to_anything() -> None:
     assert fake_module.equal_to_anything.description == 'This is the equal_to_anything object'
 
 
 @freeze_time("2012-01-14 12:00:00")
-def test_import_localtime():
+def test_import_localtime() -> None:
     struct = fake_localtime_function()
     assert struct.tm_year == 2012
     assert struct.tm_mon == 1
     assert struct.tm_mday >= 13  # eg. GMT+14
     assert struct.tm_mday <= 15  # eg. GMT-14
 
 
 @freeze_time("2012-01-14 12:00:00")
-def test_fake_gmtime_function():
+def test_fake_gmtime_function() -> None:
     struct = fake_gmtime_function()
     assert struct.tm_year == 2012
     assert struct.tm_mon == 1
     assert struct.tm_mday == 14
 
 
 @freeze_time("2012-01-14")
-def test_fake_strftime_function():
+def test_fake_strftime_function() -> None:
     assert fake_strftime_function() == '2012'
 
 
-def test_import_after_start():
+def test_import_after_start() -> None:
     with freeze_time('2012-01-14'):
         assert 'tests.another_module' not in sys.modules.keys()
         from tests import another_module
 
         # Reals
         assert another_module.get_datetime() is datetime.datetime
         assert another_module.get_datetime() is FakeDatetime
@@ -176,11 +176,11 @@
     assert another_module.get_fake_date() is FakeDate
     assert another_module.get_fake_time() is fake_time
     assert another_module.get_fake_localtime() is fake_localtime
     assert another_module.get_fake_gmtime() is fake_gmtime
     assert another_module.get_fake_strftime() is fake_strftime
     del sys.modules['tests.another_module']
 
-def test_none_as_initial():
+def test_none_as_initial() -> None:
     with freeze_time() as ft:
         ft.move_to('2012-01-14')
         assert fake_strftime_function() == '2012'
```

### Comparing `freezegun-1.4.0/tests/test_configure.py` & `freezegun-1.5.0/tests/test_configure.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,101 @@
 from unittest import mock
+import pytest
 import freezegun
 import freezegun.config
 
+from typing import List
 
-def setup_function():
+
+def setup_function() -> None:
     freezegun.config.reset_config()
 
 
-def teardown_function():
+def teardown_function() -> None:
     freezegun.config.reset_config()
 
 
-def test_default_ignore_list_is_overridden():
-    freezegun.configure(default_ignore_list=['threading', 'tensorflow'])
+@pytest.mark.parametrize('ignorelist', (['threading', 'tensorflow'], []))
+def test_default_ignore_list_is_overridden(ignorelist: List[str]) -> None:
+    freezegun.configure(default_ignore_list=list(ignorelist))
+
+    with mock.patch("freezegun.api._freeze_time.__init__", return_value=None) as _freeze_time_init_mock:
+
+        freezegun.freeze_time("2020-10-06")
+
+        _freeze_time_init_mock.assert_called_once_with(
+            time_to_freeze_str="2020-10-06",
+            tz_offset=0,
+            ignore=ignorelist,
+            tick=False,
+            as_arg=False,
+            as_kwarg='',
+            auto_tick_seconds=0,
+            real_asyncio=False,
+        )
+
+
+@pytest.mark.parametrize('ignorelist', (['tensorflow'], []))
+def test_extend_default_ignore_list(ignorelist: List[str]) -> None:
+    freezegun.configure(extend_ignore_list=list(ignorelist))
 
     with mock.patch("freezegun.api._freeze_time.__init__", return_value=None) as _freeze_time_init_mock:
 
         freezegun.freeze_time("2020-10-06")
 
         expected_ignore_list = [
+            'nose.plugins',
+            'six.moves',
+            'django.utils.six.moves',
+            'google.gax',
             'threading',
-            'tensorflow',
-        ]
+            'multiprocessing',
+            'queue',
+            'selenium',
+            '_pytest.terminal.',
+            '_pytest.runner.',
+            'gi',
+            'prompt_toolkit',
+        ] + ignorelist
 
         _freeze_time_init_mock.assert_called_once_with(
             time_to_freeze_str="2020-10-06",
             tz_offset=0,
             ignore=expected_ignore_list,
             tick=False,
             as_arg=False,
             as_kwarg='',
             auto_tick_seconds=0,
             real_asyncio=False,
         )
 
-def test_extend_default_ignore_list():
+def test_extend_default_ignore_list_duplicate_items() -> None:
+    freezegun.configure(extend_ignore_list=['tensorflow', 'pymongo', 'tensorflow','rabbitmq'])
     freezegun.configure(extend_ignore_list=['tensorflow'])
 
     with mock.patch("freezegun.api._freeze_time.__init__", return_value=None) as _freeze_time_init_mock:
 
         freezegun.freeze_time("2020-10-06")
 
         expected_ignore_list = [
             'nose.plugins',
             'six.moves',
             'django.utils.six.moves',
             'google.gax',
             'threading',
             'multiprocessing',
-            'Queue',
+            'queue',
             'selenium',
             '_pytest.terminal.',
             '_pytest.runner.',
             'gi',
             'prompt_toolkit',
             'tensorflow',
+            'pymongo',
+            'rabbitmq',
         ]
 
         _freeze_time_init_mock.assert_called_once_with(
             time_to_freeze_str="2020-10-06",
             tz_offset=0,
             ignore=expected_ignore_list,
             tick=False,
```

### Comparing `freezegun-1.4.0/tests/test_datetimes.py` & `freezegun-1.5.0/tests/test_datetimes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 import time
 import calendar
 import datetime
 import unittest
 import locale
 import sys
+from typing import Any, Callable
 from unittest import SkipTest
 from dateutil.tz import UTC
 
 import pytest
 from tests import utils
 
 from freezegun import freeze_time
 from freezegun.api import FakeDatetime, FakeDate
 
 try:
-    import maya
+    import maya  # type: ignore
 except ImportError:
     maya = None
 
 # time.clock was removed in Python 3.8
 HAS_CLOCK = hasattr(time, 'clock')
 HAS_TIME_NS = hasattr(time, 'time_ns')
 HAS_MONOTONIC_NS = hasattr(time, 'monotonic_ns')
 HAS_PERF_COUNTER_NS = hasattr(time, 'perf_counter_ns')
 
 class temp_locale:
     """Temporarily change the locale."""
 
-    def __init__(self, *targets):
+    def __init__(self, *targets: str):
         self.targets = targets
 
-    def __enter__(self):
+    def __enter__(self) -> None:
         self.old = locale.setlocale(locale.LC_ALL)
         for target in self.targets:
             try:
                 locale.setlocale(locale.LC_ALL, target)
                 return
             except locale.Error:
                 pass
         msg = 'could not set locale to any of: %s' % ', '.join(self.targets)
         raise SkipTest(msg)
 
-    def __exit__(self, *args):
+    def __exit__(self, *args: Any) -> None:
         locale.setlocale(locale.LC_ALL, self.old)
 
 # Small sample of locales where '%x' expands to a dd/mm/yyyy string,
 # which can cause trouble when parsed with dateutil.
 _dd_mm_yyyy_locales = ['da_DK.UTF-8', 'de_DE.UTF-8', 'fr_FR.UTF-8']
 
 
-def test_simple_api():
+def test_simple_api() -> None:
     # time to freeze is always provided in UTC
     freezer = freeze_time("2012-01-14")
     # expected timestamp must be a timestamp, corresponding to 2012-01-14 UTC
     local_time = datetime.datetime(2012, 1, 14)
     utc_time = local_time - datetime.timedelta(seconds=time.timezone)
     expected_timestamp = time.mktime(utc_time.timetuple())
 
@@ -73,15 +74,15 @@
     assert datetime.datetime.utcnow() != datetime.datetime(2012, 1, 14)
     freezer = freeze_time("2012-01-10 13:52:01")
     freezer.start()
     assert datetime.datetime.now() == datetime.datetime(2012, 1, 10, 13, 52, 1)
     freezer.stop()
 
 
-def test_tz_offset():
+def test_tz_offset() -> None:
     freezer = freeze_time("2012-01-14 03:21:34", tz_offset=-4)
     # expected timestamp must be a timestamp,
     # corresponding to 2012-01-14 03:21:34 UTC
     # and it doesn't depend on tz_offset
     local_time = datetime.datetime(2012, 1, 14, 3, 21, 34)
     utc_time = local_time - datetime.timedelta(seconds=time.timezone)
     expected_timestamp = time.mktime(utc_time.timetuple())
@@ -89,104 +90,102 @@
     freezer.start()
     assert datetime.datetime.now() == datetime.datetime(2012, 1, 13, 23, 21, 34)
     assert datetime.datetime.utcnow() == datetime.datetime(2012, 1, 14, 3, 21, 34)
     assert time.time() == expected_timestamp
     freezer.stop()
 
 
-def test_timedelta_tz_offset():
+def test_timestamp_tz_offset() -> None:
+    freezer = freeze_time(datetime.datetime.fromtimestamp(1), tz_offset=-1)
+    freezer.start()
+    t = datetime.datetime.now().timestamp()
+
+    assert datetime.datetime.fromtimestamp(t).timestamp() == t
+    freezer.stop()
+
+
+def test_timedelta_tz_offset() -> None:
     freezer = freeze_time("2012-01-14 03:21:34",
                           tz_offset=-datetime.timedelta(hours=3, minutes=30))
     freezer.start()
     assert datetime.datetime.now() == datetime.datetime(2012, 1, 13, 23, 51, 34)
     assert datetime.datetime.utcnow() == datetime.datetime(2012, 1, 14, 3, 21, 34)
     freezer.stop()
 
 
-def test_tz_offset_with_today():
+def test_tz_offset_with_today() -> None:
     freezer = freeze_time("2012-01-14", tz_offset=-4)
     freezer.start()
     assert datetime.date.today() == datetime.date(2012, 1, 13)
     freezer.stop()
     assert datetime.date.today() != datetime.date(2012, 1, 13)
 
 
-def test_zero_tz_offset_with_time():
+def test_zero_tz_offset_with_time() -> None:
     # we expect the system to behave like a system with UTC timezone
     # at the beginning of the Epoch
     freezer = freeze_time('1970-01-01')
     freezer.start()
     assert datetime.date.today() == datetime.date(1970, 1, 1)
     assert datetime.datetime.now() == datetime.datetime(1970, 1, 1)
     assert datetime.datetime.utcnow() == datetime.datetime(1970, 1, 1)
     assert time.time() == 0.0
     assert time.monotonic() >= 0.0
     assert time.perf_counter() >= 0.0
     freezer.stop()
 
 
-def test_tz_offset_with_time():
+def test_tz_offset_with_time() -> None:
     # we expect the system to behave like a system with UTC-4 timezone
     # at the beginning of the Epoch (wall clock should be 4 hrs late)
     freezer = freeze_time('1970-01-01', tz_offset=-4)
     freezer.start()
     assert datetime.date.today() == datetime.date(1969, 12, 31)
     assert datetime.datetime.now() == datetime.datetime(1969, 12, 31, 20)
     assert datetime.datetime.utcnow() == datetime.datetime(1970, 1, 1)
     assert time.time() == 0.0
     assert time.monotonic() >= 0
     assert time.perf_counter() >= 0
     freezer.stop()
 
 
-def test_time_with_microseconds():
+def test_time_with_microseconds() -> None:
     freezer = freeze_time(datetime.datetime(1970, 1, 1, 0, 0, 1, 123456))
     freezer.start()
     assert time.time() == 1.123456
     freezer.stop()
 
 
-def test_time_with_dst():
+def test_time_with_dst() -> None:
     freezer = freeze_time(datetime.datetime(1970, 6, 1, 0, 0, 1, 123456))
     freezer.start()
     assert time.time() == 13046401.123456
     freezer.stop()
 
 
-def test_manual_increment():
-    initial_datetime = datetime.datetime(year=1, month=7, day=12,
-                                        hour=15, minute=6, second=3)
-    with freeze_time(initial_datetime) as frozen_datetime:
-        assert frozen_datetime() == initial_datetime
-
-        frozen_datetime.tick()
-        initial_datetime += datetime.timedelta(seconds=1)
-        assert frozen_datetime() == initial_datetime
-
-        frozen_datetime.tick(delta=datetime.timedelta(seconds=10))
-        initial_datetime += datetime.timedelta(seconds=10)
-        assert frozen_datetime() == initial_datetime
-
-
-def test_manual_increment_seconds():
+def test_manual_increment() -> None:
     initial_datetime = datetime.datetime(year=1, month=7, day=12,
                                          hour=15, minute=6, second=3)
     with freeze_time(initial_datetime) as frozen_datetime:
         assert frozen_datetime() == initial_datetime
 
-        frozen_datetime.tick()
-        initial_datetime += datetime.timedelta(seconds=1)
-        assert frozen_datetime() == initial_datetime
+        expected = initial_datetime + datetime.timedelta(seconds=1)
+        assert frozen_datetime.tick() == expected
+        assert frozen_datetime() == expected
 
-        frozen_datetime.tick(10)
-        initial_datetime += datetime.timedelta(seconds=10)
-        assert frozen_datetime() == initial_datetime
+        expected = initial_datetime + datetime.timedelta(seconds=11)
+        assert frozen_datetime.tick(10) == expected
+        assert frozen_datetime() == expected
 
+        expected = initial_datetime + datetime.timedelta(seconds=21)
+        assert frozen_datetime.tick(delta=datetime.timedelta(seconds=10)) == expected
+        assert frozen_datetime() == expected
 
-def test_move_to():
+
+def test_move_to() -> None:
     initial_datetime = datetime.datetime(year=1, month=7, day=12,
                                         hour=15, minute=6, second=3)
 
     other_datetime = datetime.datetime(year=2, month=8, day=13,
                                         hour=14, minute=5, second=0)
     with freeze_time(initial_datetime) as frozen_datetime:
         assert frozen_datetime() == initial_datetime
@@ -194,30 +193,30 @@
         frozen_datetime.move_to(other_datetime)
         assert frozen_datetime() == other_datetime
 
         frozen_datetime.move_to(initial_datetime)
         assert frozen_datetime() == initial_datetime
 
 
-def test_bad_time_argument():
+def test_bad_time_argument() -> None:
     try:
         freeze_time("2012-13-14", tz_offset=-4)
     except ValueError:
         pass
     else:
         assert False, "Bad values should raise a ValueError"
 
 
 @pytest.mark.parametrize("func_name, has_func, tick_size", (
     ("monotonic", True, 1.0),
     ("monotonic_ns", HAS_MONOTONIC_NS, int(1e9)),
     ("perf_counter", True, 1.0),
     ("perf_counter_ns", HAS_PERF_COUNTER_NS, int(1e9)),)
 )
-def test_time_monotonic(func_name, has_func, tick_size):
+def test_time_monotonic(func_name: str, has_func: bool, tick_size: int) -> None:
     initial_datetime = datetime.datetime(year=1, month=7, day=12,
                                         hour=15, minute=6, second=3)
     if not has_func:
         pytest.skip("%s does not exist in current version" % func_name)
 
     with freeze_time(initial_datetime) as frozen_datetime:
         func = getattr(time, func_name)
@@ -231,15 +230,15 @@
 
         frozen_datetime.tick(10)
 
         t11 = func()
         assert t11 == t1 + 10 * tick_size
 
 
-def test_time_gmtime():
+def test_time_gmtime() -> None:
     with freeze_time('2012-01-14 03:21:34'):
         time_struct = time.gmtime()
         assert time_struct.tm_year == 2012
         assert time_struct.tm_mon == 1
         assert time_struct.tm_mday == 14
         assert time_struct.tm_hour == 3
         assert time_struct.tm_min == 21
@@ -247,39 +246,39 @@
         assert time_struct.tm_wday == 5
         assert time_struct.tm_yday == 14
         assert time_struct.tm_isdst == -1
 
 
 @pytest.mark.skipif(not HAS_CLOCK,
                     reason="time.clock was removed in Python 3.8")
-def test_time_clock():
+def test_time_clock() -> None:
     with freeze_time('2012-01-14 03:21:34'):
-        assert time.clock() == 0
+        assert time.clock() == 0  # type: ignore[attr-defined]
 
         with freeze_time('2012-01-14 03:21:35'):
-            assert time.clock() == 1
+            assert time.clock() == 1  # type: ignore[attr-defined]
 
         with freeze_time('2012-01-14 03:21:36'):
-            assert time.clock() == 2
+            assert time.clock() == 2  # type: ignore[attr-defined]
 
 
 class modify_timezone:
 
-    def __init__(self, new_timezone):
+    def __init__(self, new_timezone: int):
         self.new_timezone = new_timezone
         self.original_timezone = time.timezone
 
-    def __enter__(self):
+    def __enter__(self) -> None:
         time.timezone = self.new_timezone
 
-    def __exit__(self, *args):
+    def __exit__(self, *args: Any) -> None:
         time.timezone = self.original_timezone
 
 
-def test_time_localtime():
+def test_time_localtime() -> None:
     with modify_timezone(-3600):  # Set this for UTC-1
         with freeze_time('2012-01-14 03:21:34'):
             time_struct = time.localtime()
             assert time_struct.tm_year == 2012
             assert time_struct.tm_mon == 1
             assert time_struct.tm_mday == 14
             assert time_struct.tm_hour == 4  # offset of 1 hour due to time zone
@@ -287,352 +286,352 @@
             assert time_struct.tm_sec == 34
             assert time_struct.tm_wday == 5
             assert time_struct.tm_yday == 14
             assert time_struct.tm_isdst == -1
     assert time.localtime().tm_year != 2012
 
 
-def test_strftime():
+def test_strftime() -> None:
     with modify_timezone(0):
         with freeze_time('1970-01-01'):
             assert time.strftime("%Y") == "1970"
 
 
-def test_real_strftime_fall_through():
+def test_real_strftime_fall_through() -> None:
     this_real_year = datetime.datetime.now().year
     with freeze_time():
         assert time.strftime('%Y') == str(this_real_year)
         assert time.strftime('%Y', (2001, 1, 1, 1, 1, 1, 1, 1, 1)) == '2001'
 
 
-def test_date_object():
+def test_date_object() -> None:
     frozen_date = datetime.date(year=2012, month=11, day=10)
     date_freezer = freeze_time(frozen_date)
     regular_freezer = freeze_time('2012-11-10')
     assert date_freezer.time_to_freeze == regular_freezer.time_to_freeze
 
 
-def test_old_date_object():
+def test_old_date_object() -> None:
     frozen_date = datetime.date(year=1, month=1, day=1)
     with freeze_time(frozen_date):
         assert datetime.date.today() == frozen_date
 
 
-def test_date_with_locale():
+def test_date_with_locale() -> None:
     with temp_locale(*_dd_mm_yyyy_locales):
         frozen_date = datetime.date(year=2012, month=1, day=2)
         date_freezer = freeze_time(frozen_date)
         assert date_freezer.time_to_freeze.date() == frozen_date
 
 
-def test_invalid_type():
+def test_invalid_type() -> None:
     try:
-        freeze_time(int(4))
+        freeze_time(int(4))  # type: ignore
     except TypeError:
         pass
     else:
         assert False, "Bad types should raise a TypeError"
 
 
-def test_datetime_object():
+def test_datetime_object() -> None:
     frozen_datetime = datetime.datetime(year=2012, month=11, day=10,
                                         hour=4, minute=15, second=30)
     datetime_freezer = freeze_time(frozen_datetime)
     regular_freezer = freeze_time('2012-11-10 04:15:30')
     assert datetime_freezer.time_to_freeze == regular_freezer.time_to_freeze
 
 
-def test_function_object():
+def test_function_object() -> None:
     frozen_datetime = datetime.datetime(year=2012, month=11, day=10,
                                         hour=4, minute=15, second=30)
-    def function(): return frozen_datetime
+    def function() -> datetime.datetime: return frozen_datetime
 
     with freeze_time(function):
         assert frozen_datetime == datetime.datetime.now()
 
 
-def test_lambda_object():
+def test_lambda_object() -> None:
     frozen_datetime = datetime.datetime(year=2012, month=11, day=10,
                                         hour=4, minute=15, second=30)
     with freeze_time(lambda: frozen_datetime):
         assert frozen_datetime == datetime.datetime.now()
 
 
-def test_generator_object():
+def test_generator_object() -> None:
     frozen_datetimes = (datetime.datetime(year=y, month=1, day=1)
         for y in range(2010, 2012))
 
     with freeze_time(frozen_datetimes):
         assert datetime.datetime(2010, 1, 1) == datetime.datetime.now()
 
     with freeze_time(frozen_datetimes):
         assert datetime.datetime(2011, 1, 1) == datetime.datetime.now()
 
     with pytest.raises(StopIteration):
         freeze_time(frozen_datetimes)
 
 
-def test_maya_datetimes():
+def test_maya_datetimes() -> None:
     if not maya:
         raise SkipTest("maya is optional since it's not supported for "
                             "enough python versions")
 
     with freeze_time(maya.when("October 2nd, 1997")):
         assert datetime.datetime.now() == datetime.datetime(
             year=1997,
             month=10,
             day=2
         )
 
 
-def test_old_datetime_object():
+def test_old_datetime_object() -> None:
     frozen_datetime = datetime.datetime(year=1, month=7, day=12,
                                         hour=15, minute=6, second=3)
     with freeze_time(frozen_datetime):
         assert datetime.datetime.now() == frozen_datetime
 
 
-def test_datetime_with_locale():
+def test_datetime_with_locale() -> None:
     with temp_locale(*_dd_mm_yyyy_locales):
         frozen_datetime = datetime.datetime(year=2012, month=1, day=2)
         date_freezer = freeze_time(frozen_datetime)
         assert date_freezer.time_to_freeze == frozen_datetime
 
 
 @freeze_time("2012-01-14")
-def test_decorator():
+def test_decorator() -> None:
     assert datetime.datetime.now() == datetime.datetime(2012, 1, 14)
 
 
-def test_decorator_wrapped_attribute():
-    def to_decorate():
+def test_decorator_wrapped_attribute() -> None:
+    def to_decorate() -> None:
         pass
 
     wrapped = freeze_time("2014-01-14")(to_decorate)
 
-    assert wrapped.__wrapped__ is to_decorate
+    assert wrapped.__wrapped__ is to_decorate  # type: ignore
 
 
-class Callable:
+class Callable:  # type: ignore
 
-    def __call__(self, *args, **kws):
+    def __call__(self, *args: Any, **kws: Any) -> Any:
         return (args, kws)
 
 
 @freeze_time("2012-01-14")
 class Tester:
 
-    def test_the_class(self):
+    def test_the_class(self) -> None:
         assert datetime.datetime.now() == datetime.datetime(2012, 1, 14)
 
-    def test_still_the_same(self):
+    def test_still_the_same(self) -> None:
         assert datetime.datetime.now() == datetime.datetime(2012, 1, 14)
 
-    def test_class_name_preserved_by_decorator(self):
+    def test_class_name_preserved_by_decorator(self) -> None:
         assert self.__class__.__name__ == "Tester"
 
     class NotATestClass:
 
-        def perform_operation(self):
+        def perform_operation(self) -> datetime.date:
             return datetime.date.today()
 
     @freeze_time('2001-01-01')
-    def test_class_decorator_ignores_nested_class(self):
+    def test_class_decorator_ignores_nested_class(self) -> None:
         not_a_test = self.NotATestClass()
         assert not_a_test.perform_operation() == datetime.date(2001, 1, 1)
 
-    a_mock = Callable()
+    a_mock = Callable()  # type: ignore
 
-    def test_class_decorator_wraps_callable_object_py3(self):
+    def test_class_decorator_wraps_callable_object_py3(self) -> None:
         assert self.a_mock.__wrapped__.__class__ == Callable
 
     @staticmethod
-    def helper():
+    def helper() -> datetime.date:
         return datetime.date.today()
 
-    def test_class_decorator_respects_staticmethod(self):
+    def test_class_decorator_respects_staticmethod(self) -> None:
         assert self.helper() == datetime.date(2012, 1, 14)
 
 
 @freeze_time("Jan 14th, 2012")
-def test_nice_datetime():
+def test_nice_datetime() -> None:
     assert datetime.datetime.now() == datetime.datetime(2012, 1, 14)
 
 
 @freeze_time("2012-01-14")
-def test_datetime_date_method():
+def test_datetime_date_method() -> None:
     now = datetime.datetime.now()
     assert now.date() == FakeDate(2012, 1, 14)
 
 
-def test_context_manager():
+def test_context_manager() -> None:
     with freeze_time("2012-01-14"):
         assert datetime.datetime.now() == datetime.datetime(2012, 1, 14)
     assert datetime.datetime.now() != datetime.datetime(2012, 1, 14)
 
 
-def test_nested_context_manager():
+def test_nested_context_manager() -> None:
     with freeze_time("2012-01-14"):
         with freeze_time("2012-12-25"):
             _assert_datetime_date_and_time_are_all_equal(datetime.datetime(2012, 12, 25))
         _assert_datetime_date_and_time_are_all_equal(datetime.datetime(2012, 1, 14))
     assert datetime.datetime.now() > datetime.datetime(2013, 1, 1)
 
 
-def _assert_datetime_date_and_time_are_all_equal(expected_datetime):
+def _assert_datetime_date_and_time_are_all_equal(expected_datetime: datetime.datetime) -> None:
     assert datetime.datetime.now() == expected_datetime
     assert datetime.date.today() == expected_datetime.date()
     assert datetime.datetime.fromtimestamp(time.time()) == expected_datetime
 
 
-def test_nested_context_manager_with_tz_offsets():
+def test_nested_context_manager_with_tz_offsets() -> None:
     with freeze_time("2012-01-14 23:00:00", tz_offset=2):
         with freeze_time("2012-12-25 19:00:00", tz_offset=6):
             assert datetime.datetime.now() == datetime.datetime(2012, 12, 26, 1)
             assert datetime.date.today() == datetime.date(2012, 12, 26)
             # no assertion for time.time() since it's not affected by tz_offset
         assert datetime.datetime.now() == datetime.datetime(2012, 1, 15, 1)
         assert datetime.date.today() == datetime.date(2012, 1, 15)
     assert datetime.datetime.now() > datetime.datetime(2013, 1, 1)
 
 
 @freeze_time("Jan 14th, 2012")
-def test_isinstance_with_active():
+def test_isinstance_with_active() -> None:
     now = datetime.datetime.now()
     assert utils.is_fake_datetime(now)
     assert utils.is_fake_date(now.date())
 
     today = datetime.date.today()
     assert utils.is_fake_date(today)
 
 
-def test_isinstance_without_active():
+def test_isinstance_without_active() -> None:
     now = datetime.datetime.now()
     assert isinstance(now, datetime.datetime)
     assert isinstance(now, datetime.date)
     assert isinstance(now.date(), datetime.date)
 
     today = datetime.date.today()
     assert isinstance(today, datetime.date)
 
 
 class TestUnitTestMethodDecorator(unittest.TestCase):
     @freeze_time('2013-04-09')
-    def test_method_decorator_works_on_unittest(self):
+    def test_method_decorator_works_on_unittest(self) -> None:
         self.assertEqual(datetime.date(2013, 4, 9), datetime.date.today())
 
     @freeze_time('2013-04-09', as_kwarg='frozen_time')
-    def test_method_decorator_works_on_unittest_kwarg_frozen_time(self, frozen_time):
+    def test_method_decorator_works_on_unittest_kwarg_frozen_time(self, frozen_time: Any) -> None:
         self.assertEqual(datetime.date(2013, 4, 9), datetime.date.today())
         self.assertEqual(datetime.date(2013, 4, 9), frozen_time.time_to_freeze.today())
 
     @freeze_time('2013-04-09', as_kwarg='hello')
-    def test_method_decorator_works_on_unittest_kwarg_hello(self, **kwargs):
+    def test_method_decorator_works_on_unittest_kwarg_hello(self, **kwargs: Any) -> None:
         self.assertEqual(datetime.date(2013, 4, 9), datetime.date.today())
-        self.assertEqual(datetime.date(2013, 4, 9), kwargs.get('hello').time_to_freeze.today())
+        self.assertEqual(datetime.date(2013, 4, 9), kwargs.get('hello').time_to_freeze.today())  # type: ignore
 
     @freeze_time(lambda: datetime.date(year=2013, month=4, day=9), as_kwarg='frozen_time')
-    def test_method_decorator_works_on_unittest_kwarg_frozen_time_with_func(self, frozen_time):
+    def test_method_decorator_works_on_unittest_kwarg_frozen_time_with_func(self, frozen_time: Any) -> None:
         self.assertEqual(datetime.date(2013, 4, 9), datetime.date.today())
         self.assertEqual(datetime.date(2013, 4, 9), frozen_time.time_to_freeze.today())
 
 
 @freeze_time('2013-04-09')
 class TestUnitTestClassDecorator(unittest.TestCase):
 
     @classmethod
-    def setUpClass(cls):
+    def setUpClass(cls) -> None:
         assert datetime.date(2013, 4, 9) == datetime.date.today()
 
-    def setUp(self):
+    def setUp(self) -> None:
         self.assertEqual(datetime.date(2013, 4, 9), datetime.date.today())
 
-    def tearDown(self):
+    def tearDown(self) -> None:
         self.assertEqual(datetime.date(2013, 4, 9), datetime.date.today())
 
     @classmethod
-    def tearDownClass(cls):
+    def tearDownClass(cls) -> None:
         assert datetime.date(2013, 4, 9) == datetime.date.today()
 
-    def test_class_decorator_works_on_unittest(self):
+    def test_class_decorator_works_on_unittest(self) -> None:
         self.assertEqual(datetime.date(2013, 4, 9), datetime.date.today())
 
-    def test_class_name_preserved_by_decorator(self):
+    def test_class_name_preserved_by_decorator(self) -> None:
         self.assertEqual(self.__class__.__name__, "TestUnitTestClassDecorator")
 
 
 @freeze_time('2013-04-09')
 class TestUnitTestClassDecoratorWithNoSetUpOrTearDown(unittest.TestCase):
-    def test_class_decorator_works_on_unittest(self):
+    def test_class_decorator_works_on_unittest(self) -> None:
         self.assertEqual(datetime.date(2013, 4, 9), datetime.date.today())
 
 
 class TestUnitTestClassDecoratorSubclass(TestUnitTestClassDecorator):
     @classmethod
-    def setUpClass(cls):
+    def setUpClass(cls) -> None:
         # the super() call can fail if the class decoration was done wrong
         super().setUpClass()
 
     @classmethod
-    def tearDownClass(cls):
+    def tearDownClass(cls) -> None:
         # the super() call can fail if the class decoration was done wrong
         super().tearDownClass()
 
-    def test_class_name_preserved_by_decorator(self):
+    def test_class_name_preserved_by_decorator(self) -> None:
         self.assertEqual(self.__class__.__name__,
                          "TestUnitTestClassDecoratorSubclass")
 
 
 class BaseInheritanceFreezableTests(unittest.TestCase):
     @classmethod
-    def setUpClass(cls):
+    def setUpClass(cls) -> None:
         pass
 
     @classmethod
-    def tearDownClass(cls):
+    def tearDownClass(cls) -> None:
         pass
 
 
 class UnfrozenInheritedTests(BaseInheritanceFreezableTests):
-    def test_time_is_not_frozen(self):
+    def test_time_is_not_frozen(self) -> None:
         # In this class, time should not be frozen - and the below decorated
         # class shouldn't affect that
         self.assertNotEqual(datetime.date(2013, 4, 9), datetime.date.today())
 
 
 @freeze_time('2013-04-09')
 class FrozenInheritedTests(BaseInheritanceFreezableTests):
-    def test_time_is_frozen(self):
+    def test_time_is_frozen(self) -> None:
         # In this class, time should be frozen
         self.assertEqual(datetime.date(2013, 4, 9), datetime.date.today())
 
 
 class TestOldStyleClasses:
-    def test_direct_method(self):
+    def test_direct_method(self) -> None:
         # Make sure old style classes (not inheriting from object) is supported
         @freeze_time('2013-04-09')
         class OldStyleClass:
-            def method(self):
+            def method(self) -> datetime.date:
                 return datetime.date.today()
 
         assert OldStyleClass().method() == datetime.date(2013, 4, 9)
 
-    def test_inherited_method(self):
+    def test_inherited_method(self) -> None:
         class OldStyleBaseClass:
-            def inherited_method(self):
+            def inherited_method(self) -> datetime.date:
                 return datetime.date.today()
 
         @freeze_time('2013-04-09')
         class OldStyleClass(OldStyleBaseClass):
             pass
 
         assert OldStyleClass().inherited_method() == datetime.date(2013, 4, 9)
 
 
-def test_min_and_max():
+def test_min_and_max() -> None:
     freezer = freeze_time("2012-01-14")
     real_datetime = datetime.datetime
     real_date = datetime.date
 
     freezer.start()
     assert datetime.datetime.min.__class__ == FakeDatetime
     assert datetime.datetime.max.__class__ == FakeDatetime
@@ -651,63 +650,63 @@
     assert datetime.datetime.min.__class__ != FakeDatetime
     assert datetime.datetime.max.__class__ != FakeDatetime
     assert datetime.date.min.__class__ != FakeDate
     assert datetime.date.max.__class__ != FakeDate
 
 
 @freeze_time("2014-07-30T01:00:00Z")
-def test_freeze_with_timezone_aware_datetime_in_utc():
+def test_freeze_with_timezone_aware_datetime_in_utc() -> None:
     """
     utcnow() should always return a timezone naive datetime
     """
     utc_now = datetime.datetime.utcnow()
     assert utc_now.tzinfo is None
 
 
 @freeze_time("1970-01-01T00:00:00-04:00")
-def test_freeze_with_timezone_aware_datetime_in_non_utc():
+def test_freeze_with_timezone_aware_datetime_in_non_utc() -> None:
     """
     we expect the system to behave like a system with UTC-4 timezone
     at the beginning of the Epoch (wall clock should be 4 hrs late)
     """
     utc_now = datetime.datetime.utcnow()
     assert utc_now.tzinfo is None
     assert utc_now == datetime.datetime(1970, 1, 1, 4)
 
 
 @freeze_time('2015-01-01')
-def test_time_with_nested():
+def test_time_with_nested() -> None:
     from time import time
     first = 1420070400.0
     second = 1420070760.0
 
     assert time() == first
     with freeze_time('2015-01-01T00:06:00'):
         assert time() == second
 
 
 @pytest.mark.parametrize("func_name",
     ("monotonic", "perf_counter")
 )
-def test_monotonic_with_nested(func_name):
+def test_monotonic_with_nested(func_name: str) -> None:
     __import__("time", fromlist=[func_name])
-    invoke_time_func = lambda: getattr(time, func_name)()
+    invoke_time_func: Callable[[], float] = lambda: getattr(time, func_name)()
 
     with freeze_time('2015-01-01') as frozen_datetime_1:
         initial_t1 = invoke_time_func()
         with freeze_time('2015-12-25') as frozen_datetime_2:
             initial_t2 = invoke_time_func()
             frozen_datetime_2.tick()
             assert invoke_time_func() == initial_t2 + 1
         assert invoke_time_func() == initial_t1
         frozen_datetime_1.tick()
         assert invoke_time_func() == initial_t1 + 1
 
 
-def test_should_use_real_time():
+def test_should_use_real_time() -> None:
     frozen = datetime.datetime(2015, 3, 5)
     expected_frozen = 1425513600.0
     # TODO: local time seems to leak the local timezone, so this test fails in CI
     # expected_frozen_local = (2015, 3, 5, 1, 0, 0, 3, 64, -1)
     expected_frozen_gmt = (2015, 3, 5, 0, 0, 0, 3, 64, -1)
     expected_clock = 0
 
@@ -718,51 +717,62 @@
     time_tuple = time.gmtime(timestamp_to_convert)
 
     with freeze_time(frozen):
         assert time.time() == expected_frozen
         # assert time.localtime() == expected_frozen_local
         assert time.gmtime() == expected_frozen_gmt
         if HAS_CLOCK:
-            assert time.clock() == expected_clock
+            assert time.clock() == expected_clock  # type: ignore[attr-defined]
         if HAS_TIME_NS:
             assert time.time_ns() == expected_frozen * 1e9
 
         assert calendar.timegm(time.gmtime()) == expected_frozen
         assert calendar.timegm(time_tuple) == timestamp_to_convert
 
     with freeze_time(frozen, ignore=['_pytest']):
         assert time.time() != expected_frozen
         # assert time.localtime() != expected_frozen_local
         assert time.gmtime() != expected_frozen_gmt
         if HAS_CLOCK:
-            assert time.clock() != expected_clock
+            assert time.clock() != expected_clock  # type: ignore[attr-defined]
         if HAS_TIME_NS:
             assert time.time_ns() != expected_frozen * 1e9
 
         assert calendar.timegm(time.gmtime()) != expected_frozen
         assert calendar.timegm(time_tuple) == timestamp_to_convert
 
 
 @pytest.mark.skipif(not HAS_TIME_NS,
                     reason="time.time_ns is present only on 3.7 and above")
-def test_time_ns():
+def test_time_ns() -> None:
     freezer = freeze_time("2012-01-14")
     local_time = datetime.datetime(2012, 1, 14)
     utc_time = local_time - datetime.timedelta(seconds=time.timezone)
     expected_timestamp = time.mktime(utc_time.timetuple())
 
-    freezer.start()
-    assert time.time() == expected_timestamp
-    assert time.time_ns() == expected_timestamp * 1e9
-    freezer.stop()
+    with freezer:
+        assert time.time() == expected_timestamp
+        assert time.time_ns() == expected_timestamp * 1e9
+
     assert time.time() != expected_timestamp
     assert time.time_ns() != expected_timestamp * 1e9
 
 
-def test_compare_datetime_and_time_with_timezone(monkeypatch):
+@pytest.mark.skipif(not HAS_TIME_NS,
+                    reason="time.time_ns is present only on 3.7 and above")
+def test_time_ns_with_microseconds() -> None:
+    freezer = freeze_time("2024-03-20 18:21:10.12345")
+
+    with freezer:
+        assert time.time_ns() == 1710958870123450112
+
+    assert time.time_ns() != 1710958870123450112
+
+
+def test_compare_datetime_and_time_with_timezone(monkeypatch: pytest.MonkeyPatch) -> None:
     """
     Compare the result of datetime.datetime.now() and time.time() in a non-UTC timezone. These
     should be consistent.
     """
     try:
         with monkeypatch.context() as m, freeze_time("1970-01-01 00:00:00"):
             m.setenv("TZ", "Europe/Berlin")
@@ -773,29 +783,29 @@
             assert now == datetime.datetime.utcfromtimestamp(time.time())
             assert now == datetime.datetime.utcnow()
             assert now.timestamp() == time.time()
     finally:
         time.tzset()  # set the timezone back to what is was before
 
 
-def test_timestamp_with_tzoffset():
+def test_timestamp_with_tzoffset() -> None:
     with freeze_time("2000-01-01", tz_offset=6):
         utcnow = datetime.datetime(2000, 1, 1, 0)
         nowtz = datetime.datetime(2000, 1, 1, 0, tzinfo=UTC)
         now = datetime.datetime(2000, 1, 1, 6)
         assert now == datetime.datetime.now()
         assert now == datetime.datetime.fromtimestamp(time.time())
         assert now.timestamp() == time.time()
         assert nowtz.timestamp() == time.time()
 
         assert utcnow == datetime.datetime.utcfromtimestamp(time.time())
         assert utcnow == datetime.datetime.utcnow()
 
 @pytest.mark.skip("timezone handling is currently incorrect")
-def test_datetime_in_timezone(monkeypatch):
+def test_datetime_in_timezone(monkeypatch: pytest.MonkeyPatch) -> None:
     """
     It is assumed that the argument passed to freeze_time is in UTC, unless explicitly indicated
     otherwise. Therefore datetime.now() should return the frozen time with an offset.
     """
     try:
         with monkeypatch.context() as m, freeze_time("1970-01-01 00:00:00"):
             m.setenv("TZ", "Europe/Berlin")
```

### Comparing `freezegun-1.4.0/tests/test_import_alias.py` & `freezegun-1.5.0/tests/test_import_alias.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from freezegun import freeze_time
 from datetime import datetime as datetime_aliased
 from time import time as time_aliased
 
 
 @freeze_time("1980-01-01")
-def test_datetime_alias():
+def test_datetime_alias() -> None:
     assert datetime_aliased.now() == datetime_aliased(1980, 1, 1)
 
 
 @freeze_time("1970-01-01")
-def test_time_alias():
+def test_time_alias() -> None:
     assert time_aliased() == 0.0
 
 
 @freeze_time('2013-04-09')
 class TestCallOtherFuncInTestClassDecoratorWithAlias:
 
-    def test_calls_other_method(self):
+    def test_calls_other_method(self) -> None:
         assert datetime_aliased(2013, 4, 9) == datetime_aliased.today()
         self.some_other_func()
         assert datetime_aliased(2013, 4, 9) == datetime_aliased.today()
 
-    def some_other_func(self):
+    def some_other_func(self) -> None:
         pass
```

### Comparing `freezegun-1.4.0/tests/test_operations.py` & `freezegun-1.5.0/tests/test_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import datetime
 from freezegun import freeze_time
 from dateutil.relativedelta import relativedelta
 from datetime import timedelta, tzinfo
 from tests import utils
+from typing import Any
 
 
 @freeze_time("2012-01-14")
-def test_addition():
+def test_addition() -> None:
     now = datetime.datetime.now()
     later = now + datetime.timedelta(days=1)
     other_later = now + relativedelta(days=1)
     assert utils.is_fake_datetime(later)
     assert utils.is_fake_datetime(other_later)
 
     today = datetime.date.today()
     tomorrow = today + datetime.timedelta(days=1)
     other_tomorrow = today + relativedelta(days=1)
     assert utils.is_fake_date(tomorrow)
     assert utils.is_fake_date(other_tomorrow)
 
 
 @freeze_time("2012-01-14")
-def test_subtraction():
+def test_subtraction() -> None:
     now = datetime.datetime.now()
     before = now - datetime.timedelta(days=1)
     other_before = now - relativedelta(days=1)
     how_long = now - before
     assert utils.is_fake_datetime(before)
     assert utils.is_fake_datetime(other_before)
     assert isinstance(how_long, datetime.timedelta)
@@ -36,68 +37,68 @@
     how_long = today - yesterday
     assert utils.is_fake_date(yesterday)
     assert utils.is_fake_date(other_yesterday)
     assert isinstance(how_long, datetime.timedelta)
 
 
 @freeze_time("2012-01-14")
-def test_datetime_timezone_none():
+def test_datetime_timezone_none() -> None:
     now = datetime.datetime.now(tz=None)
     assert now == datetime.datetime(2012, 1, 14)
 
 
 class GMT5(tzinfo):
-    def utcoffset(self, dt):
+    def utcoffset(self, dt: Any) -> timedelta:
         return timedelta(hours=5)
 
-    def tzname(self, dt):
+    def tzname(self, dt: Any) -> str:
         return "GMT +5"
 
-    def dst(self, dt):
+    def dst(self, dt: Any) -> timedelta:
         return timedelta(0)
 
 
 @freeze_time("2012-01-14 2:00:00")
-def test_datetime_timezone_real():
+def test_datetime_timezone_real() -> None:
     now = datetime.datetime.now(tz=GMT5())
     assert now == datetime.datetime(2012, 1, 14, 7, tzinfo=GMT5())
     assert now.utcoffset() == timedelta(0, 60 * 60 * 5)
 
 
 @freeze_time("2012-01-14 2:00:00", tz_offset=-4)
-def test_datetime_timezone_real_with_offset():
+def test_datetime_timezone_real_with_offset() -> None:
     now = datetime.datetime.now(tz=GMT5())
     assert now == datetime.datetime(2012, 1, 14, 3, tzinfo=GMT5())
     assert now.utcoffset() == timedelta(0, 60 * 60 * 5)
 
 
 @freeze_time("2012-01-14 00:00:00")
-def test_astimezone():
+def test_astimezone() -> None:
     now = datetime.datetime.now(tz=GMT5())
     converted = now.astimezone(GMT5())
     assert utils.is_fake_datetime(converted)
 
 
 @freeze_time("2012-01-14 00:00:00")
-def test_astimezone_tz_none():
+def test_astimezone_tz_none() -> None:
     now = datetime.datetime.now(tz=GMT5())
     converted = now.astimezone()
     assert utils.is_fake_datetime(converted)
 
 
 @freeze_time("2012-01-14 00:00:00")
-def test_replace():
+def test_replace() -> None:
     now = datetime.datetime.now()
     modified_time = now.replace(year=2013)
     assert utils.is_fake_datetime(modified_time)
 
     today = datetime.date.today()
     modified_date = today.replace(year=2013)
     assert utils.is_fake_date(modified_date)
 
 
 @freeze_time("Jan 14th, 2020", auto_tick_seconds=15)
-def test_auto_tick():
+def test_auto_tick() -> None:
     first_time = datetime.datetime.now()
     auto_incremented_time = datetime.datetime.now()
     assert first_time + datetime.timedelta(seconds=15) == auto_incremented_time
```

### Comparing `freezegun-1.4.0/tests/test_pickle.py` & `freezegun-1.5.0/tests/test_pickle.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import pickle
 from freezegun import freeze_time
 
 
-def assert_pickled_datetimes_equal_original():
+def assert_pickled_datetimes_equal_original() -> None:
     min_datetime = datetime.datetime.min
     max_datetime = datetime.datetime.max
     min_date = datetime.date.min
     max_date = datetime.date.max
     now = datetime.datetime.now()
     today = datetime.date.today()
     utc_now = datetime.datetime.utcnow()
@@ -16,40 +16,40 @@
     assert pickle.loads(pickle.dumps(min_date)) == min_date
     assert pickle.loads(pickle.dumps(max_date)) == max_date
     assert pickle.loads(pickle.dumps(now)) == now
     assert pickle.loads(pickle.dumps(today)) == today
     assert pickle.loads(pickle.dumps(utc_now)) == utc_now
 
 
-def test_pickle():
+def test_pickle() -> None:
     freezer = freeze_time("2012-01-14")
 
     freezer.start()
     assert_pickled_datetimes_equal_original()
 
     freezer.stop()
     assert_pickled_datetimes_equal_original()
 
 
-def test_pickle_real_datetime():
+def test_pickle_real_datetime() -> None:
     real_datetime = datetime.datetime(1970, 2, 1)
     pickle.loads(pickle.dumps(real_datetime)) == real_datetime
 
     freezer = freeze_time("1970-01-01")
     freezer.start()
     fake_datetime = datetime.datetime.now()
     assert pickle.loads(pickle.dumps(fake_datetime)) == fake_datetime
     pickle.loads(pickle.dumps(real_datetime))
     freezer.stop()
 
     assert pickle.loads(pickle.dumps(fake_datetime)) == fake_datetime
     assert pickle.loads(pickle.dumps(real_datetime)) == real_datetime
 
 
-def test_pickle_real_date():
+def test_pickle_real_date() -> None:
     real_date = datetime.date(1970, 2, 1)
     assert pickle.loads(pickle.dumps(real_date)) == real_date
 
     freezer = freeze_time("1970-01-01")
     freezer.start()
     fake_date = datetime.datetime.now()
     assert pickle.loads(pickle.dumps(fake_date)) == fake_date
```

### Comparing `freezegun-1.4.0/tests/test_ticking.py` & `freezegun-1.5.0/tests/test_ticking.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,40 +5,40 @@
 from unittest import mock
 import pytest
 
 from freezegun import freeze_time
 from tests import utils
 
 @utils.cpython_only
-def test_ticking_datetime():
+def test_ticking_datetime() -> None:
     with freeze_time("Jan 14th, 2012", tick=True):
         time.sleep(0.001)  # Deal with potential clock resolution problems
         assert datetime.datetime.now() > datetime.datetime(2012, 1, 14)
 
 
 @pytest.mark.skipif(not hasattr(time, "clock"),
                     reason="time.clock was removed in Python 3.8")
 @utils.cpython_only
-def test_ticking_time_clock():
+def test_ticking_time_clock() -> None:
     with freeze_time('2012-01-14 03:21:34', tick=True):
-        first = time.clock()
+        first = time.clock()  # type: ignore
         time.sleep(0.001)  # Deal with potential clock resolution problems
         with freeze_time('2012-01-14 03:21:35', tick=True):
-            second = time.clock()
+            second = time.clock()  # type: ignore
             time.sleep(0.001)  # Deal with potential clock resolution problems
 
         with freeze_time('2012-01-14 03:21:36', tick=True):
-            third = time.clock()
+            third = time.clock()  # type: ignore
             time.sleep(0.001)
 
         # Rewind time backwards
         with freeze_time('2012-01-14 03:20:00', tick=True):
-            fourth = time.clock()
+            fourth = time.clock()  # type: ignore
             time.sleep(0.001)
-            fifth = time.clock()
+            fifth = time.clock()  # type: ignore
 
         assert first > 0
         assert second > first
         assert second > 1
         assert third > second
         assert third > 2
 
@@ -46,32 +46,56 @@
         assert second > fourth
         assert first > fourth
 
         assert fifth > fourth
 
 
 @utils.cpython_only
-def test_ticking_date():
+def test_ticking_date() -> None:
     with freeze_time("Jan 14th, 2012, 23:59:59.9999999", tick=True):
         time.sleep(0.001)  # Deal with potential clock resolution problems
         assert datetime.date.today() == datetime.date(2012, 1, 15)
 
 
 @utils.cpython_only
-def test_ticking_time():
+def test_ticking_time() -> None:
     with freeze_time("Jan 14th, 2012, 23:59:59", tick=True):
         time.sleep(0.001)  # Deal with potential clock resolution problems
         assert time.time() > 1326585599.0
 
 
+@utils.cpython_only
+def test_ticking_tick() -> None:
+    with freeze_time("Jan 14th, 2012, 23:59:59", tick=True) as ft:
+        ft.tick(61)
+        time.sleep(0.001)  # Deal with potential clock resolution problems
+        assert datetime.datetime.now().replace(
+            second=0, microsecond=0
+        ) == datetime.datetime(2012, 1, 15, 0, 1, 0)
+
+        ft.tick(delta=datetime.timedelta(minutes=2))
+        time.sleep(0.001)  # Deal with potential clock resolution problems
+        assert datetime.datetime.now().replace(
+            second=0, microsecond=0
+        ) == datetime.datetime(2012, 1, 15, 0, 3, 0)
+
+
+@utils.cpython_only
+def test_ticking_move_to() -> None:
+    with freeze_time("Jan 14th, 2012, 23:59:59", tick=True) as ft:
+        ft.move_to("Jan 15th, 2012, 00:59:59.999999")
+        time.sleep(0.001)  # Deal with potential clock resolution problems
+        assert datetime.datetime.now().replace(second=0, microsecond=0) == datetime.datetime(2012, 1, 15, 1, 0, 0)
+
+
 @utils.cpython_only_mark
 @pytest.mark.parametrize("func_name",
     ("monotonic", "monotonic_ns", "perf_counter", "perf_counter_ns"),
 )
-def test_ticking_monotonic(func_name):
+def test_ticking_monotonic(func_name: str) -> None:
     if sys.version_info[0:2] >= (3, 7):
         # All of these functions should exist in Python 3.7+, so this test helps
         # avoid inappropriate skipping when we've accidentally typo-ed the name
         # of one of these functions 😅
         assert hasattr(time, func_name)
     else:
         if not hasattr(time, func_name):
@@ -82,22 +106,22 @@
     with freeze_time("Jan 14th, 2012, 23:59:59", tick=True):
         initial = func()
         time.sleep(0.001)  # Deal with potential clock resolution problems
         assert func() > initial
 
 
 @mock.patch('freezegun.api._is_cpython', False)
-def test_pypy_compat():
+def test_pypy_compat() -> None:
     try:
         freeze_time("Jan 14th, 2012, 23:59:59", tick=True)
     except SystemError:
         pass
     else:
         raise AssertionError("tick=True should error on non-CPython")
 
 
 @mock.patch('freezegun.api._is_cpython', True)
-def test_non_pypy_compat():
+def test_non_pypy_compat() -> None:
     try:
         freeze_time("Jan 14th, 2012, 23:59:59", tick=True)
     except Exception:
         raise AssertionError("tick=True should not error on CPython")
```

### Comparing `freezegun-1.4.0/tests/test_utils.py` & `freezegun-1.5.0/tests/test_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 from unittest import SkipTest, mock
 
 from freezegun import api
 from tests import utils
 
 
 @mock.patch('platform.python_implementation', lambda: 'CPython')
-def test_should_not_skip_cpython():
+def test_should_not_skip_cpython() -> None:
     reload(api)
     reload(utils)
     function_mock = mock.MagicMock(__name__='function')
     try:
         utils.cpython_only(function_mock)()
     except SkipTest:
         raise AssertionError("Test was skipped in CPython")
     assert function_mock.called
 
 
 @mock.patch('platform.python_implementation', lambda: 'not-CPython')
-def test_should_skip_non_cpython():
+def test_should_skip_non_cpython() -> None:
     reload(api)
     reload(utils)
     function_mock = mock.MagicMock(__name__='function', skipped=False)
     try:
         utils.cpython_only(function_mock)()
     except SkipTest:
         function_mock.skipped = True
```

### Comparing `freezegun-1.4.0/tests/test_uuid.py` & `freezegun-1.5.0/tests/test_uuid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import datetime
 import uuid
+from typing import Any
 
 from freezegun import freeze_time
 
 
-def time_from_uuid(value):
+def time_from_uuid(value: Any) -> datetime.datetime:
     """
     Converts an UUID(1) to it's datetime value
     """
     uvalue = value if isinstance(value, uuid.UUID) else uuid.UUID(value)
     assert uvalue.version == 1
     return (datetime.datetime(1582, 10, 15) +
             datetime.timedelta(microseconds=uvalue.time // 10))
 
 
-def test_uuid1_future():
+def test_uuid1_future() -> None:
     """
     Test that we can go back in time after setting a future date.
     Normally UUID1 would disallow this, since it keeps track of
     the _last_timestamp, but we override that now.
     """
     future_target = datetime.datetime(2056, 2, 6, 14, 3, 21)
     with freeze_time(future_target):
         assert time_from_uuid(uuid.uuid1()) == future_target
 
     past_target = datetime.datetime(1978, 7, 6, 23, 6, 31)
     with freeze_time(past_target):
         assert time_from_uuid(uuid.uuid1()) == past_target
 
 
-def test_uuid1_past():
+def test_uuid1_past() -> None:
     """
     Test that we can go forward in time after setting some time in the past.
     This is simply the opposite of test_uuid1_future()
     """
     past_target = datetime.datetime(1978, 7, 6, 23, 6, 31)
     with freeze_time(past_target):
         assert time_from_uuid(uuid.uuid1()) == past_target
```

### Comparing `freezegun-1.4.0/tests/test_warnings.py` & `freezegun-1.5.0/tests/test_warnings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import contextlib
 import datetime
 import sys
 import types
 import warnings
+from typing import Iterator
 
 from freezegun import freeze_time
 
 
 class ModuleWithWarning:
     """
     A module that triggers warnings on attribute access.
@@ -26,58 +27,58 @@
     """
     __name__ = 'module_with_warning'
     __dict__ = {}
     warning_triggered = False
     counter = 0
 
     @property
-    def attribute_that_emits_a_warning(self):
+    def attribute_that_emits_a_warning(self) -> None:
         # Use unique warning messages to avoid messages being only reported once
         self.__class__.counter += 1
         warnings.warn(f'this is test warning #{self.__class__.counter}')
         self.warning_triggered = True
 
 
 @contextlib.contextmanager
-def assert_module_with_emitted_warning():
+def assert_module_with_emitted_warning() -> Iterator[None]:
     """Install a module that triggers warnings into sys.modules and ensure the
     warning was triggered in the with-block.  """
-    module = sys.modules['module_with_warning'] = ModuleWithWarning()
+    module = sys.modules['module_with_warning'] = ModuleWithWarning()  # type: ignore
 
     try:
         yield
     finally:
         del sys.modules['module_with_warning']
 
     assert module.warning_triggered
 
 
 @contextlib.contextmanager
-def assert_no_warnings():
+def assert_no_warnings() -> Iterator[None]:
     """A context manager that makes sure no warnings was emitted."""
     with warnings.catch_warnings(record=True) as caught_warnings:
         warnings.filterwarnings('always')
         yield
         assert not caught_warnings
 
 
-def test_ignore_warnings_in_start():
+def test_ignore_warnings_in_start() -> None:
     """Make sure that modules being introspected in start() does not emit warnings."""
     with assert_module_with_emitted_warning():
         freezer = freeze_time(datetime.datetime(2016, 10, 27, 9, 56))
 
         try:
             with assert_no_warnings():
                 freezer.start()
 
         finally:
             freezer.stop()
 
 
-def test_ignore_warnings_in_stop():
+def test_ignore_warnings_in_stop() -> None:
     """Make sure that modules that was loaded after start() does not trigger
     warnings in stop()"""
     freezer = freeze_time(datetime.datetime(2016, 10, 27, 9, 56))
     freezer.start()
 
     with assert_module_with_emitted_warning():
         with assert_no_warnings():
```

