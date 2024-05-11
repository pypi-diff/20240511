# Comparing `tmp/pyuilder-0.0.5.tar.gz` & `tmp/pyuilder-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuilder-0.0.5.tar", last modified: Sat May 11 04:23:50 2024, max compression
+gzip compressed data, was "pyuilder-0.0.6.tar", last modified: Sat May 11 04:57:25 2024, max compression
```

## Comparing `pyuilder-0.0.5.tar` & `pyuilder-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:23:50.239930 pyuilder-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 04:23:34.000000 pyuilder-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-11 04:23:50.239930 pyuilder-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-11 04:23:34.000000 pyuilder-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-11 04:23:34.000000 pyuilder-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 04:23:50.239930 pyuilder-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:23:50.235931 pyuilder-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:23:50.235931 pyuilder-0.0.5/src/pyuilder/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-11 04:23:34.000000 pyuilder-0.0.5/src/pyuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-11 04:23:34.000000 pyuilder-0.0.5/src/pyuilder/pyuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:23:50.239930 pyuilder-0.0.5/src/pyuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-11 04:23:50.000000 pyuilder-0.0.5/src/pyuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-11 04:23:50.000000 pyuilder-0.0.5/src/pyuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 04:23:50.000000 pyuilder-0.0.5/src/pyuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-11 04:23:50.000000 pyuilder-0.0.5/src/pyuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 04:23:50.000000 pyuilder-0.0.5/src/pyuilder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:23:50.239930 pyuilder-0.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-11 04:23:34.000000 pyuilder-0.0.5/test/test_pyuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:57:25.153827 pyuilder-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 04:57:08.000000 pyuilder-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-05-11 04:57:25.153827 pyuilder-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-11 04:57:08.000000 pyuilder-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-11 04:57:08.000000 pyuilder-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 04:57:25.153827 pyuilder-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:57:25.149827 pyuilder-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:57:25.149827 pyuilder-0.0.6/src/pyuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-11 04:57:08.000000 pyuilder-0.0.6/src/pyuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-11 04:57:08.000000 pyuilder-0.0.6/src/pyuilder/pyuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:57:25.153827 pyuilder-0.0.6/src/pyuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-05-11 04:57:25.000000 pyuilder-0.0.6/src/pyuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-11 04:57:25.000000 pyuilder-0.0.6/src/pyuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 04:57:25.000000 pyuilder-0.0.6/src/pyuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-11 04:57:25.000000 pyuilder-0.0.6/src/pyuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 04:57:25.000000 pyuilder-0.0.6/src/pyuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 04:57:25.153827 pyuilder-0.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-11 04:57:08.000000 pyuilder-0.0.6/test/test_pyuilder.py
```

### Comparing `pyuilder-0.0.5/LICENSE` & `pyuilder-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuilder-0.0.5/PKG-INFO` & `pyuilder-0.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuilder
-Version: 0.0.5
+Version: 0.0.6
 Summary: Provides functionality for implementing the builder pattern in Python.
 Author-email: Kevin Jerome <kjerome64@gmail.com>
 Maintainer-email: Kevin Jerome <kjerome64@gmail.com>
 Project-URL: Homepage, https://github.com/kevdog824/pyuilder
 Project-URL: Bug Reports, https://github.com/kevdog824/pyuilder/issues
 Project-URL: Source, https://github.com/kevdog824/pyuilder
 Keywords: builder,builder_pattern,design_patterns
@@ -31,15 +31,15 @@
 Requires-Dist: build==1.2.1; extra == "publish"
 Requires-Dist: twine==5.0.0; extra == "publish"
 Provides-Extra: ci
 Requires-Dist: pyuilder[dev]; extra == "ci"
 Requires-Dist: pyuilder[test]; extra == "ci"
 Requires-Dist: pyuilder[publish]; extra == "ci"
 
-<h1 align="center">Pyuilder ("pill-der")</h1>
+<h1 id="title" align="center">Pyuilder ("pill-der")</h1>
 
 <h2 align="center">
 Bringing the Builder Design Pattern to Python
 </h2>
 
 <!-- Shields Here -->
 <p align="center">
