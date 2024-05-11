# Comparing `tmp/logrich-1.0.4.tar.gz` & `tmp/logrich-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logrich-1.0.4.tar", max compression
+gzip compressed data, was "logrich-1.0.5.tar", max compression
```

## Comparing `logrich-1.0.4.tar` & `logrich-1.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1184 2023-03-25 11:37:39.185788 logrich-1.0.4/README.md
--rw-r--r--   0        0        0       21 2023-10-02 10:23:50.197687 logrich-1.0.4/logrich/__init__.py
--rw-r--r--   0        0        0     7982 2024-04-10 03:54:37.054485 logrich-1.0.4/logrich/app.py
--rw-r--r--   0        0        0     1505 2024-04-10 03:54:37.054485 logrich-1.0.4/logrich/config.py
--rw-r--r--   0        0        0     1145 2024-04-10 03:54:37.054485 logrich-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 logrich-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1184 2023-03-25 11:37:39.185788 logrich-1.0.5/README.md
+-rw-r--r--   0        0        0       34 2024-05-11 05:30:18.783717 logrich-1.0.5/logrich/__init__.py
+-rw-r--r--   0        0        0     8252 2024-05-11 05:46:02.327905 logrich-1.0.5/logrich/app.py
+-rw-r--r--   0        0        0     1497 2024-05-11 05:08:07.127338 logrich-1.0.5/logrich/config.py
+-rw-r--r--   0        0        0     1047 2024-05-11 05:42:54.601043 logrich-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1986 1970-01-01 00:00:00.000000 logrich-1.0.5/PKG-INFO
```

### Comparing `logrich-1.0.4/README.md` & `logrich-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `logrich-1.0.4/logrich/app.py` & `logrich-1.0.5/logrich/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import decimal
 import inspect
 import re
 from collections import deque
+from collections.abc import Callable, Sequence
 from datetime import datetime
 from functools import lru_cache
-from typing import Any, Deque
+from typing import Any
 
 from rich.console import Console
 from rich.highlighter import ReprHighlighter
 from rich.pretty import pprint  # noqa
 from rich.table import Table
 from rich.theme import Theme
 
 from logrich.config import config
 
-
 console = Console()
 
 
 def combine_regex(*regexes: str) -> str:
     """Combine a number of regexes in to a single regex.
 
     Returns:
@@ -93,29 +93,34 @@
 )
 
 
 @lru_cache
 class Log:
     """Extension log, use in tests."""
 
-    def __init__(self, config: dict, **kwargs):
-        self.deque: Deque = deque()
+    def __init__(self, config: dict, **kwargs) -> None:
+        self.deque: deque = deque()
         self.config = config
         for k, v in kwargs.items():
             self.__setattr__(k, v)
 
     def print(
         self,
         # вызов логгера без параметров выведет текущую дату
-        msg: str | datetime = datetime.now().strftime("%H:%M:%S"),
+        *msg: Sequence,
         frame=None,
         **kwargs,
     ) -> None:
         """Extension log."""
         try:
+            if msg and len(msg) == 1:
+                msg = msg[0]
+            elif not msg:
+                msg = msg or datetime.now().strftime("%H:%M:%S")
+
             if not (level := self.deque.pop()):  # noqa
                 return
 
             level_key = f"LOG_LEVEL_{level.upper()}_TPL"
             level_style = self.config.get(level_key, "").strip('"')
             if not level_style:
                 return
@@ -123,23 +128,24 @@
             frame = frame or inspect.currentframe().f_back
             len_file_name_section = 30
             file_name = kwargs.get("file_name", frame.f_code.co_filename)[-len_file_name_section:]
             line = kwargs.get("line", frame.f_lineno)
             divider = int(self.config.get("COLUMNS")) - len_file_name_section - 20
             title = kwargs.get("title", "-" * divider)
 
-            if isinstance(msg, (str, int, float, bool, type(decimal), type(None))):
+            if isinstance(msg, str | int | float | bool | type(decimal) | type(None)):
+                # if isinstance(msg, (str, int, float, bool, type(decimal), type(None))):
                 self.print_tbl(
                     message=msg,
                     file=file_name,
                     line=line,
                     level=level,
                     level_style=level_style,
                 )
-            elif isinstance(msg, (dict, tuple, list)):
+            elif isinstance(msg, (dict | tuple | list)):
                 # TODO add message for dict, tuple etc.
                 self.print_tbl(
                     message=title,
                     file=file_name,
                     line=line,
                     level=level,
                     level_style=level_style,
@@ -198,15 +204,15 @@
 
         table.add_row(stamp, msg, file_info)
 
         with console.capture() as capture:
             console_dict.print(table, markup=True)
         return capture.get()  # noqa WPS441
 
-    def __getattr__(self, *args, **kwargs):
+    def __getattr__(self, *args, **kwargs) -> Callable:
         """
         метод __getattr__ определяет поведение,
         когда наш атрибут, который мы пытаемся получить, не найден
         """
         name = args[0]
         if name.endswith(("style",)):
             return object.__getattribute__(self, name)  # noqa WPS609
```

