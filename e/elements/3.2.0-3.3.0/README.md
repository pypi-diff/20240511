# Comparing `tmp/elements-3.2.0.tar.gz` & `tmp/elements-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elements-3.2.0.tar", last modified: Mon Feb 26 02:12:36 2024, max compression
+gzip compressed data, was "elements-3.3.0.tar", last modified: Fri May 10 22:03:09 2024, max compression
```

## Comparing `elements-3.2.0.tar` & `elements-3.3.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-02-26 02:12:36.941747 elements-3.2.0/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.2.0/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.2.0/MANIFEST.in
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10797 2024-02-26 02:12:36.941747 elements-3.2.0/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10437 2023-12-10 19:43:58.000000 elements-3.2.0/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-02-26 02:12:36.933746 elements-3.2.0/elements/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      541 2024-02-26 02:12:34.000000 elements-3.2.0/elements/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.2.0/elements/agg.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3370 2023-12-10 19:55:19.000000 elements-3.2.0/elements/checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.2.0/elements/config.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.2.0/elements/counter.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.2.0/elements/flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.2.0/elements/fps.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.2.0/elements/logger.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5616 2023-12-10 19:47:00.000000 elements-3.2.0/elements/path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.2.0/elements/plotting.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.2.0/elements/printing.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.2.0/elements/rwlock.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.2.0/elements/timer.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1160 2023-12-10 19:56:27.000000 elements-3.2.0/elements/tree.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.2.0/elements/usage.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.2.0/elements/utils.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.2.0/elements/uuid.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.2.0/elements/when.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-02-26 02:12:36.933746 elements-3.2.0/elements.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10797 2024-02-26 02:12:36.000000 elements-3.2.0/elements.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      635 2024-02-26 02:12:36.000000 elements-3.2.0/elements.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-02-26 02:12:36.000000 elements-3.2.0/elements.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        6 2024-02-26 02:12:36.000000 elements-3.2.0/elements.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-02-26 02:12:36.000000 elements-3.2.0/elements.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       80 2023-12-13 02:15:19.000000 elements-3.2.0/requirements-optional.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        6 2023-12-10 19:58:55.000000 elements-3.2.0/requirements.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-02-26 02:12:36.941747 elements-3.2.0/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.2.0/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-02-26 02:12:36.941747 elements-3.2.0/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2023-12-10 20:38:32.000000 elements-3.2.0/tests/test_basics.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.2.0/tests/test_flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1506 2023-12-10 20:02:09.000000 elements-3.2.0/tests/test_path.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:03:09.573488 elements-3.3.0/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.3.0/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.3.0/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-10 22:03:09.573488 elements-3.3.0/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.3.0/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:03:09.573488 elements-3.3.0/elements/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      541 2024-05-10 22:02:50.000000 elements-3.3.0/elements/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.3.0/elements/agg.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3370 2023-12-10 19:55:19.000000 elements-3.3.0/elements/checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.3.0/elements/config.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.3.0/elements/counter.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.3.0/elements/flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.3.0/elements/fps.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.3.0/elements/logger.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5616 2023-12-10 19:47:00.000000 elements-3.3.0/elements/path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.3.0/elements/plotting.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.3.0/elements/printing.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.3.0/elements/rwlock.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.3.0/elements/timer.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.3.0/elements/tree.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.3.0/elements/usage.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.3.0/elements/utils.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.3.0/elements/uuid.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.3.0/elements/when.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:03:09.573488 elements-3.3.0/elements.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-10 22:03:09.000000 elements-3.3.0/elements.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      654 2024-05-10 22:03:09.000000 elements-3.3.0/elements.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-10 22:03:09.000000 elements-3.3.0/elements.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        6 2024-05-10 22:03:09.000000 elements-3.3.0/elements.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-10 22:03:09.000000 elements-3.3.0/elements.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       80 2023-12-13 02:15:19.000000 elements-3.3.0/requirements-optional.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        6 2023-12-10 19:58:55.000000 elements-3.3.0/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-10 22:03:09.573488 elements-3.3.0/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.3.0/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-10 22:03:09.573488 elements-3.3.0/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2023-12-10 20:38:32.000000 elements-3.3.0/tests/test_basics.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.3.0/tests/test_flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1506 2024-05-10 21:58:08.000000 elements-3.3.0/tests/test_path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.3.0/tests/test_tree.py
```

### Comparing `elements-3.2.0/LICENSE` & `elements-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/PKG-INFO` & `elements-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.2.0
+Version: 3.3.0
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -224,22 +224,22 @@
 cp.load(pretraining_directory, keys=['model'])
 print(cp.model)
 ```
 
 ### `elements.Timer`
 
 Collect timing statistics about the run time of different parts of a program.
-Measures code inside scopes and can wrap methods into scopes. Returns execution
-count, execution time, fraction of overall program time, and more. The
-resulting statisticse can be added to the logger.
+Measures code inside sections and can wrap methods into sections. Returns
+execution count, execution time, fraction of overall program time, and more.
+The resulting statisticse can be added to the logger.
 
 ```python
 timer = Timer()
 
