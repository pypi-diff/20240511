# Comparing `tmp/dyff_storage-0.7.3.tar.gz` & `tmp/dyff_storage-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_storage-0.7.3.tar", last modified: Fri May 10 22:23:46 2024, max compression
+gzip compressed data, was "dyff_storage-0.7.4.tar", last modified: Fri May 10 23:19:02 2024, max compression
```

## Comparing `dyff_storage-0.7.3.tar` & `dyff_storage-0.7.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:23:46.082432 dyff_storage-0.7.3/
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1706 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2577 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3477 2024-05-10 22:23:46.081431 dyff_storage-0.7.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:23:46.069432 dyff_storage-0.7.3/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:23:46.075432 dyff_storage-0.7.3/dyff/storage/
--rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:23:46.075432 dyff_storage-0.7.3/dyff/storage/backend/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:23:46.077432 dyff_storage-0.7.3/dyff/storage/backend/base/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/base/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/base/command.py
--rw-rw-rw-   0 root         (0) root         (0)    13398 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/base/query.py
--rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/base/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:23:46.077432 dyff_storage-0.7.3/dyff/storage/backend/gcloud/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/gcloud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6656 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/gcloud/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:23:46.077432 dyff_storage-0.7.3/dyff/storage/backend/kafka/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9209 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/kafka/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:23:46.078432 dyff_storage-0.7.3/dyff/storage/backend/mock/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/mock/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:23:46.079432 dyff_storage-0.7.3/dyff/storage/backend/mongodb/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/mongodb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/mongodb/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    23229 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/mongodb/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:23:46.079432 dyff_storage-0.7.3/dyff/storage/backend/s3/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15072 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/backend/s3/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    10386 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/config.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/dynamic_import.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/paths.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/dyff/storage/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:23:46.081431 dyff_storage-0.7.3/dyff_storage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3477 2024-05-10 22:23:46.000000 dyff_storage-0.7.3/dyff_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1176 2024-05-10 22:23:46.000000 dyff_storage-0.7.3/dyff_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 22:23:46.000000 dyff_storage-0.7.3/dyff_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-05-10 22:23:46.000000 dyff_storage-0.7.3/dyff_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-10 22:23:46.000000 dyff_storage-0.7.3/dyff_storage.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 22:23:46.082432 dyff_storage-0.7.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 22:23:46.081431 dyff_storage-0.7.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-10 22:23:39.000000 dyff_storage-0.7.3/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.465409 dyff_storage-0.7.4/
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-10 23:19:02.464409 dyff_storage-0.7.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.452409 dyff_storage-0.7.4/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.458409 dyff_storage-0.7.4/dyff/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.458409 dyff_storage-0.7.4/dyff/storage/backend/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.459409 dyff_storage-0.7.4/dyff/storage/backend/base/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/base/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/base/command.py
+-rw-rw-rw-   0 root         (0) root         (0)    13398 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/base/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/base/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.460409 dyff_storage-0.7.4/dyff/storage/backend/gcloud/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/gcloud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6656 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/gcloud/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.460409 dyff_storage-0.7.4/dyff/storage/backend/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9209 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/kafka/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.461409 dyff_storage-0.7.4/dyff/storage/backend/mock/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/mock/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.462409 dyff_storage-0.7.4/dyff/storage/backend/mongodb/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/mongodb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/mongodb/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    23188 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/mongodb/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.462409 dyff_storage-0.7.4/dyff/storage/backend/s3/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15072 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/s3/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10386 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/dynamic_import.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.464409 dyff_storage-0.7.4/dyff_storage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-10 23:19:02.000000 dyff_storage-0.7.4/dyff_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-05-10 23:19:02.000000 dyff_storage-0.7.4/dyff_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 23:19:02.000000 dyff_storage-0.7.4/dyff_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-05-10 23:19:02.000000 dyff_storage-0.7.4/dyff_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-10 23:19:02.000000 dyff_storage-0.7.4/dyff_storage.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 23:19:02.465409 dyff_storage-0.7.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.463409 dyff_storage-0.7.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/tests/test_import.py
```

### Comparing `dyff_storage-0.7.3/.gitignore` & `dyff_storage-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/.gitlab-ci.yml` & `dyff_storage-0.7.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/.licenserc.yaml` & `dyff_storage-0.7.4/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/.pre-commit-config.yaml` & `dyff_storage-0.7.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/.secrets.baseline` & `dyff_storage-0.7.4/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/CODE_OF_CONDUCT.md` & `dyff_storage-0.7.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/LICENSE` & `dyff_storage-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/PKG-INFO` & `dyff_storage-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.7.3/README.md` & `dyff_storage-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff/storage/__init__.py` & `dyff_storage-0.7.4/dyff/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff/storage/backend/base/auth.py` & `dyff_storage-0.7.4/dyff/storage/backend/base/auth.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff/storage/backend/base/command.py` & `dyff_storage-0.7.4/dyff/storage/backend/base/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff/storage/backend/base/query.py` & `dyff_storage-0.7.4/dyff/storage/backend/base/query.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff/storage/backend/base/storage.py` & `dyff_storage-0.7.4/dyff/storage/backend/base/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff/storage/backend/gcloud/storage.py` & `dyff_storage-0.7.4/dyff/storage/backend/gcloud/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff/storage/backend/kafka/command.py` & `dyff_storage-0.7.4/dyff/storage/backend/kafka/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff/storage/backend/mock/command.py` & `dyff_storage-0.7.4/dyff/storage/backend/mock/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff/storage/backend/mongodb/auth.py` & `dyff_storage-0.7.4/dyff/storage/backend/mongodb/auth.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff/storage/backend/mongodb/query.py` & `dyff_storage-0.7.4/dyff/storage/backend/mongodb/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,18 +109,17 @@
             # elif k == "annotations":
             #     pass
             elif k == "inputsAnyOf":
                 # This is a special query for Analysis-related entities. It
                 # selects entities that reference any of the listed IDs in
                 # their .inputs field.
                 entity_list = v.split(",")
-                for entity in entity_list:
-                    mongo_conjunction.append(
-                        {"inputs": {"$elemMatch": {"entity": entity}}}
-                    )
+                mongo_conjunction.append(
+                    {"inputs": {"$elemMatch": {"entity": {"$in": entity_list}}}}
+                )
             elif isinstance(v, list):
                 mongo_conjunction.append({k: {"$in": list(v)}})
             else:
                 mongo_conjunction.append({k: v})
 
         query = {"$and": mongo_conjunction} if mongo_conjunction else {}
         print(f"query: {query}")
```

### Comparing `dyff_storage-0.7.3/dyff/storage/backend/s3/storage.py` & `dyff_storage-0.7.4/dyff/storage/backend/s3/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff/storage/config.py` & `dyff_storage-0.7.4/dyff/storage/config.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff/storage/paths.py` & `dyff_storage-0.7.4/dyff/storage/paths.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff/storage/timestamp.py` & `dyff_storage-0.7.4/dyff/storage/timestamp.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/dyff_storage.egg-info/PKG-INFO` & `dyff_storage-0.7.4/dyff_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.7.3
+Version: 0.7.4
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.7.3/dyff_storage.egg-info/SOURCES.txt` & `dyff_storage-0.7.4/dyff_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/makefile` & `dyff_storage-0.7.4/makefile`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/pyproject.toml` & `dyff_storage-0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.3/tests/test_import.py` & `dyff_storage-0.7.4/tests/test_import.py`

 * *Files identical despite different names*

