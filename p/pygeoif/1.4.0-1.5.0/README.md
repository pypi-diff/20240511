# Comparing `tmp/pygeoif-1.4.0.tar.gz` & `tmp/pygeoif-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoif-1.4.0.tar", last modified: Mon Mar 25 17:58:17 2024, max compression
+gzip compressed data, was "pygeoif-1.5.0.tar", last modified: Sat May 11 12:44:55 2024, max compression
```

## Comparing `pygeoif-1.4.0.tar` & `pygeoif-1.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:58:17.435458 pygeoif-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    14528 2024-03-25 17:58:17.435458 pygeoif-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-03-25 17:58:13.000000 pygeoif-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:58:17.427457 pygeoif-1.4.0/pygeoif/
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-25 17:58:13.000000 pygeoif-1.4.0/pygeoif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-25 17:58:13.000000 pygeoif-1.4.0/pygeoif/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-25 17:58:13.000000 pygeoif-1.4.0/pygeoif/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-03-25 17:58:13.000000 pygeoif-1.4.0/pygeoif/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-03-25 17:58:13.000000 pygeoif-1.4.0/pygeoif/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2024-03-25 17:58:13.000000 pygeoif-1.4.0/pygeoif/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    32657 2024-03-25 17:58:13.000000 pygeoif-1.4.0/pygeoif/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:58:17.427457 pygeoif-1.4.0/pygeoif/hypothesis/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-25 17:58:13.000000 pygeoif-1.4.0/pygeoif/hypothesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17778 2024-03-25 17:58:13.000000 pygeoif-1.4.0/pygeoif/hypothesis/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 17:58:13.000000 pygeoif-1.4.0/pygeoif/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-25 17:58:13.000000 pygeoif-1.4.0/pygeoif/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:58:17.431458 pygeoif-1.4.0/pygeoif.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14528 2024-03-25 17:58:17.000000 pygeoif-1.4.0/pygeoif.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-25 17:58:17.000000 pygeoif-1.4.0/pygeoif.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 17:58:17.000000 pygeoif-1.4.0/pygeoif.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-25 17:58:17.000000 pygeoif-1.4.0/pygeoif.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 17:58:17.000000 pygeoif-1.4.0/pygeoif.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-03-25 17:58:13.000000 pygeoif-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 17:58:17.435458 pygeoif-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 17:58:17.431458 pygeoif-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-03-25 17:58:13.000000 pygeoif-1.4.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-25 17:58:13.000000 pygeoif-1.4.0/tests/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    19549 2024-03-25 17:58:13.000000 pygeoif-1.4.0/tests/test_factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-03-25 17:58:13.000000 pygeoif-1.4.0/tests/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    12594 2024-03-25 17:58:13.000000 pygeoif-1.4.0/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-03-25 17:58:13.000000 pygeoif-1.4.0/tests/test_geometrycollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-03-25 17:58:13.000000 pygeoif-1.4.0/tests/test_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-03-25 17:58:13.000000 pygeoif-1.4.0/tests/test_linear_ring.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-03-25 17:58:13.000000 pygeoif-1.4.0/tests/test_multiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-03-25 17:58:13.000000 pygeoif-1.4.0/tests/test_multipoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-03-25 17:58:13.000000 pygeoif-1.4.0/tests/test_multipolygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-25 17:58:13.000000 pygeoif-1.4.0/tests/test_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-03-25 17:58:13.000000 pygeoif-1.4.0/tests/test_polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:44:55.078063 pygeoif-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-05-11 12:44:55.078063 pygeoif-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-05-11 12:44:47.000000 pygeoif-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:44:55.070063 pygeoif-1.5.0/pygeoif/
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-11 12:44:47.000000 pygeoif-1.5.0/pygeoif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-11 12:44:47.000000 pygeoif-1.5.0/pygeoif/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-11 12:44:47.000000 pygeoif-1.5.0/pygeoif/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-11 12:44:47.000000 pygeoif-1.5.0/pygeoif/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-05-11 12:44:47.000000 pygeoif-1.5.0/pygeoif/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-11 12:44:47.000000 pygeoif-1.5.0/pygeoif/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32946 2024-05-11 12:44:47.000000 pygeoif-1.5.0/pygeoif/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:44:55.070063 pygeoif-1.5.0/pygeoif/hypothesis/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-11 12:44:47.000000 pygeoif-1.5.0/pygeoif/hypothesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17778 2024-05-11 12:44:47.000000 pygeoif-1.5.0/pygeoif/hypothesis/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:44:47.000000 pygeoif-1.5.0/pygeoif/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-11 12:44:47.000000 pygeoif-1.5.0/pygeoif/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:44:55.074063 pygeoif-1.5.0/pygeoif.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-05-11 12:44:55.000000 pygeoif-1.5.0/pygeoif.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-11 12:44:55.000000 pygeoif-1.5.0/pygeoif.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:44:55.000000 pygeoif-1.5.0/pygeoif.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-11 12:44:55.000000 pygeoif-1.5.0/pygeoif.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-11 12:44:55.000000 pygeoif-1.5.0/pygeoif.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-11 12:44:47.000000 pygeoif-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:44:55.078063 pygeoif-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:44:55.074063 pygeoif-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-11 12:44:47.000000 pygeoif-1.5.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-11 12:44:47.000000 pygeoif-1.5.0/tests/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19569 2024-05-11 12:44:47.000000 pygeoif-1.5.0/tests/test_factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-11 12:44:47.000000 pygeoif-1.5.0/tests/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-05-11 12:44:47.000000 pygeoif-1.5.0/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-05-11 12:44:47.000000 pygeoif-1.5.0/tests/test_geometrycollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-11 12:44:47.000000 pygeoif-1.5.0/tests/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-11 12:44:47.000000 pygeoif-1.5.0/tests/test_linear_ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-11 12:44:47.000000 pygeoif-1.5.0/tests/test_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-11 12:44:47.000000 pygeoif-1.5.0/tests/test_multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-05-11 12:44:47.000000 pygeoif-1.5.0/tests/test_multipolygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-11 12:44:47.000000 pygeoif-1.5.0/tests/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-05-11 12:44:47.000000 pygeoif-1.5.0/tests/test_polygon.py
```

### Comparing `pygeoif-1.4.0/PKG-INFO` & `pygeoif-1.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pygeoif
-Version: 1.4.0
+Version: 1.5.0
 Summary: A basic implementation of the __geo_interface__
 Author-email: Christian Ledermann <christian.ledermann@gmail.com>
 License: LGPL
 Project-URL: Changelog, https://github.com/cleder/pygeoif/blob/develop/docs/HISTORY.rst
 Project-URL: Documentation, https://pygeoif.readthedocs.io/
 Project-URL: Homepage, https://github.com/cleder/pygeoif/
-Keywords: GIS,Spatial,WKT
+Keywords: GIS,Hypothesis,Spatial,WKT
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Hypothesis
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -57,14 +58,15 @@
 Requires-Dist: flake8-super; extra == "linting"
 Requires-Dist: flake8-typing-imports; extra == "linting"
 Requires-Dist: flake8-use-fstring; extra == "linting"
 Requires-Dist: ruff; extra == "linting"
 Requires-Dist: yamllint; extra == "linting"
 Provides-Extra: tests
 Requires-Dist: hypothesis; extra == "tests"
