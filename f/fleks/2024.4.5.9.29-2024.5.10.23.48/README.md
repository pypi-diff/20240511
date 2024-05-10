# Comparing `tmp/fleks-2024.4.5.9.29.tar.gz` & `tmp/fleks-2024.5.10.23.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleks-2024.4.5.9.29.tar", last modified: Fri Apr  5 09:29:16 2024, max compression
+gzip compressed data, was "fleks-2024.5.10.23.48.tar", last modified: Fri May 10 23:48:08 2024, max compression
```

## Comparing `fleks-2024.4.5.9.29.tar` & `fleks-2024.5.10.23.48.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.720915 fleks-2024.4.5.9.29/
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-05 09:29:16.720915 fleks-2024.4.5.9.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-05 09:29:16.720915 fleks-2024.4.5.9.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.712915 fleks-2024.4.5.9.29/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.716915 fleks-2024.4.5.9.29/src/fleks/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 09:29:14.000000 fleks-2024.4.5.9.29/src/fleks/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.716915 fleks-2024.4.5.9.29/src/fleks/app/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.716915 fleks-2024.4.5.9.29/src/fleks/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/cli/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-05 09:28:39.000000 fleks-2024.4.5.9.29/src/fleks/cli/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/cli/root_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.720915 fleks-2024.4.5.9.29/src/fleks/meta/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/meta/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-05 09:28:39.000000 fleks-2024.4.5.9.29/src/fleks/meta/oop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.720915 fleks-2024.4.5.9.29/src/fleks/util/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/util/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-05 09:28:39.000000 fleks-2024.4.5.9.29/src/fleks/util/lme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-05 09:28:05.000000 fleks-2024.4.5.9.29/src/fleks/util/tagging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-05 09:28:39.000000 fleks-2024.4.5.9.29/src/fleks/util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:29:16.720915 fleks-2024.4.5.9.29/src/fleks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-05 09:29:16.000000 fleks-2024.4.5.9.29/src/fleks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-05 09:29:16.000000 fleks-2024.4.5.9.29/src/fleks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:29:16.000000 fleks-2024.4.5.9.29/src/fleks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:29:16.000000 fleks-2024.4.5.9.29/src/fleks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-05 09:29:16.000000 fleks-2024.4.5.9.29/src/fleks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 09:29:16.000000 fleks-2024.4.5.9.29/src/fleks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:48:08.677898 fleks-2024.5.10.23.48/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-10 23:48:08.677898 fleks-2024.5.10.23.48/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-10 23:48:08.677898 fleks-2024.5.10.23.48/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:48:08.669898 fleks-2024.5.10.23.48/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:48:08.673898 fleks-2024.5.10.23.48/src/fleks/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 23:48:06.000000 fleks-2024.5.10.23.48/src/fleks/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:48:08.673898 fleks-2024.5.10.23.48/src/fleks/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:48:08.673898 fleks-2024.5.10.23.48/src/fleks/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/cli/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-10 23:47:30.000000 fleks-2024.5.10.23.48/src/fleks/cli/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/cli/root_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:48:08.673898 fleks-2024.5.10.23.48/src/fleks/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/meta/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-05-10 23:47:30.000000 fleks-2024.5.10.23.48/src/fleks/meta/oop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:48:08.673898 fleks-2024.5.10.23.48/src/fleks/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/util/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/util/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-10 23:47:30.000000 fleks-2024.5.10.23.48/src/fleks/util/lme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-10 23:46:55.000000 fleks-2024.5.10.23.48/src/fleks/util/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-10 23:47:30.000000 fleks-2024.5.10.23.48/src/fleks/util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:48:08.677898 fleks-2024.5.10.23.48/src/fleks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-10 23:48:08.000000 fleks-2024.5.10.23.48/src/fleks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-10 23:48:08.000000 fleks-2024.5.10.23.48/src/fleks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:48:08.000000 fleks-2024.5.10.23.48/src/fleks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:48:08.000000 fleks-2024.5.10.23.48/src/fleks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-10 23:48:08.000000 fleks-2024.5.10.23.48/src/fleks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 23:48:08.000000 fleks-2024.5.10.23.48/src/fleks.egg-info/top_level.txt
```

### Comparing `fleks-2024.4.5.9.29/PKG-INFO` & `fleks-2024.5.10.23.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleks
-Version: 2024.4.5.9.29
+Version: 2024.5.10.23.48
 Summary: Python application framework
 Home-page: https://github.com/elo-enterprises/fleks/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/fleks/
 Project-URL: Source, https://github.com/elo-enterprises/fleks/
 Project-URL: Download, https://github.com/elo-enterprises/fleks/#files
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fleks Version: 2024.4.5.9.29 Summary: Python
+Metadata-Version: 2.1 Name: fleks Version: 2024.5.10.23.48 Summary: Python
 application framework Home-page: https://github.com/elo-enterprises/fleks/
 Author: elo License: MIT Project-URL: Documentation, https://github.com/elo-
 enterprises/fleks/ Project-URL: Source, https://github.com/elo-enterprises/
 fleks/ Project-URL: Download, https://github.com/elo-enterprises/fleks/#files
 Platform: any Classifier: Programming Language :: Python Requires-Python: >3.7
 Description-Content-Type: text/markdown Requires-Dist: pydash==7.0.1 Requires-
 Dist: memoized-property==1.0.3 Requires-Dist: pydantic==1.10.11 Requires-Dist:
```

### Comparing `fleks-2024.4.5.9.29/README.md` & `fleks-2024.5.10.23.48/README.md`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.5.9.29/setup.cfg` & `fleks-2024.5.10.23.48/setup.cfg`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.5.9.29/setup.py` & `fleks-2024.5.10.23.48/setup.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.5.9.29/src/fleks/cli/click.py` & `fleks-2024.5.10.23.48/src/fleks/cli/click.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.5.9.29/src/fleks/cli/options.py` & `fleks-2024.5.10.23.48/src/fleks/cli/options.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.5.9.29/src/fleks/cli/root_group.py` & `fleks-2024.5.10.23.48/src/fleks/cli/root_group.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.5.9.29/src/fleks/config.py` & `fleks-2024.5.10.23.48/src/fleks/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,54 +3,64 @@
 
 import pydash
 
 from fleks import models
 from fleks.util import typing
 
 
-class Config(models.BaseModel):
+class ConfProto:
+    def __getitem__(
+        self,
+        key,
+    ):
+        if isinstance(key, (slice,)):
+            start, stop, step = key.start, key.stop, key.step
+            raise Exception("niy")
+        tmp = self.dict(
+            # exclude_unset=True,
+            by_alias=True
+        )
+        try:
+            return tmp[key]
+        except (KeyError, TypeError) as exc:
+            return pydash.get(tmp, key)
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__}['{self.__class__.config_key}']>"
+
+
+from pydantic import ConfigDict
+
+
+class Config(models.BaseModel, ConfProto):
     """ """
 
-    config_key: typing.ClassVar[str] = None
+    config_key: typing.ClassVar[str] = typing.Field(default=None)
     # debug = False
     # parent = None
     # priority = 100
     # override_from_base = True
 
     def __init__(self, **this_config) -> None:
         """ """
         kls_defaults = getattr(self.__class__, "defaults", {})
         super().__init__(**{**kls_defaults, **this_config})
+        # self._bootstrappery=this_config
         # conflicts = []
         # for pname in self.__class__.__properties__:
         #     if pname in called_defaults or pname in kls_defaults:
         #         conflicts.append(pname)
         #         continue
         #     else:
         #         self[pname] = getattr(self, pname)
         # self.resolve_conflicts(conflicts)
 
