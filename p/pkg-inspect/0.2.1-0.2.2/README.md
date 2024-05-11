# Comparing `tmp/pkg_inspect-0.2.1.tar.gz` & `tmp/pkg_inspect-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkg_inspect-0.2.1.tar", last modified: Fri May 10 23:06:52 2024, max compression
+gzip compressed data, was "pkg_inspect-0.2.2.tar", last modified: Sat May 11 03:32:14 2024, max compression
```

## Comparing `pkg_inspect-0.2.1.tar` & `pkg_inspect-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.372754 pkg_inspect-0.2.1/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.2.1/LICENSE.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      389 2024-05-10 23:03:20.000000 pkg_inspect-0.2.1/MANIFEST.in
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9663 2024-05-10 23:06:52.372504 pkg_inspect-0.2.1/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.2.1/README.md
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1037 2024-05-10 23:06:52.373522 pkg_inspect-0.2.1/setup.cfg
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.2.1/setup.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.360862 pkg_inspect-0.2.1/src/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       26 2024-05-07 01:45:11.000000 pkg_inspect-0.2.1/src/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.361276 pkg_inspect-0.2.1/src/pkg_inspect/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       56 2024-05-08 03:30:25.000000 pkg_inspect-0.2.1/src/pkg_inspect/__init__.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.364808 pkg_inspect-0.2.1/src/pkg_inspect/pkg_functions/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      337 2024-05-07 01:13:31.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_functions/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    13926 2024-05-08 04:10:58.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_functions/functions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.367262 pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      166 2024-05-06 02:47:26.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47596 2024-05-08 03:30:25.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/pkg_inspect.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10513 2024-05-07 01:36:17.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/pkg_metrics.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47497 2024-05-10 22:59:58.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/pkg_versions.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.370387 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:10:43.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     5848 2024-05-10 23:06:00.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/cli.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4719 2024-05-07 01:38:11.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/exception.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      611 2024-05-10 23:01:25.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/metadata.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2235 2024-05-08 04:05:15.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/util_types.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    49570 2024-05-08 04:08:51.000000 pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/utils.py
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.363767 pkg_inspect-0.2.1/src/pkg_inspect.egg-info/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9663 2024-05-10 23:06:52.000000 pkg_inspect-0.2.1/src/pkg_inspect.egg-info/PKG-INFO
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      815 2024-05-10 23:06:52.000000 pkg_inspect-0.2.1/src/pkg_inspect.egg-info/SOURCES.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-10 23:06:52.000000 pkg_inspect-0.2.1/src/pkg_inspect.egg-info/dependency_links.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       69 2024-05-10 23:06:52.000000 pkg_inspect-0.2.1/src/pkg_inspect.egg-info/entry_points.txt
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-10 23:06:52.000000 pkg_inspect-0.2.1/src/pkg_inspect.egg-info/top_level.txt
-drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-10 23:06:52.371606 pkg_inspect-0.2.1/tests/
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.2.1/tests/__init__.py
--rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2064 2024-05-10 23:04:16.000000 pkg_inspect-0.2.1/tests/test_pkg_inspect.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-11 03:32:14.134623 pkg_inspect-0.2.2/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    11358 2024-04-29 00:57:53.000000 pkg_inspect-0.2.2/LICENSE.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      389 2024-05-10 23:03:20.000000 pkg_inspect-0.2.2/MANIFEST.in
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9663 2024-05-11 03:32:14.134317 pkg_inspect-0.2.2/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     8875 2024-05-02 01:30:15.000000 pkg_inspect-0.2.2/README.md
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     1037 2024-05-11 03:32:14.135337 pkg_inspect-0.2.2/setup.cfg
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       68 2024-04-29 00:59:29.000000 pkg_inspect-0.2.2/setup.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-11 03:32:14.122588 pkg_inspect-0.2.2/src/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       26 2024-05-07 01:45:11.000000 pkg_inspect-0.2.2/src/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-11 03:32:14.122927 pkg_inspect-0.2.2/src/pkg_inspect/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       56 2024-05-08 03:30:25.000000 pkg_inspect-0.2.2/src/pkg_inspect/__init__.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-11 03:32:14.126725 pkg_inspect-0.2.2/src/pkg_inspect/pkg_functions/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      337 2024-05-07 01:13:31.000000 pkg_inspect-0.2.2/src/pkg_inspect/pkg_functions/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    14027 2024-05-11 03:22:03.000000 pkg_inspect-0.2.2/src/pkg_inspect/pkg_functions/functions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-11 03:32:14.128978 pkg_inspect-0.2.2/src/pkg_inspect/pkg_modules/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      166 2024-05-06 02:47:26.000000 pkg_inspect-0.2.2/src/pkg_inspect/pkg_modules/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47596 2024-05-08 03:30:25.000000 pkg_inspect-0.2.2/src/pkg_inspect/pkg_modules/pkg_inspect.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    10513 2024-05-07 01:36:17.000000 pkg_inspect-0.2.2/src/pkg_inspect/pkg_modules/pkg_metrics.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    47740 2024-05-11 03:20:09.000000 pkg_inspect-0.2.2/src/pkg_inspect/pkg_modules/pkg_versions.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-11 03:32:14.132148 pkg_inspect-0.2.2/src/pkg_inspect/pkg_utils/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-08 04:10:43.000000 pkg_inspect-0.2.2/src/pkg_inspect/pkg_utils/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     5844 2024-05-11 03:09:03.000000 pkg_inspect-0.2.2/src/pkg_inspect/pkg_utils/cli.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     4719 2024-05-07 01:38:11.000000 pkg_inspect-0.2.2/src/pkg_inspect/pkg_utils/exception.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      611 2024-05-11 03:22:57.000000 pkg_inspect-0.2.2/src/pkg_inspect/pkg_utils/metadata.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2235 2024-05-08 04:05:15.000000 pkg_inspect-0.2.2/src/pkg_inspect/pkg_utils/util_types.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)    49679 2024-05-11 03:17:29.000000 pkg_inspect-0.2.2/src/pkg_inspect/pkg_utils/utils.py
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-11 03:32:14.125720 pkg_inspect-0.2.2/src/pkg_inspect.egg-info/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     9663 2024-05-11 03:32:13.000000 pkg_inspect-0.2.2/src/pkg_inspect.egg-info/PKG-INFO
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)      815 2024-05-11 03:32:14.000000 pkg_inspect-0.2.2/src/pkg_inspect.egg-info/SOURCES.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        1 2024-05-11 03:32:13.000000 pkg_inspect-0.2.2/src/pkg_inspect.egg-info/dependency_links.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       69 2024-05-11 03:32:14.000000 pkg_inspect-0.2.2/src/pkg_inspect.egg-info/entry_points.txt
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)       12 2024-05-11 03:32:14.000000 pkg_inspect-0.2.2/src/pkg_inspect.egg-info/top_level.txt
+drwxr-xr-x   0 yousefabuzahrieh   (501) staff       (20)        0 2024-05-11 03:32:14.133363 pkg_inspect-0.2.2/tests/
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)        0 2024-03-10 14:44:08.000000 pkg_inspect-0.2.2/tests/__init__.py
+-rw-r--r--   0 yousefabuzahrieh   (501) staff       (20)     2064 2024-05-11 02:19:40.000000 pkg_inspect-0.2.2/tests/test_pkg_inspect.py
```

### Comparing `pkg_inspect-0.2.1/LICENSE.md` & `pkg_inspect-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.1/PKG-INFO` & `pkg_inspect-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg_inspect
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package for inspecting Python packages and their versions.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.2.1/README.md` & `pkg_inspect-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.1/setup.cfg` & `pkg_inspect-0.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pkg_inspect
-version = 0.2.1
+version = 0.2.2
 author = Yousef Abuzahrieh
 author_email = yousefzahrieh17@gmail.com
 description = A package for inspecting Python packages and their versions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/yousefabuz17/PkgInspect
 download_url = https://github.com/yousefabuz17/PkgInspect.git
