# Comparing `tmp/interprocesspyobjects-1.0.2.tar.gz` & `tmp/interprocesspyobjects-1.0.3.tar.gz`

## Comparing `interprocesspyobjects-1.0.2.tar` & `interprocesspyobjects-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/ipc_py_objects/__init__.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/ipc_py_objects/versions/__init__.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/ipc_py_objects/versions/v_0/__init__.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/ipc_py_objects/versions/v_1/__init__.py
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/LICENSE.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/NOTICE
--rw-r--r--   0        0        0    37439 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/README.md
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    42055 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/ipc_py_objects/__init__.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/ipc_py_objects/versions/__init__.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/ipc_py_objects/versions/v_0/__init__.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/ipc_py_objects/versions/v_1/__init__.py
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/NOTICE
+-rw-r--r--   0        0        0    39612 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/README.md
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    44228 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/PKG-INFO
```

### Comparing `interprocesspyobjects-1.0.2/ipc_py_objects/__init__.py` & `interprocesspyobjects-1.0.3/ipc_py_objects/versions/v_0/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 """
 
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
 __copyright__ = "Copyright © 2012-2024 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
 __credits__ = ["ButenkoMS <gtalk@butenkoms.space>", ]
 __license__ = "Apache License, Version 2.0"
-__version__ = "1.0.2"
+__version__ = "1.0.0"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 __status__ = "Production"
 
 
-from .versions import *
+from cengal.hardware.memory.shared_memory.versions.v_0 import *
```

### Comparing `interprocesspyobjects-1.0.2/ipc_py_objects/versions/__init__.py` & `interprocesspyobjects-1.0.3/ipc_py_objects/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.2/ipc_py_objects/versions/v_0/__init__.py` & `interprocesspyobjects-1.0.3/ipc_py_objects/versions/v_1/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 __license__ = "Apache License, Version 2.0"
 __version__ = "1.0.0"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 __status__ = "Production"
 
 
-from cengal.hardware.memory.shared_memory.versions.v_0 import *
+from cengal.hardware.memory.shared_memory.versions.v_1 import *
+from cengal.parallel_execution.asyncio.ashared_memory_manager.versions.v_0 import *
```

### Comparing `interprocesspyobjects-1.0.2/ipc_py_objects/versions/v_1/__init__.py` & `interprocesspyobjects-1.0.3/ipc_py_objects/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 """
 
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
 __copyright__ = "Copyright © 2012-2024 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
 __credits__ = ["ButenkoMS <gtalk@butenkoms.space>", ]
 __license__ = "Apache License, Version 2.0"
-__version__ = "1.0.0"
+__version__ = "1.0.3"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 __status__ = "Production"
 
 
-from cengal.hardware.memory.shared_memory.versions.v_1 import *
-from cengal.parallel_execution.asyncio.ashared_memory_manager.versions.v_0 import *
+from .versions import *
```

### Comparing `interprocesspyobjects-1.0.2/.gitignore` & `interprocesspyobjects-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.2/LICENSE.md` & `interprocesspyobjects-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.2/NOTICE` & `interprocesspyobjects-1.0.3/NOTICE`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.2/README.md` & `interprocesspyobjects-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 ![PyPI - Version](https://img.shields.io/pypi/v/InterProcessPyObjects) ![PyPI - Format](https://img.shields.io/pypi/format/cengal-light?color=darkgreen) ![Static Badge](https://img.shields.io/badge/wheels-Linux_%7C_Windows_%7C_macOS-blue) ![Static Badge](https://img.shields.io/badge/Architecture-x86__64_%7C_ARM__64-blue) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cengal-light) ![Static Badge](https://img.shields.io/badge/PyPy-3.8_%7C_3.9_%7C_3.10-blue) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/cengal-light) 
 
 ![GitHub License](https://img.shields.io/github/license/FI-Mihej/InterProcessPyObjects?color=darkgreen) ![Static Badge](https://img.shields.io/badge/API_status-Stable-darkgreen)
 
 # InterProcessPyObjects package
 
+> InterProcessPyObjects is a part of the [Cengal](https://github.com/FI-Mihej/Cengal) library. If you have any questions or would like to participate in discussions, feel free to join the [Cengal Discord](https://discord.gg/TAy7xNgR). Your support and involvement are greatly appreciated as Cengal evolves.
+
 This high-performance package delivers blazing-fast inter-process communication through shared memory, enabling Python objects to be shared across processes with exceptional efficiency. By minimizing the need for frequent serialization-deserialization, it enhances overall speed and responsiveness. The package offers a comprehensive suite of functionalities designed to support a diverse array of Python types and facilitate asynchronous IPC, optimizing performance for demanding applications.
 
 ![title](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartThroughputGiBs.png)
 
 ## API State
 
 Stable. Guaranteed to not have braking changes in the future (see bellow for details).
@@ -68,23 +70,23 @@
     * Ensures each process can access and modify shared memory without contention.
 
 * Supported Python Types:
     * Handles various Python data structures including:
         * Basic types: `None`, `bool`, 64-bit `int`, large `int` (arbitrary precision integers), `float`, `complex`, `bytes`, `bytearray`, `str`.
         * Standard types: `Decimal`, `slice`, `datetime`, `timedelta`, `timezone`, `date`, `time`
         * Containers: `tuple`, `list`, classes inherited from: `AbstractSet` (`frozenset`), `MutableSet` (`set`), `Mapping` and `MutableMapping` (`dict`).
-        * Pickable classes instancess: custom classes including `dataclass`
+        * Pickable classes instances: custom classes including `dataclass`
     * Allows mutable containers (lists, sets, mappings) to save basic types (`None`, `bool`, 64 bit `int`, `float`) internally, optimizing memory use and speed.
 
 * NumPy and Torch Support:
     * Supports numpy arrays by creating shared bytes objects coupled with independent arrays.
     * Supports torch tensors by coupling them with shared numpy arrays.
 
 * Custom Class Support:
-    * Projects pickable custom classes instancess (including `dataclasses`) onto shared dictionaries in shared memory.
+    * Projects pickable custom classes instances (including `dataclasses`) onto shared dictionaries in shared memory.
     * Modifies the class instance to override attribute access methods, managing data fields within the shared dictionary.
     * supports classes with or without `__dict__` attr
     * supports classes with or without `__slots__` attr
 
 * Asyncio Compatibility:
     * Provides a wrapper module for async-await functionality, integrating seamlessly with asyncio.
     * Ensures asynchronous operations work smoothly with the package's lock-free approach.
@@ -104,27 +106,27 @@
 ```
 
 ## Main principles
 
 * only one process has access to the shared memory at the same time
 * working cycle:
     1. work on your tasks
