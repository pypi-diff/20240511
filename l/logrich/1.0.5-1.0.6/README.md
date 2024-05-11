# Comparing `tmp/logrich-1.0.5.tar.gz` & `tmp/logrich-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logrich-1.0.5.tar", max compression
+gzip compressed data, was "logrich-1.0.6.tar", max compression
```

## Comparing `logrich-1.0.5.tar` & `logrich-1.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1184 2023-03-25 11:37:39.185788 logrich-1.0.5/README.md
--rw-r--r--   0        0        0       34 2024-05-11 05:30:18.783717 logrich-1.0.5/logrich/__init__.py
--rw-r--r--   0        0        0     8252 2024-05-11 05:46:02.327905 logrich-1.0.5/logrich/app.py
--rw-r--r--   0        0        0     1497 2024-05-11 05:08:07.127338 logrich-1.0.5/logrich/config.py
--rw-r--r--   0        0        0     1047 2024-05-11 05:42:54.601043 logrich-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 logrich-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1184 2023-03-25 11:37:39.185788 logrich-1.0.6/README.md
+-rw-r--r--   0        0        0       34 2024-05-11 05:30:18.783717 logrich-1.0.6/logrich/__init__.py
+-rw-r--r--   0        0        0     8368 2024-05-11 10:55:55.540193 logrich-1.0.6/logrich/app.py
+-rw-r--r--   0        0        0     1497 2024-05-11 05:08:07.127338 logrich-1.0.6/logrich/config.py
+-rw-r--r--   0        0        0     1047 2024-05-11 10:55:55.540193 logrich-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 logrich-1.0.6/PKG-INFO
```

### Comparing `logrich-1.0.5/README.md` & `logrich-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `logrich-1.0.5/logrich/app.py` & `logrich-1.0.6/logrich/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import decimal
 import inspect
 import re
 from collections import deque
-from collections.abc import Callable, Sequence
+from collections.abc import Callable
 from datetime import datetime
 from functools import lru_cache
+from types import FrameType
 from typing import Any
 
 from rich.console import Console
 from rich.highlighter import ReprHighlighter
 from rich.pretty import pprint  # noqa
 from rich.table import Table
 from rich.theme import Theme
+from typing_extensions import reveal_type  # noqa
 
 from logrich.config import config
 
 console = Console()
 
 
 def combine_regex(*regexes: str) -> str:
@@ -102,44 +104,45 @@
         self.config = config
         for k, v in kwargs.items():
             self.__setattr__(k, v)
 
     def print(
         self,
         # вызов логгера без параметров выведет текущую дату
-        *msg: Sequence,
-        frame=None,
+        *args,
+        frame: FrameType | None = None,
         **kwargs,
     ) -> None:
         """Extension log."""
         try:
-            if msg and len(msg) == 1:
-                msg = msg[0]
-            elif not msg:
-                msg = msg or datetime.now().strftime("%H:%M:%S")
+            if args and len(args) == 1:
+                msg = args[0]
+            elif not args:
+                msg = datetime.now().strftime("%H:%M:%S")
+            else:
+                msg = args
 
             if not (level := self.deque.pop()):  # noqa
                 return
 
             level_key = f"LOG_LEVEL_{level.upper()}_TPL"
             level_style = self.config.get(level_key, "").strip('"')
             if not level_style:
                 return
+            frame = frame or inspect.currentframe().f_back  # type: ignore
 
-            frame = frame or inspect.currentframe().f_back
             len_file_name_section = 30
-            file_name = kwargs.get("file_name", frame.f_code.co_filename)[-len_file_name_section:]
-            line = kwargs.get("line", frame.f_lineno)
-            divider = int(self.config.get("COLUMNS")) - len_file_name_section - 20
+            file_name = kwargs.get("file_name", frame.f_code.co_filename)[-len_file_name_section:]  # type: ignore
+            line = kwargs.get("line", frame.f_lineno)  # type: ignore
+            divider = int(self.config.get("COLUMNS")) - len_file_name_section - 20  # type: ignore
             title = kwargs.get("title", "-" * divider)
 
             if isinstance(msg, str | int | float | bool | type(decimal) | type(None)):
-                # if isinstance(msg, (str, int, float, bool, type(decimal), type(None))):
                 self.print_tbl(
-                    message=msg,
+                    message=str(msg),
                     file=file_name,
                     line=line,
                     level=level,
                     level_style=level_style,
                 )
             elif isinstance(msg, (dict | tuple | list)):
                 # TODO add message for dict, tuple etc.
@@ -151,15 +154,15 @@
                     level_style=level_style,
                 )
                 self.format_extra_obj(message=msg)
             else:
                 self.print_tbl(
                     message=msg,
                     file=file_name,
-                    line=frame.f_lineno,
+                    line=frame.f_lineno,  # type: ignore
                     level=level,
                     level_style=level_style,
                 )
         except Exception as err:
             log.warning(err)
 
     def print_tbl(
```

### Comparing `logrich-1.0.5/logrich/config.py` & `logrich-1.0.6/logrich/config.py`

 * *Files identical despite different names*

### Comparing `logrich-1.0.5/pyproject.toml` & `logrich-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "logrich"
-version = "1.0.5"
+version = "1.0.6"
 description = "loguru + rich = logrich"
 authors = ["Dmitry Mavlin <mavlind@list.ru>"]
 license = "GPL"
 readme = "README.md"
 keywords = ["logger", "loguru", "rich"]
 
 [project.urls]
```

### Comparing `logrich-1.0.5/PKG-INFO` & `logrich-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logrich
-Version: 1.0.5
+Version: 1.0.6
 Summary: loguru + rich = logrich
 License: GPL
 Keywords: logger,loguru,rich
 Author: Dmitry Mavlin
 Author-email: mavlind@list.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