```

### Comparing `pkg_inspect-0.2.1/src/pkg_inspect/pkg_functions/functions.py` & `pkg_inspect-0.2.2/src/pkg_inspect/pkg_functions/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,25 +23,23 @@
 """
 
 
 from ..pkg_modules import PkgInspect, PkgVersions
 from ..pkg_utils.exception import PkgException, RedPkgE
 from ..pkg_utils.util_types import (
     DateTimeAndVersion,
-    Iterable,
     Literal,
     Optional,
     PyPIOptionsT,
     TupleOfPkgVersions,
     Union,
 )
 from ..pkg_utils.utils import (
     BASE_EXCEPTIONS,
-    alter_if_string,
-    equal_,
+    best_match,
     filter_empty,
     find_best_match,
     get_properties,
     has_decorators,
     is_class,
     is_function,
     partial,
@@ -139,16 +137,21 @@
         return _PkgI(package, pyversion).inspect_package(itemOrfile)
     except ModuleNotFoundError as _mnfe_error:
         raise RedPkgE(filter_empty(_mnfe_error.args[0].splitlines())[0])
     except (*BASE_EXCEPTIONS, PkgException) as _any_e:
         try:
             return inspect_pypi(package, package_manager, item=itemOrfile)
         except PkgException as pkg_error:
+            e = (
+                _any_e
+                if best_match(_any_e, pkg_error.args)
+                else f"{_any_e}\n{pkg_error.args[0]}"
+            )
             raise RedPkgE(
-                f"{_any_e}\n{pkg_error.args[0]}",
+                e,
                 "If inspecting a package on PyPI, please refer to the 'inspect_pypi' function for more information.",
             )
 
 
 @__doc_handler(add_doc=False)
 @__prettyprint()
 def inspect_pypi(
```

### Comparing `pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/pkg_inspect.py` & `pkg_inspect-0.2.2/src/pkg_inspect/pkg_modules/pkg_inspect.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/pkg_metrics.py` & `pkg_inspect-0.2.2/src/pkg_inspect/pkg_modules/pkg_metrics.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.1/src/pkg_inspect/pkg_modules/pkg_versions.py` & `pkg_inspect-0.2.2/src/pkg_inspect/pkg_modules/pkg_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1021,24 +1021,33 @@
         )
 
     def _get_dtv(self, method: MinOrMax = max) -> TupleDoubleStr:
         """Return the initial or latest release date and version of the package."""
         return [min, max][method == max](self._version_history(), key=itemgetter(1))
 
     def _get_total_downloads(self, return_url: bool = False) -> str:
-        downloads_soup = self._main_request(self.DOWNLOADS_API.format(self._pkg_name))
-        downloads_url, total_downloads = [
-            d.text
-            for d in downloads_soup.find_all(
-                "div", class_="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 css-woiofv"
-            )
-        ]
+        downloads_soup = self._main_request(
+            (downloads_url := self.DOWNLOADS_API.format(self._pkg_name))
+        )
         if return_url:
             return downloads_url
-        if (int_downloads := int(clean(total_downloads, ","))) >= int(1e6):
+        
+        try:
+            _url, total_downloads = [
+                d.text
+                for d in downloads_soup.find_all(
+                    "div",
+                    class_="MuiGrid-root MuiGrid-item MuiGrid-grid-xs-12 css-woiofv",
+                )
+            ]
+        except ValueError:
+            s = "url-webpage" if return_url else "total-downloads"
+            raise PkgException(f"Failed to retrieve the {s} from {downloads_url!r}.")
+
+        if (int_downloads := int(clean(total_downloads, ","))) >= million:
             return f"{abbreviate_number(int_downloads)} ({total_downloads})"
         return total_downloads
 
     def _get_downloads_history(self):
         downloads_soup = self._main_request(self.DOWNLOADS_API.format(self._pkg_name))
         soup_unpacker = lambda *args, **kwargs: [
             i.text for i in downloads_soup.find_all(*args, **kwargs)
@@ -1077,15 +1086,15 @@
                             else i
                             for i in version_columns
                         ),
                         v,
                     )
                 ),
                 "sum": (f"{sum_v:,}", abbreviate_number(sum_v))
-                if (sum_v := sum(v)) >= (million := int(1e6))
+                if (sum_v := sum(v)) >= million
                 else sum_v,
                 "total_downloads": (td, abbreviate_number(td))
                 if (td := int(total_downloads[idx])) >= million
                 else td,
             }
             for idx, (k, v) in enumerate(dh_dict.items())
         }
@@ -1196,13 +1205,13 @@
         # Get the updates after the current version
         updates = version_h[current_v_idx + 1 :]
         if not updates or self.is_latest(current_v):
             updates = None
             # Print a warning message if no updates are found
             # or if the specified version is the latest version.
             print(
-                f"\033[1;33mNo updates were found. The specified version ({current_v!r}) appears to be the latest.\033[0m"
+                f"\033[1;33mNo updates were found. ({current_v!r}) appears to be the latest.\033[0m"
             )
         return updates
 
 
 # endregion
```

### Comparing `pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/cli.py` & `pkg_inspect-0.2.2/src/pkg_inspect/pkg_utils/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     gvps = sub_parsers.add_parser(
         "get-version-packages", help="Retrieve version packages."
     )
     gvps_true = _store_true((gvps_add := gvps.add_argument))
     gvps_true("--gvpdoc", help="Display the documentation of 'get_version_packages'.")
     gvps_true("--pretty", help="Display the item in 'pretty' format.")
     gvps_add("-pyver", help="Choose a python version to inspect.")
-    
+
     pvc = sub_parsers.add_parser("pkg-version-compare", help="")
     pvc_true = _store_true((pvc_add := pvc.add_argument))
     pvc_true("--pvcdoc", help="Display the documentation of 'pkg_version_compare'.")
     pvc_add("-pkg", help="Choose a package to inspect.")
     pvc_add("-fpyver", help="Choose the first python version to inspect.")
     pvc_add("-opyver", help="Choose the second python version to inspect.")
     pvc_add("-item", help="Choose an 'itemOrfile' to inspect.")
```

### Comparing `pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/exception.py` & `pkg_inspect-0.2.2/src/pkg_inspect/pkg_utils/exception.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/metadata.py` & `pkg_inspect-0.2.2/src/pkg_inspect/pkg_utils/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .util_types import PackageVersion
 from ..pkg_modules.pkg_versions import PkgVersions
 
 
 # Current Version
-__version__: PackageVersion = PkgVersions.parse_version("0.2.1")
+__version__: PackageVersion = PkgVersions.parse_version("0.2.2")
 
 
 # Package Metadata
 __author__ = "Yousef Abuzahrieh <yousef.zahrieh17@gmail.com"
 __copyright__ = f"Copyright © 2024, {__author__}"
 __license__ = "Apache License, Version 2.0"
 __summary__ = "A package for inspecting Python packages and their versions."
```

### Comparing `pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/util_types.py` & `pkg_inspect-0.2.2/src/pkg_inspect/pkg_utils/util_types.py`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.1/src/pkg_inspect/pkg_utils/utils.py` & `pkg_inspect-0.2.2/src/pkg_inspect/pkg_utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,16 +211,16 @@
         return getattr(operator, comparison_ops.get(opm, opmethod), None)
 
 
 # Default operator methods
 add_ = get_opmethod("+")
 multiply_ = get_opmethod("*")
 pow_ = get_opmethod("**")
-equal_ = get_opmethod("==")
-lessthan_ = get_opmethod("<")
+eq_ = get_opmethod("==")
+lt_ = get_opmethod("<")
 
 
 # region InspectUtils
 def is_function(c):
     """This function checks if the specified object is a function."""
     return inspect.isfunction(c)
 
@@ -1181,15 +1181,15 @@
             num = float(num)
         except ValueError:
             raise PkgException(f"The specified value {num!r} must be an integer value.")
 
     results: tuple[str, float, int] = next(
         (f"{(total := num/v):.3f} {k[:2] if symbol_only else k}", total, num)
         for k, v in bytes_unit_chart().items()
-        if lessthan_(num / BYTES_BASE, v)
+        if lt_(num / BYTES_BASE, v)
     )
     if not total:
         # Return None if the total size was not calculated
         return
     if total_only:
         # Return the total size only
         return total
@@ -1353,15 +1353,15 @@
         - `prefix` (str): The prefix to remove from the string.
 
     #### Returns:
         - `str`: The string with the prefix removed.
     """
     try:
         return s.removeprefix(prefix)
