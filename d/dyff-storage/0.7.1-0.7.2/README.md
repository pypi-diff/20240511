# Comparing `tmp/dyff_storage-0.7.1.tar.gz` & `tmp/dyff_storage-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_storage-0.7.1.tar", last modified: Wed May  8 20:08:59 2024, max compression
+gzip compressed data, was "dyff_storage-0.7.2.tar", last modified: Fri May 10 21:58:00 2024, max compression
```

## Comparing `dyff_storage-0.7.1.tar` & `dyff_storage-0.7.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.973514 dyff_storage-0.7.1/
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1706 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2577 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3477 2024-05-08 20:08:59.972514 dyff_storage-0.7.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.961514 dyff_storage-0.7.1/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.967514 dyff_storage-0.7.1/dyff/storage/
--rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.967514 dyff_storage-0.7.1/dyff/storage/backend/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.968514 dyff_storage-0.7.1/dyff/storage/backend/base/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/base/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/base/command.py
--rw-rw-rw-   0 root         (0) root         (0)    14287 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/base/query.py
--rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/base/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.969514 dyff_storage-0.7.1/dyff/storage/backend/gcloud/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/gcloud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6656 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/gcloud/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.969514 dyff_storage-0.7.1/dyff/storage/backend/kafka/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9209 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/kafka/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.970514 dyff_storage-0.7.1/dyff/storage/backend/mock/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/mock/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.970514 dyff_storage-0.7.1/dyff/storage/backend/mongodb/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/mongodb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/mongodb/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    24016 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/mongodb/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.971514 dyff_storage-0.7.1/dyff/storage/backend/s3/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15072 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/backend/s3/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    10386 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/config.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/dynamic_import.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/paths.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/dyff/storage/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.972514 dyff_storage-0.7.1/dyff_storage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3477 2024-05-08 20:08:59.000000 dyff_storage-0.7.1/dyff_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1176 2024-05-08 20:08:59.000000 dyff_storage-0.7.1/dyff_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 20:08:59.000000 dyff_storage-0.7.1/dyff_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-05-08 20:08:59.000000 dyff_storage-0.7.1/dyff_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-08 20:08:59.000000 dyff_storage-0.7.1/dyff_storage.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 20:08:59.973514 dyff_storage-0.7.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 20:08:59.972514 dyff_storage-0.7.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-08 20:08:54.000000 dyff_storage-0.7.1/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 21:58:00.491062 dyff_storage-0.7.2/
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-10 21:58:00.491062 dyff_storage-0.7.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 21:58:00.479062 dyff_storage-0.7.2/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 21:58:00.485062 dyff_storage-0.7.2/dyff/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 21:58:00.485062 dyff_storage-0.7.2/dyff/storage/backend/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 21:58:00.486062 dyff_storage-0.7.2/dyff/storage/backend/base/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/base/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/base/command.py
+-rw-rw-rw-   0 root         (0) root         (0)    13398 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/base/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/base/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 21:58:00.486062 dyff_storage-0.7.2/dyff/storage/backend/gcloud/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/gcloud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6656 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/gcloud/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 21:58:00.487062 dyff_storage-0.7.2/dyff/storage/backend/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9209 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/kafka/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 21:58:00.487062 dyff_storage-0.7.2/dyff/storage/backend/mock/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/mock/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 21:58:00.488062 dyff_storage-0.7.2/dyff/storage/backend/mongodb/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/mongodb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/mongodb/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    23245 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/mongodb/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 21:58:00.488062 dyff_storage-0.7.2/dyff/storage/backend/s3/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15072 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/backend/s3/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10386 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/dynamic_import.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/dyff/storage/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 21:58:00.490062 dyff_storage-0.7.2/dyff_storage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-10 21:58:00.000000 dyff_storage-0.7.2/dyff_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-05-10 21:58:00.000000 dyff_storage-0.7.2/dyff_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 21:58:00.000000 dyff_storage-0.7.2/dyff_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-05-10 21:58:00.000000 dyff_storage-0.7.2/dyff_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-10 21:58:00.000000 dyff_storage-0.7.2/dyff_storage.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 21:58:00.491062 dyff_storage-0.7.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 21:58:00.490062 dyff_storage-0.7.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-10 21:57:54.000000 dyff_storage-0.7.2/tests/test_import.py
```

### Comparing `dyff_storage-0.7.1/.gitignore` & `dyff_storage-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/.gitlab-ci.yml` & `dyff_storage-0.7.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/.licenserc.yaml` & `dyff_storage-0.7.2/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/.pre-commit-config.yaml` & `dyff_storage-0.7.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/.secrets.baseline` & `dyff_storage-0.7.2/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/CODE_OF_CONDUCT.md` & `dyff_storage-0.7.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/LICENSE` & `dyff_storage-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/PKG-INFO` & `dyff_storage-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.7.1/README.md` & `dyff_storage-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/dyff/storage/__init__.py` & `dyff_storage-0.7.2/dyff/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/dyff/storage/backend/base/auth.py` & `dyff_storage-0.7.2/dyff/storage/backend/base/auth.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/dyff/storage/backend/base/command.py` & `dyff_storage-0.7.2/dyff/storage/backend/base/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/dyff/storage/backend/base/query.py` & `dyff_storage-0.7.2/dyff/storage/backend/base/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from __future__ import annotations
 
 import abc
 from typing import Collection, NamedTuple, Optional, Set
 
 from dyff.schema.platform import (
-    Analysis,
     Audit,
     Dataset,
     DataSource,
     Documentation,
     Evaluation,
     Family,
     InferenceService,
@@ -21,15 +20,14 @@
     Model,
     Module,
     Report,
     SafetyCase,
     Tag,
 )
 from dyff.schema.requests import (
-    AnalysisQueryRequest,
     AuditQueryRequest,
     DatasetQueryRequest,
     DocumentationEditRequest,
     EvaluationQueryRequest,
     InferenceServiceQueryRequest,
     InferenceSessionQueryRequest,
     MeasurementQueryRequest,
@@ -53,39 +51,14 @@
     @staticmethod
     def nothing():
         return Whitelist(accounts=set(), entities=set())
 
 
 class QueryBackend(abc.ABC):
     @abc.abstractmethod
-    def get_analysis(self, id: str) -> Optional[Analysis]:
-        """Retrieve an Analysis entity.
-
-        Parameters:
-          id: The unique key of the Analysis.
-
-        Returns:
-          The Analysis, or None if no Analysis with the specified key exists.
-        """
-
-    @abc.abstractmethod
-    def query_analyses(
-        self, whitelist: Whitelist, query: AnalysisQueryRequest
-    ) -> Collection[Analysis]:
-        """Retrieve all Analysis entities matching the query parameters.
-
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the Analysis entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
-        """
-
-    @abc.abstractmethod
     def get_audit(self, id: str) -> Optional[Audit]:
         """Retrieve an Audit entity.
 
         Parameters:
           id: The unique key of the Audit.
 
         Returns:
```

### Comparing `dyff_storage-0.7.1/dyff/storage/backend/base/storage.py` & `dyff_storage-0.7.2/dyff/storage/backend/base/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/dyff/storage/backend/gcloud/storage.py` & `dyff_storage-0.7.2/dyff/storage/backend/gcloud/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/dyff/storage/backend/kafka/command.py` & `dyff_storage-0.7.2/dyff/storage/backend/kafka/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/dyff/storage/backend/mock/command.py` & `dyff_storage-0.7.2/dyff/storage/backend/mock/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/dyff/storage/backend/mongodb/auth.py` & `dyff_storage-0.7.2/dyff/storage/backend/mongodb/auth.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/dyff/storage/backend/mongodb/query.py` & `dyff_storage-0.7.2/dyff/storage/backend/mongodb/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import json
 from typing import Collection, Iterable, Optional
 
 import pymongo
 
 from dyff.schema.platform import (
-    Analysis,
     Audit,
     Dataset,
     DataSource,
     Documentation,
     Entities,
     Evaluation,
     Family,
@@ -26,15 +25,14 @@
     Module,
     Report,
     Resources,
     SafetyCase,
     Tag,
 )
 from dyff.schema.requests import (
-    AnalysisQueryRequest,
     AuditQueryRequest,
     DatasetQueryRequest,
     DocumentationEditRequest,
     EvaluationQueryRequest,
     InferenceServiceQueryRequest,
     InferenceSessionQueryRequest,
     MeasurementQueryRequest,
@@ -137,45 +135,14 @@
         """If query_dict contains a value for old_key, pop the value and add it back at
         new_key."""
         unset = object()
         value = query_dict.pop(old_key, unset)
         if value is not unset:
             query_dict[new_key] = value
 
-    def get_analysis(self, id: str) -> Optional[Analysis]:
-        """Retrieve an Analysis entity.
-
-        Parameters:
-          id: The unique key of the Analysis.
-
-        Returns:
-          The Analysis, or None if no Analysis with the specified key exists.
-        """
-        result = self._get_entity(Entities.Analysis, id)
-        return Analysis.parse_obj(result) if result else None
-
-    def query_analyses(
-        self, whitelist: Whitelist, query: AnalysisQueryRequest
-    ) -> Collection[Analysis]:
-        """Retrieve all Analysis entities matching the query parameters.
-
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the Analysis entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
-        """
-        qdict = query.dict()
-        self._rename_query_key(qdict, "method", "method.id")
-        self._rename_query_key(qdict, "methodName", "method.name")
-        self._rename_query_key(qdict, "methodOutputKind", "method.output.kind")
-        results = self._query_entities(Entities.Analysis, whitelist, qdict)
-        return [Analysis.parse_obj(result) for result in results]
-
     def get_audit(self, id: str) -> Optional[Audit]:
         """Retrieve an Audit entity.
 
         Parameters:
           id: The unique key of the Audit.
 
         Returns:
@@ -435,14 +402,18 @@
           **query: Equality constraints on fields of the Measurement entity.
             The returned entities satisfy 'entity.field==value' for all items
             'field: value' in kwargs.
         """
         qdict = query.dict()
         self._rename_query_key(qdict, "method", "method.id")
         self._rename_query_key(qdict, "methodName", "method.name")
+        self._rename_query_key(qdict, "dataset", "scope.dataset")
+        self._rename_query_key(qdict, "evaluation", "scope.evaluation")
+        self._rename_query_key(qdict, "inferenceService", "scope.inferenceService")
+        self._rename_query_key(qdict, "model", "scope.model")
         results = self._query_entities(Entities.Measurement, whitelist, qdict)
         return [Measurement.parse_obj(result) for result in results]
 
     def get_method(self, id: str) -> Optional[Method]:
         """Retrieve a Method entity.
 
         Parameters:
@@ -578,14 +549,18 @@
           **query: Equality constraints on fields of the SafetyCase entity.
             The returned entities satisfy 'entity.field==value' for all items
             'field: value' in kwargs.
         """
         qdict = query.dict()
         self._rename_query_key(qdict, "method", "method.id")
         self._rename_query_key(qdict, "methodName", "method.name")
+        self._rename_query_key(qdict, "dataset", "scope.dataset")
+        self._rename_query_key(qdict, "evaluation", "scope.evaluation")
+        self._rename_query_key(qdict, "inferenceService", "scope.inferenceService")
+        self._rename_query_key(qdict, "model", "scope.model")
         results = self._query_entities(Entities.SafetyCase, whitelist, qdict)
         return [SafetyCase.parse_obj(result) for result in results]
 
     def get_tag(self, id: str) -> Optional[Tag]:
         """Retrieve a Tag entity.
 
         Parameters:
```

### Comparing `dyff_storage-0.7.1/dyff/storage/backend/s3/storage.py` & `dyff_storage-0.7.2/dyff/storage/backend/s3/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/dyff/storage/config.py` & `dyff_storage-0.7.2/dyff/storage/config.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/dyff/storage/paths.py` & `dyff_storage-0.7.2/dyff/storage/paths.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/dyff/storage/timestamp.py` & `dyff_storage-0.7.2/dyff/storage/timestamp.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/dyff_storage.egg-info/PKG-INFO` & `dyff_storage-0.7.2/dyff_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.7.1/dyff_storage.egg-info/SOURCES.txt` & `dyff_storage-0.7.2/dyff_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/makefile` & `dyff_storage-0.7.2/makefile`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/pyproject.toml` & `dyff_storage-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.1/tests/test_import.py` & `dyff_storage-0.7.2/tests/test_import.py`

 * *Files identical despite different names*