-    2. acacquire access to shared memory
+    2. acquire access to shared memory
     3. work with shared memory as fast as possible (read and/or update data structures in shared memory)
     4. release access to shared memory
     5. continue your work on other tasks
 * do not forget to manually destroy your shared objects when they are not needed already
 * feel free to not destroy your shared object if you need it for a whole run and/or do not care about the shared memory waste
 * data will not be preserved between Creator's sessions. Shared memory will be wiped just before Creator finished its work with a shared memory instance (Consumer's session will be finished already at this point)
 
 ### ! Important about hashmaps
 
 Package, currently, uses Python `hash()` call which is reliable across interpreter session but unreliable across different interpreter sessions because of random seeding.
 
-In order to use same seeding across different interpeter instancess (and as result, be able to use hashmaps) you can set 'PYTHONHASHSEED` env var to some fixed integer value
+In order to use same seeding across different interpreter instances (and as result, be able to use hashmaps) you can set 'PYTHONHASHSEED` env var to some fixed integer value
 
 <details>
 <summary title=".bashrc"><kbd> .bashrc </kbd></summary>
 
 ```bash
 export PYTHONHASHSEED=0
 ```
@@ -152,78 +154,106 @@
 
 An issue with the behavior of an integrated `hash()` call **does Not** affect the following data types:
 * `None`, `bool`, `int`, `float`, `complex`, `str`, `bytes`, `bytearray`
 * `Decimal`, `slice`, `datetime`, `timedelta`, `timezone`, `date`, `time`
 * `tuple`, `list`
 * `set` wrapped by `FastLimitedSet` class instance: for example by using `.put_message(FastLimitedSet(my_set_obj))` call
 * `dict` wrapped by `FastLimitedDict` class instance: for example by using `.put_message(FastLimitedDict(my_dict_obj))` call
-* an instancess of custom classes including `dataclass` by default: for example by using `.put_message(my_obj)` call
-* an instancess of custom classes including `dataclass` wrapped by `ForceStaticObjectCopy` or `ForceStaticObjectInplace` class instancess. For example by using `.put_message(ForceStaticObjectInplace(my_obj))` call
+* an instances of custom classes including `dataclass` by default: for example by using `.put_message(my_obj)` call
+* an instances of custom classes including `dataclass` wrapped by `ForceStaticObjectCopy` or `ForceStaticObjectInplace` class instances. For example by using `.put_message(ForceStaticObjectInplace(my_obj))` call
 
 It affects only the following data types: 
 * `AbstractSet` (`frozenset`)
 * `MutableSet` (`set`)
 * `Mapping`
 * `MutableMapping` (`dict`)
