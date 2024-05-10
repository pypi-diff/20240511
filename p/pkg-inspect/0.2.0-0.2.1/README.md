# Comparing `tmp/pkg_inspect-0.2.0.tar.gz` & `tmp/pkg_inspect-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_inspect-0.2.0.tar", last modified: Wed May  8 04:12:22 2024, max compression
+gzip compressed data, was "pkg_inspect-0.2.1.tar", last modified: Fri May 10 23:06:52 2024, max compression
```

## Comparing `pkg_inspect-0.2.0.tar` & `pkg_inspect-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:12:22.411552 pkg_inspect-0.2.0/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.2.0/LICENSE.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      399 2024-05-02 01:09:23.000000 pkg_inspect-0.2.0/MANIFEST.in
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9663 2024-05-08 04:12:22.411237 pkg_inspect-0.2.0/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.2.0/README.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1037 2024-05-08 04:12:22.412518 pkg_inspect-0.2.0/setup.cfg
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.2.0/setup.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:12:22.394899 pkg_inspect-0.2.0/src/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       26 2024-05-07 01:45:11.000000 pkg_inspect-0.2.0/src/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:12:22.395677 pkg_inspect-0.2.0/src/pkg_inspect/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       56 2024-05-08 03:30:25.000000 pkg_inspect-0.2.0/src/pkg_inspect/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:12:22.400604 pkg_inspect-0.2.0/src/pkg_inspect/pkg_functions/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      337 2024-05-07 01:13:31.000000 pkg_inspect-0.2.0/src/pkg_inspect/pkg_functions/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    13926 2024-05-08 04:10:58.000000 pkg_inspect-0.2.0/src/pkg_inspect/pkg_functions/functions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:12:22.403610 pkg_inspect-0.2.0/src/pkg_inspect/pkg_modules/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      166 2024-05-06 02:47:26.000000 pkg_inspect-0.2.0/src/pkg_inspect/pkg_modules/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47596 2024-05-08 03:30:25.000000 pkg_inspect-0.2.0/src/pkg_inspect/pkg_modules/pkg_inspect.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10513 2024-05-07 01:36:17.000000 pkg_inspect-0.2.0/src/pkg_inspect/pkg_modules/pkg_metrics.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47492 2024-05-08 03:57:52.000000 pkg_inspect-0.2.0/src/pkg_inspect/pkg_modules/pkg_versions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:12:22.407659 pkg_inspect-0.2.0/src/pkg_inspect/pkg_utils/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:10:43.000000 pkg_inspect-0.2.0/src/pkg_inspect/pkg_utils/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     5907 2024-05-08 04:11:13.000000 pkg_inspect-0.2.0/src/pkg_inspect/pkg_utils/cli.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4719 2024-05-07 01:38:11.000000 pkg_inspect-0.2.0/src/pkg_inspect/pkg_utils/exception.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      611 2024-05-08 04:11:38.000000 pkg_inspect-0.2.0/src/pkg_inspect/pkg_utils/metadata.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2235 2024-05-08 04:05:15.000000 pkg_inspect-0.2.0/src/pkg_inspect/pkg_utils/util_types.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    49570 2024-05-08 04:08:51.000000 pkg_inspect-0.2.0/src/pkg_inspect/pkg_utils/utils.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:12:22.398996 pkg_inspect-0.2.0/src/pkg_inspect.egg-info/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9663 2024-05-08 04:12:22.000000 pkg_inspect-0.2.0/src/pkg_inspect.egg-info/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      815 2024-05-08 04:12:22.000000 pkg_inspect-0.2.0/src/pkg_inspect.egg-info/SOURCES.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-08 04:12:22.000000 pkg_inspect-0.2.0/src/pkg_inspect.egg-info/dependency_links.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       69 2024-05-08 04:12:22.000000 pkg_inspect-0.2.0/src/pkg_inspect.egg-info/entry_points.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-08 04:12:22.000000 pkg_inspect-0.2.0/src/pkg_inspect.egg-info/top_level.txt
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:12:22.409620 pkg_inspect-0.2.0/tests/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.2.0/tests/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2058 2024-05-04 20:17:40.000000 pkg_inspect-0.2.0/tests/test_pkg_inspect.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.372754 pkg_inspect-0.2.1/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.2.1/LICENSE.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      389 2024-05-10 23:03:20.000000 pkg_inspect-0.2.1/MANIFEST.in
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9663 2024-05-10 23:06:52.372504 pkg_inspect-0.2.1/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.2.1/README.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1037 2024-05-10 23:06:52.373522 pkg_inspect-0.2.1/setup.cfg
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.2.1/setup.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.360862 pkg_inspect-0.2.1/src/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       26 2024-05-07 01:45:11.000000 pkg_inspect-0.2.1/src/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.361276 pkg_inspect-0.2.1/src/pkg_inspect/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       56 2024-05-08 03:30:25.000000 pkg_inspect-0.2.1/src/pkg_inspect/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.364808 pkg_inspect-0.2.1/src/pkg_inspect/pkg_functions/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      337 2024-05-07 01:13:31.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_functions/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    13926 2024-05-08 04:10:58.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_functions/functions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.367262 pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      166 2024-05-06 02:47:26.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47596 2024-05-08 03:30:25.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/pkg_inspect.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10513 2024-05-07 01:36:17.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/pkg_metrics.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47497 2024-05-10 22:59:58.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/pkg_versions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.370387 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:10:43.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     5848 2024-05-10 23:06:00.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/cli.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4719 2024-05-07 01:38:11.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/exception.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      611 2024-05-10 23:01:25.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/metadata.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2235 2024-05-08 04:05:15.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/util_types.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    49570 2024-05-08 04:08:51.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/utils.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.363767 pkg_inspect-0.2.1/src/pkg_inspect.egg-info/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9663 2024-05-10 23:06:52.000000 pkg_inspect-0.2.1/src/pkg_inspect.egg-info/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      815 2024-05-10 23:06:52.000000 pkg_inspect-0.2.1/src/pkg_inspect.egg-info/SOURCES.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-10 23:06:52.000000 pkg_inspect-0.2.1/src/pkg_inspect.egg-info/dependency_links.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       69 2024-05-10 23:06:52.000000 pkg_inspect-0.2.1/src/pkg_inspect.egg-info/entry_points.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-10 23:06:52.000000 pkg_inspect-0.2.1/src/pkg_inspect.egg-info/top_level.txt
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.371606 pkg_inspect-0.2.1/tests/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.2.1/tests/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2064 2024-05-10 23:04:16.000000 pkg_inspect-0.2.1/tests/test_pkg_inspect.py
```

### Comparing `pkg_inspect-0.2.0/LICENSE.md` & `pkg_inspect-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.0/PKG-INFO` & `pkg_inspect-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg_inspect
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for inspecting Python packages and their versions.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.2.0/README.md` & `pkg_inspect-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.0/setup.cfg` & `pkg_inspect-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pkg_inspect
-version = 0.2.0
+version = 0.2.1
 author = Yousef Abuzahrieh
 author_email = yousefzahrieh17@gmail.com
 description = A package for inspecting Python packages and their versions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yousefabuz17/PkgInspect
 download_url = https://github.com/yousefabuz17/PkgInspect.git
