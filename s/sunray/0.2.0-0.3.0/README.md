# Comparing `tmp/sunray-0.2.0-py3-none-any.whl.zip` & `tmp/sunray-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,18 @@
-Zip file size: 17801 bytes, number of entries: 12
+Zip file size: 21932 bytes, number of entries: 16
 -rw-r--r--  2.0 unx     2272 b- defN 80-Jan-01 00:00 sunray/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 sunray/_internal/__init__.py
--rw-r--r--  2.0 unx    23109 b- defN 80-Jan-01 00:00 sunray/_internal/actor_mixin.py
--rw-r--r--  2.0 unx    14899 b- defN 80-Jan-01 00:00 sunray/_internal/core.py
--rw-r--r--  2.0 unx     9677 b- defN 80-Jan-01 00:00 sunray/_internal/remote.py
--rw-r--r--  2.0 unx    18265 b- defN 80-Jan-01 00:00 sunray/_internal/typing.py
+-rw-r--r--  2.0 unx    25396 b- defN 80-Jan-01 00:00 sunray/_internal/actor_mixin.py
+-rw-r--r--  2.0 unx    65315 b- defN 80-Jan-01 00:00 sunray/_internal/callable.py
+-rw-r--r--  2.0 unx    15322 b- defN 80-Jan-01 00:00 sunray/_internal/core.py
+-rw-r--r--  2.0 unx    10468 b- defN 80-Jan-01 00:00 sunray/_internal/dag.py
+-rw-r--r--  2.0 unx      658 b- defN 80-Jan-01 00:00 sunray/_internal/io.py
+-rw-r--r--  2.0 unx    11074 b- defN 80-Jan-01 00:00 sunray/_internal/remote.py
+-rw-r--r--  2.0 unx    11210 b- defN 80-Jan-01 00:00 sunray/_internal/typing.py
 -rw-r--r--  2.0 unx      807 b- defN 80-Jan-01 00:00 sunray/_internal/util.py
+-rw-r--r--  2.0 unx      430 b- defN 80-Jan-01 00:00 sunray/dag.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 sunray/py.typed
--rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 sunray-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     8155 b- defN 80-Jan-01 00:00 sunray-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sunray-0.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      934 b- defN 16-Jan-01 00:00 sunray-0.2.0.dist-info/RECORD
-12 files, 79274 bytes uncompressed, 16247 bytes compressed:  79.5%
+-rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 sunray-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8833 b- defN 80-Jan-01 00:00 sunray-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sunray-0.3.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1249 b- defN 16-Jan-01 00:00 sunray-0.3.0.dist-info/RECORD
+16 files, 154190 bytes uncompressed, 19902 bytes compressed:  87.1%
```

## zipnote {}

```diff
@@ -3,35 +3,47 @@
 
 Filename: sunray/_internal/__init__.py
 Comment: 
 
 Filename: sunray/_internal/actor_mixin.py
 Comment: 
 
+Filename: sunray/_internal/callable.py
+Comment: 
+
 Filename: sunray/_internal/core.py
 Comment: 
 
+Filename: sunray/_internal/dag.py
+Comment: 
+
+Filename: sunray/_internal/io.py
+Comment: 
+
 Filename: sunray/_internal/remote.py
 Comment: 
 
 Filename: sunray/_internal/typing.py
 Comment: 
 
 Filename: sunray/_internal/util.py
 Comment: 
 
+Filename: sunray/dag.py
+Comment: 
+
 Filename: sunray/py.typed
 Comment: 
 
-Filename: sunray-0.2.0.dist-info/LICENSE
+Filename: sunray-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: sunray-0.2.0.dist-info/METADATA
+Filename: sunray-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: sunray-0.2.0.dist-info/WHEEL
+Filename: sunray-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: sunray-0.2.0.dist-info/RECORD
+Filename: sunray-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sunray/__init__.py

```diff
@@ -1,12 +1,12 @@
 # ruff: noqa: E402, F401
 from __future__ import annotations
 
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 __authors__ = [
     "ZhengYu, Xu <zen-xu@outlook.com>",
 ]
 
 # re-exports from ray
 from ray._private.worker import LOCAL_MODE as LOCAL_MODE
 from ray._private.worker import RESTORE_WORKER_MODE as RESTORE_WORKER_MODE
```

## sunray/_internal/actor_mixin.py

