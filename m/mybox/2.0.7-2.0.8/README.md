# Comparing `tmp/mybox-2.0.7.tar.gz` & `tmp/mybox-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mybox-2.0.7.tar", max compression
+gzip compressed data, was "mybox-2.0.8.tar", max compression
```

## Comparing `mybox-2.0.7.tar` & `mybox-2.0.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    34916 2024-05-03 11:37:38.086311 mybox-2.0.7/LICENSE.md
--rw-r--r--   0        0        0     1447 2024-05-03 11:37:38.086311 mybox-2.0.7/README.md
--rw-r--r--   0        0        0        0 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/__init__.py
--rw-r--r--   0        0        0     2621 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/compute.py
--rw-r--r--   0        0        0      741 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/configparser.py
--rw-r--r--   0        0        0    10638 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/driver.py
--rw-r--r--   0        0        0     3325 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/extractor.py
--rw-r--r--   0        0        0     2800 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/filters.py
--rw-r--r--   0        0        0     1302 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/main.py
--rw-r--r--   0        0        0     3098 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/manager.py
--rw-r--r--   0        0        0     1137 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/__init__.py
--rw-r--r--   0        0        0     4064 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/archive.py
--rw-r--r--   0        0        0     2055 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/base.py
--rw-r--r--   0        0        0     1008 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/brew_repo.py
--rw-r--r--   0        0        0     1957 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/clone.py
--rw-r--r--   0        0        0      339 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/destination.py
--rw-r--r--   0        0        0     4714 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/github.py
--rw-r--r--   0        0        0    10013 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/installer.py
--rw-r--r--   0        0        0     1939 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/links.py
--rw-r--r--   0        0        0     4774 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/manual.py
--rw-r--r--   0        0        0      858 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/manual_version.py
--rw-r--r--   0        0        0     1793 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/npm.py
--rw-r--r--   0        0        0     2963 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/pipx.py
--rw-r--r--   0        0        0      500 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/root.py
--rw-r--r--   0        0        0     1853 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/shell.py
--rw-r--r--   0        0        0     2389 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/system.py
--rw-r--r--   0        0        0      959 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/url.py
--rw-r--r--   0        0        0     1762 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/package/yum_repo.py
--rw-r--r--   0        0        0     2900 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/parallel.py
--rw-r--r--   0        0        0      156 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/state/__init__.py
--rw-r--r--   0        0        0     3677 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/state/base.py
--rw-r--r--   0        0        0     1546 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/state/db.py
--rw-r--r--   0        0        0      315 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/state/installed.py
--rw-r--r--   0        0        0      160 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/state/version.py
--rw-r--r--   0        0        0     2176 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/tracker.py
--rw-r--r--   0        0        0     3969 2024-05-03 11:37:38.086311 mybox-2.0.7/mybox/utils.py
--rw-r--r--   0        0        0     2107 2024-05-03 11:38:10.366717 mybox-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 mybox-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0    34916 2024-05-11 01:03:43.982409 mybox-2.0.8/LICENSE.md
+-rw-r--r--   0        0        0     1447 2024-05-11 01:03:43.982409 mybox-2.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 01:03:43.982409 mybox-2.0.8/mybox/__init__.py
+-rw-r--r--   0        0        0     2621 2024-05-11 01:03:43.982409 mybox-2.0.8/mybox/compute.py
+-rw-r--r--   0        0        0      741 2024-05-11 01:03:43.982409 mybox-2.0.8/mybox/configparser.py
+-rw-r--r--   0        0        0    10638 2024-05-11 01:03:43.982409 mybox-2.0.8/mybox/driver.py
+-rw-r--r--   0        0        0     3325 2024-05-11 01:03:43.982409 mybox-2.0.8/mybox/extractor.py
+-rw-r--r--   0        0        0     2800 2024-05-11 01:03:43.982409 mybox-2.0.8/mybox/filters.py
+-rw-r--r--   0        0        0     1302 2024-05-11 01:03:43.982409 mybox-2.0.8/mybox/main.py
+-rw-r--r--   0        0        0     3098 2024-05-11 01:03:43.982409 mybox-2.0.8/mybox/manager.py
+-rw-r--r--   0        0        0     1137 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/__init__.py
+-rw-r--r--   0        0        0     4064 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/archive.py
+-rw-r--r--   0        0        0     2055 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/base.py
+-rw-r--r--   0        0        0     1008 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/brew_repo.py
+-rw-r--r--   0        0        0     1957 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/clone.py
+-rw-r--r--   0        0        0      339 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/destination.py
+-rw-r--r--   0        0        0     4714 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/github.py
+-rw-r--r--   0        0        0    10013 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/installer.py
+-rw-r--r--   0        0        0     1939 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/links.py
+-rw-r--r--   0        0        0     4774 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/manual.py
+-rw-r--r--   0        0        0      858 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/manual_version.py
+-rw-r--r--   0        0        0     1793 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/npm.py
+-rw-r--r--   0        0        0     2963 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/pipx.py
+-rw-r--r--   0        0        0      500 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/root.py
+-rw-r--r--   0        0        0     1853 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/shell.py
+-rw-r--r--   0        0        0     2389 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/system.py
+-rw-r--r--   0        0        0      959 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/url.py
+-rw-r--r--   0        0        0     1762 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/package/yum_repo.py
+-rw-r--r--   0        0        0     2900 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/parallel.py
+-rw-r--r--   0        0        0      156 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/state/__init__.py
+-rw-r--r--   0        0        0     3677 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/state/base.py
+-rw-r--r--   0        0        0     1546 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/state/db.py
+-rw-r--r--   0        0        0      315 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/state/installed.py
+-rw-r--r--   0        0        0      160 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/state/version.py
+-rw-r--r--   0        0        0     2176 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/tracker.py
+-rw-r--r--   0        0        0     3969 2024-05-11 01:03:43.986409 mybox-2.0.8/mybox/utils.py
+-rw-r--r--   0        0        0     2062 2024-05-11 01:04:20.386613 mybox-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mybox-2.0.8/PKG-INFO
```

### Comparing `mybox-2.0.7/LICENSE.md` & `mybox-2.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/README.md` & `mybox-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/compute.py` & `mybox-2.0.8/mybox/compute.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/configparser.py` & `mybox-2.0.8/mybox/configparser.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/driver.py` & `mybox-2.0.8/mybox/driver.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/extractor.py` & `mybox-2.0.8/mybox/extractor.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/filters.py` & `mybox-2.0.8/mybox/filters.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/main.py` & `mybox-2.0.8/mybox/main.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/manager.py` & `mybox-2.0.8/mybox/manager.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/__init__.py` & `mybox-2.0.8/mybox/package/__init__.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/archive.py` & `mybox-2.0.8/mybox/package/archive.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/base.py` & `mybox-2.0.8/mybox/package/base.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/brew_repo.py` & `mybox-2.0.8/mybox/package/brew_repo.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/clone.py` & `mybox-2.0.8/mybox/package/clone.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/github.py` & `mybox-2.0.8/mybox/package/github.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/installer.py` & `mybox-2.0.8/mybox/package/installer.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/links.py` & `mybox-2.0.8/mybox/package/links.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/manual.py` & `mybox-2.0.8/mybox/package/manual.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/manual_version.py` & `mybox-2.0.8/mybox/package/manual_version.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/npm.py` & `mybox-2.0.8/mybox/package/npm.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/pipx.py` & `mybox-2.0.8/mybox/package/pipx.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/shell.py` & `mybox-2.0.8/mybox/package/shell.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/system.py` & `mybox-2.0.8/mybox/package/system.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/url.py` & `mybox-2.0.8/mybox/package/url.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/package/yum_repo.py` & `mybox-2.0.8/mybox/package/yum_repo.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/parallel.py` & `mybox-2.0.8/mybox/parallel.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/state/base.py` & `mybox-2.0.8/mybox/state/base.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/state/db.py` & `mybox-2.0.8/mybox/state/db.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/tracker.py` & `mybox-2.0.8/mybox/tracker.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/mybox/utils.py` & `mybox-2.0.8/mybox/utils.py`

 * *Files identical despite different names*

### Comparing `mybox-2.0.7/pyproject.toml` & `mybox-2.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [tool.poetry]
 name = "mybox"
