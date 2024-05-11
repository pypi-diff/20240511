# Comparing `tmp/tmexio-0.0.1.tar.gz` & `tmp/tmexio-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmexio-0.0.1.tar", max compression
+gzip compressed data, was "tmexio-0.1.0.tar", max compression
```

## Comparing `tmexio-0.0.1.tar` & `tmexio-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1609 2024-05-04 14:59:07.899484 tmexio-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      411 2024-04-21 15:42:25.222511 tmexio-0.0.1/README.md
--rw-r--r--   0        0        0      404 2024-05-04 22:21:51.762965 tmexio-0.0.1/tmexio/__init__.py
--rw-r--r--   0        0        0     5754 2024-05-04 23:13:56.692137 tmexio-0.0.1/tmexio/event_handlers.py
--rw-r--r--   0        0        0      197 2024-05-04 17:05:15.933243 tmexio-0.0.1/tmexio/exceptions.py
--rw-r--r--   0        0        0    15164 2024-05-04 23:18:46.403241 tmexio-0.0.1/tmexio/main.py
--rw-r--r--   0        0        0     1013 2024-05-04 23:02:09.303828 tmexio-0.0.1/tmexio/markers.py
--rw-r--r--   0        0        0     1806 2024-05-04 23:16:36.587439 tmexio-0.0.1/tmexio/packagers.py
--rw-r--r--   0        0        0        0 2024-05-05 10:52:42.132671 tmexio-0.0.1/tmexio/py.typed
--rw-r--r--   0        0        0     7858 2024-05-04 23:20:13.015841 tmexio-0.0.1/tmexio/server.py
--rw-r--r--   0        0        0      387 2024-05-04 23:18:25.059131 tmexio-0.0.1/tmexio/specs.py
--rw-r--r--   0        0        0      477 2024-05-04 22:28:19.144886 tmexio-0.0.1/tmexio/structures.py
--rw-r--r--   0        0        0      702 2024-05-01 16:59:30.610644 tmexio-0.0.1/tmexio/types.py
--rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 tmexio-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1609 2024-05-11 11:48:26.503752 tmexio-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      411 2024-04-21 15:42:25.222511 tmexio-0.1.0/README.md
+-rw-r--r--   0        0        0      453 2024-05-11 10:25:09.525589 tmexio-0.1.0/tmexio/__init__.py
+-rw-r--r--   0        0        0    11203 2024-05-10 23:13:42.672039 tmexio-0.1.0/tmexio/event_handlers.py
+-rw-r--r--   0        0        0      708 2024-05-10 16:49:06.445259 tmexio-0.1.0/tmexio/exceptions.py
+-rw-r--r--   0        0        0    14067 2024-05-11 11:43:32.291398 tmexio-0.1.0/tmexio/handler_builders.py
+-rw-r--r--   0        0        0     7238 2024-05-11 11:45:50.481598 tmexio-0.1.0/tmexio/main.py
+-rw-r--r--   0        0        0     1013 2024-05-10 21:31:02.418685 tmexio-0.1.0/tmexio/markers.py
+-rw-r--r--   0        0        0     1806 2024-05-04 23:16:36.587439 tmexio-0.1.0/tmexio/packagers.py
+-rw-r--r--   0        0        0        0 2024-05-05 10:52:42.132671 tmexio-0.1.0/tmexio/py.typed
+-rw-r--r--   0        0        0     7858 2024-05-04 23:20:13.015841 tmexio-0.1.0/tmexio/server.py
+-rw-r--r--   0        0        0      387 2024-05-04 23:18:25.059131 tmexio-0.1.0/tmexio/specs.py
+-rw-r--r--   0        0        0      477 2024-05-04 22:28:19.144886 tmexio-0.1.0/tmexio/structures.py
+-rw-r--r--   0        0        0      736 2024-05-10 23:13:42.672539 tmexio-0.1.0/tmexio/types.py
+-rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 tmexio-0.1.0/PKG-INFO
```

### Comparing `tmexio-0.0.1/pyproject.toml` & `tmexio-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tmexio"
-version = "0.0.1"
+version = "0.1.0"
 description = "Python framework for building SocketIO applications with typing, dependency injection and more"
 authors = ["niqzart <niqzart@gmail.com>"]
 readme = "README.md"
 exclude = [
     "tests",
     "docs",
 ]