```diff
@@ -8,14 +8,15 @@
 from typing import TypeVar
 from typing import overload
 
 import ray
 
 from typing_extensions import ParamSpec
 
+from . import io
 from .util import get_num_returns
 
 
 if TYPE_CHECKING:
     from typing import AsyncGenerator
     from typing import Awaitable
     from typing import Callable
@@ -24,23 +25,26 @@
     from ray.actor import ActorHandle
     from ray.actor import ActorMethod
     from typing_extensions import Concatenate
     from typing_extensions import Literal
     from typing_extensions import TypedDict
     from typing_extensions import Unpack
 
+    from .callable import ClassBindCallable
+    from .callable import ClassMethodBindCallable
+    from .callable import ClassStreamBindCallable
+    from .callable import RemoteCallable
     from .core import ObjectRef
     from .core import ObjectRefGenerator
     from .typing import ActorRemoteOptions
-    from .typing import RemoteCallable
 
 
 _Ret = TypeVar("_Ret")
 _YieldItem = TypeVar("_YieldItem")
-_RemoteRet = TypeVar("_RemoteRet")
+_RemoteRet = TypeVar("_RemoteRet", bound=io.Out)
 _ClassT = TypeVar("_ClassT")
 _P = ParamSpec("_P")
 _R0 = TypeVar("_R0")
 _R1 = TypeVar("_R1")
 _R2 = TypeVar("_R2")
 _R3 = TypeVar("_R3")
 _R4 = TypeVar("_R4")
@@ -74,52 +78,64 @@
 
 class ActorClass(Generic[_P, _ClassT]):
     def __init__(self, klass: Callable[_P, _ClassT], default_opts: ActorRemoteOptions):
         self._klass = add_var_keyword_to_klass(klass)
         self._default_opts = default_opts
 
     if TYPE_CHECKING:
-        remote: RemoteCallable[Callable[_P, _ClassT], Actor[_ClassT]]
+        remote: RemoteCallable[Callable[_P, _ClassT], io.Out[Actor[_ClassT]]]
+        bind: ClassBindCallable[Callable[_P, _ClassT], io.Actor[_ClassT]]
     else:
 
         def remote(self, *args, **kwargs):
             remote_cls = (
                 ray.remote(**self._default_opts)(self._klass)
                 if self._default_opts
                 else ray.remote(self._klass)
             )
             handle = remote_cls.remote(*args, **kwargs)
 
             return Actor(handle)
 
+        def bind(self, *args, **kwargs):
+            from .dag import ClassNode
+
+            return ClassNode(self._klass, args, kwargs, self._default_opts)
+
     def options(
         self, **opts: Unpack[ActorRemoteOptions]
     ) -> ActorClassWrapper[_P, _ClassT]:
         opts = {**self._default_opts, **opts}
         return ActorClassWrapper(self._klass, opts)
 
 
 class ActorClassWrapper(Generic[_P, _ClassT]):
     def __init__(self, klass: Callable[_P, _ClassT], opts: ActorRemoteOptions):
         self._klass = add_var_keyword_to_klass(klass)
         self._opts = opts
 
     if TYPE_CHECKING:
-        remote: RemoteCallable[Callable[_P, _ClassT], Actor[_ClassT]]
+        remote: RemoteCallable[Callable[_P, _ClassT], io.Out[Actor[_ClassT]]]
+        bind: ClassBindCallable[Callable[_P, _ClassT], io.Actor[_ClassT]]
     else:
 
         def remote(self, *args, **kwargs):
             remote_cls = (
                 ray.remote(**self._opts)(self._klass)
                 if self._opts
                 else ray.remote(self._klass)
             )
             handle = remote_cls.remote(*args, **kwargs)
             return Actor(handle)
 
+        def bind(self, *args, **kwargs):
+            from .dag import ClassNode
+
+            return ClassNode(self._klass, args, kwargs, self._opts)
+
 
 class ActorHandleProxy:
     def __init__(self, actor_handle: ActorHandle) -> None:
         self.actor_handle = actor_handle
 
     def __getattr__(self, k):
         method = getattr(self.actor_handle, k)
@@ -138,14 +154,17 @@
 
     def options(self, *, unpack: bool = False, **options):
         if self.actor_method._num_returns != "streaming" and not unpack:
             options["num_returns"] = 1
 
         return self.actor_method.options(**options)
 
+    def bind(self, *args, **kwargs):
+        return self.actor_method.bind(*args, **kwargs)
+
 
 class Actor(Generic[_ClassT]):
     def __init__(self, actor_handle: ActorHandle):
         self._actor_handle = actor_handle
 
     @property
     def methods(self) -> type[_ClassT]:  # pragma: no cover
@@ -173,388 +192,423 @@
         concurrency_group: str
         max_task_retries: int
         retry_exceptions: bool | list[type[Exception]]
         enable_task_events: bool
         _generator_backpressure_num_objects: Any
 
     class Method(Generic[_P, _Ret]):
-        remote: RemoteCallable[Callable[_P, _Ret], ObjectRef[_Ret]]
+        remote: RemoteCallable[Callable[_P, _Ret], io.Out[ObjectRef[_Ret]]]
+        bind: ClassMethodBindCallable[Callable[_P, _Ret], io.Out[ObjectRef[_Ret]]]
 
         @overload
         def options(
             self,
             *,
             unpack: Literal[False] = False,
             **options: Unpack[MethodOptions],
-        ) -> MethodWrapper[_P, _Ret, ObjectRef[_Ret]]: ...
+        ) -> MethodWrapper[_P, _Ret, io.Out[ObjectRef[_Ret]]]: ...
 
         @overload
         def options(
             self: Method[_P, tuple[_R0]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
-        ) -> MethodWrapper[_P, _Ret, tuple[ObjectRef[_R0]]]: ...
+        ) -> MethodWrapper[_P, _Ret, io.Out[tuple[ObjectRef[_R0]]]]: ...
 
         @overload
         def options(
             self: Method[_P, tuple[_R0, _R1]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
-        ) -> MethodWrapper[_P, _Ret, tuple[ObjectRef[_R0], ObjectRef[_R1]]]: ...
+        ) -> MethodWrapper[_P, _Ret, io.Out[tuple[ObjectRef[_R0], ObjectRef[_R1]]]]: ...
 
         @overload
         def options(
             self: Method[_P, tuple[_R0, _R1, _R2]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
-            _P, _Ret, tuple[ObjectRef[_R0], ObjectRef[_R1], ObjectRef[_R2]]
+            _P, _Ret, io.Out[tuple[ObjectRef[_R0], ObjectRef[_R1], ObjectRef[_R2]]]
         ]: ...
 
         @overload
         def options(
             self: Method[_P, tuple[_R0, _R1, _R2, _R3]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             _Ret,
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                ]
             ],
         ]: ...
 
         @overload
         def options(
             self: Method[_P, tuple[_R0, _R1, _R2, _R3, _R4]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             _Ret,
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
-                ObjectRef[_R4],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                    ObjectRef[_R4],
+                ]
             ],
         ]: ...
 
         @overload
         def options(
             self: Method[_P, tuple[_R0, _R1, _R2, _R3, _R4, _R5]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             _Ret,
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
-                ObjectRef[_R4],
-                ObjectRef[_R5],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                    ObjectRef[_R4],
+                    ObjectRef[_R5],
+                ]
             ],
         ]: ...
 
         @overload
         def options(
             self: Method[_P, tuple[_R0, _R1, _R2, _R3, _R4, _R5, _R6]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             _Ret,
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
-                ObjectRef[_R4],
-                ObjectRef[_R5],
-                ObjectRef[_R6],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                    ObjectRef[_R4],
+                    ObjectRef[_R5],
+                    ObjectRef[_R6],
+                ]
             ],
         ]: ...
 
         @overload
         def options(
             self: Method[_P, tuple[_R0, _R1, _R2, _R3, _R4, _R5, _R6, _R7]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             _Ret,
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
-                ObjectRef[_R4],
-                ObjectRef[_R5],
-                ObjectRef[_R6],
-                ObjectRef[_R7],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                    ObjectRef[_R4],
+                    ObjectRef[_R5],
+                    ObjectRef[_R6],
+                    ObjectRef[_R7],
+                ]
             ],
         ]: ...
 
         @overload
         def options(
             self: Method[_P, tuple[_R0, _R1, _R2, _R3, _R4, _R5, _R6, _R7, _R8]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             _Ret,
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
-                ObjectRef[_R4],
-                ObjectRef[_R5],
-                ObjectRef[_R6],
-                ObjectRef[_R7],
-                ObjectRef[_R8],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                    ObjectRef[_R4],
+                    ObjectRef[_R5],
+                    ObjectRef[_R6],
+                    ObjectRef[_R7],
+                    ObjectRef[_R8],
+                ]
             ],
         ]: ...
 
         @overload
         def options(
             self: Method[_P, tuple[_R0, _R1, _R2, _R3, _R4, _R5, _R6, _R7, _R8, _R9]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             _Ret,
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
-                ObjectRef[_R4],
-                ObjectRef[_R5],
-                ObjectRef[_R6],
-                ObjectRef[_R7],
-                ObjectRef[_R8],
-                ObjectRef[_R9],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                    ObjectRef[_R4],
+                    ObjectRef[_R5],
+                    ObjectRef[_R6],
+                    ObjectRef[_R7],
+                    ObjectRef[_R8],
+                    ObjectRef[_R9],
+                ]
             ],
         ]: ...
 
         def options(
             self, *, unpack: bool = False, **options: Unpack[MethodOptions]
         ) -> MethodWrapper: ...
 
         def __call__(self, *args: _P.args, **kwds: _P.kwargs) -> _Ret: ...
 
     class AsyncMethod(Generic[_P, _Ret]):
-        remote: RemoteCallable[Callable[_P, Awaitable[_Ret]], ObjectRef[_Ret]]
+        remote: RemoteCallable[Callable[_P, Awaitable[_Ret]], io.Out[ObjectRef[_Ret]]]
+        bind: ClassMethodBindCallable[
+            Callable[_P, Awaitable[_Ret]], io.Out[ObjectRef[_Ret]]
+        ]
 
         @overload
         def options(
             self, *, unpack: Literal[False] = False, **options: Unpack[MethodOptions]
-        ) -> MethodWrapper[_P, Awaitable[_Ret], ObjectRef[_Ret]]: ...
+        ) -> MethodWrapper[_P, Awaitable[_Ret], io.Out[ObjectRef[_Ret]]]: ...
 
         @overload
         def options(
             self: AsyncMethod[_P, tuple[_R0]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
-        ) -> MethodWrapper[_P, Awaitable[_Ret], tuple[ObjectRef[_R0]]]: ...
+        ) -> MethodWrapper[_P, Awaitable[_Ret], io.Out[tuple[ObjectRef[_R0]]]]: ...
 
         @overload
         def options(
             self: AsyncMethod[_P, tuple[_R0, _R1]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
-            _P, Awaitable[_Ret], tuple[ObjectRef[_R0], ObjectRef[_R1]]
+            _P, Awaitable[_Ret], io.Out[tuple[ObjectRef[_R0], ObjectRef[_R1]]]
         ]: ...
 
         @overload
         def options(
             self: AsyncMethod[_P, tuple[_R0, _R1, _R2]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             Awaitable[_Ret],
-            tuple[ObjectRef[_R0], ObjectRef[_R1], ObjectRef[_R2]],
+            io.Out[tuple[ObjectRef[_R0], ObjectRef[_R1], ObjectRef[_R2]]],
         ]: ...
 
         @overload
         def options(
             self: AsyncMethod[_P, tuple[_R0, _R1, _R2, _R3]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             Awaitable[_Ret],
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                ]
             ],
         ]: ...
 
         @overload
         def options(
             self: AsyncMethod[_P, tuple[_R0, _R1, _R2, _R3, _R4]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             Awaitable[_Ret],
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
-                ObjectRef[_R4],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                    ObjectRef[_R4],
+                ]
             ],
         ]: ...
 
         @overload
         def options(
             self: AsyncMethod[_P, tuple[_R0, _R1, _R2, _R3, _R4, _R5]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             Awaitable[_Ret],
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
-                ObjectRef[_R4],
-                ObjectRef[_R5],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                    ObjectRef[_R4],
+                    ObjectRef[_R5],
+                ]
             ],
         ]: ...
 
         @overload
         def options(
             self: AsyncMethod[_P, tuple[_R0, _R1, _R2, _R3, _R4, _R5, _R6]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             Awaitable[_Ret],
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
-                ObjectRef[_R4],
-                ObjectRef[_R5],
-                ObjectRef[_R6],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                    ObjectRef[_R4],
+                    ObjectRef[_R5],
+                    ObjectRef[_R6],
+                ]
             ],
         ]: ...
 
         @overload
         def options(
             self: AsyncMethod[_P, tuple[_R0, _R1, _R2, _R3, _R4, _R5, _R6, _R7]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             Awaitable[_Ret],
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
-                ObjectRef[_R4],
-                ObjectRef[_R5],
-                ObjectRef[_R6],
-                ObjectRef[_R7],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                    ObjectRef[_R4],
+                    ObjectRef[_R5],
+                    ObjectRef[_R6],
+                    ObjectRef[_R7],
+                ]
             ],
         ]: ...
 
         @overload
         def options(
             self: AsyncMethod[_P, tuple[_R0, _R1, _R2, _R3, _R4, _R5, _R6, _R7, _R8]],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             Awaitable[_Ret],
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
-                ObjectRef[_R4],
-                ObjectRef[_R5],
-                ObjectRef[_R6],
-                ObjectRef[_R7],
-                ObjectRef[_R8],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                    ObjectRef[_R4],
+                    ObjectRef[_R5],
+                    ObjectRef[_R6],
+                    ObjectRef[_R7],
+                    ObjectRef[_R8],
+                ]
             ],
         ]: ...
 
         @overload
         def options(
             self: AsyncMethod[
                 _P, tuple[_R0, _R1, _R2, _R3, _R4, _R5, _R6, _R7, _R8, _R9]
             ],
             *,
             unpack: Literal[True],
             **options: Unpack[MethodOptions],
         ) -> MethodWrapper[
             _P,
             Awaitable[_Ret],
-            tuple[
-                ObjectRef[_R0],
-                ObjectRef[_R1],
-                ObjectRef[_R2],
-                ObjectRef[_R3],
-                ObjectRef[_R4],
-                ObjectRef[_R5],
-                ObjectRef[_R6],
-                ObjectRef[_R7],
-                ObjectRef[_R8],
-                ObjectRef[_R9],
+            io.Out[
+                tuple[
+                    ObjectRef[_R0],
+                    ObjectRef[_R1],
+                    ObjectRef[_R2],
+                    ObjectRef[_R3],
+                    ObjectRef[_R4],
+                    ObjectRef[_R5],
+                    ObjectRef[_R6],
+                    ObjectRef[_R7],
+                    ObjectRef[_R8],
+                    ObjectRef[_R9],
+                ]
             ],
         ]: ...
 
         def options(
             self, *, unpack: bool = False, **options: Unpack[MethodOptions]
         ) -> MethodWrapper: ...
 
         def __call__(self, *args: _P.args, **kwds: _P.kwargs) -> Awaitable[_Ret]: ...
 
     class StreamMethod(Generic[_P, _Ret, _YieldItem]):
-        remote: RemoteCallable[Callable[_P, _Ret], ObjectRefGenerator[_YieldItem]]
+        remote: RemoteCallable[
+            Callable[_P, _Ret], io.Out[ObjectRefGenerator[_YieldItem]]
+        ]
+        bind: ClassStreamBindCallable[Callable[_P, _Ret], io.Yield[_YieldItem]]
 
         def options(
             self, **options: Unpack[MethodOptions]
-        ) -> MethodWrapper[_P, _Ret, ObjectRefGenerator[_YieldItem]]: ...
+        ) -> MethodWrapper[_P, _Ret, io.Out[ObjectRefGenerator[_YieldItem]]]: ...
 
         def __call__(self, *args: _P.args, **kwds: _P.kwargs) -> _Ret: ...
 
     class MethodWrapper(Generic[_P, _Ret, _RemoteRet]):
         remote: RemoteCallable[Callable[_P, _Ret], _RemoteRet]
 
         def __call__(self, *args: _P.args, **kwds: _P.kwargs) -> _Ret: ...
@@ -692,14 +746,19 @@
         )
 
     def remote(self, *args: Any, **kwds: Any) -> Any:
         return getattr(self._sunray_actor.methods, self.method.__name__).remote(
             *args, **kwds
         )
 
+    def bind(self, *args: Any, **kwds: Any) -> Any:
+        return getattr(self._sunray_actor.methods, self.method.__name__).bind(
+            *args, **kwds
+        )
+
 
 class ActorMixin:
     """
     Make a class into an actor class.
 
     Example:
         ```python
