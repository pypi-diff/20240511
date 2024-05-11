# Comparing `tmp/aguirre-0.1.0.tar.gz` & `tmp/aguirre-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aguirre-0.1.0.tar", last modified: Sat Apr 13 09:25:16 2024, max compression
+gzip compressed data, was "aguirre-0.1.1.tar", last modified: Sat May 11 08:43:16 2024, max compression
```

## Comparing `aguirre-0.1.0.tar` & `aguirre-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2024-04-13 09:25:16.485533 aguirre-0.1.0/
--rw-rw-r--   0 psc       (1000) psc       (1000)     1428 2024-04-06 11:51:54.000000 aguirre-0.1.0/LICENCE.txt
--rw-rw-r--   0 psc       (1000) psc       (1000)     3551 2024-04-13 09:25:16.485533 aguirre-0.1.0/PKG-INFO
--rw-rw-r--   0 psc       (1000) psc       (1000)     2167 2024-04-13 09:14:17.000000 aguirre-0.1.0/README.md
-drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2024-04-13 09:25:16.485533 aguirre-0.1.0/aguirre/
--rw-rw-r--   0 psc       (1000) psc       (1000)       22 2024-04-09 12:22:52.000000 aguirre-0.1.0/aguirre/__init__.py
-drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2024-04-13 09:25:16.485533 aguirre-0.1.0/aguirre/integrations/
--rw-rw-r--   0 psc       (1000) psc       (1000)        0 2024-04-06 11:51:54.000000 aguirre-0.1.0/aguirre/integrations/__init__.py
--rw-rw-r--   0 psc       (1000) psc       (1000)     1063 2024-04-06 11:51:54.000000 aguirre-0.1.0/aguirre/integrations/flask.py
--rw-rw-r--   0 psc       (1000) psc       (1000)     1075 2024-04-06 17:04:13.000000 aguirre-0.1.0/aguirre/integrations/quart.py
--rw-rw-r--   0 psc       (1000) psc       (1000)        0 2024-04-06 11:51:54.000000 aguirre-0.1.0/aguirre/py.typed
--rw-rw-r--   0 psc       (1000) psc       (1000)      914 2024-04-06 16:11:44.000000 aguirre-0.1.0/aguirre/util.py
-drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2024-04-13 09:25:16.485533 aguirre-0.1.0/aguirre.egg-info/
--rw-r--r--   0 psc       (1000) psc       (1000)     3551 2024-04-13 09:25:16.000000 aguirre-0.1.0/aguirre.egg-info/PKG-INFO
--rw-rw-r--   0 psc       (1000) psc       (1000)      359 2024-04-13 09:25:16.000000 aguirre-0.1.0/aguirre.egg-info/SOURCES.txt
--rw-rw-r--   0 psc       (1000) psc       (1000)        1 2024-04-13 09:25:16.000000 aguirre-0.1.0/aguirre.egg-info/dependency_links.txt
--rw-rw-r--   0 psc       (1000) psc       (1000)       35 2024-04-13 09:25:16.000000 aguirre-0.1.0/aguirre.egg-info/requires.txt
--rw-rw-r--   0 psc       (1000) psc       (1000)        8 2024-04-13 09:25:16.000000 aguirre-0.1.0/aguirre.egg-info/top_level.txt
--rw-rw-r--   0 psc       (1000) psc       (1000)     1244 2024-04-13 09:25:16.485533 aguirre-0.1.0/setup.cfg
--rw-rw-r--   0 psc       (1000) psc       (1000)      161 2024-04-06 11:51:54.000000 aguirre-0.1.0/setup.py
-drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2024-04-13 09:25:16.485533 aguirre-0.1.0/tests/
--rw-rw-r--   0 psc       (1000) psc       (1000)      363 2024-04-06 11:51:54.000000 aguirre-0.1.0/tests/test_util.py
+drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2024-05-11 08:43:16.730473 aguirre-0.1.1/
+-rw-rw-r--   0 psc       (1000) psc       (1000)     1428 2024-04-06 11:51:54.000000 aguirre-0.1.1/LICENCE.txt
+-rw-rw-r--   0 psc       (1000) psc       (1000)     4071 2024-05-11 08:43:16.730473 aguirre-0.1.1/PKG-INFO
+-rw-rw-r--   0 psc       (1000) psc       (1000)     2497 2024-05-03 12:30:18.000000 aguirre-0.1.1/README.md
+drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2024-05-11 08:43:16.730473 aguirre-0.1.1/aguirre/
+-rw-rw-r--   0 psc       (1000) psc       (1000)       22 2024-05-11 08:42:05.000000 aguirre-0.1.1/aguirre/__init__.py
+drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2024-05-11 08:43:16.730473 aguirre-0.1.1/aguirre/integrations/
+-rw-rw-r--   0 psc       (1000) psc       (1000)        0 2024-04-06 11:51:54.000000 aguirre-0.1.1/aguirre/integrations/__init__.py
+-rw-rw-r--   0 psc       (1000) psc       (1000)     1063 2024-04-06 11:51:54.000000 aguirre-0.1.1/aguirre/integrations/flask.py
+-rw-rw-r--   0 psc       (1000) psc       (1000)     1075 2024-04-06 17:04:13.000000 aguirre-0.1.1/aguirre/integrations/quart.py
+-rw-rw-r--   0 psc       (1000) psc       (1000)        0 2024-04-06 11:51:54.000000 aguirre-0.1.1/aguirre/py.typed
+-rw-rw-r--   0 psc       (1000) psc       (1000)      914 2024-04-06 16:11:44.000000 aguirre-0.1.1/aguirre/util.py
+drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2024-05-11 08:43:16.730473 aguirre-0.1.1/aguirre.egg-info/
+-rw-r--r--   0 psc       (1000) psc       (1000)     4071 2024-05-11 08:43:16.000000 aguirre-0.1.1/aguirre.egg-info/PKG-INFO
+-rw-rw-r--   0 psc       (1000) psc       (1000)      359 2024-05-11 08:43:16.000000 aguirre-0.1.1/aguirre.egg-info/SOURCES.txt
+-rw-rw-r--   0 psc       (1000) psc       (1000)        1 2024-05-11 08:43:16.000000 aguirre-0.1.1/aguirre.egg-info/dependency_links.txt
+-rw-rw-r--   0 psc       (1000) psc       (1000)       44 2024-05-11 08:43:16.000000 aguirre-0.1.1/aguirre.egg-info/requires.txt
+-rw-rw-r--   0 psc       (1000) psc       (1000)        8 2024-05-11 08:43:16.000000 aguirre-0.1.1/aguirre.egg-info/top_level.txt
+-rw-rw-r--   0 psc       (1000) psc       (1000)     1367 2024-05-11 08:43:16.734473 aguirre-0.1.1/setup.cfg
+-rw-rw-r--   0 psc       (1000) psc       (1000)      161 2024-04-06 11:51:54.000000 aguirre-0.1.1/setup.py
+drwxrwxr-x   0 psc       (1000) psc       (1000)        0 2024-05-11 08:43:16.730473 aguirre-0.1.1/tests/
+-rw-rw-r--   0 psc       (1000) psc       (1000)     1693 2024-04-27 10:46:38.000000 aguirre-0.1.1/tests/test_util.py
```

### Comparing `aguirre-0.1.0/LICENCE.txt` & `aguirre-0.1.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `aguirre-0.1.0/PKG-INFO` & `aguirre-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aguirre
-Version: 0.1.0
+Version: 0.1.1
 Summary: Let Python webservers self-host JS/CSS/etc assets like unpkg does
 Home-page: https://github.com/pscl4rke/aguirre
 Author: P. S. Clarke
 Author-email: aguirre@pscl4rke.net
 License: cf:licence
 Project-URL: Source Code, https://github.com/pscl4rke/aguirre
 Project-URL: Issues, https://github.com/pscl4rke/aguirre/issues
@@ -66,22 +66,35 @@
         There are some integrations into frameworks inside
         `aguirre.integrations`.
         Their usage is documented in the module docstrings...
         
         * [Flask](https://github.com/pscl4rke/aguirre/blob/master/aguirre/integrations/flask.py)
         * [Quart](https://github.com/pscl4rke/aguirre/blob/master/aguirre/integrations/quart.py)
         
+        ## Development and Testing
+        
+        This codebase uses
+        [ephemerun](https://github.com/pscl4rke/ephemerun)
+        to test against multiple Python versions.
+        (It's a bit like Tox,
+        except is uses containers for isolation rather than virtualenvs.)
+        
         ## Licence
         
         This code is copyright P. S. Clarke and is licensed under
         the BSD-3-Clause licence.
         
+        The test suite contains real-world example files.
+        These are covered by their own embedded licences.
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aguirre Version: 0.1.0 Summary: Let Python
+Metadata-Version: 2.1 Name: aguirre Version: 0.1.1 Summary: Let Python
 webservers self-host JS/CSS/etc assets like unpkg does Home-page: https://
 github.com/pscl4rke/aguirre Author: P. S. Clarke Author-email:
 aguirre@pscl4rke.net License: cf:licence Project-URL: Source Code, https://
 github.com/pscl4rke/aguirre Project-URL: Issues, https://github.com/pscl4rke/
 aguirre/issues Project-URL: Licence, https://github.com/pscl4rke/utterless/
 blob/master/LICENCE.txt Description: # Aguirre > Let Python webservers self-
 host JS/CSS/etc assets like unpkg does **Warning: The utility functions have
@@ -26,14 +26,20 @@
 Sure, it's not the most scalable solution. But it's a great way to quickly get
 things moving. ## Installation This code is not currently on PyPI. Consequently
 you should add the following line to your `requirements.txt` file: git+https://
 github.com/pscl4rke/aguirre.git ## Integrations There are some integrations
 into frameworks inside `aguirre.integrations`. Their usage is documented in the
 module docstrings... * [Flask](https://github.com/pscl4rke/aguirre/blob/master/
 aguirre/integrations/flask.py) * [Quart](https://github.com/pscl4rke/aguirre/
-blob/master/aguirre/integrations/quart.py) ## Licence This code is copyright P.
-S. Clarke and is licensed under the BSD-3-Clause licence. Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: testing
+blob/master/aguirre/integrations/quart.py) ## Development and Testing This
+codebase uses [ephemerun](https://github.com/pscl4rke/ephemerun) to test
+against multiple Python versions. (It's a bit like Tox, except is uses
+containers for isolation rather than virtualenvs.) ## Licence This code is
+copyright P. S. Clarke and is licensed under the BSD-3-Clause licence. The test
+suite contains real-world example files. These are covered by their own
+embedded licences. Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.7 Description-
+Content-Type: text/markdown Provides-Extra: testing
```