```

### Comparing `tmexio-0.0.1/tmexio/main.py` & `tmexio-0.1.0/tmexio/handler_builders.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,151 +1,260 @@
 from __future__ import annotations
 
+from collections import OrderedDict, defaultdict
 from collections.abc import Awaitable, Callable, Iterator
-from inspect import Parameter, Signature, iscoroutinefunction, signature
-from logging import Logger
-from typing import Annotated, Any, Generic, Literal, TypeVar, get_args, get_origin
+from contextlib import asynccontextmanager
+from dataclasses import dataclass, field
+from inspect import (
+    Parameter,
+    Signature,
+    isasyncgenfunction,
+    iscoroutinefunction,
+    isgeneratorfunction,
+    signature,
+)
+from typing import Annotated, Any, Generic, TypeVar, get_args, get_origin
 
-import socketio  # type: ignore[import-untyped]
 from asgiref.sync import sync_to_async
 from pydantic import BaseModel, create_model
-from socketio.packet import Packet  # type: ignore[import-untyped]
 
 from tmexio import markers, packagers
 from tmexio.event_handlers import (
     AsyncConnectHandler,
     AsyncDisconnectHandler,
     AsyncEventHandler,
     BaseAsyncHandler,
-    BaseAsyncHandlerWithArguments,
+    BaseDependency,
+    ContextualDependency,
+    ValueDependency,
 )
 from tmexio.exceptions import EventException
 from tmexio.server import AsyncServer, AsyncSocket
 from tmexio.specs import HandlerSpec
 from tmexio.structures import ClientEvent
-from tmexio.types import ASGIAppProtocol, DataOrTuple, DataType
-
+from tmexio.types import DependencyCacheKey
 
-class Destinations:
-    def __init__(self) -> None:
-        self.markers: dict[markers.Marker[Any], set[str]] = {}
-        self.body_annotations: dict[str, Any] = {}
-        self.body_destinations: dict[str, set[str]] = {}
 
