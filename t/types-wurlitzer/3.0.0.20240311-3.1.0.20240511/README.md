# Comparing `tmp/types-wurlitzer-3.0.0.20240311.tar.gz` & `tmp/types-wurlitzer-3.1.0.20240511.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-wurlitzer-3.0.0.20240311.tar", last modified: Mon Mar 11 02:16:53 2024, max compression
+gzip compressed data, was "types-wurlitzer-3.1.0.20240511.tar", last modified: Sat May 11 02:17:59 2024, max compression
```

## Comparing `types-wurlitzer-3.0.0.20240311.tar` & `types-wurlitzer-3.1.0.20240511.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:16:53.269317 types-wurlitzer-3.0.0.20240311/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-11 02:16:52.000000 types-wurlitzer-3.0.0.20240311/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 02:16:52.000000 types-wurlitzer-3.0.0.20240311/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-11 02:16:53.269317 types-wurlitzer-3.0.0.20240311/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 02:16:53.269317 types-wurlitzer-3.0.0.20240311/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-11 02:16:52.000000 types-wurlitzer-3.0.0.20240311/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:16:53.269317 types-wurlitzer-3.0.0.20240311/types_wurlitzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-11 02:16:53.000000 types-wurlitzer-3.0.0.20240311/types_wurlitzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-11 02:16:53.000000 types-wurlitzer-3.0.0.20240311/types_wurlitzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 02:16:53.000000 types-wurlitzer-3.0.0.20240311/types_wurlitzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-11 02:16:53.000000 types-wurlitzer-3.0.0.20240311/types_wurlitzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:16:53.269317 types-wurlitzer-3.0.0.20240311/wurlitzer-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-11 02:16:52.000000 types-wurlitzer-3.0.0.20240311/wurlitzer-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-11 02:16:52.000000 types-wurlitzer-3.0.0.20240311/wurlitzer-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:59.594139 types-wurlitzer-3.1.0.20240511/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-11 02:17:59.000000 types-wurlitzer-3.1.0.20240511/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 02:17:59.000000 types-wurlitzer-3.1.0.20240511/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-11 02:17:59.594139 types-wurlitzer-3.1.0.20240511/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 02:17:59.594139 types-wurlitzer-3.1.0.20240511/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-11 02:17:59.000000 types-wurlitzer-3.1.0.20240511/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:59.590139 types-wurlitzer-3.1.0.20240511/types_wurlitzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-11 02:17:59.000000 types-wurlitzer-3.1.0.20240511/types_wurlitzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-11 02:17:59.000000 types-wurlitzer-3.1.0.20240511/types_wurlitzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:17:59.000000 types-wurlitzer-3.1.0.20240511/types_wurlitzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 02:17:59.000000 types-wurlitzer-3.1.0.20240511/types_wurlitzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:59.594139 types-wurlitzer-3.1.0.20240511/wurlitzer-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-11 02:17:59.000000 types-wurlitzer-3.1.0.20240511/wurlitzer-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-11 02:17:59.000000 types-wurlitzer-3.1.0.20240511/wurlitzer-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:59.000000 types-wurlitzer-3.1.0.20240511/wurlitzer-stubs/py.typed
```

### Comparing `types-wurlitzer-3.0.0.20240311/PKG-INFO` & `types-wurlitzer-3.1.0.20240511/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-wurlitzer
-Version: 3.0.0.20240311
+Version: 3.1.0.20240511
 Summary: Typing stubs for wurlitzer
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/wurlitzer.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `wurlitzer`.
 
 This version of `types-wurlitzer` aims to provide accurate annotations
-for `wurlitzer==3.0.*`.
+for `wurlitzer==3.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/wurlitzer. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
+pytype 2024.4.11.
```

### Comparing `types-wurlitzer-3.0.0.20240311/setup.py` & `types-wurlitzer-3.1.0.20240511/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `wurlitzer`.
 
 This version of `types-wurlitzer` aims to provide accurate annotations
-for `wurlitzer==3.0.*`.
+for `wurlitzer==3.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/wurlitzer. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="3.0.0.20240311",
+      version="3.1.0.20240511",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/wurlitzer.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['wurlitzer-stubs'],
-      package_data={'wurlitzer-stubs': ['__init__.pyi', 'METADATA.toml']},
+      package_data={'wurlitzer-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-wurlitzer-3.0.0.20240311/types_wurlitzer.egg-info/PKG-INFO` & `types-wurlitzer-3.1.0.20240511/types_wurlitzer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-wurlitzer
-Version: 3.0.0.20240311
+Version: 3.1.0.20240511
 Summary: Typing stubs for wurlitzer
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/wurlitzer.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `wurlitzer`.
 
 This version of `types-wurlitzer` aims to provide accurate annotations
-for `wurlitzer==3.0.*`.
+for `wurlitzer==3.1.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/wurlitzer. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+with mypy 1.10.0, pyright 1.1.362, and
+pytype 2024.4.11.
```

### Comparing `types-wurlitzer-3.0.0.20240311/wurlitzer-stubs/__init__.pyi` & `types-wurlitzer-3.1.0.20240511/wurlitzer-stubs/__init__.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 __all__ = ["STDOUT", "PIPE", "Wurlitzer", "pipes", "sys_pipes", "sys_pipes_forever", "stop_sys_pipes"]
 
 import contextlib
 import io
+import logging
 from _typeshed import SupportsWrite
 from contextlib import _GeneratorContextManager
 from types import TracebackType
 from typing import Any, Final, Literal, Protocol, TextIO, TypeVar, overload
