# Comparing `tmp/peeweext-1.2.6-py3-none-any.whl.zip` & `tmp/peeweext-1.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 10172 bytes, number of entries: 12
--rw-rw-r--  2.0 unx       22 b- defN 21-Dec-29 10:20 peeweext/__init__.py
--rw-rw-r--  2.0 unx     1663 b- defN 21-Dec-29 10:20 peeweext/fields.py
--rw-rw-r--  2.0 unx     1732 b- defN 21-Dec-29 10:20 peeweext/flask.py
--rw-rw-r--  2.0 unx     3739 b- defN 21-Dec-29 10:20 peeweext/mixins.py
--rw-rw-r--  2.0 unx     5089 b- defN 21-Dec-29 10:20 peeweext/model.py
--rw-rw-r--  2.0 unx     2455 b- defN 21-Dec-29 10:20 peeweext/sea.py
--rw-rw-r--  2.0 unx     5859 b- defN 21-Dec-29 10:20 peeweext/validation.py
--rw-rw-r--  2.0 unx     1064 b- defN 21-Dec-29 10:20 peeweext-1.2.6.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1698 b- defN 21-Dec-29 10:20 peeweext-1.2.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 21-Dec-29 10:20 peeweext-1.2.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 21-Dec-29 10:20 peeweext-1.2.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      914 b- defN 21-Dec-29 10:20 peeweext-1.2.6.dist-info/RECORD
-12 files, 24336 bytes uncompressed, 8656 bytes compressed:  64.4%
+Zip file size: 10636 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       22 b- defN 24-May-11 07:30 peeweext/__init__.py
+-rw-r--r--  2.0 unx     1663 b- defN 24-May-11 07:30 peeweext/fields.py
+-rw-r--r--  2.0 unx     1795 b- defN 24-May-11 07:30 peeweext/flask.py
+-rw-r--r--  2.0 unx     3739 b- defN 24-May-11 07:30 peeweext/mixins.py
+-rw-r--r--  2.0 unx     5089 b- defN 24-May-11 07:30 peeweext/model.py
+-rw-r--r--  2.0 unx      551 b- defN 24-May-11 07:30 peeweext/otel.py
+-rw-r--r--  2.0 unx     2517 b- defN 24-May-11 07:30 peeweext/sea.py
+-rw-r--r--  2.0 unx     5859 b- defN 24-May-11 07:30 peeweext/validation.py
+-rw-r--r--  2.0 unx     1064 b- defN 24-May-11 07:30 peeweext-1.2.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1733 b- defN 24-May-11 07:30 peeweext-1.2.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-11 07:30 peeweext-1.2.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-May-11 07:30 peeweext-1.2.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      986 b- defN 24-May-11 07:30 peeweext-1.2.7.dist-info/RECORD
+13 files, 25119 bytes uncompressed, 9012 bytes compressed:  64.1%
```

## zipnote {}

```diff
@@ -9,29 +9,32 @@
 
 Filename: peeweext/mixins.py
 Comment: 
 
 Filename: peeweext/model.py
 Comment: 
 
+Filename: peeweext/otel.py
+Comment: 
+
 Filename: peeweext/sea.py
 Comment: 
 
 Filename: peeweext/validation.py
 Comment: 
 
-Filename: peeweext-1.2.6.dist-info/LICENSE
+Filename: peeweext-1.2.7.dist-info/LICENSE
 Comment: 
 
-Filename: peeweext-1.2.6.dist-info/METADATA
+Filename: peeweext-1.2.7.dist-info/METADATA
 Comment: 
 
-Filename: peeweext-1.2.6.dist-info/WHEEL
+Filename: peeweext-1.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: peeweext-1.2.6.dist-info/top_level.txt
+Filename: peeweext-1.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: peeweext-1.2.6.dist-info/RECORD
+Filename: peeweext-1.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## peeweext/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '1.2.6'
+__version__ = '1.2.7'
```

## peeweext/flask.py

```diff
@@ -1,10 +1,11 @@
 from werkzeug.local import LocalProxy
 from werkzeug.utils import import_string, cached_property
 from playhouse import db_url
+from .otel import otel_instrument
 
 
 class UninitializedException(Exception):
     pass
 
 
 class Peeweext:
@@ -16,14 +17,15 @@
 
     def init_app(self, app):
         config = app.config.get_namespace(self.ns)
         self.model_class = import_string(
             config.get('model', 'peeweext.model.Model'))
         conn_params = config.get('conn_params', {})
 
+        otel_instrument(app)
         # initialize private connection pool
         self._database = db_url.connect(config['db_url'], **conn_params)
 
         self._register_handlers(app)
 
     def _get_db(self):
         if not self._database:
```

## peeweext/sea.py

```diff
@@ -1,27 +1,28 @@
 from sea.utils import import_string, cached_property
 from sea.local import Proxy
 from sea.middleware import BaseMiddleware
 from sea.pb2 import default_pb2
 from playhouse import db_url
 from peewee import DoesNotExist, DataError
 import grpc
-
+from .otel import otel_instrument
 from .validation import ValidationError
 
 
 class Peeweext:
     def __init__(self, ns='PW_'):
         self.ns = ns
 
     def init_app(self, app):
         config = app.config.get_namespace(self.ns)
         self.model_class = import_string(
             config.get('model', 'peeweext.model.Model'))
         conn_params = config.get('conn_params', {})
+        otel_instrument(app)
         self.database = db_url.connect(config['db_url'], **conn_params)
         self._try_setup_celery()
 
     def _get_db(self):
         return self.database
 
     @cached_property
```

## Comparing `peeweext-1.2.6.dist-info/LICENSE` & `peeweext-1.2.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `peeweext-1.2.6.dist-info/METADATA` & `peeweext-1.2.7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: peeweext
-Version: 1.2.6
+Version: 1.2.7
 Summary: peewee extension
 Home-page: https://github.com/shanbay/peeweext
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 License: MIT
 Keywords: peewee,orm
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,20 +18,19 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 License-File: LICENSE
 Requires-Dist: peewee
-Requires-Dist: pendulum (>=2.0.0)
+Requires-Dist: pendulum >=2.0.0
 Requires-Dist: blinker
+Requires-Dist: opentelemetry.instrumentation.mysqlclient
 
 # [Home Page](https://shanbay.github.io/peeweext/)
 
 [![](https://img.shields.io/travis/shanbay/peeweext.svg?style=flat-square)](https://travis-ci.org/shanbay/peeweext)
 [![Maintainability](https://api.codeclimate.com/v1/badges/774db211d37720bb2599/maintainability)](https://codeclimate.com/github/shanbay/peeweext/maintainability)
 [![Coverage Status](https://coveralls.io/repos/github/shanbay/peeweext/badge.svg?branch=master)](https://coveralls.io/github/shanbay/peeweext?branch=master)
 [![](https://img.shields.io/pypi/v/peeweext.svg)](https://github.com/shanbay/peeweext)
 [![](https://img.shields.io/pypi/pyversions/peeweext.svg)](https://github.com/shanbay/peeweext)
 [![](https://img.shields.io/:license-mit-blue.svg?style=flat-square)](https://shanbay.mit-license.org)
-
-
```