-* an instancess of custom classes including `dataclass` wrapped by `ForceGeneralObjectCopy` or `ForceGeneralObjectInplace` class instancess. For example by using `.put_message(ForceGeneralObjectInplace(my_obj))` call
+* an instances of custom classes including `dataclass` wrapped by `ForceGeneralObjectCopy` or `ForceGeneralObjectInplace` class instances. For example by using `.put_message(ForceGeneralObjectInplace(my_obj))` call
 
 ## Examples
 
 * An async examples (with asyncio):
     * [sender.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/sender.py)
     * [receiver.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/receiver.py)
     * [shared_objects__types.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/shared_objects__types.py)
 
 ### Receiver.py performance measurements
 
 ```python
-sso: SomeSharedObject = None  # variable for our shared object
-
 async with ashared_memory_context_manager.if_has_messages() as shared_memory:
-    sso = shared_memory.value.take_message()  # 5_833 iterations/seconds
-    company_metrics = sso.company_info.company_metrics  # 12_479 iterations/seconds
-    k = company_metrics[CompanyMetrics.in_a_good_state]  # 1_154_454 iterations/seconds
-    company_metrics[CompanyMetrics.in_a_good_state] = False  # 1_213_175 iterations/seconds
-    company_metrics[CompanyMetrics.in_a_good_state] = None  # 1_188_630 iterations/seconds
+    # Taking a message with an object from the queue.
+    sso: SomeSharedObject = shared_memory.value.take_message()  # 5_833 iterations/seconds
+
+    # We create local variables once in order to access them many times in the future, ensuring high performance.
+    # Applying a principle that is widely recommended for improving Python code.
+    company_metrics: List = sso.company_info.company_metrics  # 12_479 iterations/seconds
+    some_employee: Employee = sso.company_info.some_employee  # 10_568 iterations/seconds
+    data_dict: Dict = sso.data_dict  # 16_362 iterations/seconds
+    numpy_ndarray: np.ndarray = data_dict['key3']  # 26_223 iterations/seconds
+
+# Optimal work with shared data (through local variables):
+async with ashared_memory_context_manager as shared_memory:
+    # List
+    k = company_metrics[CompanyMetrics.avg_salary]  # 1_535_267 iterations/seconds
     k = company_metrics[CompanyMetrics.employees]  # 1_498_278 iterations/seconds
+    k = company_metrics[CompanyMetrics.in_a_good_state]  # 1_154_454 iterations/seconds
+    k = company_metrics[CompanyMetrics.websites]  # 380_258 iterations/seconds
+    company_metrics[CompanyMetrics.annual_income] = 2_000_000.0  # 1_380_983 iterations/seconds
     company_metrics[CompanyMetrics.employees] = 20  # 1_352_799 iterations/seconds
-    company_metrics[CompanyMetrics.employees] += 1  # 247_476 iterations/seconds
-    k = company_metrics[CompanyMetrics.avg_salary]  # 1_535_267 iterations/seconds
     company_metrics[CompanyMetrics.avg_salary] = 5_000.0  # 1_300_966 iterations/seconds
+    company_metrics[CompanyMetrics.in_a_good_state] = None  # 1_224_573 iterations/seconds
+    company_metrics[CompanyMetrics.in_a_good_state] = False  # 1_213_175 iterations/seconds
     company_metrics[CompanyMetrics.avg_salary] += 1.1  # 299_415 iterations/seconds
+    company_metrics[CompanyMetrics.employees] += 1  # 247_476 iterations/seconds
+    company_metrics[CompanyMetrics.emails] = tuple()  # 55_335 iterations/seconds (memory allocation performance is planned to be improved)
+    company_metrics[CompanyMetrics.emails] = ('sails@company.com',)  # 30_314 iterations/seconds (memory allocation performance is planned to be improved)
+    company_metrics[CompanyMetrics.emails] = ('sails@company.com', 'support@company.com')  # 20_860 iterations/seconds (memory allocation performance is planned to be improved)
+    company_metrics[CompanyMetrics.websites] = ['http://company.com', 'http://company.org']  # 10_465 iterations/seconds (memory allocation performance is planned to be improved)
+    
+    # Method call on a shared object that changes a property through the method
+    some_employee.increase_years_of_employment()  # 80548 iterations/seconds
+
+    # Object properties
     k = sso.int_value  # 850_098 iterations/seconds
+    k = sso.str_value  # 228_966 iterations/seconds
     sso.int_value = 200  # 207_480 iterations/seconds
     sso.int_value += 1  # 152_263 iterations/seconds
-    company_metrics[CompanyMetrics.annual_income] = 2_000_000.0  # 1_380_983 iterations/seconds
-    company_metrics[CompanyMetrics.emails] = tuple()  # 55_335 iterations/seconds
-    company_metrics[CompanyMetrics.emails] = ('sails@company.com',)  # 30_314 iterations/seconds
-    company_metrics[CompanyMetrics.emails] = ('sails@company.com', 'support@company.com')  # 20_860 iterations/seconds
-    k = company_metrics[CompanyMetrics.websites]  # 380_258 iterations/seconds
-    company_metrics[CompanyMetrics.websites] = ['http://company.com', 'http://company.org']  # 10_465 iterations/seconds
-    k = sso.str_value  # 228_966 iterations/seconds
-    sso.str_value = 'Hello. '  # 52_390 iterations/seconds
-    sso.str_value += '!'  # 35_823 iterations/seconds
-    data_dict = sso.data_dict  # 16_362 iterations/seconds
+    sso.str_value = 'Hello. '  # 52_390 iterations/seconds (memory allocation performance is planned to be improved)
+    sso.str_value += '!'  # 35_823 iterations/seconds (memory allocation performance is planned to be improved)
+
+    # Numpy.ndarray
+    numpy_ndarray += 10  # 403_646 iterations/seconds
+    numpy_ndarray -= 15  # 402_107 iterations/seconds
+
+    # Dict
     k = data_dict['key1']  # 87_558 iterations/seconds
+    k = data_dict[('key', 2)]  # 49_338 iterations/seconds
     data_dict['key1'] = 200  # 86_744 iterations/seconds
-    data_dict['key1'] *= 1  # 40_927 iterations/seconds
     data_dict['key1'] += 3  # 41_409 iterations/seconds
-    k = data_dict[('key', 2)]  # 49_338 iterations/seconds
-    data_dict[('key', 2)] = 'value2'  # 31_460 iterations/seconds
-    data_dict[('key', 2)] = data_dict[('key', 2)] + 'd'  # 18_972 iterations/seconds
-    data_dict[('key', 2)] = 'value2'  # 10_941 iterations/seconds
-    data_dict[('key', 2)] += 'd'  # 16_568 iterations/seconds
-    ndarray: np.ndarray = data_dict['key3']  # 26_223 iterations/seconds
-    ndarray += 10  # 403_246 iterations/seconds
-    data_dict['key3'] += 10  # 6_319 iterations/seconds
+    data_dict['key1'] *= 1  # 40_927 iterations/seconds
+    data_dict[('key', 2)] = 'value2'  # 31_460 iterations/seconds (memory allocation performance is planned to be improved)
+    data_dict[('key', 2)] = data_dict[('key', 2)] + 'd'  # 18_972 iterations/seconds (memory allocation performance is planned to be improved)
+    data_dict[('key', 2)] = 'value2'  # 10_941 iterations/seconds (memory allocation performance is planned to be improved)
+    data_dict[('key', 2)] += 'd'  # 16_568 iterations/seconds (memory allocation performance is planned to be improved)
+
+# An example of non-optimal work with shared data (without using a local variables):
+async with ashared_memory_context_manager as shared_memory:
+    # An example of a non-optimal method call (without using a local variable) that changes a property through the method
+    sso.company_info.some_employee.increase_years_of_employment()  # 9_418 iterations/seconds
+
+    # An example of non-optimal work with object properties (without using local variables)
     k = sso.company_info.income  # 20_445 iterations/seconds
     sso.company_info.income = 3_000_000.0  # 13_899 iterations/seconds
     sso.company_info.income *= 1.1  # 17_272 iterations/seconds 
     sso.company_info.income += 500_000.0  # 18_376 iterations/seconds
-    sso.company_info.some_employee.increase_years_of_employment()  # 9_429 iterations/seconds
+    
+    # Example of non-optimal usage of numpy.ndarray without a proper local variable
+    data_dict['key3'] += 10  # 6_319 iterations/seconds
+
+# Notify the sender about the completion of work on the shared object
+async with ashared_memory_context_manager as shared_memory:
     sso.some_processing_stage_control = True  # 298_968 iterations/seconds
 ```
 
 ## Reference (and explaining examples line by line)
 
 Code for shared memory Creator side:
 ```python
@@ -254,28 +284,28 @@
 ```python
 ashared_memory_context_manager: ASharedMemoryContextManager = asmm()
 # creates shared memory access context manager. Create it once per coroutine. Use in the same coroutine as much as you need it.
 ```
 
 ```python
 async with ashared_memory_context_manager as shared_memory:
-# acacquire access to shared memory as soon as possible
+# acquire access to shared memory as soon as possible
 ```
 
 ```python
 async with ashared_memory_context_manager.if_has_messages() as shared_memory:
-# acacquire access to shared memory if message queue is not empty
+# acquire access to shared memory if message queue is not empty
 ```
 
 ```python
 shared_memory # is an instance of ValueHolder class from the Cengal library
 shared_memory.value  # is an instance of `SharedMemory` instance
-shared_memory.existence  # bool. Will be set to True at the beginning of an eash context (`with`) block. Set it to `False`
-    # if you want to release CPU for a small time portion before shared memory will be acacquired next time.
-    # if at least one coroutine will not set it to `False` - next acacquire attempt will be made immidiately which will
+shared_memory.existence  # bool. Will be set to True at the beginning of an each context (`with`) block. Set it to `False`
+    # if you want to release CPU for a small time portion before shared memory will be acquired next time.
+    # if at least one coroutine will not set it to `False` - next acquire attempt will be made immediately which will
     # lower latency and increase performance but at the same time will consume more CPU time.
     # Default behavior (`True`) is better for CPU intensive algorithms, 
     # while `False` on all process coroutines (which have their own memory access context managers) will be better
     # for example for desktop or mobile applications
 ```
 
 ### `SharedMemory` fields and methods you might frequently use in an async approach (in coroutines)
@@ -412,15 +442,15 @@
 company_metrics['employees'] = 200  # 86_744 iterations/seconds
 company_metrics['employees'] += 3  # 41_409 iterations/seconds
 ```
 
 </details>
 <br>
 
-or even instead operating with dataclass (classess by default operate faster then dict):
+or even instead operating with dataclass (classes by default operate faster then dict):
 
 <details>
 <summary title="Example"><kbd> Example </kbd></summary>
 
 Message sender
 
 ```python
@@ -551,15 +581,15 @@
 </details>
 
 <details>
 <summary title="Custom classes (including `dataclass`)"><kbd> Custom classes (including `dataclass`) </kbd></summary>
 
 ### Custom classes (including `dataclass`)
 
-By default, shared custom class instancess (including `dataclass` instancess) have static set of attributes (similar to instancess of classes with `__slots__`). That means that all new (dynamically added to the mapped object, attributes will not became shared). This behavior increases performance.
+By default, shared custom class instances (including `dataclass` instances) have static set of attributes (similar to instances of classes with `__slots__`). That means that all new (dynamically added to the mapped object, attributes will not became shared). This behavior increases performance.
 
 <details>
 <summary title="For example"><kbd> For example </kbd></summary>
 
 #### For example
 
 ```python
@@ -728,15 +758,15 @@
 
 - [ ] Connect more than two processes
 - [ ] Use third-party fast hashing implementations instead of or in addition to built in `hash()` call
 - [ ] Continuous performance improvements
 
 ## Conclusion
 
-This Python package provides a robust solution for interprocess communication, supporting a variety of Python data structures, types, and third-party libraries. Its lock-free synchronization and asyncio compatibility make it an ideal choice for high-performance, concurrent execution.
+This Python package provides a robust solution for inter-process communication, supporting a variety of Python data structures, types, and third-party libraries. Its lock-free synchronization and asyncio compatibility make it an ideal choice for high-performance, concurrent execution.
 
 # Based on [Cengal](https://github.com/FI-Mihej/Cengal)
 
 This is a stand-alone package for a specific Cengal module. Package is designed to offer users the ability to install specific Cengal functionality without the burden of the library's full set of dependencies.
 
 The core of this approach lies in our 'cengal-light' package, which houses both Python and compiled Cengal modules. The 'cengal' package itself serves as a lightweight shell, devoid of its own modules, but dependent on 'cengal-light[full]' for a complete Cengal library installation with all required dependencies.
 