-from typing_extensions import TypeAlias
+from typing_extensions import Self, TypeAlias
 
 STDOUT: Final = 2
 PIPE: Final = 3
 _STDOUT: TypeAlias = Literal[2]
 _PIPE: TypeAlias = Literal[3]
 _T_contra = TypeVar("_T_contra", contravariant=True)
 _StreamOutT = TypeVar("_StreamOutT", bound=_Stream[str] | _Stream[bytes])
@@ -27,16 +28,16 @@
 
 class Wurlitzer:
     flush_interval: float
     encoding: str | None
 
     def __init__(
         self,
-        stdout: SupportsWrite[str] | SupportsWrite[bytes] | None = None,
-        stderr: _STDOUT | SupportsWrite[str] | SupportsWrite[bytes] | None = None,
+        stdout: SupportsWrite[str] | SupportsWrite[bytes] | logging.Logger | None = None,
+        stderr: _STDOUT | SupportsWrite[str] | SupportsWrite[bytes] | logging.Logger | None = None,
         encoding: str | None = ...,
         bufsize: int | None = ...,
     ) -> None: ...
     def __enter__(self): ...
     def __exit__(
         self, exc_type: type[BaseException] | None, exc_value: BaseException | None, traceback: TracebackType | None
     ) -> None: ...
@@ -67,14 +68,38 @@
 ) -> _GeneratorContextManager[tuple[io.StringIO, io.StringIO]]: ...
 @overload
 def pipes(
     stdout: _PIPE, stderr: _StreamErrT, encoding: str = ..., bufsize: int | None = None
 ) -> _GeneratorContextManager[tuple[io.StringIO, _StreamErrT]]: ...
 @overload
 def pipes(
+    stdout: _PIPE, stderr: logging.Logger, encoding: str = ..., bufsize: int | None = None
+) -> _GeneratorContextManager[tuple[io.StringIO, _LogPipe]]: ...
+@overload
+def pipes(
+    stdout: logging.Logger, stderr: _STDOUT, encoding: str | None = ..., bufsize: int | None = None
+) -> _GeneratorContextManager[tuple[_LogPipe, None]]: ...
+@overload
+def pipes(
+    stdout: logging.Logger, stderr: _PIPE, encoding: None, bufsize: int | None = None
+) -> _GeneratorContextManager[tuple[_LogPipe, io.BytesIO]]: ...
+@overload
+def pipes(
+    stdout: logging.Logger, stderr: _PIPE, encoding: str = ..., bufsize: int | None = None
+) -> _GeneratorContextManager[tuple[_LogPipe, io.StringIO]]: ...
+@overload
+def pipes(
+    stdout: logging.Logger, stderr: _StreamErrT, encoding: str | None = ..., bufsize: int | None = None
+) -> _GeneratorContextManager[tuple[_LogPipe, _StreamErrT]]: ...
+@overload
+def pipes(
+    stdout: logging.Logger, stderr: logging.Logger, encoding: str | None = ..., bufsize: int | None = None
+) -> _GeneratorContextManager[tuple[_LogPipe, _LogPipe]]: ...
+@overload
+def pipes(
     stdout: _StreamOutT, stderr: _STDOUT, encoding: str | None = ..., bufsize: int | None = None
 ) -> _GeneratorContextManager[tuple[_StreamOutT, None]]: ...
 @overload
 def pipes(
     stdout: _StreamOutT, stderr: _PIPE, encoding: None, bufsize: int | None = None
 ) -> _GeneratorContextManager[tuple[_StreamOutT, io.BytesIO]]: ...
 @overload
@@ -83,16 +108,33 @@
 ) -> _GeneratorContextManager[tuple[_StreamOutT, io.StringIO]]: ...
 @overload
 def pipes(
     stdout: _StreamOutT, stderr: _StreamErrT, encoding: str | None = ..., bufsize: int | None = None
 ) -> _GeneratorContextManager[tuple[_StreamOutT, _StreamErrT]]: ...
 @overload
 def pipes(
-    stdout: _PIPE | _StreamOutT = 3,
-    stderr: _STDOUT | _PIPE | _StreamErrT = 3,
+    stdout: _StreamOutT, stderr: logging.Logger, encoding: str | None = ..., bufsize: int | None = None
+) -> _GeneratorContextManager[tuple[_StreamOutT, _LogPipe]]: ...
+@overload
+def pipes(
+    stdout: _PIPE | logging.Logger | _StreamOutT = 3,
+    stderr: _STDOUT | _PIPE | logging.Logger | _StreamErrT = 3,
     encoding: str | None = ...,
     bufsize: int | None = None,
-) -> _GeneratorContextManager[tuple[io.BytesIO | io.StringIO | _StreamOutT, io.BytesIO | io.StringIO | _StreamErrT | None]]: ...
+) -> _GeneratorContextManager[
+    tuple[io.BytesIO | io.StringIO | _StreamOutT | _LogPipe, io.BytesIO | io.StringIO | _StreamErrT | _LogPipe | None]
+]: ...
+
+class _LogPipe(io.BufferedWriter):
+    logger: logging.Logger
+    stream_name: str
+    level: int
+    def __init__(self, logger: logging.Logger, stream_name: str, level: int = 20) -> None: ...
+    def write(self, chunk: str) -> None: ...  # type: ignore[override]
+    def flush(self) -> None: ...
+    def __enter__(self) -> Self: ...
+    def __exit__(self, *exc_info: object) -> None: ...
+
 def sys_pipes_forever(encoding: str = ..., bufsize: int | None = None) -> None: ...
 def stop_sys_pipes() -> None: ...
 def load_ipython_extension(ip: _InteractiveShell) -> None: ...
 def unload_ipython_extension(ip: _InteractiveShell) -> None: ...
```