-    def __getitem__(
-        self,
-        key,
-    ):
-        if isinstance(key, (slice,)):
-            start, stop, step = key.start, key.stop, key.step
-            raise Exception("niy")
-        tmp = self.dict(
-            # exclude_unset=True,
-            by_alias=True
-        )
-        try:
-            return tmp[key]
-        except (KeyError, TypeError) as exc:
-            return pydash.get(tmp, key)
 
-    def __repr__(self):
-        return f"<{self.__class__.__name__}['{self.__class__.config_key}']>"
+class StrictConfig(models.StrictBaseModel, ConfProto):
+    model_config = ConfigDict(strict=True)
 
     # def as_dict(self, **kwargs):
     #     kwargs.update(
     #         # exclude_unset=True,
     #         by_alias=True
     #     )
     #     return self.dict(**kwargs)
```

### Comparing `fleks-2024.4.5.9.29/src/fleks/meta/namespace.py` & `fleks-2024.5.10.23.48/src/fleks/meta/namespace.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.5.9.29/src/fleks/meta/oop.py` & `fleks-2024.5.10.23.48/src/fleks/meta/oop.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.5.9.29/src/fleks/models.py` & `fleks-2024.5.10.23.48/src/fleks/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,40 +38,29 @@
         if callable(getattr(obj, "as_dict", None)):
             return obj.as_dict()
         else:
             enc = self.encoders.get(type(obj), str)
             return enc(obj)
 
 
-def to_json(obj, cls=None, minified=False, indent: int = 2) -> str:
+def to_json(obj, cls=None, minified=False, indent: int = 2, **kwargs) -> str:
     """
     custom version of `json.dumps` to always use custom JSONEncoder
     """
     indent = None if minified else indent
     cls = cls if cls is not None else JSONEncoder
-    return json.dumps(obj, indent=indent, cls=cls)
+    return json.dumps(obj, indent=indent, cls=cls, **kwargs)
 
 
 JSONEncoder.register_encoder(type=map, fxn=list)
 JSONEncoder.register_encoder(type=pathlib.Path, fxn=lambda v: str(v))
 JSONEncoder.register_encoder(type=pathlib.PosixPath, fxn=lambda v: str(v))
 
 
-class BaseModel(typing.BaseModel):
-    """
-    Extends pydantic's BaseModel with better support for
-    things like serialization & dynamic values from properties
-    """
-
-    class Config:
-        arbitrary_types_allowed = True
-        # https://github.com/pydantic/pydantic/discussions/5159
-        frozen = True
-        include: typing.Set[str] = set()
-        exclude: typing.Set[str] = set()
+class MProto(typing.BaseModel):
 
     def json(self, **kwargs):
         """Overrides pydantic for better serialization"""
         return to_json(self.dict(**kwargs))
 
     def items(self):
         """dictionary compatability"""
@@ -145,7 +134,32 @@
         """Overrides pydantic for better serialization"""
         return self._dict(*args, **kwargs)
 
     def __repr__(self):
         return f"<{self.__class__.__name__}[..]>"
 
     __str__ = __repr__
+
+
+class BaseModel(MProto):
+    """
+    Extends pydantic's BaseModel with better support for
+    things like serialization & dynamic values from properties
+    """
+
+    class Config:
+        extra = typing.Extra.allow
+        arbitrary_types_allowed = True
+        # https://github.com/pydantic/pydantic/discussions/5159
+        frozen = True
+        include: typing.Set[str] = set()
+        exclude: typing.Set[str] = set()
+
+
+class StrictBaseModel(MProto):
+    class Config:
+        extra = typing.Extra.forbid
+        arbitrary_types_allowed = False
+        # https://github.com/pydantic/pydantic/discussions/5159
+        frozen = True
+        include: typing.Set[str] = set()
+        exclude: typing.Set[str] = set()
```

### Comparing `fleks-2024.4.5.9.29/src/fleks/plugin.py` & `fleks-2024.5.10.23.48/src/fleks/plugin.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.5.9.29/src/fleks/util/click.py` & `fleks-2024.5.10.23.48/src/fleks/util/click.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.5.9.29/src/fleks/util/lme.py` & `fleks-2024.5.10.23.48/src/fleks/util/lme.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from rich.theme import Theme
 from rich.console import Console
 from rich.logging import RichHandler
 from rich.default_styles import DEFAULT_STYLES
 
 from fleks import constants
 
