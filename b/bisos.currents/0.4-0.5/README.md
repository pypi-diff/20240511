# Comparing `tmp/bisos.currents-0.4.tar.gz` & `tmp/bisos.currents-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bisos.currents-0.4.tar", last modified: Fri Aug 20 03:38:06 2021, max compression
+gzip compressed data, was "bisos.currents-0.5.tar", last modified: Fri Feb 23 20:34:49 2024, max compression
```

## Comparing `bisos.currents-0.4.tar` & `bisos.currents-0.5.tar`

### file list

```diff
@@ -1,41 +1,26 @@
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2021-08-20 03:38:06.046029 bisos.currents-0.4/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      243 2021-08-16 00:38:41.000000 bisos.currents-0.4/MANIFEST.in
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1410 2021-08-20 03:38:06.046029 bisos.currents-0.4/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      600 2021-08-20 03:38:05.000000 bisos.currents-0.4/README.rst
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       90 2021-08-16 00:38:41.000000 bisos.currents-0.4/TITLE.txt
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2021-08-20 03:38:06.042029 bisos.currents-0.4/bin/
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    20363 2021-08-20 02:53:54.000000 bisos.currents-0.4/bin/bx-currentsManage.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2021-08-20 03:38:06.042029 bisos.currents-0.4/bisos/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2021-08-16 00:38:41.000000 bisos.currents-0.4/bisos/__init__.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2021-08-20 03:38:06.046029 bisos.currents-0.4/bisos/currents/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2021-08-16 00:38:41.000000 bisos.currents-0.4/bisos/currents/__init__.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    35492 2021-08-20 02:53:54.000000 bisos.currents-0.4/bisos/currents/bxCurrentsConfig.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     9530 2021-08-20 02:53:54.000000 bisos.currents-0.4/bisos/currents/bxCurrentsThis.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2021-08-20 03:38:06.042029 bisos.currents-0.4/bisos/currents-config/
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2021-08-20 03:38:06.046029 bisos.currents-0.4/bisos/currents-config/admin/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    13223 2021-08-16 00:38:41.000000 bisos.currents-0.4/bisos/currents-config/admin/Panel.org
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       54 2021-08-16 00:38:41.000000 bisos.currents-0.4/bisos/currents-config/admin/siteCurrentsManage.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      250 2021-08-17 22:12:24.000000 bisos.currents-0.4/bisos/currents-config/admin/siteCurrentsManage.py.2to3
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       54 2021-08-16 00:38:41.000000 bisos.currents-0.4/bisos/currents-config/admin/siteCurrentsManage.py.3
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2021-08-20 03:38:06.042029 bisos.currents-0.4/bisos/currents-config/pkgInfo/
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2021-08-20 03:38:06.042029 bisos.currents-0.4/bisos/currents-config/pkgInfo/fp/
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2021-08-20 03:38:06.046029 bisos.currents-0.4/bisos/currents-config/pkgInfo/fp/anyName/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2021-08-16 00:38:41.000000 bisos.currents-0.4/bisos/currents-config/pkgInfo/fp/anyName/_tree_
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        9 2021-08-16 00:38:41.000000 bisos.currents-0.4/bisos/currents-config/pkgInfo/fp/anyName/value
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2021-08-20 03:38:06.046029 bisos.currents-0.4/bisos/currents-config/pkgInfo/fp/bxoId/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2021-08-16 00:38:41.000000 bisos.currents-0.4/bisos/currents-config/pkgInfo/fp/bxoId/_tree_
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        4 2021-08-16 00:38:41.000000 bisos.currents-0.4/bisos/currents-config/pkgInfo/fp/bxoId/value
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2021-08-20 03:38:06.046029 bisos.currents-0.4/bisos/currents-config/pkgInfo/fp/sr/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        5 2021-08-16 00:38:41.000000 bisos.currents-0.4/bisos/currents-config/pkgInfo/fp/sr/_tree_
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       14 2021-08-16 00:38:41.000000 bisos.currents-0.4/bisos/currents-config/pkgInfo/fp/sr/value
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2021-08-20 03:38:06.042029 bisos.currents-0.4/bisos.currents.egg-info/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1410 2021-08-20 03:38:05.000000 bisos.currents-0.4/bisos.currents.egg-info/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      939 2021-08-20 03:38:05.000000 bisos.currents-0.4/bisos.currents.egg-info/SOURCES.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2021-08-20 03:38:05.000000 bisos.currents-0.4/bisos.currents.egg-info/dependency_links.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2021-08-20 03:38:05.000000 bisos.currents-0.4/bisos.currents.egg-info/namespace_packages.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2021-08-20 03:38:05.000000 bisos.currents-0.4/bisos.currents.egg-info/not-zip-safe
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       11 2021-08-20 03:38:05.000000 bisos.currents-0.4/bisos.currents.egg-info/requires.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2021-08-20 03:38:05.000000 bisos.currents-0.4/bisos.currents.egg-info/top_level.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2021-08-16 00:38:41.000000 bisos.currents-0.4/lh-agpl3-LICENSE.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2021-08-20 03:38:06.046029 bisos.currents-0.4/setup.cfg
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1939 2021-08-20 03:37:51.000000 bisos.currents-0.4/setup.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-02-23 20:34:49.923825 bisos.currents-0.5/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      243 2022-06-29 18:36:54.000000 bisos.currents-0.5/MANIFEST.in
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1410 2024-02-23 20:34:49.923825 bisos.currents-0.5/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      600 2024-02-23 20:34:49.000000 bisos.currents-0.5/README.rst
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       90 2022-06-29 18:36:54.000000 bisos.currents-0.5/TITLE.txt
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-02-23 20:34:49.919825 bisos.currents-0.5/bin/
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    11015 2022-09-29 22:04:56.000000 bisos.currents-0.5/bin/bx-currents.cs
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-02-23 20:34:49.919825 bisos.currents-0.5/bisos/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2022-06-29 18:36:54.000000 bisos.currents-0.5/bisos/__init__.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-02-23 20:34:49.919825 bisos.currents-0.5/bisos/currents/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-01-18 01:38:41.000000 bisos.currents-0.5/bisos/currents/__init__.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    35492 2024-01-18 01:38:41.000000 bisos.currents-0.5/bisos/currents/bxCurrentsConfig.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     9530 2024-01-18 01:38:41.000000 bisos.currents-0.5/bisos/currents/bxCurrentsThis.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    33031 2022-10-23 01:59:55.000000 bisos.currents-0.5/bisos/currents/currentsConfig.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    34168 2022-09-29 20:52:10.000000 bisos.currents-0.5/bisos/currents/k1-currentsConfig.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-02-23 20:34:49.919825 bisos.currents-0.5/bisos.currents.egg-info/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1410 2024-02-23 20:34:49.000000 bisos.currents-0.5/bisos.currents.egg-info/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      536 2024-02-23 20:34:49.000000 bisos.currents-0.5/bisos.currents.egg-info/SOURCES.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-02-23 20:34:49.000000 bisos.currents-0.5/bisos.currents.egg-info/dependency_links.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-02-23 20:34:49.000000 bisos.currents-0.5/bisos.currents.egg-info/namespace_packages.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-02-23 20:34:49.000000 bisos.currents-0.5/bisos.currents.egg-info/not-zip-safe
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       11 2024-02-23 20:34:49.000000 bisos.currents-0.5/bisos.currents.egg-info/requires.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-02-23 20:34:49.000000 bisos.currents-0.5/bisos.currents.egg-info/top_level.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-02-23 20:34:49.000000 bisos.currents-0.5/lh-agpl3-LICENSE.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-02-23 20:34:49.923825 bisos.currents-0.5/setup.cfg
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1933 2024-02-23 20:33:43.000000 bisos.currents-0.5/setup.py
```

### Comparing `bisos.currents-0.4/PKG-INFO` & `bisos.currents-0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: bisos.currents
-Version: 0.4
+Version: 0.5
 Summary: bisos.currents: Currents Information Configuration Parameters For BISOS and BISOS Pkgs.
 Home-page: http://www.by-star.net/PLPC/180047
+Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
 License: AGPL
-Download-URL: http://www.by-star.net/PLPC/180047
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `bisos.currents-0.4/README.rst` & `bisos.currents-0.5/README.rst`

 * *Files identical despite different names*

### Comparing `bisos.currents-0.4/bisos/currents/bxCurrentsConfig.py` & `bisos.currents-0.5/bisos/currents/bxCurrentsConfig.py`

 * *Files identical despite different names*

### Comparing `bisos.currents-0.4/bisos/currents/bxCurrentsThis.py` & `bisos.currents-0.5/bisos/currents/bxCurrentsThis.py`

 * *Files identical despite different names*

### Comparing `bisos.currents-0.4/bisos.currents.egg-info/PKG-INFO` & `bisos.currents-0.5/bisos.currents.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: bisos.currents
-Version: 0.4
+Version: 0.5
 Summary: bisos.currents: Currents Information Configuration Parameters For BISOS and BISOS Pkgs.
 Home-page: http://www.by-star.net/PLPC/180047
+Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
 License: AGPL
-Download-URL: http://www.by-star.net/PLPC/180047
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `bisos.currents-0.4/lh-agpl3-LICENSE.txt` & `bisos.currents-0.5/lh-agpl3-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bisos.currents-0.4/setup.py` & `bisos.currents-0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 
 #from setuphelpers import get_version, require_python
 #from setuptools import setup
 
 
 #__version__ = get_version('unisos/icm/__init__.py')
-__version__ = '0.4'
+__version__ = '0.5'
 
 
 requires = [
     'unisos.icm',
 ]
 
 #print('Setting up under python version %s' % sys.version)
 #print('Requirements: %s' % ','.join(requires))
 
 scripts = [
-    "bin/bx-currentsManage.py",
+    "bin/bx-currents.cs",
 ]
 
 data_files = [
 ]
 
 setuptools.setup(
     name='bisos.currents',
```