+Requires-Dist: more_itertools; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: typing
 Requires-Dist: hypothesis; extra == "typing"
 Requires-Dist: mypy; extra == "typing"
 
 Introduction
@@ -103,80 +105,83 @@
 geometries in a way that when you are familiar with pygeoif,
 you will feel right at home with shapely or the other way round.
 It provides Hypothesis strategies for all geometries for property based
 testing with Hypothesis_.
 
 It was written to provide clean and python only geometries for fastkml_
 
-.. image:: https://readthedocs.org/projects/pygeoif/badge/?version=latest
+|doc| |test| |cov| |hypothesis| |black| |mypy| |openhub| |factor| |commit| |py| |implement| |latest| |license| |downloads|
+
+.. |doc| image:: https://readthedocs.org/projects/pygeoif/badge/?version=latest
     :target: https://pygeoif.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation
 
-.. image:: https://github.com/cleder/pygeoif/actions/workflows/run-all-tests.yml/badge.svg?branch=main
+.. |test| image:: https://github.com/cleder/pygeoif/actions/workflows/run-all-tests.yml/badge.svg?branch=main
     :target: https://github.com/cleder/pygeoif/actions/workflows/run-all-tests.yml
     :alt: GitHub Actions
 
-.. image:: https://codecov.io/gh/cleder/pygeoif/branch/main/graph/badge.svg?token=2EfiwBXs9X
+.. |cov| image:: https://codecov.io/gh/cleder/pygeoif/branch/main/graph/badge.svg?token=2EfiwBXs9X
     :target: https://codecov.io/gh/cleder/pygeoif
     :alt: Codecov
 
-.. image:: https://img.shields.io/badge/property_based_tests-hypothesis-green
-    :target: https://hypothesis.works
-    :alt: Hypothesis
+.. |hypothesis| image:: https://img.shields.io/badge/hypothesis-tested-brightgreen.svg
+   :alt: Tested with Hypothesis
+   :target: https://hypothesis.readthedocs.io
 
-.. image:: https://img.shields.io/badge/code_style-black-000000.svg
+.. |black| image:: https://img.shields.io/badge/code_style-black-000000.svg
     :target: https://github.com/psf/
     :alt: Black
 
-.. image:: https://img.shields.io/badge/type_checker-mypy-blue
+.. |mypy| image:: https://img.shields.io/badge/type_checker-mypy-blue
     :target: http://mypy-lang.org/
     :alt: Mypy
 
-.. image:: https://www.openhub.net/p/pygeoif/widgets/project_thin_badge.gif
+.. |openhub| image:: https://www.openhub.net/p/pygeoif/widgets/project_thin_badge.gif
     :target: https://www.openhub.net/p/pygeoif/
     :alt: Openhub
 
-.. image:: https://www.codefactor.io/repository/github/cleder/pygeoif/badge/main
+.. |factor| image:: https://www.codefactor.io/repository/github/cleder/pygeoif/badge/main
    :target: https://www.codefactor.io/repository/github/cleder/pygeoif/overview/main
    :alt: CodeFactor
 
-.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
+.. |commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 
-.. image:: https://img.shields.io/pypi/pyversions/pygeoif.svg
+.. |py| image:: https://img.shields.io/pypi/pyversions/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: Supported Python versions
 
-.. image:: https://img.shields.io/pypi/implementation/pygeoif.svg
+.. |implement| image:: https://img.shields.io/pypi/implementation/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/v/pygeoif.svg
+.. |latest| image:: https://img.shields.io/pypi/v/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: Latest Version
 
-.. image:: https://img.shields.io/pypi/l/pygeoif.svg
+.. |license| image:: https://img.shields.io/pypi/l/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: License
 
-.. image:: https://img.shields.io/pypi/dm/pygeoif.svg
+.. |downloads| image:: https://img.shields.io/pypi/dm/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: Downloads
 
 Installation
 ------------
 
 You can install PyGeoIf from pypi using pip::
 
     pip install pygeoif
 
 
 Example
 ========
+.. code-block:: pycon
 
     >>> from pygeoif import geometry
     >>> p = geometry.Point(1,1)
     >>> p.__geo_interface__
     {'type': 'Point', 'bbox': (1, 1, 1, 1), 'coordinates': (1, 1)}
     >>> print(p)
     POINT (1 1)
@@ -224,23 +229,24 @@
 Attributes
 ~~~~~~~~~~~
 x, y, z : float
     Coordinate values
 
 Example
 ~~~~~~~~
+.. code-block: pycon
 
-      >>> from pygeoif import Point
-      >>> p = Point(1.0, -1.0)
-      >>> print(p)
-      POINT (1.0 -1.0)
-      >>> p.y
-      -1.0
-      >>> p.x
-      1.0
+    >>> from pygeoif import Point
+    >>> p = Point(1.0, -1.0)
+    >>> print(p)
+    POINT (1.0 -1.0)
+    >>> p.y
+    -1.0
+    >>> p.x
+    1.0
 
 
 
 LineString
 -----------
 
 A one-dimensional figure comprising one or more line segments
@@ -332,14 +338,15 @@
 Please note:
 ``GEOMETRYCOLLECTION`` isn't supported by the Shapefile or GeoJSON_ format.
 And this sub-class isn't generally supported by ordinary GIS sw (viewers and so on).
 So it's very rarely used in the real GIS professional world.
 
 Example
 ~~~~~~~~
+.. code-block:: pycon
 
     >>> from pygeoif import geometry
     >>> p = geometry.Point(1.0, -1.0)
     >>> p2 = geometry.Point(1.0, -1.0)
     >>> geoms = [p, p2]
     >>> c = geometry.GeometryCollection(geoms)
     >>> [geom for geom in geoms]
@@ -354,14 +361,16 @@
 geometry : object
     A geometry instance
 properties : dict
     A dictionary linking field keys with values associated with with geometry instance
 
 Example
 ~~~~~~~~
+.. code-block:: pycon
+
       >>> from pygeoif import Point, Feature
       >>> p = Point(1.0, -1.0)
       >>> props = {'Name': 'Sample Point', 'Other': 'Other Data'}
       >>> a = Feature(p, props)
       >>> a.properties
       {'Name': 'Sample Point', 'Other': 'Other Data'}
       >>> a.properties['Name']
@@ -374,14 +383,15 @@
 Attributes
 ~~~~~~~~~~~
 features: sequence
     A sequence of feature instances
 
 Example
 ~~~~~~~~
+.. code-block:: pycon
 
     >>> from pygeoif import Point, Feature, FeatureCollection
     >>> p = Point(1.0, -1.0)
     >>> props = {'Name': 'Sample Point', 'Other': 'Other Data'}
     >>> a = Feature(p, props)
     >>> p2 = Point(1.0, -1.0)
     >>> props2 = {'Name': 'Sample Point2', 'Other': 'Other Data2'}
@@ -396,25 +406,29 @@
 
 shape
 --------
 
 Create a pygeoif feature from an object that provides the ``__geo_interface__``
 or any GeoJSON_ compatible dictionary.
 
