# Comparing `tmp/splupy2check-1.0.0.tar.gz` & `tmp/splupy2check-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splupy2check-1.0.0.tar", last modified: Sat May 11 09:43:36 2024, max compression
+gzip compressed data, was "splupy2check-1.0.1.tar", last modified: Sat May 11 10:09:47 2024, max compression
```

## Comparing `splupy2check-1.0.0.tar` & `splupy2check-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sschimper  (1000) sschimper  (1000)        0 2024-05-11 09:43:36.757207 splupy2check-1.0.0/
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1272 2024-05-11 09:43:36.757207 splupy2check-1.0.0/PKG-INFO
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)      656 2024-05-11 09:39:32.000000 splupy2check-1.0.0/README.md
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       38 2024-05-11 09:43:36.757207 splupy2check-1.0.0/setup.cfg
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1408 2024-05-11 09:38:17.000000 splupy2check-1.0.0/setup.py
-drwxrwxr-x   0 sschimper  (1000) sschimper  (1000)        0 2024-05-11 09:43:36.757207 splupy2check-1.0.0/splupy2check/
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)        0 2024-05-11 07:47:18.000000 splupy2check-1.0.0/splupy2check/__init__.py
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     2167 2024-05-11 09:39:38.000000 splupy2check-1.0.0/splupy2check/splupy2check.py
-drwxrwxr-x   0 sschimper  (1000) sschimper  (1000)        0 2024-05-11 09:43:36.757207 splupy2check-1.0.0/splupy2check.egg-info/
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1272 2024-05-11 09:43:36.000000 splupy2check-1.0.0/splupy2check.egg-info/PKG-INFO
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)      290 2024-05-11 09:43:36.000000 splupy2check-1.0.0/splupy2check.egg-info/SOURCES.txt
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)        1 2024-05-11 09:43:36.000000 splupy2check-1.0.0/splupy2check.egg-info/dependency_links.txt
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       72 2024-05-11 09:43:36.000000 splupy2check-1.0.0/splupy2check.egg-info/entry_points.txt
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       27 2024-05-11 09:43:36.000000 splupy2check-1.0.0/splupy2check.egg-info/requires.txt
--rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       13 2024-05-11 09:43:36.000000 splupy2check-1.0.0/splupy2check.egg-info/top_level.txt
+drwxrwxr-x   0 sschimper  (1000) sschimper  (1000)        0 2024-05-11 10:09:47.090031 splupy2check-1.0.1/
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1272 2024-05-11 10:09:47.090031 splupy2check-1.0.1/PKG-INFO
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)      656 2024-05-11 09:39:32.000000 splupy2check-1.0.1/README.md
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       38 2024-05-11 10:09:47.090031 splupy2check-1.0.1/setup.cfg
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1395 2024-05-11 10:09:14.000000 splupy2check-1.0.1/setup.py
+drwxrwxr-x   0 sschimper  (1000) sschimper  (1000)        0 2024-05-11 10:09:47.090031 splupy2check-1.0.1/splupy2check/
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)        0 2024-05-11 07:47:18.000000 splupy2check-1.0.1/splupy2check/__init__.py
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     2167 2024-05-11 10:09:16.000000 splupy2check-1.0.1/splupy2check/splupy2check.py
+drwxrwxr-x   0 sschimper  (1000) sschimper  (1000)        0 2024-05-11 10:09:47.090031 splupy2check-1.0.1/splupy2check.egg-info/
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)     1272 2024-05-11 10:09:47.000000 splupy2check-1.0.1/splupy2check.egg-info/PKG-INFO
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)      290 2024-05-11 10:09:47.000000 splupy2check-1.0.1/splupy2check.egg-info/SOURCES.txt
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)        1 2024-05-11 10:09:47.000000 splupy2check-1.0.1/splupy2check.egg-info/dependency_links.txt
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       72 2024-05-11 10:09:47.000000 splupy2check-1.0.1/splupy2check.egg-info/entry_points.txt
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       20 2024-05-11 10:09:47.000000 splupy2check-1.0.1/splupy2check.egg-info/requires.txt
+-rw-rw-r--   0 sschimper  (1000) sschimper  (1000)       13 2024-05-11 10:09:47.000000 splupy2check-1.0.1/splupy2check.egg-info/top_level.txt
```

### Comparing `splupy2check-1.0.0/PKG-INFO` & `splupy2check-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splupy2check
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scans file or folder to be scanned for containing Python 2 code.
 Home-page: UNKNOWN
 Author: Sebastian Schimper
 Author-email: sebastianschimper@gmail.com
 License: UNKNOWN
 Keywords: python,splunk,python2,scanning
 Platform: UNKNOWN
```

### Comparing `splupy2check-1.0.0/README.md` & `splupy2check-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `splupy2check-1.0.0/setup.py` & `splupy2check-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 DESCRIPTION = "Scans file or folder to be scanned for containing Python 2 code."
 LONG_DESCRIPTION = """
 Checks for occurances of Python2 files in a given folder structure.
 The program recursively traverses the folder structure, and if a .py file is encountered,
 it is compiled with Python3. 
 """
 
@@ -23,15 +23,15 @@
       },
       author="Sebastian Schimper",
       author_email="sebastianschimper@gmail.com",
       description=DESCRIPTION,
       long_description_content_type="text/markdown",
       long_description=long_description,
       packages=find_packages(),
-      install_requires=["argparse", "os", "sys", "subprocess"],
+      install_requires=["argparse", "subprocess"],
       keywords=["python", "splunk", "python2", "scanning"],
       classifiers=[
           "Development Status :: 1 - Planning",
           "Intended Audience :: Developers",
           "Programming Language :: Python :: 3",
           "Operating System :: Unix",
           "Operating System :: MacOS :: MacOS X",
```

### Comparing `splupy2check-1.0.0/splupy2check/splupy2check.py` & `splupy2check-1.0.1/splupy2check/splupy2check.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         help="File or folder to be scanned for containing Python 2 code.")
     parser.add_argument("-o",
                         "--output",
                         help="Stores program output in a file.")
     parser.add_argument("-v",
                         "--version",
                         action="version",
-                        version="1.0.0",
+                        version="1.0.1",
                         help="Prints the version.")
     return parser.parse_args()
 
 
 def compile(file):
     if not (file.endswith(".py")):
         return
```

### Comparing `splupy2check-1.0.0/splupy2check.egg-info/PKG-INFO` & `splupy2check-1.0.1/splupy2check.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splupy2check
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scans file or folder to be scanned for containing Python 2 code.
 Home-page: UNKNOWN
 Author: Sebastian Schimper
 Author-email: sebastianschimper@gmail.com
 License: UNKNOWN
 Keywords: python,splunk,python2,scanning
 Platform: UNKNOWN
```