-timer.scope('foo'):
+timer.section('foo'):
   time.sleep(10)
 
 timer.wrap('name', obj, ['method1', 'method2'])
 obj.method1()
 obj.method1()
 obj.method1()
 obj.method2()
```

### Comparing `elements-3.2.0/README.md` & `elements-3.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -213,22 +213,22 @@
 cp.load(pretraining_directory, keys=['model'])
 print(cp.model)
 ```
 
 ### `elements.Timer`
 
 Collect timing statistics about the run time of different parts of a program.
-Measures code inside scopes and can wrap methods into scopes. Returns execution
-count, execution time, fraction of overall program time, and more. The
-resulting statisticse can be added to the logger.
+Measures code inside sections and can wrap methods into sections. Returns
+execution count, execution time, fraction of overall program time, and more.
+The resulting statisticse can be added to the logger.
 
 ```python
 timer = Timer()
 
-timer.scope('foo'):
+timer.section('foo'):
   time.sleep(10)
 
 timer.wrap('name', obj, ['method1', 'method2'])
 obj.method1()
 obj.method1()
 obj.method1()
 obj.method2()
```

### Comparing `elements-3.2.0/elements/__init__.py` & `elements-3.3.0/elements/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.2.0'
+__version__ = '3.3.0'
 
 from .agg import Agg
 from .checkpoint import Checkpoint
 from .config import Config
 from .counter import Counter
 from .flags import Flags
 from .fps import FPS
```

### Comparing `elements-3.2.0/elements/agg.py` & `elements-3.3.0/elements/agg.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements/checkpoint.py` & `elements-3.3.0/elements/checkpoint.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements/config.py` & `elements-3.3.0/elements/config.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements/counter.py` & `elements-3.3.0/elements/counter.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements/flags.py` & `elements-3.3.0/elements/flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements/logger.py` & `elements-3.3.0/elements/logger.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements/path.py` & `elements-3.3.0/elements/path.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements/plotting.py` & `elements-3.3.0/elements/plotting.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements/printing.py` & `elements-3.3.0/elements/printing.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements/rwlock.py` & `elements-3.3.0/elements/rwlock.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements/timer.py` & `elements-3.3.0/elements/timer.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements/tree.py` & `elements-3.3.0/elements/tree.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 from . import printing
 
 
-def map_(fn, *trees, isleaf=None):
+def map(fn, *trees, isleaf=None):
   assert trees, 'Provide one or more nested Python structures'
   kw = dict(isleaf=isleaf)
   first = trees[0]