+.. code-block:: pycon
+
     >>> from shapely.geometry import Point
     >>> from pygeoif import geometry, shape
     >>> shape(Point(0,0))
     Point(0.0, 0.0)
 
 
 from_wkt
 ---------
 
 Create a geometry from its WKT representation
 
+.. code-block:: pycon
+
     >>> from pygeoif import from_wkt
     >>> p = from_wkt('POINT (0 1)')
     >>> print(p)
     POINT (0.0 1.0)
 
 
 signed_area
```

### Comparing `pygeoif-1.4.0/README.rst` & `pygeoif-1.5.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -34,80 +34,83 @@
 geometries in a way that when you are familiar with pygeoif,
 you will feel right at home with shapely or the other way round.
 It provides Hypothesis strategies for all geometries for property based
 testing with Hypothesis_.
 
 It was written to provide clean and python only geometries for fastkml_
 
-.. image:: https://readthedocs.org/projects/pygeoif/badge/?version=latest
+|doc| |test| |cov| |hypothesis| |black| |mypy| |openhub| |factor| |commit| |py| |implement| |latest| |license| |downloads|
+
+.. |doc| image:: https://readthedocs.org/projects/pygeoif/badge/?version=latest
     :target: https://pygeoif.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation
 
-.. image:: https://github.com/cleder/pygeoif/actions/workflows/run-all-tests.yml/badge.svg?branch=main
+.. |test| image:: https://github.com/cleder/pygeoif/actions/workflows/run-all-tests.yml/badge.svg?branch=main
     :target: https://github.com/cleder/pygeoif/actions/workflows/run-all-tests.yml
     :alt: GitHub Actions
 
-.. image:: https://codecov.io/gh/cleder/pygeoif/branch/main/graph/badge.svg?token=2EfiwBXs9X
+.. |cov| image:: https://codecov.io/gh/cleder/pygeoif/branch/main/graph/badge.svg?token=2EfiwBXs9X
     :target: https://codecov.io/gh/cleder/pygeoif
     :alt: Codecov
 
-.. image:: https://img.shields.io/badge/property_based_tests-hypothesis-green
-    :target: https://hypothesis.works
-    :alt: Hypothesis
+.. |hypothesis| image:: https://img.shields.io/badge/hypothesis-tested-brightgreen.svg
+   :alt: Tested with Hypothesis
+   :target: https://hypothesis.readthedocs.io
 
-.. image:: https://img.shields.io/badge/code_style-black-000000.svg
+.. |black| image:: https://img.shields.io/badge/code_style-black-000000.svg
     :target: https://github.com/psf/
     :alt: Black
 
-.. image:: https://img.shields.io/badge/type_checker-mypy-blue
+.. |mypy| image:: https://img.shields.io/badge/type_checker-mypy-blue
     :target: http://mypy-lang.org/
     :alt: Mypy
 
-.. image:: https://www.openhub.net/p/pygeoif/widgets/project_thin_badge.gif
+.. |openhub| image:: https://www.openhub.net/p/pygeoif/widgets/project_thin_badge.gif
     :target: https://www.openhub.net/p/pygeoif/
     :alt: Openhub
 
-.. image:: https://www.codefactor.io/repository/github/cleder/pygeoif/badge/main
+.. |factor| image:: https://www.codefactor.io/repository/github/cleder/pygeoif/badge/main
    :target: https://www.codefactor.io/repository/github/cleder/pygeoif/overview/main
    :alt: CodeFactor
 
-.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
+.. |commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 
-.. image:: https://img.shields.io/pypi/pyversions/pygeoif.svg
+.. |py| image:: https://img.shields.io/pypi/pyversions/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: Supported Python versions
 
-.. image:: https://img.shields.io/pypi/implementation/pygeoif.svg
+.. |implement| image:: https://img.shields.io/pypi/implementation/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/v/pygeoif.svg
+.. |latest| image:: https://img.shields.io/pypi/v/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: Latest Version
 
-.. image:: https://img.shields.io/pypi/l/pygeoif.svg
+.. |license| image:: https://img.shields.io/pypi/l/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: License
 
-.. image:: https://img.shields.io/pypi/dm/pygeoif.svg
+.. |downloads| image:: https://img.shields.io/pypi/dm/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: Downloads
 
 Installation
 ------------
 
 You can install PyGeoIf from pypi using pip::
 
     pip install pygeoif
 
 
 Example
 ========
+.. code-block:: pycon
 
     >>> from pygeoif import geometry
     >>> p = geometry.Point(1,1)
     >>> p.__geo_interface__
     {'type': 'Point', 'bbox': (1, 1, 1, 1), 'coordinates': (1, 1)}
     >>> print(p)
     POINT (1 1)
@@ -155,23 +158,24 @@
 Attributes
 ~~~~~~~~~~~
 x, y, z : float
     Coordinate values
 
 Example
 ~~~~~~~~
+.. code-block: pycon
 
-      >>> from pygeoif import Point
-      >>> p = Point(1.0, -1.0)
-      >>> print(p)
-      POINT (1.0 -1.0)
-      >>> p.y
-      -1.0
-      >>> p.x
-      1.0
+    >>> from pygeoif import Point
+    >>> p = Point(1.0, -1.0)
+    >>> print(p)
+    POINT (1.0 -1.0)
+    >>> p.y
+    -1.0
+    >>> p.x
+    1.0
 
 
 
 LineString
 -----------
 
 A one-dimensional figure comprising one or more line segments
@@ -263,14 +267,15 @@
 Please note:
 ``GEOMETRYCOLLECTION`` isn't supported by the Shapefile or GeoJSON_ format.
 And this sub-class isn't generally supported by ordinary GIS sw (viewers and so on).
 So it's very rarely used in the real GIS professional world.
 
 Example
 ~~~~~~~~
+.. code-block:: pycon
 
     >>> from pygeoif import geometry
     >>> p = geometry.Point(1.0, -1.0)
     >>> p2 = geometry.Point(1.0, -1.0)
     >>> geoms = [p, p2]
     >>> c = geometry.GeometryCollection(geoms)
     >>> [geom for geom in geoms]
@@ -285,14 +290,16 @@
 geometry : object
     A geometry instance
 properties : dict
     A dictionary linking field keys with values associated with with geometry instance
 
 Example
 ~~~~~~~~
+.. code-block:: pycon
+
       >>> from pygeoif import Point, Feature
       >>> p = Point(1.0, -1.0)
       >>> props = {'Name': 'Sample Point', 'Other': 'Other Data'}
       >>> a = Feature(p, props)
       >>> a.properties
       {'Name': 'Sample Point', 'Other': 'Other Data'}
       >>> a.properties['Name']
@@ -305,14 +312,15 @@
 Attributes
 ~~~~~~~~~~~
 features: sequence
     A sequence of feature instances
 
 Example
 ~~~~~~~~
+.. code-block:: pycon
 
     >>> from pygeoif import Point, Feature, FeatureCollection
     >>> p = Point(1.0, -1.0)
     >>> props = {'Name': 'Sample Point', 'Other': 'Other Data'}
     >>> a = Feature(p, props)
     >>> p2 = Point(1.0, -1.0)
     >>> props2 = {'Name': 'Sample Point2', 'Other': 'Other Data2'}