-    def add_marker_destination(
-        self, marker: markers.Marker[Any], destination: str
+class Depends:
+    def __init__(
+        self,
+        function: DependencyCacheKey,
+        exceptions: list[EventException],
+        dependencies: list[Depends],
     ) -> None:
-        self.markers.setdefault(marker, set()).add(destination)
+        self.function = function
+        self.exceptions = exceptions
+        self.dependencies = dependencies
 
-    def add_body_field(self, field_name: str, parameter_annotation: Any) -> None:
-        if get_origin(parameter_annotation) is not Annotated:
-            parameter_annotation = parameter_annotation, ...
-        self.body_annotations[field_name] = parameter_annotation
-        self.body_destinations.setdefault(field_name, set()).add(field_name)
 
-    def build_marker_destinations(self) -> list[tuple[markers.Marker[Any], list[str]]]:
-        return [
-            (marker, list(destinations))
-            for marker, destinations in self.markers.items()
-        ]
+@dataclass()
+class BuilderContext:
+    marker_definitions: set[markers.Marker[Any]] = field(default_factory=set)
+    body_annotations: dict[str, Any] = field(default_factory=dict)
+    dependency_order: OrderedDict[DependencyCacheKey, None] = field(
+        default_factory=OrderedDict
+    )  # order is reversed
+    dependency_definitions: dict[DependencyCacheKey, BaseDependency] = field(
+        default_factory=dict
+    )
+    possible_exceptions: set[EventException] = field(default_factory=set)
+
+    def build_marker_definitions(self) -> list[markers.Marker[Any]]:
+        return list(self.marker_definitions)
 
     def build_body_model(self) -> type[BaseModel] | None:
         if not self.body_annotations:
             return None
         return create_model(
             "Model",  # TODO better naming
             **self.body_annotations,
         )
 
-    def build_body_destinations(self) -> list[tuple[str, list[str]]]:
+    def build_dependency_definitions(
+        self,
+    ) -> list[tuple[DependencyCacheKey, BaseDependency]]:
         return [
-            (field, list(destinations))
-            for field, destinations in self.body_destinations.items()
+            (key, self.dependency_definitions[key])
+            for key in reversed(self.dependency_order)
         ]
 
 
-HandlerType = TypeVar("HandlerType", bound=BaseAsyncHandler)
+Key = TypeVar("Key")
 
 
-class HandlerBuilder(Generic[HandlerType]):
+class Destinations(Generic[Key]):
+    def __init__(self) -> None:
+        self.collection: dict[Key, set[str]] = defaultdict(set)
+
+    def add(self, key: Key, param_name: str) -> None:
+        self.collection[key].add(param_name)
+
+    def extract(self) -> list[tuple[Key, list[str]]]:
+        return [
+            (key, list(param_names)) for key, param_names in self.collection.items()
+        ]
+
+
+class RunnableBuilder:
     type_to_marker: dict[type[Any], markers.Marker[Any]] = {
         AsyncServer: markers.AsyncServerMarker(),
         AsyncSocket: markers.AsyncSocketMarker(),
         ClientEvent: markers.ClientEventMarker(),
     }
 
     def __init__(
         self,
         function: Callable[..., Any],
         possible_exceptions: list[EventException],
+        sub_dependencies: list[Depends],
+        builder_context: BuilderContext,
     ) -> None:
         self.function = function
         self.signature: Signature = signature(function)
-        self.destinations = Destinations()
 
-        self.possible_exceptions = possible_exceptions
+        self.marker_destinations: Destinations[markers.Marker[Any]] = Destinations()
+        self.body_destinations: Destinations[str] = Destinations()
+        self.dependency_destinations: Destinations[DependencyCacheKey] = Destinations()
+
+        self.context = builder_context
+        self.context.possible_exceptions.update(possible_exceptions)
+        for depends in reversed(sub_dependencies):
+            self.add_sub_dependency(depends)
+
+    def add_marker_destination(
+        self, marker: markers.Marker[Any], field_name: str
+    ) -> None:
+        self.context.marker_definitions.add(marker)
+        self.marker_destinations.add(marker, field_name)
+
+    def add_body_field(self, field_name: str, parameter_annotation: Any) -> None:
+        if get_origin(parameter_annotation) is not Annotated:
+            parameter_annotation = parameter_annotation, ...
+        # TODO this should check for conflicts (on context level)
+        self.context.body_annotations[field_name] = parameter_annotation
+        self.body_destinations.add(field_name, field_name)
+
+    def build_sub_dependency(self, depends: Depends) -> None:
+        # TODO reuse built dependencies from building other handlers
+        self.context.dependency_definitions[depends.function] = DependencyBuilder(
+            function=depends.function,
+            possible_exceptions=depends.exceptions,
+            sub_dependencies=depends.dependencies,
+            builder_context=self.context,
+        ).build()
+
+    def add_sub_dependency(self, depends: Depends) -> None:
+        if depends.function in self.context.dependency_order:
+            self.context.dependency_order.move_to_end(depends.function)
+        else:
+            self.context.dependency_order[  # noqa: WPS529  # linter bug
+                depends.function
+            ] = None
+            self.build_sub_dependency(depends)
+
+    def add_dependency_destination(self, depends: Depends, field_name: str) -> None:
+        self.add_sub_dependency(depends)
+        self.dependency_destinations.add(depends.function, field_name)
 
     def parse_parameter(self, parameter: Parameter) -> None:
         annotation = parameter.annotation
         if isinstance(annotation, type):
             marker = self.type_to_marker.get(annotation)
             if marker is not None:
                 annotation = Annotated[annotation, marker]
         args = get_args(annotation)
 
         if (  # noqa: WPS337
             get_origin(annotation) is Annotated
             and len(args) == 2
             and isinstance(args[1], markers.Marker)
         ):
-            self.destinations.add_marker_destination(args[1], parameter.name)
+            self.add_marker_destination(args[1], parameter.name)
+        elif (  # noqa: WPS337
+            get_origin(annotation) is Annotated
+            and len(args) == 2
+            and isinstance(args[1], Depends)
+        ):
+            self.add_dependency_destination(args[1], parameter.name)
         else:
-            self.destinations.add_body_field(parameter.name, parameter.annotation)
+            self.add_body_field(parameter.name, parameter.annotation)
+
+    def parse_parameters(self) -> None:
+        for parameter in self.signature.parameters.values():
+            self.parse_parameter(parameter)
 
     def build_async_callable(self) -> Callable[..., Awaitable[Any]]:
         if iscoroutinefunction(self.function):
             return self.function
         elif callable(self.function):
             return sync_to_async(self.function)
         raise TypeError("Handler is not callable")
 
-    def build_handler(self) -> HandlerType:
-        raise NotImplementedError
 
-    @classmethod
-    def build_spec_from_handler(
-        cls,
-        handler: HandlerType,
-        summary: str | None,
-        description: str | None,
-    ) -> HandlerSpec:
-        raise NotImplementedError
+class DependencyBuilder(RunnableBuilder):
+    def build(self) -> BaseDependency:
+        self.parse_parameters()
+
+        if isasyncgenfunction(self.function):
+            return ContextualDependency(
+                dependency_function=asynccontextmanager(self.function),
+                marker_destinations=self.marker_destinations.extract(),
+                body_destinations=self.body_destinations.extract(),
+                dependency_destinations=self.dependency_destinations.extract(),
+            )
+        elif isgeneratorfunction(self.function):
+            raise NotImplementedError("Sync generators are not supported")  # TODO
+
+        return ValueDependency(
+            async_callable=self.build_async_callable(),
+            marker_destinations=self.marker_destinations.extract(),
+            body_destinations=self.body_destinations.extract(),
+            dependency_destinations=self.dependency_destinations.extract(),
+        )
 
 
-HandlerWithExceptionsType = TypeVar(
-    "HandlerWithExceptionsType", bound=BaseAsyncHandlerWithArguments
-)
+HandlerType = TypeVar("HandlerType", bound=BaseAsyncHandler)
+
+
+class HandlerBuilder(RunnableBuilder, Generic[HandlerType]):
+    def __init__(
+        self,
+        function: Callable[..., Any],
+        possible_exceptions: list[EventException],
+        sub_dependencies: list[Depends],
+    ) -> None:
+        super().__init__(
+            function=function,
+            possible_exceptions=possible_exceptions,
+            sub_dependencies=sub_dependencies,
+            builder_context=BuilderContext(),
+        )
 
+    def build_handler(self) -> HandlerType:
+        raise NotImplementedError
 
-class HandlerWithExceptionsBuilder(
-    HandlerBuilder[HandlerWithExceptionsType],
-    Generic[HandlerWithExceptionsType],
-):
     @classmethod
-    def build_exceptions(
-        cls, handler: HandlerWithExceptionsType
-    ) -> Iterator[EventException]:
+    def build_exceptions(cls, handler: HandlerType) -> Iterator[EventException]:
         yield from list(handler.possible_exceptions)
         if handler.body_model is None:
             yield handler.zero_arguments_expected_error
         else:
             yield handler.one_argument_expected_error
 
+    @classmethod
+    def build_spec_from_handler(
+        cls,
+        handler: HandlerType,
+        summary: str | None,
+        description: str | None,
+    ) -> HandlerSpec:
+        raise NotImplementedError
 
-class EventHandlerBuilder(HandlerWithExceptionsBuilder[AsyncEventHandler]):
+
+class EventHandlerBuilder(HandlerBuilder[AsyncEventHandler]):
     def parse_return_annotation(self) -> packagers.CodedPackager[Any]:
         annotation = self.signature.return_annotation
         args = get_args(annotation)
 
         if annotation is None:
             return packagers.NoContentPackager()
         elif (  # noqa: WPS337
@@ -153,24 +262,26 @@
             and len(args) == 2
             and isinstance(args[1], packagers.CodedPackager)
         ):
             return args[1]
         return packagers.PydanticPackager(annotation)
 
     def build_handler(self) -> AsyncEventHandler:
-        for parameter in self.signature.parameters.values():
-            self.parse_parameter(parameter)
+        self.parse_parameters()
         ack_packager = self.parse_return_annotation()
 
         return AsyncEventHandler(
             async_callable=self.build_async_callable(),
-            marker_destinations=self.destinations.build_marker_destinations(),
-            body_model=self.destinations.build_body_model(),
-            body_destinations=self.destinations.build_body_destinations(),
-            possible_exceptions=set(self.possible_exceptions),
+            marker_definitions=self.context.build_marker_definitions(),
+            marker_destinations=self.marker_destinations.extract(),
+            body_model=self.context.build_body_model(),
+            body_destinations=self.body_destinations.extract(),
+            dependency_definitions=self.context.build_dependency_definitions(),
+            dependency_destinations=self.dependency_destinations.extract(),
+            possible_exceptions=self.context.possible_exceptions,
             ack_packager=ack_packager,
         )
 
     @classmethod
     def build_spec_from_handler(
         cls,
         handler: AsyncEventHandler,
@@ -183,28 +294,30 @@
             exceptions=list(cls.build_exceptions(handler)),
             ack_code=handler.ack_packager.code,
             ack_body_schema=handler.ack_packager.body_json_schema(),
             event_body_model=handler.body_model,
         )
 
 
-class ConnectHandlerBuilder(HandlerWithExceptionsBuilder[AsyncConnectHandler]):
+class ConnectHandlerBuilder(HandlerBuilder[AsyncConnectHandler]):
     def build_handler(self) -> AsyncConnectHandler:
-        for parameter in self.signature.parameters.values():
-            self.parse_parameter(parameter)
+        self.parse_parameters()
 
         if self.signature.return_annotation is not None:
             raise TypeError("Connection handlers can not return anything")
 
         return AsyncConnectHandler(
             async_callable=self.build_async_callable(),
-            marker_destinations=self.destinations.build_marker_destinations(),
-            body_model=self.destinations.build_body_model(),
-            body_destinations=self.destinations.build_body_destinations(),
-            possible_exceptions=set(self.possible_exceptions),
+            marker_definitions=self.context.build_marker_definitions(),
+            marker_destinations=self.marker_destinations.extract(),
+            body_model=self.context.build_body_model(),
+            body_destinations=self.body_destinations.extract(),
+            dependency_definitions=self.context.build_dependency_definitions(),
+            dependency_destinations=self.dependency_destinations.extract(),
+            possible_exceptions=self.context.possible_exceptions,
         )
 
     @classmethod
     def build_spec_from_handler(
         cls,
         handler: AsyncConnectHandler,
         summary: str | None,
@@ -218,29 +331,31 @@
             ack_body_schema=None,
             event_body_model=handler.body_model,
         )
 
 
 class DisconnectHandlerBuilder(HandlerBuilder[AsyncDisconnectHandler]):
     def build_handler(self) -> AsyncDisconnectHandler:
-        if self.possible_exceptions:
+        if self.context.possible_exceptions:
             raise TypeError("Disconnection handlers can not have possible exceptions")
 
-        for parameter in self.signature.parameters.values():
-            self.parse_parameter(parameter)
+        self.parse_parameters()
 
-        if self.destinations.build_body_model() is not None:
+        if self.context.build_body_model() is not None:
             raise TypeError("Disconnection handlers can not have arguments")
 
         if self.signature.return_annotation is not None:
             raise TypeError("Disconnection handlers can not return anything")
 
         return AsyncDisconnectHandler(
             async_callable=self.build_async_callable(),
-            marker_destinations=self.destinations.build_marker_destinations(),
+            marker_definitions=self.context.build_marker_definitions(),
+            marker_destinations=self.marker_destinations.extract(),
+            dependency_definitions=self.context.build_dependency_definitions(),
+            dependency_destinations=self.dependency_destinations.extract(),
         )
 
     @classmethod
     def build_spec_from_handler(
         cls,
         handler: AsyncDisconnectHandler,
         summary: str | None,
@@ -260,169 +375,7 @@
     "connect": ConnectHandlerBuilder,
     "disconnect": DisconnectHandlerBuilder,
 }
 
 
 def pick_handler_class_by_event_name(event_name: str) -> type[HandlerBuilder[Any]]:
     return EVENT_NAME_TO_HANDLER_BUILDER.get(event_name, EventHandlerBuilder)
-
-
-class EventRouter:
-    def __init__(self) -> None:
-        self.event_handlers: dict[str, tuple[AsyncEventHandler, HandlerSpec]] = {}
-
-    def add_handler(
-        self,
-        event_name: str,
-        handler: AsyncEventHandler,
-        spec: HandlerSpec,
-    ) -> None:
-        self.event_handlers[event_name] = handler, spec
-
-    def on(
-        self,
-        event_name: str,
-        summary: str | None = None,
-        description: str | None = None,
-        exceptions: list[EventException] | None = None,
-    ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
-        handler_builder_class = pick_handler_class_by_event_name(event_name)
-
-        def on_inner(function: Callable[..., Any]) -> Callable[..., Any]:
-            handler = handler_builder_class(
-                function=function,
-                possible_exceptions=exceptions or [],
-            ).build_handler()
-            self.add_handler(
-                event_name=event_name,
-                handler=handler,
-                spec=handler_builder_class.build_spec_from_handler(
-                    handler=handler,
-                    summary=summary,
-                    description=description,
-                ),
-            )
-            return function
-
-        return on_inner
-
-    def on_connect(
-        self,
-        summary: str | None = None,
-        description: str | None = None,
-        exceptions: list[EventException] | None = None,
-    ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
-        return self.on(
-            event_name="connect",
-            summary=summary,
-            description=description,
-            exceptions=exceptions,
-        )
-
-    def on_disconnect(
-        self,
-        summary: str | None = None,
-        description: str | None = None,
-        exceptions: list[EventException] | None = None,
-    ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
-        return self.on(
-            event_name="disconnect",
-            summary=summary,
-            description=description,
-            exceptions=exceptions,
-        )
-
-    def on_other(
-        self,
-        summary: str | None = None,
-        description: str | None = None,
-        exceptions: list[EventException] | None = None,
-    ) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
-        return self.on(
-            event_name="*",
-            summary=summary,
-            description=description,
-            exceptions=exceptions,
-        )
-
-    def include_router(self, router: EventRouter) -> None:
-        for event_name, (handler, spec) in router.event_handlers.items():
-            self.add_handler(event_name, handler, spec)
-
-
-class TMEXIO(EventRouter):
-    def __init__(
-        self,
-        client_manager: socketio.AsyncManager | None = None,
-        logger: bool | Logger = False,
-        engineio_logger: bool | Logger = False,
-        namespaces: Literal["*"] | list[str] | None = None,
-        always_connect: bool = False,
-        serializer: type[Packet] = Packet,
-        **kwargs: Any,
-    ) -> None:
-        super().__init__()
-        self.backend = socketio.AsyncServer(
-            client_manager=client_manager,
-            logger=logger,
-            namespaces=namespaces,
-            always_connect=always_connect,
-            serializer=serializer,
-            engineio_logger=engineio_logger,
-            **kwargs,
-        )
-        self.server = AsyncServer(backend=self.backend)
-
-    def add_handler(
-        self,
-        event_name: str,
-        handler: AsyncEventHandler,
-        spec: HandlerSpec,
-    ) -> None:
-        super().add_handler(event_name=event_name, handler=handler, spec=spec)
-
-        if event_name == "connect":
-
-            async def add_handler_inner(
-                sid: str, _environ: Any, auth: DataType = None
-            ) -> DataOrTuple:
-                return await handler(ClientEvent(self.server, "connect", sid, auth))
-
-        elif event_name == "disconnect":
-
-            async def add_handler_inner(sid: str) -> DataOrTuple:  # type: ignore[misc]
-                return await handler(ClientEvent(self.server, "disconnect", sid))
-
-        elif event_name == "*":
-
-            async def add_handler_inner(  # type: ignore[misc]
-                event: str, sid: str, *args: DataType
-            ) -> DataOrTuple:
-                return await handler(ClientEvent(self.server, event, sid, *args))
-
-        else:
-
-            async def add_handler_inner(sid: str, *args: DataType) -> DataOrTuple:  # type: ignore[misc]
-                return await handler(ClientEvent(self.server, event_name, sid, *args))
-
-        self.backend.on(
-            event=event_name,
-            handler=add_handler_inner,
-            namespace="/",  # TODO support for multiple namespaces
-        )
-
-    def build_asgi_app(
-        self,
-        other_asgi_app: ASGIAppProtocol | None = None,
-        static_files: dict[str, str] | None = None,
-        socketio_path: str | None = "socket.io",
-        on_startup: Callable[[], Awaitable[None]] | None = None,
-        on_shutdown: Callable[[], Awaitable[None]] | None = None,
-    ) -> ASGIAppProtocol:
-        return socketio.ASGIApp(  # type: ignore[no-any-return]
-            socketio_server=self.backend,
-            other_asgi_app=other_asgi_app,
-            static_files=static_files,
-            socketio_path=socketio_path,
-            on_startup=on_startup,
-            on_shutdown=on_shutdown,
-        )
```

### Comparing `tmexio-0.0.1/tmexio/markers.py` & `tmexio-0.1.0/tmexio/markers.py`

 * *Files identical despite different names*

### Comparing `tmexio-0.0.1/tmexio/packagers.py` & `tmexio-0.1.0/tmexio/packagers.py`

 * *Files identical despite different names*

### Comparing `tmexio-0.0.1/tmexio/server.py` & `tmexio-0.1.0/tmexio/server.py`

 * *Files identical despite different names*

### Comparing `tmexio-0.0.1/tmexio/types.py` & `tmexio-0.1.0/tmexio/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections.abc import Awaitable, Callable, MutableMapping
 from typing import Any, Protocol
 
 AnyKwargs = dict[str, Any]
 AnyCallable = Callable[..., Any]
+DependencyCacheKey = AnyCallable
 
 DataType = None | int | str | bytes | dict["DataType", "DataType"] | list["DataType"]
 DataOrTuple = DataType | tuple[DataType, ...]
 
 
 class CallbackProtocol(Protocol):
     def __call__(self, *args: DataType) -> None:
```

### Comparing `tmexio-0.0.1/PKG-INFO` & `tmexio-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmexio
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python framework for building SocketIO applications with typing, dependency injection and more
 Author: niqzart
 Author-email: niqzart@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asgiref (>=3.8.1,<4.0.0)
```