```

## sunray/_internal/core.py

```diff
@@ -150,14 +150,20 @@
     def get(
         __object_refs: ObjectRef[_R0],
         *,
         timeout: float = ...,
     ) -> _R0: ...
     @overload
     def get(
+        __object_refs: tuple[ObjectRef[_R0]],
+        *,
+        timeout: float = ...,
+    ) -> tuple[_R0]: ...
+    @overload
+    def get(
         __object_refs: tuple[ObjectRef[_R0], ObjectRef[_R1]],
         *,
         timeout: float = ...,
     ) -> tuple[_R0, _R1]: ...
     @overload
     def get(
         __object_refs: tuple[ObjectRef[_R0], ObjectRef[_R1], ObjectRef[_R2]],
@@ -271,14 +277,16 @@
     @overload
     def get(
         __object_refs: list[ObjectRef],
         *,
         timeout: float | None = ...,
     ) -> tuple: ...
 
+    def get(__object_refs, *, timeout: float | None = ...) -> Any: ...
+
     def put(value: _T, *, _owner: ray.actor.ActorHandle = ...) -> ObjectRef[_T]: ...
 
     @overload
     def wait(
         object_refs: list[ObjectRef[_T]],
         *,
         num_returns: int = ...,
@@ -290,14 +298,22 @@
         object_refs: list[ObjectRef],
         *,
         num_returns: int = ...,
         timeout: float | None = ...,
         fetch_local: bool = ...,
     ) -> tuple[list[ObjectRef], list[ObjectRef]]: ...
 
+    def wait(
+        object_refs,
+        *,
+        num_returns: int = ...,
+        timeout: float | None = ...,
+        fetch_local: bool = ...,
+    ) -> Any: ...
+
     class Language(enum.IntEnum):
         JAVA = 1
         CPP = 2
         PYTHON = 3
 
     class RuntimeContext(ray.runtime_context.RuntimeContext):
         @deprecated("Use get_xxx_id() methods to get relevant ids instead.")
@@ -406,14 +422,16 @@
 
     @overload
     def timeline(filename: str | Path) -> None: ...
 
     @overload
     def timeline(filename: None = None) -> list[ProfileEvent]: ...
 
+    def timeline(filename=None) -> Any: ...
+
     def cancel(
         ray_waitable: ObjectRef[_R] | ObjectRefGenerator[_R],
         *,
         force: bool = False,
         recursive: bool = True,
     ) -> None: ...
```

## sunray/_internal/remote.py

```diff
@@ -10,33 +10,39 @@
 
 import ray
 import ray.actor
 
 from ray import remote_function as ray_func
 from typing_extensions import ParamSpec
 
+from .dag import FunctionNode
+from .dag import StreamNode
+from .io import Out
+from .io import Yield
 from .util import get_num_returns
 
 
 if TYPE_CHECKING:
     from typing import Any
     from typing import Generator
     from typing import Literal
 
     from ray.actor import ActorClass
     from typing_extensions import Unpack
 
+    from .callable import FunctionBindCallable
+    from .callable import RemoteCallable
+    from .callable import StreamBindCallable
     from .core import ObjectRef
     from .core import ObjectRefGenerator
     from .typing import FunctionRemoteOptions
-    from .typing import RemoteCallable
 
 
 _Callable_co = TypeVar("_Callable_co", covariant=True, bound=Callable)
-_RemoteRet = TypeVar("_RemoteRet")
+_RemoteRet = TypeVar("_RemoteRet", bound=Out)
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 _R0 = TypeVar("_R0")
 _R1 = TypeVar("_R1")
 _R2 = TypeVar("_R2")
 _R3 = TypeVar("_R3")
 _R4 = TypeVar("_R4")
@@ -52,247 +58,284 @@
         self, remote_func: ray_func.RemoteFunction, opts: FunctionRemoteOptions
     ) -> None:
         self._remote_func = remote_func
         self._opts = opts
 
     if TYPE_CHECKING:
         remote: RemoteCallable[_Callable_co, _RemoteRet]
