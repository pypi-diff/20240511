# Comparing `tmp/robotcode_core-0.82.1.tar.gz` & `tmp/robotcode_core-0.82.2.tar.gz`

## Comparing `robotcode_core-0.82.1.tar` & `robotcode_core-0.82.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/__version__.py
--rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/async_tools.py
--rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/concurrent.py
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/documents_manager.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/event.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/filewatcher.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/language.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/py.typed
--rw-r--r--   0        0        0     9484 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/text_document.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/types.py
--rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/uri.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/lsp/__init__.py
--rw-r--r--   0        0        0   233360 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/lsp/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/utils/__init__.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/utils/caching.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/utils/cli.py
--rw-r--r--   0        0        0    21972 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/utils/dataclasses.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/utils/debugpy.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/utils/glob_path.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/utils/inspect.py
--rw-r--r--   0        0        0    16387 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/utils/logging.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/utils/net.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/utils/path.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/utils/process.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/utils/safe_eval.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/src/robotcode/core/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/LICENSE.txt
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/README.md
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/pyproject.toml
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 robotcode_core-0.82.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/__version__.py
+-rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/async_tools.py
+-rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/concurrent.py
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/documents_manager.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/event.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/filewatcher.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/language.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/py.typed
+-rw-r--r--   0        0        0     9484 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/text_document.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/types.py
+-rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/uri.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/lsp/__init__.py
+-rw-r--r--   0        0        0   233360 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/lsp/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/utils/__init__.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/utils/caching.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/utils/cli.py
+-rw-r--r--   0        0        0    21972 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/utils/dataclasses.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/utils/debugpy.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/utils/glob_path.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/utils/inspect.py
+-rw-r--r--   0        0        0    16387 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/utils/logging.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/utils/net.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/utils/path.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/utils/process.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/utils/safe_eval.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/src/robotcode/core/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/LICENSE.txt
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/README.md
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/pyproject.toml
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 robotcode_core-0.82.2/PKG-INFO
```

### Comparing `robotcode_core-0.82.1/src/robotcode/core/async_tools.py` & `robotcode_core-0.82.2/src/robotcode/core/async_tools.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/concurrent.py` & `robotcode_core-0.82.2/src/robotcode/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/documents_manager.py` & `robotcode_core-0.82.2/src/robotcode/core/documents_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/event.py` & `robotcode_core-0.82.2/src/robotcode/core/event.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/filewatcher.py` & `robotcode_core-0.82.2/src/robotcode/core/filewatcher.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/language.py` & `robotcode_core-0.82.2/src/robotcode/core/language.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/text_document.py` & `robotcode_core-0.82.2/src/robotcode/core/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/uri.py` & `robotcode_core-0.82.2/src/robotcode/core/uri.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/workspace.py` & `robotcode_core-0.82.2/src/robotcode/core/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/lsp/types.py` & `robotcode_core-0.82.2/src/robotcode/core/lsp/types.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/utils/caching.py` & `robotcode_core-0.82.2/src/robotcode/core/utils/caching.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/utils/dataclasses.py` & `robotcode_core-0.82.2/src/robotcode/core/utils/dataclasses.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/utils/debugpy.py` & `robotcode_core-0.82.2/src/robotcode/core/utils/debugpy.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/utils/glob_path.py` & `robotcode_core-0.82.2/src/robotcode/core/utils/glob_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/utils/inspect.py` & `robotcode_core-0.82.2/src/robotcode/core/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/utils/logging.py` & `robotcode_core-0.82.2/src/robotcode/core/utils/logging.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/utils/net.py` & `robotcode_core-0.82.2/src/robotcode/core/utils/net.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/utils/path.py` & `robotcode_core-0.82.2/src/robotcode/core/utils/path.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/utils/process.py` & `robotcode_core-0.82.2/src/robotcode/core/utils/process.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/utils/safe_eval.py` & `robotcode_core-0.82.2/src/robotcode/core/utils/safe_eval.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/src/robotcode/core/utils/version.py` & `robotcode_core-0.82.2/src/robotcode/core/utils/version.py`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/.gitignore` & `robotcode_core-0.82.2/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/LICENSE.txt` & `robotcode_core-0.82.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/README.md` & `robotcode_core-0.82.2/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/pyproject.toml` & `robotcode_core-0.82.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_core-0.82.1/PKG-INFO` & `robotcode_core-0.82.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: robotcode-core
-Version: 0.82.1
+Version: 0.82.2
 Summary: Some core classes for RobotCode
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://opencollective.com/robotcode
 Project-URL: Documentation, https://github.com/robotcodedev/robotcode#readme
 Project-URL: Changelog, https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/robotcodedev/robotcode/issues
 Project-URL: Source, https://github.com/robotcodedev/robotcode
```

