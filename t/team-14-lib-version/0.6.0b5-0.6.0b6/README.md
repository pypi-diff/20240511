# Comparing `tmp/team_14_lib_version-0.6.0b5.tar.gz` & `tmp/team_14_lib_version-0.6.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "team_14_lib_version-0.6.0b5.tar", last modified: Sat May 11 12:29:20 2024, max compression
+gzip compressed data, was "team_14_lib_version-0.6.0b6.tar", last modified: Sat May 11 12:37:31 2024, max compression
```

## Comparing `team_14_lib_version-0.6.0b5.tar` & `team_14_lib_version-0.6.0b6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:29:20.736574 team_14_lib_version-0.6.0b5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:29:20.732574 team_14_lib_version-0.6.0b5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:29:20.736574 team_14_lib_version-0.6.0b5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-11 12:29:05.000000 team_14_lib_version-0.6.0b5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 12:29:05.000000 team_14_lib_version-0.6.0b5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 12:29:05.000000 team_14_lib_version-0.6.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-11 12:29:20.736574 team_14_lib_version-0.6.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-11 12:29:05.000000 team_14_lib_version-0.6.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:29:20.736574 team_14_lib_version-0.6.0b5/libversion/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-11 12:29:05.000000 team_14_lib_version-0.6.0b5/libversion/VersionUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:29:05.000000 team_14_lib_version-0.6.0b5/libversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-11 12:29:20.000000 team_14_lib_version-0.6.0b5/libversion/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-11 12:29:05.000000 team_14_lib_version-0.6.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-11 12:29:05.000000 team_14_lib_version-0.6.0b5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:29:20.736574 team_14_lib_version-0.6.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-11 12:29:05.000000 team_14_lib_version-0.6.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:29:20.736574 team_14_lib_version-0.6.0b5/team_14_lib_version.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-11 12:29:20.000000 team_14_lib_version-0.6.0b5/team_14_lib_version.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-11 12:29:20.000000 team_14_lib_version-0.6.0b5/team_14_lib_version.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:29:20.000000 team_14_lib_version-0.6.0b5/team_14_lib_version.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 12:29:20.000000 team_14_lib_version-0.6.0b5/team_14_lib_version.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 12:29:20.000000 team_14_lib_version-0.6.0b5/team_14_lib_version.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:37:31.415857 team_14_lib_version-0.6.0b6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:37:31.411857 team_14_lib_version-0.6.0b6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:37:31.411857 team_14_lib_version-0.6.0b6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-11 12:37:11.000000 team_14_lib_version-0.6.0b6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 12:37:11.000000 team_14_lib_version-0.6.0b6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 12:37:11.000000 team_14_lib_version-0.6.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-11 12:37:31.415857 team_14_lib_version-0.6.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-11 12:37:11.000000 team_14_lib_version-0.6.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:37:31.415857 team_14_lib_version-0.6.0b6/libversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-11 12:37:11.000000 team_14_lib_version-0.6.0b6/libversion/VersionUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 12:37:11.000000 team_14_lib_version-0.6.0b6/libversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-11 12:37:31.000000 team_14_lib_version-0.6.0b6/libversion/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-11 12:37:11.000000 team_14_lib_version-0.6.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 12:37:11.000000 team_14_lib_version-0.6.0b6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:37:31.415857 team_14_lib_version-0.6.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-11 12:37:11.000000 team_14_lib_version-0.6.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:37:31.415857 team_14_lib_version-0.6.0b6/team_14_lib_version.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-11 12:37:31.000000 team_14_lib_version-0.6.0b6/team_14_lib_version.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-11 12:37:31.000000 team_14_lib_version-0.6.0b6/team_14_lib_version.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:37:31.000000 team_14_lib_version-0.6.0b6/team_14_lib_version.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-11 12:37:31.000000 team_14_lib_version-0.6.0b6/team_14_lib_version.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 12:37:31.000000 team_14_lib_version-0.6.0b6/team_14_lib_version.egg-info/top_level.txt
```

### Comparing `team_14_lib_version-0.6.0b5/.github/workflows/release.yml` & `team_14_lib_version-0.6.0b6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `team_14_lib_version-0.6.0b5/LICENSE` & `team_14_lib_version-0.6.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `team_14_lib_version-0.6.0b5/PKG-INFO` & `team_14_lib_version-0.6.0b6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: team-14-lib-version
-Version: 0.6.0b5
+Version: 0.6.0b6
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
-Requires-Dist: importlib
 Provides-Extra: dev
 Requires-Dist: twine>=4.0.2; extra == "dev"
 
 # lib-version
 A version-aware library consumed by the URL fishing detection application service
 The library parses the version from the metadata in the package.
```

### Comparing `team_14_lib_version-0.6.0b5/setup.py` & `team_14_lib_version-0.6.0b6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,15 @@
     packages=find_packages(),
     description='version aware library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Team 14',
     author_email='justinluu2000@gmail.com',
     url='https://github.com/remla2024-team14/lib-version',
-    install_requires=[
-        'importlib'
-    ],
+    install_requires=[],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     extras_require={'dev': ['twine>=4.0.2']},
     python_requires='>=3.8',
```

### Comparing `team_14_lib_version-0.6.0b5/team_14_lib_version.egg-info/PKG-INFO` & `team_14_lib_version-0.6.0b6/team_14_lib_version.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: team-14-lib-version
-Version: 0.6.0b5
+Version: 0.6.0b6
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
-Requires-Dist: importlib
 Provides-Extra: dev
 Requires-Dist: twine>=4.0.2; extra == "dev"
 
 # lib-version
 A version-aware library consumed by the URL fishing detection application service
 The library parses the version from the metadata in the package.
```

