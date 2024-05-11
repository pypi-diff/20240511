# Comparing `tmp/zrcl-0.1.0.tar.gz` & `tmp/zrcl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zrcl-0.1.0.tar", max compression
+gzip compressed data, was "zrcl-0.2.1.tar", max compression
```

## Comparing `zrcl-0.1.0.tar` & `zrcl-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,32 @@
--rw-r--r--   0        0        0     1085 2024-05-09 17:36:26.540318 zrcl-0.1.0/LICENSE
--rw-r--r--   0        0        0     1278 2024-05-09 18:40:32.506454 zrcl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        9 2024-05-09 17:36:26.521175 zrcl-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-09 17:37:17.169306 zrcl-0.1.0/src/zrcl3_utils/__init__.py
--rw-r--r--   0        0        0     1371 2024-05-09 18:05:40.432405 zrcl-0.1.0/src/zrcl3_utils/easyocr.py
--rw-r--r--   0        0        0      837 2024-05-09 18:05:40.415956 zrcl-0.1.0/src/zrcl3_utils/hashlib.py
--rw-r--r--   0        0        0      208 2024-05-09 18:05:40.415956 zrcl-0.1.0/src/zrcl3_utils/json.py
--rw-r--r--   0        0        0      427 2024-05-09 18:05:40.415956 zrcl-0.1.0/src/zrcl3_utils/keyring.py
--rw-r--r--   0        0        0      128 2024-05-09 18:05:40.415450 zrcl-0.1.0/src/zrcl3_utils/logging.py
--rw-r--r--   0        0        0      149 2024-05-09 18:05:40.415956 zrcl-0.1.0/src/zrcl3_utils/os.py
--rw-r--r--   0        0        0      234 2024-05-09 18:05:40.415956 zrcl-0.1.0/src/zrcl3_utils/pillow.py
--rw-r--r--   0        0        0     1824 2024-05-09 18:05:40.446413 zrcl-0.1.0/src/zrcl3_utils/pygetwindow.py
--rw-r--r--   0        0        0     2374 2024-05-09 18:05:40.448673 zrcl-0.1.0/src/zrcl3_utils/pyscreeze.py
--rw-r--r--   0        0        0      441 2024-05-09 18:05:40.439260 zrcl-0.1.0/src/zrcl3_utils/pywin32.py
--rw-r--r--   0        0        0     1691 2024-05-09 18:05:40.455832 zrcl-0.1.0/src/zrcl3_utils/screeninfo.py
--rw-r--r--   0        0        0     4434 2024-05-09 18:05:40.464698 zrcl-0.1.0/src/zrcl3_utils/subprocess.py
--rw-r--r--   0        0        0     1511 2024-05-09 18:05:40.456834 zrcl-0.1.0/src/zrcl3_utils/time.py
--rw-r--r--   0        0        0     2055 2024-05-09 18:05:40.465138 zrcl-0.1.0/src/zrcl3_utils/typing.py
--rw-r--r--   0        0        0        0 2024-05-09 17:37:17.169306 zrcl-0.1.0/src/zrcl4/__init__.py
--rw-r--r--   0        0        0     8689 2024-05-09 18:36:43.510299 zrcl-0.1.0/src/zrcl4/automation.py
--rw-r--r--   0        0        0      245 2024-05-09 18:05:40.455832 zrcl-0.1.0/src/zrcl4/bit.py
--rw-r--r--   0        0        0     2240 2024-05-09 18:05:40.471062 zrcl-0.1.0/src/zrcl4/cli_selection.py
--rw-r--r--   0        0        0      276 2024-05-09 18:05:40.453821 zrcl-0.1.0/src/zrcl4/do_nothing.py
--rw-r--r--   0        0        0     5049 2024-05-09 18:13:49.682755 zrcl-0.1.0/src/zrcl4/file.py
--rw-r--r--   0        0        0        0 2024-05-09 17:37:17.169306 zrcl-0.1.0/src/zrcl4/github.py
--rw-r--r--   0        0        0     1478 2024-05-09 18:05:40.475062 zrcl-0.1.0/src/zrcl4/markdown.py
--rw-r--r--   0        0        0      455 2024-05-09 18:05:40.469121 zrcl-0.1.0/src/zrcl4/singleton.py
--rw-r--r--   0        0        0     1228 2024-05-09 18:05:40.415956 zrcl-0.1.0/src/zrcl4/zip_crack.py
--rw-r--r--   0        0        0      377 1970-01-01 00:00:00.000000 zrcl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-05-09 17:36:26.540318 zrcl-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1524 2024-05-11 15:07:05.569684 zrcl-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1093 2024-05-11 15:06:11.869950 zrcl-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 17:37:17.169306 zrcl-0.2.1/src/zrcl3_uses/__init__.py
+-rw-r--r--   0        0        0     8659 2024-05-10 17:35:14.805179 zrcl-0.2.1/src/zrcl3_uses/automation.py
+-rw-r--r--   0        0        0      245 2024-05-09 18:05:40.455832 zrcl-0.2.1/src/zrcl3_uses/bit.py
+-rw-r--r--   0        0        0     2240 2024-05-09 18:05:40.471062 zrcl-0.2.1/src/zrcl3_uses/cli_selection.py
+-rw-r--r--   0        0        0      276 2024-05-09 18:05:40.453821 zrcl-0.2.1/src/zrcl3_uses/do_nothing.py
+-rw-r--r--   0        0        0     5043 2024-05-10 17:35:14.805179 zrcl-0.2.1/src/zrcl3_uses/file.py
+-rw-r--r--   0        0        0     4764 2024-05-10 19:06:51.955640 zrcl-0.2.1/src/zrcl3_uses/github.py
+-rw-r--r--   0        0        0     1478 2024-05-09 18:05:40.475062 zrcl-0.2.1/src/zrcl3_uses/markdown.py
+-rw-r--r--   0        0        0     6922 2024-05-10 17:45:30.801464 zrcl-0.2.1/src/zrcl3_uses/png_meta.py
+-rw-r--r--   0        0        0      455 2024-05-09 18:05:40.469121 zrcl-0.2.1/src/zrcl3_uses/singleton.py
+-rw-r--r--   0        0        0     1228 2024-05-09 18:05:40.415956 zrcl-0.2.1/src/zrcl3_uses/zip_crack.py
+-rw-r--r--   0        0        0       49 2024-05-10 18:43:59.832504 zrcl-0.2.1/src/zrcl4/__init__.py
+-rw-r--r--   0        0        0     2594 2024-05-10 18:43:59.862096 zrcl-0.2.1/src/zrcl4/__primitive__.py
+-rw-r--r--   0        0        0     5144 2024-05-10 18:43:59.867653 zrcl-0.2.1/src/zrcl4/cryptography.py
+-rw-r--r--   0        0        0     1371 2024-05-09 18:05:40.432405 zrcl-0.2.1/src/zrcl4/easyocr.py
+-rw-r--r--   0        0        0      837 2024-05-09 18:05:40.415956 zrcl-0.2.1/src/zrcl4/hashlib.py
+-rw-r--r--   0        0        0      208 2024-05-09 18:05:40.415956 zrcl-0.2.1/src/zrcl4/json.py
+-rw-r--r--   0        0        0      427 2024-05-09 18:05:40.415956 zrcl-0.2.1/src/zrcl4/keyring.py
+-rw-r--r--   0        0        0      128 2024-05-09 18:05:40.415450 zrcl-0.2.1/src/zrcl4/logging.py
+-rw-r--r--   0        0        0      149 2024-05-09 18:05:40.415956 zrcl-0.2.1/src/zrcl4/os.py
+-rw-r--r--   0        0        0      234 2024-05-09 18:05:40.415956 zrcl-0.2.1/src/zrcl4/pillow.py
+-rw-r--r--   0        0        0     1824 2024-05-09 18:05:40.446413 zrcl-0.2.1/src/zrcl4/pygetwindow.py
+-rw-r--r--   0        0        0     2374 2024-05-09 18:05:40.448673 zrcl-0.2.1/src/zrcl4/pyscreeze.py
+-rw-r--r--   0        0        0      441 2024-05-09 18:05:40.439260 zrcl-0.2.1/src/zrcl4/pywin32.py
+-rw-r--r--   0        0        0     1691 2024-05-09 18:05:40.455832 zrcl-0.2.1/src/zrcl4/screeninfo.py
+-rw-r--r--   0        0        0     4434 2024-05-09 18:05:40.464698 zrcl-0.2.1/src/zrcl4/subprocess.py
+-rw-r--r--   0        0        0     1511 2024-05-09 18:05:40.456834 zrcl-0.2.1/src/zrcl4/time.py
+-rw-r--r--   0        0        0     2055 2024-05-09 18:05:40.465138 zrcl-0.2.1/src/zrcl4/typing.py
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 zrcl-0.2.1/PKG-INFO
```

### Comparing `zrcl-0.1.0/LICENSE` & `zrcl-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zrcl-0.1.0/pyproject.toml` & `zrcl-0.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 [tool.poetry]
 name = "zrcl"