```

### Comparing `pkg_inspect-0.2.0/src/pkg_inspect/pkg_functions/functions.py` & `pkg_inspect-0.2.1/src/pkg_inspect/pkg_functions/functions.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.0/src/pkg_inspect/pkg_modules/pkg_inspect.py` & `pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/pkg_inspect.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.0/src/pkg_inspect/pkg_modules/pkg_metrics.py` & `pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/pkg_metrics.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.0/src/pkg_inspect/pkg_modules/pkg_versions.py` & `pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/pkg_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1030,15 +1030,15 @@
             d.text
             for d in downloads_soup.find_all(
                 "div", class_="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 css-woiofv"
             )
         ]
         if return_url:
             return downloads_url
-        if (int_downloads := int(clean(total_downloads))) >= int(1e6):
+        if (int_downloads := int(clean(total_downloads, ","))) >= int(1e6):
             return f"{abbreviate_number(int_downloads)} ({total_downloads})"
         return total_downloads
 
     def _get_downloads_history(self):
         downloads_soup = self._main_request(self.DOWNLOADS_API.format(self._pkg_name))
         soup_unpacker = lambda *args, **kwargs: [
             i.text for i in downloads_soup.find_all(*args, **kwargs)
```

### Comparing `pkg_inspect-0.2.0/src/pkg_inspect/pkg_utils/cli.py` & `pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from .metadata import __version__
-from .utils import DUMMY_PATH, Any, PathOrStr, PackageVersion, CallableT, iread, partial
+from .metadata import __version__ as __current_version
+from .utils import DUMMY_PATH, Any, CallableT, PathOrStr, iread, partial
 from ..pkg_functions.functions import (
     INSPECTION_FIELDS,
     get_available_updates,
     get_installed_pythons,
     get_version_packages,
     inspect_package,
     inspect_pypi,
     pkg_version_compare,
 )
 
 from argparse import ArgumentParser
 
 
-def cli_parser(__current_version: PackageVersion = __version__):
+def cli_parser():
     """Command-line interface for 'pkg_inspect'."""
 
     # Functions for the CLI
     def _read(fp: PathOrStr) -> str:
         return iread(DUMMY_PATH / fp)
 
     def _store_true(func: CallableT, *args, **kwargs) -> partial[Any]:
@@ -33,63 +33,62 @@
     ap_true("--license", help="Display the LICENSE.md file.")
     ap_true("--options", help="Display all possible inspections options.")
     ap_true("--req", help="Display the requirements.txt file.")
     ap_true("--source", help="Display the source code of 'pkg_inspect'.")
     ap_true("--version", help="Display the current version of 'pkg_inspect'.")
     ap_true("--installed-pythons", help="Display all installed python versions.")
 
-    # Inspect Package
+    # region Inspect Package
     i_package = sub_parsers.add_parser("inspect-package", help="Inspect a package.")
     ip_true = _store_true((ip_add := i_package.add_argument))
     ip_true("--ipdoc", help="Display the documentation of 'inspect_package'.")
     ip_true("--pretty", help="Display the item in 'pretty' format.")
     ip_add("-pkg", help="Choose a package to inspect.")
     ip_add("-pyver", help="Choose a python version to inspect.")
     ip_add("-item", help="Choose an 'itemOrfile' to inspect.")
 
-    # Inspect PyPI
+    # region Inspect PyPI
     ipypi = sub_parsers.add_parser("inspect-pypi", help="Inspect a package on PyPI.")
     ipypi_true = _store_true((ipypi_add := ipypi.add_argument))
     ipypi_true("--ipdoc", help="Display the documentation of 'inspect_pypi'.")
     ipypi_true("--pretty", help="Display the item in 'pretty' format.")
     ipypi_add("-pkg", help="Choose a package to inspect.")
     ipypi_add("-pyver", help="Choose a python version to inspect.")
     ipypi_add("-pkgm", help="Choose a package manager to inspect.")
     ipypi_add("-item", help="Choose an 'itemOrfile' to inspect.")
 
-    # Retrieve Version Packages
+    # region Version Packages
     gvps = sub_parsers.add_parser(
         "get-version-packages", help="Retrieve version packages."
     )
     gvps_true = _store_true((gvps_add := gvps.add_argument))
     gvps_true("--gvpdoc", help="Display the documentation of 'get_version_packages'.")
     gvps_true("--pretty", help="Display the item in 'pretty' format.")
     gvps_add("-pyver", help="Choose a python version to inspect.")
+    
+    pvc = sub_parsers.add_parser("pkg-version-compare", help="")
+    pvc_true = _store_true((pvc_add := pvc.add_argument))
+    pvc_true("--pvcdoc", help="Display the documentation of 'pkg_version_compare'.")
+    pvc_add("-pkg", help="Choose a package to inspect.")
+    pvc_add("-fpyver", help="Choose the first python version to inspect.")
+    pvc_add("-opyver", help="Choose the second python version to inspect.")
+    pvc_add("-item", help="Choose an 'itemOrfile' to inspect.")
+    pvc_add("-opmethod", help="Choose an 'opmethod' to use.")
 
-    # Retrieve Available Updates
+    # region Available Updates
     gaup = sub_parsers.add_parser(
         "get-available-updates", help="Retrieve available updates."
     )
     gaup_true = _store_true((gaup_add := gaup.add_argument))
     gaup_true("--gaupdoc", help="Display the documentation of 'get_available_updates'.")
     gaup_true("--pretty", help="Display the item in 'pretty' format.")
     gaup_true("--include-betas", help="A flag to include beta versions.")
     gaup_add("-pkg", help="Choose a package to inspect.")
     gaup_add("-current-version", help="Choose a current version to inspect.")
 
-    # Compare Version Packages
-    pvc = sub_parsers.add_parser("pkg-version-compare", help="")
-    pvc_true = _store_true((pvc_add := pvc.add_argument))
-    pvc_true("--pvcdoc", help="Display the documentation of 'pkg_version_compare'.")
-    pvc_add("-pkg", help="Choose a package to inspect.")
-    pvc_add("-fpyver", help="Choose the first python version to inspect.")
-    pvc_add("-opyver", help="Choose the second python version to inspect.")
-    pvc_add("-item", help="Choose an 'itemOrfile' to inspect.")
-    pvc_add("-opmethod", help="Choose an 'opmethod' to use.")
-
     # Parse Arguments
     args = arg_parser.parse_args()
     if args.doc:
         return _read("README.md")
     elif args.installed_pythons:
         return get_installed_pythons()
     elif args.license:
```

### Comparing `pkg_inspect-0.2.0/src/pkg_inspect/pkg_utils/exception.py` & `pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/exception.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.0/src/pkg_inspect/pkg_utils/metadata.py` & `pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .util_types import PackageVersion
 from ..pkg_modules.pkg_versions import PkgVersions
 
 
 # Current Version
-__version__: PackageVersion = PkgVersions.parse_version("0.2.0")
+__version__: PackageVersion = PkgVersions.parse_version("0.2.1")
 
 
 # Package Metadata
 __author__ = "Yousef Abuzahrieh <yousef.zahrieh17@gmail.com"
 __copyright__ = f"Copyright © 2024, {__author__}"
 __license__ = "Apache License, Version 2.0"
 __summary__ = "A package for inspecting Python packages and their versions."
```

### Comparing `pkg_inspect-0.2.0/src/pkg_inspect/pkg_utils/util_types.py` & `pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/util_types.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.0/src/pkg_inspect/pkg_utils/utils.py` & `pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/utils.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.0/src/pkg_inspect.egg-info/PKG-INFO` & `pkg_inspect-0.2.1/src/pkg_inspect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-inspect
-Version: 0.2.0
+Version: 0.2.1
 Summary: A package for inspecting Python packages and their versions.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.2.0/src/pkg_inspect.egg-info/SOURCES.txt` & `pkg_inspect-0.2.1/src/pkg_inspect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.0/tests/test_pkg_inspect.py` & `pkg_inspect-0.2.1/tests/test_pkg_inspect.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 import unittest
 
 from src import *
 
 
 class TestPkgInspect(unittest.TestCase):
     def test_inspect_package(self):
-        # Create an instance of PipInspect
+        # Create an instance of PkgInspect
         pkg_inspect = PkgInspect(package="key_craftsman", pyversion="3.12")
 
-        # Inspect the details of the 'pipinspect' package
-        result = pkg_inspect.inspect_package(item="total_versions")
+        # Inspect the details of the 'pkgInspect' package
+        result = pkg_inspect.inspect_package(itemOrfile="total_versions")
 
         # Assert that the result is a dictionary
         self.assertIsInstance(result, int)
 
     def test_check_package(self):
-        # Create an instance of PipInspect
+        # Create an instance of PkgInspect
         pkg_inspect = PkgInspect()
 
-        # Check the 'pipinspect' package for the specified Python version
+        # Check the 'pkgInspect' package for the specified Python version
         result = pkg_inspect._check_package(
             py_version="3.12", package_name="key_craftsman"
         )
 
         # Assert that the result is True
         self.assertTrue(result)
 
     def test_package_paths(self):
-        # Create an instance of PipInspect
+        # Create an instance of PkgInspect
         pkg_inspect = PkgInspect()
 
         # Get the package paths for each Python version
         result = pkg_inspect.package_paths
 
         # Assert that the result is not empty
         self.assertIsNotNone(result)
 
     def test_package_versions(self):
-        # Create an instance of PipInspect
+        # Create an instance of PkgInspect
         pkg_inspect = PkgInspect()
 
         # Get the package versions for each Python version
         result = pkg_inspect.package_versions
 
         # Assert that the result is not empty
         self.assertIsNotNone(result)
 
     def test_pyversions(self):
-        # Create an instance of PipInspect
+        # Create an instance of PkgInspect
         pkg_inspect = PkgInspect()
 
         # Get the installed Python versions
         result = pkg_inspect.pyversions
 
         # Assert that the result is not empty
         self.assertIsNotNone(result)
 
     def test_site_packages(self):
-        # Create an instance of PipInspect
+        # Create an instance of PkgInspect
         pkg_inspect = PkgInspect()
 
         # Get the site packages for each Python version
         result = pkg_inspect.site_packages
 
         # Assert that the result is not empty
         self.assertIsNotNone(result)
```

