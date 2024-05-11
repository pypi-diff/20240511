# Comparing `tmp/dyff_client-0.4.2.tar.gz` & `tmp/dyff_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_client-0.4.2.tar", last modified: Thu May  9 00:38:48 2024, max compression
+gzip compressed data, was "dyff_client-0.5.0.tar", last modified: Fri May 10 23:58:54 2024, max compression
```

## Comparing `dyff_client-0.4.2.tar` & `dyff_client-0.5.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.573569 dyff_client-0.4.2/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-09 00:38:42.000000 dyff_client-0.4.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1777 2024-05-09 00:38:42.000000 dyff_client-0.4.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-05-09 00:38:42.000000 dyff_client-0.4.2/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-09 00:38:42.000000 dyff_client-0.4.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-09 00:38:42.000000 dyff_client-0.4.2/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-09 00:38:42.000000 dyff_client-0.4.2/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-09 00:38:42.000000 dyff_client-0.4.2/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-09 00:38:42.000000 dyff_client-0.4.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-09 00:38:42.000000 dyff_client-0.4.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4008 2024-05-09 00:38:48.573569 dyff_client-0.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2781 2024-05-09 00:38:42.000000 dyff_client-0.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.559569 dyff_client-0.4.2/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.564569 dyff_client-0.4.2/dyff/client/
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.566569 dyff_client-0.4.2/dyff/client/_generated/
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)    80932 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/_serialization.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.567569 dyff_client-0.4.2/dyff/client/_generated/aio/
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6649 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.569569 dyff_client-0.4.2/dyff/client/_generated/aio/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   821473 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/operations/_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.570569 dyff_client-0.4.2/dyff/client/_generated/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   877754 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/operations/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    77153 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.572569 dyff_client-0.4.2/dyff_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4008 2024-05-09 00:38:48.000000 dyff_client-0.4.2/dyff_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1464 2024-05-09 00:38:48.000000 dyff_client-0.4.2/dyff_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 00:38:48.000000 dyff_client-0.4.2/dyff_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2024-05-09 00:38:48.000000 dyff_client-0.4.2/dyff_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-09 00:38:48.000000 dyff_client-0.4.2/dyff_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-09 00:38:42.000000 dyff_client-0.4.2/makefile
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-09 00:38:42.000000 dyff_client-0.4.2/package-lock.json
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-05-09 00:38:42.000000 dyff_client-0.4.2/package.json
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-09 00:38:42.000000 dyff_client-0.4.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.560569 dyff_client-0.4.2/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.571569 dyff_client-0.4.2/scripts/inferenceservices/
--rw-rw-rw-   0 root         (0) root         (0)     2529 2024-05-09 00:38:42.000000 dyff_client-0.4.2/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
--rw-rw-rw-   0 root         (0) root         (0)     2537 2024-05-09 00:38:42.000000 dyff_client-0.4.2/scripts/inferenceservices/tiiuae--falcon-7b--default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.572569 dyff_client-0.4.2/scripts/models/
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-09 00:38:42.000000 dyff_client-0.4.2/scripts/models/databricks--dolly-v2-3b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-09 00:38:42.000000 dyff_client-0.4.2/scripts/models/databricks--dolly-v2-3b.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-09 00:38:42.000000 dyff_client-0.4.2/scripts/models/tiiuae--falcon-7b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1356 2024-05-09 00:38:42.000000 dyff_client-0.4.2/scripts/models/tiiuae--falcon-7b.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 00:38:48.573569 dyff_client-0.4.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.572569 dyff_client-0.4.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-09 00:38:42.000000 dyff_client-0.4.2/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:58:54.445450 dyff_client-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-10 23:58:48.000000 dyff_client-0.5.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2024-05-10 23:58:48.000000 dyff_client-0.5.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-05-10 23:58:48.000000 dyff_client-0.5.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-10 23:58:48.000000 dyff_client-0.5.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-10 23:58:48.000000 dyff_client-0.5.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-10 23:58:48.000000 dyff_client-0.5.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-10 23:58:48.000000 dyff_client-0.5.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-10 23:58:48.000000 dyff_client-0.5.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-10 23:58:48.000000 dyff_client-0.5.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-05-10 23:58:54.445450 dyff_client-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2024-05-10 23:58:48.000000 dyff_client-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:58:54.429450 dyff_client-0.5.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:58:54.435450 dyff_client-0.5.0/dyff/client/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:58:54.437450 dyff_client-0.5.0/dyff/client/_generated/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    80932 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/_serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:58:54.438450 dyff_client-0.5.0/dyff/client/_generated/aio/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/aio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6649 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/aio/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/aio/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/aio/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/aio/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:58:54.440450 dyff_client-0.5.0/dyff/client/_generated/aio/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/aio/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   830387 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/aio/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/aio/operations/_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:58:54.441450 dyff_client-0.5.0/dyff/client/_generated/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   888309 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/operations/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/_generated/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    82979 2024-05-10 23:58:48.000000 dyff_client-0.5.0/dyff/client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:58:54.444450 dyff_client-0.5.0/dyff_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-05-10 23:58:54.000000 dyff_client-0.5.0/dyff_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-05-10 23:58:54.000000 dyff_client-0.5.0/dyff_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 23:58:54.000000 dyff_client-0.5.0/dyff_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-05-10 23:58:54.000000 dyff_client-0.5.0/dyff_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-10 23:58:54.000000 dyff_client-0.5.0/dyff_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-10 23:58:48.000000 dyff_client-0.5.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-10 23:58:48.000000 dyff_client-0.5.0/package-lock.json
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-05-10 23:58:48.000000 dyff_client-0.5.0/package.json
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-10 23:58:48.000000 dyff_client-0.5.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:58:54.431450 dyff_client-0.5.0/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:58:54.443450 dyff_client-0.5.0/scripts/inferenceservices/
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2024-05-10 23:58:48.000000 dyff_client-0.5.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2024-05-10 23:58:48.000000 dyff_client-0.5.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:58:54.444450 dyff_client-0.5.0/scripts/models/
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-10 23:58:48.000000 dyff_client-0.5.0/scripts/models/databricks--dolly-v2-3b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-10 23:58:48.000000 dyff_client-0.5.0/scripts/models/databricks--dolly-v2-3b.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-10 23:58:48.000000 dyff_client-0.5.0/scripts/models/tiiuae--falcon-7b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2024-05-10 23:58:48.000000 dyff_client-0.5.0/scripts/models/tiiuae--falcon-7b.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 23:58:54.445450 dyff_client-0.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:58:54.444450 dyff_client-0.5.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-10 23:58:48.000000 dyff_client-0.5.0/tests/test_import.py
```

### Comparing `dyff_client-0.4.2/.gitlab-ci.yml` & `dyff_client-0.5.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/.licenserc.yaml` & `dyff_client-0.5.0/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/.pre-commit-config.yaml` & `dyff_client-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/.secrets.baseline` & `dyff_client-0.5.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/CODE_OF_CONDUCT.md` & `dyff_client-0.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/LICENSE` & `dyff_client-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/PKG-INFO` & `dyff_client-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.4.2
+Version: 0.5.0
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_client-0.4.2/README.md` & `dyff_client-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/__init__.py` & `dyff_client-0.5.0/dyff/client/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/_client.py` & `dyff_client-0.5.0/dyff/client/_generated/_client.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/_configuration.py` & `dyff_client-0.5.0/dyff/client/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/_patch.py` & `dyff_client-0.5.0/dyff/client/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/_serialization.py` & `dyff_client-0.5.0/dyff/client/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/_vendor.py` & `dyff_client-0.5.0/dyff/client/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/aio/__init__.py` & `dyff_client-0.5.0/dyff/client/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/aio/_client.py` & `dyff_client-0.5.0/dyff/client/_generated/aio/_client.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/aio/_configuration.py` & `dyff_client-0.5.0/dyff/client/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/aio/_patch.py` & `dyff_client-0.5.0/dyff/client/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/aio/_vendor.py` & `dyff_client-0.5.0/dyff/client/_generated/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/aio/operations/__init__.py` & `dyff_client-0.5.0/dyff/client/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/aio/operations/_operations.py` & `dyff_client-0.5.0/dyff/client/_generated/aio/operations/_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import sys
 from io import IOBase
 from typing import (
     IO,
     Any,
-    AsyncIterator,
     Callable,
     Dict,
     List,
     Optional,
     Type,
     TypeVar,
     Union,
@@ -32,26 +31,26 @@
 from azure.core.pipeline import PipelineResponse
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 
 from ...operations._operations import (
     build_datasets_create_request,
-    build_datasets_data_request,
     build_datasets_delete_request,
     build_datasets_documentation_request,
+    build_datasets_downlinks_request,
     build_datasets_edit_documentation_request,
     build_datasets_finalize_request,
     build_datasets_get_request,
     build_datasets_label_request,
     build_datasets_query_request,
-    build_datasets_strata_request,
     build_datasets_upload_request,
     build_evaluations_create_request,
     build_evaluations_delete_request,
+    build_evaluations_downlinks_request,
     build_evaluations_get_request,
     build_evaluations_label_request,
     build_evaluations_query_request,
     build_inferenceservices_create_request,
     build_inferenceservices_delete_request,
     build_inferenceservices_documentation_request,
     build_inferenceservices_edit_documentation_request,
@@ -86,23 +85,24 @@
     build_models_edit_documentation_request,
     build_models_get_request,
     build_models_label_request,
     build_models_query_request,
     build_modules_create_request,
     build_modules_delete_request,
     build_modules_documentation_request,
+    build_modules_downlinks_request,
     build_modules_edit_documentation_request,
     build_modules_finalize_request,
     build_modules_get_request,
     build_modules_label_request,
     build_modules_query_request,
     build_modules_upload_request,
     build_reports_create_request,
-    build_reports_data_request,
     build_reports_delete_request,
+    build_reports_downlinks_request,
     build_reports_get_request,
     build_reports_label_request,
     build_reports_query_request,
     build_safetycases_create_request,
     build_safetycases_delete_request,
     build_safetycases_downlinks_request,
     build_safetycases_get_request,
@@ -1301,111 +1301,33 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace_async
-    async def strata(
-        self, dataset_id: str, **kwargs: Any
-    ) -> Union[AsyncIterator[bytes], JSON]:
-        """Get the strata corresponding to a Dataset.
+    async def delete(self, dataset_id: str, **kwargs: Any) -> JSON:
+        """Mark a Dataset for deletion.
 
-        Get the strata corresponding to a Dataset. The data is returned as a
-        Parquet file suitable for reading with libraries like Pandas.
+        Mark a Dataset for deletion.
 
         :param dataset_id: Required.
         :type dataset_id: str
-        :return: AsyncIterator[bytes] or JSON object or None
-        :rtype: AsyncIterator[bytes] or JSON or None
+        :return: JSON object
+        :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
-                # response body for status code(s): 422
+                # response body for status code(s): 200
                 response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
-        """
-        error_map: MutableMapping[int, Type[HttpResponseError]] = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = kwargs.pop("params", {}) or {}
-
-        cls: ClsType[Union[AsyncIterator[bytes], JSON]] = kwargs.pop("cls", None)
-
-        _request = build_datasets_strata_request(
-            dataset_id=dataset_id,
-            headers=_headers,
-            params=_params,
-        )
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = True
-        pipeline_response: PipelineResponse = (
-            await self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
-            )
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 404, 422]:
-            if _stream:
-                await response.read()  # Load the body in memory and close the socket
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
-            raise HttpResponseError(response=response)
-
-        deserialized = None
-        if response.status_code == 200:
-            deserialized = response.iter_bytes()
-
-        if response.status_code == 422:
-            deserialized = response.iter_bytes()
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})  # type: ignore
-
-        return deserialized  # type: ignore
-
-    @distributed_trace_async
-    async def data(
-        self, dataset_id: str, **kwargs: Any
-    ) -> Union[AsyncIterator[bytes], JSON]:
-        """Get the raw data for the Dataset.
-
-        Get the raw data for the Dataset. The data is streamed in pyarrow.ipc
-        format.
-
-        :param dataset_id: Required.
-        :type dataset_id: str
-        :return: AsyncIterator[bytes] or JSON object or None
-        :rtype: AsyncIterator[bytes] or JSON or None
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
                                 {}
                             ],
@@ -1422,71 +1344,82 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[Union[AsyncIterator[bytes], JSON]] = kwargs.pop("cls", None)
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        _request = build_datasets_data_request(
+        _request = build_datasets_delete_request(
             dataset_id=dataset_id,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
-        _stream = True
+        _stream = False
         pipeline_response: PipelineResponse = (
             await self._client._pipeline.run(  # pylint: disable=protected-access
                 _request, stream=_stream, **kwargs
             )
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 404, 422]:
+        if response.status_code not in [200, 422]:
             if _stream:
                 await response.read()  # Load the body in memory and close the socket
             map_error(
                 status_code=response.status_code, response=response, error_map=error_map
             )
             raise HttpResponseError(response=response)
 
-        deserialized = None
         if response.status_code == 200:
-            deserialized = response.iter_bytes()
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
 
         if response.status_code == 422:
-            deserialized = response.iter_bytes()
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
 
         if cls:
-            return cls(pipeline_response, deserialized, {})  # type: ignore
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
-        return deserialized  # type: ignore
+        return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace_async
-    async def delete(self, dataset_id: str, **kwargs: Any) -> JSON:
-        """Mark a Dataset for deletion.
+    async def upload(self, dataset_id: str, artifact_path: str, **kwargs: Any) -> JSON:
+        """Get a signed URL to which the given artifact can be uploaded.
 
-        Mark a Dataset for deletion.
+        Get a signed URL to which the given artifact can be uploaded.
 
         :param dataset_id: Required.
         :type dataset_id: str
+        :param artifact_path: Required.
+        :type artifact_path: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
-                    "reason": "str",  # Optional. Reason for current status (assigned by system).
-                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                    "method": "str",  # The HTTP method applicable to the URL. Required.
+                    "url": "str",  # The signed URL. Required.
+                    "headers": {
+                        "str": "str"  # Optional. Mandatory headers that must be passed with
+                          the request.
+                    }
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
                                 {}
@@ -1506,16 +1439,17 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        _request = build_datasets_delete_request(
+        _request = build_datasets_upload_request(
             dataset_id=dataset_id,
+            artifact_path=artifact_path,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = (
@@ -1548,39 +1482,28 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace_async
-    async def upload(self, dataset_id: str, artifact_path: str, **kwargs: Any) -> JSON:
-        """Get a signed URL to which the given artifact can be uploaded.
+    async def finalize(self, dataset_id: str, **kwargs: Any) -> Union[Any, JSON]:
+        """Indicate that all dataset artifacts have been uploaded.
 
-        Get a signed URL to which the given artifact can be uploaded.
+        Indicate that all dataset artifacts have been uploaded.
 
         :param dataset_id: Required.
         :type dataset_id: str
-        :param artifact_path: Required.
-        :type artifact_path: str
-        :return: JSON object
-        :rtype: JSON
+        :return: any or JSON object
+        :rtype: any or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
-                # response body for status code(s): 200
-                response == {
-                    "method": "str",  # The HTTP method applicable to the URL. Required.
-                    "url": "str",  # The signed URL. Required.
-                    "headers": {
-                        "str": "str"  # Optional. Mandatory headers that must be passed with
-                          the request.
-                    }
-                }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
                                 {}
                             ],
@@ -1597,19 +1520,18 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[JSON] = kwargs.pop("cls", None)
+        cls: ClsType[Union[Any, JSON]] = kwargs.pop("cls", None)
 
-        _request = build_datasets_upload_request(
+        _request = build_datasets_finalize_request(
             dataset_id=dataset_id,
-            artifact_path=artifact_path,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = (
@@ -1637,33 +1559,58 @@
         if response.status_code == 422:
             if response.content:
                 deserialized = response.json()
             else:
                 deserialized = None
 
         if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+            return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
 
-        return cast(JSON, deserialized)  # type: ignore
+        return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
-    async def finalize(self, dataset_id: str, **kwargs: Any) -> Union[Any, JSON]:
-        """Indicate that all dataset artifacts have been uploaded.
+    async def downlinks(
+        self, dataset_id: str, **kwargs: Any
+    ) -> Union[List[JSON], JSON]:
+        """Get a list of signed GET URLs from which Dataset artifacts can be downloaded.
 
-        Indicate that all dataset artifacts have been uploaded.
+        Get a list of signed GET URLs from which Dataset artifacts can be downloaded.
 
         :param dataset_id: Required.
         :type dataset_id: str
-        :return: any or JSON object
-        :rtype: any or JSON
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "artifact": {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
+                            "digest": {
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
+                            },
+                            "kind": "str"  # Optional. The kind of artifact.
+                        },
+                        "signedURL": {
+                            "method": "str",  # The HTTP method applicable to the URL.
+                              Required.
+                            "url": "str",  # The signed URL. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Mandatory headers that must
+                                  be passed with the request.
+                            }
+                        }
+                    }
+                ]
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
                                 {}
                             ],
@@ -1680,17 +1627,17 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[Union[Any, JSON]] = kwargs.pop("cls", None)
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
-        _request = build_datasets_finalize_request(
+        _request = build_datasets_downlinks_request(
             dataset_id=dataset_id,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
@@ -1719,17 +1666,17 @@
         if response.status_code == 422:
             if response.content:
                 deserialized = response.json()
             else:
                 deserialized = None
 
         if cls:
-            return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
 
-        return cast(Union[Any, JSON], deserialized)  # type: ignore
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
     async def documentation(self, dataset_id: str, **kwargs: Any) -> JSON:
         # pylint: disable=line-too-long
         """Get the documentation associated with a Dataset.
 
         Get the documentation associated with a Dataset. Raises a 404
@@ -3827,14 +3774,122 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
+    @distributed_trace_async
+    async def downlinks(
+        self, evaluation_id: str, **kwargs: Any
+    ) -> Union[List[JSON], JSON]:
+        """Get a list of signed GET URLs from which Evaluation artifacts can be
+        downloaded.
+
+        Get a list of signed GET URLs from which Evaluation artifacts can be downloaded.
+
+        :param evaluation_id: Required.
+        :type evaluation_id: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "artifact": {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
+                            "digest": {
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
+                            },
+                            "kind": "str"  # Optional. The kind of artifact.
+                        },
+                        "signedURL": {
+                            "method": "str",  # The HTTP method applicable to the URL.
+                              Required.
+                            "url": "str",  # The signed URL. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Mandatory headers that must
+                                  be passed with the request.
+                            }
+                        }
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_evaluations_downlinks_request(
+            evaluation_id=evaluation_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
+
 
 class InferenceservicesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -8138,17 +8193,20 @@
         self,
         *,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
-        analysis: Optional[str] = None,
         method: Optional[str] = None,
         method_name: Optional[str] = None,
+        dataset: Optional[str] = None,
+        evaluation: Optional[str] = None,
+        inference_service: Optional[str] = None,
+        model: Optional[str] = None,
         inputs_any_of: Optional[str] = None,
         **kwargs: Any,
     ) -> Union[List[JSON], JSON]:
         # pylint: disable=line-too-long
         """Get all Measurements matching a query.
 
         Get all Measurements matching a query. The query is a set of equality
@@ -8160,20 +8218,26 @@
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
         :paramtype reason: str
         :keyword labels: Default value is None.
         :paramtype labels: str
-        :keyword analysis: Default value is None.
-        :paramtype analysis: str
         :keyword method: Default value is None.
         :paramtype method: str
         :keyword method_name: Default value is None.
         :paramtype method_name: str
+        :keyword dataset: Default value is None.
+        :paramtype dataset: str
+        :keyword evaluation: Default value is None.
+        :paramtype evaluation: str
+        :keyword inference_service: Default value is None.
+        :paramtype inference_service: str
+        :keyword model: Default value is None.
+        :paramtype model: str
         :keyword inputs_any_of: Default value is None.
         :paramtype inputs_any_of: str
         :return: list of JSON object or JSON object
         :rtype: list[JSON] or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
@@ -8386,17 +8450,20 @@
 
         _request = build_measurements_query_request(
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
-            analysis=analysis,
             method=method,
             method_name=method_name,
+            dataset=dataset,
+            evaluation=evaluation,
+            inference_service=inference_service,
+            model=model,
             inputs_any_of=inputs_any_of,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
@@ -14111,14 +14178,119 @@
 
         if cls:
             return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
+    async def downlinks(self, module_id: str, **kwargs: Any) -> Union[List[JSON], JSON]:
+        """Get a list of signed GET URLs from which Module artifacts can be downloaded.
+
+        Get a list of signed GET URLs from which Module artifacts can be downloaded.
+
+        :param module_id: Required.
+        :type module_id: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "artifact": {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
+                            "digest": {
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
+                            },
+                            "kind": "str"  # Optional. The kind of artifact.
+                        },
+                        "signedURL": {
+                            "method": "str",  # The HTTP method applicable to the URL.
+                              Required.
+                            "url": "str",  # The signed URL. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Mandatory headers that must
+                                  be passed with the request.
+                            }
+                        }
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_modules_downlinks_request(
+            module_id=module_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
+
+    @distributed_trace_async
     async def documentation(self, module_id: str, **kwargs: Any) -> JSON:
         # pylint: disable=line-too-long
         """Get the documentation associated with a Module.
 
         Get the documentation associated with a Module. Raises a 404
         error if no entity exists with that key.
 
@@ -15703,30 +15875,51 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace_async
-    async def data(
-        self, report_id: str, **kwargs: Any
-    ) -> Union[AsyncIterator[bytes], JSON]:
-        """Get the raw data for the Report.
+    async def downlinks(self, report_id: str, **kwargs: Any) -> Union[List[JSON], JSON]:
+        """Get a list of signed GET URLs from which Report artifacts can be downloaded.
 
-        Get the raw data for the Report.
+        Get a list of signed GET URLs from which Report artifacts can be downloaded.
 
         :param report_id: Required.
         :type report_id: str
-        :return: AsyncIterator[bytes] or JSON object or None
-        :rtype: AsyncIterator[bytes] or JSON or None
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "artifact": {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
+                            "digest": {
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
+                            },
+                            "kind": "str"  # Optional. The kind of artifact.
+                        },
+                        "signedURL": {
+                            "method": "str",  # The HTTP method applicable to the URL.
+                              Required.
+                            "url": "str",  # The signed URL. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Mandatory headers that must
+                                  be passed with the request.
+                            }
+                        }
+                    }
+                ]
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
                                 {}
                             ],
@@ -15743,51 +15936,56 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[Union[AsyncIterator[bytes], JSON]] = kwargs.pop("cls", None)
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
-        _request = build_reports_data_request(
+        _request = build_reports_downlinks_request(
             report_id=report_id,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
-        _stream = True
+        _stream = False
         pipeline_response: PipelineResponse = (
             await self._client._pipeline.run(  # pylint: disable=protected-access
                 _request, stream=_stream, **kwargs
             )
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 404, 422]:
+        if response.status_code not in [200, 422]:
             if _stream:
                 await response.read()  # Load the body in memory and close the socket
             map_error(
                 status_code=response.status_code, response=response, error_map=error_map
             )
             raise HttpResponseError(response=response)
 
-        deserialized = None
         if response.status_code == 200:
-            deserialized = response.iter_bytes()
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
 
         if response.status_code == 422:
-            deserialized = response.iter_bytes()
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
 
         if cls:
-            return cls(pipeline_response, deserialized, {})  # type: ignore
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
 
-        return deserialized  # type: ignore
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
 
 
 class SafetycasesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
@@ -16022,17 +16220,20 @@
         self,
         *,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
-        analysis: Optional[str] = None,
         method: Optional[str] = None,
         method_name: Optional[str] = None,
+        dataset: Optional[str] = None,
+        evaluation: Optional[str] = None,
+        inference_service: Optional[str] = None,
+        model: Optional[str] = None,
         inputs_any_of: Optional[str] = None,
         **kwargs: Any,
     ) -> Union[List[JSON], JSON]:
         # pylint: disable=line-too-long
         """Get all SafetyCase entities matching a query.
 
         Get all SafetyCase entities matching a query. The query is a set of equality
@@ -16044,20 +16245,26 @@
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
         :paramtype reason: str
         :keyword labels: Default value is None.
         :paramtype labels: str
-        :keyword analysis: Default value is None.
-        :paramtype analysis: str
         :keyword method: Default value is None.
         :paramtype method: str
         :keyword method_name: Default value is None.
         :paramtype method_name: str
+        :keyword dataset: Default value is None.
+        :paramtype dataset: str
+        :keyword evaluation: Default value is None.
+        :paramtype evaluation: str
+        :keyword inference_service: Default value is None.
+        :paramtype inference_service: str
+        :keyword model: Default value is None.
+        :paramtype model: str
         :keyword inputs_any_of: Default value is None.
         :paramtype inputs_any_of: str
         :return: list of JSON object or JSON object
         :rtype: list[JSON] or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
@@ -16252,17 +16459,20 @@
 
         _request = build_safetycases_query_request(
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
-            analysis=analysis,
             method=method,
             method_name=method_name,
+            dataset=dataset,
+            evaluation=evaluation,
+            inference_service=inference_service,
+            model=model,
             inputs_any_of=inputs_any_of,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
```

### Comparing `dyff_client-0.4.2/dyff/client/_generated/aio/operations/_patch.py` & `dyff_client-0.5.0/dyff/client/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/operations/__init__.py` & `dyff_client-0.5.0/dyff/client/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/_generated/operations/_operations.py` & `dyff_client-0.5.0/dyff/client/_generated/operations/_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import sys
 from io import IOBase
 from typing import (
     IO,
     Any,
     Callable,
     Dict,
-    Iterator,
     List,
     Optional,
     Type,
     TypeVar,
     Union,
     cast,
     overload,
@@ -154,112 +153,93 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
-def build_datasets_strata_request(dataset_id: str, **kwargs: Any) -> HttpRequest:
+def build_datasets_delete_request(dataset_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = "/datasets/{dataset_id}/strata"
+    _url = "/datasets/{dataset_id}/delete"
     path_format_arguments = {
         "dataset_id": _SERIALIZER.url("dataset_id", dataset_id, "str"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+    return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
 
 
-def build_datasets_data_request(dataset_id: str, **kwargs: Any) -> HttpRequest:
+def build_datasets_upload_request(
+    dataset_id: str, artifact_path: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = "/datasets/{dataset_id}/data"
+    _url = "/datasets/{dataset_id}/upload/{artifact_path}"
     path_format_arguments = {
         "dataset_id": _SERIALIZER.url("dataset_id", dataset_id, "str"),
+        "artifact_path": _SERIALIZER.url("artifact_path", artifact_path, "str"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
-def build_datasets_delete_request(dataset_id: str, **kwargs: Any) -> HttpRequest:
+def build_datasets_finalize_request(dataset_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = "/datasets/{dataset_id}/delete"
+    _url = "/datasets/{dataset_id}/finalize"
     path_format_arguments = {
         "dataset_id": _SERIALIZER.url("dataset_id", dataset_id, "str"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-    return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
-def build_datasets_upload_request(
-    dataset_id: str, artifact_path: str, **kwargs: Any
-) -> HttpRequest:
+def build_datasets_downlinks_request(dataset_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = "/datasets/{dataset_id}/upload/{artifact_path}"
+    _url = "/datasets/{dataset_id}/downlinks"
     path_format_arguments = {
         "dataset_id": _SERIALIZER.url("dataset_id", dataset_id, "str"),
-        "artifact_path": _SERIALIZER.url("artifact_path", artifact_path, "str"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
-def build_datasets_finalize_request(dataset_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/datasets/{dataset_id}/finalize"
-    path_format_arguments = {
-        "dataset_id": _SERIALIZER.url("dataset_id", dataset_id, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
-
-
 def build_datasets_documentation_request(dataset_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/datasets/{dataset_id}/documentation"
@@ -440,14 +420,35 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
 
 
+def build_evaluations_downlinks_request(
+    evaluation_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/evaluations/{evaluation_id}/downlinks"
+    path_format_arguments = {
+        "evaluation_id": _SERIALIZER.url("evaluation_id", evaluation_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
 def build_inferenceservices_label_request(
     service_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop(
         "content_type", _headers.pop("Content-Type", None)
@@ -889,17 +890,20 @@
 def build_measurements_query_request(
     *,
     id: Optional[str] = None,
     account: Optional[str] = None,
     status: Optional[str] = None,
     reason: Optional[str] = None,
     labels: Optional[str] = None,
-    analysis: Optional[str] = None,
     method: Optional[str] = None,
     method_name: Optional[str] = None,
+    dataset: Optional[str] = None,
+    evaluation: Optional[str] = None,
+    inference_service: Optional[str] = None,
+    model: Optional[str] = None,
     inputs_any_of: Optional[str] = None,
     **kwargs: Any,
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
@@ -914,20 +918,28 @@
         _params["account"] = _SERIALIZER.query("account", account, "str")
     if status is not None:
         _params["status"] = _SERIALIZER.query("status", status, "str")
     if reason is not None:
         _params["reason"] = _SERIALIZER.query("reason", reason, "str")
     if labels is not None:
         _params["labels"] = _SERIALIZER.query("labels", labels, "str")
-    if analysis is not None:
-        _params["analysis"] = _SERIALIZER.query("analysis", analysis, "str")
     if method is not None:
         _params["method"] = _SERIALIZER.query("method", method, "str")
     if method_name is not None:
         _params["methodName"] = _SERIALIZER.query("method_name", method_name, "str")
+    if dataset is not None:
+        _params["dataset"] = _SERIALIZER.query("dataset", dataset, "str")
+    if evaluation is not None:
+        _params["evaluation"] = _SERIALIZER.query("evaluation", evaluation, "str")
+    if inference_service is not None:
+        _params["inferenceService"] = _SERIALIZER.query(
+            "inference_service", inference_service, "str"
+        )
+    if model is not None:
+        _params["model"] = _SERIALIZER.query("model", model, "str")
     if inputs_any_of is not None:
         _params["inputsAnyOf"] = _SERIALIZER.query(
             "inputs_any_of", inputs_any_of, "str"
         )
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
@@ -1528,14 +1540,33 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
+def build_modules_downlinks_request(module_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/modules/{module_id}/downlinks"
+    path_format_arguments = {
+        "module_id": _SERIALIZER.url("module_id", module_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
 def build_modules_documentation_request(module_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/modules/{module_id}/documentation"
@@ -1714,21 +1745,21 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
 
 
-def build_reports_data_request(report_id: str, **kwargs: Any) -> HttpRequest:
+def build_reports_downlinks_request(report_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = "/reports/{report_id}/data"
+    _url = "/reports/{report_id}/downlinks"
     path_format_arguments = {
         "report_id": _SERIALIZER.url("report_id", report_id, "str"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
@@ -1766,17 +1797,20 @@
 def build_safetycases_query_request(
     *,
     id: Optional[str] = None,
     account: Optional[str] = None,
     status: Optional[str] = None,
     reason: Optional[str] = None,
     labels: Optional[str] = None,
-    analysis: Optional[str] = None,
     method: Optional[str] = None,
     method_name: Optional[str] = None,
+    dataset: Optional[str] = None,
+    evaluation: Optional[str] = None,
+    inference_service: Optional[str] = None,
+    model: Optional[str] = None,
     inputs_any_of: Optional[str] = None,
     **kwargs: Any,
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
@@ -1791,20 +1825,28 @@
         _params["account"] = _SERIALIZER.query("account", account, "str")
     if status is not None:
         _params["status"] = _SERIALIZER.query("status", status, "str")
     if reason is not None:
         _params["reason"] = _SERIALIZER.query("reason", reason, "str")
     if labels is not None:
         _params["labels"] = _SERIALIZER.query("labels", labels, "str")
-    if analysis is not None:
-        _params["analysis"] = _SERIALIZER.query("analysis", analysis, "str")
     if method is not None:
         _params["method"] = _SERIALIZER.query("method", method, "str")
     if method_name is not None:
         _params["methodName"] = _SERIALIZER.query("method_name", method_name, "str")
+    if dataset is not None:
+        _params["dataset"] = _SERIALIZER.query("dataset", dataset, "str")
+    if evaluation is not None:
+        _params["evaluation"] = _SERIALIZER.query("evaluation", evaluation, "str")
+    if inference_service is not None:
+        _params["inferenceService"] = _SERIALIZER.query(
+            "inference_service", inference_service, "str"
+        )
+    if model is not None:
+        _params["model"] = _SERIALIZER.query("model", model, "str")
     if inputs_any_of is not None:
         _params["inputsAnyOf"] = _SERIALIZER.query(
             "inputs_any_of", inputs_any_of, "str"
         )
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
@@ -3072,107 +3114,33 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace
-    def strata(self, dataset_id: str, **kwargs: Any) -> Union[Iterator[bytes], JSON]:
-        """Get the strata corresponding to a Dataset.
+    def delete(self, dataset_id: str, **kwargs: Any) -> JSON:
+        """Mark a Dataset for deletion.
 
-        Get the strata corresponding to a Dataset. The data is returned as a
-        Parquet file suitable for reading with libraries like Pandas.
+        Mark a Dataset for deletion.
 
         :param dataset_id: Required.
         :type dataset_id: str
-        :return: Iterator[bytes] or JSON object or None
-        :rtype: Iterator[bytes] or JSON or None
+        :return: JSON object
+        :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
-                # response body for status code(s): 422
+                # response body for status code(s): 200
                 response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
+                    "reason": "str",  # Optional. Reason for current status (assigned by system).
+                    "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
-        """
-        error_map: MutableMapping[int, Type[HttpResponseError]] = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = kwargs.pop("params", {}) or {}
-
-        cls: ClsType[Union[Iterator[bytes], JSON]] = kwargs.pop("cls", None)
-
-        _request = build_datasets_strata_request(
-            dataset_id=dataset_id,
-            headers=_headers,
-            params=_params,
-        )
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = True
-        pipeline_response: PipelineResponse = (
-            self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
-            )
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 404, 422]:
-            if _stream:
-                response.read()  # Load the body in memory and close the socket
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
-            raise HttpResponseError(response=response)
-
-        deserialized = None
-        if response.status_code == 200:
-            deserialized = response.iter_bytes()
-
-        if response.status_code == 422:
-            deserialized = response.iter_bytes()
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})  # type: ignore
-
-        return deserialized  # type: ignore
-
-    @distributed_trace
-    def data(self, dataset_id: str, **kwargs: Any) -> Union[Iterator[bytes], JSON]:
-        """Get the raw data for the Dataset.
-
-        Get the raw data for the Dataset. The data is streamed in pyarrow.ipc
-        format.
-
-        :param dataset_id: Required.
-        :type dataset_id: str
-        :return: Iterator[bytes] or JSON object or None
-        :rtype: Iterator[bytes] or JSON or None
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
                                 {}
                             ],
@@ -3189,71 +3157,82 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[Union[Iterator[bytes], JSON]] = kwargs.pop("cls", None)
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        _request = build_datasets_data_request(
+        _request = build_datasets_delete_request(
             dataset_id=dataset_id,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
-        _stream = True
+        _stream = False
         pipeline_response: PipelineResponse = (
             self._client._pipeline.run(  # pylint: disable=protected-access
                 _request, stream=_stream, **kwargs
             )
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 404, 422]:
+        if response.status_code not in [200, 422]:
             if _stream:
                 response.read()  # Load the body in memory and close the socket
             map_error(
                 status_code=response.status_code, response=response, error_map=error_map
             )
             raise HttpResponseError(response=response)
 
-        deserialized = None
         if response.status_code == 200:
-            deserialized = response.iter_bytes()
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
 
         if response.status_code == 422:
-            deserialized = response.iter_bytes()
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
 
         if cls:
-            return cls(pipeline_response, deserialized, {})  # type: ignore
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
-        return deserialized  # type: ignore
+        return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace
-    def delete(self, dataset_id: str, **kwargs: Any) -> JSON:
-        """Mark a Dataset for deletion.
+    def upload(self, dataset_id: str, artifact_path: str, **kwargs: Any) -> JSON:
+        """Get a signed URL to which the given artifact can be uploaded.
 
-        Mark a Dataset for deletion.
+        Get a signed URL to which the given artifact can be uploaded.
 
         :param dataset_id: Required.
         :type dataset_id: str
+        :param artifact_path: Required.
+        :type artifact_path: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
-                    "reason": "str",  # Optional. Reason for current status (assigned by system).
-                    "status": "str"  # Optional. Top-level resource status (assigned by system).
+                    "method": "str",  # The HTTP method applicable to the URL. Required.
+                    "url": "str",  # The signed URL. Required.
+                    "headers": {
+                        "str": "str"  # Optional. Mandatory headers that must be passed with
+                          the request.
+                    }
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
                                 {}
@@ -3273,16 +3252,17 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        _request = build_datasets_delete_request(
+        _request = build_datasets_upload_request(
             dataset_id=dataset_id,
+            artifact_path=artifact_path,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = (
@@ -3315,39 +3295,28 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace
-    def upload(self, dataset_id: str, artifact_path: str, **kwargs: Any) -> JSON:
-        """Get a signed URL to which the given artifact can be uploaded.
+    def finalize(self, dataset_id: str, **kwargs: Any) -> Union[Any, JSON]:
+        """Indicate that all dataset artifacts have been uploaded.
 
-        Get a signed URL to which the given artifact can be uploaded.
+        Indicate that all dataset artifacts have been uploaded.
 
         :param dataset_id: Required.
         :type dataset_id: str
-        :param artifact_path: Required.
-        :type artifact_path: str
-        :return: JSON object
-        :rtype: JSON
+        :return: any or JSON object
+        :rtype: any or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
-                # response body for status code(s): 200
-                response == {
-                    "method": "str",  # The HTTP method applicable to the URL. Required.
-                    "url": "str",  # The signed URL. Required.
-                    "headers": {
-                        "str": "str"  # Optional. Mandatory headers that must be passed with
-                          the request.
-                    }
-                }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
                                 {}
                             ],
@@ -3364,19 +3333,18 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[JSON] = kwargs.pop("cls", None)
+        cls: ClsType[Union[Any, JSON]] = kwargs.pop("cls", None)
 
-        _request = build_datasets_upload_request(
+        _request = build_datasets_finalize_request(
             dataset_id=dataset_id,
-            artifact_path=artifact_path,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = (
@@ -3404,33 +3372,56 @@
         if response.status_code == 422:
             if response.content:
                 deserialized = response.json()
             else:
                 deserialized = None
 
         if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+            return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
 
-        return cast(JSON, deserialized)  # type: ignore
+        return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace
-    def finalize(self, dataset_id: str, **kwargs: Any) -> Union[Any, JSON]:
-        """Indicate that all dataset artifacts have been uploaded.
+    def downlinks(self, dataset_id: str, **kwargs: Any) -> Union[List[JSON], JSON]:
+        """Get a list of signed GET URLs from which Dataset artifacts can be downloaded.
 
-        Indicate that all dataset artifacts have been uploaded.
+        Get a list of signed GET URLs from which Dataset artifacts can be downloaded.
 
         :param dataset_id: Required.
         :type dataset_id: str
-        :return: any or JSON object
-        :rtype: any or JSON
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "artifact": {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
+                            "digest": {
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
+                            },
+                            "kind": "str"  # Optional. The kind of artifact.
+                        },
+                        "signedURL": {
+                            "method": "str",  # The HTTP method applicable to the URL.
+                              Required.
+                            "url": "str",  # The signed URL. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Mandatory headers that must
+                                  be passed with the request.
+                            }
+                        }
+                    }
+                ]
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
                                 {}
                             ],
@@ -3447,17 +3438,17 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[Union[Any, JSON]] = kwargs.pop("cls", None)
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
-        _request = build_datasets_finalize_request(
+        _request = build_datasets_downlinks_request(
             dataset_id=dataset_id,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
@@ -3486,17 +3477,17 @@
         if response.status_code == 422:
             if response.content:
                 deserialized = response.json()
             else:
                 deserialized = None
 
         if cls:
-            return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
 
-        return cast(Union[Any, JSON], deserialized)  # type: ignore
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
 
     @distributed_trace
     def documentation(self, dataset_id: str, **kwargs: Any) -> JSON:
         # pylint: disable=line-too-long
         """Get the documentation associated with a Dataset.
 
         Get the documentation associated with a Dataset. Raises a 404
@@ -5594,14 +5585,120 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
+    @distributed_trace
+    def downlinks(self, evaluation_id: str, **kwargs: Any) -> Union[List[JSON], JSON]:
+        """Get a list of signed GET URLs from which Evaluation artifacts can be
+        downloaded.
+
+        Get a list of signed GET URLs from which Evaluation artifacts can be downloaded.
+
+        :param evaluation_id: Required.
+        :type evaluation_id: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "artifact": {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
+                            "digest": {
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
+                            },
+                            "kind": "str"  # Optional. The kind of artifact.
+                        },
+                        "signedURL": {
+                            "method": "str",  # The HTTP method applicable to the URL.
+                              Required.
+                            "url": "str",  # The signed URL. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Mandatory headers that must
+                                  be passed with the request.
+                            }
+                        }
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_evaluations_downlinks_request(
+            evaluation_id=evaluation_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
+
 
 class InferenceservicesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -9905,17 +10002,20 @@
         self,
         *,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
-        analysis: Optional[str] = None,
         method: Optional[str] = None,
         method_name: Optional[str] = None,
+        dataset: Optional[str] = None,
+        evaluation: Optional[str] = None,
+        inference_service: Optional[str] = None,
+        model: Optional[str] = None,
         inputs_any_of: Optional[str] = None,
         **kwargs: Any,
     ) -> Union[List[JSON], JSON]:
         # pylint: disable=line-too-long
         """Get all Measurements matching a query.
 
         Get all Measurements matching a query. The query is a set of equality
@@ -9927,20 +10027,26 @@
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
         :paramtype reason: str
         :keyword labels: Default value is None.
         :paramtype labels: str
-        :keyword analysis: Default value is None.
-        :paramtype analysis: str
         :keyword method: Default value is None.
         :paramtype method: str
         :keyword method_name: Default value is None.
         :paramtype method_name: str
+        :keyword dataset: Default value is None.
+        :paramtype dataset: str
+        :keyword evaluation: Default value is None.
+        :paramtype evaluation: str
+        :keyword inference_service: Default value is None.
+        :paramtype inference_service: str
+        :keyword model: Default value is None.
+        :paramtype model: str
         :keyword inputs_any_of: Default value is None.
         :paramtype inputs_any_of: str
         :return: list of JSON object or JSON object
         :rtype: list[JSON] or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
@@ -10153,17 +10259,20 @@
 
         _request = build_measurements_query_request(
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
-            analysis=analysis,
             method=method,
             method_name=method_name,
+            dataset=dataset,
+            evaluation=evaluation,
+            inference_service=inference_service,
+            model=model,
             inputs_any_of=inputs_any_of,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
@@ -15876,14 +15985,119 @@
 
         if cls:
             return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace
+    def downlinks(self, module_id: str, **kwargs: Any) -> Union[List[JSON], JSON]:
+        """Get a list of signed GET URLs from which Module artifacts can be downloaded.
+
+        Get a list of signed GET URLs from which Module artifacts can be downloaded.
+
+        :param module_id: Required.
+        :type module_id: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "artifact": {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
+                            "digest": {
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
+                            },
+                            "kind": "str"  # Optional. The kind of artifact.
+                        },
+                        "signedURL": {
+                            "method": "str",  # The HTTP method applicable to the URL.
+                              Required.
+                            "url": "str",  # The signed URL. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Mandatory headers that must
+                                  be passed with the request.
+                            }
+                        }
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_modules_downlinks_request(
+            module_id=module_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
+
+    @distributed_trace
     def documentation(self, module_id: str, **kwargs: Any) -> JSON:
         # pylint: disable=line-too-long
         """Get the documentation associated with a Module.
 
         Get the documentation associated with a Module. Raises a 404
         error if no entity exists with that key.
 
@@ -17468,28 +17682,51 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace
-    def data(self, report_id: str, **kwargs: Any) -> Union[Iterator[bytes], JSON]:
-        """Get the raw data for the Report.
+    def downlinks(self, report_id: str, **kwargs: Any) -> Union[List[JSON], JSON]:
+        """Get a list of signed GET URLs from which Report artifacts can be downloaded.
 
-        Get the raw data for the Report.
+        Get a list of signed GET URLs from which Report artifacts can be downloaded.
 
         :param report_id: Required.
         :type report_id: str
-        :return: Iterator[bytes] or JSON object or None
-        :rtype: Iterator[bytes] or JSON or None
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "artifact": {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
+                            "digest": {
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
+                            },
+                            "kind": "str"  # Optional. The kind of artifact.
+                        },
+                        "signedURL": {
+                            "method": "str",  # The HTTP method applicable to the URL.
+                              Required.
+                            "url": "str",  # The signed URL. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Mandatory headers that must
+                                  be passed with the request.
+                            }
+                        }
+                    }
+                ]
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
                                 {}
                             ],
@@ -17506,51 +17743,56 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[Union[Iterator[bytes], JSON]] = kwargs.pop("cls", None)
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
-        _request = build_reports_data_request(
+        _request = build_reports_downlinks_request(
             report_id=report_id,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
-        _stream = True
+        _stream = False
         pipeline_response: PipelineResponse = (
             self._client._pipeline.run(  # pylint: disable=protected-access
                 _request, stream=_stream, **kwargs
             )
         )
 
         response = pipeline_response.http_response
 
-        if response.status_code not in [200, 404, 422]:
+        if response.status_code not in [200, 422]:
             if _stream:
                 response.read()  # Load the body in memory and close the socket
             map_error(
                 status_code=response.status_code, response=response, error_map=error_map
             )
             raise HttpResponseError(response=response)
 
-        deserialized = None
         if response.status_code == 200:
-            deserialized = response.iter_bytes()
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
 
         if response.status_code == 422:
-            deserialized = response.iter_bytes()
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
 
         if cls:
-            return cls(pipeline_response, deserialized, {})  # type: ignore
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
 
-        return deserialized  # type: ignore
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
 
 
 class SafetycasesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
@@ -17785,17 +18027,20 @@
         self,
         *,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
-        analysis: Optional[str] = None,
         method: Optional[str] = None,
         method_name: Optional[str] = None,
+        dataset: Optional[str] = None,
+        evaluation: Optional[str] = None,
+        inference_service: Optional[str] = None,
+        model: Optional[str] = None,
         inputs_any_of: Optional[str] = None,
         **kwargs: Any,
     ) -> Union[List[JSON], JSON]:
         # pylint: disable=line-too-long
         """Get all SafetyCase entities matching a query.
 
         Get all SafetyCase entities matching a query. The query is a set of equality
@@ -17807,20 +18052,26 @@
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
         :paramtype reason: str
         :keyword labels: Default value is None.
         :paramtype labels: str
-        :keyword analysis: Default value is None.
-        :paramtype analysis: str
         :keyword method: Default value is None.
         :paramtype method: str
         :keyword method_name: Default value is None.
         :paramtype method_name: str
+        :keyword dataset: Default value is None.
+        :paramtype dataset: str
+        :keyword evaluation: Default value is None.
+        :paramtype evaluation: str
+        :keyword inference_service: Default value is None.
+        :paramtype inference_service: str
+        :keyword model: Default value is None.
+        :paramtype model: str
         :keyword inputs_any_of: Default value is None.
         :paramtype inputs_any_of: str
         :return: list of JSON object or JSON object
         :rtype: list[JSON] or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
@@ -18015,17 +18266,20 @@
 
         _request = build_safetycases_query_request(
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
-            analysis=analysis,
             method=method,
             method_name=method_name,
+            dataset=dataset,
+            evaluation=evaluation,
+            inference_service=inference_service,
+            model=model,
             inputs_any_of=inputs_any_of,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
```

### Comparing `dyff_client-0.4.2/dyff/client/_generated/operations/_patch.py` & `dyff_client-0.5.0/dyff/client/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/dyff/client/client.py` & `dyff_client-0.5.0/dyff/client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
 # mypy: disable-error-code="import-untyped"
 from __future__ import annotations
 
 import json
-import pathlib
 import sys
 import time
-from io import BytesIO
+from pathlib import Path
 from typing import Any, Callable, Optional, TypeVar
 from warnings import warn
 
 import httpx
-import pandas
-import pyarrow.dataset
 from azure.core.credentials import AccessToken, TokenCredential
 
 # We bring this into our namespace so that people can catch it without being
 # confused by having to import 'azure.core'
 from azure.core.exceptions import HttpResponseError
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.policies import BearerTokenCredentialPolicy
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 
 from dyff.schema.adapters import Adapter, create_pipeline
 from dyff.schema.dataset import arrow, binary
 from dyff.schema.platform import (
     Artifact,
+    ArtifactURL,
     DataSchema,
     Dataset,
     Digest,
     Documentation,
     DyffEntity,
     Evaluation,
     InferenceInterface,
@@ -161,14 +159,43 @@
                     retries += 1
                 else:
                     raise
 
     return _impl
 
 
+def _downlinks(raw_ops, resource_id: str) -> list[ArtifactURL]:
+    return [ArtifactURL.parse_obj(link) for link in raw_ops.downlinks(resource_id)]
+
+
+def _download(
+    ops, resource_id: str, destination: Path | str, *, insecure: bool = False
+) -> None:
+    destination = Path(destination).resolve()
+    if not destination.is_dir():
+        raise ValueError("destination must be am empty directory")
+    empty = not any(destination.iterdir())
+    if not empty:
+        raise ValueError("destination must be an empty directory")
+    links = ops.downlinks(resource_id)
+    for link in links:
+        file_path = destination / link.artifact.path
+        if file_path.is_dir():
+            # Sometimes paths like "." get included because s3 is weird
+            continue
+        file_path.parent.mkdir(parents=True, exist_ok=True)
+        with open(file_path, "wb") as fout:
+            response = httpx.get(
+                link.signedURL.url,
+                headers=link.signedURL.headers,
+                verify=not insecure,
+            )
+            fout.write(response.content)
+
+
 class InferenceSessionClient:
     """A client used for making inference requests to a running
     :class:`~dyff.schema.platform.InferenceSession`.
 
     .. note::
 
       Do not instantiate this class. Create an instance using
@@ -228,22 +255,31 @@
 
         def once(x):
             yield x
 
         body = once(body)
         if self._input_adapter is not None:
             body = self._input_adapter(body)
-        for x in body:
-            request = self._client.build_request("POST", url, headers=headers, json=x)
-            response = self._client.send(request, stream=True)
-            response.raise_for_status()
-            response.read()
-            json_response = once(response.json())
-            if self._output_adapter is not None:
-                json_response = self._output_adapter(json_response)
+        request_body = None
+        for i, x in enumerate(body):
+            if i > 0:
+                raise ValueError("adapted input should contain exactly one element")
+            request_body = x
+        if request_body is None:
+            raise ValueError("adapted input should contain exactly one element")
+
+        request = self._client.build_request(
+            "POST", url, headers=headers, json=request_body
+        )
+        response = self._client.send(request, stream=True)
+        response.raise_for_status()
+        response.read()
+        json_response = once(response.json())
+        if self._output_adapter is not None:
+            json_response = self._output_adapter(json_response)
         return list(json_response)
 
 
 class DatasetsOperations:
     """Operations on :class:`~dyff.schema.platform.Dataset` entities.
 
     .. note::
@@ -347,68 +383,28 @@
         :type labels: dict[str, Optional[str]]
         """
         if not labels:
             return
         labels = LabelUpdateRequest(labels=labels).dict()
         self._raw_ops.label(dataset_id, labels)
 
-    def strata(self, dataset: Dataset | str) -> pandas.DataFrame:
-        """Fetch the strata of the dataset.
-
-        :param dataset: The identifier of the dataset
-        :type dataset: Dataset | str
-        :return: The strata of the dataset
-        """
-        dataset = _require_id(dataset)
-        stream = self._raw_ops.strata(dataset)
-        blob = bytearray()
-        for chunk in stream:
-            blob.extend(chunk)  # type: ignore
-        with BytesIO(blob) as fin:
-            return pandas.read_parquet(fin)
-
-    def data(self, dataset: Dataset | str) -> pyarrow.dataset.Scanner:
-        """Fetch the raw data of the dataset.
-
-        The data is returned as a read-once pyarrow Dataset.
-
-        :param dataset: The identifier of the dataset
-        :type dataset: Dataset | str
-        :return: The strata of the dataset
-        """
-        dataset = _require_id(dataset)
-        stream = self._raw_ops.data(dataset)
-        buffer = bytearray()
-        for chunk in stream:
-            buffer.extend(chunk)  # type: ignore
-        with pyarrow.ipc.open_stream(buffer) as reader:
-            # Note: We should be able to pass 'reader' to 'from_batches()' directly
-            # because it's already a batch generator, but if we do that then the
-            # generator sometimes blocks program exit for some reason.
-            def batch_generator():
-                yield from reader
-
-            return pyarrow.dataset.Scanner.from_batches(
-                batch_generator(), schema=reader.schema
-            )
-
     def create(self, dataset_request: DatasetCreateRequest) -> Dataset:
         """Create a Dataset.
 
         .. note::
             This operation may incur compute costs.
 
         :param dataset_request: The dataset request specification.
         :type dataset_request: DatasetCreateRequest
         :return: A full Dataset entity with .id and other properties set.
         """
         return Dataset.parse_obj(self._raw_ops.create(dataset_request.dict()))
 
     def create_arrow_dataset(
-        self, dataset_directory: str, *, account: str, name: str
+        self, dataset_directory: Path | str, *, account: str, name: str
     ) -> Dataset:
         """Create a Dataset resource describing an existing Arrow dataset.
 
         Internally, constructs a ``DatasetCreateRequest`` using information
         obtained from the Arrow dataset, then calls ``create()`` with the
         constructed request.
 
@@ -422,20 +418,19 @@
         :keyword account: The account that will own the Dataset resource.
         :type account: str
         :keyword name: The name of the Dataset resource.
         :type name: str
         :returns: The complete Dataset resource.
         :rtype: Dataset
         """
-        dataset_path = pathlib.Path(dataset_directory)
+        dataset_path = Path(dataset_directory)
         ds = arrow.open_dataset(str(dataset_path))
         file_paths = list(ds.files)
         artifact_paths = [
-            str(pathlib.Path(file_path).relative_to(dataset_path))
-            for file_path in file_paths
+            str(Path(file_path).relative_to(dataset_path)) for file_path in file_paths
         ]
         artifacts = [
             Artifact(
                 kind="parquet",
                 path=artifact_path,
                 digest=Digest(
                     md5=binary.encode(binary.file_digest("md5", file_path)),
@@ -450,15 +445,17 @@
             account=account,
             name=name,
             artifacts=artifacts,
             schema=schema,
         )
         return self.create(request)
 
-    def upload_arrow_dataset(self, dataset: Dataset, dataset_directory: str) -> None:
+    def upload_arrow_dataset(
+        self, dataset: Dataset, dataset_directory: Path | str
+    ) -> None:
         """Uploads the data files in an existing Arrow dataset for which a Dataset
         resource has already been created.
 
         Typical usage::
 
             dataset = client.datasets.create_arrow_dataset(dataset_directory, ...)
             client.datasets.upload_arrow_dataset(dataset, dataset_directory)
@@ -468,15 +465,15 @@
         :param dataset_directory: The root directory of the Arrow dataset.
         :type dataset_directory: str
         """
         if any(artifact.digest.md5 is None for artifact in dataset.artifacts):
             raise ValueError("artifact.digest.md5 must be set for all artifacts")
         for artifact in dataset.artifacts:
             assert artifact.digest.md5 is not None
-            file_path = pathlib.Path(dataset_directory) / artifact.path
+            file_path = Path(dataset_directory) / artifact.path
             put_url_json = _retry_not_found(self._raw_ops.upload)(
                 dataset.id, artifact.path
             )
             put_url = StorageSignedURL.parse_obj(put_url_json)
             if put_url.method != "PUT":
                 raise ValueError(f"expected a PUT URL; got {put_url.method}")
             with open(file_path, "rb") as fin:
@@ -489,14 +486,39 @@
                     content=fin,
                     headers=headers,
                     verify=not self._insecure,
                 )
                 response.raise_for_status()
         _retry_not_found(self._raw_ops.finalize)(dataset.id)
 
+    def downlinks(self, dataset_id: str) -> list[ArtifactURL]:
+        """Get a list of signed GET URLs from which Dataset artifacts can be downloaded.
+
+        :param dataset_id: The ID of the Dataset.
+        :type dataset_id: str
+        :return: List of signed GET URLs.
+        :rtype: list[ArtifactURL] :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return _downlinks(self._raw_ops, dataset_id)
+
+    def download(self, dataset_id: str, destination: Path | str) -> None:
+        """Download all of the files in a dataset to a local directory.
+
+        The destination directory must be an empty directory that exists.
+
+        :param dataset_id: The ID of the Dataset.
+        :type dataset_id: str
+        :param destination: The destination directory. Must exist and be empty.
+        :type destination: Path | str
+        :raises ~azure.core.exceptions.HttpResponseError: If
+            ``datasets.downlinks(dataset_id)`` raises
+        :raises ValueError: If arguments are invalid
+        """
+        return _download(self, dataset_id, destination, insecure=self._insecure)
+
     def documentation(self, dataset_id: str) -> Documentation:
         """Get the documentation associated with a Dataset.
 
         Get the documentation associated with a Dataset. Raises a 404 error if no entity
         exists with that key.
 
         :param dataset_id: The ID of the Dataset.
@@ -535,16 +557,19 @@
 
     .. note::
 
       Do not instantiate this class. Access it through the
       ``.evaluations`` attribute of :class:`~dyff.client.Client`.
     """
 
-    def __init__(self, _raw_ops: EvaluationsOperationsGenerated):
+    def __init__(
+        self, _raw_ops: EvaluationsOperationsGenerated, *, insecure: bool = False
+    ):
         self._raw_ops = _raw_ops
+        self._insecure = insecure
 
     def get(self, evaluation_id: str) -> Evaluation:
         """Get an Evaluation by its key.
 
         :param evaluation_id: The evaluation id
         :type evaluation_id: str
         :return: The Evaluation with the given key.
@@ -646,14 +671,40 @@
         :param evaluation_request: The evaluation request specification.
         :type evaluation_request: EvaluationCreateRequest
         :return: A full Evaluation entity with .id and other properties set.
         """
         evaluation = _retry_not_found(self._raw_ops.create)(evaluation_request.dict())
         return Evaluation.parse_obj(evaluation)
 
+    def downlinks(self, evaluation_id: str) -> list[ArtifactURL]:
+        """Get a list of signed GET URLs from which Evaluation artifacts can be
+        downloaded.
+
+        :param evaluation_id: The ID of the Evaluation.
+        :type evaluation_id: str
+        :return: List of signed GET URLs.
+        :rtype: list[ArtifactURL] :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return _downlinks(self._raw_ops, evaluation_id)
+
+    def download(self, evaluation_id: str, destination: Path | str) -> None:
+        """Download all of the files in an evaluation to a local directory.
+
+        The destination directory must be an empty directory that exists.
+
+        :param evaluation_id: The ID of the Evaluation.
+        :type evaluation_id: str
+        :param destination: The destination directory. Must exist and be empty.
+        :type destination: Path | str
+        :raises ~azure.core.exceptions.HttpResponseError: If
+            ``evaluations.downlinks(evaluation_id)`` raises
+        :raises ValueError: If arguments are invalid
+        """
+        return _download(self, evaluation_id, destination, insecure=self._insecure)
+
 
 class InferenceservicesOperations:
     """Operations on :class:`~dyff.schema.platform.InferenceService` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
@@ -1057,16 +1108,19 @@
 
     .. note::
 
       Do not instantiate this class. Access it through the
       ``.measurements`` attribute of :class:`~dyff.client.Client`.
     """
 
-    def __init__(self, _raw_ops: MeasurementsOperationsGenerated):
+    def __init__(
+        self, _raw_ops: MeasurementsOperationsGenerated, *, insecure: bool = False
+    ):
         self._raw_ops = _raw_ops
+        self._insecure = insecure
 
     def get(self, measurement_id: str) -> Measurement:
         """Get a Measurement by its key.
 
         :param measurement_id: The Measurement ID
         :type measurement_id: str
         :return: The Measurement with the given ID.
@@ -1077,76 +1131,70 @@
         self,
         *,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
+        method: Optional[str] = None,
+        methodName: Optional[str] = None,
         dataset: Optional[str] = None,
-        dataset_name: Optional[str] = None,
         evaluation: Optional[str] = None,
-        inference_service: Optional[str] = None,
-        inference_service_name: Optional[str] = None,
-        method: Optional[str] = None,
-        method_name: Optional[str] = None,
+        inferenceService: Optional[str] = None,
         model: Optional[str] = None,
-        model_name: Optional[str] = None,
+        inputsAnyOf: Optional[list[str]] = None,
     ) -> list[Measurement]:
         """Get all Measurement entities matching a query. The query is a set of equality
         constraints specified as key-value pairs.
 
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
         :paramtype reason: str
         :keyword labels: Default value is None.
-        :paramtype labels: dict[str, str]
+        :paramtype labels: str
+        :keyword method: Default value is None.
+        :paramtype method: str
+        :keyword methodName: Default value is None.
+        :paramtype methodName: str
         :keyword dataset: Default value is None.
         :paramtype dataset: str
-        :keyword dataset_name: Default value is None.
-        :paramtype dataset_name: str
         :keyword evaluation: Default value is None.
         :paramtype evaluation: str
-        :keyword inference_service: Default value is None.
-        :paramtype inference_service: str
-        :keyword inference_service_name: Default value is None.
-        :paramtype inference_service_name: str
-        :keyword method: Default value is None.
-        :paramtype method: str
-        :keyword method_name: Default value is None.
-        :paramtype method_name: str
+        :keyword inferenceService: Default value is None.
+        :paramtype inferenceService: str
         :keyword model: Default value is None.
         :paramtype model: str
-        :keyword model_name: Default value is None.
-        :paramtype model_name: str
+        :keyword inputsAnyOf: Default value is None.
+        :paramtype inputsAnyOf: str
         :return: Entities matching the query
         :rtype: list[Measurement]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return [
             Measurement.parse_obj(obj)
             for obj in self._raw_ops.query(
                 id=id,
                 account=account,
                 status=status,
                 reason=reason,
                 labels=_encode_labels(labels),
+                method=method,
+                method_name=methodName,
                 dataset=dataset,
-                dataset_name=dataset_name,
                 evaluation=evaluation,
-                inference_service=inference_service,
-                inference_service_name=inference_service_name,
-                method=method,
-                method_name=method_name,
+                inference_service=inferenceService,
                 model=model,
-                model_name=model_name,
+                inputs_any_of=(
+                    ",".join(inputsAnyOf) if inputsAnyOf is not None else None
+                ),
             )
         ]
 
     def label(self, measurement_id: str, labels: dict[str, Optional[str]]) -> None:
         """Label the specified Measurement with key-value pairs (stored in the
         ``.labels`` field of the resource).
 
@@ -1171,14 +1219,40 @@
         :param analysis_request: The Measurement specification.
         :type analysis_request: AnalysisCreateRequest
         :return: A full Meausrement entity with .id and other properties set.
         """
         measurement = _retry_not_found(self._raw_ops.create)(analysis_request.dict())
         return Measurement.parse_obj(measurement)
 
+    def downlinks(self, measurement_id: str) -> list[ArtifactURL]:
+        """Get a list of signed GET URLs from which Measurement artifacts can be
+        downloaded.
+
+        :param measurement_id: The ID of the Measurement.
+        :type measurement_id: str
+        :return: List of signed GET URLs.
+        :rtype: list[ArtifactURL] :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return _downlinks(self._raw_ops, measurement_id)
+
+    def download(self, measurement_id: str, destination: Path | str) -> None:
+        """Download all of the files in a measurement to a local directory.
+
+        The destination directory must be an empty directory that exists.
+
+        :param measurement_id: The ID of the Measurement.
+        :type measurement_id: str
+        :param destination: The destination directory. Must exist and be empty.
+        :type destination: Path | str
+        :raises ~azure.core.exceptions.HttpResponseError: If
+            ``measurements.downlinks(measurement_id)`` raises
+        :raises ValueError: If arguments are invalid
+        """
+        return _download(self, measurement_id, destination, insecure=self._insecure)
+
 
 class MethodsOperations:
     """Operations on :class:`~dyff.schema.platform.Method` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
@@ -1570,15 +1644,15 @@
         :type module_request: ModuleCreateRequest
         :return: A full Module entity with .id and other properties set.
         """
         module = _retry_not_found(self._raw_ops.create)(module_request.dict())
         return Module.parse_obj(module)
 
     def create_package(
-        self, package_directory: str, *, account: str, name: str
+        self, package_directory: Path | str, *, account: str, name: str
     ) -> Module:
         """Create a Module resource describing a package structured as a directory tree.
 
         Internally, constructs a ``ModuleCreateRequest`` using information
         obtained from the directory tree, then calls ``create()`` with the
         constructed request.
 
@@ -1592,21 +1666,20 @@
         :keyword account: The account that will own the Module resource.
         :type account: str
         :keyword name: The name of the Module resource.
         :type name: str
         :returns: The complete Module resource.
         :rtype: Module
         """
-        package_root = pathlib.Path(package_directory)
+        package_root = Path(package_directory)
         file_paths = [path for path in package_root.rglob("*") if path.is_file()]
         if not file_paths:
             raise ValueError(f"package_directory is empty: {package_directory}")
         artifact_paths = [
-            str(pathlib.Path(file_path).relative_to(package_root))
-            for file_path in file_paths
+            str(Path(file_path).relative_to(package_root)) for file_path in file_paths
         ]
         artifacts = [
             Artifact(
                 # FIXME: Is this a useful thing to do? It's redundant with
                 # information in 'path'. Maybe it should just be 'code' or
                 # something generic.
                 kind="".join(file_path.suffixes),
@@ -1620,15 +1693,15 @@
         request = ModuleCreateRequest(
             account=account,
             name=name,
             artifacts=artifacts,
         )
         return self.create(request)
 
-    def upload_package(self, module: Module, package_directory: str) -> None:
+    def upload_package(self, module: Module, package_directory: Path | str) -> None:
         """Uploads the files in a package directory for which a Module resource has
         already been created.
 
         Typical usage::
 
             module = client.modules.create_package(package_directory, ...)
             client.modules.upload_package(module, package_directory)
@@ -1638,15 +1711,15 @@
         :param package_directory: The root directory of the package.
         :type package_directory: str
         """
         if any(artifact.digest.md5 is None for artifact in module.artifacts):
             raise ValueError("artifact.digest.md5 must be set for all artifacts")
         for artifact in module.artifacts:
             assert artifact.digest.md5 is not None
-            file_path = pathlib.Path(package_directory) / artifact.path
+            file_path = Path(package_directory) / artifact.path
             put_url_json = _retry_not_found(self._raw_ops.upload)(
                 module.id, artifact.path
             )
             put_url = StorageSignedURL.parse_obj(put_url_json)
             if put_url.method != "PUT":
                 raise ValueError(f"expected a PUT URL; got {put_url.method}")
             with open(file_path, "rb") as fin:
@@ -1659,14 +1732,39 @@
                     content=fin,
                     headers=headers,
                     verify=not self._insecure,
                 )
                 response.raise_for_status()
         _retry_not_found(self._raw_ops.finalize)(module.id)
 
+    def downlinks(self, module_id: str) -> list[ArtifactURL]:
+        """Get a list of signed GET URLs from which Module artifacts can be downloaded.
+
+        :param measurement_id: The ID of the Module.
+        :type measurement_id: str
+        :return: List of signed GET URLs.
+        :rtype: list[ArtifactURL] :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return _downlinks(self._raw_ops, module_id)
+
+    def download(self, module_id: str, destination: Path | str) -> None:
+        """Download all of the files in a module to a local directory.
+
+        The destination directory must be an empty directory that exists.
+
+        :param module_id: The ID of the Module.
+        :type module_id: str
+        :param destination: The destination directory. Must exist and be empty.
+        :type destination: Path | str
+        :raises ~azure.core.exceptions.HttpResponseError: If
+            ``modules.downlinks(module_id)`` raises
+        :raises ValueError: If arguments are invalid
+        """
+        return _download(self, module_id, destination, insecure=self._insecure)
+
     def documentation(self, module_id: str) -> Documentation:
         """Get the documentation associated with a Module.
 
         Get the documentation associated with a Module. Raises a 404 error if no entity
         exists with that key.
 
         :param module_id: The ID of the Module.
@@ -1705,16 +1803,17 @@
 
     .. note::
 
       Do not instantiate this class. Access it through the
       ``.reports`` attribute of :class:`~dyff.client.Client`.
     """
 
-    def __init__(self, _raw_ops: ReportsOperationsGenerated):
+    def __init__(self, _raw_ops: ReportsOperationsGenerated, *, insecure: bool = False):
         self._raw_ops = _raw_ops
+        self._insecure = insecure
 
     def get(self, report_id: str) -> Report:
         """Get a Report by its key.
 
         :param report_id: The report id
         :type report_id: str
         :return: The Report with the given key.
@@ -1816,41 +1915,54 @@
         :param report_request: The report specification.
         :type report: ReportCreateRequest
         :return: A full Report entity with .id and other properties set.
         """
         report = _retry_not_found(self._raw_ops.create)(report_request.dict())
         return Report.parse_obj(report)
 
-    def data(self, report: Report | str) -> pandas.DataFrame:
-        """Fetch the output data of the report.
+    def downlinks(self, report_id: str) -> list[ArtifactURL]:
+        """Get a list of signed GET URLs from which Report artifacts can be downloaded.
 
-        :param report: The identifier of the report
-        :type report: Report | str
-        :return: The output data of the report
-        """
-        report = _require_id(report)
-        stream = self._raw_ops.data(report)
-        blob = bytearray()
-        for chunk in stream:
-            blob.extend(chunk)  # type: ignore
-        with BytesIO(blob) as fin:
-            return pandas.read_parquet(fin)
+        :param report_id: The ID of the Report.
+        :type report_id: str
+        :return: List of signed GET URLs.
+        :rtype: list[ArtifactURL] :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return _downlinks(self._raw_ops, report_id)
+
+    def download(self, report_id: str, destination: Path | str) -> None:
+        """Download all of the files in a report to a local directory.
+
+        The destination directory must be an empty directory that exists.
+
+        :param report_id: The ID of the Report.
+        :type report_id: str
+        :param destination: The destination directory. Must exist and be empty.
+        :type destination: Path | str
+        :raises ~azure.core.exceptions.HttpResponseError: If
+            ``reports.downlinks(report_id)`` raises
+        :raises ValueError: If arguments are invalid
+        """
+        return _download(self, report_id, destination, insecure=self._insecure)
 
 
 class SafetycasesOperations:
     """Operations on :class:`~dyff.schema.platform.SafetyCase` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
       ``.safetycases`` attribute of :class:`~dyff.client.Client`.
     """
 
-    def __init__(self, _raw_ops: SafetycasesOperationsGenerated):
+    def __init__(
+        self, _raw_ops: SafetycasesOperationsGenerated, *, insecure: bool = False
+    ):
         self._raw_ops = _raw_ops
+        self._insecure = insecure
 
     def get(self, safetycase_id: str) -> SafetyCase:
         """Get a SafetyCase by its key.
 
         :param safetycase_id: The SafetyCase ID
         :type safetycase_id: str
         :return: The SafetyCase with the given ID.
@@ -1861,76 +1973,70 @@
         self,
         *,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
+        method: Optional[str] = None,
+        methodName: Optional[str] = None,
         dataset: Optional[str] = None,
-        dataset_name: Optional[str] = None,
         evaluation: Optional[str] = None,
-        inference_service: Optional[str] = None,
-        inference_service_name: Optional[str] = None,
-        method: Optional[str] = None,
-        method_name: Optional[str] = None,
+        inferenceService: Optional[str] = None,
         model: Optional[str] = None,
-        model_name: Optional[str] = None,
+        inputsAnyOf: Optional[str] = None,
     ) -> list[SafetyCase]:
         """Get all SafetyCase entities matching a query. The query is a set of equality
         constraints specified as key-value pairs.
 
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
         :paramtype reason: str
         :keyword labels: Default value is None.
-        :paramtype labels: dict[str, str]
+        :paramtype labels: str
+        :keyword method: Default value is None.
+        :paramtype method: str
+        :keyword methodName: Default value is None.
+        :paramtype methodName: str
         :keyword dataset: Default value is None.
         :paramtype dataset: str
-        :keyword dataset_name: Default value is None.
-        :paramtype dataset_name: str
         :keyword evaluation: Default value is None.
         :paramtype evaluation: str
-        :keyword inference_service: Default value is None.
-        :paramtype inference_service: str
-        :keyword inference_service_name: Default value is None.
-        :paramtype inference_service_name: str
-        :keyword method: Default value is None.
-        :paramtype method: str
-        :keyword method_name: Default value is None.
-        :paramtype method_name: str
+        :keyword inferenceService: Default value is None.
+        :paramtype inferenceService: str
         :keyword model: Default value is None.
         :paramtype model: str
-        :keyword model_name: Default value is None.
-        :paramtype model_name: str
+        :keyword inputsAnyOf: Default value is None.
+        :paramtype inputsAnyOf: str
         :return: Entities matching the query
         :rtype: list[SafetyCase]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return [
             SafetyCase.parse_obj(obj)
             for obj in self._raw_ops.query(
                 id=id,
                 account=account,
                 status=status,
                 reason=reason,
                 labels=_encode_labels(labels),
+                method=method,
+                method_name=methodName,
                 dataset=dataset,
-                dataset_name=dataset_name,
                 evaluation=evaluation,
-                inference_service=inference_service,
-                inference_service_name=inference_service_name,
-                method=method,
-                method_name=method_name,
+                inference_service=inferenceService,
                 model=model,
-                model_name=model_name,
+                inputs_any_of=(
+                    ",".join(inputsAnyOf) if inputsAnyOf is not None else None
+                ),
             )
         ]
 
     def label(self, safetycase_id: str, labels: dict[str, Optional[str]]) -> None:
         """Label the specified SafetyCase with key-value pairs (stored in the
         ``.labels`` field of the resource).
 
@@ -1955,14 +2061,40 @@
         :param analysis_request: The SafetyCase specification.
         :type analysis_request: AnalysisCreateRequest
         :return: A full SafetyCase entity with .id and other properties set.
         """
         safetycase = _retry_not_found(self._raw_ops.create)(analysis_request.dict())
         return SafetyCase.parse_obj(safetycase)
 
+    def downlinks(self, safetycase_id: str) -> list[ArtifactURL]:
+        """Get a list of signed GET URLs from which SafetyCase artifacts can be
+        downloaded.
+
+        :param safetycase_id: The ID of the SafetyCase.
+        :type safetycase_id: str
+        :return: List of signed GET URLs.
+        :rtype: list[ArtifactURL] :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return _downlinks(self._raw_ops, safetycase_id)
+
+    def download(self, safetycase_id: str, destination: Path | str) -> None:
+        """Download all of the files in a safety case to a local directory.
+
+        The destination directory must be an empty directory that exists.
+
+        :param safetycase_id: The ID of the SafetyCase.
+        :type safetycase_id: str
+        :param destination: The destination directory. Must exist and be empty.
+        :type destination: Path | str
+        :raises ~azure.core.exceptions.HttpResponseError: If
+            ``safetycases.downlinks(safetycase_id)`` raises
+        :raises ValueError: If arguments are invalid
+        """
+        return _download(self, safetycase_id, destination, insecure=self._insecure)
+
 
 class _APIKeyCredential(TokenCredential):
     def __init__(self, *, api_key: str):
         self.api_key = api_key
 
     def get_token(
         self,
@@ -2048,31 +2180,37 @@
         # >> print(self._pipeline._transport.connection_config.verify)
         # True
         self._raw._client._pipeline._transport.connection_config.verify = (  # type: ignore
             not insecure
         )
 
         self._datasets = DatasetsOperations(self._raw.datasets, insecure=insecure)
-        self._evaluations = EvaluationsOperations(self._raw.evaluations)
+        self._evaluations = EvaluationsOperations(
+            self._raw.evaluations, insecure=insecure
+        )
         self._inferenceservices = InferenceservicesOperations(
             self._raw.inferenceservices
         )
         self._inferencesessions = InferencesessionsOperations(
             self._raw.inferencesessions,
             insecure=insecure,
         )
-        self._measurements = MeasurementsOperations(self._raw.measurements)
+        self._measurements = MeasurementsOperations(
+            self._raw.measurements, insecure=insecure
+        )
         self._methods = MethodsOperations(self._raw.methods)
         self._models = ModelsOperations(self._raw.models)
         self._modules = ModulesOperations(
             self._raw.modules,
             insecure=insecure,
         )
-        self._reports = ReportsOperations(self._raw.reports)
-        self._safetycases = SafetycasesOperations(self._raw.safetycases)
+        self._reports = ReportsOperations(self._raw.reports, insecure=insecure)
+        self._safetycases = SafetycasesOperations(
+            self._raw.safetycases, insecure=insecure
+        )
 
     @property
     def raw(self) -> RawClient:
         """The "raw" API client, which can be used to send JSON requests directly."""
         return self._raw
 
     @property
```

### Comparing `dyff_client-0.4.2/dyff_client.egg-info/PKG-INFO` & `dyff_client-0.5.0/dyff_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.4.2
+Version: 0.5.0
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_client-0.4.2/dyff_client.egg-info/SOURCES.txt` & `dyff_client-0.5.0/dyff_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/makefile` & `dyff_client-0.5.0/makefile`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/pyproject.toml` & `dyff_client-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/scripts/inferenceservices/databricks--dolly-v2-3b--default.py` & `dyff_client-0.5.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/scripts/inferenceservices/tiiuae--falcon-7b--default.py` & `dyff_client-0.5.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/scripts/models/databricks--dolly-v2-3b.py` & `dyff_client-0.5.0/scripts/models/databricks--dolly-v2-3b.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/scripts/models/tiiuae--falcon-7b.py` & `dyff_client-0.5.0/scripts/models/tiiuae--falcon-7b.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.4.2/tests/test_import.py` & `dyff_client-0.5.0/tests/test_import.py`

 * *Files identical despite different names*

