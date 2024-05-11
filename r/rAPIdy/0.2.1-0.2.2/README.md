# Comparing `tmp/rapidy-0.2.1.tar.gz` & `tmp/rapidy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidy-0.2.1.tar", max compression
+gzip compressed data, was "rapidy-0.2.2.tar", max compression
```

## Comparing `rapidy-0.2.1.tar` & `rapidy-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1079 2024-04-22 08:38:32.528691 rapidy-0.2.1/LICENSE
--rw-r--r--   0        0        0    19477 2024-05-03 20:23:55.332530 rapidy-0.2.1/README.md
--rw-r--r--   0        0        0     5921 2024-05-07 20:37:17.601436 rapidy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7822 2024-05-07 20:28:28.108186 rapidy-0.2.1/rapidy/__init__.py
--rw-r--r--   0        0        0    13191 2024-05-07 20:12:13.909384 rapidy-0.2.1/rapidy/_annotation_container.py
--rw-r--r--   0        0        0     9154 2024-04-22 03:22:22.724232 rapidy-0.2.1/rapidy/_annotation_extractor.py
--rw-r--r--   0        0        0     4382 2024-04-22 08:38:32.528691 rapidy-0.2.1/rapidy/_client_errors.py
--rw-r--r--   0        0        0     9279 2024-05-01 21:05:46.329849 rapidy-0.2.1/rapidy/_extractors.py
--rw-r--r--   0        0        0     6045 2024-05-07 20:12:13.909384 rapidy-0.2.1/rapidy/_fields.py
--rw-r--r--   0        0        0      627 2024-05-01 21:05:46.329849 rapidy-0.2.1/rapidy/_parsers.py
--rw-r--r--   0        0        0      474 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/_request_params_base.py
--rw-r--r--   0        0        0     2565 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/_validators.py
--rw-r--r--   0        0        0      614 2024-04-22 08:38:32.528691 rapidy-0.2.1/rapidy/_version.py
--rw-r--r--   0        0        0     1011 2024-05-07 20:13:27.764531 rapidy-0.2.1/rapidy/_web_request_validation.py
--rw-r--r--   0        0        0      285 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/constants.py
--rw-r--r--   0        0        0     3496 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/hdrs.py
--rw-r--r--   0        0        0      290 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/media_types.py
--rw-r--r--   0        0        0      169 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/mypy/__init__.py
--rw-r--r--   0        0        0      929 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/mypy/_api_errors.py
--rw-r--r--   0        0        0     4463 2024-05-01 21:05:46.329849 rapidy-0.2.1/rapidy/mypy/_type_helpers.py
--rw-r--r--   0        0        0      146 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/mypy/_version.py
--rw-r--r--   0        0        0     5485 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/mypy/plugin.py
--rw-r--r--   0        0        0        7 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/py.typed
--rw-r--r--   0        0        0    11108 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/request_params.py
--rw-r--r--   0        0        0      218 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/streams.py
--rw-r--r--   0        0        0     2363 2024-05-02 21:51:29.755968 rapidy-0.2.1/rapidy/typedefs.py
--rw-r--r--   0        0        0     9009 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/web.py
--rw-r--r--   0        0        0     7956 2024-05-07 20:12:13.909384 rapidy-0.2.1/rapidy/web_app.py
--rw-r--r--   0        0        0    12391 2024-05-02 21:51:29.755968 rapidy-0.2.1/rapidy/web_exceptions.py
--rw-r--r--   0        0        0      140 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/web_middlewares.py
--rw-r--r--   0        0        0      130 2024-04-22 03:22:22.725232 rapidy-0.2.1/rapidy/web_request.py
--rw-r--r--   0        0        0     2483 2024-05-02 22:30:37.510688 rapidy-0.2.1/rapidy/web_response.py
--rw-r--r--   0        0        0     2926 2024-04-22 03:22:22.726232 rapidy-0.2.1/rapidy/web_routedef.py
--rw-r--r--   0        0        0      350 2024-04-22 03:22:22.726232 rapidy-0.2.1/rapidy/web_runner.py
--rw-r--r--   0        0        0     5801 2024-05-07 20:12:13.910385 rapidy-0.2.1/rapidy/web_urldispatcher.py
--rw-r--r--   0        0        0    20927 1970-01-01 00:00:00.000000 rapidy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-22 08:38:32.528691 rapidy-0.2.2/LICENSE
+-rw-r--r--   0        0        0    19477 2024-05-03 20:23:55.332530 rapidy-0.2.2/README.md
+-rw-r--r--   0        0        0     5921 2024-05-11 11:47:16.998239 rapidy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7822 2024-05-11 11:37:18.929264 rapidy-0.2.2/rapidy/__init__.py
+-rw-r--r--   0        0        0    12644 2024-05-09 17:07:44.037954 rapidy-0.2.2/rapidy/_annotation_container.py
+-rw-r--r--   0        0        0     9154 2024-04-22 03:22:22.724232 rapidy-0.2.2/rapidy/_annotation_extractor.py
+-rw-r--r--   0        0        0     4382 2024-04-22 08:38:32.528691 rapidy-0.2.2/rapidy/_client_errors.py
+-rw-r--r--   0        0        0     9279 2024-05-01 21:05:46.329849 rapidy-0.2.2/rapidy/_extractors.py
+-rw-r--r--   0        0        0     5893 2024-05-11 11:36:36.006548 rapidy-0.2.2/rapidy/_fields.py
+-rw-r--r--   0        0        0      627 2024-05-01 21:05:46.329849 rapidy-0.2.2/rapidy/_parsers.py
+-rw-r--r--   0        0        0      474 2024-04-22 03:22:22.725232 rapidy-0.2.2/rapidy/_request_params_base.py
+-rw-r--r--   0        0        0     2565 2024-04-22 03:22:22.725232 rapidy-0.2.2/rapidy/_validators.py
+-rw-r--r--   0        0        0      614 2024-04-22 08:38:32.528691 rapidy-0.2.2/rapidy/_version.py
+-rw-r--r--   0        0        0     3940 2024-05-11 11:27:07.046451 rapidy-0.2.2/rapidy/_web_request_validation.py
+-rw-r--r--   0        0        0      285 2024-04-22 03:22:22.725232 rapidy-0.2.2/rapidy/constants.py
+-rw-r--r--   0        0        0     3496 2024-04-22 03:22:22.725232 rapidy-0.2.2/rapidy/hdrs.py
+-rw-r--r--   0        0        0      290 2024-04-22 03:22:22.725232 rapidy-0.2.2/rapidy/media_types.py
+-rw-r--r--   0        0        0      169 2024-04-22 03:22:22.725232 rapidy-0.2.2/rapidy/mypy/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-22 03:22:22.725232 rapidy-0.2.2/rapidy/mypy/_api_errors.py
+-rw-r--r--   0        0        0     4463 2024-05-01 21:05:46.329849 rapidy-0.2.2/rapidy/mypy/_type_helpers.py
+-rw-r--r--   0        0        0      146 2024-04-22 03:22:22.725232 rapidy-0.2.2/rapidy/mypy/_version.py
+-rw-r--r--   0        0        0     5485 2024-04-22 03:22:22.725232 rapidy-0.2.2/rapidy/mypy/plugin.py
+-rw-r--r--   0        0        0        7 2024-04-22 03:22:22.725232 rapidy-0.2.2/rapidy/py.typed
+-rw-r--r--   0        0        0    11213 2024-05-11 11:36:36.006548 rapidy-0.2.2/rapidy/request_params.py
+-rw-r--r--   0        0        0      218 2024-04-22 03:22:22.725232 rapidy-0.2.2/rapidy/streams.py
+-rw-r--r--   0        0        0     2363 2024-05-02 21:51:29.755968 rapidy-0.2.2/rapidy/typedefs.py
+-rw-r--r--   0        0        0     9090 2024-05-09 18:46:07.068061 rapidy-0.2.2/rapidy/web.py
+-rw-r--r--   0        0        0     4412 2024-05-11 09:00:26.861990 rapidy-0.2.2/rapidy/web_app.py
+-rw-r--r--   0        0        0     4297 2024-05-11 09:00:26.861990 rapidy-0.2.2/rapidy/web_exceptions.py
+-rw-r--r--   0        0        0      772 2024-05-09 17:07:44.037954 rapidy-0.2.2/rapidy/web_middlewares.py
+-rw-r--r--   0        0        0      130 2024-04-22 03:22:22.725232 rapidy-0.2.2/rapidy/web_request.py
+-rw-r--r--   0        0        0      183 2024-05-11 09:00:26.861990 rapidy-0.2.2/rapidy/web_response.py
+-rw-r--r--   0        0        0     2926 2024-04-22 03:22:22.726232 rapidy-0.2.2/rapidy/web_routedef.py
+-rw-r--r--   0        0        0      350 2024-04-22 03:22:22.726232 rapidy-0.2.2/rapidy/web_runner.py
+-rw-r--r--   0        0        0     4005 2024-05-09 17:07:44.037954 rapidy-0.2.2/rapidy/web_urldispatcher.py
+-rw-r--r--   0        0        0    20927 1970-01-01 00:00:00.000000 rapidy-0.2.2/PKG-INFO
```

### Comparing `rapidy-0.2.1/LICENSE` & `rapidy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/README.md` & `rapidy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/pyproject.toml` & `rapidy-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rAPIdy"
-version = "0.2.1"
+version = "0.2.2"
 description = "rAPIdy - write quickly - write beautifully"
 authors = [
     "Daniil Grois <daniil.grois@gmail.com>",
     "Lev Zaplatin <lev@zaplatin.dev>",
 ]
 keywords = [
     "rAPIdy",
```

### Comparing `rapidy-0.2.1/rapidy/__init__.py` & `rapidy-0.2.2/rapidy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 
 from typing import Tuple, TYPE_CHECKING
 
 from aiohttp.client import (
     BaseConnector as BaseConnector,
     ClientConnectionError as ClientConnectionError,
     ClientConnectorCertificateError as ClientConnectorCertificateError,
```

### Comparing `rapidy-0.2.1/rapidy/_annotation_container.py` & `rapidy-0.2.2/rapidy/_annotation_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,23 @@
 import inspect
 from abc import ABC, abstractmethod
-from enum import Enum
 from types import FunctionType
 from typing import Any, Dict, Iterator, Optional, Set, Type, Union
 
 from aiohttp.web_request import Request
 from typing_extensions import get_args
 
 from rapidy._annotation_extractor import extract_handler_attr_annotations, NotParameterError
 from rapidy._client_errors import _create_handler_attr_info_msg, _create_handler_info_msg, ExtractError
 from rapidy._fields import ModelField
 from rapidy._validators import validate_request_param_data
 from rapidy.request_params import create_param_model_field_by_request_param, ParamFieldInfo, ParamType, ValidateType
 from rapidy.typedefs import Handler, MethodHandler, Middleware, NoArgAnyCallable, ValidateReturn
 
 
-# FIXME: I don't like this solution as it is being used now.
-#  We need to mark handlers somehow so that we don't have
-#  to check them every time for issubclass(handler, AbstractView) or isinstance(handler, FunctionType).
-class HandlerEnumType(str, Enum):
-    func = 'func'
-    method = 'method'
-    middleware = 'middleware'
-
-    @property
-    def is_func(self) -> bool:
-        return self == self.func
-
-
 class AnnotationContainerAddFieldError(TypeError):
     pass
 
 
 class RequestFieldAlreadyExistError(Exception):
     _base_err_msg = (
         'Error during attribute definition in the handler - request param defined twice.'
@@ -246,21 +232,19 @@
     raise  # pragma: no cover
 
 
 class AnnotationContainer:
     def __init__(
             self,
             handler: Union[Handler, MethodHandler, Middleware],
-            handler_type: HandlerEnumType,
     ) -> None:
         self._handler = handler
         self._params: Dict[str, ParamAnnotationContainer] = {}
         self._request_exists: bool = False
         self._request_param_name: Optional[str] = None
-        self._handler_type = handler_type
 
     def __iter__(self) -> Iterator[ParamAnnotationContainer]:
         for param_container in self._params.values():
             if param_container:
                 yield param_container
 
     def set_request_field(self, request_param_name: str) -> None:
@@ -332,30 +316,30 @@
         )
         self._params[param_type] = param_container
         return param_container
 
 
 def create_annotation_container(
         handler: Union[FunctionType, Middleware],
-        handler_type: HandlerEnumType,
+        is_func_handler: bool = False,
 ) -> AnnotationContainer:
-    container = AnnotationContainer(handler=handler, handler_type=handler_type)
+    container = AnnotationContainer(handler=handler)
 
     endpoint_signature = inspect.signature(handler)
     signature_params = endpoint_signature.parameters.items()
 
     num_of_extracted_signatures = 0
 
     for param_name, param in signature_params:
         num_of_extracted_signatures += 1
 
         try:
             annotation, param_field_info, default = extract_handler_attr_annotations(param=param, handler=handler)
         except NotParameterError:
-            if handler_type.is_func:
+            if is_func_handler:
                 if not get_args(param.annotation):
                     # FIXME: Fix the processing logic for the 1-st attribute to return a specific error
                     if issubclass(Request, param.annotation) or num_of_extracted_signatures == 1:
                         container.set_request_field(param_name)
 
             continue
```

### Comparing `rapidy-0.2.1/rapidy/_annotation_extractor.py` & `rapidy-0.2.2/rapidy/_annotation_extractor.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/rapidy/_client_errors.py` & `rapidy-0.2.2/rapidy/_client_errors.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/rapidy/_extractors.py` & `rapidy-0.2.2/rapidy/_extractors.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/rapidy/_fields.py` & `rapidy-0.2.2/rapidy/_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,18 +29,14 @@
             default=default,
             default_factory=default_factory,
             **field_info_kwargs,
         )
         if PYDANTIC_V1:
             self._validate()  # check specify both default and default_factory
 
-        extractor = getattr(self, 'extractor') or getattr(self.__class__, 'extractor', None)  # noqa: B009
-        if not extractor:
-            raise
-
 
 if PYDANTIC_V1:  # noqa: C901
     from pydantic import BaseConfig  # noqa: WPS433
     from pydantic.class_validators import Validator as Validator  # noqa: WPS433
     from pydantic.fields import ModelField as PydanticModelField  # noqa: WPS433
     from pydantic.schema import get_annotation_from_field_info  # noqa: WPS433
```

### Comparing `rapidy-0.2.1/rapidy/_parsers.py` & `rapidy-0.2.2/rapidy/_parsers.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/rapidy/_validators.py` & `rapidy-0.2.2/rapidy/_validators.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/rapidy/_version.py` & `rapidy-0.2.2/rapidy/_version.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/rapidy/hdrs.py` & `rapidy-0.2.2/rapidy/hdrs.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/rapidy/mypy/_api_errors.py` & `rapidy-0.2.2/rapidy/mypy/_api_errors.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/rapidy/mypy/_type_helpers.py` & `rapidy-0.2.2/rapidy/mypy/_type_helpers.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/rapidy/mypy/plugin.py` & `rapidy-0.2.2/rapidy/mypy/plugin.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/rapidy/request_params.py` & `rapidy-0.2.2/rapidy/request_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,14 +140,16 @@
             self,
             default: Any = Undefined,
             *,
             default_factory: Optional[NoArgAnyCallable] = None,
             body_max_size: Optional[int] = None,
             **field_info_kwargs: Any,
     ) -> None:
+        # FIXME:
+        #  now must be called after the definition of extractor in the inheritor class.
         self.body_max_size = body_max_size or MAX_BODY_SIZE
 
         self.extractor = partial(self.extractor, max_size=self.body_max_size)
 
         super().__init__(default=default, default_factory=default_factory, **field_info_kwargs)
```

### Comparing `rapidy-0.2.1/rapidy/typedefs.py` & `rapidy-0.2.2/rapidy/typedefs.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/rapidy/web.py` & `rapidy-0.2.2/rapidy/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
     HTTPTooManyRequests as HTTPTooManyRequests,
     HTTPUnauthorized as HTTPUnauthorized,
     HTTPUnavailableForLegalReasons as HTTPUnavailableForLegalReasons,
     HTTPUnprocessableEntity as HTTPUnprocessableEntity,
     HTTPUnsupportedMediaType as HTTPUnsupportedMediaType,
     HTTPUpgradeRequired as HTTPUpgradeRequired,
     HTTPUseProxy as HTTPUseProxy,
+    HTTPValidationFailure as HTTPValidationFailure,
     HTTPVariantAlsoNegotiates as HTTPVariantAlsoNegotiates,
     HTTPVersionNotSupported as HTTPVersionNotSupported,
 )
 from rapidy.web_middlewares import middleware as middleware, normalize_path_middleware as normalize_path_middleware
 from rapidy.web_request import BaseRequest as BaseRequest, FileField as FileField, Request as Request
 from rapidy.web_response import (
     ContentCoding as ContentCoding,
@@ -202,14 +203,15 @@
     'HTTPServiceUnavailable',
     'HTTPSuccessful',
     'HTTPTemporaryRedirect',
     'HTTPTooManyRequests',
     'HTTPUnauthorized',
     'HTTPUnavailableForLegalReasons',
     'HTTPUnprocessableEntity',
+    'HTTPValidationFailure',
     'HTTPUnsupportedMediaType',
     'HTTPUpgradeRequired',
     'HTTPUseProxy',
     'HTTPVariantAlsoNegotiates',
     'HTTPVersionNotSupported',
     # web_fileresponse
     'FileResponse',
```

### Comparing `rapidy-0.2.1/rapidy/web_routedef.py` & `rapidy-0.2.2/rapidy/web_routedef.py`

 * *Files identical despite different names*

### Comparing `rapidy-0.2.1/PKG-INFO` & `rapidy-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rAPIdy
-Version: 0.2.1
+Version: 0.2.2
 Summary: rAPIdy - write quickly - write beautifully
 License: MIT
 Keywords: rAPIdy,aiohttp,pydantic,api,fast,http server,Daniil Grois,Lev Zaplatin
 Author: Daniil Grois
 Author-email: daniil.grois@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
```