@@ -327,25 +335,29 @@
 
 shape
 --------
 
 Create a pygeoif feature from an object that provides the ``__geo_interface__``
 or any GeoJSON_ compatible dictionary.
 
+.. code-block:: pycon
+
     >>> from shapely.geometry import Point
     >>> from pygeoif import geometry, shape
     >>> shape(Point(0,0))
     Point(0.0, 0.0)
 
 
 from_wkt
 ---------
 
 Create a geometry from its WKT representation
 
+.. code-block:: pycon
+
     >>> from pygeoif import from_wkt
     >>> p = from_wkt('POINT (0 1)')
     >>> print(p)
     POINT (0.0 1.0)
 
 
 signed_area
```

### Comparing `pygeoif-1.4.0/pygeoif/__init__.py` & `pygeoif-1.5.0/pygeoif/__init__.py`

 * *Files identical despite different names*

### Comparing `pygeoif-1.4.0/pygeoif/exceptions.py` & `pygeoif-1.5.0/pygeoif/exceptions.py`

 * *Files identical despite different names*

### Comparing `pygeoif-1.4.0/pygeoif/factories.py` & `pygeoif-1.5.0/pygeoif/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,23 +146,20 @@
     geometry = context if isinstance(context, dict) else mapping(context)
     if not geometry:
         msg = (  # type: ignore [unreachable]
             "Object does not implement __geo_interface__"
         )
         raise TypeError(msg)
 
-    constructor = type_map.get(geometry["type"])
-    if constructor:
+    if constructor := type_map.get(geometry["type"]):
         return constructor._from_dict(  # type: ignore [attr-defined, no-any-return]
             geometry,
         )
     if geometry["type"] == "GeometryCollection":
-        geometries = [
-            shape(fi) for fi in geometry["geometries"]  # type: ignore [typeddict-item]
-        ]
+        geometries = [shape(fi) for fi in geometry["geometries"]]
         return GeometryCollection(geometries)
     msg = f"[{geometry['type']} is not implemented"
     raise NotImplementedError(msg)
 
 
 def num(number: str) -> float:
     """
```

### Comparing `pygeoif-1.4.0/pygeoif/feature.py` & `pygeoif-1.5.0/pygeoif/feature.py`

 * *Files identical despite different names*

### Comparing `pygeoif-1.4.0/pygeoif/functions.py` & `pygeoif-1.5.0/pygeoif/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,43 +37,47 @@
 def signed_area(coords: LineType) -> float:
     """
     Return the signed area enclosed by a ring.
 
     Linear time algorithm: http://www.cgafaq.info/wiki/Polygon_Area.
     A value >= 0 indicates a counter-clockwise oriented ring.
     """
+    if len(coords) < 3:  # noqa: PLR2004
+        return 0.0
     xs, ys = map(list, zip(*(coord[:2] for coord in coords)))
     xs.append(xs[1])  # pragma: no mutate
     ys.append(ys[1])  # pragma: no mutate
     return cast(
         float,
         sum(xs[i] * (ys[i + 1] - ys[i - 1]) for i in range(1, len(coords))) / 2.0,
     )
 
 
 def centroid(coords: LineType) -> Tuple[Point2D, float]:
     """Calculate the coordinates of the centroid and the area of a LineString."""
     ans: List[float] = [0, 0]
-
     n = len(coords)
     signed_area = 0.0
 
     # For all vertices
     for i, coord in enumerate(coords):
         next_coord = coords[(i + 1) % n]
         # Calculate area using shoelace formula
         area = (coord[0] * next_coord[1]) - (next_coord[0] * coord[1])
         signed_area += area
 
         # Calculate coordinates of centroid of polygon
         ans[0] += (coord[0] + next_coord[0]) * area
         ans[1] += (coord[1] + next_coord[1]) * area
 
-    ans[0] = (ans[0]) / (3 * signed_area)
-    ans[1] = (ans[1]) / (3 * signed_area)
+    if signed_area == 0 or math.isnan(signed_area):
+        return ((math.nan, math.nan), signed_area)
+
+    ans[0] = ans[0] / (3 * signed_area)
+    ans[1] = ans[1] / (3 * signed_area)
 
     return cast(Point2D, tuple(ans)), signed_area / 2.0
 
 
 def dedupe(coords: LineType) -> LineType:
     """Remove duplicate Points from a LineString."""
     return cast(LineType, tuple(coord for coord, _count in groupby(coords)))
@@ -163,21 +167,21 @@
     try:
         if first["type"] != second["type"]:
             return False
         if first["type"] == "GeometryCollection":
             return all(
                 compare_geo_interface(first=g1, second=g2)  # type: ignore [arg-type]
                 for g1, g2 in zip_longest(
-                    first["geometries"],  # type: ignore [typeddict-item]
+                    first["geometries"],
                     second["geometries"],  # type: ignore [typeddict-item]
                     fillvalue={"type": None, "coordinates": ()},
                 )
             )
         return compare_coordinates(
-            coords=first["coordinates"],  # type: ignore [typeddict-item]
+            coords=first["coordinates"],
             other=second["coordinates"],  # type: ignore [typeddict-item]
         )
     except KeyError:
         return False
 
 
 def move_coordinate(
@@ -216,14 +220,16 @@
     >>> move_coordinates(((0, 0), (-1, 1)), (-1, 1))
     ((-1, 1), (-2, 2))
     >>> move_coordinates(((0, 0, 0), (-1, 1, 0)), (-1, 1))
     ((-1, 1), (-2, 2))
     >>> move_coordinates(((0, 0), (-1, 1)), (-1, 1, 0))
     ((-1, 1, 0), (-2, 2, 0))
     """
+    if not coordinates:
+        return coordinates
     if isinstance(coordinates[0], (int, float)):
         return move_coordinate(cast(PointType, coordinates), move_by)
     return cast(
         CoordinatesType,
         tuple(move_coordinates(cast(CoordinatesType, c), move_by) for c in coordinates),
     )
 
