# Comparing `tmp/mongo_objects-1.1.2.tar.gz` & `tmp/mongo_objects-1.2.0.tar.gz`

## Comparing `mongo_objects-1.1.2.tar` & `mongo_objects-1.2.0.tar`

### file list

```diff
@@ -1,32 +1,88 @@
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/.readthedocs.yaml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/requirements.txt
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/MongoDictProxy.rst
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/MongoListProxy.rst
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/MongoSingleProxy.rst
--rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/MongoUserDict.rst
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/conf.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/customization.rst
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/index.rst
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/quickstart.rst
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/docs/source/sample.rst
--rw-r--r--   0        0        0    33427 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/src/mongo_objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/conftest.py
--rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_MongoDictProxy.py
--rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_MongoListProxy.py
--rw-r--r--   0        0        0    27139 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_MongoSingleProxy.py
--rw-r--r--   0        0        0    41394 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_MongoUserDict.py
--rw-r--r--   0        0        0    13920 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_PolymorphicMongoDictProxy.py
--rw-r--r--   0        0        0    16023 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_PolymorphicMongoListProxy.py
--rw-r--r--   0        0        0    15580 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_PolymorphicMongoSingleProxy.py
--rw-r--r--   0        0        0    13775 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_PolymorphicMongoUserDict.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tests/test_proxy_combo.py
--rwxr-xr-x   0        0        0     1326 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tools/buildProject
--rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tools/runTests
--rwxr-xr-x   0        0        0     2399 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tools/setupPythonVenv
--rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/tools/updateRequirements
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/README.rst
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 mongo_objects-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/.buildinfo
+-rw-r--r--   0        0        0    32726 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/MongoDictProxy.html
+-rw-r--r--   0        0        0    37165 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/MongoListProxy.html
+-rw-r--r--   0        0        0    34866 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/MongoSingleProxy.html
+-rw-r--r--   0        0        0    86142 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/MongoUserDict.html
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/customization.html
+-rw-r--r--   0        0        0    21639 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/genindex.html
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/index.html
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/objects.inv
+-rw-r--r--   0        0        0    32630 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/proxy_overview.html
+-rw-r--r--   0        0        0    15225 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/quickstart.html
+-rw-r--r--   0        0        0    49234 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/sample.html
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/search.html
+-rw-r--r--   0        0        0    30606 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/searchindex.js
+-rw-r--r--   0        0        0    40155 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/add-feature.png
+-rw-r--r--   0        0        0    40656 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/add-gift.png
+-rw-r--r--   0        0        0    41876 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/add-ticket-type-1.png
+-rw-r--r--   0        0        0    42916 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/add-ticket-type-2.png
+-rw-r--r--   0        0        0    43187 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/add-ticket-type-3.png
+-rw-r--r--   0        0        0    39029 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/add-venue.png
+-rw-r--r--   0        0        0    37878 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/create-event.png
+-rw-r--r--   0        0        0    41100 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/purchase-ticket.png
+-rw-r--r--   0        0        0    69499 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_images/vip-ticket-detail-1.png
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/MongoDictProxy.rst.txt
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/MongoListProxy.rst.txt
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/MongoSingleProxy.rst.txt
+-rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/MongoUserDict.rst.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/customization.rst.txt
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/index.rst.txt
+-rw-r--r--   0        0        0    11126 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/proxy_overview.rst.txt
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/quickstart.rst.txt
+-rw-r--r--   0        0        0    19506 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_sources/sample.rst.txt
+-rw-r--r--   0        0        0    40155 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/add-feature.png
+-rw-r--r--   0        0        0    40656 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/add-gift.png
+-rw-r--r--   0        0        0    41876 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/add-ticket-type-1.png
+-rw-r--r--   0        0        0    42916 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/add-ticket-type-2.png
+-rw-r--r--   0        0        0    43187 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/add-ticket-type-3.png
+-rw-r--r--   0        0        0    39029 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/add-venue.png
+-rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/alabaster.css
+-rw-r--r--   0        0        0    15096 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/basic.css
+-rw-r--r--   0        0        0    37878 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/create-event.png
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/doctools.js
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/plus.png
+-rw-r--r--   0        0        0    41100 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/purchase-ticket.png
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/pygments.css
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/searchtools.js
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0    69499 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/docs/_static/vip-ticket-detail-1.png
+-rw-r--r--   0        0        0    29582 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/mongo_objects_sample.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/requirements.txt
+-rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/run-sample-app
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/static/base.css
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/admin-event-detail.jinja
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/admin-event-list.jinja
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/admin-ticket-detail.jinja
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/base.jinja
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/create-update-event.jinja
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/create-update-feature.jinja
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/create-update-gift.jinja
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/create-update-ticket-type.jinja
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/create-update-venue.jinja
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/customer-event-detail.jinja
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/customer-event-list.jinja
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/customer-purchase-ticket.jinja
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/form-tools.jinja
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/sample/templates/index.jinja
+-rw-r--r--   0        0        0    62761 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/src/mongo_objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0    34946 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_MongoDictProxy.py
+-rw-r--r--   0        0        0    38456 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_MongoListProxy.py
+-rw-r--r--   0        0        0    34289 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_MongoSingleProxy.py
+-rw-r--r--   0        0        0    40908 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_MongoUserDict.py
+-rw-r--r--   0        0        0    22162 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_PolymorphicMongoDictProxy.py
+-rw-r--r--   0        0        0    23836 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_PolymorphicMongoListProxy.py
+-rw-r--r--   0        0        0    20130 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_PolymorphicMongoSingleProxy.py
+-rw-r--r--   0        0        0    24806 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_PolymorphicMongoUserDict.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/tests/test_proxy_combo.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/README.rst
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5257 2020-02-02 00:00:00.000000 mongo_objects-1.2.0/PKG-INFO
```

### Comparing `mongo_objects-1.1.2/docs/source/index.rst` & `mongo_objects-1.2.0/docs/_sources/index.rst.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 mongo_objects wraps pymongo with new classes to simplify access to MongoDB
 documents and subdocuments.
 
 Documents are returned as user-defined UserDict subclasses, seamlessly linking user code
 with MongoDB data.
 
 Subdocuments are accessed through user-defined, dictionary-like subclasses that proxy
-access back to the original parent document.
+data from the original parent document.
 
 
 Installation
 ------------
 
 Install from PyPI. We recommend installing into the virtual environment
 for your Python project.::
@@ -54,27 +54,20 @@
 
 Manage subdocuments as lightweight dictionary-like proxies back to
 the parent document object.
 
 .. toctree::
    :maxdepth: 2
 
+   proxy_overview
    MongoDictProxy
    MongoListProxy
    MongoSingleProxy
 
 
-Additional Information
-----------------------
-.. toctree::
-   :maxdepth: 2
-
-   customization
-
-
 Credits
 -------
 
 Development sponsored by `Headwaters Entrepreneurs Pte Ltd <https://headwaters.com.sg>`_.
 
 Originally developed by `Frontier Tech Team LLC <https://frontiertechteam.com>`_
 for the `Wasted Minutes <https://wasted-minutes.com>`_ ™️ language study tool.
```

### Comparing `mongo_objects-1.1.2/docs/source/quickstart.rst` & `mongo_objects-1.2.0/docs/_sources/quickstart.rst.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Quickstart
 ========================
 
 MongoDB Documents
 -----------------
 
-Subclass :doc:`MongoUserDict` and provide the class with two pieces of information,
+Get started by subclassing :doc:`MongoUserDict` and providing the class with
+two pieces of information,
 the pymongo object for your MongoDB database and the name of the collection.
 
-To illustrate we'll use snippets of the event management application
-from the sample code.::
+To illustrate we'll use snippets from the event management application
+in the sample code. ::
 
     import mongo_objects
 
     class Event( mongo_objects.MongoUserDict ):
-        db = ...          # provide your MongoDB database object here
+        db = ...          # provide your pymongo database object here
         collection_name = 'events'
 
 
 You can now manage your data as follows::
 
     # Initialize a new, empty MongoDB document as an Event object,
     # a subclass of UserDict with full dictionary features.
@@ -121,10 +122,10 @@
     # a classmethod on the parent document
     ticket = Event.load_proxy_by_id(
         '66277dcce66752e012bf62e6g73',
         Ticket
         )
 
 
-You can read more in the :doc:`MongoDictProxy` documentation. Lists
+You can read more in the :doc:`proxy_overview` and :doc:`MongoDictProxy` documentation. Lists
 can also be used as subdocument containers with :doc:`MongoListProxy`.
 Single dictionary proxies are managed with :doc:`MongoSingleProxy`.
```

### Comparing `mongo_objects-1.1.2/tests/test_MongoDictProxy.py` & `mongo_objects-1.2.0/tests/test_MongoDictProxy.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pymongo.collection import Collection
 import pytest
 import secrets
 
 
 @pytest.fixture( scope='class' )
 def getMMUDClasses( mongo_db ):
-    '''Return a MongoUserDict configured for a per-class unique collection'''
+    """Return a MongoUserDict configured for a per-class unique collection"""
 
     class MyMongoUserDict( mongo_objects.MongoUserDict ):
         collection_name = secrets.token_hex(6)
         database = mongo_db
 
     class MyMongoDictProxyA( mongo_objects.MongoDictProxy ):
         container_name = 'proxyA'
@@ -22,15 +22,15 @@
     class MyMongoDictProxyA1( mongo_objects.MongoDictProxy ):
         container_name = 'proxyA1'
 
     class MyMongoDictProxyB( mongo_objects.MongoDictProxy ):
         container_name = 'proxyB'
 
     return {
-        'base' : MyMongoUserDict,
+        'parent_doc' : MyMongoUserDict,
         'A' : MyMongoDictProxyA,
         'A1' : MyMongoDictProxyA1,
         'B' : MyMongoDictProxyB
     }
 
 
 
@@ -38,15 +38,15 @@
 def getPopulatedMMUDClasses( getMMUDClasses ):
 
     classes = getMMUDClasses
     itemMax = 3     # make three of everything
 
     # make parent objects
     for i in range( itemMax ):
