# Comparing `tmp/picodi-0.5.0.tar.gz` & `tmp/picodi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picodi-0.5.0.tar", max compression
+gzip compressed data, was "picodi-0.6.0.tar", max compression
```

## Comparing `picodi-0.5.0.tar` & `picodi-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1064 2024-05-09 12:30:57.572187 picodi-0.5.0/LICENSE
--rw-r--r--   0        0        0     6904 2024-05-09 12:30:57.572187 picodi-0.5.0/README.md
--rw-r--r--   0        0        0      265 2024-05-09 12:30:57.572187 picodi-0.5.0/picodi/__init__.py
--rw-r--r--   0        0        0     9882 2024-05-09 12:30:57.572187 picodi-0.5.0/picodi/picodi.py
--rw-r--r--   0        0        0        0 2024-05-09 12:30:57.572187 picodi-0.5.0/picodi/py.typed
--rw-r--r--   0        0        0     2973 2024-05-09 12:30:57.572187 picodi-0.5.0/picodi/scopes.py
--rw-r--r--   0        0        0     2604 2024-05-09 12:30:57.572187 picodi-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7666 1970-01-01 00:00:00.000000 picodi-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-11 14:33:47.444728 picodi-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7352 2024-05-11 14:33:47.444728 picodi-0.6.0/README.md
+-rw-r--r--   0        0        0      266 2024-05-11 14:33:47.444728 picodi-0.6.0/picodi/__init__.py
+-rw-r--r--   0        0        0     2005 2024-05-11 14:33:47.444728 picodi-0.6.0/picodi/_internal.py
+-rw-r--r--   0        0        0    10133 2024-05-11 14:33:47.444728 picodi-0.6.0/picodi/_picodi.py
+-rw-r--r--   0        0        0     1284 2024-05-11 14:33:47.444728 picodi-0.6.0/picodi/_scopes.py
+-rw-r--r--   0        0        0     1649 2024-05-11 14:33:47.444728 picodi-0.6.0/picodi/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:33:47.444728 picodi-0.6.0/picodi/py.typed
+-rw-r--r--   0        0        0     2604 2024-05-11 14:33:47.448727 picodi-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8114 1970-01-01 00:00:00.000000 picodi-0.6.0/PKG-INFO
```

### Comparing `picodi-0.5.0/LICENSE` & `picodi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picodi-0.5.0/README.md` & `picodi-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -271,14 +271,28 @@
 ### `shutdown_resources()`
 
 Cleans up all resources.
 It should be called when the application is shutting down to ensure proper resource cleanup.
 
 Can be called as `shutdown_resources()` in sync context and `await shutdown_resources()` in async context.
 
+### `helpers` module
+
+Module with helper functions for working with dependencies.
+
+#### `helpers.get_value(path, obj, default)`
+
+Function to get a value from a nested dictionary or object.
+Can deal with dictionary keys as well as object attributes.
+
+- **Parameters**:
+  - `path`: A string with keys separated by dots.
+  - `obj`: A dictionary or object from which to get the value.
+  - `default`: A default value to return if the key is not found.
+
 ## License
 
 [MIT](https://github.com/yakimka/picodi/blob/main/LICENSE)
 
 
 ## Credits
```

### Comparing `picodi-0.5.0/picodi/picodi.py` & `picodi-0.6.0/picodi/_picodi.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     AsyncContextManager,
     ContextManager,
     ParamSpec,
     TypeVar,
     cast,
 )
 
-from picodi.scopes import GlobalScope, NullScope, Scope, SingletonScope
+from picodi._internal import DummyAwaitable
+from picodi._scopes import GlobalScope, NullScope, Scope, SingletonScope
 
 if TYPE_CHECKING:
     from inspect import BoundArguments, Signature
 
 DependencyCallable = Callable[..., Any]
 T = TypeVar("T")
 P = ParamSpec("P")
@@ -99,15 +100,17 @@
             result_or_gen = fn(*bound.args, **bound.kwargs)
             if inspect.isasyncgen(result_or_gen):
                 result = result_or_gen
             else:
                 result = await result_or_gen  # type: ignore[misc]
 
             for scope in _scopes.values():
