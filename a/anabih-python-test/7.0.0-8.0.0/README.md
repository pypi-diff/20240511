# Comparing `tmp/anabih_python_test-7.0.0.tar.gz` & `tmp/anabih_python_test-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anabih_python_test-7.0.0.tar", last modified: Sat May 11 20:13:37 2024, max compression
+gzip compressed data, was "anabih_python_test-8.0.0.tar", last modified: Sat May 11 20:15:59 2024, max compression
```

## Comparing `anabih_python_test-7.0.0.tar` & `anabih_python_test-8.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 20:13:37.944333 anabih_python_test-7.0.0/
--rw-rw-rw-   0        0        0      537 2024-05-11 20:13:37.943333 anabih_python_test-7.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       19 2024-05-09 00:01:05.000000 anabih_python_test-7.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 20:13:37.942333 anabih_python_test-7.0.0/anabih_python_test.egg-info/
--rw-rw-rw-   0        0        0      537 2024-05-11 20:13:37.000000 anabih_python_test-7.0.0/anabih_python_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-11 20:13:37.000000 anabih_python_test-7.0.0/anabih_python_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 20:13:37.000000 anabih_python_test-7.0.0/anabih_python_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-11 20:13:37.000000 anabih_python_test-7.0.0/anabih_python_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 20:13:37.000000 anabih_python_test-7.0.0/anabih_python_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-11 20:13:37.941333 anabih_python_test-7.0.0/my_package/
--rw-rw-rw-   0        0        0        0 2024-05-09 03:08:34.000000 anabih_python_test-7.0.0/my_package/__init__.py
--rw-rw-rw-   0        0        0      468 2024-05-11 20:09:15.000000 anabih_python_test-7.0.0/my_package/greetings.py
--rw-rw-rw-   0        0        0      715 2024-05-11 20:13:25.000000 anabih_python_test-7.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 20:13:37.945334 anabih_python_test-7.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 20:15:59.810819 anabih_python_test-8.0.0/
+-rw-rw-rw-   0        0        0      537 2024-05-11 20:15:59.808797 anabih_python_test-8.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2024-05-09 00:01:05.000000 anabih_python_test-8.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 20:15:59.806795 anabih_python_test-8.0.0/anabih_python_test.egg-info/
+-rw-rw-rw-   0        0        0      537 2024-05-11 20:15:59.000000 anabih_python_test-8.0.0/anabih_python_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-11 20:15:59.000000 anabih_python_test-8.0.0/anabih_python_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 20:15:59.000000 anabih_python_test-8.0.0/anabih_python_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-11 20:15:59.000000 anabih_python_test-8.0.0/anabih_python_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 20:15:59.000000 anabih_python_test-8.0.0/anabih_python_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 20:15:59.803800 anabih_python_test-8.0.0/my_package/
+-rw-rw-rw-   0        0        0        0 2024-05-09 03:08:34.000000 anabih_python_test-8.0.0/my_package/__init__.py
+-rw-rw-rw-   0        0        0      468 2024-05-11 20:09:15.000000 anabih_python_test-8.0.0/my_package/greetings.py
+-rw-rw-rw-   0        0        0      715 2024-05-11 20:15:36.000000 anabih_python_test-8.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 20:15:59.810819 anabih_python_test-8.0.0/setup.cfg
```

### Comparing `anabih_python_test-7.0.0/PKG-INFO` & `anabih_python_test-8.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anabih-python-test
-Version: 7.0.0
+Version: 8.0.0
 Summary: Python Test
 Author-email: Ahmed nabih <anabih2000@yahoo.com.com>
 Project-URL: Homepage, https://github.com/anabih/cicd-teamcity
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.8
```

### Comparing `anabih_python_test-7.0.0/anabih_python_test.egg-info/PKG-INFO` & `anabih_python_test-8.0.0/anabih_python_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anabih-python-test
-Version: 7.0.0
+Version: 8.0.0
 Summary: Python Test
 Author-email: Ahmed nabih <anabih2000@yahoo.com.com>
 Project-URL: Homepage, https://github.com/anabih/cicd-teamcity
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6.8
```

### Comparing `anabih_python_test-7.0.0/pyproject.toml` & `anabih_python_test-8.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Update the values as per your requirement
 [build-system]
 requires = ["setuptools>=57.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "anabih-python-test"
-version = "7.0.0"
+version = "8.0.0"
 authors = [
     { name = "Ahmed nabih", email = "anabih2000@yahoo.com.com" },
 ]
 description = "Python Test"
 readme = "README.md"
 requires-python = ">=3.6.8"
 classifiers = [
```