### Comparing `aguirre-0.1.0/README.md` & `aguirre-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -55,11 +55,22 @@
 There are some integrations into frameworks inside
 `aguirre.integrations`.
 Their usage is documented in the module docstrings...
 
 * [Flask](https://github.com/pscl4rke/aguirre/blob/master/aguirre/integrations/flask.py)
 * [Quart](https://github.com/pscl4rke/aguirre/blob/master/aguirre/integrations/quart.py)
 
+## Development and Testing
+
+This codebase uses
+[ephemerun](https://github.com/pscl4rke/ephemerun)
+to test against multiple Python versions.
+(It's a bit like Tox,
+except is uses containers for isolation rather than virtualenvs.)
+
 ## Licence
 
 This code is copyright P. S. Clarke and is licensed under
 the BSD-3-Clause licence.
+
+The test suite contains real-world example files.
+These are covered by their own embedded licences.
```

#### html2text {}

```diff
@@ -19,9 +19,14 @@
 Sure, it's not the most scalable solution. But it's a great way to quickly get
 things moving. ## Installation This code is not currently on PyPI. Consequently
 you should add the following line to your `requirements.txt` file: git+https://
 github.com/pscl4rke/aguirre.git ## Integrations There are some integrations
 into frameworks inside `aguirre.integrations`. Their usage is documented in the
 module docstrings... * [Flask](https://github.com/pscl4rke/aguirre/blob/master/
 aguirre/integrations/flask.py) * [Quart](https://github.com/pscl4rke/aguirre/
-blob/master/aguirre/integrations/quart.py) ## Licence This code is copyright P.
-S. Clarke and is licensed under the BSD-3-Clause licence.
+blob/master/aguirre/integrations/quart.py) ## Development and Testing This
+codebase uses [ephemerun](https://github.com/pscl4rke/ephemerun) to test
+against multiple Python versions. (It's a bit like Tox, except is uses
+containers for isolation rather than virtualenvs.) ## Licence This code is
+copyright P. S. Clarke and is licensed under the BSD-3-Clause licence. The test
+suite contains real-world example files. These are covered by their own
+embedded licences.
```

### Comparing `aguirre-0.1.0/aguirre/integrations/flask.py` & `aguirre-0.1.1/aguirre/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `aguirre-0.1.0/aguirre/integrations/quart.py` & `aguirre-0.1.1/aguirre/integrations/quart.py`

 * *Files identical despite different names*

### Comparing `aguirre-0.1.0/aguirre/util.py` & `aguirre-0.1.1/aguirre/util.py`

 * *Files identical despite different names*

### Comparing `aguirre-0.1.0/aguirre.egg-info/PKG-INFO` & `aguirre-0.1.1/aguirre.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aguirre
-Version: 0.1.0
+Version: 0.1.1
 Summary: Let Python webservers self-host JS/CSS/etc assets like unpkg does
 Home-page: https://github.com/pscl4rke/aguirre
 Author: P. S. Clarke
 Author-email: aguirre@pscl4rke.net
 License: cf:licence
 Project-URL: Source Code, https://github.com/pscl4rke/aguirre
 Project-URL: Issues, https://github.com/pscl4rke/aguirre/issues
@@ -66,22 +66,35 @@
         There are some integrations into frameworks inside
         `aguirre.integrations`.
         Their usage is documented in the module docstrings...
         
         * [Flask](https://github.com/pscl4rke/aguirre/blob/master/aguirre/integrations/flask.py)
         * [Quart](https://github.com/pscl4rke/aguirre/blob/master/aguirre/integrations/quart.py)
         
+        ## Development and Testing
+        
+        This codebase uses
+        [ephemerun](https://github.com/pscl4rke/ephemerun)
+        to test against multiple Python versions.
+        (It's a bit like Tox,
+        except is uses containers for isolation rather than virtualenvs.)
+        
         ## Licence
         
         This code is copyright P. S. Clarke and is licensed under
         the BSD-3-Clause licence.
         
+        The test suite contains real-world example files.
+        These are covered by their own embedded licences.
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aguirre Version: 0.1.0 Summary: Let Python
+Metadata-Version: 2.1 Name: aguirre Version: 0.1.1 Summary: Let Python
 webservers self-host JS/CSS/etc assets like unpkg does Home-page: https://
 github.com/pscl4rke/aguirre Author: P. S. Clarke Author-email:
 aguirre@pscl4rke.net License: cf:licence Project-URL: Source Code, https://
 github.com/pscl4rke/aguirre Project-URL: Issues, https://github.com/pscl4rke/
 aguirre/issues Project-URL: Licence, https://github.com/pscl4rke/utterless/
 blob/master/LICENCE.txt Description: # Aguirre > Let Python webservers self-
 host JS/CSS/etc assets like unpkg does **Warning: The utility functions have
@@ -26,14 +26,20 @@
 Sure, it's not the most scalable solution. But it's a great way to quickly get
 things moving. ## Installation This code is not currently on PyPI. Consequently
 you should add the following line to your `requirements.txt` file: git+https://
 github.com/pscl4rke/aguirre.git ## Integrations There are some integrations
 into frameworks inside `aguirre.integrations`. Their usage is documented in the
 module docstrings... * [Flask](https://github.com/pscl4rke/aguirre/blob/master/
 aguirre/integrations/flask.py) * [Quart](https://github.com/pscl4rke/aguirre/
-blob/master/aguirre/integrations/quart.py) ## Licence This code is copyright P.
-S. Clarke and is licensed under the BSD-3-Clause licence. Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: testing
+blob/master/aguirre/integrations/quart.py) ## Development and Testing This
+codebase uses [ephemerun](https://github.com/pscl4rke/ephemerun) to test
+against multiple Python versions. (It's a bit like Tox, except is uses
+containers for isolation rather than virtualenvs.) ## Licence This code is
+copyright P. S. Clarke and is licensed under the BSD-3-Clause licence. The test
+suite contains real-world example files. These are covered by their own
+embedded licences. Platform: UNKNOWN Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.7 Description-
+Content-Type: text/markdown Provides-Extra: testing
```

### Comparing `aguirre-0.1.0/setup.cfg` & `aguirre-0.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -15,25 +15,28 @@
 author_email = aguirre@pscl4rke.net
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Internet :: WWW/HTTP
 
 [options]
 python_requires = >=3.7
 packages = 
 	aguirre
 	aguirre.integrations
 include-package-data = True
 
 [options.extras_require]
 testing = 
+	coverage
 	flask
 	mypy
 	pyroma
 	quart
 
 [options.package_data]
 aguirre = py.typed
@@ -41,14 +44,17 @@
 [mypy]
 check_untyped_defs = True
 disallow_incomplete_defs = True
 disallow_untyped_defs = True
 disallow_untyped_decorators = True
 disallow_untyped_calls = True
 
+[coverage:run]
+source = aguirre
+
 [tool:check-wheel-contents]
 package = aguirre
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