@@ -233,22 +239,21 @@
     move_by: PointType,
 ) -> Union[GeoInterface, GeoCollectionInterface]:
     """Move the coordinates of the geo interface by the given vector."""
     if interface["type"] == "GeometryCollection":
         return {
             "type": "GeometryCollection",
             "geometries": tuple(
-                move_geo_interface(g, move_by)
-                for g in interface["geometries"]  # type: ignore [typeddict-item]
+                move_geo_interface(g, move_by) for g in interface["geometries"]
             ),
         }
     return {
         "type": interface["type"],
         "coordinates": move_coordinates(
-            interface["coordinates"],  # type: ignore [typeddict-item, arg-type]
+            interface["coordinates"],  # type: ignore [arg-type]
             move_by,
         ),
     }
 
 
 __all__ = [
     "centroid",
```

### Comparing `pygeoif-1.4.0/pygeoif/geometry.py` & `pygeoif-1.5.0/pygeoif/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from pygeoif.functions import compare_geo_interface
 from pygeoif.functions import convex_hull
 from pygeoif.functions import dedupe
 from pygeoif.functions import signed_area
 from pygeoif.types import Bounds
 from pygeoif.types import GeoCollectionInterface
 from pygeoif.types import GeoInterface
+from pygeoif.types import GeomType
 from pygeoif.types import GeoType
 from pygeoif.types import LineType
 from pygeoif.types import Point2D
 from pygeoif.types import PointType
 from pygeoif.types import PolygonType
 
 
@@ -162,15 +163,15 @@
 
     @property
     def __geo_interface__(self) -> GeoInterface:
         if self.is_empty:
             msg = "Empty Geometry"
             raise AttributeError(msg)
         return {
-            "type": self.geom_type,
+            "type": cast(GeomType, self.geom_type),
             "bbox": cast(Bounds, self.bounds),
             "coordinates": (),
         }
 
     @property
     def _wkt_coords(self) -> str:
         msg = "Must be implemented by subclass"
@@ -244,39 +245,35 @@
 
         Parameters
         ----------
         2 or 3 coordinate parameters: x, y, [z] : float
             Easting, northing, and elevation.
 
         """
+        geoms = (x, y, z) if z is not None else (x, y)
         object.__setattr__(
             self,
             "_geoms",
-            cast(
-                PointType,
-                tuple(
-                    coordinate
-                    for coordinate in (x, y, z)
-                    if coordinate is not None and not math.isnan(coordinate)
-                ),
-            ),
+            geoms,
         )
 
     def __repr__(self) -> str:
         """Return the representation."""
+        if self.is_empty:
+            return f"{self.geom_type}()"
         return f"{self.geom_type}{self._geoms}"
 
     @property
     def is_empty(self) -> bool:
         """
         Return if this geometry is empty.
 
-        A Point is considered empty when it has fewer than 2 coordinates.
+        A Point is considered empty when it has no valid coordinates.
         """
-        return len(self._geoms) < 2  # noqa: PLR2004
+        return any(coord is None or math.isnan(coord) for coord in self._geoms)
 
     @property
     def x(self) -> float:
         """Return x coordinate."""
         return self._geoms[0]
 
     @property
@@ -289,17 +286,17 @@
         """Return z coordinate."""
         if self.has_z:
             return self._geoms[2]  # type: ignore [misc]
         msg = f"The {self!r} geometry does not have z values"
         raise DimensionError(msg)
 
     @property
-    def coords(self) -> Tuple[PointType]:
+    def coords(self) -> Union[Tuple[PointType], Tuple[()]]:
         """Return the geometry coordinates."""
-        return (self._geoms,)
+        return () if self.is_empty else (self._geoms,)
 
     @property
     def has_z(self) -> bool:
         """Return True if the geometry's coordinate sequence(s) have z values."""
         return len(self._geoms) == 3  # noqa: PLR2004
 
     @property
@@ -372,15 +369,18 @@
     def geoms(self) -> Tuple[Point, ...]:
         """Return the underlying geometries."""
         return self._geoms
 
     @property
     def coords(self) -> LineType:
         """Return the geometry coordinates."""
-        return cast(LineType, tuple(point.coords[0] for point in self.geoms))
+        return cast(
+            LineType,
+            tuple(point.coords[0] for point in self.geoms if point.coords),
+        )
 
     @property
     def is_empty(self) -> bool:
         """
         Return if this geometry is empty.
 
         A Linestring is considered empty when it has no points.
@@ -407,15 +407,17 @@
     def from_coordinates(cls, coordinates: LineType) -> "LineString":
         """Construct a linestring from coordinates."""
         return cls(coordinates)
 
     @classmethod
     def from_points(cls, *args: Point) -> "LineString":
         """Create a linestring from points."""
-        return cls(cast(LineType, tuple(point.coords[0] for point in args)))
+        return cls(
+            cast(LineType, tuple(point.coords[0] for point in args if point.coords)),
+        )
 
     @classmethod
     def _from_dict(cls, geo_interface: GeoInterface) -> "LineString":
         cls._check_dict(geo_interface)
         return cls(cast(LineType, geo_interface["coordinates"]))
 
     @staticmethod
@@ -476,17 +478,17 @@
 
     @property
     def centroid(self) -> Optional[Point]:
         """Return the centroid of the ring."""
         if self.has_z:
             msg = "Centeroid is only implemented for 2D coordinates"
             raise DimensionError(msg)
-        try:
-            cent, area = centroid(self.coords)
-        except ZeroDivisionError:
+
+        cent, area = centroid(self.coords)
+        if any(math.isnan(coord) for coord in cent):
             return None
         return (
             Point(x=cent[0], y=cent[1])
             if math.isclose(a=area, b=signed_area(self.coords))
             else None
         )
 
@@ -620,14 +622,16 @@
             shell=shell.coords,
             holes=tuple(lr.coords for lr in args),
         )
 
     @classmethod
     def _from_dict(cls, geo_interface: GeoInterface) -> "Polygon":
         cls._check_dict(geo_interface)
+        if not geo_interface["coordinates"]:
+            return cls(shell=(), holes=())
         return cls(
             shell=cast(LineType, geo_interface["coordinates"][0]),
             holes=cast(Tuple[LineType], geo_interface["coordinates"][1:]),
         )
 
     def _get_bounds(self) -> Bounds:
         return self.exterior._get_bounds()  # noqa: SLF001
@@ -729,36 +733,41 @@
 
     def __len__(self) -> int:
         """Return the number of points in this MultiPoint."""
         return len(self._geoms)
 
     def __repr__(self) -> str:
         """Return the representation."""
-        return f"{self.geom_type}({tuple(geom.coords[0] for geom in self._geoms)})"
+        return (
+            f"{self.geom_type}"
+            f"({tuple(geom.coords[0] for geom in self._geoms if geom.coords)})"
+        )
 
     @property
     def geoms(self) -> Iterator[Point]:
         """Iterate over the points."""
         yield from (cast(Point, p) for p in super().geoms)
 
     @property
     def _wkt_coords(self) -> str:
         return ", ".join(point._wkt_coords for point in self.geoms)  # noqa: SLF001
 
     @property
     def __geo_interface__(self) -> GeoInterface:
         """Return the geo interface."""
         geo_interface = super().__geo_interface__
-        geo_interface["coordinates"] = tuple(geom.coords[0] for geom in self.geoms)
+        geo_interface["coordinates"] = tuple(
+            geom.coords[0] for geom in self.geoms if geom.coords
+        )
         return geo_interface
 
     @classmethod
     def from_points(cls, *args: Point, unique: bool = False) -> "MultiPoint":
         """Create a MultiPoint from Points."""
-        return cls([point.coords[0] for point in args], unique=unique)
+        return cls([point.coords[0] for point in args if point.coords], unique=unique)
 
     @classmethod
     def _from_dict(cls, geo_interface: GeoInterface) -> "MultiPoint":
         cls._check_dict(geo_interface)
         return cls(cast(Sequence[PointType], geo_interface["coordinates"]))
 
     def _prepare_hull(self) -> Iterable[Point2D]:
```

### Comparing `pygeoif-1.4.0/pygeoif/hypothesis/strategies.py` & `pygeoif-1.5.0/pygeoif/hypothesis/strategies.py`

 * *Files identical despite different names*

### Comparing `pygeoif-1.4.0/pygeoif/types.py` & `pygeoif-1.5.0/pygeoif/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,29 @@
 CoordinatesType = Union[
     PointType,
     LineType,
     Sequence[LineType],
 ]
 MultiCoordinatesType = Sequence[CoordinatesType]
 
+GeomType = Literal[
+    "Point",
+    "LineString",
+    "LinearRing",
+    "Polygon",
+    "MultiPoint",
+    "MultiLineString",
+    "MultiPolygon",
+]
+
 
 class GeoInterface(TypedDict):
     """Required keys for the GeoInterface."""
 
-    type: str
+    type: GeomType
     coordinates: Union[CoordinatesType, MultiCoordinatesType]
     bbox: NotRequired[Bounds]
 
 
 class GeoCollectionInterface(TypedDict):
     """Geometry Collection Interface."""
```

### Comparing `pygeoif-1.4.0/pygeoif.egg-info/PKG-INFO` & `pygeoif-1.5.0/pygeoif.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pygeoif
-Version: 1.4.0
+Version: 1.5.0
 Summary: A basic implementation of the __geo_interface__
 Author-email: Christian Ledermann <christian.ledermann@gmail.com>
 License: LGPL
 Project-URL: Changelog, https://github.com/cleder/pygeoif/blob/develop/docs/HISTORY.rst
 Project-URL: Documentation, https://pygeoif.readthedocs.io/
 Project-URL: Homepage, https://github.com/cleder/pygeoif/
-Keywords: GIS,Spatial,WKT
+Keywords: GIS,Hypothesis,Spatial,WKT
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Hypothesis
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -57,14 +58,15 @@
 Requires-Dist: flake8-super; extra == "linting"
 Requires-Dist: flake8-typing-imports; extra == "linting"
 Requires-Dist: flake8-use-fstring; extra == "linting"
 Requires-Dist: ruff; extra == "linting"
 Requires-Dist: yamllint; extra == "linting"
 Provides-Extra: tests
 Requires-Dist: hypothesis; extra == "tests"
+Requires-Dist: more_itertools; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: typing
 Requires-Dist: hypothesis; extra == "typing"
 Requires-Dist: mypy; extra == "typing"
 
 Introduction
@@ -103,80 +105,83 @@
 geometries in a way that when you are familiar with pygeoif,
 you will feel right at home with shapely or the other way round.
 It provides Hypothesis strategies for all geometries for property based
 testing with Hypothesis_.
 
 It was written to provide clean and python only geometries for fastkml_
 
-.. image:: https://readthedocs.org/projects/pygeoif/badge/?version=latest
+|doc| |test| |cov| |hypothesis| |black| |mypy| |openhub| |factor| |commit| |py| |implement| |latest| |license| |downloads|
+
+.. |doc| image:: https://readthedocs.org/projects/pygeoif/badge/?version=latest
     :target: https://pygeoif.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation
 
-.. image:: https://github.com/cleder/pygeoif/actions/workflows/run-all-tests.yml/badge.svg?branch=main
+.. |test| image:: https://github.com/cleder/pygeoif/actions/workflows/run-all-tests.yml/badge.svg?branch=main
     :target: https://github.com/cleder/pygeoif/actions/workflows/run-all-tests.yml
     :alt: GitHub Actions
 
-.. image:: https://codecov.io/gh/cleder/pygeoif/branch/main/graph/badge.svg?token=2EfiwBXs9X
+.. |cov| image:: https://codecov.io/gh/cleder/pygeoif/branch/main/graph/badge.svg?token=2EfiwBXs9X
     :target: https://codecov.io/gh/cleder/pygeoif
     :alt: Codecov
 
-.. image:: https://img.shields.io/badge/property_based_tests-hypothesis-green
-    :target: https://hypothesis.works
-    :alt: Hypothesis
+.. |hypothesis| image:: https://img.shields.io/badge/hypothesis-tested-brightgreen.svg
+   :alt: Tested with Hypothesis
+   :target: https://hypothesis.readthedocs.io
 
-.. image:: https://img.shields.io/badge/code_style-black-000000.svg
+.. |black| image:: https://img.shields.io/badge/code_style-black-000000.svg
     :target: https://github.com/psf/
     :alt: Black
 
-.. image:: https://img.shields.io/badge/type_checker-mypy-blue
+.. |mypy| image:: https://img.shields.io/badge/type_checker-mypy-blue
     :target: http://mypy-lang.org/
     :alt: Mypy
 
-.. image:: https://www.openhub.net/p/pygeoif/widgets/project_thin_badge.gif
+.. |openhub| image:: https://www.openhub.net/p/pygeoif/widgets/project_thin_badge.gif
     :target: https://www.openhub.net/p/pygeoif/
     :alt: Openhub
 
-.. image:: https://www.codefactor.io/repository/github/cleder/pygeoif/badge/main
+.. |factor| image:: https://www.codefactor.io/repository/github/cleder/pygeoif/badge/main
    :target: https://www.codefactor.io/repository/github/cleder/pygeoif/overview/main
    :alt: CodeFactor
 
-.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
+.. |commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 
-.. image:: https://img.shields.io/pypi/pyversions/pygeoif.svg
+.. |py| image:: https://img.shields.io/pypi/pyversions/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: Supported Python versions
 
-.. image:: https://img.shields.io/pypi/implementation/pygeoif.svg
+.. |implement| image:: https://img.shields.io/pypi/implementation/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: Supported Python implementations
 
-.. image:: https://img.shields.io/pypi/v/pygeoif.svg
+.. |latest| image:: https://img.shields.io/pypi/v/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: Latest Version
 
-.. image:: https://img.shields.io/pypi/l/pygeoif.svg
+.. |license| image:: https://img.shields.io/pypi/l/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: License
 
-.. image:: https://img.shields.io/pypi/dm/pygeoif.svg
+.. |downloads| image:: https://img.shields.io/pypi/dm/pygeoif.svg
     :target: https://pypi.python.org/pypi/pygeoif/
     :alt: Downloads
 
 Installation
 ------------
 
 You can install PyGeoIf from pypi using pip::
 
     pip install pygeoif
 
 
 Example
 ========
+.. code-block:: pycon
 
     >>> from pygeoif import geometry
     >>> p = geometry.Point(1,1)
     >>> p.__geo_interface__
     {'type': 'Point', 'bbox': (1, 1, 1, 1), 'coordinates': (1, 1)}
     >>> print(p)
     POINT (1 1)
@@ -224,23 +229,24 @@
 Attributes
 ~~~~~~~~~~~
 x, y, z : float
     Coordinate values
 
 Example
 ~~~~~~~~
+.. code-block: pycon
 
-      >>> from pygeoif import Point
-      >>> p = Point(1.0, -1.0)
-      >>> print(p)
-      POINT (1.0 -1.0)
-      >>> p.y
-      -1.0
-      >>> p.x
-      1.0
+    >>> from pygeoif import Point
+    >>> p = Point(1.0, -1.0)
+    >>> print(p)
+    POINT (1.0 -1.0)
+    >>> p.y
+    -1.0
+    >>> p.x
+    1.0
 
 
 
 LineString
 -----------
 
 A one-dimensional figure comprising one or more line segments
@@ -332,14 +338,15 @@
 Please note:
 ``GEOMETRYCOLLECTION`` isn't supported by the Shapefile or GeoJSON_ format.
 And this sub-class isn't generally supported by ordinary GIS sw (viewers and so on).
 So it's very rarely used in the real GIS professional world.
 
 Example
 ~~~~~~~~
+.. code-block:: pycon
 
     >>> from pygeoif import geometry
     >>> p = geometry.Point(1.0, -1.0)
     >>> p2 = geometry.Point(1.0, -1.0)
     >>> geoms = [p, p2]
     >>> c = geometry.GeometryCollection(geoms)
     >>> [geom for geom in geoms]
@@ -354,14 +361,16 @@
 geometry : object
     A geometry instance
 properties : dict
     A dictionary linking field keys with values associated with with geometry instance
 
 Example
 ~~~~~~~~
+.. code-block:: pycon
+
       >>> from pygeoif import Point, Feature
       >>> p = Point(1.0, -1.0)
       >>> props = {'Name': 'Sample Point', 'Other': 'Other Data'}
       >>> a = Feature(p, props)
       >>> a.properties
       {'Name': 'Sample Point', 'Other': 'Other Data'}
       >>> a.properties['Name']
@@ -374,14 +383,15 @@
 Attributes
 ~~~~~~~~~~~
 features: sequence
     A sequence of feature instances
 
 Example
 ~~~~~~~~
+.. code-block:: pycon
 
     >>> from pygeoif import Point, Feature, FeatureCollection
     >>> p = Point(1.0, -1.0)
     >>> props = {'Name': 'Sample Point', 'Other': 'Other Data'}
     >>> a = Feature(p, props)
     >>> p2 = Point(1.0, -1.0)
     >>> props2 = {'Name': 'Sample Point2', 'Other': 'Other Data2'}
@@ -396,25 +406,29 @@
 
 shape
 --------
 
 Create a pygeoif feature from an object that provides the ``__geo_interface__``
 or any GeoJSON_ compatible dictionary.
 
+.. code-block:: pycon
+
     >>> from shapely.geometry import Point
     >>> from pygeoif import geometry, shape
     >>> shape(Point(0,0))
     Point(0.0, 0.0)
 
 
 from_wkt
 ---------
 
 Create a geometry from its WKT representation
 
+.. code-block:: pycon
+
     >>> from pygeoif import from_wkt
     >>> p = from_wkt('POINT (0 1)')
     >>> print(p)
     POINT (0.0 1.0)
 
 
 signed_area
```

### Comparing `pygeoif-1.4.0/pygeoif.egg-info/SOURCES.txt` & `pygeoif-1.5.0/pygeoif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeoif-1.4.0/pygeoif.egg-info/requires.txt` & `pygeoif-1.5.0/pygeoif.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -34,13 +34,14 @@
 flake8-typing-imports
 flake8-use-fstring
 ruff
 yamllint
 
 [tests]
 hypothesis
+more_itertools
 pytest
 pytest-cov
 
 [typing]
 hypothesis
 mypy
```

### Comparing `pygeoif-1.4.0/pyproject.toml` & `pygeoif-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 [project]
 authors = [
     { email = "christian.ledermann@gmail.com", name = "Christian Ledermann" },
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
+    "Framework :: Hypothesis",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -31,14 +32,15 @@
 ]
 description = "A basic implementation of the __geo_interface__"
 dynamic = [
     "version",
 ]
 keywords = [
     "GIS",
+    "Hypothesis",
     "Spatial",
     "WKT",
 ]
 name = "pygeoif"
 requires-python = ">=3.8"
 
 [project.license]
@@ -79,14 +81,15 @@
     "flake8-typing-imports",
     "flake8-use-fstring",
     "ruff",
     "yamllint",
 ]
 tests = [
     "hypothesis",
+    "more_itertools",
     "pytest",
     "pytest-cov",
 ]
 typing = [
     "hypothesis",
     "mypy",
 ]
```

### Comparing `pygeoif-1.4.0/tests/test_base.py` & `pygeoif-1.5.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pygeoif-1.4.0/tests/test_bounds.py` & `pygeoif-1.5.0/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `pygeoif-1.4.0/tests/test_factories.py` & `pygeoif-1.5.0/tests/test_factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 def test_force_2d_polygon() -> None:
     # 2d to 2d (no actual change)
     external = [(0, 0), (0, 2), (2, 2), (2, 0), (0, 0)]
     internal = [(0.5, 0.5), (0.5, 1.5), (1.5, 1.5), (1.5, 0.5), (0.5, 0.5)]
     p = geometry.Polygon(external, [internal])
     p2d = factories.force_2d(p)
-    assert p2d.coords[0] == (((0, 0), (0, 2), (2, 2), (2, 0), (0, 0)))
+    assert p2d.coords[0] == ((0, 0), (0, 2), (2, 2), (2, 0), (0, 0))
     assert p2d.coords[1] == (
         ((0.5, 0.5), (0.5, 1.5), (1.5, 1.5), (1.5, 0.5), (0.5, 0.5)),
     )
     assert not p2d.has_z
 
     # 3d to 2d
     external = [(0, 0, 1), (0, 2, 1), (2, 2, 1), (2, 0, 1), (0, 0, 1)]
@@ -103,15 +103,15 @@
         (1.5, 1.5, 1),
         (1.5, 0.5, 1),
         (0.5, 0.5, 1),
     ]
 
     p = geometry.Polygon(external, [internal])
     p2d = factories.force_2d(p)
-    assert p2d.coords[0] == (((0, 0), (0, 2), (2, 2), (2, 0), (0, 0)))
+    assert p2d.coords[0] == ((0, 0), (0, 2), (2, 2), (2, 0), (0, 0))
     assert p2d.coords[1] == (
         ((0.5, 0.5), (0.5, 1.5), (1.5, 1.5), (1.5, 0.5), (0.5, 0.5)),
     )
     assert not p2d.has_z
 
 
 def test_force_2d_multipolygon() -> None:
@@ -257,16 +257,18 @@
 class TestWKT:
     # valid and supported WKTs
     wkt_ok = [
         "POINT(6 10)",
         "POINT M (1 1 80)",
         "LINESTRING(3 4,10 50,20 25)",
         "LINESTRING (30 10, 10 30, 40 40)",
-        "MULTIPOLYGON (((10 10, 10 20, 20 20, 20 15, 10 10)),"
-        "((60 60, 70 70, 80 60, 60 60 )))",
+        (
+            "MULTIPOLYGON (((10 10, 10 20, 20 20, 20 15, 10 10)),"
+            "((60 60, 70 70, 80 60, 60 60 )))"
+        ),
         """MULTIPOLYGON (((40 40, 20 45, 45 30, 40 40)),
               ((20 35, 45 20, 30 5, 10 10, 10 30, 20 35),
               (30 20, 20 25, 20 15, 30 20)))""",
         """MULTIPOLYGON (((30 20, 10 40, 45 40, 30 20)),
               ((15 5, 40 10, 10 20, 5 10, 15 5)))""",
         "MULTIPOLYGON (((0 0,10 0,10 10,0 10,0 0)),((5 5,7 5,7 7,5 7, 5 5)))",
         "GEOMETRYCOLLECTION (POINT(10 10), POINT(30 30), LINESTRING(15 15, 20 20))",
@@ -381,16 +383,16 @@
 
     def test_multilinestring(self) -> None:
         p = factories.from_wkt(
             "MULTILINESTRING ((3 4,10 50,20 25),(-5 -8,-10 -8,-15 -4))",
         )
 
         assert isinstance(p, geometry.MultiLineString)
-        assert next(iter(p.geoms)).coords == (((3, 4), (10, 50), (20, 25)))
-        assert list(p.geoms)[1].coords == (((-5, -8), (-10, -8), (-15, -4)))
+        assert next(iter(p.geoms)).coords == ((3, 4), (10, 50), (20, 25))
+        assert list(p.geoms)[1].coords == ((-5, -8), (-10, -8), (-15, -4))
         assert (
             p.wkt == "MULTILINESTRING ((3 4, 10 50, "
             "20 25),(-5 -8, "
             "-10 -8, -15 -4))"
         )
 
     def test_multilinestring_1(self) -> None:
```

### Comparing `pygeoif-1.4.0/tests/test_feature.py` & `pygeoif-1.5.0/tests/test_feature.py`

 * *Files identical despite different names*

### Comparing `pygeoif-1.4.0/tests/test_functions.py` & `pygeoif-1.5.0/tests/test_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,15 @@
 def test_signed_area2() -> None:
     a0 = [(0, 0), (0, 1), (1, 1), (0, 0)]
     assert centroid(a0)[1] == signed_area(a0)
 
 
 def test_centroid_line() -> None:
     a0 = [(0, 0), (1, 1), (0, 0)]
-    with pytest.raises(ZeroDivisionError):
-        assert centroid(a0)
+    assert centroid(a0) == ((math.nan, math.nan), 0)
 
 
 def test_signed_area_0_3d() -> None:
     assert signed_area(((0.0, 0.0, 0.0), (0.0, 0.0, 0.0))) == 0.0
 
 
 def test_signed_area_0_2d() -> None:
```

### Comparing `pygeoif-1.4.0/tests/test_geometrycollection.py` & `pygeoif-1.5.0/tests/test_geometrycollection.py`

 * *Files identical despite different names*

### Comparing `pygeoif-1.4.0/tests/test_line.py` & `pygeoif-1.5.0/tests/test_line.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Test LineString."""
 
+import math
 from unittest import mock
 
 import pytest
 
 from pygeoif import exceptions
 from pygeoif import geometry
 
@@ -16,14 +17,20 @@
 
 def test_coords_get_3d() -> None:
     line = geometry.LineString([(0, 0, 0), (1, 1, 1)])
 
     assert line.coords == ((0.0, 0.0, 0), (1.0, 1.0, 1))
 
 
+def test_coords_get_nan() -> None:
+    line = geometry.LineString([(0, math.nan, 0), (1, 1, math.nan), (2, 2, 2)])
+
+    assert line.coords == ((2, 2, 2),)
+
+
 def test_empty_points_omitted() -> None:
     line = geometry.LineString([(0, 0, 0), (None, None, None), (2, 2, 2)])
 
     assert line.coords == ((0, 0, 0), (2, 2, 2))
 
 
 def test_set_geoms_raises() -> None:
@@ -209,7 +216,25 @@
     assert repr(line) == "LineString(())"
 
 
 def test_empty_bounds() -> None:
     line = geometry.LineString([])
 
     assert line.bounds == ()
+
+
+def test_bounds_1_pt() -> None:
+    line = geometry.LineString([(0, 0)])
+
+    assert line.bounds == (0, 0, 0, 0)
+
+
+def test_empty_coords() -> None:
+    line = geometry.LineString([])
+
+    assert line.coords == ()
+
+
+def test_empty_coords_nan() -> None:
+    line = geometry.LineString(((math.nan, math.nan),))
+
+    assert line.coords == ()
```

### Comparing `pygeoif-1.4.0/tests/test_linear_ring.py` & `pygeoif-1.5.0/tests/test_linear_ring.py`

 * *Files identical despite different names*

### Comparing `pygeoif-1.4.0/tests/test_multiline.py` & `pygeoif-1.5.0/tests/test_multiline.py`

 * *Files identical despite different names*

### Comparing `pygeoif-1.4.0/tests/test_multipoint.py` & `pygeoif-1.5.0/tests/test_multipoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Test MultiPoint."""
 
+import math
+
 import pytest
 
 from pygeoif import geometry
 
 
 def test_geoms() -> None:
     multipoint = geometry.MultiPoint([(0, 0), (1, 1), (1, 2), (2, 2)])
@@ -152,16 +154,22 @@
 def test_empty() -> None:
     multipoint = geometry.MultiPoint([(1, None)])
 
     assert multipoint.is_empty
 
 
 def test_repr_empty() -> None:
-    multipoint = geometry.MultiPoint([(None, None)])
+    multipoint = geometry.MultiPoint([(math.nan, math.nan)])
 
-    assert repr(multipoint) == "MultiPoint(((),))"
+    assert repr(multipoint) == "MultiPoint(())"
 
 
 def test_empty_bounds() -> None:
     multipoint = geometry.MultiPoint([(None, None)])
 
     assert multipoint.bounds == ()
+
+
+def test_empty_geoms() -> None:
+    multipoint = geometry.MultiPoint([(math.nan, math.nan)])
+
+    assert not list(multipoint.geoms)
```

### Comparing `pygeoif-1.4.0/tests/test_multipolygon.py` & `pygeoif-1.5.0/tests/test_multipolygon.py`

 * *Files identical despite different names*

### Comparing `pygeoif-1.4.0/tests/test_point.py` & `pygeoif-1.5.0/tests/test_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,20 @@
 
 def test_repr_empty() -> None:
     point = geometry.Point(None, None)
 
     assert repr(point) == "Point()"
 
 
+def test_coords_empty() -> None:
+    point = geometry.Point(None, None)
+
+    assert point.coords == ()
+
+
 def test_repr2d() -> None:
     point = geometry.Point(1, 0)
 
     assert repr(point) == "Point(1, 0)"
     assert not point.has_z
```

### Comparing `pygeoif-1.4.0/tests/test_polygon.py` & `pygeoif-1.5.0/tests/test_polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,26 @@
     assert polygon.__geo_interface__, {
         "type": "Polygon",
         "bbox": (0.0, 0.0, 1.0, 1.0),
         "coordinates": (((0.0, 0.0), (1.0, 1.0), (1.0, 0.0), (0.0, 0.0)),),
     }
 
 
+def test_from_dict_empty_coordinates() -> None:
+    polygon = geometry.Polygon._from_dict(
+        {
+            "type": "Polygon",
+            "bbox": (0.0, 0.0, 1.0, 1.0),
+            "coordinates": (),
+        },
+    )
+
+    assert polygon.is_empty
+
+
 def test_from_dict_with_holes() -> None:
     polygon = geometry.Polygon._from_dict(
         {
             "type": "Polygon",
             "bbox": (0.0, 0.0, 2.0, 2.0),
             "coordinates": (
                 ((0.0, 0.0), (0.0, 2.0), (2.0, 2.0), (2.0, 0.0), (0.0, 0.0)),
```