-        parent = classes['base']( {
+        parent = classes['parent_doc']( {
             'name' : f"Record {i}",
             'amount' : i * 10,
         } )
 
         # make first-level proxies
         for j in range( itemMax ):
             proxyA = classes['A'].create( parent, {
@@ -71,15 +71,15 @@
     return classes
 
 
 @pytest.fixture( scope='class' )
 def getSampleParent( getPopulatedMMUDClasses ):
     classes = getPopulatedMMUDClasses
     # find a random entry of the base class
-    return classes['base'].find_one()
+    return classes['parent_doc'].find_one()
 
 
 @pytest.fixture( scope='class' )
 def getSampleProxyA( getPopulatedMMUDClasses, getSampleParent ):
     classes = getPopulatedMMUDClasses
     # return the first proxyA in the list
     return classes['A'].get_proxies( getSampleParent )[0]
@@ -97,15 +97,15 @@
 class TestCreate:
     def test_create( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         count = len( proxyA.get_subdoc_container().keys() )
 
         # create a new entry in a level one proxy
         newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'} )
 
         # verify a new entry was created
         assert len( proxyA.get_subdoc_container().keys() ) == count+1
@@ -117,15 +117,15 @@
 
     def test_create_no_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         count = len( proxyA.get_subdoc_container().keys() )
 
         # create a new entry in a level one proxy without saving the parent
         newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'}, autosave=False )
 
         # verify a new entry was created
         assert len( proxyA.get_subdoc_container().keys() ) == count+1
@@ -138,15 +138,15 @@
     def test_create_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
         parent = proxyA1.ultimate_parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         countA = len( proxyA.get_subdoc_container().keys() )
         countA1 = len( proxyA1.get_subdoc_container().keys() )
 
         # create a new entry in a level two proxy
         newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'} )
 
         # verify a new entry was created at the second (proxyA1) level
@@ -161,15 +161,15 @@
     def test_create_A1_no_save( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
         parent = proxyA1.ultimate_parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         countA = len( proxyA.get_subdoc_container().keys() )
         countA1 = len( proxyA1.get_subdoc_container().keys() )
 
         # create a new entry in a level two proxy without saving the parent
         newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'}, autosave=None )
 
         # verify a new entry was created at the second (proxyA1) level
@@ -186,15 +186,15 @@
 class TestDelete_ProxyA:
     def test_delete( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         count = len( proxyA.get_subdoc_container().keys() )
         key = proxyA.key
 
         # delete the level one proxy
         proxyA.delete()
 
         # verify the entry was deleted
@@ -209,15 +209,15 @@
 class TestDelete_ProxyA_No_Save:
     def test_delete_no_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         count = len( proxyA.get_subdoc_container().keys() )
         key = proxyA.key
 
         # delete the level one proxy without saving the parent
         proxyA.delete( autosave=False )
 
         # verify the entry was deleted
@@ -235,15 +235,15 @@
     def test_delete_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
         parent = proxyA1.ultimate_parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         countA = len( proxyA.get_subdoc_container().keys() )
         countA1 = len( proxyA1.get_subdoc_container().keys() )
         key = proxyA1.key
 
         # delete the level one proxy
         proxyA1.delete()
 
@@ -263,15 +263,15 @@
     def test_delete_A1_no_save( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
         parent = proxyA1.ultimate_parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         countA = len( proxyA.get_subdoc_container().keys() )
         countA1 = len( proxyA1.get_subdoc_container().keys() )
         key = proxyA1.key
 
         # delete the level one proxy
         proxyA1.delete( autosave=False )
 
@@ -301,15 +301,15 @@
         # verify that the key no longer exists
         assert 'nameA' not in proxy
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : proxy.parent['_id'] } )
 
         # verify that the key no longer exists in the database as well
         assert 'nameA' not in doc['proxyA'][ proxy.key ]
 
 
 
 class TestDelItem_A1:
@@ -326,15 +326,15 @@
         # verify that the key no longer exists
         assert 'nameA1' not in proxy
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
 
         # verify that the key no longer exists in the database as well
         assert 'nameA1' not in doc['proxyA'][ proxy.parent.key ]['proxyA1'][ proxy.key ]
 
 
 
 class TestSetDefault:
@@ -412,15 +412,15 @@
         assert 'newKey' in proxy
         assert proxy['newKey'] == 'this is a new value'
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : proxy.parent['_id'] } )
 
         # verify that the new key exists in the database as well
         assert 'newKey' in doc['proxyA'][ proxy.key ]
         assert doc['proxyA'][ proxy.key ]['newKey'] == 'this is a new value'
 
 
 
@@ -439,15 +439,15 @@
         assert 'newKey' in proxy
         assert proxy['newKey'] == 'this is a new value'
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
 
         # verify that the new key exists in the database as well
         assert 'newKey' in doc['proxyA'][ proxy.parent.key ]['proxyA1'][ proxy.key ]
         assert doc['proxyA'][ proxy.parent.key ]['proxyA1'][ proxy.key ]['newKey'] == 'this is a new value'
 
 
 
@@ -503,37 +503,65 @@
         assert proxy['newKey2'] == 2
         assert len( proxy.keys() ) == count + 2
 
 
 
 
 class TestBasics:
+    def test_copy( self, getSampleProxyA ):
+        proxyA = getSampleProxyA
+        copied = proxyA.copy()
+
+        # Verify data is the same
+        assert copied == proxyA.data()
+        # Verify that data location is not the same
+        assert id( copied ) != id( proxyA.data() )
+
+
     def test_create_key( self, getPopulatedMMUDClasses, getSampleProxyA ):
-        '''Test key creation for single and two-level proxies'''
+        """Test key creation for single and two-level proxies"""
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
         updated = parent['_updated']
 
         # create a proxyA key
-        keyA = classes['A'].create_key( parent )
+        keyA = classes['A'].create_key( parent, {} )
         assert isinstance( keyA, str )
         assert keyA == f"{parent['_last_unique_integer']:x}"
 
         # create a proxyA1 key
-        keyA1 = classes['A1'].create_key( proxyA )
+        keyA1 = classes['A1'].create_key( proxyA, {} )
         assert isinstance( keyA1, str )
         assert keyA1 == f"{parent['_last_unique_integer']:x}"
         assert keyA != keyA1
 
         # verify that create_key doesn't save the parent object
-        doc = classes['base'].collection().find_one( { '_id' : parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : parent['_id'] } )
         assert doc['_updated'] == updated
 
 
+    def test_create_key_override( self, getPopulatedMMUDClasses, getSampleParent ):
+        """Test custom key creation"""
+        parent = getSampleParent
+        subdoc = { 'custom' : 'XYZ', 'more-data' : 3.1415 }
+
+        class LocalProxyClass( getPopulatedMMUDClasses['A'] ):
+            @classmethod
+            def create_key( cls, parent, subdoc ):
+                return subdoc['custom']
+
+        # confirm key is extracted as expected
+        assert LocalProxyClass.create_key( parent, subdoc ) == 'XYZ'
+
+        # confirm a new object uses the expected key
+        proxy = LocalProxyClass.create( parent, subdoc )
+        assert proxy.key == 'XYZ'
+
+
     def test_contains( self, getSampleProxyA ):
         proxy = getSampleProxyA
         assert 'nameA' in proxy
         assert 'will-not-match' not in proxy
 
 
     def test_contains_A1( self, getSampleProxyA1 ):
@@ -550,14 +578,27 @@
 
     def test_data_A1( self, getSampleProxyA1 ):
         proxy = getSampleProxyA1
         # verify that the data references the same dictionary
         assert id( proxy.data() ) == id( proxy.ultimate_parent['proxyA'][proxy.parent.key]['proxyA1'][proxy.key] )
 
 
+    def test_exists( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxy = getSampleProxyA
+        # verify the class can find this key within this parent
+        assert classes['A'].exists( proxy.parent, proxy.key )
+
+
+    def test_exists_non_existent( self, getPopulatedMMUDClasses, getSampleParent ):
+        classes = getPopulatedMMUDClasses
+        # verify a non-existent key can't be located
+        assert not classes['A'].exists( getSampleParent, 'non-existent-key' )
+
+
     def test_get( self, getSampleProxyA ):
         proxy = getSampleProxyA
         assert proxy.get('nameA') is not None
         assert proxy.get('will-not-match') is None
 
 
     def test_get( self, getSampleProxyA1 ):
@@ -577,15 +618,15 @@
         proxy = getSampleProxyA1
         assert proxy['nameA1'] is not None
         with pytest.raises( Exception ):
             assert proxy['will-not-match']
 
 
     def test_get_proxies( self, getPopulatedMMUDClasses, getSampleParent ):
-        '''Test accessing both first-level and second-level proxy lists'''
+        """Test accessing both first-level and second-level proxy lists"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # get all keys in the proxy A container
         keysA = list( parent[ classes['A'].container_name ].keys() )
 
         # get all first-level proxies
@@ -620,24 +661,24 @@
 
         # verify type matches
         for proxy in result:
             assert isinstance( proxy, classes['A1'])
 
 
     def test_get_proxies_empty( self, getPopulatedMMUDClasses ):
-        '''Test get proxies from an empty object'''
+        """Test get proxies from an empty object"""
         classes = getPopulatedMMUDClasses
 
         # collect proxies from an empty object
         result = classes['A'].get_proxies( {} )
         assert len(result) == 0
 
 
     def test_get_proxy( self, getPopulatedMMUDClasses, getSampleParent ):
-        '''Test accessing both first-level and second-level proxies'''
+        """Test accessing both first-level and second-level proxies"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # locate the first key in the proxy A container
         keyA = list( parent[ classes['A'].container_name ].keys() )[0]
 
         # create a first-level proxy object
@@ -687,27 +728,27 @@
         proxyA1 = getSampleProxyA1
 
         # verify data location
         assert id( proxyA1.get_subdoc_container() ) == id( proxyA1.ultimate_parent[ classes['A'].container_name ][ proxyA1.parent.key ][ classes['A1'].container_name ] )
 
 
     def test_id( self, getSampleProxyA ):
-        '''Test ID for single level proxy'''
+        """Test ID for single level proxy"""
         proxy = getSampleProxyA
         assert proxy.id() == f"{proxy.parent.id()}{proxy.parent.subdoc_key_sep}{proxy.key}"
 
 
     def test_id_A1( self, getSampleProxyA1 ):
-        '''Test ID for two-level proxy'''
+        """Test ID for two-level proxy"""
         proxy = getSampleProxyA1
         assert proxy.id() == f"{proxy.ultimate_parent.id()}{proxy.ultimate_parent.subdoc_key_sep}{proxy.parent.key}{proxy.ultimate_parent.subdoc_key_sep}{proxy.key}"
 
 
     def test_init( self, getPopulatedMMUDClasses, getSampleParent ):
-        '''Test initialization of single and two-level proxies'''
+        """Test initialization of single and two-level proxies"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # pick the first proxyA key
         keyA = list( parent['proxyA'].keys() )[0]
 
         # create the proxy
@@ -723,27 +764,27 @@
         proxyA1 = classes['A1']( proxyA, keyA1 )
 
         # verify that the data references the same dictionary
         assert id( proxyA1.data() ) == id( parent['proxyA'][keyA]['proxyA1'][keyA1] )
 
 
     def test_init_bad_key( self, getPopulatedMMUDClasses, getSampleParent ):
-        '''Test initialization of single and two-level proxies'''
+        """Test initialization of single and two-level proxies"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # creating a first-level proxy with a bad key raises an exception
         with pytest.raises( Exception ):
             classes['A']( parent, 'not-a-valid-key')
 
         # create a proxy for the first proxyA key
         keyA = list( parent['proxyA'].keys() )[0]
         proxyA = classes['A']( parent, keyA )
 
-        # creating a first-level proxy with a bad key raises an exception
+        # creating a second-level proxy with a bad key raises an exception
         with pytest.raises( Exception ):
             classes['A1']( proxyA, 'not-a-valid-key')
 
 
 
     def test_items( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
@@ -783,34 +824,177 @@
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
 
         assert proxyA1.keys() == proxyA1.ultimate_parent[ classes['A'].container_name ][ proxyA.key ][ classes['A1'].container_name ][ proxyA1.key ].keys()
 
 
+    def test_load_proxy_by_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['A'] )
+
+        # verify the objects are the same
+        assert result.data() == proxyA.data()
+
+        # verify the parent is not readonly
+        assert result.ultimate_parent.readonly is False
+
+
+
+    def test_load_proxy_by_id_readonly( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['A'], readonly=True )
+
+        # verify the objects are the same
+        assert result.data() == proxyA.data()
+
+        # verify the parent is readonly
+        assert result.ultimate_parent.readonly is True
+
+
+    def test_load_proxy_by_id_invalid_proxy_id( self, getPopulatedMMUDClasses ):
+        """Test load_proxy_by_id() with a totally invalid ID"""
+        classes = getPopulatedMMUDClasses
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( 'this-is-not-a-proxy-id', classes['A'] )
+
+        # verify the return value is None
+        assert result == None
+
+
+    def test_load_proxy_by_id_invalid_object_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        """Test load_proxy_by_id() with a non-existent ObjectId"""
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # tamper with the ID to replace its ObjectId
+        proxyId = str( ObjectId() ) + proxyA.id()[24:]
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyId, classes['A'] )
+
+        # verify the return value is None
+        assert result == None
+
+
+    def test_load_proxy_by_id_invalid_local_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        """Test load_proxy_by_id() with a non-existent proxy ID"""
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # Can't load proxyB with proxyA's ID
+        with pytest.raises( mongo_objects.MongoObjectsNonexistentKey ):
+            result = classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['B'] )
+
+
+    def test_load_proxy_by_id_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'], classes['A1'] )
+
+        # verify the objects are the same
+        assert result.data() == proxyA1.data()
+
+        # verify the parent is not readonly
+        assert result.ultimate_parent.readonly is False
+
+
+    def test_load_proxy_by_id_readonly_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'], classes['A1'], readonly=True )
+
+        # verify the objects are the same
+        assert result.data() == proxyA1.data()
+
+        # verify the parent is readonly
+        assert result.ultimate_parent.readonly is True
+
+
+    def test_load_proxy_by_local_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # reload the proxy by its local ID
+        result = proxyA.ultimate_parent.load_proxy_by_local_id( proxyA.proxy_id(), classes['A'] )
+
+        # verify the objects are the same
+        assert result.data() == proxyA.data()
+
+
+    def test_load_proxy_by_local_id_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # reload the proxy by its ID
+        result = proxyA1.ultimate_parent.load_proxy_by_local_id( proxyA1.proxy_id(), classes['A'], classes['A1'] )
+
+        # verify the objects are the same
+        assert result.data() == proxyA1.data()
+
+
+    def test_proxy_id( self, getSampleProxyA ):
+        """Test single level proxy ID"""
+        proxy = getSampleProxyA
+        assert proxy.proxy_id() == f"{proxy.key}"
+
+
+    def test_proxy_id_with_parent_id( self, getSampleProxyA ):
+        """Test single level proxy ID with parent ID
+        This should be the same as id()"""
+        proxy = getSampleProxyA
+        assert proxy.proxy_id( include_parent_doc_id=True ) == f"{proxy.parent.id()}{proxy.parent.subdoc_key_sep}{proxy.key}"
+        assert proxy.proxy_id( include_parent_doc_id=True ) == proxy.id()
+
+
+    def test_id_A1( self, getSampleProxyA1 ):
+        """Test second level proxy ID"""
+        proxy = getSampleProxyA1
+        assert proxy.proxy_id() == f"{proxy.parent.key}{proxy.ultimate_parent.subdoc_key_sep}{proxy.key}"
+
+
+    def test_id_A1_id_with_parent_id( self, getSampleProxyA1 ):
+        """Test second level proxy ID with parent ID.
+        This should be the same as id()"""
+        proxy = getSampleProxyA1
+        assert proxy.proxy_id( include_parent_doc_id=True ) == f"{proxy.ultimate_parent.id()}{proxy.ultimate_parent.subdoc_key_sep}{proxy.parent.key}{proxy.ultimate_parent.subdoc_key_sep}{proxy.key}"
+        assert proxy.proxy_id( include_parent_doc_id=True ) == proxy.id()
+
+
     def test_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # preserve original state
-        original = dict( proxyA.parent )
+        original = proxyA.parent.copy()
 
         # save the object
         proxyA.save()
 
         # verify the parent document was saved
         assert proxyA.parent['_updated'] > original['_updated']
 
 
     def test_save_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # preserve original state
-        original = dict( proxyA1.ultimate_parent )
+        original = proxyA1.ultimate_parent.copy()
 
         # save the object
         proxyA1.save()
 
         # verify the parent document was saved
         assert proxyA1.ultimate_parent['_updated'] > original['_updated']
```

### Comparing `mongo_objects-1.1.2/tests/test_MongoListProxy.py` & `mongo_objects-1.2.0/tests/test_MongoListProxy.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pymongo.collection import Collection
 import pytest
 import secrets
 
 
 @pytest.fixture( scope='class' )
 def getMMUDClasses( mongo_db ):
-    '''Return a MongoUserDict configured for a per-class unique collection'''
+    """Return a MongoUserDict configured for a per-class unique collection"""
 
     class MyMongoUserDict( mongo_objects.MongoUserDict ):
         collection_name = secrets.token_hex(6)
         database = mongo_db
 
     class MyMongoListProxyA( mongo_objects.MongoListProxy ):
         container_name = 'proxyA'
@@ -22,15 +22,15 @@
     class MyMongoListProxyA1( mongo_objects.MongoListProxy ):
         container_name = 'proxyA1'
 
     class MyMongoListProxyB( mongo_objects.MongoListProxy ):
         container_name = 'proxyB'
 
     return {
-        'base' : MyMongoUserDict,
+        'parent_doc' : MyMongoUserDict,
         'A' : MyMongoListProxyA,
         'A1' : MyMongoListProxyA1,
         'B' : MyMongoListProxyB
     }
 
 
 
@@ -38,15 +38,15 @@
 def getPopulatedMMUDClasses( getMMUDClasses ):
 
     classes = getMMUDClasses
     itemMax = 3     # make three of everything
 
     # make parent objects
     for i in range( itemMax ):
-        parent = classes['base']( {
+        parent = classes['parent_doc']( {
             'name' : f"Record {i}",
             'amount' : i * 10,
         } )
 
         # make first-level proxies
         for j in range( itemMax ):
             proxyA = classes['A'].create( parent, {
@@ -71,15 +71,15 @@
     return classes
 
 
 @pytest.fixture( scope='class' )
 def getSampleParent( getPopulatedMMUDClasses ):
     classes = getPopulatedMMUDClasses
     # find a random entry of the base class
-    return classes['base'].find_one()
+    return classes['parent_doc'].find_one()
 
 
 @pytest.fixture( scope='class' )
 def getSampleProxyA( getPopulatedMMUDClasses, getSampleParent ):
     classes = getPopulatedMMUDClasses
     # return the first proxyA in the list
     return classes['A'].get_proxies( getSampleParent )[0]
@@ -101,15 +101,15 @@
 class TestCreate:
     def test_create( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         count = len( proxyA.get_subdoc_container() )
 
         # create a new entry in a level one proxy
         newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'} )
 
         # verify a key was added to the proxy
         assert proxyA.subdoc_key_name in newProxy
@@ -127,15 +127,15 @@
 
     def test_create_no_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         count = len( proxyA.get_subdoc_container() )
 
         # create a new entry in a level one proxy without saving the parent
         newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'}, autosave=False )
 
         # verify a key was added to the proxy
         assert proxyA.subdoc_key_name in newProxy
@@ -154,15 +154,15 @@
     def test_create_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
         parent = proxyA1.ultimate_parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         countA = len( proxyA.get_subdoc_container() )
         countA1 = len( proxyA1.get_subdoc_container() )
 
         # create a new entry in a level two proxy
         newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'} )
 
         # verify a key was added to the proxy
@@ -183,15 +183,15 @@
     def test_create_A1_no_save( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
         parent = proxyA1.ultimate_parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         countA = len( proxyA.get_subdoc_container() )
         countA1 = len( proxyA1.get_subdoc_container() )
 
         # create a new entry in a level two proxy without saving the parent
         newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'}, autosave=None )
 
         # verify a key was added to the proxy
@@ -214,15 +214,15 @@
 class TestDelete_ProxyA:
     def test_delete( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         count = len( proxyA.get_subdoc_container() )
         key = proxyA.key
 
         # delete the level one proxy
         proxyA.delete()
 
         # verify the entry was deleted
@@ -237,15 +237,15 @@
 class TestDelete_ProxyA_No_Save:
     def test_delete_no_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         count = len( proxyA.get_subdoc_container() )
         key = proxyA.key
 
         # delete the level one proxy without saving the parent
         proxyA.delete( autosave=False )
 
         # verify the entry was deleted
@@ -263,15 +263,15 @@
     def test_delete_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
         parent = proxyA1.ultimate_parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         countA = len( proxyA.get_subdoc_container() )
         countA1 = len( proxyA1.get_subdoc_container() )
         key = proxyA1.key
 
         # delete the level one proxy
         proxyA1.delete()
 
@@ -291,15 +291,15 @@
     def test_delete_A1_no_save( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
         parent = proxyA1.ultimate_parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         countA = len( proxyA.get_subdoc_container() )
         countA1 = len( proxyA1.get_subdoc_container() )
         key = proxyA1.key
 
         # delete the level one proxy
         proxyA1.delete( autosave=False )
 
@@ -329,15 +329,15 @@
         # verify that the key no longer exists
         assert 'nameA' not in proxy
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : proxy.parent['_id'] } )
 
         # verify that the key no longer exists in the database as well
         assert 'nameA' not in doc['proxyA'][ proxy.seq ]
 
 
 
 class TestDelItem_A1:
@@ -354,15 +354,15 @@
         # verify that the key no longer exists
         assert 'nameA1' not in proxy
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
 
         # verify that the key no longer exists in the database as well
         assert 'nameA1' not in doc['proxyA'][ proxy.parent.seq ]['proxyA1'][ proxy.seq ]
 
 
 
 class TestSetDefault:
@@ -438,15 +438,15 @@
         assert 'newKey' in proxy
         assert proxy['newKey'] == 'this is a new value'
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : proxy.parent['_id'] } )
 
         # verify that the new key exists in the database as well
         assert 'newKey' in doc['proxyA'][ proxy.seq ]
         assert doc['proxyA'][ proxy.seq ]['newKey'] == 'this is a new value'
 
 
 
@@ -465,15 +465,15 @@
         assert 'newKey' in proxy
         assert proxy['newKey'] == 'this is a new value'
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
 
         # verify that the new key exists in the database as well
         assert 'newKey' in doc['proxyA'][ proxy.parent.seq ]['proxyA1'][ proxy.seq ]
         assert doc['proxyA'][ proxy.parent.seq ]['proxyA1'][ proxy.seq ]['newKey'] == 'this is a new value'
 
 
 
@@ -529,37 +529,65 @@
         assert proxy['newKey2'] == 2
         assert len( proxy.keys() ) == count + 2
 
 
 
 
 class TestBasics:
+    def test_copy( self, getSampleProxyA ):
+        proxyA = getSampleProxyA
+        copied = proxyA.copy()
+
+        # Verify data is the same
+        assert copied == proxyA.data()
+        # Verify that data location is not the same
+        assert id( copied ) != id( proxyA.data() )
+
+
     def test_create_key( self, getPopulatedMMUDClasses, getSampleProxyA ):
-        '''Test key creation for single and two-level proxies'''
+        """Test key creation for single and two-level proxies"""
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
         updated = parent['_updated']
 
         # create a proxyA key
-        keyA = classes['A'].create_key( parent )
+        keyA = classes['A'].create_key( parent, {} )
         assert isinstance( keyA, str )
         assert keyA == f"{parent['_last_unique_integer']:x}"
 
         # create a proxyA1 key
-        keyA1 = classes['A1'].create_key( proxyA )
+        keyA1 = classes['A1'].create_key( proxyA, {} )
         assert isinstance( keyA1, str )
         assert keyA1 == f"{parent['_last_unique_integer']:x}"
         assert keyA != keyA1
 
         # verify that create_key doesn't save the parent object
-        doc = classes['base'].collection().find_one( { '_id' : parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : parent['_id'] } )
         assert doc['_updated'] == updated
 
 
+    def test_create_key_override( self, getPopulatedMMUDClasses, getSampleParent ):
+        """Test custom key creation"""
+        parent = getSampleParent
+        subdoc = { 'custom' : 'XYZ', 'more-data' : 3.1415 }
+
+        class LocalProxyClass( getPopulatedMMUDClasses['A'] ):
+            @classmethod
+            def create_key( cls, parent, subdoc ):
+                return subdoc['custom']
+
+        # confirm key is extracted as expected
+        assert LocalProxyClass.create_key( parent, subdoc ) == 'XYZ'
+
+        # confirm a new object uses the expected key
+        proxy = LocalProxyClass.create( parent, subdoc )
+        assert proxy.key == 'XYZ'
+
+
     def test_contains( self, getSampleProxyA ):
         proxy = getSampleProxyA
         assert 'nameA' in proxy
         assert 'will-not-match' not in proxy
 
 
     def test_contains_A1( self, getSampleProxyA1 ):
@@ -576,14 +604,27 @@
 
     def test_data_A1( self, getSampleProxyA1 ):
         proxy = getSampleProxyA1
         # verify that the data references the same dictionary
         assert id( proxy.data() ) == id( proxy.ultimate_parent['proxyA'][ proxy.parent.seq ]['proxyA1'][ proxy.seq ] )
 
 
+    def test_exists( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxy = getSampleProxyA
+        # verify the class can find this key within this parent
+        assert classes['A'].exists( proxy.parent, proxy.key )
+
+
+    def test_exists_non_existent( self, getPopulatedMMUDClasses, getSampleParent ):
+        classes = getPopulatedMMUDClasses
+        # verify a non-existent key can't be located
+        assert not classes['A'].exists( getSampleParent, 'non-existent-key' )
+
+
     def test_get( self, getSampleProxyA ):
         proxy = getSampleProxyA
         assert proxy.get('nameA') is not None
         assert proxy.get('will-not-match') is None
 
 
     def test_get( self, getSampleProxyA1 ):
@@ -619,15 +660,15 @@
             subdoc_key_name = 'alt-subdoc-key-name'
 
         sample = { 'alt-subdoc-key-name' : 'proxy-key'}
         assert MyAltListProxy.get_key( sample ) == 'proxy-key'
 
 
     def test_get_proxies( self, getPopulatedMMUDClasses, getSampleParent ):
-        '''Test accessing both first-level and second-level proxy lists'''
+        """Test accessing both first-level and second-level proxy lists"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # get all first-level proxies
         result = classes['A'].get_proxies( parent )
 
         # verify type and length of the result
@@ -650,24 +691,24 @@
 
         # verify type matches
         for proxy in result:
             assert isinstance( proxy, classes['A1'])
 
 
     def test_get_proxies_empty( self, getPopulatedMMUDClasses ):
-        '''Test get proxies from an empty object'''
+        """Test get proxies from an empty object"""
         classes = getPopulatedMMUDClasses
 
         # collect proxies from an empty object
         result = classes['A'].get_proxies( {} )
         assert len(result) == 0
 
 
     def test_get_proxy( self, getPopulatedMMUDClasses, getSampleParent ):
-        '''Test accessing both first-level and second-level proxies'''
+        """Test accessing both first-level and second-level proxies"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # locate the key for the first entry in the proxy A container
         keyA = parent[ classes['A'].container_name ][0][ classes['A'].subdoc_key_name ]
 
         # create a first-level proxy object
@@ -685,15 +726,15 @@
 
         # verify dictionary and type matches
         assert id( proxyA1.data() ) == id( parent[ classes['A'].container_name ][0][ classes['A1'].container_name ][0] )
         assert isinstance( proxyA1, classes['A1'] )
 
 
     def test_get_proxy_by_sequence( self, getPopulatedMMUDClasses, getSampleParent ):
-        '''Test accessing both first-level and second-level proxies'''
+        """Test accessing both first-level and second-level proxies"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # create a first-level proxy object
         proxyA = classes['A'].get_proxy( parent, seq=0 )
 
         # verify dictionary and type matches
@@ -737,27 +778,27 @@
         proxyA1 = getSampleProxyA1
 
         # verify data location
         assert id( proxyA1.get_subdoc_container() ) == id( proxyA1.ultimate_parent[ classes['A'].container_name ][ proxyA1.parent.seq ][ classes['A1'].container_name ] )
 
 
     def test_id( self, getSampleProxyA ):
-        '''Test ID for single level proxy'''
+        """Test ID for single level proxy"""
         proxy = getSampleProxyA
         assert proxy.id() == f"{proxy.parent.id()}{proxy.parent.subdoc_key_sep}{proxy.key}"
 
 
     def test_id_A1( self, getSampleProxyA1 ):
-        '''Test ID for two-level proxy'''
+        """Test ID for two-level proxy"""
         proxy = getSampleProxyA1
         assert proxy.id() == f"{proxy.ultimate_parent.id()}{proxy.ultimate_parent.subdoc_key_sep}{proxy.parent.key}{proxy.ultimate_parent.subdoc_key_sep}{proxy.key}"
 
 
     def test_init( self, getPopulatedMMUDClasses, getSampleParent ):
-        '''Test initialization of single and two-level proxies'''
+        """Test initialization of single and two-level proxies"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # pick the first proxyA key
         keyA = parent[ classes['A'].container_name ][0][ classes['A'].subdoc_key_name ]
 
         # create the proxy
@@ -773,38 +814,38 @@
         proxyA1 = classes['A1']( proxyA, keyA1 )
 
         # verify that the data references the same dictionary
         assert id( proxyA1.data() ) == id( parent['proxyA'][0]['proxyA1'][0] )
 
 
     def test_init_bad_key( self, getPopulatedMMUDClasses, getSampleParent ):
-        '''Test initialization of single and two-level proxies'''
+        """Test initialization of single and two-level proxies"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # creating a first-level proxy with a bad key raises an exception
         # proxy must be accessed before the invalid key is detected
         with pytest.raises( Exception ):
             proxyA = classes['A']( parent, 'not-a-valid-key')
             proxyA.keys()
 
         # create a proxy for the first proxyA key
         proxyA = classes['A']( parent, seq=0 )
 
-        # creating a first-level proxy with a bad key raises an exception
+        # creating a second-level proxy with a bad key raises an exception
         # proxy must be accessed before the invalid key is detected
         with pytest.raises( Exception ):
             proxyA1 = classes['A1']( proxyA, 'not-a-valid-key')
             proxyA1.keys()
 
 
 
     def test_init_bad_seq( self, getPopulatedMMUDClasses, getSampleParent ):
-        '''Test initialization of single and two-level proxies with a bad sequence.
-        Invalid sequence values are automatically corrected.'''
+        """Test initialization of single and two-level proxies with a bad sequence.
+        Invalid sequence values are automatically corrected."""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # pick the first proxyA key
         keyA = parent[ classes['A'].container_name ][0][ classes['A'].subdoc_key_name ]
 
         # create the proxy with a bad sequence
@@ -820,15 +861,15 @@
         proxyA1 = classes['A1']( proxyA, keyA1, seq=1.0 )
 
         # verify that the data references the same dictionary
         assert id( proxyA1.data() ) == id( parent['proxyA'][0]['proxyA1'][0] )
 
 
     def test_init_sequence( self, getPopulatedMMUDClasses, getSampleParent ):
-        '''Test initialization of single and two-level proxies'''
+        """Test initialization of single and two-level proxies"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # create the proxy
         proxyA = classes['A']( parent, seq=0 )
 
         # verify that the data references the same dictionary
@@ -864,34 +905,179 @@
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
 
         assert proxyA1.keys() == proxyA1.ultimate_parent[ classes['A'].container_name ][ proxyA.seq ][ classes['A1'].container_name ][ proxyA1.seq ].keys()
 
 
+    def test_load_proxy_by_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['A'] )
+
+        # verify the objects are the same
+        assert result.data() == proxyA.data()
+
+        # verify the parent is not readonly
+        assert result.ultimate_parent.readonly is False
+
+
+
+    def test_load_proxy_by_id_readonly( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['A'], readonly=True )
+
+        # verify the objects are the same
+        assert result.data() == proxyA.data()
+
+        # verify the parent is readonly
+        assert result.ultimate_parent.readonly is True
+
+
+    def test_load_proxy_by_id_invalid_proxy_id( self, getPopulatedMMUDClasses ):
+        """Test load_proxy_by_id() with a totally invalid ID"""
+        classes = getPopulatedMMUDClasses
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( 'this-is-not-a-proxy-id', classes['A'] )
+
+        # verify the return value is None
+        assert result == None
+
+
+    def test_load_proxy_by_id_invalid_object_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        """Test load_proxy_by_id() with a non-existent ObjectId"""
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # tamper with the ID to replace its ObjectId
+        proxyId = str( ObjectId() ) + proxyA.id()[24:]
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyId, classes['A'] )
+
+        # verify the return value is None
+        assert result == None
+
+
+    def test_load_proxy_by_id_invalid_local_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        """Test load_proxy_by_id() with a non-existent proxy ID"""
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # Can't load proxyB with proxyA's ID
+        with pytest.raises( mongo_objects.MongoObjectsNonexistentKey ):
+            result = classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['B'] )
+            # list proxies are lazy lookups and must be used to be resolved
+            result.keys()
+
+
+    def test_load_proxy_by_id_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'], classes['A1'] )
+
+        # verify the objects are the same
+        assert result.data() == proxyA1.data()
+
+        # verify the parent is not readonly
+        assert result.ultimate_parent.readonly is False
+
+
+    def test_load_proxy_by_id_readonly_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'], classes['A1'], readonly=True )
+
+        # verify the objects are the same
+        assert result.data() == proxyA1.data()
+
+        # verify the parent is readonly
+        assert result.ultimate_parent.readonly is True
+
+
+    def test_load_proxy_by_local_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # reload the proxy by its local ID
+        result = proxyA.ultimate_parent.load_proxy_by_local_id( proxyA.proxy_id(), classes['A'] )
+
+        # verify the objects are the same
+        assert result.data() == proxyA.data()
+
+
+    def test_load_proxy_by_local_id_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # reload the proxy by its ID
+        result = proxyA1.ultimate_parent.load_proxy_by_local_id( proxyA1.proxy_id(), classes['A'], classes['A1'] )
+
+        # verify the objects are the same
+        assert result.data() == proxyA1.data()
+
+
+    def test_id_A1( self, getSampleProxyA1 ):
+        """Test second level proxy ID"""
+        proxy = getSampleProxyA1
+        assert proxy.proxy_id() == f"{proxy.parent.key}{proxy.ultimate_parent.subdoc_key_sep}{proxy.key}"
+
+
+    def test_id_A1_id_with_parent_id( self, getSampleProxyA1 ):
+        """Test second level proxy ID with parent ID.
+        This should be the same as id()"""
+        proxy = getSampleProxyA1
+        assert proxy.proxy_id( include_parent_doc_id=True ) == f"{proxy.ultimate_parent.id()}{proxy.ultimate_parent.subdoc_key_sep}{proxy.parent.key}{proxy.ultimate_parent.subdoc_key_sep}{proxy.key}"
+        assert proxy.proxy_id( include_parent_doc_id=True ) == proxy.id()
+
+
+    def test_proxy_id( self, getSampleProxyA ):
+        """Test single level proxy ID"""
+        proxy = getSampleProxyA
+        assert proxy.proxy_id() == f"{proxy.key}"
+
+
+    def test_proxy_id_with_parent_id( self, getSampleProxyA ):
+        """Test single level proxy ID with parent ID
+        This should be the same as id()"""
+        proxy = getSampleProxyA
+        assert proxy.proxy_id( include_parent_doc_id=True ) == f"{proxy.parent.id()}{proxy.parent.subdoc_key_sep}{proxy.key}"
+        assert proxy.proxy_id( include_parent_doc_id=True ) == proxy.id()
+
+
     def test_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # preserve original state
-        original = dict( proxyA.parent )
+        original = proxyA.parent.copy()
 
         # save the object
         proxyA.save()
 
         # verify the parent document was saved
         assert proxyA.parent['_updated'] > original['_updated']
 
 
     def test_save_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # preserve original state
-        original = dict( proxyA1.ultimate_parent )
+        original = proxyA1.ultimate_parent.copy()
 
         # save the object
         proxyA1.save()
 
         # verify the parent document was saved
         assert proxyA1.ultimate_parent['_updated'] > original['_updated']
```

### Comparing `mongo_objects-1.1.2/tests/test_MongoSingleProxy.py` & `mongo_objects-1.2.0/tests/test_MongoSingleProxy.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,35 +6,32 @@
 from pymongo.collection import Collection
 import pytest
 import secrets
 
 
 @pytest.fixture( scope='class' )
 def getMMUDClasses( mongo_db ):
-    '''Return a MongoUserDict configured for a per-class unique collection
-
-    Since the single proxy classes are used multiple times,
-    we don't provide a container_name. Otherwise, each instance
-    would use the same location by default.'''
+    """Return a MongoUserDict configured for a per-class unique collection
+    """
 
     class MyMongoUserDict( mongo_objects.MongoUserDict ):
         collection_name = secrets.token_hex(6)
         database = mongo_db
 
     class MyMongoSingleProxyA( mongo_objects.MongoSingleProxy ):
-        pass
+        container_name = 'proxyA'
 
     class MyMongoSingleProxyA1( mongo_objects.MongoSingleProxy ):
-        pass
+        container_name = 'proxyA1'
 
     class MyMongoSingleProxyB( mongo_objects.MongoSingleProxy ):
-        pass
+        container_name = 'proxyB'
 
     return {
-        'base' : MyMongoUserDict,
+        'parent_doc' : MyMongoUserDict,
         'A' : MyMongoSingleProxyA,
         'A1' : MyMongoSingleProxyA1,
         'B' : MyMongoSingleProxyB
     }
 
 
 
@@ -42,236 +39,208 @@
 def getPopulatedMMUDClasses( getMMUDClasses ):
 
     classes = getMMUDClasses
     itemMax = 3     # make three of everything
 
     # make parent objects
     for i in range( itemMax ):
-        parent = classes['base']( {
+        parent = classes['parent_doc']( {
             'name' : f"Record {i}",
             'amount' : i * 10,
         } )
 
         # make first-level proxies
-        for j in range( itemMax ):
-            proxyA = classes['A'].create(
-                parent,
-                {
-                    'nameA' : f"Proxy A-{j}",
-                    'amountA' : j * 100,
-                },
-                key=f"proxyA-{j}",
-            )
-            proxyB = classes['B'].create(
-                parent,
-                {
-                    'nameB' : f"Proxy B-{j}",
-                    'amountB' : j * 100 + 1,
-                },
-                key=f"proxyB-{j}"
-            )
-
-            # make second-level proxies
-            for k in range( itemMax ):
-                proxyA1 = classes['A1'].create(
-                    proxyA,
-                    {
-                        'nameA1' : f"Proxy A1-{k}",
-                        'amountA1' : k * 1000,
-                    },
-                    key=f"proxyA1-{k}"
-                )
+        proxyA = classes['A'].create(
+            parent,
+            {
+                'nameA' : f"Proxy A",
+                'amountA' : 100,
+            },
+        )
+        proxyB = classes['B'].create(
+            parent,
+            {
+                'nameB' : f"Proxy B",
+                'amountB' : 101,
+            },
+        )
+
+        proxyA1 = classes['A1'].create(
+            proxyA,
+            {
+                'nameA1' : f"Proxy A1",
+                'amountA1' : 1000,
+            },
+        )
 
         # save data
         parent.save()
 
     return classes
 
 
 @pytest.fixture( scope='class' )
 def getSampleParent( getPopulatedMMUDClasses ):
     classes = getPopulatedMMUDClasses
     # find a random entry of the base class
-    return classes['base'].find_one()
-
-
-@pytest.fixture( scope='class' )
-def getSampleProxyAKey():
-    '''Return a fixed sample key for first-level A proxy testing'''
-    return 'proxyA-0'
+    return classes['parent_doc'].find_one()
 
 
 @pytest.fixture( scope='class' )
-def getSampleProxyA( getPopulatedMMUDClasses, getSampleParent, getSampleProxyAKey ):
+def getSampleProxyA( getPopulatedMMUDClasses, getSampleParent ):
     classes = getPopulatedMMUDClasses
-    return classes['A'].get_proxy( getSampleParent, getSampleProxyAKey )
+    return classes['A'].get_proxy( getSampleParent )
 
 
 @pytest.fixture( scope='class' )
-def getSampleProxyA1Key():
-    '''Return a fixed sample key for second-level A1 proxy testing'''
-    return 'proxyA1-0'
-
-
-@pytest.fixture( scope='class' )
-def getSampleProxyA1( getPopulatedMMUDClasses, getSampleProxyA, getSampleProxyA1Key ):
+def getSampleProxyA1( getPopulatedMMUDClasses, getSampleProxyA ):
     classes = getPopulatedMMUDClasses
-    return classes['A1'].get_proxy( getSampleProxyA, getSampleProxyA1Key )
+    return classes['A1'].get_proxy( getSampleProxyA )
 
 
 
 
 class TestCreate:
-    def test_create( self, getPopulatedMMUDClasses, getSampleProxyA ):
-        classes = getPopulatedMMUDClasses
-        proxyA = getSampleProxyA
-        parent = proxyA.parent
+    def test_create( self, getMMUDClasses ):
+        classes = getMMUDClasses
 
         # record current state
-        original = dict( parent )
-        count = len( proxyA.get_subdoc_container().keys() )
+        parent = classes['parent_doc']()
+        parent.save()
+        original = parent.copy()
 
         # create a new entry in a level one proxy
         newProxy = classes['A'].create(
             parent,
             { 'name' : 'new proxyA entry'},
-            key='newProxyA'
         )
 
         # verify a new entry was created
-        assert len( proxyA.get_subdoc_container().keys() ) == count+1
+        assert len( parent.keys() ) == len( original.keys() ) + 1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
+
 class TestCreateNoSave:
-    def test_create_no_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
-        classes = getPopulatedMMUDClasses
-        proxyA = getSampleProxyA
-        parent = proxyA.parent
+    def test_create_no_save( self, getMMUDClasses ):
+        classes = getMMUDClasses
 
         # record current state
-        original = dict( parent )
-        count = len( proxyA.get_subdoc_container().keys() )
+        parent = classes['parent_doc']()
+        parent.save()
+        original = parent.copy()
 
         # create a new entry in a level one proxy without saving the parent
         newProxy = classes['A'].create(
             parent,
             { 'name' : 'new proxyA entry'},
-            key='newProxyA',
             autosave=False
         )
 
         # verify a new entry was created
-        assert len( proxyA.get_subdoc_container().keys() ) == count+1
+        assert len( parent.keys() ) == len( original.keys() ) + 1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
+
 class TestCreateA1:
-    def test_create_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
-        classes = getPopulatedMMUDClasses
-        proxyA1 = getSampleProxyA1
-        proxyA = proxyA1.parent
-        parent = proxyA1.ultimate_parent
+    def test_create_A1( self, getMMUDClasses ):
+        classes = getMMUDClasses
+        parent = classes['parent_doc']()
+        proxyA = classes['A'].create( parent )
 
         # record current state
-        original = dict( parent )
-        countA = len( proxyA.get_subdoc_container().keys() )
-        countA1 = len( proxyA1.get_subdoc_container().keys() )
+        # this is a shallow copy, so we save proxyA separately
+        original_parent = parent.copy()
+        original_proxyA = proxyA.copy()
 
         # create a new entry in a level two proxy
-        newProxy = classes['A1'].create(
+        proxyA1 = classes['A1'].create(
             proxyA,
             { 'name' : 'new proxyA1 entry'},
-            key='newProxyA1'
         )
 
         # verify a new entry was created at the second (proxyA1) level
-        assert len( proxyA.get_subdoc_container().keys() ) == countA
-        assert len( proxyA1.get_subdoc_container().keys() ) == countA1 + 1
+        assert len( parent.keys() ) == len( original_parent.keys() )
+        assert len( proxyA.keys() ) == len( original_proxyA.keys() ) + 1
 
         # confirm the parent document was saved
-        assert parent['_updated'] > original['_updated']
+        assert parent['_updated'] > original_parent['_updated']
 
 
 class TestCreateA1NoSave:
-    def test_create_A1_no_save( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
-        classes = getPopulatedMMUDClasses
-        proxyA1 = getSampleProxyA1
-        proxyA = proxyA1.parent
-        parent = proxyA1.ultimate_parent
+    def test_create_A1_no_save( self, getMMUDClasses ):
+        classes = getMMUDClasses
+        parent = classes['parent_doc']()
+        proxyA = classes['A'].create( parent )
 
         # record current state
-        original = dict( parent )
-        countA = len( proxyA.get_subdoc_container().keys() )
-        countA1 = len( proxyA1.get_subdoc_container().keys() )
+        # this is a shallow copy, so we save proxyA separately
+        original_parent = parent.copy()
+        original_proxyA = proxyA.copy()
 
         # create a new entry in a level two proxy without saving the parent
-        newProxy = classes['A1'].create(
+        proxyA1 = classes['A1'].create(
             proxyA,
             { 'name' : 'new proxyA1 entry'},
-            key='newProxyA1',
             autosave=None
         )
 
         # verify a new entry was created at the second (proxyA1) level
-        assert len( proxyA.get_subdoc_container().keys() ) == countA
-        assert len( proxyA1.get_subdoc_container().keys() ) == countA1 + 1
+        assert len( parent.keys() ) == len( original_parent.keys() )
+        assert len( proxyA.keys() ) == len( original_proxyA.keys() ) + 1
 
         # confirm the parent document was not saved
-        assert parent['_updated'] == original['_updated']
+        assert parent['_updated'] == original_parent['_updated']
 
 
 
 
 class TestCreatecontainer_name:
     def test_create_by_container( self, getMMUDClasses ):
         classes = getMMUDClasses
         parent = {}
 
-        # adjust class to have a container name
-        classes['A'].container_name = 'proxyAByContainer'
-        classes['A1'].container_name = 'proxyA1ByContainer'
-
         # create a new entry in a first level proxy
         newProxyA = classes['A'].create(
             parent,
             { 'name' : 'new proxyA entry by container'},
             autosave=False
         )
 
         # verify a new first level entry was created
         assert len( parent.keys() ) == 1
-        assert 'proxyAByContainer' in parent
+        assert 'proxyA' in parent
 
         # create a new entry in a second level proxy
         newProxyA1 = classes['A1'].create(
             newProxyA,
             { 'name' : 'new proxyA1 entry by container'},
             autosave=False
         )
 
         # verify a new second level entry was created
         assert len( newProxyA1.keys() ) == 1
-        assert 'proxyA1ByContainer' in newProxyA
+        assert 'proxyA1' in newProxyA
 
 
 
 
 class TestDelete_ProxyA:
     def test_delete( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         count = len( proxyA.get_subdoc_container().keys() )
         key = proxyA.key
 
         # delete the level one proxy
         proxyA.delete()
 
         # verify the entry was deleted
@@ -286,15 +255,15 @@
 class TestDelete_ProxyA_No_Save:
     def test_delete_no_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         count = len( proxyA.get_subdoc_container().keys() )
         key = proxyA.key
 
         # delete the level one proxy without saving the parent
         proxyA.delete( autosave=False )
 
         # verify the entry was deleted
@@ -312,15 +281,15 @@
     def test_delete_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
         parent = proxyA1.ultimate_parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         countA = len( proxyA.get_subdoc_container().keys() )
         countA1 = len( proxyA1.get_subdoc_container().keys() )
         key = proxyA1.key
 
         # delete the level one proxy
         proxyA1.delete()
 
@@ -340,15 +309,15 @@
     def test_delete_A1_no_save( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
         parent = proxyA1.ultimate_parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         countA = len( proxyA.get_subdoc_container().keys() )
         countA1 = len( proxyA1.get_subdoc_container().keys() )
         key = proxyA1.key
 
         # delete the level one proxy
         proxyA1.delete( autosave=False )
 
@@ -378,15 +347,15 @@
         # verify that the key no longer exists
         assert 'nameA' not in proxy
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : proxy.parent['_id'] } )
 
         # verify that the key no longer exists in the database as well
         assert 'nameA' not in doc[ proxy.key ]
 
 
 
 class TestDelItem_A1:
@@ -403,15 +372,15 @@
         # verify that the key no longer exists
         assert 'nameA1' not in proxy
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
 
         # verify that the key no longer exists in the database as well
         assert 'nameA1' not in doc[ proxy.parent.key ][ proxy.key ]
 
 
 
 class TestSetDefault:
@@ -487,15 +456,15 @@
         assert 'newKey' in proxy
         assert proxy['newKey'] == 'this is a new value'
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : proxy.parent['_id'] } )
 
         # verify that the new key exists in the database as well
         assert 'newKey' in doc[ proxy.key ]
         assert doc[ proxy.key ]['newKey'] == 'this is a new value'
 
 
 
@@ -514,15 +483,15 @@
         assert 'newKey' in proxy
         assert proxy['newKey'] == 'this is a new value'
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
 
         # verify that the new key exists in the database as well
         assert 'newKey' in doc[ proxy.parent.key ][ proxy.key ]
         assert doc[ proxy.parent.key ][ proxy.key ]['newKey'] == 'this is a new value'
 
 
 
@@ -578,34 +547,44 @@
         assert proxy['newKey2'] == 2
         assert len( proxy.keys() ) == count + 2
 
 
 
 
 class TestBasics:
+    def test_copy( self, getSampleProxyA ):
+        proxyA = getSampleProxyA
+        copied = proxyA.copy()
+
+        # Verify data is the same
+        assert copied == proxyA.data()
+        # Verify that data location is not the same
+        assert id( copied ) != id( proxyA.data() )
+
+
     def test_create_key( self, getPopulatedMMUDClasses, getSampleProxyA ):
-        '''Test key creation for single and two-level proxies'''
+        """Test key creation for single and two-level proxies"""
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
         updated = parent['_updated']
 
         # create a proxyA key
-        keyA = classes['A'].create_key( parent )
+        keyA = classes['A'].create_key( parent, {} )
         assert isinstance( keyA, str )
         assert keyA == f"{parent['_last_unique_integer']:x}"
 
         # create a proxyA1 key
-        keyA1 = classes['A1'].create_key( proxyA )
+        keyA1 = classes['A1'].create_key( proxyA, {} )
         assert isinstance( keyA1, str )
         assert keyA1 == f"{parent['_last_unique_integer']:x}"
         assert keyA != keyA1
 
         # verify that create_key doesn't save the parent object
-        doc = classes['base'].collection().find_one( { '_id' : parent['_id'] } )
+        doc = classes['parent_doc'].collection().find_one( { '_id' : parent['_id'] } )
         assert doc['_updated'] == updated
 
 
     def test_contains( self, getSampleProxyA ):
         proxy = getSampleProxyA
         assert 'nameA' in proxy
         assert 'will-not-match' not in proxy
@@ -625,14 +604,58 @@
 
     def test_data_A1( self, getSampleProxyA1 ):
         proxy = getSampleProxyA1
         # verify that the data references the same dictionary
         assert id( proxy.data() ) == id( proxy.ultimate_parent[proxy.parent.key][proxy.key] )
 
 
+    def test_exists_1( self, getPopulatedMMUDClasses, getSampleParent ):
+        classes = getPopulatedMMUDClasses
+        parent = getSampleParent
+        # verify the class can find this key within this parent
+        # exists() uses the container_name from the single proxy class
+        assert classes['A'].exists( parent )
+
+
+    def test_exists_2( self, getPopulatedMMUDClasses, getSampleParent ):
+        classes = getPopulatedMMUDClasses
+        parent = getSampleParent
+        # verify the class can find this key within this parent
+        assert classes['A'].exists( parent, classes['A'].container_name )
+
+
+    def test_exists_3( self, getPopulatedMMUDClasses, getSampleParent ):
+        classes = getPopulatedMMUDClasses
+        parent = getSampleParent
+        # verify the class can find this key within this parent
+        # even with a bad key, since exists() ignored the key for
+        # single proxies
+        assert classes['A'].exists( parent, 'not-existent key' )
+
+
+    def test_exists_non_existent_1( self, getMMUDClasses ):
+        classes = getMMUDClasses
+        # verify a proxy can't be located in an empty document
+        assert not classes['A'].exists( {} )
+
+
+    def test_exists_non_existent_2( self, getMMUDClasses ):
+        classes = getMMUDClasses
+        # verify a proxy can't be located in an empty document
+        # even with the correct key name (which exists() ignores for single proxies)
+        assert not classes['A'].exists( {}, classes['A'].container_name )
+
+
+    def test_exists_non_existent_( self, getMMUDClasses ):
+        classes = getMMUDClasses
+        # verify a proxy can't be located in an empty document
+        # with an incorrect key name (which is also ignored by exists())
+        assert not classes['A'].exists( {}, 'non-existent key' )
+
+
     def test_get( self, getSampleProxyA ):
         proxy = getSampleProxyA
         assert proxy.get('nameA') is not None
         assert proxy.get('will-not-match') is None
 
 
     def test_get( self, getSampleProxyA1 ):
@@ -652,46 +675,40 @@
         proxy = getSampleProxyA1
         assert proxy['nameA1'] is not None
         with pytest.raises( Exception ):
             assert proxy['will-not-match']
 
 
     def test_get_proxies( self, getPopulatedMMUDClasses, getSampleParent ):
-        '''single proxy objects don't support get_proxies()'''
+        """single proxy objects don't support get_proxies()"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         with pytest.raises( Exception ):
             classes['A'].get_proxies( parent )
 
 
-    def test_get_proxy( self, getPopulatedMMUDClasses, getSampleParent, getSampleProxyAKey ):
-        '''Test accessing both first-level and second-level proxies'''
+    def test_get_proxy( self, getPopulatedMMUDClasses, getSampleParent ):
+        """Test accessing both first-level and second-level proxies"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
-        # locate the first key in the proxy A container
-        keyA = getSampleProxyAKey
-
         # create a first-level proxy object
-        proxyA = classes['A'].get_proxy( parent, keyA )
+        proxyA = classes['A'].get_proxy( parent )
 
         # verify dictionary and type matches
-        assert id( proxyA.data() ) == id( parent[ keyA ] )
-        assert isinstance( proxyA, classes['A'])
-
-        # locate the first key in the proxy A1 container
-        keyA1 = list( parent[ keyA ].keys() )[0]
+        assert id( proxyA.data() ) == id( parent[ classes['A'].container_name ] )
+        assert isinstance( proxyA, classes['A'] )
 
         # create a second-level proxy object
-        proxyA1 = classes['A1'].get_proxy( proxyA, keyA1 )
+        proxyA1 = classes['A1'].get_proxy( proxyA )
 
         # verify dictionary and type matches
-        assert id( proxyA1.data() ) == id( parent[ keyA ][ keyA1 ] )
-        assert isinstance( proxyA1, classes['A1'])
+        assert id( proxyA1.data() ) == id( parent[ classes['A'].container_name ][ classes['A1'].container_name ] )
+        assert isinstance( proxyA1, classes['A1'] )
 
 
     def test_get_subdoc( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # verify data location
@@ -719,60 +736,85 @@
         proxyA1 = getSampleProxyA1
 
         # verify data location
         assert id( proxyA1.get_subdoc_container() ) == id( proxyA1.parent )
 
 
     def test_id( self, getSampleProxyA ):
-        '''Test ID for single level proxy'''
+        """Test ID for single level proxy"""
         proxy = getSampleProxyA
         assert proxy.id() == f"{proxy.parent.id()}{proxy.parent.subdoc_key_sep}0"
 
 
     def test_id_A1( self, getSampleProxyA1 ):
-        '''Test ID for two-level proxy'''
+        """Test ID for two-level proxy"""
         proxy = getSampleProxyA1
         assert proxy.id() == f"{proxy.ultimate_parent.id()}{proxy.ultimate_parent.subdoc_key_sep}0{proxy.ultimate_parent.subdoc_key_sep}0"
 
 
-    def test_init( self, getPopulatedMMUDClasses, getSampleParent, getSampleProxyAKey, getSampleProxyA1Key ):
-        '''Test initialization of single and two-level proxies'''
+    def test_init( self, getPopulatedMMUDClasses, getSampleParent ):
+        """Test initialization of single and two-level proxies"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
-        keyA = getSampleProxyAKey
-        keyA1 = getSampleProxyA1Key
 
-        # create the proxy
-        proxyA = classes['A']( parent, keyA )
+        # Create the proxy
+        # No key is needed since it comes from cls.container_name
+        proxyA = classes['A']( parent )
 
         # verify that the data references the same dictionary
-        assert id( proxyA.data() ) == id( parent[keyA] )
+        assert id( proxyA.data() ) == id( parent[ classes['A'].container_name ] )
+
+        # verify that the proxy key matches the class container name
+        assert proxyA.key == classes['A'].container_name
 
         # create the proxy
-        proxyA1 = classes['A1']( proxyA, keyA1 )
+        proxyA1 = classes['A1']( proxyA )
 
         # verify that the data references the same dictionary
-        assert id( proxyA1.data() ) == id( parent[keyA][keyA1] )
+        assert id( proxyA1.data() ) == id( parent[ classes['A'].container_name ][ classes['A1'].container_name ] )
+
+        # verify that the proxy key matches the class container name
+        assert proxyA.key == classes['A'].container_name
 
 
-    def test_init_bad_key( self, getPopulatedMMUDClasses, getSampleParent, getSampleProxyAKey ):
-        '''Test initialization of single and two-level proxies'''
+    def test_init_with_key( self, getPopulatedMMUDClasses, getSampleParent ):
+        """Test initialization of single and two-level proxies
+        that the key is ignored"""
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
-        # creating a first-level proxy with a bad key raises an exception
-        with pytest.raises( Exception ):
-            classes['A']( parent, 'not-a-valid-key')
+        # Create a first-level proxy with and without a key
+        proxyA = classes['A']( parent )
+        proxyAWithKey = classes['A']( parent, classes['A'].container_name )
+
+        # verify that the data references the same dictionary
+        assert id( proxyA.data() ) == id(proxyAWithKey.data() )
 
-        # create a first-level proxy
-        proxyA = classes['A']( parent, getSampleProxyAKey )
+        # create the second level proxies
+        proxyA1 = classes['A1']( proxyA )
+        proxyA1WithKey = classes['A1']( proxyA, classes['A1'].container_name )
 
-        # creating a first-level proxy with a bad key raises an exception
-        with pytest.raises( Exception ):
-            classes['A1']( proxyA, 'not-a-valid-key')
+        # verify that the data references the same dictionary
+        assert id( proxyA1.data() ) == id(proxyA1WithKey.data() )
+
+
+    def test_init_bad_key( self, getPopulatedMMUDClasses, getSampleParent ):
+        """Test initialization of single and two-level proxies"""
+        classes = getPopulatedMMUDClasses
+        parent = getSampleParent
+
+        # creating a first-level proxy ignores a bad key
+        # the data still points to the same place as a normal proxy
+        proxyA = classes['A']( parent, 'not-a-valid-key')
+        assert id( proxyA.data() ) == id( classes['A']( parent ).data() )
+
+        # creating a second-level proxy ignores a bad key
+        # the data still points to the same place as a normal proxy
+        proxyA1 = classes['A1']( proxyA, 'not-a-valid-key')
+        assert id( proxyA1.data() ) == id( classes['A1']( proxyA ).data() )
 
 
 
     def test_items( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxy = getSampleProxyA
 
@@ -810,34 +852,179 @@
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
 
         assert proxyA1.keys() == proxyA1.ultimate_parent[ proxyA.key ][ proxyA1.key ].keys()
 
 
+    def test_load_proxy_by_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['A'] )
+
+        # verify the objects are the same
+        assert result.data() == proxyA.data()
+
+        # verify the parent is not readonly
+        assert result.ultimate_parent.readonly is False
+
+
+
+    def test_load_proxy_by_id_readonly( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['A'], readonly=True )
+
+        # verify the objects are the same
+        assert result.data() == proxyA.data()
+
+        # verify the parent is readonly
+        assert result.ultimate_parent.readonly is True
+
+
+    def test_load_proxy_by_id_invalid_proxy_id( self, getPopulatedMMUDClasses ):
+        """Test load_proxy_by_id() with a totally invalid ID"""
+        classes = getPopulatedMMUDClasses
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( 'this-is-not-a-proxy-id', classes['A'] )
+
+        # verify the return value is None
+        assert result == None
+
+
+    def test_load_proxy_by_id_invalid_object_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        """Test load_proxy_by_id() with a non-existent ObjectId"""
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # tamper with the ID to replace its ObjectId
+        proxyId = str( ObjectId() ) + proxyA.id()[24:]
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyId, classes['A'] )
+
+        # verify the return value is None
+        assert result == None
+
+
+    def test_load_proxy_by_id_invalid_local_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        """Test load_proxy_by_id() with a non-existent proxy ID
+        Since single proxies get their key from :attr:`container_name`,
+        not the ID, this actually works."""
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # Loading class B with class A's ID will work and give us class B
+        result = classes['parent_doc'].load_proxy_by_id( proxyA.id(), classes['B'] )
+        assert isinstance( result, classes['B'] )
+
+
+    def test_load_proxy_by_id_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'], classes['A1'] )
+
+        # verify the objects are the same
+        assert result.data() == proxyA1.data()
+
+        # verify the parent is not readonly
+        assert result.ultimate_parent.readonly is False
+
+
+    def test_load_proxy_by_id_readonly_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # reload the proxy by its ID
+        result = classes['parent_doc'].load_proxy_by_id( proxyA1.id(), classes['A'], classes['A1'], readonly=True )
+
+        # verify the objects are the same
+        assert result.data() == proxyA1.data()
+
+        # verify the parent is readonly
+        assert result.ultimate_parent.readonly is True
+
+
+    def test_load_proxy_by_local_id( self, getPopulatedMMUDClasses, getSampleProxyA ):
+        classes = getPopulatedMMUDClasses
+        proxyA = getSampleProxyA
+
+        # reload the proxy by its local ID
+        result = proxyA.ultimate_parent.load_proxy_by_local_id( proxyA.proxy_id(), classes['A'] )
+
+        # verify the objects are the same
+        assert result.data() == proxyA.data()
+
+
+    def test_load_proxy_by_local_id_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+        classes = getPopulatedMMUDClasses
+        proxyA1 = getSampleProxyA1
+
+        # reload the proxy by its ID
+        result = proxyA1.ultimate_parent.load_proxy_by_local_id( proxyA1.proxy_id(), classes['A'], classes['A1'] )
+
+        # verify the objects are the same
+        assert result.data() == proxyA1.data()
+
+
+    def test_proxy_id( self, getSampleProxyA ):
+        """Test single level proxy ID"""
+        proxy = getSampleProxyA
+        assert proxy.proxy_id() == f"0"
+
+
+    def test_proxy_id_with_parent_id( self, getSampleProxyA ):
+        """Test single level proxy ID with parent ID
+        This should be the same as id()"""
+        proxy = getSampleProxyA
+        assert proxy.proxy_id( include_parent_doc_id=True ) == f"{proxy.parent.id()}{proxy.parent.subdoc_key_sep}0"
+        assert proxy.proxy_id( include_parent_doc_id=True ) == proxy.id()
+
+
+    def test_id_A1( self, getSampleProxyA1 ):
+        """Test second level proxy ID"""
+        proxy = getSampleProxyA1
+        assert proxy.proxy_id() == f"0{proxy.ultimate_parent.subdoc_key_sep}0"
+
+
+    def test_id_A1_id_with_parent_id( self, getSampleProxyA1 ):
+        """Test second level proxy ID with parent ID.
+        This should be the same as id()"""
+        proxy = getSampleProxyA1
+        assert proxy.proxy_id( include_parent_doc_id=True ) == f"{proxy.ultimate_parent.id()}{proxy.ultimate_parent.subdoc_key_sep}0{proxy.ultimate_parent.subdoc_key_sep}0"
+        assert proxy.proxy_id( include_parent_doc_id=True ) == proxy.id()
+
+
     def test_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # preserve original state
-        original = dict( proxyA.parent )
+        original = proxyA.parent.copy()
 
         # save the object
         proxyA.save()
 
         # verify the parent document was saved
         assert proxyA.parent['_updated'] > original['_updated']
 
 
     def test_save_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # preserve original state
-        original = dict( proxyA1.ultimate_parent )
+        original = proxyA1.ultimate_parent.copy()
 
         # save the object
         proxyA1.save()
 
         # verify the parent document was saved
         assert proxyA1.ultimate_parent['_updated'] > original['_updated']
```

### Comparing `mongo_objects-1.1.2/tests/test_MongoUserDict.py` & `mongo_objects-1.2.0/tests/test_MongoUserDict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # test_MongoUserDict
 
 from bson import ObjectId
-from datetime import datetime
+import datetime
 import mongo_objects
 from pymongo.collection import Collection
 import pytest
 import secrets
 
 
 @pytest.fixture(scope='session' )
@@ -27,15 +27,15 @@
 
         }
     ]
 
 
 @pytest.fixture( scope='class' )
 def getMMUDClass( mongo_db ):
-    '''Return a MongoUserDict configured for a per-class unique collection'''
+    """Return a MongoUserDict configured for a per-class unique collection"""
 
     class MyMongoUserDict( mongo_objects.MongoUserDict ):
         collection_name = secrets.token_hex(6)
         database = mongo_db
 
     return MyMongoUserDict
 
@@ -52,32 +52,32 @@
         obj.save()
     return MMUD
 
 
 
 @pytest.fixture( scope='class' )
 def getVersionedPopulatedMMUDClass( getMMUDClass, sampleData ):
-    '''Like getPopulatedMMUDClass except each document is saved
+    """Like getPopulatedMMUDClass except each document is saved
     with a different version number.
 
-    MMUD is left with the final object version number.'''
+    MMUD is left with the final object version number."""
 
     MMUD = getMMUDClass
 
     # for each entry in the sampleData, save it to the collection configured in MMUD
     for (ver, x) in enumerate( sampleData ):
         MMUD.object_version = ver+1
         obj = MMUD(x)
         obj.save()
     return MMUD
 
 
 
 class TestVersioning:
-    '''Test how various function perform with object versioning'''
+    """Test how various methods perform with object versioning"""
 
     def test_find_all_current_version( self, getVersionedPopulatedMMUDClass ):
         MMUD = getVersionedPopulatedMMUDClass
 
         # verify there is a current object version
         assert MMUD.object_version is not None
 
@@ -126,15 +126,15 @@
 
         # verify there is a current object version
         assert MMUD.object_version is not None
 
         # There should only be one document at the current version (the default query)
         matches = 0
         for doc in sampleData:
-            filter = dict( doc )
+            filter = doc.copy()
             result = MMUD.find_one( filter )
             if result is not None:
                 assert result['_objver'] == MMUD.object_version
                 matches += 1
 
         assert matches == 1
 
@@ -144,15 +144,15 @@
 
         # verify there is a current object version
         assert MMUD.object_version is not None
 
         # There should only be one document at version 1
         matches = 0
         for doc in sampleData:
-            filter = dict( doc )
+            filter = doc.copy()
             result = MMUD.find_one( filter, object_version=1 )
             if result is not None:
                 assert result['_objver'] == 1
                 matches += 1
 
         assert matches == 1
 
@@ -161,27 +161,27 @@
         MMUD = getVersionedPopulatedMMUDClass
 
         # verify there is a current object version
         assert MMUD.object_version is not None
 
         # Any document may be returned if object versioning is suppressed
         for doc in sampleData:
-            filter = dict( doc )
+            filter = doc.copy()
             assert MMUD.find_one( filter, object_version=False ) is not None
 
 
     def test_find_one_nonexistent_version( self, getVersionedPopulatedMMUDClass, sampleData ):
         MMUD = getVersionedPopulatedMMUDClass
 
         # verify there is a current object version
         assert MMUD.object_version is not None
 
         # None should be returned at a non-existent version for any document
         for doc in sampleData:
-            filter = dict( doc )
+            filter = doc.copy()
             assert MMUD.find_one( filter, object_version=10000000 ) is None
 
 
 
 class TestVersionedSave:
 
     def test_save_version( self, getVersionedPopulatedMMUDClass ):
@@ -222,22 +222,22 @@
 
         # verify that the object version was removed during rollback
         assert '_objver' not in obj
 
 
 
 class TestSave:
-    '''Test various permutations of MongoUserDict.save()
-    Other functionality is tested in a separate class'''
+    """Test various permutations of MongoUserDict.save()
+    Other functionality is tested in a separate class"""
 
     def test_save( self, getMMUDClass, sampleData ):
-        '''Verify a basic dictionary is saved properly.
+        """Verify a basic dictionary is saved properly.
         Confirm original object is updated with time and ID
         and that data is stored as expected in the database.
-        '''
+        """
 
         MMUD = getMMUDClass
 
         # count documents
         assert MMUD.collection().count_documents( {} ) == 0
 
         # record the current time
@@ -254,40 +254,40 @@
         assert '_id' in obj
         assert isinstance( obj['_id'], ObjectId )
 
         # verify that _created timestamp was added to original document
         # timestamp microseconds should be set to 0
         # time should be later than the start of this test (disregarding microseconds)
         assert '_created' in obj
-        assert isinstance( obj['_created'], datetime )
+        assert isinstance( obj['_created'], datetime.datetime )
         assert obj['_created'].microsecond % 1000 == 0
         assert obj['_created'].replace(microsecond=0) >= startTime.replace(microsecond=0)
 
         # verify that _updated was also added and matches _created
         assert '_updated' in obj
-        assert isinstance( obj['_updated'], datetime )
+        assert isinstance( obj['_updated'], datetime.datetime )
         assert obj['_created'] == obj['_updated']
 
         # save the document again and confirm _updated changes but _created doesn't
-        original = dict( obj )
+        original = obj.copy()
         obj.save()
         assert obj['_created'] == original['_created']
         assert obj['_updated'] > original['_updated']
 
         # find document directly from database driver
         doc = MMUD.collection().find_one( { '_id' : obj['_id'] } )
 
         # make sure the database object as the exact same data as the in-memory object
         assert len( set( obj.keys() ).symmetric_difference( doc.keys() ) ) == 0, "missing keys"
         for key in obj.keys():
             assert doc[key] == obj[key]
 
 
     def test_save_exception_1( self, getMMUDClass ):
-        '''Test that an exception saving a new document removes _created, _updated timestamps'''
+        """Test that an exception saving a new document removes _created, _updated timestamps"""
         MMUD = getMMUDClass
 
         # count documents
         count =  MMUD.collection().count_documents( {} )
 
         # Create an empty document
         obj = MMUD()
@@ -309,24 +309,24 @@
         # verify that _created and _updated were removed; _objver won't have been added anyway
         assert '_created' not in obj
         assert '_updated' not in obj
         assert '_objver' not in obj
 
 
     def test_save_exception_2( self, getMMUDClass ):
-        '''Test that an exception saving a previously saved document leaves the _updated timestamp unchanged'''
+        """Test that an exception saving a previously saved document leaves the _updated timestamp unchanged"""
         MMUD = getMMUDClass
 
         # count documents
         count = MMUD.collection().count_documents( {} )
 
         # save an empty document
         obj = MMUD()
         obj.save()
-        original = dict( obj )
+        original = obj.copy()
 
         # verify that the object was saved
         assert MMUD.collection().count_documents( {} ) == count + 1
 
         # Confirm _id, _created and _updated are all set
         assert '_id' in obj
         assert '_created' in obj
@@ -395,15 +395,15 @@
         doc = MMUD.collection().find_one( { '_id' : obj['_id'] } )
 
         # verify database object _updated timestamp
         assert doc['_updated'] == obj['_updated']
 
 
     def test_save_overwrite( self, getMMUDClass, sampleData ):
-        '''Test attempting to save over an already-updated object'''
+        """Test attempting to save over an already-updated object"""
         MMUD = getMMUDClass
 
         # count documents
         count =  MMUD.collection().count_documents( {} )
 
         # record the current time
         startTime = MMUD.utcnow()
@@ -434,45 +434,45 @@
 
         # locate object on disk and verify _updated matches obj (not obj2)
         doc = MMUD.collection().find_one( { '_id' : obj['_id'] } )
         assert doc['_updated'] == obj['_updated']
 
 
     def test_save_readonly( self, getPopulatedMMUDClass ):
-        '''Test attempting to save a readonly object'''
+        """Test attempting to save a readonly object"""
         MMUD = getPopulatedMMUDClass
         result = MMUD.find_one( readonly=True )
         assert result.readonly is True
 
         # saving a readonly document produces an exception
         with pytest.raises( mongo_objects.MongoObjectsReadOnly ):
             result.save()
 
 
     def test_save_no_auth( self, getPopulatedMMUDClass ):
-        '''Test attempting to save a document without authorization'''
+        """Test attempting to save a document without authorization"""
         class LocalMMUD( getPopulatedMMUDClass):
             def authorize_save( self ):
                 return False
 
         obj = LocalMMUD.find_one()
-        original = dict( obj )
+        original = obj.copy()
 
         # verify saving a document without authorization produces an exception
         with pytest.raises( mongo_objects.MongoObjectsAuthFailed ):
             obj.save()
 
         # verify nothing was saved
         assert obj['_updated'] == original['_updated']
 
 
 
 
 class TestDelete:
-    '''Test MongoUserDict.delete() in its own database'''
+    """Test MongoUserDict.delete() in its own database"""
 
     def test_delete( self, getMMUDClass, sampleData ):
         MMUD = getMMUDClass
 
         # save the first record
         obj = MMUD( sampleData[0] )
         obj.save()
@@ -487,15 +487,15 @@
         assert '_id' not in obj
 
         # verify a record was removed and the database is empty
         assert MMUD.collection().count_documents( {} ) == 0
 
 
     def test_delete_new( self, getMMUDClass, sampleData ):
-        '''Delete an object that was never saved. This should be a no-op'''
+        """Delete an object that was never saved. This should be a no-op"""
         MMUD = getMMUDClass
 
         # create but don't save the first record
         obj = MMUD( sampleData[0] )
 
         # verify that no _id is present
         assert '_id' not in obj
@@ -507,15 +507,15 @@
         obj.delete()
 
         # verify the database document count hasn't changed
         assert count == MMUD.collection().count_documents( {} )
 
 
     def test_delete_no_auth( self, getPopulatedMMUDClass ):
-        '''Test attempting to delete a document without authorization'''
+        """Test attempting to delete a document without authorization"""
         class LocalMMUD( getPopulatedMMUDClass):
             def authorize_delete( self ):
                 return False
 
         obj = LocalMMUD.find_one()
 
         # note the number of documents in the database
@@ -528,15 +528,15 @@
         # verify the database document count hasn't changed
         assert count == LocalMMUD.collection().count_documents( {} )
 
 
 
 
 class TestBasics:
-    '''Test all other functionality of MongoUserDict'''
+    """Test all other functionality of MongoUserDict"""
 
     def test_init( self, getMMUDClass, sampleData ):
         MMUD = getMMUDClass
         obj = MMUD( sampleData[0] )
         assert obj.data == sampleData[0]
         assert obj.readonly is False
 
@@ -569,16 +569,16 @@
 
         # verify initializing a document without authorization produces an exception
         with pytest.raises( mongo_objects.MongoObjectsAuthFailed ):
             obj = LocalMMUD( sampleData[0] )
 
 
     def test_add_object_version( self ):
-        '''Verify add_object_version adds the correct filter
-        The original filter should be left intact.'''
+        """Verify add_object_version adds the correct filter
+        The original filter should be left intact."""
         class LocalClass( mongo_objects.MongoUserDict ):
             object_version = 5
 
         # object_version = False never adds a filter
         filter = {}
         result = LocalClass.add_object_version_filter( filter, False )
         assert len(filter) == 0
@@ -595,17 +595,17 @@
         filter = {}
         result = LocalClass.add_object_version_filter( filter, 10 )
         assert len(filter) == 0
         assert result == { '_objver' : 10 }
 
 
     def test_add_object_version_empty( self ):
-        '''Verify add_object_version() if the class has no object version
+        """Verify add_object_version() if the class has no object version
         Since the class has no object version, no filter should be
-        added under any circumstances'''
+        added under any circumstances"""
         class LocalClass( mongo_objects.MongoUserDict ):
             pass
 
         # object_version = False never adds a filter
         filter = {}
         result = LocalClass.add_object_version_filter( filter, False )
         assert len(filter) == 0
@@ -672,15 +672,15 @@
         result = list( MMUD.find( { 'not-a-field' : 'wont-match-anything' } ) )
 
         # verify that we found nothing
         assert len( result ) == 0
 
 
     def test_find_single( self, getPopulatedMMUDClass, sampleData ):
-        '''Use a filter to find a single record, in this case, the first sample by name'''
+        """Use a filter to find a single record, in this case, the first sample by name"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         result = list( MMUD.find( { 'name' : sampleData[0]['name'] } ) )
 
@@ -689,15 +689,15 @@
 
         # since no projection was used and readonly wasn't True,
         # verify object is not marked readonly
         assert result[0].readonly is False
 
 
     def test_find_projection_1( self, getPopulatedMMUDClass ):
-        '''Test find() with a "positive" projection'''
+        """Test find() with a "positive" projection"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
@@ -707,15 +707,15 @@
             assert '_updated' not in x
             assert 'amount' in x
             assert 'name' not in x
             assert x.readonly is True
 
 
     def test_find_projection_2( self, getPopulatedMMUDClass ):
-        '''Test find() with a "positive" projection but suppress _id'''
+        """Test find() with a "positive" projection but suppress _id"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
@@ -725,15 +725,15 @@
             assert '_updated' not in x
             assert 'amount' not in x
             assert 'name' in x
             assert x.readonly is True
 
 
     def test_find_projection_3( self, getPopulatedMMUDClass ):
-        '''Test find() with a "negative" projection'''
+        """Test find() with a "negative" projection"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
@@ -743,15 +743,15 @@
             assert '_updated' in x
             assert 'amount' not in x
             assert 'name' in x
             assert x.readonly is True
 
 
     def test_find_projection_4( self, getPopulatedMMUDClass ):
-        '''Test find() with a "negative" projection and suppress _id'''
+        """Test find() with a "negative" projection and suppress _id"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
@@ -761,15 +761,15 @@
             assert '_updated' in x
             assert 'amount' in x
             assert 'name' not in x
             assert x.readonly is True
 
 
     def test_find_projection_5( self, getPopulatedMMUDClass ):
-        '''Test find() with a "negative" projection with readonly forced to False'''
+        """Test find() with a "negative" projection with readonly forced to False"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         # Verify projection produced the proper key set
         # Also confirm object is not marked readonly
@@ -792,39 +792,39 @@
 
         # verify all objects are marked readonly
         for x in result:
             assert x.readonly is True
 
 
     def test_find_no_pre_auth( self, getPopulatedMMUDClass ):
-        '''Test attempting to read without pre-authorization'''
+        """Test attempting to read without pre-authorization"""
         class LocalMMUD( getPopulatedMMUDClass ):
             @classmethod
             def authorize_pre_read( cls ):
                 return False
 
         # verify reading documents without pre-read authorization produces an exception
         # must convert to a list or the generator is never called
         with pytest.raises( mongo_objects.MongoObjectsAuthFailed ):
             list( LocalMMUD.find() )
 
 
     def test_find_no_auth_1( self, getPopulatedMMUDClass ):
-        '''Test attempting to read without authorization'''
+        """Test attempting to read without authorization"""
         class LocalMMUD( getPopulatedMMUDClass):
             def authorize_read( self ):
                 return False
 
         # verify reading documents without read authorization produces an empty list
         result = LocalMMUD.find()
         assert len( list( result ) ) == 0
 
 
     def test_find_no_auth_2( self, getPopulatedMMUDClass ):
-        '''Test attempting to read without authorization for certain objects'''
+        """Test attempting to read without authorization for certain objects"""
 
         # first collect a list of object IDs
         ids = [ x.id() for x in getPopulatedMMUDClass.find() ]
 
         # create a class authorized to read all but the first ID
         class LocalMMUD( getPopulatedMMUDClass):
             def authorize_read( self ):
@@ -836,15 +836,15 @@
         diff = list( set(ids).difference( ids2 ) )
         # verify that only ids[0] is missing (the ID excluded by authorize_read() )
         assert len( diff ) == 1
         assert diff[0] == ids[0]
 
 
     def test_find_one( self, getPopulatedMMUDClass ):
-        '''Test returning a single (random) object'''
+        """Test returning a single (random) object"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         result = MMUD.find_one()
         assert isinstance( result, MMUD )
@@ -853,56 +853,56 @@
         assert '_updated' in result
         assert 'amount' in result
         assert 'name' in result
         assert result.readonly is False
 
 
     def test_find_one_none( self, getPopulatedMMUDClass ):
-        '''Verify a non-matching filter produces a None result'''
+        """Verify a non-matching filter produces a None result"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         result = MMUD.find_one( { 'not-a-field' : 'wont-match-anything' } )
 
         # verify that we found nothing
         assert result is None
 
 
     def test_find_one_none_custom_return( self, getPopulatedMMUDClass ):
-        '''Verify a non-matching filter produces our custom "no_match" result'''
+        """Verify a non-matching filter produces our custom "no_match" result"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         class EmptyResponse( object ):
             pass
 
         result = MMUD.find_one( { 'not-a-field' : 'wont-match-anything' }, no_match=EmptyResponse() )
 
         assert isinstance( result, EmptyResponse )
 
 
     def test_find_one_filter( self, getPopulatedMMUDClass, sampleData ):
-        '''Use a filter to find a specific single record, in this case, the third sample by name'''
+        """Use a filter to find a specific single record, in this case, the third sample by name"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         result = MMUD.find_one( { 'name' : sampleData[2]['name'] } )
 
         # verify that we found the right record
         assert result['name'] == sampleData[2]['name']
 
 
     def test_find_one_projection_1( self, getPopulatedMMUDClass ):
-        '''Test find() with a "positive" projection'''
+        """Test find() with a "positive" projection"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
@@ -912,15 +912,15 @@
         assert '_updated' not in result
         assert 'amount' in result
         assert 'name' not in result
         assert result.readonly is True
 
 
     def test_find_one_projection_2( self, getPopulatedMMUDClass ):
-        '''Test find() with a "positive" projection but suppress _id'''
+        """Test find() with a "positive" projection but suppress _id"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
@@ -930,15 +930,15 @@
         assert '_updated' not in result
         assert 'amount' not in result
         assert 'name' in result
         assert result.readonly is True
 
 
     def test_find_one_projection_3( self, getPopulatedMMUDClass ):
-        '''Test find() with a "negative" projection'''
+        """Test find() with a "negative" projection"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
@@ -948,15 +948,15 @@
         assert '_updated' in result
         assert 'amount' not in result
         assert 'name' in result
         assert result.readonly is True
 
 
     def test_find_one_projection_4( self, getPopulatedMMUDClass ):
-        '''Test find() with a "negative" projection and suppress _id'''
+        """Test find() with a "negative" projection and suppress _id"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
@@ -966,15 +966,15 @@
         assert '_updated' in result
         assert 'amount' in result
         assert 'name' not in result
         assert result.readonly is True
 
 
     def test_find_one_projection_5( self, getPopulatedMMUDClass ):
-        '''Test find() with a "negative" projection with readonly forced to False'''
+        """Test find() with a "negative" projection with readonly forced to False"""
         MMUD = getPopulatedMMUDClass
 
         # verify that this is an unversioned test
         assert MMUD.object_version is None
 
         # Verify projection produced the proper key set
         # Also confirm object is not marked readonly
@@ -992,27 +992,27 @@
         result = MMUD.find_one( readonly=True )
 
         # verify object are marked readonly
         result.readonly is True
 
 
     def test_find_one_no_pre_auth( self, getPopulatedMMUDClass ):
-        '''Test attempting to read without pre-authorization'''
+        """Test attempting to read without pre-authorization"""
         class LocalMMUD( getPopulatedMMUDClass ):
             @classmethod
             def authorize_pre_read( cls ):
                 return False
 
         # verify reading a document without pre-read authorization produces an exception
         with pytest.raises( mongo_objects.MongoObjectsAuthFailed ):
             LocalMMUD.find_one()
 
 
     def test_find_one_no_auth( self, getPopulatedMMUDClass ):
-        '''Test attempting to read without authorization'''
+        """Test attempting to read without authorization"""
         class LocalMMUD( getPopulatedMMUDClass):
             def authorize_read( self ):
                 return False
 
         # verify reading documents without read authorization produces an empty list
         result = LocalMMUD.find_one()
         assert result is None
@@ -1195,44 +1195,23 @@
         # verify the objects are the same
         assert source == result
 
         # verify the object is readonly
         assert result.readonly is True
 
 
-    def test_load_proxy_by_id( self, getPopulatedMMUDClass ):
+    def test_load_by_id_invalid( self, getPopulatedMMUDClass ):
         MMUD = getPopulatedMMUDClass
 
-        # load a random object
-        source = MMUD.find_one()
-
-        # load the same object with an empty proxy tree
-        result = MMUD.load_proxy_by_id( source.id() )
-
-        # verify the objects are the same
-        assert source == result
-
-        # verify the object is readonly
-        assert result.readonly is False
-
+        # verify that loading an invalid object returns None
+        assert MMUD.load_by_id( 'ZYX' ) is None
 
-    def test_load_proxy_by_id_readonly( self, getPopulatedMMUDClass ):
-        MMUD = getPopulatedMMUDClass
-
-        # load a random object
-        source = MMUD.find_one()
-
-        # load the same object with an empty proxy tree
-        result = MMUD.load_proxy_by_id( source.id(), readonly=True )
 
-        # verify the objects are the same
-        assert source == result
-
-        # verify the object is readonly
-        assert result.readonly is True
+# Test load_proxy_by_id() and load_proxy_by_local_id() in the
+# proxy tests as proxy classes are required
 
 
     def test_split_id( self, getMMUDClass ):
         MMUD = getMMUDClass
 
         # verify that the subdocument key separator exists
         assert hasattr( MMUD, 'subdoc_key_sep' )
@@ -1243,17 +1222,17 @@
 
         # split the ID back into components
         assert MMUD.split_id( id ) == a
 
 
     def test_utcnow( self, getMMUDClass ):
         MMUD = getMMUDClass
-        startTime = datetime.utcnow()
+        startTime = datetime.datetime.now( datetime.UTC ).replace( tzinfo=None )
         mongoNow = MMUD.utcnow()
-        endTime = datetime.utcnow()
+        endTime = datetime.datetime.now( datetime.UTC ).replace( tzinfo=None )
 
         # verify that mongoNow has no microseconds
         assert mongoNow.microsecond % 1000 == 0
 
         # disregarding microseconds, verify mongoNow >= startTime
         assert mongoNow.replace(microsecond=0) >= startTime.replace(microsecond=0)
```

### Comparing `mongo_objects-1.1.2/tests/test_PolymorphicMongoListProxy.py` & `mongo_objects-1.2.0/tests/test_PolymorphicMongoListProxy.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import pytest
 import secrets
 
 
 
 @pytest.fixture( scope='class' )
 def getMPMUDClasses( mongo_db ):
-    '''Return a set of polymorphic MongoUserDict classes configured for a per-test-class unique collection'''
+    """Return a set of polymorphic MongoUserDict classes configured for a per-test-class unique collection"""
 
     class MyMongoUserDict( mongo_objects.MongoUserDict ):
         collection_name = secrets.token_hex(6)
         database = mongo_db
 
     class MyMongoListProxyA( mongo_objects.PolymorphicMongoListProxy ):
         container_name = 'proxyA'
@@ -57,15 +57,15 @@
         proxy_subclass_key = 'Bb'
 
     class MyMongoListProxyBc( MyMongoListProxyB ):
         proxy_subclass_key = 'Bc'
 
 
     return {
-        'base' : MyMongoUserDict,
+        'parent_doc' : MyMongoUserDict,
         'A' : MyMongoListProxyA,
         'Aa' : MyMongoListProxyAa,
         'Ab' : MyMongoListProxyAb,
         'Ac' : MyMongoListProxyAc,
         'A1' : MyMongoListProxyA1,
         'A1a' : MyMongoListProxyA1a,
         'A1b' : MyMongoListProxyA1b,
@@ -82,15 +82,15 @@
 def getPopulatedMPMUDClasses( getMPMUDClasses ):
 
     classes = getMPMUDClasses
     itemMax = 3     # make three of everything
 
     # make parent objects
     for i in range( itemMax ):
-        parent = classes['base']( {
+        parent = classes['parent_doc']( {
             'name' : f"Record {i}",
             'amount' : i * 10,
         } )
 
         # make "A" proxies include a base-class proxy
         for keyA in ('A', 'Aa', 'Ab', 'Ac'):
             proxyA = classes[keyA].create( parent, {
@@ -119,15 +119,15 @@
     return classes
 
 
 @pytest.fixture( scope='class' )
 def getSampleParent( getPopulatedMPMUDClasses ):
     classes = getPopulatedMPMUDClasses
     # find a random entry of the base class
-    return classes['base'].find_one()
+    return classes['parent_doc'].find_one()
 
 
 @pytest.fixture( scope='class' )
 def getSampleProxyA( getPopulatedMPMUDClasses, getSampleParent ):
     classes = getPopulatedMPMUDClasses
     # return the first proxyA in the list
     return classes['A'].get_proxies( getSampleParent )[0]
@@ -138,39 +138,40 @@
     classes = getPopulatedMPMUDClasses
     # return the first proxyA1 in the list
     return classes['A1'].get_proxies( getSampleProxyA )[0]
 
 
 
 class TestInitSubclass:
-    '''Test __init_subclass__ permutations'''
+    """Test __init_subclass__ permutations"""
 
     def test_init_subclass( self ):
         class MyTestClassBase( mongo_objects.PolymorphicMongoListProxy ):
             # create our own local testing namespace
             proxy_subclass_map = {}
 
         class MyTestSubclassA( MyTestClassBase ):
             proxy_subclass_key = 'A'
 
         class MyTestSubclassB( MyTestClassBase ):
             proxy_subclass_key = 'B'
 
         class MyTestSubclassC( MyTestClassBase ):
-            pass
+            proxy_subclass_key = 'C'
 
-        # Verify that classes A and B were added to the map
-        # Class C should be skipped because it doesn't have a non-None subclass_key
+        # Verify that all classes were added to the map
         assert MyTestClassBase.proxy_subclass_map == {
+            None : MyTestClassBase,
             'A' : MyTestSubclassA,
-            'B' : MyTestSubclassB
+            'B' : MyTestSubclassB,
+            'C' : MyTestSubclassC
         }
 
         # verify our local subclass map namespace didn't affect the module base class map
-        assert len( mongo_objects.PolymorphicMongoBaseProxy.proxy_subclass_map ) == 0
+        assert len( mongo_objects.PolymorphicMongoListProxy.proxy_subclass_map ) == 0
 
 
     def test_init_subclass_duplicate_key( self ):
         with pytest.raises( mongo_objects.MongoObjectsSubclassError ):
 
             class MyTestClassBase( mongo_objects.PolymorphicMongoListProxy ):
                 # create our own local testing namespace
@@ -188,15 +189,15 @@
 class TestCreate:
     def test_create( self, getPopulatedMPMUDClasses, getSampleProxyA ):
         classes = getPopulatedMPMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         count = len( proxyA.get_subdoc_container() )
 
         # create a base class proxy object
         newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'} )
 
         # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
@@ -222,15 +223,15 @@
 
     def test_create_no_save( self, getPopulatedMPMUDClasses, getSampleProxyA ):
         classes = getPopulatedMPMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         count = len( proxyA.get_subdoc_container() )
 
         # create a base class proxy object
         newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'}, autosave=False )
 
         # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
@@ -257,15 +258,15 @@
     def test_create_A1( self, getPopulatedMPMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMPMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
         parent = proxyA1.ultimate_parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         countA = len( proxyA.get_subdoc_container() )
         countA1 = len( proxyA1.get_subdoc_container() )
 
         # create a base class second-level proxy object
         newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'} )
 
         # Since the base class does not define a proxy_subclass_key, verify none was added to the record
@@ -290,15 +291,15 @@
     def test_create_A1_no_save( self, getPopulatedMPMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMPMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
         parent = proxyA1.ultimate_parent
 
         # record current state
-        original = dict( parent )
+        original = parent.copy()
         countA = len( proxyA.get_subdoc_container() )
         countA1 = len( proxyA1.get_subdoc_container() )
 
         # create a base class second-level proxy object
         newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'}, autosave=False )
 
         # Since the base class does not define a proxy_subclass_key, verify none was added to the record
@@ -319,29 +320,28 @@
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 
 class TestPolymorphicBasics:
     def test_subclass_map( self , getPopulatedMPMUDClasses ):
-        '''getMPMUDClasses create a new proxy_subclass_map namespace for each proxy base class
+        """getMPMUDClasses create a new proxy_subclass_map namespace for each proxy base class
         Verify the keys in the proxy_subclass map
-        Verify the base class proxy_subclass map is empty'''
+        Verify the base class proxy_subclass map is empty"""
         classes = getPopulatedMPMUDClasses
         assert len( mongo_objects.PolymorphicMongoListProxy.proxy_subclass_map ) == 0
-        assert sorted( classes['A'].proxy_subclass_map ) == ['Aa', 'Ab', 'Ac']
-        assert sorted( classes['A1'].proxy_subclass_map ) == ['A1a', 'A1b', 'A1c']
-        assert sorted( classes['B'].proxy_subclass_map ) == ['Ba', 'Bb', 'Bc']
+        assert len( set( classes['A'].proxy_subclass_map ).difference( [None, 'Aa', 'Ab', 'Ac'] ) ) == 0
+        assert len( set( classes['A1'].proxy_subclass_map ).difference( [None, 'A1a', 'A1b', 'A1c'] ) ) == 0
+        assert len( set( classes['B'].proxy_subclass_map ).difference( [None, 'Ba', 'Bb', 'Bc'] ) ) == 0
 
 
     def test_get_proxy( self, getPopulatedMPMUDClasses, getSampleParent ):
-        '''Test accessing both first-level and second-level proxies
-
-        For testing convenience, the keys of the getPopulatedMPMUDClasses dictionary
-        match the proxy_subclass_key for each subclass'''
+        """
+        Test accessing both first-level and second-level proxies
+        """
         classes = getPopulatedMPMUDClasses
         parent = getSampleParent
 
         # loop through keys in the proxy A container
         for keyA in [ entry['_sdkey'] for entry in parent[ classes['A'].container_name ] ]:
 
             # create a first-level proxy object
@@ -369,18 +369,17 @@
                 if '_psckey' not in proxyA1:
                     assert isinstance( proxyA1, classes['A1'] )
                 else:
                     assert isinstance( proxyA1, classes[ proxyA1['_psckey'] ] )
 
 
     def test_get_proxy_by_sequence( self, getPopulatedMPMUDClasses, getSampleParent ):
-        '''Test accessing both first-level and second-level proxies
-
-        For testing convenience, the keys of the getPopulatedMPMUDClasses dictionary
-        match the proxy_subclass_key for each subclass'''
+        """
+        Test accessing both first-level and second-level proxies
+        """
         classes = getPopulatedMPMUDClasses
         parent = getSampleParent
 
         # loop through keys in the proxy A container
         for seqA in range( len( parent[ classes['A'].container_name ] ) ):
 
             # create a first-level proxy object
@@ -407,17 +406,192 @@
                 # the base class object won't have _psckey
                 if '_psckey' not in proxyA1:
                     assert isinstance( proxyA1, classes['A1'] )
                 else:
                     assert isinstance( proxyA1, classes[ proxyA1['_psckey'] ] )
 
 
+    def test_get_proxy_subclass( self, getPopulatedMPMUDClasses, getSampleParent ):
+        """
+        Test accessing both first-level and second-level proxies with subclasses
+        """
+        classes = getPopulatedMPMUDClasses
+        parent = getSampleParent
+
+        # loop through keys in the proxy A container
+        for itemA in parent[ classes['A'].container_name ]:
+            keyA = itemA['_sdkey']
+
+            # create a first-level proxy object
+            # This should always work
+            proxyA = classes['A'].get_proxy( parent, keyA )
+
+            # loop through the subclasses
+            for subclass in ('Aa', 'Ab', 'Ac'):
+                # we should also be able to locate the proxy with its subclass
+                if proxyA.get('_psckey') == subclass:
+                    proxyA_by_subclass = classes[subclass].get_proxy( parent, keyA )
+                    assert id( proxyA.data() ) == id( proxyA_by_subclass.data() )
+
+                # creating a proxy with the wrong class raises an exception
+                else:
+                    with pytest.raises( mongo_objects.MongoObjectsPolymorphicMismatch ):
+                        proxyA_by_subclass = classes[subclass].get_proxy( parent, keyA )
+                        proxyA_by_subclass.keys()
+
+                # loop through the keys of the second level proxy A1 container
+                for itemA1 in proxyA[ classes['A1'].container_name ]:
+                    keyA1 = itemA1['_sdkey']
+
+                    # create a second-level proxy object
+                    # This should always work
+                    proxyA1 = classes['A1'].get_proxy( proxyA, keyA1 )
+
+                    # loop through the subclasses
+                    for subclassA1 in ('A1a', 'A1b', 'A1c'):
+                        # we should also be able to locate the proxy with its subclass
+                        if proxyA1.get('_psckey') == subclassA1:
+                            proxyA1_by_subclass = classes[subclassA1].get_proxy( proxyA, keyA1 )
+                            assert id( proxyA1.data() ) == id( proxyA1_by_subclass.data() )
+
+                        # creating a proxy with the wrong class raises an exception
+                        else:
+                            with pytest.raises( mongo_objects.MongoObjectsPolymorphicMismatch ):
+                                proxyA1_by_subclass = classes[subclassA1].get_proxy( proxyA, keyA1 )
+                                proxyA1_by_subclass.keys()
+
+
+    def test_get_proxies( self, getPopulatedMPMUDClasses, getSampleParent ):
+        """
+        Test accessing both first-level and second-level proxies with subclasses
+        """
+        classes = getPopulatedMPMUDClasses
+        parent = getSampleParent
+
+        # collect all first-level proxies from the base class
+        proxiesA = list( classes['A'].get_proxies( parent ) )
+
+        # verify all proxies were found
+        assert len( proxiesA ) == 4
+
+        # verify proper subclass was returned
+        for proxyA in proxiesA:
+            assert isinstance( proxyA, classes[ proxyA.get('_psckey', 'A') ] )
+
+            # collect all second-level proxies from the base class
+            proxiesA1 = list( classes['A1'].get_proxies( proxyA ) )
+
+            # verify all proxies were found
+            assert len( proxiesA1 ) == 4
+
+            # verify proper subclass was returned
+            for proxyA1 in proxiesA1:
+                assert isinstance( proxyA1, classes[ proxyA1.get('_psckey', 'A1') ] )
+
+
+    def test_get_proxies_subclass( self, getPopulatedMPMUDClasses, getSampleParent ):
+        """
+        Test accessing both first-level and second-level proxies with subclasses
+        """
+        classes = getPopulatedMPMUDClasses
+        parent = getSampleParent
+
+        # loop through the first-level subclasses
+        for subclass in ('Aa', 'Ab', 'Ac'):
+            # collect the proxies from this subclass
+            proxiesA = list( classes[subclass].get_proxies( parent ) )
+
+            # only one proxy should be found
+            assert len( proxiesA ) == 1
+
+            # verify proper subclass was returned
+            assert isinstance( proxiesA[0], classes[ subclass ] )
+            assert subclass == proxiesA[0].get('_psckey')
+
+            # loop through the second level subclasses
+            for subclassA1 in ('A1a', 'A1b', 'A1c'):
+                # collect the proxies from this subclass
+                proxiesA1 = list( classes[subclassA1].get_proxies( proxiesA[0] ) )
+
+                # only one proxy should be found
+                assert len( proxiesA1 ) == 1
+
+                # verify proper subclass was returned
+                assert isinstance( proxiesA1[0], classes[ subclassA1 ] )
+                assert subclassA1 == proxiesA1[0].get('_psckey')
+
+
     def test_get_subclass_by_key( self, getMPMUDClasses ):
         classes = getMPMUDClasses
+
+        # Check the map from the base class
         assert classes['A'].get_subclass_by_key( 'Aa' ) == classes['Aa']
+        assert classes['A'].get_subclass_by_key( 'Ab' ) == classes['Ab']
+        assert classes['A'].get_subclass_by_key( 'Ac' ) == classes['Ac']
+
+        # In the default classes, the base doc class has None
+        # as a subclass key and so is the default for all unknown
+        # subclass keys
+        assert classes['A'].get_subclass_by_key( 'A' ) == classes['A']
+        assert classes['A'].get_subclass_by_key( 'Ad' ) == classes['A']
+
+
+    def test_get_subclass_by_key_from_subclass( self, getMPMUDClasses ):
+        classes = getMPMUDClasses
+
+        # Check the map from the base class
+        assert classes['Aa'].get_subclass_by_key( 'Aa' ) == classes['Aa']
+        assert classes['Aa'].get_subclass_by_key( 'Ab' ) == classes['Ab']
+        assert classes['Aa'].get_subclass_by_key( 'Ac' ) == classes['Ac']
+
+        # In the default classes, the base doc class has None
+        # as a subclass key and so is the default for all unknown
+        # subclass keys
+        assert classes['Aa'].get_subclass_by_key( 'A' ) == classes['A']
+        assert classes['Aa'].get_subclass_by_key( 'Ad' ) == classes['A']
+
+
+    def test_get_subclass_by_key_no_default( self ):
+        '''Test get_subclass_by_key with a different class structure
+        where the base class has its own proxy_subclass_key and thus
+        there is no default class.'''
+        class LocalMongoListProxyA( mongo_objects.PolymorphicMongoListProxy ):
+            container_name = 'proxyA'
+            proxy_subclass_map = {}
+            proxy_subclass_key = 'A'
+
+        class LocalMongoListProxyAa( LocalMongoListProxyA ):
+            proxy_subclass_key = 'Aa'
+
+        class LocalMongoListProxyAb( LocalMongoListProxyA ):
+            proxy_subclass_key = 'Ab'
+
+        class LocalMongoListProxyAc( LocalMongoListProxyA ):
+            proxy_subclass_key = 'Ac'
+
+        assert LocalMongoListProxyA.get_subclass_by_key( 'A' ) == LocalMongoListProxyA
+        assert LocalMongoListProxyA.get_subclass_by_key( 'Aa' ) == LocalMongoListProxyAa
+        assert LocalMongoListProxyA.get_subclass_by_key( 'Ab' ) == LocalMongoListProxyAb
+        assert LocalMongoListProxyA.get_subclass_by_key( 'Ac' ) == LocalMongoListProxyAc
+
+        # There is no default class (no class with a None subclass_key)
+        # so unknown subclass keys will raise an exception
+        with pytest.raises( mongo_objects.MongoObjectsPolymorphicMismatch ):
+            LocalMongoListProxyA.get_subclass_by_key( 'Ad' )
+
+        # Also check the return from a subclass
+        assert LocalMongoListProxyAa.get_subclass_by_key( 'A' ) == LocalMongoListProxyA
+        assert LocalMongoListProxyAa.get_subclass_by_key( 'Aa' ) == LocalMongoListProxyAa
+        assert LocalMongoListProxyAa.get_subclass_by_key( 'Ab' ) == LocalMongoListProxyAb
+        assert LocalMongoListProxyAa.get_subclass_by_key( 'Ac' ) == LocalMongoListProxyAc
+
+        # There is no default class (no class with a None subclass_key)
+        # so unknown subclass keys will raise an exception
+        with pytest.raises( mongo_objects.MongoObjectsPolymorphicMismatch ):
+            LocalMongoListProxyAa.get_subclass_by_key( 'Ad' )
 
 
     def test_get_subclass_from_doc( self, getMPMUDClasses ):
         classes = getMPMUDClasses
         assert classes['A'].get_subclass_by_key( 'Aa' ) == classes['Aa']
         assert classes['A'].get_subclass_from_doc( { classes['A'].proxy_subclass_key_name : 'Aa' } ) == classes['Aa']
```

### Comparing `mongo_objects-1.1.2/tests/test_PolymorphicMongoSingleProxy.py` & `mongo_objects-1.2.0/tests/test_PolymorphicMongoSingleProxy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,72 @@
 # test_PolymorphicMongoSingleProxy
 #
 # Since MongoSingleProxy has been thoroughly exercised elsewhere,
 # only test functionality unique to PolymorphicMongoSingleProxy
 
 from bson import ObjectId
+import copy
 from datetime import datetime
 import mongo_objects
 from pymongo.collection import Collection
 import pytest
 import secrets
 
 
 
 @pytest.fixture( scope='class' )
 def getMPMUDClasses( mongo_db ):
-    '''Return a set of polymorphic MongoUserDict classes configured for a per-test-class unique collection
-
-    Since each class is only used once per object, we can predefine the container_name'''
+    """Return a set of polymorphic MongoUserDict classes configured for a per-test-class unique collection"""
 
     class MyMongoUserDict( mongo_objects.MongoUserDict ):
         collection_name = secrets.token_hex(6)
         database = mongo_db
 
     class MyMongoSingleProxyA( mongo_objects.PolymorphicMongoSingleProxy ):
         proxy_subclass_map = {}
-        container_name = "proxyA-0"
+        container_name = "proxyA"
 
     class MyMongoSingleProxyAa( MyMongoSingleProxyA ):
         proxy_subclass_key = 'Aa'
-        container_name = "proxyA-1"
 
     class MyMongoSingleProxyAb( MyMongoSingleProxyA ):
         proxy_subclass_key = 'Ab'
-        container_name = "proxyA-2"
 
     class MyMongoSingleProxyAc( MyMongoSingleProxyA ):
         proxy_subclass_key = 'Ac'
-        container_name = "proxyA-3"
 
     class MyMongoSingleProxyA1( mongo_objects.PolymorphicMongoSingleProxy ):
         proxy_subclass_map = {}
-        container_name = "proxyA1-0"
+        container_name = "proxyA1"
 
     class MyMongoSingleProxyA1a( MyMongoSingleProxyA1 ):
         proxy_subclass_key = 'A1a'
-        container_name = "proxyA1-1"
 
     class MyMongoSingleProxyA1b( MyMongoSingleProxyA1 ):
         proxy_subclass_key = 'A1b'
-        container_name = "proxyA1-2"
 
     class MyMongoSingleProxyA1c( MyMongoSingleProxyA1 ):
         proxy_subclass_key = 'A1c'
-        container_name = "proxyA1-3"
 
     class MyMongoSingleProxyB( mongo_objects.PolymorphicMongoSingleProxy ):
         proxy_subclass_map = {}
-        container_name = "proxyB-0"
+        container_name = "proxyB"
 
     class MyMongoSingleProxyBa( MyMongoSingleProxyB ):
         proxy_subclass_key = 'Ba'
-        container_name = "proxyB-1"
 
     class MyMongoSingleProxyBb( MyMongoSingleProxyB ):
         proxy_subclass_key = 'Bb'
-        container_name = "proxyB-2"
 
     class MyMongoSingleProxyBc( MyMongoSingleProxyB ):
         proxy_subclass_key = 'Bc'
-        container_name = "proxyB-3"
 
 
     return {
-        'base' : MyMongoUserDict,
+        'parent' : MyMongoUserDict,
         'A' : MyMongoSingleProxyA,
         'Aa' : MyMongoSingleProxyAa,
         'Ab' : MyMongoSingleProxyAb,
         'Ac' : MyMongoSingleProxyAc,
         'A1' : MyMongoSingleProxyA1,
         'A1a' : MyMongoSingleProxyA1a,
         'A1b' : MyMongoSingleProxyA1b,
@@ -87,132 +77,105 @@
         'Bc' : MyMongoSingleProxyBc,
     }
 
 
 
 @pytest.fixture( scope='class' )
 def getPopulatedMPMUDClasses( getMPMUDClasses ):
+    '''Make four objects, one with the base classes and one for
+    each of the *a, *b and *c subclasses.'''
 
     classes = getMPMUDClasses
-    itemMax = 3     # make three of everything
-
-    # make parent objects
-    for i in range( itemMax ):
-        parent = classes['base']( {
-            'name' : f"Record {i}",
-            'amount' : i * 10,
-        } )
-
-        # make "A" proxies include a base-class proxy
-        for (j, keyA) in enumerate( ['A', 'Aa', 'Ab', 'Ac'] ):
-            proxyA = classes[keyA].create(
-                parent,
-                {
-                    'nameA' : f"Proxy A-{j}",
-                    'amountA' : j * 100,
-                },
-            )
-
-            # make second-level A1 proxies
-            for (k, keyA1) in enumerate( ['A1', 'A1a', 'A1b', 'A1c'] ):
-                proxyA1 = classes[keyA1].create(
-                    proxyA,
-                    {
-                        'nameA1' : f"Proxy A1-{k}",
-                        'amountA1' : k * 1000,
-                    },
-                )
-
-        # make "B" proxies
-        for (j, keyB) in enumerate( ['B', 'Ba', 'Bb', 'Bc'] ):
-            proxyB = classes[keyB].create(
-                parent,
-                {
-                    'nameB' : f"Proxy B-{j}",
-                    'amountB' : j * 100 + 1,
-                },
-            )
-
 
+    # one document with just base classes
+    for (seq, A, A1, B) in [
+        (0, 'A',  'A1',  'B'  ),
+        (1, 'Aa', 'A1a', 'Ba' ),
+        (2, 'Ab', 'A1b', 'Bb' ),
+        (3, 'Ac', 'A1c', 'Bc' ),
+    ]:
+        parent = classes['parent']( {
+            'name' : f"Parent Document {seq}",
+            'amount' : 10,
+            }
+        )
+        proxyA = classes[A].create(
+            parent,
+            {
+                'nameA' : f"Proxy A-{seq}",
+                'amountA' : 100 + seq,
+            },
+        )
+        proxyA1 = classes[A1].create(
+            proxyA,
+            {
+                'nameA1' : f"Proxy A1-{seq}",
+                'amountA1' : 1000 + seq,
+            },
+        )
+        proxyB = classes['B'].create(
+            parent,
+            {
+                'nameB' : f"Proxy B-{seq}",
+                'amountB' : 200 + seq,
+            },
+        )
         # save data
         parent.save()
 
     return classes
 
 
 @pytest.fixture( scope='class' )
 def getSampleParent( getPopulatedMPMUDClasses ):
     classes = getPopulatedMPMUDClasses
-    # find a random entry of the base class
-    return classes['base'].find_one()
-
-
-@pytest.fixture( scope='class' )
-def getSampleProxyAKey():
-    '''Return a fixed sample key for first-level A proxy testing'''
-    return 'proxyA-0'
-
-
-@pytest.fixture( scope='class' )
-def getSampleProxyAKeys():
-    '''Return a fixed sample keys for first-level A proxy testing'''
-    return [ 'proxyA-0', 'proxyA-1', 'proxyA-2' ]
+    # find a random entry of the parent class
+    return classes['parent'].find_one()
 
 
 @pytest.fixture( scope='class' )
-def getSampleProxyA( getPopulatedMPMUDClasses, getSampleParent, getSampleProxyAKey ):
+def getSampleProxyA( getPopulatedMPMUDClasses, getSampleParent ):
     classes = getPopulatedMPMUDClasses
-    return classes['A'].get_proxy( getSampleParent, getSampleProxyAKey )
-
-
-@pytest.fixture( scope='class' )
-def getSampleProxyA1Key():
-    '''Return a fixed sample key for second-level A1 proxy testing'''
-    return 'proxyA1-0'
+    return classes['A'].get_proxy( getSampleParent )
 
 
 @pytest.fixture( scope='class' )
-def getSampleProxyA1Keys():
-    '''Return a fixed sample keys for first-level A proxy testing'''
-    return [ 'proxyA1-0', 'proxyA1-1', 'proxyA1-2' ]
-
-
-@pytest.fixture( scope='class' )
-def getSampleProxyA1( getPopulatedMPMUDClasses, getSampleProxyA, getSampleProxyA1Key ):
+def getSampleProxyA1( getPopulatedMPMUDClasses, getSampleProxyA ):
     classes = getPopulatedMPMUDClasses
-    return classes['A1'].get_proxy( getSampleProxyA, getSampleProxyA1Key )
+    return classes['A1'].get_proxy( getSampleProxyA )
 
 
 
 class TestInitSubclass:
-    '''Test __init_subclass__ permutations'''
+    """Test __init_subclass__ permutations"""
 
     def test_init_subclass( self ):
         class MyTestClassBase( mongo_objects.PolymorphicMongoSingleProxy ):
             # create our own local testing namespace
             proxy_subclass_map = {}
 
         class MyTestSubclassA( MyTestClassBase ):
             proxy_subclass_key = 'A'
 
         class MyTestSubclassB( MyTestClassBase ):
             proxy_subclass_key = 'B'
 
         class MyTestSubclassC( MyTestClassBase ):
-            pass
+            proxy_subclass_key = 'C'
 
-        # Verify that classes A and B were added to the map
-        # Class C should be skipped because it doesn't have a non-None subclass_key
+        # Verify that all classes were added to the map
         assert MyTestClassBase.proxy_subclass_map == {
+            None : MyTestClassBase,
             'A' : MyTestSubclassA,
-            'B' : MyTestSubclassB
+            'B' : MyTestSubclassB,
+            'C' : MyTestSubclassC
         }
 
         # verify our local subclass map namespace didn't affect the module base class map
-        assert len( mongo_objects.PolymorphicMongoBaseProxy.proxy_subclass_map ) == 0
+        assert len( mongo_objects.PolymorphicMongoSingleProxy.proxy_subclass_map ) == 0
 
 
     def test_init_subclass_duplicate_key( self ):
         with pytest.raises( mongo_objects.MongoObjectsSubclassError ):
 
             class MyTestClassBase( mongo_objects.PolymorphicMongoSingleProxy ):
                 # create our own local testing namespace
@@ -224,230 +187,362 @@
             class MyTestSubclassAnotherA( MyTestClassBase ):
                 proxy_subclass_key = 'A'
 
 
 
 
 class TestCreate:
-    def test_create( self, getPopulatedMPMUDClasses, getSampleProxyA ):
-        classes = getPopulatedMPMUDClasses
-        proxyA = getSampleProxyA
-        parent = proxyA.parent
+    def test_create( self, getMPMUDClasses ):
+        classes = getMPMUDClasses
+
+        # create an empty parent document
+        parent = classes['parent']( {} )
+        parent.save()
 
         # record current state
-        original = dict( parent )
-        count = len( proxyA.get_subdoc_container().keys() )
+        original = copy.deepcopy( parent.data )
 
         # create a base class proxy object
-        # Override the container name since there is already a proxyA at the default location
-        newProxy = classes['A'].create( 
+        newProxy = classes['A'].create(
             parent,
             { 'name' : 'new proxyA entry'},
-            key='newProxyA'
         )
 
         # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
         assert isinstance( newProxy, classes['A'] )
 
-        # Now create new subclass objects
+        # Now create new subclass objects; these will overwrite each other
         for key in ('Aa', 'Ab', 'Ac'):
             newProxy = classes[key].create(
                 parent,
-                { 'name' : f"new proxy{key} entry" },
-                key=f"newProxy{key}" )
+                { 'name' : f"new proxy{key} entry" }
+            )
             assert newProxy['_psckey'] == key
             assert isinstance( newProxy, classes[key] )
 
-        # verify four new entries created
-        assert len( proxyA.get_subdoc_container().keys() ) == count+4
+        # verify one new subdoc created
+        assert len( parent.keys() ) == len( original.keys() ) + 1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
 class TestCreateNoSave:
-    def test_create_no_save( self, getPopulatedMPMUDClasses, getSampleProxyA ):
-        classes = getPopulatedMPMUDClasses
-        proxyA = getSampleProxyA
-        parent = proxyA.parent
+    def test_create_no_save( self, getMPMUDClasses ):
+        classes = getMPMUDClasses
+
+        # create an empty parent document
+        parent = classes['parent']( {} )
+        parent.save()
 
         # record current state
-        original = dict( parent )
-        count = len( proxyA.get_subdoc_container().keys() )
+        original = copy.deepcopy( parent.data )
 
         # create a base class proxy object
         newProxy = classes['A'].create( 
             parent,
             { 'name' : 'new proxyA entry'},
-            key='newProxyA',
             autosave=False
         )
 
         # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
         assert isinstance( newProxy, classes['A'] )
 
-        # Now create new subclass objects
+        # Now create new subclass objects; these will overwrite each other
         for key in ('Aa', 'Ab', 'Ac'):
             newProxy = classes[key].create(
                 parent,
                 { 'name' : f"new proxy{key} entry" },
-                key=f"newProxy{key}",
                 autosave=False
             )
             assert newProxy['_psckey'] == key
             assert isinstance( newProxy, classes[key] )
 
-        # verify four new entries created
-        assert len( proxyA.get_subdoc_container().keys() ) == count+4
+        # verify one new subdoc created
+        assert len( parent.keys() ) == len( original.keys() ) + 1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 class TestCreateA1:
-    def test_create_A1( self, getPopulatedMPMUDClasses, getSampleProxyA1 ):
-        classes = getPopulatedMPMUDClasses
-        proxyA1 = getSampleProxyA1
-        proxyA = proxyA1.parent
-        parent = proxyA1.ultimate_parent
+    def test_create_A1( self, getMPMUDClasses ):
+        classes = getMPMUDClasses
+
+        # create an empty parent document
+        parent = classes['parent']( {} )
+        proxyA = classes['A'].create( parent, {} )
+        parent.save()
 
         # record current state
-        original = dict( parent )
-        countA = len( proxyA.get_subdoc_container().keys() )
-        countA1 = len( proxyA1.get_subdoc_container().keys() )
+        original = copy.deepcopy( parent.data )
 
         # create a base class second-level proxy object
         newProxy = classes['A1'].create(
             proxyA,
             { 'name' : 'new proxyA1 entry'},
-            key='newProxyA1'
         )
 
         # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
         assert isinstance( newProxy, classes['A1'] )
 
         # Now create new second-level subclass objects
         for key in ('A1a', 'A1b', 'A1c'):
             newProxy = classes[key].create(
                 proxyA,
                 { 'name' : f"new proxy{key} entry" },
-                key=f"newProxy{key}",
             )
             assert newProxy['_psckey'] == key
             assert isinstance( newProxy, classes[key] )
 
-        # verify four new entries created at the second level
-        assert len( proxyA.get_subdoc_container().keys() ) == countA
-        assert len( proxyA1.get_subdoc_container().keys() ) == countA1+4
+        # verify one new subdoc created at the second level
+        assert len( parent.keys() ) == len( original.keys() )
+        assert len( proxyA.keys() ) == len( original[ classes['A'].container_name ].keys() ) + 1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
 class TestCreateA1NoSave:
-    def test_create_A1_no_save( self, getPopulatedMPMUDClasses, getSampleProxyA1 ):
-        classes = getPopulatedMPMUDClasses
-        proxyA1 = getSampleProxyA1
-        proxyA = proxyA1.parent
-        parent = proxyA1.ultimate_parent
+    def test_create_A1_no_save( self, getMPMUDClasses ):
+        classes = getMPMUDClasses
+
+        # create an empty parent document
+        parent = classes['parent']( {} )
+        proxyA = classes['A'].create( parent, {} )
+        parent.save()
 
         # record current state
-        original = dict( parent )
-        countA = len( proxyA.get_subdoc_container().keys() )
-        countA1 = len( proxyA1.get_subdoc_container().keys() )
+        original = copy.deepcopy( parent.data )
 
         # create a base class second-level proxy object
         newProxy = classes['A1'].create(
             proxyA,
             { 'name' : 'new proxyA1 entry'},
-            key='newProxyA',
             autosave=False
         )
 
         # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
         assert isinstance( newProxy, classes['A1'] )
 
         # Now create new second-level subclass objects
         for key in ('A1a', 'A1b', 'A1c'):
             newProxy = classes[key].create(
                 proxyA,
                 { 'name' : f"new proxy{key} entry" },
-                key=f"newProxy{key}",
                 autosave=False
             )
             assert newProxy['_psckey'] == key
             assert isinstance( newProxy, classes[key] )
 
-        # verify four new entries created at the second level
-        assert len( proxyA.get_subdoc_container().keys() ) == countA
-        assert len( proxyA1.get_subdoc_container().keys() ) == countA1+4
+        # verify one new subdoc created at the second level
+        assert len( parent.keys() ) == len( original.keys() )
+        assert len( proxyA.keys() ) == len( original[ classes['A'].container_name ].keys() ) + 1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 
 class TestPolymorphicBasics:
     def test_subclass_map( self , getPopulatedMPMUDClasses ):
-        '''getMPMUDClasses create a new proxy_subclass_map namespace for each proxy base class
+        """getMPMUDClasses create a new proxy_subclass_map namespace for each proxy base class
         Verify the keys in the proxy_subclass map
-        Verify the base class proxy_subclass map is empty'''
+        Verify the base class proxy_subclass map is empty"""
         classes = getPopulatedMPMUDClasses
         assert len( mongo_objects.PolymorphicMongoSingleProxy.proxy_subclass_map ) == 0
-        assert sorted( classes['A'].proxy_subclass_map ) == ['Aa', 'Ab', 'Ac']
-        assert sorted( classes['A1'].proxy_subclass_map ) == ['A1a', 'A1b', 'A1c']
-        assert sorted( classes['B'].proxy_subclass_map ) == ['Ba', 'Bb', 'Bc']
-
+        assert len( set( classes['A'].proxy_subclass_map ).difference( [None, 'Aa', 'Ab', 'Ac'] ) ) == 0
+        assert len( set( classes['A1'].proxy_subclass_map ).difference( [None, 'A1a', 'A1b', 'A1c'] ) ) == 0
+        assert len( set( classes['B'].proxy_subclass_map ).difference( [None, 'Ba', 'Bb', 'Bc'] ) ) == 0
 
-    def test_get_proxy( self, getPopulatedMPMUDClasses, getSampleParent, getSampleProxyAKeys, getSampleProxyA1Keys ):
-        '''Test accessing both first-level and second-level proxies
 
-        For testing convenience, the keys of the getPopulatedMPMUDClasses dictionary
-        match the proxy_subclass_key for each subclass'''
+    def test_get_proxy( self, getPopulatedMPMUDClasses ):
+        """
+        Test accessing both first-level and second-level proxies
+        """
         classes = getPopulatedMPMUDClasses
-        parent = getSampleParent
-
-        # loop through keys in the proxy A container
-        for keyA in getSampleProxyAKeys:
 
-            # create a first-level proxy object
-            proxyA = classes['A'].get_proxy( parent, keyA )
+        # record how many documents we find and how many subclasses
+        docCount = 0
+        proxyAVariants = set()
+        proxyA1Variants = set()
+
+        # loop through all pre-populated objects as they contain different
+        # subclasses of the proxies
+        for parent in classes['parent'].find():
+            docCount += 1
+
+            # load the polymorphic proxyA
+            proxyA = classes['A'].get_proxy( parent )
+
+            # verify dictionary content; all subclasses use the same container name
+            assert id( proxyA.data() ) == id( parent[ classes['A'].container_name ] )
+
+            # verify polymorphic subclass key and add it to the list
+            assert proxyA.get( '_psckey' ) in (None, 'Aa', 'Ab', 'Ac')
+            proxyAVariants.add( proxyA.get('_psckey') )
 
-            # verify dictionary
-            assert id( proxyA.data() ) == id( parent[ keyA ] )
+            # verify instance type; all objects must be a instance of A or one of its subclasses
+            assert isinstance( proxyA, classes['A'] )
 
-            # the base class object won't have _psckey
-            if '_psckey' not in proxyA:
-                assert isinstance( proxyA, classes['A'] )
-            else:
+            # for subclasses, verify the exact class
+            if '_psckey' in proxyA:
                 assert isinstance( proxyA, classes[ proxyA['_psckey'] ] )
 
-            # loop through the keys of the second level proxy A1 container
-            for keyA1 in getSampleProxyA1Keys:
 
-                # create a second-level proxy object
-                proxyA1 = classes['A1'].get_proxy( proxyA, keyA1 )
+            # load the polymorphic proxyA1
+            proxyA1 = classes['A1'].get_proxy( proxyA )
+
+            # verify dictionary content; all subclasses use the same container name
+            assert id( proxyA1.data() ) == id( parent[ classes['A'].container_name ][ classes['A1'].container_name ] )
+
+            # verify polymorphic subclass key and add it to the list
+            assert proxyA1.get( '_psckey' ) in (None, 'A1a', 'A1b', 'A1c')
+            proxyA1Variants.add( proxyA1.get('_psckey') )
+
+            # verify instance type; all objects must be a instance of A1 or one of its subclasses
+            assert isinstance( proxyA1, classes['A1'] )
+
+            # for subclasses, verify the exact class
+            if '_psckey' in proxyA1:
+                assert isinstance( proxyA1, classes[ proxyA1['_psckey'] ] )
+
+        # the way the sample data is created, make sure we found as many
+        # polymorphic subclasses as documents themselves
+        assert docCount == len( proxyAVariants )
+        assert docCount == len( proxyA1Variants )
+
+
+    def test_get_proxy_subclass( self, getPopulatedMPMUDClasses ):
+        """
+        Test accessing both first-level and second-level proxies via sublcass
+        """
+        classes = getPopulatedMPMUDClasses
+
+        # loop through all pre-populated objects as they contain different
+        # subclasses of the proxies
+        for parent in classes['parent'].find():
+
+            # load the polymorphic proxyA
+            proxyA = classes['A'].get_proxy( parent )
+
+            # loop through the subclasses
+            for subclass in ('Aa', 'Ab', 'Ac'):
+                # we should also be able to locate the proxy with its subclass
+                if proxyA.get('_psckey') == subclass:
+                    proxyA_by_subclass = classes[subclass].get_proxy( parent )
+                    assert id( proxyA.data() ) == id( proxyA_by_subclass.data() )
 
-                # verify dictionary
-                assert id( proxyA1.data() ) == id( parent[ keyA ][ keyA1 ] )
+                # creating a proxy with the wrong class raises an exception
+                else:
+                    with pytest.raises( mongo_objects.MongoObjectsPolymorphicMismatch ):
+                        proxyA_by_subclass = classes[subclass].get_proxy( parent )
+                        proxyA_by_subclass.keys()
+
+
+            # load the polymorphic proxyA1
+            proxyA1 = classes['A1'].get_proxy( proxyA )
+
+            # loop through the subclasses
+            for subclassA1 in ('A1a', 'A1b', 'A1c'):
+                # we should also be able to locate the proxy with its subclass
+                if proxyA1.get('_psckey') == subclassA1:
+                    proxyA1_by_subclass = classes[subclassA1].get_proxy( proxyA )
+                    assert id( proxyA1.data() ) == id( proxyA1_by_subclass.data() )
 
-                # the base class object won't have _psckey
-                if '_psckey' not in proxyA1:
-                    assert isinstance( proxyA1, classes['A1'] )
+                # creating a proxy with the wrong class raises an exception
                 else:
-                    assert isinstance( proxyA1, classes[ proxyA1['_psckey'] ] )
+                    with pytest.raises( mongo_objects.MongoObjectsPolymorphicMismatch ):
+                        proxyA1_by_subclass = classes[subclassA1].get_proxy( proxyA )
+                        proxyA1_by_subclass.keys()
+
+
+    def test_get_proxies( self, getMPMUDClasses, getSampleParent ):
+        '''
+        Single proxies don't support get_proxes()
+        Verify an exception is raised
+        '''
+        classes = getMPMUDClasses
+        parent = getSampleParent
+        with pytest.raises( Exception ):
+            classes['A'].get_proxies( parent )
 
 
     def test_get_subclass_by_key( self, getMPMUDClasses ):
         classes = getMPMUDClasses
+
+        # Check the map from the base class
         assert classes['A'].get_subclass_by_key( 'Aa' ) == classes['Aa']
+        assert classes['A'].get_subclass_by_key( 'Ab' ) == classes['Ab']
+        assert classes['A'].get_subclass_by_key( 'Ac' ) == classes['Ac']
+
+        # In the default classes, the base doc class has None
+        # as a subclass key and so is the default for all unknown
+        # subclass keys
+        assert classes['A'].get_subclass_by_key( 'A' ) == classes['A']
+        assert classes['A'].get_subclass_by_key( 'Ad' ) == classes['A']
+
+
+    def test_get_subclass_by_key_from_subclass( self, getMPMUDClasses ):
+        classes = getMPMUDClasses
+
+        # Check the map from the base class
+        assert classes['Aa'].get_subclass_by_key( 'Aa' ) == classes['Aa']
+        assert classes['Aa'].get_subclass_by_key( 'Ab' ) == classes['Ab']
+        assert classes['Aa'].get_subclass_by_key( 'Ac' ) == classes['Ac']
+
+        # In the default classes, the base doc class has None
+        # as a subclass key and so is the default for all unknown
+        # subclass keys
+        assert classes['Aa'].get_subclass_by_key( 'A' ) == classes['A']
+        assert classes['Aa'].get_subclass_by_key( 'Ad' ) == classes['A']
+
+
+    def test_get_subclass_by_key_no_default( self ):
+        '''Test get_subclass_by_key with a different class structure
+        where the base class has its own proxy_subclass_key and thus
+        there is no default class.'''
+        class LocalMongoSingleProxyA( mongo_objects.PolymorphicMongoSingleProxy ):
+            container_name = 'proxyA'
+            proxy_subclass_map = {}
+            proxy_subclass_key = 'A'
+
+        class LocalMongoSingleProxyAa( LocalMongoSingleProxyA ):
+            proxy_subclass_key = 'Aa'
+
+        class LocalMongoSingleProxyAb( LocalMongoSingleProxyA ):
+            proxy_subclass_key = 'Ab'
+
+        class LocalMongoSingleProxyAc( LocalMongoSingleProxyA ):
+            proxy_subclass_key = 'Ac'
+
+        assert LocalMongoSingleProxyA.get_subclass_by_key( 'A' ) == LocalMongoSingleProxyA
+        assert LocalMongoSingleProxyA.get_subclass_by_key( 'Aa' ) == LocalMongoSingleProxyAa
+        assert LocalMongoSingleProxyA.get_subclass_by_key( 'Ab' ) == LocalMongoSingleProxyAb
+        assert LocalMongoSingleProxyA.get_subclass_by_key( 'Ac' ) == LocalMongoSingleProxyAc
+
+        # There is no default class (no class with a None subclass_key)
+        # so unknown subclass keys will raise an exception
+        with pytest.raises( mongo_objects.MongoObjectsPolymorphicMismatch ):
+            LocalMongoSingleProxyA.get_subclass_by_key( 'Ad' )
+
+        # Also check the return from a subclass
+        assert LocalMongoSingleProxyAa.get_subclass_by_key( 'A' ) == LocalMongoSingleProxyA
+        assert LocalMongoSingleProxyAa.get_subclass_by_key( 'Aa' ) == LocalMongoSingleProxyAa
+        assert LocalMongoSingleProxyAa.get_subclass_by_key( 'Ab' ) == LocalMongoSingleProxyAb
+        assert LocalMongoSingleProxyAa.get_subclass_by_key( 'Ac' ) == LocalMongoSingleProxyAc
+
+        # There is no default class (no class with a None subclass_key)
+        # so unknown subclass keys will raise an exception
+        with pytest.raises( mongo_objects.MongoObjectsPolymorphicMismatch ):
+            LocalMongoSingleProxyAa.get_subclass_by_key( 'Ad' )
 
 
     def test_get_subclass_from_doc( self, getMPMUDClasses ):
         classes = getMPMUDClasses
         assert classes['A'].get_subclass_by_key( 'Aa' ) == classes['Aa']
         assert classes['A'].get_subclass_from_doc( { classes['A'].proxy_subclass_key_name : 'Aa' } ) == classes['Aa']
```

### Comparing `mongo_objects-1.1.2/tests/test_proxy_combo.py` & `mongo_objects-1.2.0/tests/test_proxy_combo.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pymongo.collection import Collection
 import pytest
 import secrets
 
 
 @pytest.fixture( scope='class' )
 def getMMUDBaseClass( mongo_db ):
-    '''Return a MongoUserDict configured for a per-class unique collection'''
+    """Return a MongoUserDict configured for a per-class unique collection"""
 
     class MyMongoUserDict( mongo_objects.MongoUserDict ):
         collection_name = secrets.token_hex(6)
         database = mongo_db
 
     return MyMongoUserDict
```

### Comparing `mongo_objects-1.1.2/LICENSE.txt` & `mongo_objects-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.1.2/README.rst` & `mongo_objects-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 MongoUserDict
 -------------
 
 ``mongo_objects`` allows us to create our own class for viewing these event documents::
 
     class Event( mongo_objects.MongoUserDict ):
 
-        db = ...     # provide your MongoDB database object here
+        db = ...     # provide your pymongo database object here
         collection_name = 'events'
 
         def isFuture( self ):
             return self['date'] >= datetime.utcnow()
 
 Loop through all events::
```

### Comparing `mongo_objects-1.1.2/pyproject.toml` & `mongo_objects-1.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [project]
 name = "mongo_objects"
 authors = [
   { name="Jonathan Lindstrom", email="lindstrom.j@headwaters.com.sg" },
 ]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "pymongo",
 ]
@@ -27,16 +27,28 @@
 
 [project.urls]
 Homepage = "https://github.com/lindstrom-j/mongo_objects"
 Documentation = "https://mongo-objects.headwaters.com.sg/en/latest/"
 Issues = "https://github.com/lindstrom-j/mongo_objects/issues"
 
 [tool.hatch.version]
-path = "src/__about__.py"
+path = "docs/source/conf.py"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/mongo_objects.py"]
 
-[tool.pytest.ini_options]
-filterwarnings = [
-    'ignore:datetime.datetime.utcnow\(\) is deprecated and scheduled for removal in a future version.:DeprecationWarning',
-]
+[tool.hatch.build.targets.sdist]
+artifacts = [
+  "docs/build/html",
+]
+exclude = [
+  ".gitignore",
+  "pyproject.toml",
+]
+include = [
+  "src",
+  "tests",
+  "sample",
+]
+
+[tool.hatch.build.targets.sdist.sources]
+"docs/build/html" = "docs"
```

### Comparing `mongo_objects-1.1.2/PKG-INFO` & `mongo_objects-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: mongo_objects
-Version: 1.1.2
+Version: 1.2.0
 Summary: Access MongoDB documents and subdocuments through user-defined UserDict and proxy objects.
 Project-URL: Homepage, https://github.com/lindstrom-j/mongo_objects
 Project-URL: Documentation, https://mongo-objects.headwaters.com.sg/en/latest/
 Project-URL: Issues, https://github.com/lindstrom-j/mongo_objects/issues
 Author-email: Jonathan Lindstrom <lindstrom.j@headwaters.com.sg>
 License: MIT License
 License-File: LICENSE.txt
 Keywords: Mongo,MongoDB,pymongo
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: pymongo
 Description-Content-Type: text/x-rst
 
@@ -83,15 +83,15 @@
 MongoUserDict
 -------------
 
 ``mongo_objects`` allows us to create our own class for viewing these event documents::
 
     class Event( mongo_objects.MongoUserDict ):
 
-        db = ...     # provide your MongoDB database object here
+        db = ...     # provide your pymongo database object here
         collection_name = 'events'
 
         def isFuture( self ):
             return self['date'] >= datetime.utcnow()
 
 Loop through all events::
```