-version = "0.1.0"
+version = "0.2.1"
 description = ""
 authors = ["ZackaryW <36378555+ZackaryW@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "zrcl4", from = "src" },
-    { include = "zrcl3_utils", from = "src" },
+    { include = "zrcl3_uses", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.12, <4.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.1,<25.0"
+
+[tool.poetry.group.extra-dev.dependencies]
 pygetwindow = ">=0.0.9"
 readchar=">=4.0.6"
 pytest="8.2.0"
 click=">=8.1.7"
 toml = ">=0.10.2"
 easyocr = ">=1.7.1"
 pyautogui = ">=0.9.54"
 pandas = ">=2.2.2"
 thefuzz = ">=0.22.1"
 orjson = ">=3.10.3"
-pywin32 = ">=306"
 marisa-trie = ">=1.1.1"
 py7zr = ">=0.21.0"
-
-
 screeninfo = "^0.8.1"
+cryptography = "^42.0.7"
+pywin32 = { version = "^304", optional = true }
+
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=7.2.6"
 sphinx-autobuild = ">=2024.2.4"
 sphinx-copybutton = ">=0.5.2"
 furo = ">=2024.1.29"
 
 [tool.black]
@@ -58,7 +60,16 @@
     | buck-out
     | build
     | dist
   )/
 )
 '''
 
+[tool.pytest.ini_options]
+addopts = "-ra -q"
+testpaths = [
+    "tests",
+]
+pythonpath  = ["src"]
+
+[tool.poetry.extras]
+extra = ["extra-dev"]
```

### Comparing `zrcl-0.1.0/src/zrcl3_utils/easyocr.py` & `zrcl-0.2.1/src/zrcl4/easyocr.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.1.0/src/zrcl3_utils/hashlib.py` & `zrcl-0.2.1/src/zrcl4/hashlib.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.1.0/src/zrcl3_utils/pygetwindow.py` & `zrcl-0.2.1/src/zrcl4/pygetwindow.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.1.0/src/zrcl3_utils/pyscreeze.py` & `zrcl-0.2.1/src/zrcl4/pyscreeze.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.1.0/src/zrcl3_utils/screeninfo.py` & `zrcl-0.2.1/src/zrcl4/screeninfo.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.1.0/src/zrcl3_utils/subprocess.py` & `zrcl-0.2.1/src/zrcl4/subprocess.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.1.0/src/zrcl3_utils/time.py` & `zrcl-0.2.1/src/zrcl4/time.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.1.0/src/zrcl3_utils/typing.py` & `zrcl-0.2.1/src/zrcl4/typing.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.1.0/src/zrcl4/automation.py` & `zrcl-0.2.1/src/zrcl3_uses/automation.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 from functools import cached_property
 import time
 import typing
 import numpy
 import pygetwindow as gw
 from PIL import Image
 import screeninfo
-from zrcl3_utils.pillow import load_base64_img
-from zrcl3_utils.pygetwindow import activate_wnd
-from zrcl3_utils.screeninfo import get_primary_monitor, wnd_on_monitor
+from zrcl4.pillow import load_base64_img
+from zrcl4.pygetwindow import activate_wnd
+from zrcl4.screeninfo import get_primary_monitor, wnd_on_monitor
 
 
 def img_reg(token: "AutoToken"):
-    from zrcl3_utils.pyscreeze import locate
+    from zrcl4.pyscreeze import locate
 
     return locate(
         token.sourceImg,
         token.targetImg,
         _algo=token.cfg_imgAlgo,
         confidence=token.confidence,
     )
 
 
 def ocr(token: "AutoToken"):
-    from zrcl3_utils.easyocr import get_text_coordinates, EasyOCRMeta
+    from zrcl4.easyocr import get_text_coordinates, EasyOCRMeta
 
     imagearr = numpy.array(token.targetImg)
     res: list[EasyOCRMeta] = get_text_coordinates(imagearr, token.cfg_ocrLang)
     token.ocrMatchResult = res
     if token.cfg_ocrMatchMethod == "fuzz":
         from thefuzz import process
```

### Comparing `zrcl-0.1.0/src/zrcl4/cli_selection.py` & `zrcl-0.2.1/src/zrcl3_uses/cli_selection.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.1.0/src/zrcl4/file.py` & `zrcl-0.2.1/src/zrcl3_uses/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections.abc import Callable
 import os
 import typing
-from zrcl3_utils.hashlib import hash_file
+from zrcl4.hashlib import hash_file
 
 
 # ANCHOR loading files
 def get_serialize_data(path: str):
     if path.endswith(".json"):
         import json
```

### Comparing `zrcl-0.1.0/src/zrcl4/markdown.py` & `zrcl-0.2.1/src/zrcl3_uses/markdown.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.1.0/src/zrcl4/zip_crack.py` & `zrcl-0.2.1/src/zrcl3_uses/zip_crack.py`

 * *Files identical despite different names*

