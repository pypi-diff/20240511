# Comparing `tmp/that_depends-1.6.5.tar.gz` & `tmp/that_depends-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that_depends-1.6.5.tar", max compression
+gzip compressed data, was "that_depends-1.6.6.tar", max compression
```

## Comparing `that_depends-1.6.5.tar` & `that_depends-1.6.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.6.5/LICENSE
--rw-r--r--   0        0        0     7277 2024-04-28 07:52:26.184942 that_depends-1.6.5/README.md
--rw-r--r--   0        0        0     1482 2024-04-28 10:06:28.387006 that_depends-1.6.5/pyproject.toml
--rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.6.5/that_depends/__init__.py
--rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.6.5/that_depends/container.py
--rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.6.5/that_depends/injection.py
--rw-r--r--   0        0        0      739 2024-04-22 06:16:04.333831 that_depends-1.6.5/that_depends/providers/__init__.py
--rw-r--r--   0        0        0      642 2024-04-16 06:00:18.298948 that_depends-1.6.5/that_depends/providers/base.py
--rw-r--r--   0        0        0      465 2024-04-16 06:00:22.046508 that_depends-1.6.5/that_depends/providers/collections.py
--rw-r--r--   0        0        0     3792 2024-04-28 07:52:26.186980 that_depends-1.6.5/that_depends/providers/context_resources.py
--rw-r--r--   0        0        0     1365 2024-04-16 06:00:22.046739 that_depends-1.6.5/that_depends/providers/factories.py
--rw-r--r--   0        0        0     2948 2024-04-21 21:10:28.406639 that_depends-1.6.5/that_depends/providers/resources.py
--rw-r--r--   0        0        0      993 2024-04-17 05:36:03.299156 that_depends-1.6.5/that_depends/providers/singleton.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.6.5/that_depends/py.typed
--rw-r--r--   0        0        0     7757 1970-01-01 00:00:00.000000 that_depends-1.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.6.6/LICENSE
+-rw-r--r--   0        0        0     7277 2024-05-10 11:45:17.705570 that_depends-1.6.6/README.md
+-rw-r--r--   0        0        0     1482 2024-05-11 10:28:58.661919 that_depends-1.6.6/pyproject.toml
+-rw-r--r--   0        0        0      164 2024-05-09 18:37:39.636094 that_depends-1.6.6/that_depends/__init__.py
+-rw-r--r--   0        0        0     1984 2024-05-11 10:19:08.451499 that_depends-1.6.6/that_depends/container.py
+-rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.6.6/that_depends/injection.py
+-rw-r--r--   0        0        0      739 2024-05-09 12:44:56.346923 that_depends-1.6.6/that_depends/providers/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-16 06:00:18.298948 that_depends-1.6.6/that_depends/providers/base.py
+-rw-r--r--   0        0        0      465 2024-04-16 06:00:22.046508 that_depends-1.6.6/that_depends/providers/collections.py
+-rw-r--r--   0        0        0     3792 2024-04-28 07:52:26.186980 that_depends-1.6.6/that_depends/providers/context_resources.py
+-rw-r--r--   0        0        0     1365 2024-04-16 06:00:22.046739 that_depends-1.6.6/that_depends/providers/factories.py
+-rw-r--r--   0        0        0     2948 2024-04-21 21:10:28.406639 that_depends-1.6.6/that_depends/providers/resources.py
+-rw-r--r--   0        0        0      993 2024-05-09 12:45:32.587857 that_depends-1.6.6/that_depends/providers/singleton.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.6.6/that_depends/py.typed
+-rw-r--r--   0        0        0     7757 1970-01-01 00:00:00.000000 that_depends-1.6.6/PKG-INFO
```

### Comparing `that_depends-1.6.5/LICENSE` & `that_depends-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.5/README.md` & `that_depends-1.6.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,22 +20,23 @@
 ```python
 from tests.container import DIContainer
 
 async def main():
     some_dependency = await DIContainer.independent_factory()
 ```
 2. No wiring for injections in function arguments -> achieved by decision that only one instance of container is supported
+
 ```python
 from tests import container
 from that_depends import Provide, inject
 
 
 @inject
 async def some_function(
-    independent_factory: container.IndependentFactory = Provide[container.DIContainer.independent_factory],
+        independent_factory: container.SimpleFactory = Provide[container.DIContainer.independent_factory],
 ) -> None:
     assert independent_factory.dep1
 ```
 
 # Quickstart
 ## Install
```

### Comparing `that_depends-1.6.5/pyproject.toml` & `that_depends-1.6.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "that-depends"
-version = "1.6.5"
+version = "1.6.6"
 description = "Simple Dependency Injection framework"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 homepage = "https://github.com/modern-python/that-depends"
 packages = [
     { include = "that_depends" },
 ]
```

### Comparing `that_depends-1.6.5/that_depends/injection.py` & `that_depends-1.6.6/that_depends/injection.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.5/that_depends/providers/__init__.py` & `that_depends-1.6.6/that_depends/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.5/that_depends/providers/base.py` & `that_depends-1.6.6/that_depends/providers/base.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.5/that_depends/providers/context_resources.py` & `that_depends-1.6.6/that_depends/providers/context_resources.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.5/that_depends/providers/factories.py` & `that_depends-1.6.6/that_depends/providers/factories.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.5/that_depends/providers/resources.py` & `that_depends-1.6.6/that_depends/providers/resources.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.5/that_depends/providers/singleton.py` & `that_depends-1.6.6/that_depends/providers/singleton.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.6.5/PKG-INFO` & `that_depends-1.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: that-depends
-Version: 1.6.5
+Version: 1.6.6
 Summary: Simple Dependency Injection framework
 Home-page: https://github.com/modern-python/that-depends
 Author: Artur Shiriev
 Author-email: me@shiriev.ru
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -34,22 +34,23 @@
 ```python
 from tests.container import DIContainer
 
 async def main():
     some_dependency = await DIContainer.independent_factory()
 ```
 2. No wiring for injections in function arguments -> achieved by decision that only one instance of container is supported
+
 ```python
 from tests import container
 from that_depends import Provide, inject
 
 
 @inject
 async def some_function(
-    independent_factory: container.IndependentFactory = Provide[container.DIContainer.independent_factory],
+        independent_factory: container.SimpleFactory = Provide[container.DIContainer.independent_factory],
 ) -> None:
     assert independent_factory.dep1
 ```
 
 # Quickstart
 ## Install
```