@@ -758,15 +788,15 @@
 
 
 # Projects using Cengal
 
 * [CengalPolyBuild](https://github.com/FI-Mihej/CengalPolyBuild) - A Comprehensive and Hackable Build System for Multilingual Python Packages: Cython (including automatic conversion from Python to Cython), C/C++, Objective-C, Go, and Nim, with ongoing expansions to include additional languages. (Planned to be released soon) 
 * [cengal_app_dir_path_finder](https://github.com/FI-Mihej/cengal_app_dir_path_finder) - A Python module offering a unified API for easy retrieval of OS-specific application directories, enhancing data management across Windows, Linux, and macOS 
 * [cengal_cpu_info](https://github.com/FI-Mihej/cengal_cpu_info) - Extended, cached CPU info with consistent output format.
-* [cengal_memory_barriers](https://github.com/FI-Mihej/cengal_memory_barriers) - Fast crossplatform memory barriers for Python.
+* [cengal_memory_barriers](https://github.com/FI-Mihej/cengal_memory_barriers) - Fast cross-platform memory barriers for Python.
 * [flet_async](https://github.com/FI-Mihej/flet_async) - wrapper which makes [Flet](https://github.com/flet-dev/flet) async and brings booth Cengal.coroutines and asyncio to Flet (Flutter based UI)
 * [justpy_containers](https://github.com/FI-Mihej/justpy_containers) - wrapper around [JustPy](https://github.com/justpy-org/justpy) in order to bring more security and more production-needed features to JustPy (VueJS based UI)
 * [Bensbach](https://github.com/FI-Mihej/Bensbach) - decompiler from Unreal Engine 3 bytecode to a Lisp-like script and compiler back to Unreal Engine 3 bytecode. Made for a game modding purposes
 * [Realistic-Damage-Model-mod-for-Long-War](https://github.com/FI-Mihej/Realistic-Damage-Model-mod-for-Long-War) - Mod for both the original XCOM:EW and the mod Long War. Was made with a Bensbach, which was made with Cengal
 * [SmartCATaloguer.com](http://www.smartcataloguer.com/index.html) - TagDB based catalog of images (tags), music albums (genre tags) and apps (categories)
 
 # License
```

### Comparing `interprocesspyobjects-1.0.2/pyproject.toml` & `interprocesspyobjects-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.2/PKG-INFO` & `interprocesspyobjects-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: InterProcessPyObjects
-Version: 1.0.2
+Version: 1.0.3
 Summary: This high-performance package delivers blazing-fast inter-process communication through shared memory, enabling Python objects to be shared across processes with exceptional efficiency
 Project-URL: Homepage, https://github.com/FI-Mihej/InterProcessPyObjects
 Author-email: ButenkoMS <gtalk@butenkoms.space>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
 License-File: NOTICE
 Keywords: Android,IPC,Linux,Windows,cengal,crossplatform,iOS,inter-process communication,macOS,multiprocessing,shared dict,shared memory,shared numpy ndarray,shared object,shared objects,shared set,shared torch Tensor
@@ -94,14 +94,16 @@
 
 ![PyPI - Version](https://img.shields.io/pypi/v/InterProcessPyObjects) ![PyPI - Format](https://img.shields.io/pypi/format/cengal-light?color=darkgreen) ![Static Badge](https://img.shields.io/badge/wheels-Linux_%7C_Windows_%7C_macOS-blue) ![Static Badge](https://img.shields.io/badge/Architecture-x86__64_%7C_ARM__64-blue) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cengal-light) ![Static Badge](https://img.shields.io/badge/PyPy-3.8_%7C_3.9_%7C_3.10-blue) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/cengal-light) 
 
 ![GitHub License](https://img.shields.io/github/license/FI-Mihej/InterProcessPyObjects?color=darkgreen) ![Static Badge](https://img.shields.io/badge/API_status-Stable-darkgreen)
 
 # InterProcessPyObjects package
 
+> InterProcessPyObjects is a part of the [Cengal](https://github.com/FI-Mihej/Cengal) library. If you have any questions or would like to participate in discussions, feel free to join the [Cengal Discord](https://discord.gg/TAy7xNgR). Your support and involvement are greatly appreciated as Cengal evolves.
+
 This high-performance package delivers blazing-fast inter-process communication through shared memory, enabling Python objects to be shared across processes with exceptional efficiency. By minimizing the need for frequent serialization-deserialization, it enhances overall speed and responsiveness. The package offers a comprehensive suite of functionalities designed to support a diverse array of Python types and facilitate asynchronous IPC, optimizing performance for demanding applications.
 
 ![title](https://github.com/FI-Mihej/Cengal/raw/master/docs/assets/InterProcessPyObjects/ChartThroughputGiBs.png)
 
 ## API State
 
 Stable. Guaranteed to not have braking changes in the future (see bellow for details).
@@ -160,23 +162,23 @@
     * Ensures each process can access and modify shared memory without contention.
 
 * Supported Python Types:
     * Handles various Python data structures including:
         * Basic types: `None`, `bool`, 64-bit `int`, large `int` (arbitrary precision integers), `float`, `complex`, `bytes`, `bytearray`, `str`.
         * Standard types: `Decimal`, `slice`, `datetime`, `timedelta`, `timezone`, `date`, `time`
         * Containers: `tuple`, `list`, classes inherited from: `AbstractSet` (`frozenset`), `MutableSet` (`set`), `Mapping` and `MutableMapping` (`dict`).
-        * Pickable classes instancess: custom classes including `dataclass`
+        * Pickable classes instances: custom classes including `dataclass`
     * Allows mutable containers (lists, sets, mappings) to save basic types (`None`, `bool`, 64 bit `int`, `float`) internally, optimizing memory use and speed.
 
 * NumPy and Torch Support:
     * Supports numpy arrays by creating shared bytes objects coupled with independent arrays.
     * Supports torch tensors by coupling them with shared numpy arrays.
 
 * Custom Class Support:
-    * Projects pickable custom classes instancess (including `dataclasses`) onto shared dictionaries in shared memory.
+    * Projects pickable custom classes instances (including `dataclasses`) onto shared dictionaries in shared memory.
     * Modifies the class instance to override attribute access methods, managing data fields within the shared dictionary.
     * supports classes with or without `__dict__` attr
     * supports classes with or without `__slots__` attr
 
 * Asyncio Compatibility:
     * Provides a wrapper module for async-await functionality, integrating seamlessly with asyncio.
     * Ensures asynchronous operations work smoothly with the package's lock-free approach.
@@ -196,27 +198,27 @@
 ```
 
 ## Main principles
 
 * only one process has access to the shared memory at the same time
 * working cycle:
     1. work on your tasks
-    2. acacquire access to shared memory
+    2. acquire access to shared memory
     3. work with shared memory as fast as possible (read and/or update data structures in shared memory)
     4. release access to shared memory
     5. continue your work on other tasks
 * do not forget to manually destroy your shared objects when they are not needed already
 * feel free to not destroy your shared object if you need it for a whole run and/or do not care about the shared memory waste
 * data will not be preserved between Creator's sessions. Shared memory will be wiped just before Creator finished its work with a shared memory instance (Consumer's session will be finished already at this point)
 
 ### ! Important about hashmaps
 
 Package, currently, uses Python `hash()` call which is reliable across interpreter session but unreliable across different interpreter sessions because of random seeding.
 
-In order to use same seeding across different interpeter instancess (and as result, be able to use hashmaps) you can set 'PYTHONHASHSEED` env var to some fixed integer value
+In order to use same seeding across different interpreter instances (and as result, be able to use hashmaps) you can set 'PYTHONHASHSEED` env var to some fixed integer value
 
 <details>
 <summary title=".bashrc"><kbd> .bashrc </kbd></summary>
 
 ```bash
 export PYTHONHASHSEED=0
 ```
@@ -244,78 +246,106 @@
 
 An issue with the behavior of an integrated `hash()` call **does Not** affect the following data types:
 * `None`, `bool`, `int`, `float`, `complex`, `str`, `bytes`, `bytearray`
 * `Decimal`, `slice`, `datetime`, `timedelta`, `timezone`, `date`, `time`
 * `tuple`, `list`
 * `set` wrapped by `FastLimitedSet` class instance: for example by using `.put_message(FastLimitedSet(my_set_obj))` call
 * `dict` wrapped by `FastLimitedDict` class instance: for example by using `.put_message(FastLimitedDict(my_dict_obj))` call
-* an instancess of custom classes including `dataclass` by default: for example by using `.put_message(my_obj)` call
-* an instancess of custom classes including `dataclass` wrapped by `ForceStaticObjectCopy` or `ForceStaticObjectInplace` class instancess. For example by using `.put_message(ForceStaticObjectInplace(my_obj))` call
+* an instances of custom classes including `dataclass` by default: for example by using `.put_message(my_obj)` call
+* an instances of custom classes including `dataclass` wrapped by `ForceStaticObjectCopy` or `ForceStaticObjectInplace` class instances. For example by using `.put_message(ForceStaticObjectInplace(my_obj))` call
 
 It affects only the following data types: 
 * `AbstractSet` (`frozenset`)
 * `MutableSet` (`set`)
 * `Mapping`
 * `MutableMapping` (`dict`)
-* an instancess of custom classes including `dataclass` wrapped by `ForceGeneralObjectCopy` or `ForceGeneralObjectInplace` class instancess. For example by using `.put_message(ForceGeneralObjectInplace(my_obj))` call
+* an instances of custom classes including `dataclass` wrapped by `ForceGeneralObjectCopy` or `ForceGeneralObjectInplace` class instances. For example by using `.put_message(ForceGeneralObjectInplace(my_obj))` call
 
 ## Examples
 
 * An async examples (with asyncio):
     * [sender.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/sender.py)
     * [receiver.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/receiver.py)
     * [shared_objects__types.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/shared_objects__types.py)
 
 ### Receiver.py performance measurements
 
 ```python
-sso: SomeSharedObject = None  # variable for our shared object
-
 async with ashared_memory_context_manager.if_has_messages() as shared_memory:
-    sso = shared_memory.value.take_message()  # 5_833 iterations/seconds
-    company_metrics = sso.company_info.company_metrics  # 12_479 iterations/seconds
-    k = company_metrics[CompanyMetrics.in_a_good_state]  # 1_154_454 iterations/seconds
-    company_metrics[CompanyMetrics.in_a_good_state] = False  # 1_213_175 iterations/seconds
-    company_metrics[CompanyMetrics.in_a_good_state] = None  # 1_188_630 iterations/seconds
+    # Taking a message with an object from the queue.
+    sso: SomeSharedObject = shared_memory.value.take_message()  # 5_833 iterations/seconds
+
+    # We create local variables once in order to access them many times in the future, ensuring high performance.
+    # Applying a principle that is widely recommended for improving Python code.
+    company_metrics: List = sso.company_info.company_metrics  # 12_479 iterations/seconds
+    some_employee: Employee = sso.company_info.some_employee  # 10_568 iterations/seconds
+    data_dict: Dict = sso.data_dict  # 16_362 iterations/seconds
+    numpy_ndarray: np.ndarray = data_dict['key3']  # 26_223 iterations/seconds
+
+# Optimal work with shared data (through local variables):
+async with ashared_memory_context_manager as shared_memory:
+    # List
+    k = company_metrics[CompanyMetrics.avg_salary]  # 1_535_267 iterations/seconds
     k = company_metrics[CompanyMetrics.employees]  # 1_498_278 iterations/seconds
+    k = company_metrics[CompanyMetrics.in_a_good_state]  # 1_154_454 iterations/seconds
+    k = company_metrics[CompanyMetrics.websites]  # 380_258 iterations/seconds
+    company_metrics[CompanyMetrics.annual_income] = 2_000_000.0  # 1_380_983 iterations/seconds
     company_metrics[CompanyMetrics.employees] = 20  # 1_352_799 iterations/seconds
-    company_metrics[CompanyMetrics.employees] += 1  # 247_476 iterations/seconds
-    k = company_metrics[CompanyMetrics.avg_salary]  # 1_535_267 iterations/seconds
     company_metrics[CompanyMetrics.avg_salary] = 5_000.0  # 1_300_966 iterations/seconds
+    company_metrics[CompanyMetrics.in_a_good_state] = None  # 1_224_573 iterations/seconds
+    company_metrics[CompanyMetrics.in_a_good_state] = False  # 1_213_175 iterations/seconds
     company_metrics[CompanyMetrics.avg_salary] += 1.1  # 299_415 iterations/seconds
+    company_metrics[CompanyMetrics.employees] += 1  # 247_476 iterations/seconds
+    company_metrics[CompanyMetrics.emails] = tuple()  # 55_335 iterations/seconds (memory allocation performance is planned to be improved)
+    company_metrics[CompanyMetrics.emails] = ('sails@company.com',)  # 30_314 iterations/seconds (memory allocation performance is planned to be improved)
+    company_metrics[CompanyMetrics.emails] = ('sails@company.com', 'support@company.com')  # 20_860 iterations/seconds (memory allocation performance is planned to be improved)
+    company_metrics[CompanyMetrics.websites] = ['http://company.com', 'http://company.org']  # 10_465 iterations/seconds (memory allocation performance is planned to be improved)
+    
+    # Method call on a shared object that changes a property through the method
+    some_employee.increase_years_of_employment()  # 80548 iterations/seconds
+
+    # Object properties
     k = sso.int_value  # 850_098 iterations/seconds
+    k = sso.str_value  # 228_966 iterations/seconds
     sso.int_value = 200  # 207_480 iterations/seconds
     sso.int_value += 1  # 152_263 iterations/seconds
-    company_metrics[CompanyMetrics.annual_income] = 2_000_000.0  # 1_380_983 iterations/seconds
-    company_metrics[CompanyMetrics.emails] = tuple()  # 55_335 iterations/seconds
-    company_metrics[CompanyMetrics.emails] = ('sails@company.com',)  # 30_314 iterations/seconds
-    company_metrics[CompanyMetrics.emails] = ('sails@company.com', 'support@company.com')  # 20_860 iterations/seconds
-    k = company_metrics[CompanyMetrics.websites]  # 380_258 iterations/seconds
-    company_metrics[CompanyMetrics.websites] = ['http://company.com', 'http://company.org']  # 10_465 iterations/seconds
-    k = sso.str_value  # 228_966 iterations/seconds
-    sso.str_value = 'Hello. '  # 52_390 iterations/seconds
-    sso.str_value += '!'  # 35_823 iterations/seconds
-    data_dict = sso.data_dict  # 16_362 iterations/seconds
+    sso.str_value = 'Hello. '  # 52_390 iterations/seconds (memory allocation performance is planned to be improved)
+    sso.str_value += '!'  # 35_823 iterations/seconds (memory allocation performance is planned to be improved)
+
+    # Numpy.ndarray
+    numpy_ndarray += 10  # 403_646 iterations/seconds
+    numpy_ndarray -= 15  # 402_107 iterations/seconds
+
+    # Dict
     k = data_dict['key1']  # 87_558 iterations/seconds
+    k = data_dict[('key', 2)]  # 49_338 iterations/seconds
     data_dict['key1'] = 200  # 86_744 iterations/seconds
-    data_dict['key1'] *= 1  # 40_927 iterations/seconds
     data_dict['key1'] += 3  # 41_409 iterations/seconds
-    k = data_dict[('key', 2)]  # 49_338 iterations/seconds
-    data_dict[('key', 2)] = 'value2'  # 31_460 iterations/seconds
-    data_dict[('key', 2)] = data_dict[('key', 2)] + 'd'  # 18_972 iterations/seconds
-    data_dict[('key', 2)] = 'value2'  # 10_941 iterations/seconds
-    data_dict[('key', 2)] += 'd'  # 16_568 iterations/seconds
-    ndarray: np.ndarray = data_dict['key3']  # 26_223 iterations/seconds
-    ndarray += 10  # 403_246 iterations/seconds
-    data_dict['key3'] += 10  # 6_319 iterations/seconds
+    data_dict['key1'] *= 1  # 40_927 iterations/seconds
+    data_dict[('key', 2)] = 'value2'  # 31_460 iterations/seconds (memory allocation performance is planned to be improved)
+    data_dict[('key', 2)] = data_dict[('key', 2)] + 'd'  # 18_972 iterations/seconds (memory allocation performance is planned to be improved)
+    data_dict[('key', 2)] = 'value2'  # 10_941 iterations/seconds (memory allocation performance is planned to be improved)
+    data_dict[('key', 2)] += 'd'  # 16_568 iterations/seconds (memory allocation performance is planned to be improved)
+
+# An example of non-optimal work with shared data (without using a local variables):
+async with ashared_memory_context_manager as shared_memory:
+    # An example of a non-optimal method call (without using a local variable) that changes a property through the method
+    sso.company_info.some_employee.increase_years_of_employment()  # 9_418 iterations/seconds
+
+    # An example of non-optimal work with object properties (without using local variables)
     k = sso.company_info.income  # 20_445 iterations/seconds
     sso.company_info.income = 3_000_000.0  # 13_899 iterations/seconds
     sso.company_info.income *= 1.1  # 17_272 iterations/seconds 
     sso.company_info.income += 500_000.0  # 18_376 iterations/seconds
-    sso.company_info.some_employee.increase_years_of_employment()  # 9_429 iterations/seconds
+    
+    # Example of non-optimal usage of numpy.ndarray without a proper local variable
+    data_dict['key3'] += 10  # 6_319 iterations/seconds
+
+# Notify the sender about the completion of work on the shared object
+async with ashared_memory_context_manager as shared_memory:
     sso.some_processing_stage_control = True  # 298_968 iterations/seconds
 ```
 
 ## Reference (and explaining examples line by line)
 
 Code for shared memory Creator side:
 ```python
@@ -346,28 +376,28 @@
 ```python
 ashared_memory_context_manager: ASharedMemoryContextManager = asmm()
 # creates shared memory access context manager. Create it once per coroutine. Use in the same coroutine as much as you need it.
 ```
 
 ```python
 async with ashared_memory_context_manager as shared_memory:
-# acacquire access to shared memory as soon as possible
+# acquire access to shared memory as soon as possible
 ```
 
 ```python
 async with ashared_memory_context_manager.if_has_messages() as shared_memory:
-# acacquire access to shared memory if message queue is not empty
+# acquire access to shared memory if message queue is not empty
 ```
 
 ```python
 shared_memory # is an instance of ValueHolder class from the Cengal library
 shared_memory.value  # is an instance of `SharedMemory` instance
-shared_memory.existence  # bool. Will be set to True at the beginning of an eash context (`with`) block. Set it to `False`
-    # if you want to release CPU for a small time portion before shared memory will be acacquired next time.
-    # if at least one coroutine will not set it to `False` - next acacquire attempt will be made immidiately which will
+shared_memory.existence  # bool. Will be set to True at the beginning of an each context (`with`) block. Set it to `False`
+    # if you want to release CPU for a small time portion before shared memory will be acquired next time.
+    # if at least one coroutine will not set it to `False` - next acquire attempt will be made immediately which will
     # lower latency and increase performance but at the same time will consume more CPU time.
     # Default behavior (`True`) is better for CPU intensive algorithms, 
     # while `False` on all process coroutines (which have their own memory access context managers) will be better
     # for example for desktop or mobile applications
 ```
 
 ### `SharedMemory` fields and methods you might frequently use in an async approach (in coroutines)
@@ -504,15 +534,15 @@
 company_metrics['employees'] = 200  # 86_744 iterations/seconds
 company_metrics['employees'] += 3  # 41_409 iterations/seconds
 ```
 
 </details>
 <br>
 
-or even instead operating with dataclass (classess by default operate faster then dict):
+or even instead operating with dataclass (classes by default operate faster then dict):
 
 <details>
 <summary title="Example"><kbd> Example </kbd></summary>
 
 Message sender
 
 ```python
@@ -643,15 +673,15 @@
 </details>
 
 <details>
 <summary title="Custom classes (including `dataclass`)"><kbd> Custom classes (including `dataclass`) </kbd></summary>
 
 ### Custom classes (including `dataclass`)
 
-By default, shared custom class instancess (including `dataclass` instancess) have static set of attributes (similar to instancess of classes with `__slots__`). That means that all new (dynamically added to the mapped object, attributes will not became shared). This behavior increases performance.
+By default, shared custom class instances (including `dataclass` instances) have static set of attributes (similar to instances of classes with `__slots__`). That means that all new (dynamically added to the mapped object, attributes will not became shared). This behavior increases performance.
 
 <details>
 <summary title="For example"><kbd> For example </kbd></summary>
 
 #### For example
 
 ```python
@@ -820,15 +850,15 @@
 
 - [ ] Connect more than two processes
 - [ ] Use third-party fast hashing implementations instead of or in addition to built in `hash()` call
 - [ ] Continuous performance improvements
 
 ## Conclusion
 
-This Python package provides a robust solution for interprocess communication, supporting a variety of Python data structures, types, and third-party libraries. Its lock-free synchronization and asyncio compatibility make it an ideal choice for high-performance, concurrent execution.
+This Python package provides a robust solution for inter-process communication, supporting a variety of Python data structures, types, and third-party libraries. Its lock-free synchronization and asyncio compatibility make it an ideal choice for high-performance, concurrent execution.
 
 # Based on [Cengal](https://github.com/FI-Mihej/Cengal)
 
 This is a stand-alone package for a specific Cengal module. Package is designed to offer users the ability to install specific Cengal functionality without the burden of the library's full set of dependencies.
 
 The core of this approach lies in our 'cengal-light' package, which houses both Python and compiled Cengal modules. The 'cengal' package itself serves as a lightweight shell, devoid of its own modules, but dependent on 'cengal-light[full]' for a complete Cengal library installation with all required dependencies.
 
@@ -850,15 +880,15 @@
 
 
 # Projects using Cengal
 
 * [CengalPolyBuild](https://github.com/FI-Mihej/CengalPolyBuild) - A Comprehensive and Hackable Build System for Multilingual Python Packages: Cython (including automatic conversion from Python to Cython), C/C++, Objective-C, Go, and Nim, with ongoing expansions to include additional languages. (Planned to be released soon) 
 * [cengal_app_dir_path_finder](https://github.com/FI-Mihej/cengal_app_dir_path_finder) - A Python module offering a unified API for easy retrieval of OS-specific application directories, enhancing data management across Windows, Linux, and macOS 
 * [cengal_cpu_info](https://github.com/FI-Mihej/cengal_cpu_info) - Extended, cached CPU info with consistent output format.
-* [cengal_memory_barriers](https://github.com/FI-Mihej/cengal_memory_barriers) - Fast crossplatform memory barriers for Python.
+* [cengal_memory_barriers](https://github.com/FI-Mihej/cengal_memory_barriers) - Fast cross-platform memory barriers for Python.
 * [flet_async](https://github.com/FI-Mihej/flet_async) - wrapper which makes [Flet](https://github.com/flet-dev/flet) async and brings booth Cengal.coroutines and asyncio to Flet (Flutter based UI)
 * [justpy_containers](https://github.com/FI-Mihej/justpy_containers) - wrapper around [JustPy](https://github.com/justpy-org/justpy) in order to bring more security and more production-needed features to JustPy (VueJS based UI)
 * [Bensbach](https://github.com/FI-Mihej/Bensbach) - decompiler from Unreal Engine 3 bytecode to a Lisp-like script and compiler back to Unreal Engine 3 bytecode. Made for a game modding purposes
 * [Realistic-Damage-Model-mod-for-Long-War](https://github.com/FI-Mihej/Realistic-Damage-Model-mod-for-Long-War) - Mod for both the original XCOM:EW and the mod Long War. Was made with a Bensbach, which was made with Cengal
 * [SmartCATaloguer.com](http://www.smartcataloguer.com/index.html) - TagDB based catalog of images (tags), music albums (genre tags) and apps (categories)
 
 # License
```