+        bind: FunctionBindCallable[_Callable_co, _RemoteRet]
     else:
 
         def remote(self, *args, **kwargs):
             opts = dict(self._opts)
             return self._remote_func.options(**opts).remote(*args, **kwargs)
 
+        def bind(self, *args, **kwargs):
+            return FunctionNode(self._remote_func._function, args, kwargs, self._opts)
+
 
 class RemoteFunction(RemoteFunctionWrapper, Generic[_Callable_co, _R]):
-    remote: RemoteCallable[_Callable_co, ObjectRef[_R]]
+    remote: RemoteCallable[_Callable_co, Out[ObjectRef[_R]]]
 
     @overload
     def options(
         self,
         *,
         unpack: Literal[False] = False,
         **opts: Unpack[FunctionRemoteOptions],
-    ) -> RemoteFunctionWrapper[_Callable_co, ObjectRef[_R]]: ...
+    ) -> RemoteFunctionWrapper[_Callable_co, Out[ObjectRef[_R]]]: ...
 
     @overload
     def options(
         self: RemoteFunction[_Callable_co, tuple[_R0]],
         *,
         unpack: Literal[True],
         **opts: Unpack[FunctionRemoteOptions],
-    ) -> RemoteFunctionWrapper[_Callable_co, tuple[ObjectRef[_R0]]]: ...
+    ) -> RemoteFunctionWrapper[_Callable_co, Out[tuple[ObjectRef[_R0]]]]: ...
 
     @overload
     def options(
         self: RemoteFunction[_Callable_co, tuple[_R0, _R1]],
         *,
         unpack: Literal[True],
         **opts: Unpack[FunctionRemoteOptions],
-    ) -> RemoteFunctionWrapper[_Callable_co, tuple[ObjectRef[_R0], ObjectRef[_R1]]]: ...
+    ) -> RemoteFunctionWrapper[
+        _Callable_co, Out[tuple[ObjectRef[_R0], ObjectRef[_R1]]]
+    ]: ...
 
     @overload
     def options(
         self: RemoteFunction[_Callable_co, tuple[_R0, _R1, _R2]],
         *,
         unpack: Literal[True],
         **opts: Unpack[FunctionRemoteOptions],
     ) -> RemoteFunctionWrapper[
-        _Callable_co, tuple[ObjectRef[_R0], ObjectRef[_R1], ObjectRef[_R2]]
+        _Callable_co, Out[tuple[ObjectRef[_R0], ObjectRef[_R1], ObjectRef[_R2]]]
     ]: ...
 
     @overload
     def options(
         self: RemoteFunction[_Callable_co, tuple[_R0, _R1, _R2, _R3]],
         *,
         unpack: Literal[True],
         **opts: Unpack[FunctionRemoteOptions],
     ) -> RemoteFunctionWrapper[
         _Callable_co,
-        tuple[
-            ObjectRef[_R0],
-            ObjectRef[_R1],
-            ObjectRef[_R2],
-            ObjectRef[_R3],
+        Out[
+            tuple[
+                ObjectRef[_R0],
+                ObjectRef[_R1],
+                ObjectRef[_R2],
+                ObjectRef[_R3],
+            ]
         ],
     ]: ...
 
     @overload
     def options(
         self: RemoteFunction[_Callable_co, tuple[_R0, _R1, _R2, _R3, _R4]],
         *,
         unpack: Literal[True],
         **opts: Unpack[FunctionRemoteOptions],
     ) -> RemoteFunctionWrapper[
         _Callable_co,
-        tuple[
-            ObjectRef[_R0],
-            ObjectRef[_R1],
-            ObjectRef[_R2],
-            ObjectRef[_R3],
-            ObjectRef[_R4],
+        Out[
+            tuple[
+                ObjectRef[_R0],
+                ObjectRef[_R1],
+                ObjectRef[_R2],
+                ObjectRef[_R3],
+                ObjectRef[_R4],
+            ]
         ],
     ]: ...
 
     @overload
     def options(
         self: RemoteFunction[_Callable_co, tuple[_R0, _R1, _R2, _R3, _R4, _R5]],
         *,
         unpack: Literal[True],
         **opts: Unpack[FunctionRemoteOptions],
     ) -> RemoteFunctionWrapper[
         _Callable_co,
-        tuple[
-            ObjectRef[_R0],
-            ObjectRef[_R1],
-            ObjectRef[_R2],
-            ObjectRef[_R3],
-            ObjectRef[_R4],
-            ObjectRef[_R5],
+        Out[
+            tuple[
+                ObjectRef[_R0],
+                ObjectRef[_R1],
+                ObjectRef[_R2],
+                ObjectRef[_R3],
+                ObjectRef[_R4],
+                ObjectRef[_R5],
+            ]
         ],
     ]: ...
 
     @overload
     def options(
         self: RemoteFunction[_Callable_co, tuple[_R0, _R1, _R2, _R3, _R4, _R5, _R6]],
         *,
         unpack: Literal[True],
         **opts: Unpack[FunctionRemoteOptions],
     ) -> RemoteFunctionWrapper[
         _Callable_co,
-        tuple[
-            ObjectRef[_R0],
-            ObjectRef[_R1],
-            ObjectRef[_R2],
-            ObjectRef[_R3],
-            ObjectRef[_R4],
-            ObjectRef[_R5],
-            ObjectRef[_R6],
+        Out[
+            tuple[
+                ObjectRef[_R0],
+                ObjectRef[_R1],
+                ObjectRef[_R2],
+                ObjectRef[_R3],
+                ObjectRef[_R4],
+                ObjectRef[_R5],
+                ObjectRef[_R6],
+            ]
         ],
     ]: ...
 
     @overload
     def options(
         self: RemoteFunction[
             _Callable_co, tuple[_R0, _R1, _R2, _R3, _R4, _R5, _R6, _R7]
         ],
         *,
         unpack: Literal[True],
         **opts: Unpack[FunctionRemoteOptions],
     ) -> RemoteFunctionWrapper[
         _Callable_co,
-        tuple[
-            ObjectRef[_R0],
-            ObjectRef[_R1],
-            ObjectRef[_R2],
-            ObjectRef[_R3],
-            ObjectRef[_R4],
-            ObjectRef[_R5],
-            ObjectRef[_R6],
-            ObjectRef[_R7],
+        Out[
+            tuple[
+                ObjectRef[_R0],
+                ObjectRef[_R1],
+                ObjectRef[_R2],
+                ObjectRef[_R3],
+                ObjectRef[_R4],
+                ObjectRef[_R5],
+                ObjectRef[_R6],
+                ObjectRef[_R7],
+            ]
         ],
     ]: ...
 
     @overload
     def options(
         self: RemoteFunction[
             _Callable_co, tuple[_R0, _R1, _R2, _R3, _R4, _R5, _R6, _R7, _R8]
         ],
         *,
         unpack: Literal[True],
         **opts: Unpack[FunctionRemoteOptions],
     ) -> RemoteFunctionWrapper[
         _Callable_co,
-        tuple[
-            ObjectRef[_R0],
-            ObjectRef[_R1],
-            ObjectRef[_R2],
-            ObjectRef[_R3],
-            ObjectRef[_R4],
-            ObjectRef[_R5],
-            ObjectRef[_R6],
-            ObjectRef[_R7],
-            ObjectRef[_R8],
+        Out[
+            tuple[
+                ObjectRef[_R0],
+                ObjectRef[_R1],
+                ObjectRef[_R2],
+                ObjectRef[_R3],
+                ObjectRef[_R4],
+                ObjectRef[_R5],
+                ObjectRef[_R6],
+                ObjectRef[_R7],
+                ObjectRef[_R8],
+            ]
         ],
     ]: ...
 
     @overload
     def options(
         self: RemoteFunction[
             _Callable_co, tuple[_R0, _R1, _R2, _R3, _R4, _R5, _R6, _R7, _R8, _R9]
         ],
         *,
         unpack: Literal[True],
         **opts: Unpack[FunctionRemoteOptions],
     ) -> RemoteFunctionWrapper[
         _Callable_co,
-        tuple[
-            ObjectRef[_R0],
-            ObjectRef[_R1],
-            ObjectRef[_R2],
-            ObjectRef[_R3],
-            ObjectRef[_R4],
-            ObjectRef[_R5],
-            ObjectRef[_R6],
-            ObjectRef[_R7],
-            ObjectRef[_R8],
-            ObjectRef[_R9],
+        Out[
+            tuple[
+                ObjectRef[_R0],
+                ObjectRef[_R1],
+                ObjectRef[_R2],
+                ObjectRef[_R3],
+                ObjectRef[_R4],
+                ObjectRef[_R5],
+                ObjectRef[_R6],
+                ObjectRef[_R7],
+                ObjectRef[_R8],
+                ObjectRef[_R9],
+            ]
         ],
     ]: ...
 
     def options(
         self,
         *,
         unpack: bool = False,
         **opts: Unpack[FunctionRemoteOptions],
     ):
         opts = {**self._opts, **opts}
         num_returns = get_num_returns(self._remote_func._function) if unpack else 1
         opts["num_returns"] = num_returns  # type: ignore[typeddict-unknown-key]
         return RemoteFunctionWrapper(self._remote_func, opts)
 
+    if TYPE_CHECKING:
+        bind: FunctionBindCallable[_Callable_co, Out[ObjectRef[_R]]]
+    else:
+
+        def bind(self, *args, **kwargs):
+            return self._remote_func.bind(*args, **kwargs)
+
 
-class RemoteStreamWrapper(Generic[_Callable_co, _RemoteRet]):
+class RemoteStreamWrapper(Generic[_Callable_co, _R]):
     def __init__(
         self, remote_func: ray_func.RemoteFunction, opts: FunctionRemoteOptions
     ) -> None:
         self._remote_func = remote_func
         self._opts = opts
 
     if TYPE_CHECKING:
-        remote: RemoteCallable[_Callable_co, _RemoteRet]
+        remote: RemoteCallable[_Callable_co, Out[ObjectRefGenerator[_R]]]
+        bind: StreamBindCallable[_Callable_co, Yield[_R]]
     else:
 
         def remote(self, *args, **kwargs):
             opts = dict(self._opts)
             opts["num_returns"] = "streaming"
 
             return self._remote_func.options(**opts).remote(*args, **kwargs)
 
+        def bind(self, *args, **kwargs):
+            opts = dict(self._opts)
+            opts["num_returns"] = "streaming"
+
+            return StreamNode(self._remote_func._function, args, kwargs, self._opts)
 
-class RemoteStream(RemoteStreamWrapper[_Callable_co, _RemoteRet]):
+
+class RemoteStream(RemoteStreamWrapper[_Callable_co, _R]):
     def options(
         self, **opts: Unpack[FunctionRemoteOptions]
-    ) -> RemoteStreamWrapper[_Callable_co, _RemoteRet]:
+    ) -> RemoteStreamWrapper[_Callable_co, _R]:
         opts = {**self._opts, **opts}
         return RemoteStreamWrapper(self._remote_func, opts)
 
+    if not TYPE_CHECKING:
+
+        def bind(self, *args, **kwargs):  # pragma: no cover
+            return self._remote_func.bind(*args, **kwargs)
+
 
 if TYPE_CHECKING:
 
     class RemoteDecorator:
         @overload
         def __call__(self, __obj: type) -> ActorClass: ...
 
         @overload
         def __call__(
             self, __obj: Callable[_P, Generator[_R, Any, Any]]
-        ) -> RemoteStream[
-            Callable[_P, Generator[_R, Any, Any]], ObjectRefGenerator[_R]
-        ]: ...
+        ) -> RemoteStream[Callable[_P, Generator[_R, Any, Any]], _R]: ...
 
         @overload
         def __call__(
             self, __obj: Callable[_P, _R]
         ) -> RemoteFunction[Callable[_P, _R], _R]: ...
 
         def __call__(self, __obj) -> Any: ...
@@ -301,15 +344,15 @@
 @overload
 def remote(__type: type) -> ActorClass: ...
 
 
 @overload
 def remote(
     __func: Callable[_P, Generator[_R, Any, Any]],
-) -> RemoteStream[Callable[_P, Generator[_R, Any, Any]], ObjectRefGenerator[_R]]: ...
+) -> RemoteStream[Callable[_P, Generator[_R, Any, Any]], _R]: ...
 
 
 @overload
 def remote(__func: Callable[_P, _R]) -> RemoteFunction[Callable[_P, _R], _R]: ...
 
 
 @overload
```

## sunray/_internal/typing.py

```diff
@@ -2,47 +2,23 @@
 
 from typing import TYPE_CHECKING
 
 
 if TYPE_CHECKING:
     import types
 
-    from typing import Any
-    from typing import Callable
-    from typing import Generic
-    from typing import TypeVar
     from typing import Union
-    from typing import overload
-
-    import ray
 
     from ray import runtime_env
     from ray.util import scheduling_strategies
-    from typing_extensions import Concatenate
     from typing_extensions import Literal
     from typing_extensions import NotRequired
-    from typing_extensions import ParamSpec
     from typing_extensions import Required
     from typing_extensions import TypedDict
 
-    _P = ParamSpec("_P")
-    _T = TypeVar("_T")
-    _T0 = TypeVar("_T0")
-    _T1 = TypeVar("_T1")
-    _T2 = TypeVar("_T2")
-    _T3 = TypeVar("_T3")
-    _T4 = TypeVar("_T4")
-    _T5 = TypeVar("_T5")
-    _T6 = TypeVar("_T6")
-    _T7 = TypeVar("_T7")
-    _T8 = TypeVar("_T8")
-    _T9 = TypeVar("_T9")
-
-    RemoteArg = Union[_T, ray.ObjectRef[_T]]
-
     SchedulingStrategy = Union[
         Literal["DEFAULT", "SPREAD"],
         scheduling_strategies.PlacementGroupSchedulingStrategy,
         scheduling_strategies.NodeAffinitySchedulingStrategy,
         scheduling_strategies.NodeLabelSchedulingStrategy,
         None,
     ]
@@ -223,225 +199,7 @@
         packages: Required[list[str]]
         pip_check: NotRequired[bool]
         pip_version: NotRequired[str]
 
     class RuntimeEnvConfig(TypedDict, total=False):
         setup_timeout_seconds: int
         eager_install: bool
-
-    _Callable_co = TypeVar("_Callable_co", covariant=True, bound=Callable)
-    _RemoteRet = TypeVar("_RemoteRet")
-
-    class RemoteCallable(Generic[_Callable_co, _RemoteRet]):
-        @overload
-        def __call__(
-            self: RemoteCallable[
-                Callable[
-                    Concatenate[_T0, _T1, _T2, _T3, _T4, _T5, _T6, _T7, _T8, _T9, _P],
-                    Any,
-                ],
-                _RemoteRet,
-            ],
-            __arg0: RemoteArg[_T0],
-            __arg1: RemoteArg[_T1],
-            __arg2: RemoteArg[_T2],
-            __arg3: RemoteArg[_T3],
-            __arg4: RemoteArg[_T4],
-            __arg5: RemoteArg[_T5],
-            __arg6: RemoteArg[_T6],
-            __arg7: RemoteArg[_T7],
-            __arg8: RemoteArg[_T8],
-            __arg9: RemoteArg[_T9],
-            *args: _P.args,
-            **kwargs: _P.kwargs,
-        ) -> _RemoteRet: ...
-
-        @overload
-        def __call__(
-            self: RemoteCallable[
-                Callable[
-                    Concatenate[_T0, _T1, _T2, _T3, _T4, _T5, _T6, _T7, _T8, _P],
-                    Any,
-                ],
-                _RemoteRet,
-            ],
-            __arg0: RemoteArg[_T0],
-            __arg1: RemoteArg[_T1],
-            __arg2: RemoteArg[_T2],
-            __arg3: RemoteArg[_T3],
-            __arg4: RemoteArg[_T4],
-            __arg5: RemoteArg[_T5],
-            __arg6: RemoteArg[_T6],
-            __arg7: RemoteArg[_T7],
-            __arg8: RemoteArg[_T8],
-            *args: _P.args,
-            **kwargs: _P.kwargs,
-        ) -> _RemoteRet: ...
-
-        @overload
-        def __call__(
-            self: RemoteCallable[
-                Callable[
-                    Concatenate[_T0, _T1, _T2, _T3, _T4, _T5, _T6, _T7, _P],
-                    Any,
-                ],
-                _RemoteRet,
-            ],
-            __arg0: RemoteArg[_T0],
-            __arg1: RemoteArg[_T1],
-            __arg2: RemoteArg[_T2],
-            __arg3: RemoteArg[_T3],
-            __arg4: RemoteArg[_T4],
-            __arg5: RemoteArg[_T5],
-            __arg6: RemoteArg[_T6],
-            __arg7: RemoteArg[_T7],
-            *args: _P.args,
-            **kwargs: _P.kwargs,
-        ) -> _RemoteRet: ...
-
-        @overload
-        def __call__(
-            self: RemoteCallable[
-                Callable[
-                    Concatenate[_T0, _T1, _T2, _T3, _T4, _T5, _T6, _P],
-                    Any,
-                ],
-                _RemoteRet,
-            ],
-            __arg0: RemoteArg[_T0],
-            __arg1: RemoteArg[_T1],
-            __arg2: RemoteArg[_T2],
-            __arg3: RemoteArg[_T3],
-            __arg4: RemoteArg[_T4],
-            __arg5: RemoteArg[_T5],
-            __arg6: RemoteArg[_T6],
-            *args: _P.args,
-            **kwargs: _P.kwargs,
-        ) -> _RemoteRet: ...
-
-        @overload
-        def __call__(
-            self: RemoteCallable[
-                Callable[
-                    Concatenate[_T0, _T1, _T2, _T3, _T4, _T5, _T6, _P],
-                    Any,
-                ],
-                _RemoteRet,
-            ],
-            __arg0: RemoteArg[_T0],
-            __arg1: RemoteArg[_T1],
-            __arg2: RemoteArg[_T2],
-            __arg3: RemoteArg[_T3],
-            __arg4: RemoteArg[_T4],
-            __arg5: RemoteArg[_T5],
-            __arg6: RemoteArg[_T6],
-            *args: _P.args,
-            **kwargs: _P.kwargs,
-        ) -> _RemoteRet: ...
-
-        @overload
-        def __call__(
-            self: RemoteCallable[
-                Callable[
-                    Concatenate[_T0, _T1, _T2, _T3, _T4, _T5, _P],
-                    Any,
-                ],
-                _RemoteRet,
-            ],
-            __arg0: RemoteArg[_T0],
-            __arg1: RemoteArg[_T1],
-            __arg2: RemoteArg[_T2],
-            __arg3: RemoteArg[_T3],
-            __arg4: RemoteArg[_T4],
-            __arg5: RemoteArg[_T5],
-            *args: _P.args,
-            **kwargs: _P.kwargs,
-        ) -> _RemoteRet: ...
-
-        @overload
-        def __call__(
-            self: RemoteCallable[
-                Callable[
-                    Concatenate[_T0, _T1, _T2, _T3, _T4, _P],
-                    Any,
-                ],
-                _RemoteRet,
-            ],
-            __arg0: RemoteArg[_T0],
-            __arg1: RemoteArg[_T1],
-            __arg2: RemoteArg[_T2],
-            __arg3: RemoteArg[_T3],
-            __arg4: RemoteArg[_T4],
-            *args: _P.args,
-            **kwargs: _P.kwargs,
-        ) -> _RemoteRet: ...
-
-        @overload
-        def __call__(
-            self: RemoteCallable[
-                Callable[
-                    Concatenate[_T0, _T1, _T2, _T3, _P],
-                    Any,
-                ],
-                _RemoteRet,
-            ],
-            __arg0: RemoteArg[_T0],
-            __arg1: RemoteArg[_T1],
-            __arg2: RemoteArg[_T2],
-            __arg3: RemoteArg[_T3],
-            *args: _P.args,
-            **kwargs: _P.kwargs,
-        ) -> _RemoteRet: ...
-
-        @overload
-        def __call__(
-            self: RemoteCallable[
-                Callable[
-                    Concatenate[_T0, _T1, _T2, _P],
-                    Any,
-                ],
-                _RemoteRet,
-            ],
-            __arg0: RemoteArg[_T0],
-            __arg1: RemoteArg[_T1],
-            __arg2: RemoteArg[_T2],
-            *args: _P.args,
-            **kwargs: _P.kwargs,
-        ) -> _RemoteRet: ...
-
-        @overload
-        def __call__(
-            self: RemoteCallable[
-                Callable[
-                    Concatenate[_T0, _T1, _P],
-                    Any,
-                ],
-                _RemoteRet,
-            ],
-            __arg0: RemoteArg[_T0],
-            __arg1: RemoteArg[_T1],
-            *args: _P.args,
-            **kwargs: _P.kwargs,
-        ) -> _RemoteRet: ...
-
-        @overload
-        def __call__(
-            self: RemoteCallable[
-                Callable[
-                    Concatenate[_T0, _P],
-                    Any,
-                ],
-                _RemoteRet,
-            ],
-            __arg0: RemoteArg[_T0],
-            *args: _P.args,
-            **kwargs: _P.kwargs,
-        ) -> _RemoteRet: ...
-
-        @overload
-        def __call__(
-            self: RemoteCallable[Callable[_P, Any], _RemoteRet],
-            *args: _P.args,
-            **kwargs: _P.kwargs,
-        ) -> _RemoteRet: ...
-
-        def __call__(self, *args: Any, **kwds: Any) -> _RemoteRet: ...
```

## Comparing `sunray-0.2.0.dist-info/LICENSE` & `sunray-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sunray-0.2.0.dist-info/METADATA` & `sunray-0.3.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunray
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: ZhengYu, Xu
 Author-email: zen-xu@outlook.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -101,17 +101,25 @@
 |                                     sunray                                      |                                     ray                                      |
 | :-----------------------------------------------------------------------------: | :--------------------------------------------------------------------------: |
 | ![](https://zenxu-github-asset.s3.us-east-2.amazonaws.com/sunray_call_self_remote_method.jpg) | ![](https://zenxu-github-asset.s3.us-east-2.amazonaws.com/ray_call_self_remote_method.jpg) |
 
 - sunray maintains a consistent calling convention, whether it's from internal or external functions.
 - ray, you need to first obtain the current actor from the running context, and then call through the actor.
 
+### Round 9: Lazy Computation
+|                                            sunray                                             |                                            ray                                             |
+| :-------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------: |
+| ![](https://zenxu-github-asset.s3.us-east-2.amazonaws.com/sunray_bind.jpg) | ![](https://zenxu-github-asset.s3.us-east-2.amazonaws.com/ray_bind.jpg) |
+
+- sunray can successfully track the input parameter types and output types.
+- ray does not have this capability.
+
 ## API
 
-`sunray` re-export all apis from `ray.core` with friendly type hinting. In addition, `sunray` provides `ActorMixin` which is used to help creating more robust actors.
+`sunray` re-export all apis from `ray.core` with friendly type hints. In addition, `sunray` provides `ActorMixin` which is used to help creating more robust actors.
 
 ### ActorMixin
 
 `ActorMixin` is a mixin, and provides a classmethod `new_actor`
 
 ```python
 import sunray
```

## Comparing `sunray-0.2.0.dist-info/RECORD` & `sunray-0.3.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-sunray/__init__.py,sha256=T04TCSknAWk4UJcTVqHaqpEr9ToX23omZfN2_5l7VO8,2272
+sunray/__init__.py,sha256=2NZbK6w7bnGNC_jPVPMokLlQotKBC3-ezjVKHIxTjOU,2272
 sunray/_internal/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sunray/_internal/actor_mixin.py,sha256=0wJKE0IP5iuY7YVbrALgUxk_mKT_19oSQtS-fVkbY1s,23109
-sunray/_internal/core.py,sha256=Akvhl4lMFMy4RrbEF2xOyPpt4CwYITzXYHhFobVcuFU,14899
-sunray/_internal/remote.py,sha256=fluvXvivQWYyKZ56Sddx-05K6iPFZSGr6tXovXsBfcw,9677
-sunray/_internal/typing.py,sha256=pq__-UV4WWq9t5NjbbvdNEj0d_W1M96AsKAqqm7tsJU,18265
+sunray/_internal/actor_mixin.py,sha256=zhtKOKSdrMURT2cTf3Bq-WqVyrpiemSVt5uAToZxNBI,25396
+sunray/_internal/callable.py,sha256=eVi_mmJjOsZzVwqaP1DTfWBDF3nRMXhacBC6yT_fPpM,65315
+sunray/_internal/core.py,sha256=QE5Vgx1e50Z4N4jc6w4JnutKgtlIJTXeWQ_7xAx8ck0,15322
+sunray/_internal/dag.py,sha256=B3g-Z0zVGfv7zWj2jO7eTrYsHdvzdxSel54UF_IeKU0,10468
+sunray/_internal/io.py,sha256=44YKqLW-oeKI8ehhGtc8ZhJ2yk4jx2Zrfh4pa3trNPs,658
+sunray/_internal/remote.py,sha256=Qsrql1NiiW26E_O6euuZ3U-E_RY_vz-6uqY6KdObsok,11074
+sunray/_internal/typing.py,sha256=jpgUvdGXrDN62G_fS3Ta_4l7cALlpNr5h3FcDZ58i5U,11210
 sunray/_internal/util.py,sha256=WQ6WLD_b2uY1d_6nyf24R7SbP1nqZ1CmUnzS5NMaiLA,807
+sunray/dag.py,sha256=ydCtgNVf_E2K0AFABzRhPkvlLPPUq6HQLR7QXswODJM,430
 sunray/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-sunray-0.2.0.dist-info/LICENSE,sha256=4ix-bYe2BfMr6RchyTiQ2g18h5fXPTdVrjB6LLsxoaQ,1068
-sunray-0.2.0.dist-info/METADATA,sha256=ia_lShze8GqYLtaSFOe8re6H_VQg9ATRmSfi_em3hUk,8155
-sunray-0.2.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-sunray-0.2.0.dist-info/RECORD,,
+sunray-0.3.0.dist-info/LICENSE,sha256=4ix-bYe2BfMr6RchyTiQ2g18h5fXPTdVrjB6LLsxoaQ,1068
+sunray-0.3.0.dist-info/METADATA,sha256=XzmIGicc3y0Z5xNjzasGaJgdMQzOo2QsEcO2dWk0I2Y,8833
+sunray-0.3.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+sunray-0.3.0.dist-info/RECORD,,
```

