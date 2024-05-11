# Comparing `tmp/bisos.banna-0.2.tar.gz` & `tmp/bisos.banna-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bisos.banna-0.2.tar", last modified: Wed Mar 13 17:09:31 2024, max compression
+gzip compressed data, was "bisos.banna-0.3.tar", last modified: Sat May 11 19:47:25 2024, max compression
```

## Comparing `bisos.banna-0.2.tar` & `bisos.banna-0.3.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-03-13 17:09:31.449900 bisos.banna-0.2/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      175 2024-02-08 18:44:39.000000 bisos.banna-0.2/MANIFEST.in
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1351 2024-03-13 17:09:31.445901 bisos.banna-0.2/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      582 2024-03-13 17:09:30.000000 bisos.banna-0.2/README.rst
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       50 2024-02-08 18:53:10.000000 bisos.banna-0.2/TITLE.txt
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-03-13 17:09:31.445901 bisos.banna-0.2/bin/
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)    11104 2024-02-08 19:19:13.000000 bisos.banna-0.2/bin/bannaInfo.cs
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-03-13 17:09:31.445901 bisos.banna-0.2/bisos/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2024-02-08 18:44:39.000000 bisos.banna-0.2/bisos/__init__.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-03-13 17:09:31.445901 bisos.banna-0.2/bisos/banna/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-02-08 18:44:39.000000 bisos.banna-0.2/bisos/banna/__init__.py
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    13448 2024-02-21 05:43:57.000000 bisos.banna-0.2/bisos/banna/bannaPortNu.py
-drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-03-13 17:09:31.445901 bisos.banna-0.2/bisos.banna.egg-info/
--rw-rw-r--   0 bystar    (2001) bisos     (2222)     1351 2024-03-13 17:09:31.000000 bisos.banna-0.2/bisos.banna.egg-info/PKG-INFO
--rw-rw-r--   0 bystar    (2001) bisos     (2222)      400 2024-03-13 17:09:31.000000 bisos.banna-0.2/bisos.banna.egg-info/SOURCES.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-03-13 17:09:31.000000 bisos.banna-0.2/bisos.banna.egg-info/dependency_links.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-03-13 17:09:31.000000 bisos.banna-0.2/bisos.banna.egg-info/namespace_packages.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-03-13 17:09:31.000000 bisos.banna-0.2/bisos.banna.egg-info/not-zip-safe
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       15 2024-03-13 17:09:31.000000 bisos.banna-0.2/bisos.banna.egg-info/requires.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-03-13 17:09:31.000000 bisos.banna-0.2/bisos.banna.egg-info/top_level.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-03-13 17:09:30.000000 bisos.banna-0.2/lh-agpl3-LICENSE.txt
--rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-03-13 17:09:31.449900 bisos.banna-0.2/setup.cfg
--rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1770 2024-03-13 17:08:22.000000 bisos.banna-0.2/setup.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 19:47:25.282233 bisos.banna-0.3/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      175 2024-02-08 18:44:39.000000 bisos.banna-0.3/MANIFEST.in
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1351 2024-05-11 19:47:25.282233 bisos.banna-0.3/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      582 2024-05-11 19:47:24.000000 bisos.banna-0.3/README.rst
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       50 2024-02-08 18:53:10.000000 bisos.banna-0.3/TITLE.txt
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 19:47:25.282233 bisos.banna-0.3/bin/
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)    11104 2024-02-08 19:19:13.000000 bisos.banna-0.3/bin/bannaInfo.cs
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 19:47:25.282233 bisos.banna-0.3/bisos/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       56 2024-02-08 18:44:39.000000 bisos.banna-0.3/bisos/__init__.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 19:47:25.282233 bisos.banna-0.3/bisos/banna/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        0 2024-02-08 18:44:39.000000 bisos.banna-0.3/bisos/banna/__init__.py
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    13548 2024-05-11 19:13:02.000000 bisos.banna-0.3/bisos/banna/bannaPortNu.py
+drwxrwsr-x   0 bystar    (2001) bisos     (2222)        0 2024-05-11 19:47:25.282233 bisos.banna-0.3/bisos.banna.egg-info/
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)     1351 2024-05-11 19:47:25.000000 bisos.banna-0.3/bisos.banna.egg-info/PKG-INFO
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)      356 2024-05-11 19:47:25.000000 bisos.banna-0.3/bisos.banna.egg-info/SOURCES.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 19:47:25.000000 bisos.banna-0.3/bisos.banna.egg-info/dependency_links.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        1 2024-05-11 19:47:25.000000 bisos.banna-0.3/bisos.banna.egg-info/not-zip-safe
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       15 2024-05-11 19:47:25.000000 bisos.banna-0.3/bisos.banna.egg-info/requires.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)        6 2024-05-11 19:47:25.000000 bisos.banna-0.3/bisos.banna.egg-info/top_level.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)    35067 2024-05-11 19:47:24.000000 bisos.banna-0.3/lh-agpl3-LICENSE.txt
+-rw-rw-r--   0 bystar    (2001) bisos     (2222)       38 2024-05-11 19:47:25.282233 bisos.banna-0.3/setup.cfg
+-rwxrwxr-x   0 bystar    (2001) bisos     (2222)     1772 2024-05-11 19:46:37.000000 bisos.banna-0.3/setup.py
```

### Comparing `bisos.banna-0.2/PKG-INFO` & `bisos.banna-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisos.banna
-Version: 0.2
+Version: 0.3
 Summary: BANA (Bisos Assigned Names and Numbers Authority)
 Home-page: http://www.by-star.net/PLPC/180047
 Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
