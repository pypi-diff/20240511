# Comparing `tmp/pyuilder-0.0.4.tar.gz` & `tmp/pyuilder-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuilder-0.0.4.tar", last modified: Mon May  6 04:04:53 2024, max compression
+gzip compressed data, was "pyuilder-0.0.5.tar", last modified: Sat May 11 04:23:50 2024, max compression
```

## Comparing `pyuilder-0.0.4.tar` & `pyuilder-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:04:53.729673 pyuilder-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 04:04:37.000000 pyuilder-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-06 04:04:53.729673 pyuilder-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-06 04:04:37.000000 pyuilder-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-06 04:04:37.000000 pyuilder-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 04:04:53.729673 pyuilder-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:04:53.725673 pyuilder-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:04:53.725673 pyuilder-0.0.4/src/pyuilder/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-06 04:04:37.000000 pyuilder-0.0.4/src/pyuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-06 04:04:37.000000 pyuilder-0.0.4/src/pyuilder/pyuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:04:53.729673 pyuilder-0.0.4/src/pyuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-06 04:04:53.000000 pyuilder-0.0.4/src/pyuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-06 04:04:53.000000 pyuilder-0.0.4/src/pyuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 04:04:53.000000 pyuilder-0.0.4/src/pyuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-06 04:04:53.000000 pyuilder-0.0.4/src/pyuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 04:04:53.000000 pyuilder-0.0.4/src/pyuilder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 04:04:53.729673 pyuilder-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-06 04:04:37.000000 pyuilder-0.0.4/test/test_pyuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:23:50.239930 pyuilder-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 04:23:34.000000 pyuilder-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-11 04:23:50.239930 pyuilder-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-11 04:23:34.000000 pyuilder-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-11 04:23:34.000000 pyuilder-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 04:23:50.239930 pyuilder-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:23:50.235931 pyuilder-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:23:50.235931 pyuilder-0.0.5/src/pyuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-11 04:23:34.000000 pyuilder-0.0.5/src/pyuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-11 04:23:34.000000 pyuilder-0.0.5/src/pyuilder/pyuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:23:50.239930 pyuilder-0.0.5/src/pyuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-11 04:23:50.000000 pyuilder-0.0.5/src/pyuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-11 04:23:50.000000 pyuilder-0.0.5/src/pyuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 04:23:50.000000 pyuilder-0.0.5/src/pyuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-11 04:23:50.000000 pyuilder-0.0.5/src/pyuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 04:23:50.000000 pyuilder-0.0.5/src/pyuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:23:50.239930 pyuilder-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-11 04:23:34.000000 pyuilder-0.0.5/test/test_pyuilder.py
```

### Comparing `pyuilder-0.0.4/LICENSE` & `pyuilder-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuilder-0.0.4/PKG-INFO` & `pyuilder-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuilder
-Version: 0.0.4
+Version: 0.0.5
 Summary: Provides functionality for implementing the builder pattern in Python.
 Author-email: Kevin Jerome <kjerome64@gmail.com>
 Maintainer-email: Kevin Jerome <kjerome64@gmail.com>
 Project-URL: Homepage, https://github.com/kevdog824/pyuilder
 Project-URL: Bug Reports, https://github.com/kevdog824/pyuilder/issues
 Project-URL: Source, https://github.com/kevdog824/pyuilder
 Keywords: builder,builder_pattern,design_patterns
```

### Comparing `pyuilder-0.0.4/README.md` & `pyuilder-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyuilder-0.0.4/pyproject.toml` & `pyuilder-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pyuilder"
-version = "0.0.4"
+version = "0.0.5"
 description = "Provides functionality for implementing the builder pattern in Python."
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE.txt" }
 keywords = ["builder", "builder_pattern", "design_patterns"]
 authors = [{ name = "Kevin Jerome", email = "kjerome64@gmail.com" }]
 maintainers = [{ name = "Kevin Jerome", email = "kjerome64@gmail.com" }]