-version = "2.0.7"
+version = "2.0.8"
 description = "Manage the configuration and tools on your workstation without bothering the OS too much"
 readme = "README.md"
 repository = "https://github.com/koterpillar/mybox"
 authors = ["Alexey Kotlyarov <a@koterpillar.com>"]
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 pydantic = "^2.7.1"
-python = ">=3.11,<3.13"
+python = "^3.11"
 PyYAML = "^6.0.1"
 requests = "^2.31.0"
 trio = "^0.25.0"
 tqdm = "^4.66.4"
 typed-argparse = "^0.3.1"
 jsonpath-ng = "^1.6.1"
 beautifulsoup4 = "^4.12.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.2"
 coverage = {extras = ["toml"], version = "^7.4.4"}
-coveralls = "^4.0.0"
 fawltydeps = "^0.15.0"
 isort = "^5.13.2"
 mypy = "^1.10.0"
 pylint = "^3.1.0"
 pylint-pydantic = "^0.3.2"
 pytest = "^8.2.0"
 pytest-trio = "^0.8.0"
@@ -36,15 +35,15 @@
 types-tqdm = "^4.66.0.4"
 
 [tool.poetry.scripts]
 mybox = "mybox.main:sync_main"
 
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.9.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 disable_error_code = [
@@ -74,15 +73,14 @@
 output-format = "colorized"
 
 [tool.fawltydeps]
 ignore_undeclared = ["_typeshed"]
 ignore_unused = [
     "black",
     "coverage",
-    "coveralls",
     "fawltydeps",
     "isort",
     "mypy",
     "pylint",
     "pylint-pydantic",
     "pytest-trio",
 ]
```

### Comparing `mybox-2.0.7/PKG-INFO` & `mybox-2.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mybox
-Version: 2.0.7
+Version: 2.0.8
 Summary: Manage the configuration and tools on your workstation without bothering the OS too much
 Home-page: https://github.com/koterpillar/mybox
 License: GPL-3.0-or-later
 Author: Alexey Kotlyarov
 Author-email: a@koterpillar.com
-Requires-Python: >=3.11,<3.13
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: jsonpath-ng (>=1.6.1,<2.0.0)
```