### Comparing `logrich-1.0.4/logrich/config.py` & `logrich-1.0.5/logrich/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     LOG_LEVEL_RUN_TPL="[reverse yellow] RUN    [/]",
     LOG_LEVEL_GO_TPL="[reverse royal_blue1] GO     [/]",
     LOG_LEVEL_LIST_TPL="[reverse wheat4] LIST   [/]",
     LOG_LEVEL_DEBUG_TPL="[reverse #9f2844] DEBUG  [/]",
     LOG_LEVEL_SUCCESS_TPL="[reverse green] SUCCS  [/]",
     LOG_LEVEL_LOG_TPL="[reverse chartreuse4] LOG    [/]",
     LOG_LEVEL_TIME_TPL="[reverse spring_green4] TIME   [/]",
-    LOG_LEVEL_WARN_TPL="[reverse bright_red] WARN   [/]",
-    LOG_LEVEL_WARNING_TPL="[reverse bright_red] WARN   [/]",
+    LOG_LEVEL_WARN_TPL="[reverse yellow] WARN   [/]",
+    LOG_LEVEL_WARNING_TPL="[reverse yellow] WARN   [/]",
     LOG_LEVEL_FATAL_TPL="[reverse bright_red] FATAL  [/]",
     LOG_LEVEL_ERR_TPL="[reverse #ff5252] ERR    [/]",
     LOG_LEVEL_ERROR_TPL="[reverse #ff5252] ERROR  [/]",
 )
 
 config.update(
     **os.environ,  # override loaded values with environment variables
```

### Comparing `logrich-1.0.4/pyproject.toml` & `logrich-1.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "logrich"
-version = "1.0.4"
+version = "1.0.5"
 description = "loguru + rich = logrich"
 authors = ["Dmitry Mavlin <mavlind@list.ru>"]
 license = "GPL"
 readme = "README.md"
 keywords = ["logger", "loguru", "rich"]
 
 [project.urls]
@@ -13,36 +13,29 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 toml = "0.10.2"
 rich = "^12.4.4"
 importlib-metadata = "^5.2.0"
 python-dotenv = "^1.0.0"
+ruff = "^0.4.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "6.2.4"
 pytest-picked = "0.4.6"
 pytest-testmon = "1.1.1"
 pytest-watch = "4.2.0"
-black = "^22.1.0"
-pylint = "^2.12.2"
 mypy = "^0.961"
 pre-commit = "^2.19.0"
 watchdog = "^2.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 100
-include = '\.pyi?$'
-quiet = true
-fast = true
-
 [tool.mypy]
 strict = false
 ignore_missing_imports = true
 allow_subclassing_any = true
 allow_untyped_calls = true
 pretty = true
 show_error_codes = true
```

### Comparing `logrich-1.0.4/PKG-INFO` & `logrich-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logrich
-Version: 1.0.4
+Version: 1.0.5
 Summary: loguru + rich = logrich
 License: GPL
 Keywords: logger,loguru,rich
 Author: Dmitry Mavlin
 Author-email: mavlind@list.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: importlib-metadata (>=5.2.0,<6.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rich (>=12.4.4,<13.0.0)
+Requires-Dist: ruff (>=0.4.4,<0.5.0)
 Requires-Dist: toml (==0.10.2)
 Description-Content-Type: text/markdown
 
 ### Логгер
 
 #### Совместная работа [loguru](https://loguru.readthedocs.io) & [rich](https://rich.readthedocs.io).
```

