# Comparing `tmp/pybunch-1.0.8.tar.gz` & `tmp/pybunch-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybunch-1.0.8.tar", last modified: Tue Apr 23 10:14:37 2024, max compression
+gzip compressed data, was "pybunch-1.0.9.tar", last modified: Tue Apr 23 14:28:45 2024, max compression
```

## Comparing `pybunch-1.0.8.tar` & `pybunch-1.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.743774 pybunch-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-23 10:14:33.000000 pybunch-1.0.8/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 10:14:33.000000 pybunch-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 10:14:33.000000 pybunch-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 10:14:37.747774 pybunch-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 10:14:33.000000 pybunch-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/example/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 10:14:33.000000 pybunch-1.0.8/example/fibonnaci.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-23 10:14:33.000000 pybunch-1.0.8/example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/example/submodule/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:33.000000 pybunch-1.0.8/example/submodule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 10:14:33.000000 pybunch-1.0.8/example/submodule/motd.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:33.000000 pybunch-1.0.8/example/unused.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 10:14:33.000000 pybunch-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 10:14:37.747774 pybunch-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/src/pybunch/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 10:14:33.000000 pybunch-1.0.8/src/pybunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-23 10:14:33.000000 pybunch-1.0.8/src/pybunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-23 10:14:33.000000 pybunch-1.0.8/src/pybunch/packed_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-23 10:14:33.000000 pybunch-1.0.8/src/pybunch/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:14:37.747774 pybunch-1.0.8/src/pybunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 10:14:37.000000 pybunch-1.0.8/src/pybunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 10:14:37.000000 pybunch-1.0.8/src/pybunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 10:14:37.000000 pybunch-1.0.8/src/pybunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 10:14:37.000000 pybunch-1.0.8/src/pybunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 10:14:37.000000 pybunch-1.0.8/src/pybunch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.588784 pybunch-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.580783 pybunch-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.584784 pybunch-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-23 14:28:40.000000 pybunch-1.0.9/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 14:28:40.000000 pybunch-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 14:28:40.000000 pybunch-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 14:28:45.584784 pybunch-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 14:28:40.000000 pybunch-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.584784 pybunch-1.0.9/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 14:28:40.000000 pybunch-1.0.9/example/fibonnaci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-23 14:28:40.000000 pybunch-1.0.9/example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.584784 pybunch-1.0.9/example/submodule/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:40.000000 pybunch-1.0.9/example/submodule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 14:28:40.000000 pybunch-1.0.9/example/submodule/motd.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:40.000000 pybunch-1.0.9/example/unused.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 14:28:40.000000 pybunch-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:28:45.588784 pybunch-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.580783 pybunch-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.584784 pybunch-1.0.9/src/pybunch/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 14:28:40.000000 pybunch-1.0.9/src/pybunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-23 14:28:40.000000 pybunch-1.0.9/src/pybunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-04-23 14:28:40.000000 pybunch-1.0.9/src/pybunch/packed_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-23 14:28:40.000000 pybunch-1.0.9/src/pybunch/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:45.584784 pybunch-1.0.9/src/pybunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 14:28:45.000000 pybunch-1.0.9/src/pybunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 14:28:45.000000 pybunch-1.0.9/src/pybunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:28:45.000000 pybunch-1.0.9/src/pybunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 14:28:45.000000 pybunch-1.0.9/src/pybunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 14:28:45.000000 pybunch-1.0.9/src/pybunch.egg-info/top_level.txt
```

### Comparing `pybunch-1.0.8/.github/workflows/publish-to-pypi.yaml` & `pybunch-1.0.9/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.8/LICENSE` & `pybunch-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.8/PKG-INFO` & `pybunch-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybunch-1.0.8/pyproject.toml` & `pybunch-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.8/src/pybunch/__main__.py` & `pybunch-1.0.9/src/pybunch/__main__.py`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.8/src/pybunch/packed_base.py` & `pybunch-1.0.9/src/pybunch/packed_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -74,14 +74,16 @@
 
 class ModuleDescription(object):
     def __init__(self, name, code):
         # type: (str, str) -> None
         self.name = name
         self.file_name = 'pybunch <%s>' % name
         self.path = ModulePath(*name.split('.'))
+        self.parent_name = '.'.join(self.path.parts[:-1])
+        self.package = None  # type: str
         self.source_code = code
         self._compiled = None  # type: 'code'
         self._module = None  # type: _module_type | None
 
 
     @property
     def compiled(self):
@@ -92,28 +94,53 @@
     def is_package(self, name):
         # type: (str) -> bool
         return self.path.parts[-1] == '__init__'
 
     def load_module(self, name):
         # type: (str) -> _module_type
         if self._module is None:
-            parent = '.'.join(self.path.parts[:-1])
             if self.is_package(None):
-                module = _module_type(parent)
+                module = _module_type(self.parent_name)
+                self.package = '.'.join(self.path.parts[:-2])
+                self.name = self.parent_name
                 module.__path__ = []
             else:
                 module = _module_type(self.name)
+                self.package = self.parent_name
 
-            module.__package__ = parent
+            module.__package__ = self.package
             module.__file__ = self.file_name
-            exec(self.compiled, module.__dict__)
+            self.run_module(_globals=module.__dict__)
             self._module = module
 
         return sys.modules.setdefault(name, self._module)
 
+    def run_module(self, _globals=None, name=None):
+        # type: (str) -> None
+        if _globals is None:
+            _globals = {}
+
+        _globals.update(__name__=name if name is not None else self.name,
+                        __file__=self.file_name,
+                        __loader__=self,
+                        __package__=self.parent_name)
+
+        restore_name = '__name__' in _globals
+        old_filename = _globals.get('__name__', None)
+        if name is not None:
+            _globals['__name__'] = name
+
+        exec(self.compiled, _globals)
+        if restore_name:
+            _globals[''] = old_filename
+        else:
+            del _globals['__name__']
+
+        return _globals
+
     def get_code(self, name):
         # type: (str) -> 'code'
         return self.compiled
 
     def get_source(self, *args, **kwargs):
         return self.source_code
 
@@ -188,20 +215,25 @@
         sys.excepthook = except_hook
         yield
         sys.excepthook = old_except_hook
 
     def import_module(self, module):
         # type: (str) -> _module_type
         with self.add_to_meta_path, self.with_custom_stacktrace:
-            importlib.import_module(module)
+            return importlib.import_module(module)
 
     def execute_module(self, module):
         # type: (str) -> _module_type
         with self.add_to_meta_path, self.with_custom_stacktrace:
-            new_globals = runpy.run_module(module, run_name='__main__')
+            try:
+                new_globals = runpy.run_module(module, run_name='__main__')
+            except ImportError:
+                # Fallback for jython
+                imported_module = importlib.import_module(module)
+                new_globals = imported_module.__loader__.run_module(name='__main__')
 
         current_globals = globals()
         keys_to_delete = set(current_globals.keys()).difference(new_globals)
         current_globals.update(new_globals)
         for key in keys_to_delete:
             del current_globals[key]
```

### Comparing `pybunch-1.0.8/src/pybunch/project.py` & `pybunch-1.0.9/src/pybunch/project.py`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.8/src/pybunch.egg-info/PKG-INFO` & `pybunch-1.0.9/src/pybunch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

