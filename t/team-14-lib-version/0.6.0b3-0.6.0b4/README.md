# Comparing `tmp/team_14_lib_version-0.6.0b3.tar.gz` & `tmp/team_14_lib_version-0.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "team_14_lib_version-0.6.0b3.tar", last modified: Sat May 11 12:17:05 2024, max compression
+gzip compressed data, was "team_14_lib_version-0.6.0b4.tar", last modified: Sat May 11 12:20:49 2024, max compression
```

## Comparing `team_14_lib_version-0.6.0b3.tar` & `team_14_lib_version-0.6.0b4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:17:05.111609 team_14_lib_version-0.6.0b3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:17:05.107609 team_14_lib_version-0.6.0b3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:17:05.107609 team_14_lib_version-0.6.0b3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-11 12:17:05.111609 team_14_lib_version-0.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:17:05.107609 team_14_lib_version-0.6.0b3/libversion/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/libversion/VersionUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/libversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-11 12:17:05.000000 team_14_lib_version-0.6.0b3/libversion/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:17:05.111609 team_14_lib_version-0.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:17:05.111609 team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-11 12:17:05.000000 team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-11 12:17:05.000000 team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:17:05.000000 team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 12:17:05.000000 team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 12:17:05.000000 team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:20:49.045183 team_14_lib_version-0.6.0b4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:20:49.041183 team_14_lib_version-0.6.0b4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:20:49.041183 team_14_lib_version-0.6.0b4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-11 12:20:30.000000 team_14_lib_version-0.6.0b4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 12:20:30.000000 team_14_lib_version-0.6.0b4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 12:20:30.000000 team_14_lib_version-0.6.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-11 12:20:49.045183 team_14_lib_version-0.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-11 12:20:30.000000 team_14_lib_version-0.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:20:49.045183 team_14_lib_version-0.6.0b4/libversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-11 12:20:30.000000 team_14_lib_version-0.6.0b4/libversion/VersionUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:20:30.000000 team_14_lib_version-0.6.0b4/libversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-11 12:20:48.000000 team_14_lib_version-0.6.0b4/libversion/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-11 12:20:30.000000 team_14_lib_version-0.6.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 12:20:30.000000 team_14_lib_version-0.6.0b4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:20:49.045183 team_14_lib_version-0.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-11 12:20:30.000000 team_14_lib_version-0.6.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:20:49.045183 team_14_lib_version-0.6.0b4/team_14_lib_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-11 12:20:49.000000 team_14_lib_version-0.6.0b4/team_14_lib_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-11 12:20:49.000000 team_14_lib_version-0.6.0b4/team_14_lib_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:20:49.000000 team_14_lib_version-0.6.0b4/team_14_lib_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 12:20:49.000000 team_14_lib_version-0.6.0b4/team_14_lib_version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 12:20:49.000000 team_14_lib_version-0.6.0b4/team_14_lib_version.egg-info/top_level.txt
```

### Comparing `team_14_lib_version-0.6.0b3/LICENSE` & `team_14_lib_version-0.6.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `team_14_lib_version-0.6.0b3/PKG-INFO` & `team_14_lib_version-0.6.0b4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: team-14-lib-version
-Version: 0.6.0b3
+Version: 0.6.0b4
 Summary: version aware library
 Home-page: https://github.com/remla2024-team14/lib-version
 Author: Team 14
 Author-email: justinluu2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `team_14_lib_version-0.6.0b3/setup.py` & `team_14_lib_version-0.6.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/PKG-INFO` & `team_14_lib_version-0.6.0b4/team_14_lib_version.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: team-14-lib-version
-Version: 0.6.0b3
+Version: 0.6.0b4
 Summary: version aware library
 Home-page: https://github.com/remla2024-team14/lib-version
 Author: Team 14
 Author-email: justinluu2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