-  assert all(isinstance(x, type(first)) for x in trees)
-  if isleaf and isleaf(trees):
-    return fn(*trees)
-  if isinstance(first, list):
-    assert all(len(x) == len(first) for x in trees), printing.format_(trees)
-    return [map_(
-        fn, *[t[i] for t in trees], **kw) for i in range(len(first))]
-  if isinstance(first, tuple):
-    assert all(len(x) == len(first) for x in trees), printing.format_(trees)
-    return tuple([map_(
-        fn, *[t[i] for t in trees], **kw) for i in range(len(first))])
-  if isinstance(first, dict):
-    assert all(set(x.keys()) == set(first.keys()) for x in trees), (
-        printing.format_(trees))
-    return {k: map_(fn, *[t[k] for t in trees], **kw) for k in first}
-  if hasattr(first, 'keys') and hasattr(first, 'get'):
-    assert all(set(x.keys()) == set(first.keys()) for x in trees), (
-        printing.format_(trees))
-    return type(first)(
-        {k: map_(fn, *[t[k] for t in trees], **kw) for k in first})
+  try:
+    assert all(isinstance(x, type(first)) for x in trees)
+    if isleaf and isleaf(trees[0]):
+      return fn(*trees)
+    if isinstance(first, list):
+      assert all(len(x) == len(first) for x in trees)
+      return [map(
+          fn, *[t[i] for t in trees], **kw) for i in range(len(first))]
+    if isinstance(first, tuple):
+      assert all(len(x) == len(first) for x in trees)
+      return tuple([map(
+          fn, *[t[i] for t in trees], **kw) for i in range(len(first))])
+    if isinstance(first, dict):
+      assert all(set(x.keys()) == set(first.keys()) for x in trees)
+      return {k: map(fn, *[t[k] for t in trees], **kw) for k in first}
+    if hasattr(first, 'keys') and hasattr(first, 'get'):
+      assert all(set(x.keys()) == set(first.keys()) for x in trees)
+      return type(first)(
+          {k: map(fn, *[t[k] for t in trees], **kw) for k in first})
+  except AssertionError:
+    raise TypeError(printing.format_(trees))
   return fn(*trees)
 
 
-map = map_
+def flatten(tree, isleaf=None):
+  leaves = []
+  map(lambda x: leaves.append(x), tree, isleaf=isleaf)
+  structure = map(lambda x: None, tree, isleaf=isleaf)
+  return tuple(leaves), structure
+
+
+def unflatten(leaves, structure):
+  leaves = iter(tuple(leaves))
+  return map(lambda x: next(leaves), structure)
```

### Comparing `elements-3.2.0/elements/usage.py` & `elements-3.3.0/elements/usage.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements/uuid.py` & `elements-3.3.0/elements/uuid.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements/when.py` & `elements-3.3.0/elements/when.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/elements.egg-info/PKG-INFO` & `elements-3.3.0/elements.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.2.0
+Version: 3.3.0
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -224,22 +224,22 @@
 cp.load(pretraining_directory, keys=['model'])
 print(cp.model)
 ```
 
 ### `elements.Timer`
 
 Collect timing statistics about the run time of different parts of a program.
-Measures code inside scopes and can wrap methods into scopes. Returns execution
-count, execution time, fraction of overall program time, and more. The
-resulting statisticse can be added to the logger.
+Measures code inside sections and can wrap methods into sections. Returns
+execution count, execution time, fraction of overall program time, and more.
+The resulting statisticse can be added to the logger.
 
 ```python
 timer = Timer()
 
-timer.scope('foo'):
+timer.section('foo'):
   time.sleep(10)
 
 timer.wrap('name', obj, ['method1', 'method2'])
 obj.method1()
 obj.method1()
 obj.method1()
 obj.method2()
```

### Comparing `elements-3.2.0/setup.py` & `elements-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/tests/test_basics.py` & `elements-3.3.0/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/tests/test_flags.py` & `elements-3.3.0/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.2.0/tests/test_path.py` & `elements-3.3.0/tests/test_path.py`

 * *Files identical despite different names*

