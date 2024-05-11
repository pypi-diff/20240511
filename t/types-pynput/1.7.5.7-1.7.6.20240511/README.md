# Comparing `tmp/types-pynput-1.7.5.7.tar.gz` & `tmp/types-pynput-1.7.6.20240511.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pynput-1.7.5.7.tar", last modified: Thu Jul 20 15:18:55 2023, max compression
+gzip compressed data, was "types-pynput-1.7.6.20240511.tar", last modified: Sat May 11 02:18:03 2024, max compression
```

## Comparing `types-pynput-1.7.5.7.tar` & `types-pynput-1.7.6.20240511.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:55.147114 types-pynput-1.7.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-20 15:18:54.000000 types-pynput-1.7.5.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:18:54.000000 types-pynput-1.7.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 15:18:55.143114 types-pynput-1.7.5.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:55.143114 types-pynput-1.7.5.7/pynput-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 15:18:54.000000 types-pynput-1.7.5.7/pynput-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/_util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:55.143114 types-pynput-1.7.5.7/pynput-stubs/keyboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/keyboard/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/keyboard/_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/keyboard/_dummy.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:55.143114 types-pynput-1.7.5.7/pynput-stubs/mouse/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/mouse/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/mouse/_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/mouse/_dummy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:55.147114 types-pynput-1.7.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-20 15:18:54.000000 types-pynput-1.7.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:55.143114 types-pynput-1.7.5.7/types_pynput.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 15:18:55.000000 types-pynput-1.7.5.7/types_pynput.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 15:18:55.000000 types-pynput-1.7.5.7/types_pynput.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:55.000000 types-pynput-1.7.5.7/types_pynput.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:18:55.000000 types-pynput-1.7.5.7/types_pynput.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:03.642156 types-pynput-1.7.6.20240511/
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-11 02:18:03.642156 types-pynput-1.7.6.20240511/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:03.638156 types-pynput-1.7.6.20240511/pynput-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/pynput-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/_util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:03.642156 types-pynput-1.7.6.20240511/pynput-stubs/keyboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/keyboard/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/keyboard/_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/keyboard/_dummy.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:03.642156 types-pynput-1.7.6.20240511/pynput-stubs/mouse/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/mouse/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/mouse/_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/mouse/_dummy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/pynput-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 02:18:03.642156 types-pynput-1.7.6.20240511/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:03.642156 types-pynput-1.7.6.20240511/types_pynput.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/types_pynput.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/types_pynput.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/types_pynput.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/types_pynput.egg-info/top_level.txt
```

### Comparing `types-pynput-1.7.5.7/PKG-INFO` & `types-pynput-1.7.6.20240511/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: types-pynput
-Version: 1.7.5.7
+Version: 1.7.6.20240511
 Summary: Typing stubs for pynput
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pynput.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for pynput
 
