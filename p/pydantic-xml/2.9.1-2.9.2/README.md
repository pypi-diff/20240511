# Comparing `tmp/pydantic_xml-2.9.1.tar.gz` & `tmp/pydantic_xml-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xml-2.9.1.tar", max compression
+gzip compressed data, was "pydantic_xml-2.9.2.tar", max compression
```

## Comparing `pydantic_xml-2.9.1.tar` & `pydantic_xml-2.9.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1211 2024-04-12 14:01:50.246366 pydantic_xml-2.9.1/LICENSE
--rw-r--r--   0        0        0     3218 2024-04-12 14:01:50.246366 pydantic_xml-2.9.1/README.rst
--rw-r--r--   0        0        0      453 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/__init__.py
--rw-r--r--   0        0        0      489 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/config.py
--rw-r--r--   0        0        0      134 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/element/__init__.py
--rw-r--r--   0        0        0    17277 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/element/element.py
--rw-r--r--   0        0        0      394 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/element/native/__init__.py
--rw-r--r--   0        0        0     1948 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/element/native/lxml.py
--rw-r--r--   0        0        0     1322 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/element/native/std.py
--rw-r--r--   0        0        0      413 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/element/utils.py
--rw-r--r--   0        0        0      712 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/errors.py
--rw-r--r--   0        0        0    15400 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/model.py
--rw-r--r--   0        0        0     3702 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/mypy.py
--rw-r--r--   0        0        0        0 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/py.typed
--rw-r--r--   0        0        0       36 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/__init__.py
--rw-r--r--   0        0        0      151 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/__init__.py
--rw-r--r--   0        0        0     4121 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/heterogeneous.py
--rw-r--r--   0        0        0     4486 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/homogeneous.py
--rw-r--r--   0        0        0      460 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/is_instance.py
--rw-r--r--   0        0        0     5761 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/mapping.py
--rw-r--r--   0        0        0    15611 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/model.py
--rw-r--r--   0        0        0     6731 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/primitive.py
--rw-r--r--   0        0        0     2858 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/raw.py
--rw-r--r--   0        0        0     5287 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/tagged_union.py
--rw-r--r--   0        0        0     1047 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/tuple.py
--rw-r--r--   0        0        0     1428 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/typed_mapping.py
--rw-r--r--   0        0        0     5880 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/union.py
--rw-r--r--   0        0        0     2996 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/wrapper.py
--rw-r--r--   0        0        0    10871 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/serializer.py
--rw-r--r--   0        0        0      375 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/typedefs.py
--rw-r--r--   0        0        0     3978 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/utils.py
--rw-r--r--   0        0        0     2149 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pyproject.toml
--rw-r--r--   0        0        0     5010 1970-01-01 00:00:00.000000 pydantic_xml-2.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-18 19:31:10.819750 pydantic_xml-2.9.2/LICENSE
+-rw-r--r--   0        0        0     3218 2024-04-18 19:31:10.819750 pydantic_xml-2.9.2/README.rst
+-rw-r--r--   0        0        0      453 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/__init__.py
+-rw-r--r--   0        0        0      489 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/config.py
+-rw-r--r--   0        0        0      134 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/element/__init__.py
+-rw-r--r--   0        0        0    17277 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/element/element.py
+-rw-r--r--   0        0        0      394 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/element/native/__init__.py
+-rw-r--r--   0        0        0     1948 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/element/native/lxml.py
+-rw-r--r--   0        0        0     1322 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/element/native/std.py
+-rw-r--r--   0        0        0      413 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/element/utils.py
+-rw-r--r--   0        0        0      712 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/errors.py
+-rw-r--r--   0        0        0    15400 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/model.py
+-rw-r--r--   0        0        0     4027 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/mypy.py
+-rw-r--r--   0        0        0        0 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/py.typed
+-rw-r--r--   0        0        0       36 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/factories/__init__.py
+-rw-r--r--   0        0        0     4121 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/factories/heterogeneous.py
+-rw-r--r--   0        0        0     4486 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/factories/homogeneous.py
+-rw-r--r--   0        0        0      460 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/factories/is_instance.py
+-rw-r--r--   0        0        0     5761 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/factories/mapping.py
+-rw-r--r--   0        0        0    15611 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/factories/model.py
+-rw-r--r--   0        0        0     6731 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/factories/primitive.py
+-rw-r--r--   0        0        0     2858 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/factories/raw.py
+-rw-r--r--   0        0        0     5287 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/factories/tagged_union.py
+-rw-r--r--   0        0        0     1047 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/factories/tuple.py
+-rw-r--r--   0        0        0     1428 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/factories/typed_mapping.py
+-rw-r--r--   0        0        0     5880 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/factories/union.py
+-rw-r--r--   0        0        0     2996 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/factories/wrapper.py
+-rw-r--r--   0        0        0    10871 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/serializers/serializer.py
+-rw-r--r--   0        0        0      375 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/typedefs.py
+-rw-r--r--   0        0        0     3978 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pydantic_xml/utils.py
+-rw-r--r--   0        0        0     2149 2024-04-18 19:31:10.823750 pydantic_xml-2.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5010 1970-01-01 00:00:00.000000 pydantic_xml-2.9.2/PKG-INFO
```

### Comparing `pydantic_xml-2.9.1/LICENSE` & `pydantic_xml-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/README.rst` & `pydantic_xml-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/element/element.py` & `pydantic_xml-2.9.2/pydantic_xml/element/element.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/element/native/lxml.py` & `pydantic_xml-2.9.2/pydantic_xml/element/native/lxml.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/element/native/std.py` & `pydantic_xml-2.9.2/pydantic_xml/element/native/std.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/errors.py` & `pydantic_xml-2.9.2/pydantic_xml/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/model.py` & `pydantic_xml-2.9.2/pydantic_xml/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/mypy.py` & `pydantic_xml-2.9.2/pydantic_xml/mypy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from typing import Callable, Optional, Tuple, Union
 
 from mypy import nodes
 from mypy.plugin import ClassDefContext, FunctionContext, Plugin, Type
 from pydantic.mypy import PydanticModelTransformer, PydanticPlugin
 