-    except BASE_EXCEPTIONS + (AttributeError,):
+    except (*BASE_EXCEPTIONS, AttributeError,):
         return s[s.startswith(prefix) and len(prefix) :]
 
 
 def best_match(
     query: str, choices: Iterable[str], *, min_ratio: int = None
 ) -> Union[str, None]:
     """
@@ -1467,18 +1467,20 @@
 def abbreviate_number(num: Union[int, str]):
     """Converts a large number into an abbreviated form with common terms like Thousand, Million, Billion, etc."""
     # Remove commas and convert to integer
     if isinstance(num, str):
         num = int(clean(num))
 
     # Define abbreviations and their respective scales
+    global million, billion, trillion
+    
     abbrevs = (
-        (1_000_000_000_000, "Trillion"),
-        (1_000_000_000, "Billion"),
-        (1_000_000, "Million"),
+        ((trillion := 1_000_000_000_000), "Trillion"),
+        ((billion := 1_000_000_000), "Billion"),
+        ((million := 1_000_000), "Million"),
     )
 
     for scale, abbrev in abbrevs:
         if num >= scale:
             # Convert to the appropriate scale and round to two decimal places
             value = num / scale
             # If rounded value is whole number, return it without decimal
@@ -1525,11 +1527,11 @@
 
 # endregion
 
 __all__ = tuple(
     k
     for k, v in globals().items()
     # Constants, not private, and is a class
-    if any((k.isupper(), not k.startswith("_"), is_class(k)))
+    if any((k.isupper(), not k.startswith("_"), is_class(k), k in ("million", "billion", "trillion")))
     # Functions and not decorators
     and any((is_function(v), not has_decorators(v, "_cached_property")))
 )
```

### Comparing `pkg_inspect-0.2.1/src/pkg_inspect.egg-info/PKG-INFO` & `pkg_inspect-0.2.2/src/pkg_inspect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkg-inspect
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package for inspecting Python packages and their versions.
 Home-page: https://github.com/yousefabuz17/PkgInspect
 Download-URL: https://github.com/yousefabuz17/PkgInspect.git
 Author: Yousef Abuzahrieh
 Author-email: yousefzahrieh17@gmail.com
 License: Apache Software License
 Platform: Windows
```

### Comparing `pkg_inspect-0.2.1/src/pkg_inspect.egg-info/SOURCES.txt` & `pkg_inspect-0.2.2/src/pkg_inspect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkg_inspect-0.2.1/tests/test_pkg_inspect.py` & `pkg_inspect-0.2.2/tests/test_pkg_inspect.py`

 * *Files identical despite different names*