-This is a PEP 561 type stub package for the `pynput` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`pynput`](https://github.com/moses-palmer/pynput) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`pynput`. The source for this package can be found at
+`pynput`.
+
+This version of `types-pynput` aims to provide accurate annotations
+for `pynput==1.7.6`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pynput. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
+pytype 2024.4.11.
```

### Comparing `types-pynput-1.7.5.7/pynput-stubs/_util.pyi` & `types-pynput-1.7.6.20240511/pynput-stubs/_util.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import threading
 from collections.abc import Callable
 from queue import Queue
 from types import ModuleType, TracebackType
-from typing import Any, ClassVar, Generic, TypeVar
-from typing_extensions import ParamSpec, Self, TypedDict
+from typing import Any, ClassVar, Generic, TypedDict, TypeVar
+from typing_extensions import ParamSpec, Self
 
 _T = TypeVar("_T")
 _AbstractListener_T = TypeVar("_AbstractListener_T", bound=AbstractListener)
 _P = ParamSpec("_P")
 
 class _RESOLUTIONS(TypedDict):
     darwin: str
@@ -50,14 +50,15 @@
     def join(self, *args: Any) -> None: ...
 
 class Events(Generic[_T, _AbstractListener_T]):
     _Listener: type[_AbstractListener_T] | None  # undocumented
 
     class Event:
         def __eq__(self, other: object) -> bool: ...
+
     _event_queue: Queue[_T]  # undocumented
     _sentinel: object  # undocumented
     _listener: _AbstractListener_T  # undocumented
     start: Callable[[], None]
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     def __enter__(self) -> Self: ...
     def __exit__(
```

### Comparing `types-pynput-1.7.5.7/pynput-stubs/keyboard/__init__.pyi` & `types-pynput-1.7.6.20240511/pynput-stubs/keyboard/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pynput-1.7.5.7/pynput-stubs/keyboard/_base.pyi` & `types-pynput-1.7.6.20240511/pynput-stubs/keyboard/_base.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -21,79 +21,79 @@
     def from_vk(cls, vk: int, **kwargs: Any) -> Self: ...
     @classmethod
     def from_char(cls, char: str, **kwargs: Any) -> Self: ...
     @classmethod
     def from_dead(cls, char: str, **kwargs: Any) -> Self: ...
 
 class Key(enum.Enum):
-    alt: int
-    alt_l: int
-    alt_r: int
-    alt_gr: int
-    backspace: int
-    caps_lock: int
-    cmd: int
-    cmd_l: int
-    cmd_r: int
-    ctrl: int
-    ctrl_l: int
-    ctrl_r: int
-    delete: int
-    down: int
-    end: int
-    enter: int
-    esc: int
-    f1: int
-    f2: int
-    f3: int
-    f4: int
-    f5: int
-    f6: int
-    f7: int
-    f8: int
-    f9: int
-    f10: int
-    f11: int
-    f12: int
-    f13: int
-    f14: int
-    f15: int
-    f16: int
-    f17: int
-    f18: int
-    f19: int
-    f20: int
+    alt = 0
+    alt_l = alt
+    alt_r = alt
+    alt_gr = alt
+    backspace = alt
+    caps_lock = alt
+    cmd = alt
+    cmd_l = alt
+    cmd_r = alt
+    ctrl = alt
+    ctrl_l = alt
+    ctrl_r = alt
+    delete = alt
+    down = alt
+    end = alt
+    enter = alt
+    esc = alt
+    f1 = alt
+    f2 = alt
+    f3 = alt
+    f4 = alt
+    f5 = alt
+    f6 = alt
+    f7 = alt
+    f8 = alt
+    f9 = alt
+    f10 = alt
+    f11 = alt
+    f12 = alt
+    f13 = alt
+    f14 = alt
+    f15 = alt
+    f16 = alt
+    f17 = alt
+    f18 = alt
+    f19 = alt
+    f20 = alt
     if sys.platform == "win32":
-        f21: int
-        f22: int
-        f23: int
-        f24: int
-    home: int
-    left: int
-    page_down: int
-    page_up: int
-    right: int
-    shift: int
-    shift_l: int
-    shift_r: int
-    space: int
-    tab: int
-    up: int
-    media_play_pause: int
-    media_volume_mute: int
-    media_volume_down: int
-    media_volume_up: int
-    media_previous: int
-    media_next: int
-    insert: int
-    menu: int
-    num_lock: int
-    pause: int
-    print_screen: int
-    scroll_lock: int
+        f21 = alt
+        f22 = alt
+        f23 = alt
+        f24 = alt
+    home = alt
+    left = alt
+    page_down = alt
+    page_up = alt
+    right = alt
+    shift = alt
+    shift_l = alt
+    shift_r = alt
+    space = alt
+    tab = alt
+    up = alt
+    media_play_pause = alt
+    media_volume_mute = alt
+    media_volume_down = alt
+    media_volume_up = alt
+    media_previous = alt
+    media_next = alt
+    insert = alt
+    menu = alt
+    num_lock = alt
+    pause = alt
+    print_screen = alt
+    scroll_lock = alt
 
 class Controller:
     _KeyCode: ClassVar[type[KeyCode]]  # undocumented
     _Key: ClassVar[type[Key]]  # undocumented
 
     if sys.platform == "linux":
         CTRL_MASK: ClassVar[int]
```

### Comparing `types-pynput-1.7.5.7/pynput-stubs/mouse/__init__.pyi` & `types-pynput-1.7.6.20240511/pynput-stubs/mouse/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pynput-1.7.5.7/pynput-stubs/mouse/_base.pyi` & `types-pynput-1.7.6.20240511/pynput-stubs/mouse/_base.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -4,49 +4,49 @@
 from types import TracebackType
 from typing import Any
 from typing_extensions import Self
 
 from pynput._util import AbstractListener
 
 class Button(enum.Enum):
-    unknown: int
-    left: int
-    middle: int
-    right: int
+    unknown = 0
+    left = 1
+    middle = 2
+    right = 3
     if sys.platform == "linux":
-        button8: int
-        button9: int
-        button10: int
-        button11: int
-        button12: int
-        button13: int
-        button14: int
-        button15: int
-        button16: int
-        button17: int
-        button18: int
-        button19: int
-        button20: int
-        button21: int
-        button22: int
-        button23: int
-        button24: int
-        button25: int
-        button26: int
-        button27: int
-        button28: int
-        button29: int
-        button30: int
-        scroll_down: int
-        scroll_left: int
-        scroll_right: int
-        scroll_up: int
+        button8 = 8
+        button9 = 9
+        button10 = 10
+        button11 = 11
+        button12 = 12
+        button13 = 13
+        button14 = 14
+        button15 = 15
+        button16 = 16
+        button17 = 17
+        button18 = 18
+        button19 = 19
+        button20 = 20
+        button21 = 21
+        button22 = 22
+        button23 = 23
+        button24 = 24
+        button25 = 25
+        button26 = 26
+        button27 = 27
+        button28 = 28
+        button29 = 29
+        button30 = 30
+        scroll_down = 5
+        scroll_left = 6
+        scroll_right = 7
+        scroll_up = 4
     if sys.platform == "win32":
-        x1: int
-        x2: int
+        x1 = 0  # Value unknown
+        x2 = 0  # Value unknown
 
 class Controller:
     def __init__(self) -> None: ...
     @property
     def position(self) -> tuple[int, int]: ...
     @position.setter
     def position(self, position: tuple[int, int]) -> None: ...
```

### Comparing `types-pynput-1.7.5.7/setup.py` & `types-pynput-1.7.6.20240511/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 from setuptools import setup
 
 name = "types-pynput"
 description = "Typing stubs for pynput"
 long_description = '''
 ## Typing stubs for pynput
 
-This is a PEP 561 type stub package for the `pynput` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`pynput`](https://github.com/moses-palmer/pynput) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`pynput`. The source for this package can be found at
+`pynput`.
+
+This version of `types-pynput` aims to provide accurate annotations
+for `pynput==1.7.6`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pynput. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="1.7.5.7",
+      version="1.7.6.20240511",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pynput.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['pynput-stubs'],
-      package_data={'pynput-stubs': ['__init__.pyi', '_info.pyi', '_util.pyi', 'keyboard/__init__.pyi', 'keyboard/_base.pyi', 'keyboard/_dummy.pyi', 'mouse/__init__.pyi', 'mouse/_base.pyi', 'mouse/_dummy.pyi', 'METADATA.toml']},
+      package_data={'pynput-stubs': ['__init__.pyi', '_info.pyi', '_util.pyi', 'keyboard/__init__.pyi', 'keyboard/_base.pyi', 'keyboard/_dummy.pyi', 'mouse/__init__.pyi', 'mouse/_base.pyi', 'mouse/_dummy.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
+      python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-pynput-1.7.5.7/types_pynput.egg-info/PKG-INFO` & `types-pynput-1.7.6.20240511/types_pynput.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
 Name: types-pynput
-Version: 1.7.5.7
+Version: 1.7.6.20240511
 Summary: Typing stubs for pynput
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pynput.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for pynput
 
-This is a PEP 561 type stub package for the `pynput` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`pynput`](https://github.com/moses-palmer/pynput) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`pynput`. The source for this package can be found at
+`pynput`.
+
+This version of `types-pynput` aims to provide accurate annotations
+for `pynput==1.7.6`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pynput. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
+pytype 2024.4.11.
```

