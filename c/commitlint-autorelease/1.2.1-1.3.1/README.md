# Comparing `tmp/commitlint_autorelease-1.2.1.tar.gz` & `tmp/commitlint_autorelease-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitlint_autorelease-1.2.1.tar", last modified: Sat May 11 11:58:02 2024, max compression
+gzip compressed data, was "commitlint_autorelease-1.3.1.tar", last modified: Sat May 11 12:16:27 2024, max compression
```

## Comparing `commitlint_autorelease-1.2.1.tar` & `commitlint_autorelease-1.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:58:02.470806 commitlint_autorelease-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-11 11:58:02.466806 commitlint_autorelease-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-11 11:58:02.470806 commitlint_autorelease-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:58:02.466806 commitlint_autorelease-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:58:02.466806 commitlint_autorelease-1.2.1/src/commitlint/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/src/commitlint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/src/commitlint/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/src/commitlint/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/src/commitlint/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/src/commitlint/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/src/commitlint/git_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:58:02.466806 commitlint_autorelease-1.2.1/src/commitlint/linter/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/src/commitlint/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/src/commitlint/linter/_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/src/commitlint/linter/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/src/commitlint/linter/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/src/commitlint/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:58:02.466806 commitlint_autorelease-1.2.1/src/commitlint_autorelease.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-11 11:58:02.000000 commitlint_autorelease-1.2.1/src/commitlint_autorelease.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-11 11:58:02.000000 commitlint_autorelease-1.2.1/src/commitlint_autorelease.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 11:58:02.000000 commitlint_autorelease-1.2.1/src/commitlint_autorelease.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-11 11:58:02.000000 commitlint_autorelease-1.2.1/src/commitlint_autorelease.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 11:58:02.000000 commitlint_autorelease-1.2.1/src/commitlint_autorelease.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 11:58:02.466806 commitlint_autorelease-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-11 11:57:58.000000 commitlint_autorelease-1.2.1/tests/test_git_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:16:27.431688 commitlint_autorelease-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-11 12:16:27.431688 commitlint_autorelease-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-11 12:16:27.431688 commitlint_autorelease-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:16:27.427688 commitlint_autorelease-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:16:27.431688 commitlint_autorelease-1.3.1/src/commitlint/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/src/commitlint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/src/commitlint/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/src/commitlint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/src/commitlint/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/src/commitlint/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/src/commitlint/git_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:16:27.431688 commitlint_autorelease-1.3.1/src/commitlint/linter/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/src/commitlint/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/src/commitlint/linter/_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/src/commitlint/linter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/src/commitlint/linter/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/src/commitlint/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:16:27.431688 commitlint_autorelease-1.3.1/src/commitlint_autorelease.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-11 12:16:27.000000 commitlint_autorelease-1.3.1/src/commitlint_autorelease.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-11 12:16:27.000000 commitlint_autorelease-1.3.1/src/commitlint_autorelease.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:16:27.000000 commitlint_autorelease-1.3.1/src/commitlint_autorelease.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-11 12:16:27.000000 commitlint_autorelease-1.3.1/src/commitlint_autorelease.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 12:16:27.000000 commitlint_autorelease-1.3.1/src/commitlint_autorelease.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:16:27.431688 commitlint_autorelease-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-11 12:16:10.000000 commitlint_autorelease-1.3.1/tests/test_git_helpers.py
```

### Comparing `commitlint_autorelease-1.2.1/LICENSE` & `commitlint_autorelease-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commitlint_autorelease-1.2.1/PKG-INFO` & `commitlint_autorelease-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitlint-autorelease
-Version: 1.2.1
+Version: 1.3.1
 Summary: commitlint is is a pre-commit hook designed to lint your commit messages according to the Conventional Commits standard.
 Home-page: https://github.com/opensource-nepal/commitlint
 Author: opensource-nepal
 Author-email: aj3sshh@gmail.com, sugatbajracharya49@gmail.com
 License: GPL-3.0
 Project-URL: Source, https://github.com/opensource-nepal/commitlint
 Project-URL: Changelog, https://github.com/opensource-nepal/commitlint/blob/main/CHANGELOG.md
```

### Comparing `commitlint_autorelease-1.2.1/README.md` & `commitlint_autorelease-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `commitlint_autorelease-1.2.1/setup.cfg` & `commitlint_autorelease-1.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `commitlint_autorelease-1.2.1/src/commitlint/cli.py` & `commitlint_autorelease-1.3.1/src/commitlint/cli.py`

 * *Files identical despite different names*

### Comparing `commitlint_autorelease-1.2.1/src/commitlint/constants.py` & `commitlint_autorelease-1.3.1/src/commitlint/constants.py`

 * *Files identical despite different names*

### Comparing `commitlint_autorelease-1.2.1/src/commitlint/git_helpers.py` & `commitlint_autorelease-1.3.1/src/commitlint/git_helpers.py`

 * *Files identical despite different names*

### Comparing `commitlint_autorelease-1.2.1/src/commitlint/linter/_linter.py` & `commitlint_autorelease-1.3.1/src/commitlint/linter/_linter.py`

 * *Files identical despite different names*

### Comparing `commitlint_autorelease-1.2.1/src/commitlint/linter/utils.py` & `commitlint_autorelease-1.3.1/src/commitlint/linter/utils.py`

 * *Files identical despite different names*

### Comparing `commitlint_autorelease-1.2.1/src/commitlint/linter/validators.py` & `commitlint_autorelease-1.3.1/src/commitlint/linter/validators.py`

 * *Files identical despite different names*

### Comparing `commitlint_autorelease-1.2.1/src/commitlint/messages.py` & `commitlint_autorelease-1.3.1/src/commitlint/messages.py`

 * *Files identical despite different names*

### Comparing `commitlint_autorelease-1.2.1/src/commitlint_autorelease.egg-info/PKG-INFO` & `commitlint_autorelease-1.3.1/src/commitlint_autorelease.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitlint-autorelease
-Version: 1.2.1
+Version: 1.3.1
 Summary: commitlint is is a pre-commit hook designed to lint your commit messages according to the Conventional Commits standard.
 Home-page: https://github.com/opensource-nepal/commitlint
 Author: opensource-nepal
 Author-email: aj3sshh@gmail.com, sugatbajracharya49@gmail.com
 License: GPL-3.0
 Project-URL: Source, https://github.com/opensource-nepal/commitlint
 Project-URL: Changelog, https://github.com/opensource-nepal/commitlint/blob/main/CHANGELOG.md
```

### Comparing `commitlint_autorelease-1.2.1/src/commitlint_autorelease.egg-info/SOURCES.txt` & `commitlint_autorelease-1.3.1/src/commitlint_autorelease.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commitlint_autorelease-1.2.1/tests/test_cli.py` & `commitlint_autorelease-1.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `commitlint_autorelease-1.2.1/tests/test_git_helpers.py` & `commitlint_autorelease-1.3.1/tests/test_git_helpers.py`

 * *Files identical despite different names*

