# Comparing `tmp/pytrydan-0.6.0.tar.gz` & `tmp/pytrydan-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrydan-0.6.0.tar", max compression
+gzip compressed data, was "pytrydan-0.6.1.tar", max compression
```

## Comparing `pytrydan-0.6.0.tar` & `pytrydan-0.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2024-05-09 14:56:18.883314 pytrydan-0.6.0/LICENSE
--rw-r--r--   0        0        0     4822 2024-05-09 14:56:18.883314 pytrydan-0.6.0/README.md
--rw-r--r--   0        0        0     3517 2024-05-09 14:56:19.603303 pytrydan-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      754 2024-05-09 14:56:18.883314 pytrydan-0.6.0/src/pytrydan/__init__.py
--rw-r--r--   0        0        0      102 2024-05-09 14:56:18.883314 pytrydan-0.6.0/src/pytrydan/__main__.py
--rw-r--r--   0        0        0     2003 2024-05-09 14:56:18.883314 pytrydan-0.6.0/src/pytrydan/cli.py
--rw-r--r--   0        0        0      340 2024-05-09 14:56:18.883314 pytrydan-0.6.0/src/pytrydan/const.py
--rw-r--r--   0        0        0      562 2024-05-09 14:56:18.883314 pytrydan-0.6.0/src/pytrydan/exceptions.py
--rw-r--r--   0        0        0     2053 2024-05-09 14:56:18.883314 pytrydan-0.6.0/src/pytrydan/main.py
--rw-r--r--   0        0        0     4132 2024-05-09 14:56:18.883314 pytrydan-0.6.0/src/pytrydan/models/trydan.py
--rw-r--r--   0        0        0        0 2024-05-09 14:56:18.883314 pytrydan-0.6.0/src/pytrydan/py.typed
--rw-r--r--   0        0        0     9434 2024-05-09 14:56:18.883314 pytrydan-0.6.0/src/pytrydan/trydan.py
--rw-r--r--   0        0        0     6029 1970-01-01 00:00:00.000000 pytrydan-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-11 13:49:57.271379 pytrydan-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4822 2024-05-11 13:49:57.271379 pytrydan-0.6.1/README.md
+-rw-r--r--   0        0        0     3517 2024-05-11 13:49:57.963380 pytrydan-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      754 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/__init__.py
+-rw-r--r--   0        0        0      102 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/__main__.py
+-rw-r--r--   0        0        0     2003 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/cli.py
+-rw-r--r--   0        0        0      340 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/const.py
+-rw-r--r--   0        0        0      562 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/exceptions.py
+-rw-r--r--   0        0        0     2053 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/main.py
+-rw-r--r--   0        0        0     4129 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/models/trydan.py
+-rw-r--r--   0        0        0        0 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/py.typed
+-rw-r--r--   0        0        0     9434 2024-05-11 13:49:57.271379 pytrydan-0.6.1/src/pytrydan/trydan.py
+-rw-r--r--   0        0        0     6029 1970-01-01 00:00:00.000000 pytrydan-0.6.1/PKG-INFO
```

### Comparing `pytrydan-0.6.0/LICENSE` & `pytrydan-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.0/README.md` & `pytrydan-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.0/pyproject.toml` & `pytrydan-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytrydan"
-version = "0.6.0"
+version = "0.6.1"
 description = "Library to interface with V2C EVSE Trydan"
 authors = ["Diogo Gomes <diogogomes@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dgomes/pytrydan"
 documentation = "https://pytrydan.readthedocs.io"
 classifiers = [
```

### Comparing `pytrydan-0.6.0/src/pytrydan/__init__.py` & `pytrydan-0.6.1/src/pytrydan/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.0/src/pytrydan/cli.py` & `pytrydan-0.6.1/src/pytrydan/cli.py`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.0/src/pytrydan/exceptions.py` & `pytrydan-0.6.1/src/pytrydan/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.0/src/pytrydan/main.py` & `pytrydan-0.6.1/src/pytrydan/main.py`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.0/src/pytrydan/models/trydan.py` & `pytrydan-0.6.1/src/pytrydan/models/trydan.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,23 +44,23 @@
     NEGATIVE_ACKNOWLEDGE = 27
     MEMORY_PARITY_ERROR = 28
     GATEWAY_PATH_UNAVAILABLE = 30
     GATEWAY_TARGET_NO_RESP = 31
     SERVER_RTU_INACTIVE244_TIMEOUT = 32
     INVALID_SERVER = 245
     CRC_ERROR = 246
-    FC_MISSMATCH = 247
-    SERVER_ID_MISSMATCH = 248
+    FC_MISMATCH = 247
+    SERVER_ID_MISMATCH = 248
     PACKET_LENGTH_ERROR = 249
     PARAMETER_COUNT_ERROR = 250
     PARAMETER_LIMIT_ERROR = 251
     REQUEST_QUEUE_FULL = 252
     ILLEGAL_IP_OR_PORT = 253
     IP_CONNECTION_FAILED = 254
-    TCP_HEAD_MISSMATCH = 255
+    TCP_HEAD_MISMATCH = 255
     EMPTY_MESSAGE = 256
     UNDEFINED_ERROR = 257
 
 
 class PauseState(IntEnum):
     """Enum for Pause State."""
```

### Comparing `pytrydan-0.6.0/src/pytrydan/trydan.py` & `pytrydan-0.6.1/src/pytrydan/trydan.py`

 * *Files identical despite different names*

### Comparing `pytrydan-0.6.0/PKG-INFO` & `pytrydan-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrydan
-Version: 0.6.0
+Version: 0.6.1
 Summary: Library to interface with V2C EVSE Trydan
 Home-page: https://github.com/dgomes/pytrydan
 License: MIT
 Author: Diogo Gomes
 Author-email: diogogomes@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytrydan Version: 0.6.0 Summary: Library to
+Metadata-Version: 2.1 Name: pytrydan Version: 0.6.1 Summary: Library to
 interface with V2C EVSE Trydan Home-page: https://github.com/dgomes/pytrydan
 License: MIT Author: Diogo Gomes Author-email: diogogomes@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