+MODEL_METACLASS_FULLNAME = 'pydantic_xml.model.XmlModelMeta'
 ATTR_FULLNAME = 'pydantic_xml.model.attr'
 ELEMENT_FULLNAME = 'pydantic_xml.model.element'
 WRAPPED_FULLNAME = 'pydantic_xml.model.wrapped'
 ENTITIES_FULLNAME = (ATTR_FULLNAME, ELEMENT_FULLNAME, WRAPPED_FULLNAME)
 
 
 def plugin(version: str) -> type[Plugin]:
     return PydanticXmlPlugin
 
 
 class PydanticXmlPlugin(PydanticPlugin):
+    def get_metaclass_hook(self, fullname: str) -> Optional[Callable[[ClassDefContext], None]]:
+        if fullname == MODEL_METACLASS_FULLNAME:
+            return self._pydantic_model_metaclass_marker_callback
+        return super().get_metaclass_hook(fullname)
+
     def get_function_hook(self, fullname: str) -> Optional[Callable[[FunctionContext], Type]]:
         sym = self.lookup_fully_qualified(fullname)
         if sym and sym.fullname == ATTR_FULLNAME:
             return self._attribute_callback
         elif sym and sym.fullname == ELEMENT_FULLNAME:
             return self._element_callback
         elif sym and sym.fullname == WRAPPED_FULLNAME:
```

### Comparing `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/heterogeneous.py` & `pydantic_xml-2.9.2/pydantic_xml/serializers/factories/heterogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/homogeneous.py` & `pydantic_xml-2.9.2/pydantic_xml/serializers/factories/homogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/mapping.py` & `pydantic_xml-2.9.2/pydantic_xml/serializers/factories/mapping.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/model.py` & `pydantic_xml-2.9.2/pydantic_xml/serializers/factories/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/primitive.py` & `pydantic_xml-2.9.2/pydantic_xml/serializers/factories/primitive.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/raw.py` & `pydantic_xml-2.9.2/pydantic_xml/serializers/factories/raw.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/tagged_union.py` & `pydantic_xml-2.9.2/pydantic_xml/serializers/factories/tagged_union.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/tuple.py` & `pydantic_xml-2.9.2/pydantic_xml/serializers/factories/tuple.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/typed_mapping.py` & `pydantic_xml-2.9.2/pydantic_xml/serializers/factories/typed_mapping.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/union.py` & `pydantic_xml-2.9.2/pydantic_xml/serializers/factories/union.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/wrapper.py` & `pydantic_xml-2.9.2/pydantic_xml/serializers/factories/wrapper.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/serializers/serializer.py` & `pydantic_xml-2.9.2/pydantic_xml/serializers/serializer.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pydantic_xml/utils.py` & `pydantic_xml-2.9.2/pydantic_xml/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.1/pyproject.toml` & `pydantic_xml-2.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xml"
-version = "2.9.1"
+version = "2.9.2"
 description = "pydantic xml extension"
 authors = ["Dmitry Pershin <dapper1291@gmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 homepage = "https://github.com/dapper91/pydantic-xml"
 repository = "https://github.com/dapper91/pydantic-xml"
 documentation = "https://pydantic-xml.readthedocs.io"
```

### Comparing `pydantic_xml-2.9.1/PKG-INFO` & `pydantic_xml-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-xml
-Version: 2.9.1
+Version: 2.9.2
 Summary: pydantic xml extension
 Home-page: https://github.com/dapper91/pydantic-xml
 License: Unlicense
 Keywords: pydantic,xml,serialization,deserialization,lxml
 Author: Dmitry Pershin
 Author-email: dapper1291@gmail.com
 Requires-Python: >=3.8
```

