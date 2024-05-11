# Comparing `tmp/team_14_lib_version-0.6.0b0.tar.gz` & `tmp/team_14_lib_version-0.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "team_14_lib_version-0.6.0b0.tar", last modified: Sat May 11 10:19:56 2024, max compression
+gzip compressed data, was "team_14_lib_version-0.6.0b1.tar", last modified: Sat May 11 11:07:58 2024, max compression
```

## Comparing `team_14_lib_version-0.6.0b0.tar` & `team_14_lib_version-0.6.0b1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:19:56.439463 team_14_lib_version-0.6.0b0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:19:56.435464 team_14_lib_version-0.6.0b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:19:56.435464 team_14_lib_version-0.6.0b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-11 10:19:44.000000 team_14_lib_version-0.6.0b0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 10:19:44.000000 team_14_lib_version-0.6.0b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 10:19:44.000000 team_14_lib_version-0.6.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-11 10:19:56.439463 team_14_lib_version-0.6.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-11 10:19:44.000000 team_14_lib_version-0.6.0b0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-11 10:19:44.000000 team_14_lib_version-0.6.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 10:19:44.000000 team_14_lib_version-0.6.0b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 10:19:56.439463 team_14_lib_version-0.6.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-11 10:19:44.000000 team_14_lib_version-0.6.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:19:56.435464 team_14_lib_version-0.6.0b0/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-11 10:19:44.000000 team_14_lib_version-0.6.0b0/src/VersionUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 10:19:44.000000 team_14_lib_version-0.6.0b0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-11 10:19:56.000000 team_14_lib_version-0.6.0b0/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 10:19:56.435464 team_14_lib_version-0.6.0b0/team_14_lib_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-11 10:19:56.000000 team_14_lib_version-0.6.0b0/team_14_lib_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-11 10:19:56.000000 team_14_lib_version-0.6.0b0/team_14_lib_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 10:19:56.000000 team_14_lib_version-0.6.0b0/team_14_lib_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-11 10:19:56.000000 team_14_lib_version-0.6.0b0/team_14_lib_version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-11 10:19:56.000000 team_14_lib_version-0.6.0b0/team_14_lib_version.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-11 10:19:44.000000 team_14_lib_version-0.6.0b0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:07:58.374448 team_14_lib_version-0.6.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:07:58.370448 team_14_lib_version-0.6.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:07:58.370448 team_14_lib_version-0.6.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-11 11:07:43.000000 team_14_lib_version-0.6.0b1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 11:07:43.000000 team_14_lib_version-0.6.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 11:07:43.000000 team_14_lib_version-0.6.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-11 11:07:58.370448 team_14_lib_version-0.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-11 11:07:43.000000 team_14_lib_version-0.6.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-11 11:07:43.000000 team_14_lib_version-0.6.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-11 11:07:43.000000 team_14_lib_version-0.6.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 11:07:58.374448 team_14_lib_version-0.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-11 11:07:43.000000 team_14_lib_version-0.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:07:58.370448 team_14_lib_version-0.6.0b1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-11 11:07:43.000000 team_14_lib_version-0.6.0b1/src/VersionUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 11:07:43.000000 team_14_lib_version-0.6.0b1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-11 11:07:58.000000 team_14_lib_version-0.6.0b1/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:07:58.370448 team_14_lib_version-0.6.0b1/team_14_lib_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-11 11:07:58.000000 team_14_lib_version-0.6.0b1/team_14_lib_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-11 11:07:58.000000 team_14_lib_version-0.6.0b1/team_14_lib_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 11:07:58.000000 team_14_lib_version-0.6.0b1/team_14_lib_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-11 11:07:58.000000 team_14_lib_version-0.6.0b1/team_14_lib_version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-11 11:07:58.000000 team_14_lib_version-0.6.0b1/team_14_lib_version.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-11 11:07:43.000000 team_14_lib_version-0.6.0b1/version.txt
```

### Comparing `team_14_lib_version-0.6.0b0/.github/workflows/release.yml` & `team_14_lib_version-0.6.0b1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `team_14_lib_version-0.6.0b0/LICENSE` & `team_14_lib_version-0.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `team_14_lib_version-0.6.0b0/PKG-INFO` & `team_14_lib_version-0.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: team-14-lib-version
-Version: 0.6.0b0
+Version: 0.6.0b1
 Summary: version aware library
 Home-page: https://github.com/remla2024-team14/lib-version
 Author: Team 14
 Author-email: justinluu2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `team_14_lib_version-0.6.0b0/README.md` & `team_14_lib_version-0.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `team_14_lib_version-0.6.0b0/setup.py` & `team_14_lib_version-0.6.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `team_14_lib_version-0.6.0b0/team_14_lib_version.egg-info/PKG-INFO` & `team_14_lib_version-0.6.0b1/team_14_lib_version.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: team-14-lib-version
-Version: 0.6.0b0
+Version: 0.6.0b1
 Summary: version aware library
 Home-page: https://github.com/remla2024-team14/lib-version
 Author: Team 14
 Author-email: justinluu2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```