+from .console import color_disabled, is_notebook
+
 THEME = Theme(
     {
         **DEFAULT_STYLES,
         **{
             "logging.keyword": Style(bold=True, color="yellow"),
             # "logging.level.notset": Style(dim=True),
             "logging.level.debug": Style(color="green"),
@@ -32,15 +34,22 @@
             "log.level": Style.null(),
             "log.time": Style(color="cyan", dim=True),
             "log.message": Style.null(),
             "log.path": Style(dim=True),
         },
     }
 )
-CONSOLE = Console(theme=THEME, stderr=True)
+
+COLOR_SYSTEM = None if any([is_notebook(), color_disabled()]) else "auto"
+CONSOLE = Console(
+    theme=THEME,
+    stderr=True,
+    color_system=COLOR_SYSTEM,
+)
+print = CONSOLE.print
 
 
 def set_global_level(level):
     """
     https://stackoverflow.com/questions/19617355/dynamically-changing-log-level-without-restarting-the-application
     """
     logger = logging.getLogger()
```

### Comparing `fleks-2024.4.5.9.29/src/fleks/util/tagging.py` & `fleks-2024.5.10.23.48/src/fleks/util/tagging.py`

 * *Files identical despite different names*

### Comparing `fleks-2024.4.5.9.29/src/fleks/util/typing.py` & `fleks-2024.5.10.23.48/src/fleks/util/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import typing
 from pathlib import Path as BasePath
 
 from types import *  # noqa
 from typing import *  # noqa
 
-from pydantic import BaseModel, Field, validate_arguments  # noqa
+from pydantic import BaseModel, Extra, Field, validate_arguments  # noqa
 
 validate = validate_arguments
 
 OptionalAny = typing.Optional[typing.Any]
 PathType = type(BasePath())
 
 Bool = bool
```

### Comparing `fleks-2024.4.5.9.29/src/fleks.egg-info/PKG-INFO` & `fleks-2024.5.10.23.48/src/fleks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleks
-Version: 2024.4.5.9.29
+Version: 2024.5.10.23.48
 Summary: Python application framework
 Home-page: https://github.com/elo-enterprises/fleks/
 Author: elo
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/fleks/
 Project-URL: Source, https://github.com/elo-enterprises/fleks/
 Project-URL: Download, https://github.com/elo-enterprises/fleks/#files
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fleks Version: 2024.4.5.9.29 Summary: Python
+Metadata-Version: 2.1 Name: fleks Version: 2024.5.10.23.48 Summary: Python
 application framework Home-page: https://github.com/elo-enterprises/fleks/
 Author: elo License: MIT Project-URL: Documentation, https://github.com/elo-
 enterprises/fleks/ Project-URL: Source, https://github.com/elo-enterprises/
 fleks/ Project-URL: Download, https://github.com/elo-enterprises/fleks/#files
 Platform: any Classifier: Programming Language :: Python Requires-Python: >3.7
 Description-Content-Type: text/markdown Requires-Dist: pydash==7.0.1 Requires-
 Dist: memoized-property==1.0.3 Requires-Dist: pydantic==1.10.11 Requires-Dist:
```

### Comparing `fleks-2024.4.5.9.29/src/fleks.egg-info/SOURCES.txt` & `fleks-2024.5.10.23.48/src/fleks.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,10 +21,11 @@
 src/fleks/cli/options.py
 src/fleks/cli/root_group.py
 src/fleks/meta/__init__.py
 src/fleks/meta/namespace.py
 src/fleks/meta/oop.py
 src/fleks/util/__init__.py
 src/fleks/util/click.py
+src/fleks/util/console.py
 src/fleks/util/lme.py
 src/fleks/util/tagging.py
 src/fleks/util/typing.py
```

