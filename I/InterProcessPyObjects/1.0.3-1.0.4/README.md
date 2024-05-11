# Comparing `tmp/interprocesspyobjects-1.0.3.tar.gz` & `tmp/interprocesspyobjects-1.0.4.tar.gz`

## Comparing `interprocesspyobjects-1.0.3.tar` & `interprocesspyobjects-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/ipc_py_objects/__init__.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/ipc_py_objects/versions/__init__.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/ipc_py_objects/versions/v_0/__init__.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/ipc_py_objects/versions/v_1/__init__.py
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/LICENSE.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/NOTICE
--rw-r--r--   0        0        0    39612 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/README.md
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    44228 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.4/ipc_py_objects/__init__.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.4/ipc_py_objects/versions/__init__.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.4/ipc_py_objects/versions/v_0/__init__.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.4/ipc_py_objects/versions/v_1/__init__.py
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.4/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.4/LICENSE.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.4/NOTICE
+-rw-r--r--   0        0        0    39743 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.4/README.md
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    44359 2020-02-02 00:00:00.000000 interprocesspyobjects-1.0.4/PKG-INFO
```

### Comparing `interprocesspyobjects-1.0.3/ipc_py_objects/__init__.py` & `interprocesspyobjects-1.0.4/ipc_py_objects/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 """
 
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
 __copyright__ = "Copyright © 2012-2024 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
 __credits__ = ["ButenkoMS <gtalk@butenkoms.space>", ]
 __license__ = "Apache License, Version 2.0"
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 __status__ = "Production"
 
 
 from .versions import *
```

### Comparing `interprocesspyobjects-1.0.3/ipc_py_objects/versions/__init__.py` & `interprocesspyobjects-1.0.4/ipc_py_objects/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.3/ipc_py_objects/versions/v_0/__init__.py` & `interprocesspyobjects-1.0.4/ipc_py_objects/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.3/ipc_py_objects/versions/v_1/__init__.py` & `interprocesspyobjects-1.0.4/ipc_py_objects/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.3/.gitignore` & `interprocesspyobjects-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.3/LICENSE.md` & `interprocesspyobjects-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.3/NOTICE` & `interprocesspyobjects-1.0.4/NOTICE`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.3/README.md` & `interprocesspyobjects-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,18 @@
 * An async examples (with asyncio):
     * [sender.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/sender.py)
     * [receiver.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/receiver.py)
     * [shared_objects__types.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/shared_objects__types.py)
 
 ### Receiver.py performance measurements
 
+* CPU: i5-3570@3.40GHz (Ivy Bridge)
+* RAM: 32 GBytes, DDR3, dual channel, 655 MHz
+* OS: Ubuntu 20.04.6 LTS under WSL2. Windows 10
+
 ```python
 async with ashared_memory_context_manager.if_has_messages() as shared_memory:
     # Taking a message with an object from the queue.
     sso: SomeSharedObject = shared_memory.value.take_message()  # 5_833 iterations/seconds
 
     # We create local variables once in order to access them many times in the future, ensuring high performance.
     # Applying a principle that is widely recommended for improving Python code.
```

### Comparing `interprocesspyobjects-1.0.3/pyproject.toml` & `interprocesspyobjects-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `interprocesspyobjects-1.0.3/PKG-INFO` & `interprocesspyobjects-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: InterProcessPyObjects
-Version: 1.0.3
+Version: 1.0.4
 Summary: This high-performance package delivers blazing-fast inter-process communication through shared memory, enabling Python objects to be shared across processes with exceptional efficiency
 Project-URL: Homepage, https://github.com/FI-Mihej/InterProcessPyObjects
 Author-email: ButenkoMS <gtalk@butenkoms.space>
 License-Expression: Apache-2.0
 License-File: LICENSE.md
 License-File: NOTICE
 Keywords: Android,IPC,Linux,Windows,cengal,crossplatform,iOS,inter-process communication,macOS,multiprocessing,shared dict,shared memory,shared numpy ndarray,shared object,shared objects,shared set,shared torch Tensor
@@ -265,14 +265,18 @@
 * An async examples (with asyncio):
     * [sender.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/sender.py)
     * [receiver.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/receiver.py)
     * [shared_objects__types.py](https://github.com/FI-Mihej/InterProcessPyObjects/blob/master/example/shared_objects__types.py)
 
 ### Receiver.py performance measurements
 
+* CPU: i5-3570@3.40GHz (Ivy Bridge)
+* RAM: 32 GBytes, DDR3, dual channel, 655 MHz
+* OS: Ubuntu 20.04.6 LTS under WSL2. Windows 10
+
 ```python
 async with ashared_memory_context_manager.if_has_messages() as shared_memory:
     # Taking a message with an object from the queue.
     sso: SomeSharedObject = shared_memory.value.take_message()  # 5_833 iterations/seconds
 
     # We create local variables once in order to access them many times in the future, ensuring high performance.
     # Applying a principle that is widely recommended for improving Python code.
```

