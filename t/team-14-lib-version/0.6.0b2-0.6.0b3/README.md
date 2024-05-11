# Comparing `tmp/team_14_lib_version-0.6.0b2.tar.gz` & `tmp/team_14_lib_version-0.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "team_14_lib_version-0.6.0b2.tar", last modified: Sat May 11 11:27:32 2024, max compression
+gzip compressed data, was "team_14_lib_version-0.6.0b3.tar", last modified: Sat May 11 12:17:05 2024, max compression
```

## Comparing `team_14_lib_version-0.6.0b2.tar` & `team_14_lib_version-0.6.0b3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:32.834039 team_14_lib_version-0.6.0b2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:32.830039 team_14_lib_version-0.6.0b2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:32.830039 team_14_lib_version-0.6.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-11 11:27:16.000000 team_14_lib_version-0.6.0b2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 11:27:16.000000 team_14_lib_version-0.6.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 11:27:16.000000 team_14_lib_version-0.6.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-11 11:27:32.834039 team_14_lib_version-0.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-11 11:27:16.000000 team_14_lib_version-0.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:32.830039 team_14_lib_version-0.6.0b2/lib-version/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-11 11:27:16.000000 team_14_lib_version-0.6.0b2/lib-version/VersionUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:16.000000 team_14_lib_version-0.6.0b2/lib-version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-11 11:27:32.000000 team_14_lib_version-0.6.0b2/lib-version/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-11 11:27:16.000000 team_14_lib_version-0.6.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-11 11:27:16.000000 team_14_lib_version-0.6.0b2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 11:27:32.834039 team_14_lib_version-0.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-11 11:27:16.000000 team_14_lib_version-0.6.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:27:32.834039 team_14_lib_version-0.6.0b2/team_14_lib_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-11 11:27:32.000000 team_14_lib_version-0.6.0b2/team_14_lib_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-11 11:27:32.000000 team_14_lib_version-0.6.0b2/team_14_lib_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 11:27:32.000000 team_14_lib_version-0.6.0b2/team_14_lib_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-11 11:27:32.000000 team_14_lib_version-0.6.0b2/team_14_lib_version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-11 11:27:32.000000 team_14_lib_version-0.6.0b2/team_14_lib_version.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:17:05.111609 team_14_lib_version-0.6.0b3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:17:05.107609 team_14_lib_version-0.6.0b3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:17:05.107609 team_14_lib_version-0.6.0b3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-11 12:17:05.111609 team_14_lib_version-0.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:17:05.107609 team_14_lib_version-0.6.0b3/libversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/libversion/VersionUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/libversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-11 12:17:05.000000 team_14_lib_version-0.6.0b3/libversion/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:17:05.111609 team_14_lib_version-0.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-11 12:16:47.000000 team_14_lib_version-0.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:17:05.111609 team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-11 12:17:05.000000 team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-11 12:17:05.000000 team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:17:05.000000 team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 12:17:05.000000 team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 12:17:05.000000 team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/top_level.txt
```

### Comparing `team_14_lib_version-0.6.0b2/.github/workflows/release.yml` & `team_14_lib_version-0.6.0b3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `team_14_lib_version-0.6.0b2/LICENSE` & `team_14_lib_version-0.6.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `team_14_lib_version-0.6.0b2/PKG-INFO` & `team_14_lib_version-0.6.0b3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: team-14-lib-version
-Version: 0.6.0b2
+Version: 0.6.0b3
 Summary: version aware library
 Home-page: https://github.com/remla2024-team14/lib-version
 Author: Team 14
 Author-email: justinluu2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: flask
-Requires-Dist: flask-cors
+Requires-Dist: importlib
 Provides-Extra: dev
 Requires-Dist: twine>=4.0.2; extra == "dev"
 
 # lib-version
 A version-aware library consumed by the URL fishing detection application service
 The library parses the version from the metadata in the package.
```

### Comparing `team_14_lib_version-0.6.0b2/setup.py` & `team_14_lib_version-0.6.0b3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     description='version aware library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Team 14',
     author_email='justinluu2000@gmail.com',
     url='https://github.com/remla2024-team14/lib-version',
     install_requires=[
-        'flask',  'flask-cors'
+        'importlib'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     extras_require={'dev': ['twine>=4.0.2']},
```

### Comparing `team_14_lib_version-0.6.0b2/team_14_lib_version.egg-info/PKG-INFO` & `team_14_lib_version-0.6.0b3/team_14_lib_version.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: team-14-lib-version
-Version: 0.6.0b2
+Version: 0.6.0b3
 Summary: version aware library
 Home-page: https://github.com/remla2024-team14/lib-version
 Author: Team 14
 Author-email: justinluu2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: flask
-Requires-Dist: flask-cors
+Requires-Dist: importlib
 Provides-Extra: dev
 Requires-Dist: twine>=4.0.2; extra == "dev"
 
 # lib-version
 A version-aware library consumed by the URL fishing detection application service
 The library parses the version from the metadata in the package.
```

