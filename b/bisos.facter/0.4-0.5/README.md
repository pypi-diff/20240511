# Comparing `tmp/bisos.facter-0.4.tar.gz` & `tmp/bisos.facter-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bisos.facter-0.4.tar", last modified: Sat May 11 04:33:43 2024, max compression
+gzip compressed data, was "bisos.facter-0.5.tar", last modified: Sat May 11 04:38:44 2024, max compression
```

## Comparing `bisos.facter-0.4.tar` & `bisos.facter-0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:33:43.340991 bisos.facter-0.4/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       71 2024-05-10 16:52:15.000000 bisos.facter-0.4/MANIFEST.in
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1572 2024-05-11 04:33:43.340991 bisos.facter-0.4/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      677 2024-05-11 04:33:42.000000 bisos.facter-0.4/README.rst
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      112 2024-05-10 16:52:15.000000 bisos.facter-0.4/TITLE.txt
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:33:43.340991 bisos.facter-0.4/bin/
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.4/bin/facter.cs
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.4/bin/roInv-facter.cs
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.4/bin/roPerf-facter.cs
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:33:43.340991 bisos.facter-0.4/bisos/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2024-05-10 16:52:15.000000 bisos.facter-0.4/bisos/__init__.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:33:43.340991 bisos.facter-0.4/bisos/facter/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-05-10 16:52:15.000000 bisos.facter-0.4/bisos/facter/__init__.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    17084 2024-05-10 16:52:15.000000 bisos.facter-0.4/bisos/facter/facter.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    33972 2024-05-10 16:52:15.000000 bisos.facter-0.4/bisos/facter/facter_csu.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:33:43.340991 bisos.facter-0.4/bisos.facter.egg-info/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1572 2024-05-11 04:33:43.000000 bisos.facter-0.4/bisos.facter.egg-info/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      430 2024-05-11 04:33:43.000000 bisos.facter-0.4/bisos.facter.egg-info/SOURCES.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 04:33:43.000000 bisos.facter-0.4/bisos.facter.egg-info/dependency_links.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 04:33:43.000000 bisos.facter-0.4/bisos.facter.egg-info/not-zip-safe
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       33 2024-05-11 04:33:43.000000 bisos.facter-0.4/bisos.facter.egg-info/requires.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-11 04:33:43.000000 bisos.facter-0.4/bisos.facter.egg-info/top_level.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-11 04:33:42.000000 bisos.facter-0.4/lh-agpl3-LICENSE.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-11 04:33:43.340991 bisos.facter-0.4/setup.cfg
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1707 2024-05-11 04:32:53.000000 bisos.facter-0.4/setup.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:38:44.671281 bisos.facter-0.5/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       71 2024-05-10 16:52:15.000000 bisos.facter-0.5/MANIFEST.in
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1588 2024-05-11 04:38:44.671281 bisos.facter-0.5/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      677 2024-05-11 04:38:43.000000 bisos.facter-0.5/README.rst
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      112 2024-05-10 16:52:15.000000 bisos.facter-0.5/TITLE.txt
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:38:44.671281 bisos.facter-0.5/bin/
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.5/bin/facter.cs
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.5/bin/roInv-facter.cs
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    12432 2024-05-10 16:52:15.000000 bisos.facter-0.5/bin/roPerf-facter.cs
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:38:44.671281 bisos.facter-0.5/bisos/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2024-05-10 16:52:15.000000 bisos.facter-0.5/bisos/__init__.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:38:44.671281 bisos.facter-0.5/bisos/facter/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-05-10 16:52:15.000000 bisos.facter-0.5/bisos/facter/__init__.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    17084 2024-05-10 16:52:15.000000 bisos.facter-0.5/bisos/facter/facter.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    33972 2024-05-10 16:52:15.000000 bisos.facter-0.5/bisos/facter/facter_csu.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 04:38:44.671281 bisos.facter-0.5/bisos.facter.egg-info/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1588 2024-05-11 04:38:44.000000 bisos.facter-0.5/bisos.facter.egg-info/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      430 2024-05-11 04:38:44.000000 bisos.facter-0.5/bisos.facter.egg-info/SOURCES.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 04:38:44.000000 bisos.facter-0.5/bisos.facter.egg-info/dependency_links.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 04:38:44.000000 bisos.facter-0.5/bisos.facter.egg-info/not-zip-safe
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       39 2024-05-11 04:38:44.000000 bisos.facter-0.5/bisos.facter.egg-info/requires.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-11 04:38:44.000000 bisos.facter-0.5/bisos.facter.egg-info/top_level.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-11 04:38:43.000000 bisos.facter-0.5/lh-agpl3-LICENSE.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-11 04:38:44.671281 bisos.facter-0.5/setup.cfg
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1720 2024-05-11 04:37:57.000000 bisos.facter-0.5/setup.py
```

### Comparing `bisos.facter-0.4/PKG-INFO` & `bisos.facter-0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisos.facter
-Version: 0.4
+Version: 0.5
 Summary: bisos.facter: Adoption and adaptation of facter to Python and PyCS-Framework and BISOS for use with BISOS-CMDB.
 Home-page: http://www.by-star.net/PLPC/180047
 Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
@@ -13,14 +13,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires: bisos
 Requires: bisos.b
 Requires: bisos.banna
 Requires: bisos.common
 
 ============
 bisos.facter
 ============
```

### Comparing `bisos.facter-0.4/README.rst` & `bisos.facter-0.5/README.rst`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.4/bin/facter.cs` & `bisos.facter-0.5/bin/facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.4/bin/roInv-facter.cs` & `bisos.facter-0.5/bin/roInv-facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.4/bin/roPerf-facter.cs` & `bisos.facter-0.5/bin/roPerf-facter.cs`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.4/bisos/facter/facter.py` & `bisos.facter-0.5/bisos/facter/facter.py`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.4/bisos/facter/facter_csu.py` & `bisos.facter-0.5/bisos/facter/facter_csu.py`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.4/bisos.facter.egg-info/PKG-INFO` & `bisos.facter-0.5/bisos.facter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisos.facter
-Version: 0.4
+Version: 0.5
 Summary: bisos.facter: Adoption and adaptation of facter to Python and PyCS-Framework and BISOS for use with BISOS-CMDB.
 Home-page: http://www.by-star.net/PLPC/180047
 Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
@@ -13,14 +13,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires: bisos
 Requires: bisos.b
 Requires: bisos.banna
 Requires: bisos.common
 
 ============
 bisos.facter
 ============
```

### Comparing `bisos.facter-0.4/lh-agpl3-LICENSE.txt` & `bisos.facter-0.5/lh-agpl3-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bisos.facter-0.4/setup.py` & `bisos.facter-0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,19 @@
         return f.read()
 
 
 # from setuphelpers import get_version, require_python
 # from setuptools import setup
 
 # __version__ = get_version('unisos/icm/__init__.py')
-__version__ = '0.4'
+__version__ = '0.5'
 
 
 requires = [
+    "bisos",
     "bisos.b",
     "bisos.banna",
     "bisos.common",
 ]
 
 
 # print('Setting up under python version %s' % sys.version)
```