```

### Comparing `bisos.banna-0.2/README.rst` & `bisos.banna-0.3/README.rst`

 * *Files identical despite different names*

### Comparing `bisos.banna-0.2/bin/bannaInfo.cs` & `bisos.banna-0.3/bin/bannaInfo.cs`

 * *Files identical despite different names*

### Comparing `bisos.banna-0.2/bisos/banna/bannaPortNu.py` & `bisos.banna-0.3/bisos/banna/bannaPortNu.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,19 +176,18 @@
 ####+END:
         if self.cmndDocStr(""" #+begin_org
 ** [[elisp:(org-cycle)][| *CmndDesc:* | ]]  Map svcName to portNu. Outcome is a list of port numbers.
         #+end_org """): return(cmndOutcome)
 
         self.captureRunStr(""" #+begin_org
 #+begin_src sh :results output :session shared
-  bannaInfo.cs -i bannaPortNuOf svcSiteRegistrars
+  bannaInfo.cs -i bannaPortNuOf svcFacter
 #+end_src
 #+RESULTS:
-:
-: ['22222003']
+: ['22222004']
         #+end_org """)
         if self.justCaptureP(): return cmndOutcome
 
         result: list[str] = []
         actionArgs = self.cmndArgsGet("0&9999", cmndArgsSpecDict, argsList)
 
         # print(f"{actionArgs}")
@@ -205,14 +204,17 @@
             if svcName == 'svcSiteRegBox':
                 portNu = "22222001"
             elif svcName == 'svcSiteRegContainer':
                 portNu = "22222002"
             elif svcName == 'svcSiteRegistrars':
                 # combination of
                 portNu = "22222003"
+            elif svcName == 'svcFacter':
+                # combination of
+                portNu = "22222004"
             else:
                 #b_io.eh.problem_usageError(f"Unknown svcName={svcName}")
                 portNu = "NOTFOUND"
 
             return portNu
 
         for each in actionArgs:
```

### Comparing `bisos.banna-0.2/bisos.banna.egg-info/PKG-INFO` & `bisos.banna-0.3/bisos.banna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisos.banna
-Version: 0.2
+Version: 0.3
 Summary: BANA (Bisos Assigned Names and Numbers Authority)
 Home-page: http://www.by-star.net/PLPC/180047
 Download-URL: http://www.by-star.net/PLPC/180047
 Author: Mohsen Banan
 Author-email: libre@mohsen.1.banan.byname.net
 Maintainer: Mohsen Banan
 Maintainer-email: libre@mohsen.1.banan.byname.net
```

### Comparing `bisos.banna-0.2/lh-agpl3-LICENSE.txt` & `bisos.banna-0.3/lh-agpl3-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bisos.banna-0.2/setup.py` & `bisos.banna-0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 #from setuphelpers import get_version, require_python
 #from setuptools import setup
 
 
 #__version__ = get_version('unisos/icm/__init__.py')
-__version__ = '0.2'
+__version__ = '0.3'
 
 
 requires = [
     'bisos.currents',
 ]
 
 #print('Setting up under python version %s' % sys.version)
@@ -39,15 +39,15 @@
     
 data_files = [
 ]
 
 setuptools.setup(
     name='bisos.banna',
     version=__version__,
-    namespace_packages=['bisos'],
+    # namespace_packages=['bisos'],
     packages=setuptools.find_packages(),
     scripts=scripts,
     #data_files=data_files,
     include_package_data=True,
     zip_safe=False,
     author='Mohsen Banan',
     author_email='libre@mohsen.1.banan.byname.net',
```

