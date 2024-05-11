# Comparing `tmp/pynrw-1.1.1.tar.gz` & `tmp/pynrw-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynrw-1.1.1.tar", last modified: Wed May  8 14:18:46 2024, max compression
+gzip compressed data, was "pynrw-1.2.0.tar", last modified: Sat May 11 01:11:39 2024, max compression
```

## Comparing `pynrw-1.1.1.tar` & `pynrw-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:18:46.272993 pynrw-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 14:18:35.000000 pynrw-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-05-08 14:18:46.272993 pynrw-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-05-08 14:18:35.000000 pynrw-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:18:46.264993 pynrw-1.1.1/nrw/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:18:46.264993 pynrw-1.1.1/nrw/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/algorithms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/algorithms/_searching.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/algorithms/_searching.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/algorithms/_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/algorithms/_sorting.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/algorithms/_traversal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/algorithms/_traversal.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:18:46.268993 pynrw-1.1.1/nrw/datastructures/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_binary_search_tree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_binary_tree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_comparable_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_edge.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_graph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_list.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_queue.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_stack.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_vertex.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/datastructures/_vertex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 14:18:35.000000 pynrw-1.1.1/nrw/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:18:46.268993 pynrw-1.1.1/pynrw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-05-08 14:18:46.000000 pynrw-1.1.1/pynrw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-08 14:18:46.000000 pynrw-1.1.1/pynrw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:18:46.000000 pynrw-1.1.1/pynrw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-08 14:18:46.000000 pynrw-1.1.1/pynrw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 14:18:46.000000 pynrw-1.1.1/pynrw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-08 14:18:35.000000 pynrw-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:18:46.272993 pynrw-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:11:39.141213 pynrw-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-11 01:11:29.000000 pynrw-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-11 01:11:39.137213 pynrw-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-11 01:11:29.000000 pynrw-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:11:39.133213 pynrw-1.2.0/nrw/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:11:39.133213 pynrw-1.2.0/nrw/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/algorithms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/algorithms/_searching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/algorithms/_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/algorithms/_traversal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:11:39.137213 pynrw-1.2.0/nrw/datastructures/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_binary_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_binary_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_comparable_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/datastructures/_vertex.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 01:11:29.000000 pynrw-1.2.0/nrw/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:11:39.137213 pynrw-1.2.0/pynrw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-11 01:11:39.000000 pynrw-1.2.0/pynrw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-11 01:11:39.000000 pynrw-1.2.0/pynrw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:11:39.000000 pynrw-1.2.0/pynrw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-11 01:11:39.000000 pynrw-1.2.0/pynrw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-11 01:11:39.000000 pynrw-1.2.0/pynrw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-05-11 01:11:29.000000 pynrw-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 01:11:39.141213 pynrw-1.2.0/setup.cfg
```

### Comparing `pynrw-1.1.1/LICENSE` & `pynrw-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynrw-1.1.1/PKG-INFO` & `pynrw-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrw
-Version: 1.1.1
+Version: 1.2.0
 Summary: Materialien zu den zentralen NRW-Abiturprüfungen im Fach Informatik ab 2018 implementiert in Python.
 Author: realshouzy
 License: MIT
 Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung,abitur
 Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -37,15 +37,15 @@
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/realshouzy/pynrw/main.svg)](https://results.pre-commit.ci/latest/github/realshouzy/pynrw/main)
 [![pylint status](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml)
 [![test status](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml)
 [![CodeQL](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml)
 [![PyPI - Version](https://img.shields.io/pypi/v/pynrw)](https://github.com/realshouzy/pynrw/releases/latest)
 [![Python versions](https://img.shields.io/pypi/pyversions/pynrw.svg)](https://pypi.org/project/pynrw/)
-[![semantic-release](https://img.shields.io/badge/%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/realshouzy/YTDownloader/releases)
+[![semantic-release](https://img.shields.io/badge/%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/realshouzy/pynrw/releases)
 [![PyPI - Format](https://img.shields.io/pypi/format/pynrw)](https://pypi.org/project/pynrw/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/realshouzy/pynrw/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 This package implements the datastructures given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
@@ -63,17 +63,37 @@
 - [`BinarySearchTree`](/nrw/datastructures/_binary_search_tree.py)
 - [`Vertex`](/nrw/datastructures/_vertex.py)
 - [`Edge`](/nrw/datastructures/_edge.py)
 - [`Graph`](/nrw/datastructures/_graph.py)
 
 Die Implementation ist semantisch identisch zu der Implementation des Landes mit dem einzigen Unterschied, dass alles mehr *pythonic* ist, d.h. die Benennung der Methoden folgt [`pep8`](https://peps.python.org/pep-0008/), `Getter` und `Setter` sind, wo es sinnvoll ist, in [`properties`](https://docs.python.org/3/library/functions.html#property) transformiert und die Dokumentation (*doc strings*) sind ebenfalls angepasst worden.
 
-Das Interface `ComparableContent` ist ein gleichnamiges [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol), definiert in [`nrw.datastructures._comparable_content`](/nrw/datastructures/_comparable_content.py). Es gibt die [*dunder special methods*](https://docs.python.org/3/reference/datamodel.html#object.__lt__), `__eq__`, `__lt__` und `__gt__` für einfache Vergleichsoperationen vor. Das Module stellt auch ein `TypeVar`(<https://docs.python.org/3/library/typing.html#typing.TypeVar>) `ComparableContentT` zur Verfügung.
+Das Interface `ComparableContent` ist ein gleichnamiges [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol), definiert in [`nrw.datastructures._comparable_content`](/nrw/datastructures/_comparable_content.py). Es gibt die [*dunder special methods*](https://docs.python.org/3/reference/datamodel.html#object.__lt__), `__eq__`, `__lt__` und `__gt__` für einfache Vergleichsoperationen vor. Das Module stellt auch ein [`TypeVar`](https://docs.python.org/3/library/typing.html#typing.TypeVar) `ComparableContentT` zur Verfügung.
 
-Außerdem implementieren die linearen Datenstrukturen `__str__`, welches das Arbeiten mit diesen deutlich vereinfacht.
+Außerdem implementieren die Datenstrukturen `__str__`, welches das Arbeiten mit diesen deutlich vereinfacht (besonders für `Binary(Search)Tree`) und `__repr__`, welches eine grobe Idee der internen Strukture gibt, z.B.:
+
+```python
+from nrw.datastructures import BinarySearchTree
+
+bst: BinarySearchTree[int] = BinarySearchTree()
+bst.insert(3)
+bst.insert(2)
+bst.insert(5)
+bst.insert(0)
+bst.insert(1)
+bst.insert(4)
+print(bst)
+#    _4_
+#   /   \
+#  _2   6
+# /  \ /
+# 0  3 5
+#  \
+#  1
+```
 
 Des weiteren sind (triviale) Optimierungen vorgenommen worden:
 
 - Verwendung von [`__slots__`](https://docs.python.org/3/reference/datamodel.html#slots)
 - redundante Aufrufe werden weggelassen
 - interne Optimierungen bei Zuweisungen
 
@@ -89,15 +109,15 @@
 - [`quick_sort`](/nrw/algorithms/_sorting.py)
 - [`preorder`](/nrw/algorithms/_traversal.py)
 - [`inorder`](/nrw/algorithms/_traversal.py)
 - [`reverse_inorder`](/nrw/algorithms/_traversal.py)
 - [`postorder`](/nrw/algorithms/_traversal.py)
 - [`levelorder`](/nrw/algorithms/_traversal.py)
 
-Allerdings muss annotiert werden, dass aufgrund den Natur der Datastrukturen, wie sie vom Land vorgegeben werden, die Laufzeiten nicht optimal sind. Zudem kann es zu ungewollten Nebeneffekte für die Argumente kommen. Welche dies sind, wird dem Leser als Übung überlassen. Es soll nicht vor einem Blick in den Quellcode zurückgeschreckt werden.
+Allerdings muss annotiert werden, dass aufgrund der Vorgaben des Landes die Laufzeiten nicht optimal sind. Zudem kann es zu ungewollten Nebeneffekte kommen. Welche dies sind, wird dem Leser als Übung überlassen. Es soll nicht vor einem Blick in den Quellcode zurückgeschreckt werden.
 
 Für Hilfe zum jeweiligen Objekt (gilt für alle oben genannte Objekte), z.B.:
 
 ```python
 from nrw.datastructures import List
 help(List)
 help(List.insert)
```

### Comparing `pynrw-1.1.1/README.md` & `pynrw-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/realshouzy/pynrw/main.svg)](https://results.pre-commit.ci/latest/github/realshouzy/pynrw/main)
 [![pylint status](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml)
 [![test status](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml)
 [![CodeQL](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml)
 [![PyPI - Version](https://img.shields.io/pypi/v/pynrw)](https://github.com/realshouzy/pynrw/releases/latest)
 [![Python versions](https://img.shields.io/pypi/pyversions/pynrw.svg)](https://pypi.org/project/pynrw/)
-[![semantic-release](https://img.shields.io/badge/%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/realshouzy/YTDownloader/releases)
+[![semantic-release](https://img.shields.io/badge/%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/realshouzy/pynrw/releases)
 [![PyPI - Format](https://img.shields.io/pypi/format/pynrw)](https://pypi.org/project/pynrw/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/realshouzy/pynrw/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 This package implements the datastructures given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
@@ -28,17 +28,37 @@
 - [`BinarySearchTree`](/nrw/datastructures/_binary_search_tree.py)
 - [`Vertex`](/nrw/datastructures/_vertex.py)
 - [`Edge`](/nrw/datastructures/_edge.py)
 - [`Graph`](/nrw/datastructures/_graph.py)
 
 Die Implementation ist semantisch identisch zu der Implementation des Landes mit dem einzigen Unterschied, dass alles mehr *pythonic* ist, d.h. die Benennung der Methoden folgt [`pep8`](https://peps.python.org/pep-0008/), `Getter` und `Setter` sind, wo es sinnvoll ist, in [`properties`](https://docs.python.org/3/library/functions.html#property) transformiert und die Dokumentation (*doc strings*) sind ebenfalls angepasst worden.
 
-Das Interface `ComparableContent` ist ein gleichnamiges [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol), definiert in [`nrw.datastructures._comparable_content`](/nrw/datastructures/_comparable_content.py). Es gibt die [*dunder special methods*](https://docs.python.org/3/reference/datamodel.html#object.__lt__), `__eq__`, `__lt__` und `__gt__` für einfache Vergleichsoperationen vor. Das Module stellt auch ein `TypeVar`(<https://docs.python.org/3/library/typing.html#typing.TypeVar>) `ComparableContentT` zur Verfügung.
+Das Interface `ComparableContent` ist ein gleichnamiges [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol), definiert in [`nrw.datastructures._comparable_content`](/nrw/datastructures/_comparable_content.py). Es gibt die [*dunder special methods*](https://docs.python.org/3/reference/datamodel.html#object.__lt__), `__eq__`, `__lt__` und `__gt__` für einfache Vergleichsoperationen vor. Das Module stellt auch ein [`TypeVar`](https://docs.python.org/3/library/typing.html#typing.TypeVar) `ComparableContentT` zur Verfügung.
 
-Außerdem implementieren die linearen Datenstrukturen `__str__`, welches das Arbeiten mit diesen deutlich vereinfacht.
+Außerdem implementieren die Datenstrukturen `__str__`, welches das Arbeiten mit diesen deutlich vereinfacht (besonders für `Binary(Search)Tree`) und `__repr__`, welches eine grobe Idee der internen Strukture gibt, z.B.:
+
+```python
+from nrw.datastructures import BinarySearchTree
+
+bst: BinarySearchTree[int] = BinarySearchTree()
+bst.insert(3)
+bst.insert(2)
+bst.insert(5)
+bst.insert(0)
+bst.insert(1)
+bst.insert(4)
+print(bst)
+#    _4_
+#   /   \
+#  _2   6
+# /  \ /
+# 0  3 5
+#  \
+#  1
+```
 
 Des weiteren sind (triviale) Optimierungen vorgenommen worden:
 
 - Verwendung von [`__slots__`](https://docs.python.org/3/reference/datamodel.html#slots)
 - redundante Aufrufe werden weggelassen
 - interne Optimierungen bei Zuweisungen
 
@@ -54,15 +74,15 @@
 - [`quick_sort`](/nrw/algorithms/_sorting.py)
 - [`preorder`](/nrw/algorithms/_traversal.py)
 - [`inorder`](/nrw/algorithms/_traversal.py)
 - [`reverse_inorder`](/nrw/algorithms/_traversal.py)
 - [`postorder`](/nrw/algorithms/_traversal.py)
 - [`levelorder`](/nrw/algorithms/_traversal.py)
 
-Allerdings muss annotiert werden, dass aufgrund den Natur der Datastrukturen, wie sie vom Land vorgegeben werden, die Laufzeiten nicht optimal sind. Zudem kann es zu ungewollten Nebeneffekte für die Argumente kommen. Welche dies sind, wird dem Leser als Übung überlassen. Es soll nicht vor einem Blick in den Quellcode zurückgeschreckt werden.
+Allerdings muss annotiert werden, dass aufgrund der Vorgaben des Landes die Laufzeiten nicht optimal sind. Zudem kann es zu ungewollten Nebeneffekte kommen. Welche dies sind, wird dem Leser als Übung überlassen. Es soll nicht vor einem Blick in den Quellcode zurückgeschreckt werden.
 
 Für Hilfe zum jeweiligen Objekt (gilt für alle oben genannte Objekte), z.B.:
 
 ```python
 from nrw.datastructures import List
 help(List)
 help(List.insert)
```

### Comparing `pynrw-1.1.1/nrw/algorithms/__init__.py` & `pynrw-1.2.0/nrw/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.1.1/nrw/algorithms/_searching.py` & `pynrw-1.2.0/nrw/algorithms/_searching.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.1.1/nrw/algorithms/_sorting.py` & `pynrw-1.2.0/nrw/algorithms/_sorting.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.1.1/nrw/algorithms/_traversal.py` & `pynrw-1.2.0/nrw/algorithms/_traversal.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.1.1/nrw/algorithms/_traversal.pyi` & `pynrw-1.2.0/nrw/algorithms/__init__.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,44 @@
 __all__: Final[tuple[str, ...]] = (
+    "linear_search",
+    "depth_first_search",
+    "breadth_first_search",
+    "bubble_sort",
+    "selection_sort",
+    "insertion_sort",
+    "merge_sort",
+    "quick_sort",
     "preorder",
     "inorder",
     "reverse_inorder",
     "postorder",
     "levelorder",
 )
 
 from typing import Final, TypeVar, overload
 
-from nrw.datastructures import BinarySearchTree, BinaryTree, ComparableContentT, List
+from nrw.datastructures import (
+    BinarySearchTree,
+    BinaryTree,
+    ComparableContentT,
+    Graph,
+    List,
+    Vertex,
+)
 
 _T = TypeVar("_T")
 
+def linear_search(lst: List[_T], element: _T) -> int: ...
+def depth_first_search(graph: Graph, vertex: Vertex) -> List[Vertex]: ...
+def breadth_first_search(graph: Graph, vertex: Vertex) -> List[Vertex]: ...
+def bubble_sort(lst: List[ComparableContentT]) -> List[ComparableContentT]: ...
+def selection_sort(lst: List[ComparableContentT]) -> List[ComparableContentT]: ...
+def insertion_sort(lst: List[ComparableContentT]) -> List[ComparableContentT]: ...
+def merge_sort(lst: List[ComparableContentT]) -> List[ComparableContentT]: ...
+def quick_sort(lst: List[ComparableContentT]) -> List[ComparableContentT]: ...
 @overload
 def preorder(tree: BinaryTree[_T]) -> List[_T]: ...
 @overload
 def preorder(
     tree: BinarySearchTree[ComparableContentT],
 ) -> List[ComparableContentT]: ...
 @overload
```

### Comparing `pynrw-1.1.1/nrw/datastructures/__init__.py` & `pynrw-1.2.0/nrw/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.1.1/nrw/datastructures/_binary_search_tree.py` & `pynrw-1.2.0/nrw/datastructures/_binary_search_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Implementation der generischen Klasse `BinarySearchTree[ComparableContentT]`."""
 
 from __future__ import annotations
 
 from typing import Final, Generic
 
 from nrw.datastructures._comparable_content import ComparableContentT
+from nrw.datastructures._utils import display_binary_node
 
 
 class _BSTNode(Generic[ComparableContentT]):
     """Durch diese innere Klasse kann man dafür sorgen, dass ein leerer Baum
     `None` ist, ein nicht-leerer Baum jedoch immer eine nicht-`None`-Wurzel sowie
     nicht-`None`-Teilbäume hat.
     """
@@ -17,14 +18,23 @@
     __hash__ = None  # type: ignore[assignment]
 
     def __init__(self, content: ComparableContentT) -> None:
         self._content: ComparableContentT = content
         self._left: BinarySearchTree[ComparableContentT] = BinarySearchTree()
         self._right: BinarySearchTree[ComparableContentT] = BinarySearchTree()
 
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}(content={self._content!r}, "
+            f"left_tree={self._left!r}, right_tree={self._right!r})"
+        )
+
+    def __str__(self) -> str:
+        return display_binary_node(self)
+
 
 class BinarySearchTree(Generic[ComparableContentT]):
     """Mithilfe der generischen Klasse `BinarySearchTree` können beliebig viele
     Objekte in einem Binaerbaum (binaerer Suchbaum) entsprechend einer
     Ordnungsrelation verwaltet werden.
 
     Ein Objekt der Klasse stellt entweder einen leeren binären Suchbaum dar oder
@@ -48,14 +58,22 @@
     __slots__: Final[tuple[str]] = ("_node",)
     __hash__ = None  # type: ignore[assignment]
 
     def __init__(self) -> None:
         """Der Konstruktor erzeugt einen leeren Suchbaum."""
         self._node: _BSTNode[ComparableContentT] | None = None
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(node={self._node!r})"
+
+    def __str__(self) -> str:
+        if self.is_empty:
+            return ""
+        return str(self._node)
+
     @property
     def is_empty(self) -> bool:
         """Diese Anfrage liefert den Wahrheitswert `True`, wenn der Suchbaum leer ist,
         sonst liefert sie den Wert `False`.
         """
         return self._node is None
```

### Comparing `pynrw-1.1.1/nrw/datastructures/_binary_tree.py` & `pynrw-1.2.0/nrw/datastructures/_binary_tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from __future__ import annotations
 
 __all__: Final[tuple[str]] = ("BinaryTree",)
 
 from typing import Final, Generic, TypeVar
 
+from nrw.datastructures._utils import display_binary_node
+
 _T = TypeVar("_T")
 
 
 class _BTNode(Generic[_T]):
     """Durch diese innere Klasse kann man dafür sorgen, dass ein leerer Baum `None`
     ist, ein nicht-leerer Baum jedoch immer eine nicht-`None`-Wurzel sowie
     nicht-`None`-Teilbäume, ggf. leere Teilbäume hat.
@@ -19,14 +21,23 @@
     __hash__ = None  # type: ignore[assignment]
 
     def __init__(self, content: _T) -> None:
         self._content: _T = content
         self._left: BinaryTree[_T] | None = BinaryTree()
         self._right: BinaryTree[_T] | None = BinaryTree()
 
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}(content={self._content!r}, "
+            f"left_tree={self._left!r}, right_tree={self._right!r})"
+        )
+
+    def __str__(self) -> str:
+        return display_binary_node(self)
+
 
 class BinaryTree(Generic[_T]):
     """Mithilfe der generischen Klasse `BinaryTree` können beliebig viele
     Inhaltsobjekte in einem Binaerbaum verwaltet werden. Ein
     Objekt der Klasse stellt entweder einen leeren Baum dar oder verwaltet ein
     Inhaltsobjekt sowie einen linken und einen rechten Teilbaum, die ebenfalls
     Objekte der generischen Klasse `BinaryTree` sind.
@@ -62,14 +73,22 @@
         if content is None:
             self._node: _BTNode[_T] | None = None
         else:
             self._node = _BTNode(content)
             self._node._left = left_tree if left_tree is not None else BinaryTree()
             self._node._right = right_tree if right_tree is not None else BinaryTree()
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(node={self._node!r})"
+
+    def __str__(self) -> str:
+        if self.is_empty:
+            return ""
+        return str(self._node)
+
     @property
     def is_empty(self) -> bool:
         """Diese Anfrage liefert das Inhaltsobjekt des Binaerbaums. Wenn der Binaerbaum
         leer ist, wird `None` zurueckgegeben.
         """
         return self._node is None
```

### Comparing `pynrw-1.1.1/nrw/datastructures/_comparable_content.py` & `pynrw-1.2.0/nrw/datastructures/_comparable_content.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.1.1/nrw/datastructures/_edge.py` & `pynrw-1.2.0/nrw/datastructures/_edge.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,24 @@
         repraesentierte Kante verbindet die Knoten `vertex` und `another_vertex` mit der
         Gewichtung `weight`. Ihre Markierung hat den Wert `False`.
         """
         self._vertices: tuple[Vertex, Vertex] = (vertex, another_vertex)
         self._weight: int = weight
         self._mark: bool = False
 
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}(vertices={self._vertices!r}, "
+            f"weight={self._weight!r}, mark={self._mark!r})"
+        )
+
+    def __str__(self) -> str:
+        vertex1, vertex2 = self._vertices
+        return f"{vertex1} --{self._weight}-- {vertex2}"
+
     @property
     def vertices(self) -> tuple[Vertex, Vertex]:
         """Die Anfrage gibt die beiden Knoten, die durch die Kante verbunden werden,
         als `tuple` vom Typ `Vertex` zurück.
         Das `tuple` hat genau zwei Einträge mit den Indexwerten 0 und 1.
         """
         return self._vertices
```

### Comparing `pynrw-1.1.1/nrw/datastructures/_graph.py` & `pynrw-1.2.0/nrw/datastructures/_graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Implementation der Klasse `Graph`."""
 
 from __future__ import annotations
 
 __all__: Final[tuple[str]] = ("Graph",)
 
+from io import StringIO
 from typing import TYPE_CHECKING, Final
 
 from nrw.datastructures._list import List
 
 if TYPE_CHECKING:
     from nrw.datastructures._edge import Edge
     from nrw.datastructures._vertex import Vertex
@@ -32,14 +33,34 @@
     def __init__(self) -> None:
         """Ein Objekt vom Typ `Graph` wird erstellt.
         Der von diesem Objekt repraesentierte Graph ist leer.
         """
         self._vertices: List[Vertex] = List()
         self._edges: List[Edge] = List()
 
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}(vertices={self._vertices!r}, "
+            f"edges={self._edges!r})"
+        )
+
+    def __str__(self) -> str:
+        if self.is_empty:
+            return f"{self.__class__.__name__}()"
+
+        with StringIO() as buffer:
+            buffer.write(f"{self.__class__.__name__}(")
+            self._vertices.to_first()
+            while self._vertices.has_access:
+                current: Vertex | None = self._vertices.content
+                assert current is not None
+                buffer.write(f"{current} -> {self.get_neighbours(current)}, ")
+                self._vertices.next()
+            return f"{buffer.getvalue().rstrip(', ')})"
+
     @property
     def vertices(self) -> List[Vertex]:
         """Die Anfrage liefert eine neue Liste aller Knotenobjekte
         vom Typ `List[Vertex]`.
         """
         result: List[Vertex] = List()
         self._vertices.to_first()
```

### Comparing `pynrw-1.1.1/nrw/datastructures/_list.py` & `pynrw-1.2.0/nrw/datastructures/_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,20 @@
     def __init__(self, content: _T) -> None:
         """Ein neues Objekt vom Typ `_ListNode[_T]` wird erschaffen.
         Der Inhalt wird per Parameter gesetzt. Der Verweis ist leer.
         """
         self._content: _T = content
         self._next_node: _ListNode[_T] | None = None
 
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}(content={self._content!r}, "
+            f"next_node={self._next_node!r})"
+        )
+
     @property
     def content(self) -> _T:
         """Liefert das Inhaltsobjekt des Knotens."""
         return self._content
 
     @content.setter
     def content(self, new_content: _T) -> None:
@@ -60,14 +66,20 @@
 
     def __init__(self) -> None:
         """Eine leere Liste wird erzeugt."""
         self._first: _ListNode[_T] | None = None
         self._last: _ListNode[_T] | None = None
         self._current: _ListNode[_T] | None = None
 
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}(first={self._first!r}, last={self._last!r}, "
+            f"current={self._current!r})"
+        )
+
     def __str__(self) -> str:
         if self.is_empty:
             return f"{self.__class__.__name__}()"
 
         with StringIO() as buffer:
             buffer.write(f"{self.__class__.__name__}(")
             temp: _ListNode[_T] | None = self._first
```

### Comparing `pynrw-1.1.1/nrw/datastructures/_queue.py` & `pynrw-1.2.0/nrw/datastructures/_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,20 @@
     def __init__(self, content: _T) -> None:
         """Ein neues Objekt vom Typ `_QueueNode[_T]` wird erschaffen.
         Der Inhalt wird per Parameter gesetzt. Der Verweis ist leer.
         """
         self._content: _T = content
         self._next_node: _QueueNode[_T] | None = None
 
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}(content={self._content!r}, "
+            f"next_node={self._next_node!r})"
+        )
+
     @property
     def content(self) -> _T:
         """Liefert das Inhaltsobjekt des Knotens."""
         return self._content
 
     @property
     def next_node(self) -> _QueueNode[_T] | None:
@@ -47,14 +53,17 @@
     __hash__ = None  # type: ignore[assignment]
 
     def __init__(self) -> None:
         """Eine leere Schlange wird erzeugt."""
         self._head: _QueueNode[_T] | None = None
         self._tail: _QueueNode[_T] | None = None
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(head={self._head!r}, tail={self._tail!r})"
+
     def __str__(self) -> str:
         if self.is_empty:
             return f"{self.__class__.__name__}()"
 
         with StringIO() as buffer:
             buffer.write(f"{self.__class__.__name__}(")
             temp: _QueueNode[_T] | None = self._head
```

### Comparing `pynrw-1.1.1/nrw/datastructures/_stack.py` & `pynrw-1.2.0/nrw/datastructures/_stack.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,20 @@
     def __init__(self, content: _T) -> None:
         """Ein neues Objekt vom Typ `_StackNode[_T]` wird erschaffen.
         Der Inhalt wird per Parameter gesetzt. Der Verweis ist leer.
         """
         self._content: _T = content
         self._next_node: _StackNode[_T] | None = None
 
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}(content={self._content!r}, "
+            f"next_node={self._next_node!r})"
+        )
+
     @property
     def content(self) -> _T:
         """Liefert das Inhaltsobjekt des Knotens."""
         return self._content
 
     @property
     def next_node(self) -> _StackNode[_T] | None:
@@ -47,14 +53,17 @@
     __slots__: Final[tuple[str]] = ("_head",)
     __hash__ = None  # type: ignore[assignment]
 
     def __init__(self) -> None:
         """Ein leerer Stapel wird erzeugt."""
         self._head: _StackNode[_T] | None = None
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(head={self._head!r})"
+
     def __str__(self) -> str:
         if self.is_empty:
             return f"{self.__class__.__name__}()"
 
         with StringIO() as buffer:
             buffer.write(f"{self.__class__.__name__}(")
             temp: _StackNode[_T] | None = self._head
```

### Comparing `pynrw-1.1.1/nrw/datastructures/_vertex.py` & `pynrw-1.2.0/nrw/datastructures/_vertex.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,20 @@
     def __init__(self, id_: str) -> None:
         """Ein neues Objekt vom Typ `Vertex` wird erstellt.
         Seine Markierung hat den Wert `False`.
         """
         self._id: str = id_
         self._mark: bool = False
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}(id={self._id!r}, mark={self._mark!r})"
+
+    def __str__(self) -> str:
+        return self._id
+
     @property
     def id(self) -> str:
         """Die Anfrage liefert die ID des Knotens als String."""
         return self._id
 
     @property
     def mark(self) -> bool:
```

### Comparing `pynrw-1.1.1/pynrw.egg-info/PKG-INFO` & `pynrw-1.2.0/pynrw.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrw
-Version: 1.1.1
+Version: 1.2.0
 Summary: Materialien zu den zentralen NRW-Abiturprüfungen im Fach Informatik ab 2018 implementiert in Python.
 Author: realshouzy
 License: MIT
 Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung,abitur
 Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -37,15 +37,15 @@
 
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/realshouzy/pynrw/main.svg)](https://results.pre-commit.ci/latest/github/realshouzy/pynrw/main)
 [![pylint status](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/pylint.yaml)
 [![test status](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/test.yaml)
 [![CodeQL](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml/badge.svg)](https://github.com/realshouzy/pynrw/actions/workflows/codeql.yaml)
 [![PyPI - Version](https://img.shields.io/pypi/v/pynrw)](https://github.com/realshouzy/pynrw/releases/latest)
 [![Python versions](https://img.shields.io/pypi/pyversions/pynrw.svg)](https://pypi.org/project/pynrw/)
-[![semantic-release](https://img.shields.io/badge/%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/realshouzy/YTDownloader/releases)
+[![semantic-release](https://img.shields.io/badge/%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/realshouzy/pynrw/releases)
 [![PyPI - Format](https://img.shields.io/pypi/format/pynrw)](https://pypi.org/project/pynrw/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/realshouzy/pynrw/blob/main/LICENSE)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 This package implements the datastructures given by the German state NRW in Python, thus futher documentation will be in German. This code is purely intended for educational purposes and should not be used in production!
@@ -63,17 +63,37 @@
 - [`BinarySearchTree`](/nrw/datastructures/_binary_search_tree.py)
 - [`Vertex`](/nrw/datastructures/_vertex.py)
 - [`Edge`](/nrw/datastructures/_edge.py)
 - [`Graph`](/nrw/datastructures/_graph.py)
 
 Die Implementation ist semantisch identisch zu der Implementation des Landes mit dem einzigen Unterschied, dass alles mehr *pythonic* ist, d.h. die Benennung der Methoden folgt [`pep8`](https://peps.python.org/pep-0008/), `Getter` und `Setter` sind, wo es sinnvoll ist, in [`properties`](https://docs.python.org/3/library/functions.html#property) transformiert und die Dokumentation (*doc strings*) sind ebenfalls angepasst worden.
 
-Das Interface `ComparableContent` ist ein gleichnamiges [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol), definiert in [`nrw.datastructures._comparable_content`](/nrw/datastructures/_comparable_content.py). Es gibt die [*dunder special methods*](https://docs.python.org/3/reference/datamodel.html#object.__lt__), `__eq__`, `__lt__` und `__gt__` für einfache Vergleichsoperationen vor. Das Module stellt auch ein `TypeVar`(<https://docs.python.org/3/library/typing.html#typing.TypeVar>) `ComparableContentT` zur Verfügung.
+Das Interface `ComparableContent` ist ein gleichnamiges [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol), definiert in [`nrw.datastructures._comparable_content`](/nrw/datastructures/_comparable_content.py). Es gibt die [*dunder special methods*](https://docs.python.org/3/reference/datamodel.html#object.__lt__), `__eq__`, `__lt__` und `__gt__` für einfache Vergleichsoperationen vor. Das Module stellt auch ein [`TypeVar`](https://docs.python.org/3/library/typing.html#typing.TypeVar) `ComparableContentT` zur Verfügung.
 
-Außerdem implementieren die linearen Datenstrukturen `__str__`, welches das Arbeiten mit diesen deutlich vereinfacht.
+Außerdem implementieren die Datenstrukturen `__str__`, welches das Arbeiten mit diesen deutlich vereinfacht (besonders für `Binary(Search)Tree`) und `__repr__`, welches eine grobe Idee der internen Strukture gibt, z.B.:
+
+```python
+from nrw.datastructures import BinarySearchTree
+
+bst: BinarySearchTree[int] = BinarySearchTree()
+bst.insert(3)
+bst.insert(2)
+bst.insert(5)
+bst.insert(0)
+bst.insert(1)
+bst.insert(4)
+print(bst)
+#    _4_
+#   /   \
+#  _2   6
+# /  \ /
+# 0  3 5
+#  \
+#  1
+```
 
 Des weiteren sind (triviale) Optimierungen vorgenommen worden:
 
 - Verwendung von [`__slots__`](https://docs.python.org/3/reference/datamodel.html#slots)
 - redundante Aufrufe werden weggelassen
 - interne Optimierungen bei Zuweisungen
 
@@ -89,15 +109,15 @@
 - [`quick_sort`](/nrw/algorithms/_sorting.py)
 - [`preorder`](/nrw/algorithms/_traversal.py)
 - [`inorder`](/nrw/algorithms/_traversal.py)
 - [`reverse_inorder`](/nrw/algorithms/_traversal.py)
 - [`postorder`](/nrw/algorithms/_traversal.py)
 - [`levelorder`](/nrw/algorithms/_traversal.py)
 
-Allerdings muss annotiert werden, dass aufgrund den Natur der Datastrukturen, wie sie vom Land vorgegeben werden, die Laufzeiten nicht optimal sind. Zudem kann es zu ungewollten Nebeneffekte für die Argumente kommen. Welche dies sind, wird dem Leser als Übung überlassen. Es soll nicht vor einem Blick in den Quellcode zurückgeschreckt werden.
+Allerdings muss annotiert werden, dass aufgrund der Vorgaben des Landes die Laufzeiten nicht optimal sind. Zudem kann es zu ungewollten Nebeneffekte kommen. Welche dies sind, wird dem Leser als Übung überlassen. Es soll nicht vor einem Blick in den Quellcode zurückgeschreckt werden.
 
 Für Hilfe zum jeweiligen Objekt (gilt für alle oben genannte Objekte), z.B.:
 
 ```python
 from nrw.datastructures import List
 help(List)
 help(List.insert)
```

### Comparing `pynrw-1.1.1/pynrw.egg-info/SOURCES.txt` & `pynrw-1.2.0/pynrw.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -3,36 +3,26 @@
 pyproject.toml
 nrw/__init__.py
 nrw/__init__.pyi
 nrw/py.typed
 nrw/algorithms/__init__.py
 nrw/algorithms/__init__.pyi
 nrw/algorithms/_searching.py
-nrw/algorithms/_searching.pyi
 nrw/algorithms/_sorting.py
-nrw/algorithms/_sorting.pyi
 nrw/algorithms/_traversal.py
-nrw/algorithms/_traversal.pyi
 nrw/datastructures/__init__.py
 nrw/datastructures/__init__.pyi
 nrw/datastructures/_binary_search_tree.py
-nrw/datastructures/_binary_search_tree.pyi
 nrw/datastructures/_binary_tree.py
-nrw/datastructures/_binary_tree.pyi
 nrw/datastructures/_comparable_content.py
 nrw/datastructures/_edge.py
-nrw/datastructures/_edge.pyi
 nrw/datastructures/_graph.py
-nrw/datastructures/_graph.pyi
 nrw/datastructures/_list.py
-nrw/datastructures/_list.pyi
 nrw/datastructures/_queue.py
-nrw/datastructures/_queue.pyi
 nrw/datastructures/_stack.py
-nrw/datastructures/_stack.pyi
+nrw/datastructures/_utils.py
 nrw/datastructures/_vertex.py
-nrw/datastructures/_vertex.pyi
 pynrw.egg-info/PKG-INFO
 pynrw.egg-info/SOURCES.txt
 pynrw.egg-info/dependency_links.txt
 pynrw.egg-info/requires.txt
 pynrw.egg-info/top_level.txt
```

### Comparing `pynrw-1.1.1/pyproject.toml` & `pynrw-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,15 @@
   "D205",
   "UP035",
   "UP036",
   "SLF001",
   "FBT001",
   "S101",
   "PYI026",
+  "B905",
 ]
 lint.fixable = ["ALL"]
 lint.unfixable = []
 show-fixes = true
 target-version = "py312"
 line-length = 88
 
@@ -123,15 +124,15 @@
 known-first-party = ["nrw"]
 required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "pep257"
 
 [tool.pylint]
-disable = ["C0116", "R0801", "W0212", "R0903"]
+disable = ["C0116", "R0801", "W0212", "R0903", "C0114"]
 load-plugins = "pylint_pytest"
 
 [tool.bandit]
 skips = ["B101"]
 exclude_dirs = ["tests"]
 
 [tool.pytest.ini_options]
```