@@ -51,48 +51,53 @@
 ---
 
 ## Summary
 
 - [Getting started](#getting-started)
   - [Installation](#installation)
   - [Usage](#usage)
-    - [Simple example](#customize-the-builder--add-type-annotations)
-    - [Customize the Builder & Add Type Annotations](#simple-example)
+    - [Simple example](#simple-example)
+    - [Customize the Builder & Add Type Annotations](#customize-the-builder-and-add-type-annotations)
+    - [Set How Strict Static Type Checking Is Done on Builders](#set-how-strict-static-type-checking-is-done-on-builders)
     - [Customize the Way Fields Are Set](#customize-the-way-fields-are-set)
 - [Change log](#change-log)
 - [License](#license)
 
-## Getting started
+<h2 id="getting-started">Getting started</h2>
 
-### Installation
+<h3 id="installation">Installation</h3>
 
 ```shell
 pip install pyuilder
 ```
 
-### Usage
+<p align="right"><small><a href="#title">Back to top</a></small></p>
 
-#### Simple example
+<h3 id="usage">Usage</h3>
+
+<h4 id="simple-example">Simple example</h4>
 
 Getting started is as easily as inheriting from `pyuilder.Buildable`:
 
 ```py
 import pyuilder
 
 
 class MyBuildable(pyuilder.Buildable):
     def __init__(self, field1: int, field2: str) -> None:
         self.field1 = field1
         self.field2 = field2
 
 
-MyBuildable.build().field1(1).field2("hello world").build()
+MyBuildable.builder().field1(1).field2("hello world").build()
 ```
 
-#### Customize the Builder & Add Type Annotations
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h4 id="customize-the-builder-and-add-type-annotations">Customize the Builder & Add Type Annotations</h4>
 
 The last example was great and easy to set up but you'll quickly notice you get no intellisense or typing annotations in your IDE. If that's alright with you: great! However, if you want a little more out of pyuilder it's pretty trivial to provide as much information as you want to pyuilder's `Buildable` to get auto-complete, type-hinting, and other useful information in your IDE:
 
 ```py
 from __future__ import annotations
 
 from pyuilder import Buildable, Builder, Setter
@@ -104,15 +109,15 @@
         field2: Setter[MyBuildable.builder, str]
 
     def __init__(self, field1: int, field2: str) -> None:
         self.field1 = field1
         self.field2 = field2
 
 
-MyBuildable.build()\
+MyBuildable.builder()\
     .field1(1)\
     .field2("hello world")\
     .build()
 ```
 
 The setup here ensures correct auto-complete, type hints, etc.:
 
@@ -120,15 +125,27 @@
 - The name of the builder class here (`builder`), is what you will actually will call to invoke the builder: `MyBuildable.builder()`.
   Since the `Buildable` class is annotated to have a method named `builder` I recommend sticking with the same name.
 - The `Setter[...]` annotations on the fields take two `TypeVars` which provide type hinting:
   - The first `TypeVar` indicates the return type after calling a field setter: `.field1() -> MyBuildable.builder`.
     This ensures that type hints aren't lost on chained field setter calls: `field1(1).field2("hello world")`.
   - The second `TypeVar` indicates the value type the field setter accepts: `.field1(value: int).field2(value: str)`.
 
-#### Customize the Way Fields Are Set
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h4 id="set-how-strict-static-type-checking-is-done-on-builders">Set How Strict Static Type Checking Is Done on Builders</h4>
+
+If you try out the example about in an IDE you may notice that trying to use the builder with any field name other than the ones you annotated in your custom builder class will end with red squigglies under your code. This is because the `Builder` class is set up to *appear* (see note below) to only allow the fields you explicitly declared to static type checkers.
+
+However, you may want to maintain intellisense for annotated fields but want to be able to use any field without warnings from your static type check. pyuilder offers a variant of `Bulder` called `RelaxedBuilder` that does just that. The setup is exactly the same as above. Just replace `Builder` with `RelaxedBuilder`.
+
+**NOTE**: Under the hood `Builder` and `RelaxBuilder` really do exactly the same thing. There is no behavioral difference between the two classes during runtime. They only differ in how they are processed during static type analysis.
+
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h4 id="customize-the-way-fields-are-set">Customize the Way Fields Are Set</h4>
 
 The other thing you might want to do is have better control how fields are set when you do something like `.builder().field(...)`. If `field` was a `list` for example you might want to be able to call `field(...)` on the builder multiple times to continuously append values to it (similar to Lombok's `@Singular` in Java). This is certainly possible with pyuilder:
 
 ```py
 from __future__ import annotations
 
 from pyuilder import Buildable, Builder, Setter
@@ -141,34 +158,40 @@
     def __init__(self, field: list[str]) -> None:
         self.field = field
 
 
 # Examples
 
 # Setting the field as a list explicitly
-MyBuildable.build().field(["foo", "bar"]).build()
+MyBuildable.builder().field(["foo", "bar"]).build()
 
 # Specifying how it should be added via str
-MyBuildable.build()\
+MyBuildable.builder()\
     .field([])\
     .field("foo", "append")\
     .field("bar", "append")\
     .build()
 
 # Specifying how it should be added via callable
-MyBuildable.build()\
+MyBuildable.builder()\
     .field(["foo"])\
     .field("bar", list.append)\
     .build()
 ```
 
 If the second parameter to a field setter is a `str` as it is in the second example it is assumed to be a name of a method on the existing value for that field. In the example above, by the second call of `field()`, the existing value for field is a `list`. The setter will find the "append" method on the existing `list` value and call it with the provided value as the first argument.
 
 If the second parameter to a field setter is a `Callable` as it is in the third example the setter will call that method. When the setter calls it it will give the existing value as the first argument to the callable and the provided value as the second argument to the callable. In the example above, the provided `list.append` callable is called with two arguments as described above: `list.append(existing, value)` where `existing = ["foo"]` and `value = "bar"`.
 
-## Change log
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h2 id="change-log">Change log</h2>
 
 See [CHANGELOG](https://github.com/kevdog824/pyuilder/blob/main/CHANGELOG.md).
 
-## License
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h2 id="license">License</h2>
 
 MIT.
+
+<p align="right"><small><a href="#title">Back to top</a></small></p>
```

### Comparing `pyuilder-0.0.5/README.md` & `pyuilder-0.0.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<h1 align="center">Pyuilder ("pill-der")</h1>
+<h1 id="title" align="center">Pyuilder ("pill-der")</h1>
 
 <h2 align="center">
 Bringing the Builder Design Pattern to Python
 </h2>
 
 <!-- Shields Here -->
 <p align="center">
@@ -14,48 +14,53 @@
 ---
 
 ## Summary
 
 - [Getting started](#getting-started)
   - [Installation](#installation)
   - [Usage](#usage)
-    - [Simple example](#customize-the-builder--add-type-annotations)
-    - [Customize the Builder & Add Type Annotations](#simple-example)
+    - [Simple example](#simple-example)
+    - [Customize the Builder & Add Type Annotations](#customize-the-builder-and-add-type-annotations)
+    - [Set How Strict Static Type Checking Is Done on Builders](#set-how-strict-static-type-checking-is-done-on-builders)
     - [Customize the Way Fields Are Set](#customize-the-way-fields-are-set)
 - [Change log](#change-log)
 - [License](#license)
 
-## Getting started
+<h2 id="getting-started">Getting started</h2>
 
-### Installation
+<h3 id="installation">Installation</h3>
 
 ```shell
 pip install pyuilder
 ```
 
-### Usage
+<p align="right"><small><a href="#title">Back to top</a></small></p>
 
-#### Simple example
+<h3 id="usage">Usage</h3>
+
+<h4 id="simple-example">Simple example</h4>
 
 Getting started is as easily as inheriting from `pyuilder.Buildable`:
 
 ```py
 import pyuilder
 
 
 class MyBuildable(pyuilder.Buildable):
     def __init__(self, field1: int, field2: str) -> None:
         self.field1 = field1
         self.field2 = field2
 
 
-MyBuildable.build().field1(1).field2("hello world").build()
+MyBuildable.builder().field1(1).field2("hello world").build()
 ```
 
-#### Customize the Builder & Add Type Annotations
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h4 id="customize-the-builder-and-add-type-annotations">Customize the Builder & Add Type Annotations</h4>
 
 The last example was great and easy to set up but you'll quickly notice you get no intellisense or typing annotations in your IDE. If that's alright with you: great! However, if you want a little more out of pyuilder it's pretty trivial to provide as much information as you want to pyuilder's `Buildable` to get auto-complete, type-hinting, and other useful information in your IDE:
 
 ```py
 from __future__ import annotations
 
 from pyuilder import Buildable, Builder, Setter
@@ -67,15 +72,15 @@
         field2: Setter[MyBuildable.builder, str]
 
     def __init__(self, field1: int, field2: str) -> None:
         self.field1 = field1
         self.field2 = field2
 
 
-MyBuildable.build()\
+MyBuildable.builder()\
     .field1(1)\
     .field2("hello world")\
     .build()
 ```
 
 The setup here ensures correct auto-complete, type hints, etc.:
 
@@ -83,15 +88,27 @@
 - The name of the builder class here (`builder`), is what you will actually will call to invoke the builder: `MyBuildable.builder()`.
   Since the `Buildable` class is annotated to have a method named `builder` I recommend sticking with the same name.
 - The `Setter[...]` annotations on the fields take two `TypeVars` which provide type hinting:
   - The first `TypeVar` indicates the return type after calling a field setter: `.field1() -> MyBuildable.builder`.
     This ensures that type hints aren't lost on chained field setter calls: `field1(1).field2("hello world")`.
   - The second `TypeVar` indicates the value type the field setter accepts: `.field1(value: int).field2(value: str)`.
 
-#### Customize the Way Fields Are Set
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h4 id="set-how-strict-static-type-checking-is-done-on-builders">Set How Strict Static Type Checking Is Done on Builders</h4>
+
+If you try out the example about in an IDE you may notice that trying to use the builder with any field name other than the ones you annotated in your custom builder class will end with red squigglies under your code. This is because the `Builder` class is set up to *appear* (see note below) to only allow the fields you explicitly declared to static type checkers.
+
+However, you may want to maintain intellisense for annotated fields but want to be able to use any field without warnings from your static type check. pyuilder offers a variant of `Bulder` called `RelaxedBuilder` that does just that. The setup is exactly the same as above. Just replace `Builder` with `RelaxedBuilder`.
+
+**NOTE**: Under the hood `Builder` and `RelaxBuilder` really do exactly the same thing. There is no behavioral difference between the two classes during runtime. They only differ in how they are processed during static type analysis.
+
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h4 id="customize-the-way-fields-are-set">Customize the Way Fields Are Set</h4>
 
 The other thing you might want to do is have better control how fields are set when you do something like `.builder().field(...)`. If `field` was a `list` for example you might want to be able to call `field(...)` on the builder multiple times to continuously append values to it (similar to Lombok's `@Singular` in Java). This is certainly possible with pyuilder:
 
 ```py
 from __future__ import annotations
 
 from pyuilder import Buildable, Builder, Setter
@@ -104,34 +121,40 @@
     def __init__(self, field: list[str]) -> None:
         self.field = field
 
 
 # Examples
 
 # Setting the field as a list explicitly
-MyBuildable.build().field(["foo", "bar"]).build()
+MyBuildable.builder().field(["foo", "bar"]).build()
 
 # Specifying how it should be added via str
-MyBuildable.build()\
+MyBuildable.builder()\
     .field([])\
     .field("foo", "append")\
     .field("bar", "append")\
     .build()
 
 # Specifying how it should be added via callable
-MyBuildable.build()\
+MyBuildable.builder()\
     .field(["foo"])\
     .field("bar", list.append)\
     .build()
 ```
 
 If the second parameter to a field setter is a `str` as it is in the second example it is assumed to be a name of a method on the existing value for that field. In the example above, by the second call of `field()`, the existing value for field is a `list`. The setter will find the "append" method on the existing `list` value and call it with the provided value as the first argument.
 
 If the second parameter to a field setter is a `Callable` as it is in the third example the setter will call that method. When the setter calls it it will give the existing value as the first argument to the callable and the provided value as the second argument to the callable. In the example above, the provided `list.append` callable is called with two arguments as described above: `list.append(existing, value)` where `existing = ["foo"]` and `value = "bar"`.
 
-## Change log
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h2 id="change-log">Change log</h2>
 
 See [CHANGELOG](https://github.com/kevdog824/pyuilder/blob/main/CHANGELOG.md).
 
-## License
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h2 id="license">License</h2>
 
 MIT.
+
+<p align="right"><small><a href="#title">Back to top</a></small></p>
```

### Comparing `pyuilder-0.0.5/pyproject.toml` & `pyuilder-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pyuilder"
-version = "0.0.5"
+version = "0.0.6"
 description = "Provides functionality for implementing the builder pattern in Python."
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE.txt" }
 keywords = ["builder", "builder_pattern", "design_patterns"]
 authors = [{ name = "Kevin Jerome", email = "kjerome64@gmail.com" }]
 maintainers = [{ name = "Kevin Jerome", email = "kjerome64@gmail.com" }]
```

### Comparing `pyuilder-0.0.5/src/pyuilder/pyuilder.py` & `pyuilder-0.0.6/src/pyuilder/pyuilder.py`

 * *Files identical despite different names*

### Comparing `pyuilder-0.0.5/src/pyuilder.egg-info/PKG-INFO` & `pyuilder-0.0.6/src/pyuilder.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuilder
-Version: 0.0.5
+Version: 0.0.6
 Summary: Provides functionality for implementing the builder pattern in Python.
 Author-email: Kevin Jerome <kjerome64@gmail.com>
 Maintainer-email: Kevin Jerome <kjerome64@gmail.com>
 Project-URL: Homepage, https://github.com/kevdog824/pyuilder
 Project-URL: Bug Reports, https://github.com/kevdog824/pyuilder/issues
 Project-URL: Source, https://github.com/kevdog824/pyuilder
 Keywords: builder,builder_pattern,design_patterns
@@ -31,15 +31,15 @@
 Requires-Dist: build==1.2.1; extra == "publish"
 Requires-Dist: twine==5.0.0; extra == "publish"
 Provides-Extra: ci
 Requires-Dist: pyuilder[dev]; extra == "ci"
 Requires-Dist: pyuilder[test]; extra == "ci"
 Requires-Dist: pyuilder[publish]; extra == "ci"
 
-<h1 align="center">Pyuilder ("pill-der")</h1>
+<h1 id="title" align="center">Pyuilder ("pill-der")</h1>
 
 <h2 align="center">
 Bringing the Builder Design Pattern to Python
 </h2>
 
 <!-- Shields Here -->
 <p align="center">
@@ -51,48 +51,53 @@
 ---
 
 ## Summary
 
 - [Getting started](#getting-started)
   - [Installation](#installation)
   - [Usage](#usage)
-    - [Simple example](#customize-the-builder--add-type-annotations)
-    - [Customize the Builder & Add Type Annotations](#simple-example)
+    - [Simple example](#simple-example)
+    - [Customize the Builder & Add Type Annotations](#customize-the-builder-and-add-type-annotations)
+    - [Set How Strict Static Type Checking Is Done on Builders](#set-how-strict-static-type-checking-is-done-on-builders)
     - [Customize the Way Fields Are Set](#customize-the-way-fields-are-set)
 - [Change log](#change-log)
 - [License](#license)
 
-## Getting started
+<h2 id="getting-started">Getting started</h2>
 
-### Installation
+<h3 id="installation">Installation</h3>
 
 ```shell
 pip install pyuilder
 ```
 
-### Usage
+<p align="right"><small><a href="#title">Back to top</a></small></p>
 
-#### Simple example
+<h3 id="usage">Usage</h3>
+
+<h4 id="simple-example">Simple example</h4>
 
 Getting started is as easily as inheriting from `pyuilder.Buildable`:
 
 ```py
 import pyuilder
 
 
 class MyBuildable(pyuilder.Buildable):
     def __init__(self, field1: int, field2: str) -> None:
         self.field1 = field1
         self.field2 = field2
 
 
-MyBuildable.build().field1(1).field2("hello world").build()
+MyBuildable.builder().field1(1).field2("hello world").build()
 ```
 
-#### Customize the Builder & Add Type Annotations
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h4 id="customize-the-builder-and-add-type-annotations">Customize the Builder & Add Type Annotations</h4>
 
 The last example was great and easy to set up but you'll quickly notice you get no intellisense or typing annotations in your IDE. If that's alright with you: great! However, if you want a little more out of pyuilder it's pretty trivial to provide as much information as you want to pyuilder's `Buildable` to get auto-complete, type-hinting, and other useful information in your IDE:
 
 ```py
 from __future__ import annotations
 
 from pyuilder import Buildable, Builder, Setter
@@ -104,15 +109,15 @@
         field2: Setter[MyBuildable.builder, str]
 
     def __init__(self, field1: int, field2: str) -> None:
         self.field1 = field1
         self.field2 = field2
 
 
-MyBuildable.build()\
+MyBuildable.builder()\
     .field1(1)\
     .field2("hello world")\
     .build()
 ```
 
 The setup here ensures correct auto-complete, type hints, etc.:
 
@@ -120,15 +125,27 @@
 - The name of the builder class here (`builder`), is what you will actually will call to invoke the builder: `MyBuildable.builder()`.
   Since the `Buildable` class is annotated to have a method named `builder` I recommend sticking with the same name.
 - The `Setter[...]` annotations on the fields take two `TypeVars` which provide type hinting:
   - The first `TypeVar` indicates the return type after calling a field setter: `.field1() -> MyBuildable.builder`.
     This ensures that type hints aren't lost on chained field setter calls: `field1(1).field2("hello world")`.
   - The second `TypeVar` indicates the value type the field setter accepts: `.field1(value: int).field2(value: str)`.
 
-#### Customize the Way Fields Are Set
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h4 id="set-how-strict-static-type-checking-is-done-on-builders">Set How Strict Static Type Checking Is Done on Builders</h4>
+
+If you try out the example about in an IDE you may notice that trying to use the builder with any field name other than the ones you annotated in your custom builder class will end with red squigglies under your code. This is because the `Builder` class is set up to *appear* (see note below) to only allow the fields you explicitly declared to static type checkers.
+
+However, you may want to maintain intellisense for annotated fields but want to be able to use any field without warnings from your static type check. pyuilder offers a variant of `Bulder` called `RelaxedBuilder` that does just that. The setup is exactly the same as above. Just replace `Builder` with `RelaxedBuilder`.
+
+**NOTE**: Under the hood `Builder` and `RelaxBuilder` really do exactly the same thing. There is no behavioral difference between the two classes during runtime. They only differ in how they are processed during static type analysis.
+
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h4 id="customize-the-way-fields-are-set">Customize the Way Fields Are Set</h4>
 
 The other thing you might want to do is have better control how fields are set when you do something like `.builder().field(...)`. If `field` was a `list` for example you might want to be able to call `field(...)` on the builder multiple times to continuously append values to it (similar to Lombok's `@Singular` in Java). This is certainly possible with pyuilder:
 
 ```py
 from __future__ import annotations
 
 from pyuilder import Buildable, Builder, Setter
@@ -141,34 +158,40 @@
     def __init__(self, field: list[str]) -> None:
         self.field = field
 
 
 # Examples
 
 # Setting the field as a list explicitly
-MyBuildable.build().field(["foo", "bar"]).build()
+MyBuildable.builder().field(["foo", "bar"]).build()
 
 # Specifying how it should be added via str
-MyBuildable.build()\
+MyBuildable.builder()\
     .field([])\
     .field("foo", "append")\
     .field("bar", "append")\
     .build()
 
 # Specifying how it should be added via callable
-MyBuildable.build()\
+MyBuildable.builder()\
     .field(["foo"])\
     .field("bar", list.append)\
     .build()
 ```
 
 If the second parameter to a field setter is a `str` as it is in the second example it is assumed to be a name of a method on the existing value for that field. In the example above, by the second call of `field()`, the existing value for field is a `list`. The setter will find the "append" method on the existing `list` value and call it with the provided value as the first argument.
 
 If the second parameter to a field setter is a `Callable` as it is in the third example the setter will call that method. When the setter calls it it will give the existing value as the first argument to the callable and the provided value as the second argument to the callable. In the example above, the provided `list.append` callable is called with two arguments as described above: `list.append(existing, value)` where `existing = ["foo"]` and `value = "bar"`.
 
-## Change log
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h2 id="change-log">Change log</h2>
 
 See [CHANGELOG](https://github.com/kevdog824/pyuilder/blob/main/CHANGELOG.md).
 
-## License
+<p align="right"><small><a href="#title">Back to top</a></small></p>
+
+<h2 id="license">License</h2>
 
 MIT.
+
+<p align="right"><small><a href="#title">Back to top</a></small></p>
```

### Comparing `pyuilder-0.0.5/test/test_pyuilder.py` & `pyuilder-0.0.6/test/test_pyuilder.py`

 * *Files identical despite different names*