```

### Comparing `pyuilder-0.0.4/src/pyuilder/pyuilder.py` & `pyuilder-0.0.5/src/pyuilder/pyuilder.py`

 * *Files 14% similar despite different names*

```diff
@@ -74,16 +74,18 @@
         """
         self._data: _t.Dict[str, _t.Any] = {**kwargs}
         self._init_param_kinds = [
             inspect._ParameterKind.POSITIONAL_OR_KEYWORD,
             inspect._ParameterKind.KEYWORD_ONLY,
         ]
 
-    def __getattr__(self, __name: str) -> Setter[_te.Self, _t.Any]:
-        return Setter(self, __name)
+    if not _t.TYPE_CHECKING:
+
+        def __getattr__(self, __name: str) -> Setter[_te.Self, _t.Any]:
+            return Setter(self, __name)
 
     def _break_args(
         self, typ: _t.Type[_T]
     ) -> _t.Tuple[_t.Dict[str, _t.Any], _t.Dict[str, _t.Any]]:
         kwargs: _t.Dict[str, _t.Any] = {}
         sig = inspect.signature(typ)
         for p in sig.parameters.values():
@@ -101,33 +103,47 @@
         kwargs, attrs = self._break_args(self.typ)
         inst = self.typ(**kwargs)
         for name, value in attrs.items():
             setattr(inst, name, value)
         return inst
 
 
+class RelaxedBuilder(Builder[_T]):
+    """Class for adding builders to other classes.
+
+    Much like Builder except it adds static type support for `__getattr__`.
+    Functionally, this will allow the builder to support any field name from a static
+    type checking perspective.
+    """
+
+    if _t.TYPE_CHECKING:
+
+        def __getattr__(self, __name: str) -> Setter[_te.Self, _t.Any]:
+            return Setter(self, __name)
+
+
 ### Builder Generation
 
 
 class Buildable:
     if _t.TYPE_CHECKING:
 
         class builder(Builder[_te.Self]): ...  # type: ignore # pragma: no cover
 
     @classmethod  # type: ignore[no-redef]
-    def builder(cls, **kwargs: _t.Any) -> Builder[_te.Self]:
+    def builder(cls, **kwargs: _t.Any) -> RelaxedBuilder[_te.Self]:
         """Create a new builder instance for building the class
 
         Args:
             **kwargs (Any): Can set any number of fields here at construction
         """
-        b: Builder[_te.Self] = Builder(**kwargs)
+        b: RelaxedBuilder[_te.Self] = RelaxedBuilder(**kwargs)
         b.typ = cls
         return b
 
     def __init_subclass__(cls, **_: _t.Any) -> None:
         for value in cls.__dict__.values():
             if isinstance(value, type) and issubclass(value, Builder):
                 value.typ = cls  # type: ignore
 
 
-__all__ = ["Buildable", "Builder", "Setter"]
+__all__ = ["Buildable", "Builder", "RelaxedBuilder", "Setter"]
```

### Comparing `pyuilder-0.0.4/src/pyuilder.egg-info/PKG-INFO` & `pyuilder-0.0.5/src/pyuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuilder
-Version: 0.0.4
+Version: 0.0.5
 Summary: Provides functionality for implementing the builder pattern in Python.
 Author-email: Kevin Jerome <kjerome64@gmail.com>
 Maintainer-email: Kevin Jerome <kjerome64@gmail.com>
 Project-URL: Homepage, https://github.com/kevdog824/pyuilder
 Project-URL: Bug Reports, https://github.com/kevdog824/pyuilder/issues
 Project-URL: Source, https://github.com/kevdog824/pyuilder
 Keywords: builder,builder_pattern,design_patterns
```

### Comparing `pyuilder-0.0.4/test/test_pyuilder.py` & `pyuilder-0.0.5/test/test_pyuilder.py`

 * *Files identical despite different names*