-                await scope.close_local()
+                coro = scope.close_local()
+                if coro is not None:
+                    await coro
             return cast("T", result)
 
     else:
 
         @functools.wraps(fn)
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
             bound, dep_arguments = _arguments_to_getters(
@@ -154,23 +157,29 @@
     for provider in _registry.values():
         if provider.in_use and issubclass(provider.scope_class, GlobalScope):
             if provider.is_async:
                 async_resources.append(_resolve_value_async(provider))
             else:
                 _resolve_value(provider)
 
-    return asyncio.gather(*async_resources)
+    if async_resources:
+        return asyncio.gather(*async_resources)
+    return DummyAwaitable()
 
 
 def shutdown_resources() -> Awaitable:
     """
     Call this function to close all resources. Usually, it should be called
     when your application is shut down.
     """
-    tasks = [scope.close_global() for scope in _scopes.values()]
+    tasks = []
+    for scope in _scopes.values():
+        coro = scope.close_global()
+        if coro is not None:
+            tasks.append(coro)
     return asyncio.gather(*tasks)
 
 
 def make_dependency(fn: Callable[P, T], *args: Any, **kwargs: Any) -> Callable[..., T]:
     signature = inspect.signature(fn)
     bound = signature.bind(*args, **kwargs)
     bound.apply_defaults()
```

### Comparing `picodi-0.5.0/picodi/scopes.py` & `picodi-0.6.0/picodi/_internal.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,63 +2,22 @@
 
 import asyncio
 from contextlib import AsyncExitStack
 from contextlib import ExitStack as SyncExitStack
 from typing import TYPE_CHECKING, Any, AsyncContextManager, ContextManager
 
 if TYPE_CHECKING:
-    from collections.abc import Awaitable, Hashable
+    from collections.abc import Awaitable, Generator
     from types import TracebackType
 
 
-class Scope:
-    def __init__(self) -> None:
-        self.exit_stack = ExitStack()
-
-    def get(self, key: Hashable) -> Any:
-        raise NotImplementedError
-
-    def set(self, key: Hashable, value: Any) -> None:
-        raise NotImplementedError
-
-    def close_local(self) -> Awaitable:
-        return asyncio.sleep(0)
-
-    def close_global(self) -> Awaitable:
-        return asyncio.sleep(0)
-
-
-class GlobalScope(Scope):
-    def close_global(self) -> Awaitable:
-        return self.exit_stack.close()
-
-
-class LocalScope(Scope):
-    def close_local(self) -> Awaitable:
-        return self.exit_stack.close()
-
-
-class NullScope(LocalScope):
-    def get(self, key: Hashable) -> Any:
-        raise KeyError(key)
-
-    def set(self, key: Hashable, value: Any) -> None:
-        pass
-
-
-class SingletonScope(GlobalScope):
-    def __init__(self) -> None:
-        super().__init__()
-        self._store: dict[Hashable, Any] = {}
-
-    def get(self, key: Hashable) -> Any:
-        return self._store[key]
-
-    def set(self, key: Hashable, value: Any) -> None:
-        self._store[key] = value
+class DummyAwaitable:
+    def __await__(self) -> Generator[None, None, None]:
+        yield
+        return None
 
 
 class ExitStack:
     def __init__(self) -> None:
         self._sync_stack = SyncExitStack()
         self._async_stack = AsyncExitStack()
 
@@ -94,15 +53,15 @@
 
         raise TypeError(f"Unsupported context manager: {cm}")
 
     def close(self) -> Awaitable:
         self.__exit__(None, None, None)
         if is_async_environment():
             return self.__aexit__(None, None, None)
-        return asyncio.sleep(0)
+        return DummyAwaitable()
 
 
 def is_async_environment() -> bool:
     try:
         asyncio.get_running_loop()
     except RuntimeError:
         return False
```

### Comparing `picodi-0.5.0/pyproject.toml` & `picodi-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "picodi"
 description = "Simple Dependency Injection for Python"
-version = "0.5.0"
+version = "0.6.0"
 license = "MIT"
 authors = [
   "yakimka"
 ]
 
 readme = "README.md"
```

### Comparing `picodi-0.5.0/PKG-INFO` & `picodi-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picodi
-Version: 0.5.0
+Version: 0.6.0
 Summary: Simple Dependency Injection for Python
 Home-page: https://github.com/yakimka/picodi
 License: MIT
 Author: yakimka
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -291,14 +291,28 @@
 ### `shutdown_resources()`
 
 Cleans up all resources.
 It should be called when the application is shutting down to ensure proper resource cleanup.
 
 Can be called as `shutdown_resources()` in sync context and `await shutdown_resources()` in async context.
 
+### `helpers` module
+
+Module with helper functions for working with dependencies.
+
+#### `helpers.get_value(path, obj, default)`
+
+Function to get a value from a nested dictionary or object.
+Can deal with dictionary keys as well as object attributes.
+
+- **Parameters**:
+  - `path`: A string with keys separated by dots.
+  - `obj`: A dictionary or object from which to get the value.
+  - `default`: A default value to return if the key is not found.
+
 ## License
 
 [MIT](https://github.com/yakimka/picodi/blob/main/LICENSE)
 
 
 ## Credits
```

