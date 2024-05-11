# Comparing `tmp/silverback-0.4.2.tar.gz` & `tmp/silverback-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverback-0.4.2.tar", last modified: Tue May  7 20:03:19 2024, max compression
+gzip compressed data, was "silverback-0.5.0.tar", last modified: Sat May 11 01:18:26 2024, max compression
```

## Comparing `silverback-0.4.2.tar` & `silverback-0.5.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.032619 silverback-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-07 20:02:19.000000 silverback-0.4.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-07 20:02:19.000000 silverback-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-07 20:02:19.000000 silverback-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-07 20:02:19.000000 silverback-0.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-07 20:02:19.000000 silverback-0.4.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-07 20:02:19.000000 silverback-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-07 20:03:19.032619 silverback-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-07 20:02:19.000000 silverback-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-07 20:02:19.000000 silverback-0.4.2/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.024619 silverback-0.4.2/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/commands/run.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.028619 silverback-0.4.2/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/methoddocs/application.md
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/methoddocs/middlewares.md
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/methoddocs/runner.md
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/methoddocs/subscriptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.028619 silverback-0.4.2/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/userguides/development.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 20:02:19.000000 silverback-0.4.2/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-07 20:02:19.000000 silverback-0.4.2/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-07 20:02:19.000000 silverback-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-07 20:03:19.032619 silverback-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-07 20:02:19.000000 silverback-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.028619 silverback-0.4.2/silverback/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-07 20:02:19.000000 silverback-0.4.2/silverback/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.032619 silverback-0.4.2/silverback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 20:03:18.000000 silverback-0.4.2/silverback.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:03:19.032619 silverback-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:02:19.000000 silverback-0.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 20:02:19.000000 silverback-0.4.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-07 20:02:19.000000 silverback-0.4.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-07 20:02:19.000000 silverback-0.4.2/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.451690 silverback-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.443690 silverback-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.443690 silverback-0.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.443690 silverback-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-11 01:17:31.000000 silverback-0.5.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-11 01:17:31.000000 silverback-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-11 01:17:31.000000 silverback-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-11 01:17:31.000000 silverback-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-11 01:17:31.000000 silverback-0.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-11 01:17:31.000000 silverback-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-11 01:18:26.451690 silverback-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-11 01:17:31.000000 silverback-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-11 01:17:31.000000 silverback-0.5.0/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.447690 silverback-0.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.447690 silverback-0.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.447690 silverback-0.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.447690 silverback-0.5.0/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/commands/run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.447690 silverback-0.5.0/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/methoddocs/application.md
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/methoddocs/middlewares.md
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/methoddocs/runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/methoddocs/subscriptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.447690 silverback-0.5.0/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/userguides/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-11 01:17:31.000000 silverback-0.5.0/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-11 01:17:31.000000 silverback-0.5.0/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-11 01:17:31.000000 silverback-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-11 01:18:26.451690 silverback-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-11 01:17:31.000000 silverback-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.451690 silverback-0.5.0/silverback/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16078 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-11 01:17:31.000000 silverback-0.5.0/silverback/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.451690 silverback-0.5.0/silverback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 01:18:26.000000 silverback-0.5.0/silverback.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:18:26.451690 silverback-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 01:17:31.000000 silverback-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-11 01:17:31.000000 silverback-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-11 01:17:31.000000 silverback-0.5.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-11 01:17:31.000000 silverback-0.5.0/tests/test_types.py
```

### Comparing `silverback-0.4.2/.github/ISSUE_TEMPLATE/bug.md` & `silverback-0.5.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/.github/ISSUE_TEMPLATE/feature.md` & `silverback-0.5.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/.github/ISSUE_TEMPLATE/work-item.md` & `silverback-0.5.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/.github/release-drafter.yml` & `silverback-0.5.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/.github/workflows/codeql.yaml` & `silverback-0.5.0/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/.github/workflows/commitlint.yaml` & `silverback-0.5.0/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/.github/workflows/docs.yaml` & `silverback-0.5.0/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/.github/workflows/prtitle.yaml` & `silverback-0.5.0/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/.github/workflows/publish.yaml` & `silverback-0.5.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/.github/workflows/test.yaml` & `silverback-0.5.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/.gitignore` & `silverback-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/.pre-commit-config.yaml` & `silverback-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/CONTRIBUTING.md` & `silverback-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/Dockerfile` & `silverback-0.5.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/LICENSE` & `silverback-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/PKG-INFO` & `silverback-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.4.2
+Version: 0.5.0
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.4.2/README.md` & `silverback-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/build_docs.py` & `silverback-0.5.0/build_docs.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/docs/_static/custom.css` & `silverback-0.5.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/docs/_static/custom.js` & `silverback-0.5.0/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/docs/_templates/layout.html` & `silverback-0.5.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/docs/conf.py` & `silverback-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/docs/favicon.ico` & `silverback-0.5.0/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/docs/logo.gif` & `silverback-0.5.0/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/docs/userguides/development.md` & `silverback-0.5.0/docs/userguides/development.md`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/example.py` & `silverback-0.5.0/example.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/pyproject.toml` & `silverback-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/setup.py` & `silverback-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     url="https://github.com/ApeWorX/silverback",
     include_package_data=True,
     install_requires=[
         "click",  # Use same version as eth-ape
         "eth-ape>=0.7,<1.0",
         "ethpm-types>=0.6.10",  # lower pin only, `eth-ape` governs upper pin
         "eth-pydantic-types",  # Use same version as eth-ape
+        "packaging",  # Use same version as eth-ape
         "pydantic_settings",  # Use same version as eth-ape
         "taskiq[metrics]>=0.11.3,<0.12",
     ],
     entry_points={
         "console_scripts": ["silverback=silverback._cli:cli"],
     },
     python_requires=">=3.10,<4",
```

### Comparing `silverback-0.4.2/silverback/_cli.py` & `silverback-0.5.0/silverback/_cli.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/silverback/_importer.py` & `silverback-0.5.0/silverback/_importer.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/silverback/application.py` & `silverback-0.5.0/silverback/application.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 import atexit
-from collections import defaultdict
-from dataclasses import dataclass
 from datetime import timedelta
-from typing import Callable
+from typing import Any, Callable
 
 from ape.api.networks import LOCAL_NETWORK_NAME
 from ape.contracts import ContractEvent, ContractInstance
 from ape.logging import logger
 from ape.managers.chain import BlockContainer
 from ape.utils import ManagerAccessMixin
+from packaging.version import Version
+from pydantic import BaseModel
 from taskiq import AsyncTaskiqDecoratedTask, TaskiqEvents
 
 from .exceptions import ContainerTypeMismatchError, InvalidContainerTypeError
 from .settings import Settings
 from .types import SilverbackID, TaskType
 
 
-@dataclass
-class TaskData:
-    container: BlockContainer | ContractEvent | None
-    handler: AsyncTaskiqDecoratedTask
+class SystemConfig(BaseModel):
+    # NOTE: Do not change this datatype unless major breaking
+
+    # NOTE: Useful for determining if Runner can handle this app
+    sdk_version: str
+    # NOTE: Useful for specifying what task types can be specified by app
+    task_types: list[str]
+
+
+class TaskData(BaseModel):
+    # NOTE: Data we need to know how to call a task via kicker
+    name: str  # Name of user function
+    labels: dict[str, Any]
+
+    # NOTE: Any other items here must have a default value
 
 
 class SilverbackApp(ManagerAccessMixin):
     """
     The application singleton. Must be initialized prior to use.
 
     Usage example::
@@ -62,36 +73,73 @@
         ):
             settings.NEW_BLOCK_TIMEOUT = int(timedelta(days=1).total_seconds())
 
         settings_str = "\n  ".join(f'{key}="{val}"' for key, val in settings.dict().items() if val)
         logger.info(f"Loading Silverback App with settings:\n  {settings_str}")
 
         self.broker = settings.get_broker()
-        # NOTE: If no tasks registered yet, defaults to empty list instead of raising KeyError
-        self.tasks: defaultdict[TaskType, list[TaskData]] = defaultdict(list)
+        self.tasks: dict[TaskType, list[TaskData]] = {
+            task_type: []
+            for task_type in TaskType
+            # NOTE: Dont track system tasks
+            if not str(task_type).startswith("system:")
+        }
         self.poll_settings: dict[str, dict] = {}
 
         atexit.register(provider_context.__exit__, None, None, None)
 
         self.signer = settings.get_signer()
         self.new_block_timeout = settings.NEW_BLOCK_TIMEOUT
-        self.start_block = settings.START_BLOCK
 
         signer_str = f"\n  SIGNER={repr(self.signer)}"
-        start_block_str = f"\n  START_BLOCK={self.start_block}" if self.start_block else ""
         new_block_timeout_str = (
             f"\n  NEW_BLOCK_TIMEOUT={self.new_block_timeout}" if self.new_block_timeout else ""
         )
 
         network_choice = f"{self.identifier.ecosystem}:{self.identifier.network}"
         logger.success(
             f'Loaded Silverback App:\n  NETWORK="{network_choice}"'
-            f"{signer_str}{start_block_str}{new_block_timeout_str}"
+            f"{signer_str}{new_block_timeout_str}"
         )
 
+        # NOTE: Runner must call this to configure itself for all SDK hooks
+        self._get_system_config = self.__register_system_task(
+            TaskType.SYSTEM_CONFIG, self.__get_system_config_handler
+        )
+        # NOTE: Register other system tasks here
+        self._get_user_taskdata = self.__register_system_task(
+            TaskType.SYSTEM_USER_TASKDATA, self.__get_user_taskdata_handler
+        )
+
+    def __register_system_task(
+        self, task_type: TaskType, task_handler: Callable
+    ) -> AsyncTaskiqDecoratedTask:
+        assert str(task_type).startswith("system:"), "Can only add system tasks"
+        # NOTE: This has to be registered with the broker in the worker
+        return self.broker.register_task(
+            task_handler,
+            # NOTE: Name makes it impossible to conflict with user's handler fn names
+            task_name=str(task_type),
+            task_type=str(task_type),
+        )
+
+    def __get_system_config_handler(self) -> SystemConfig:
+        # NOTE: This is actually executed on the worker side
+        from silverback.version import __version__
+
+        return SystemConfig(
+            sdk_version=Version(__version__).base_version,
+            task_types=[str(t) for t in TaskType],
+        )
+
+    def __get_user_taskdata_handler(self, task_type: TaskType) -> list[TaskData]:
+        # NOTE: This is actually executed on the worker side
+        assert str(task_type).startswith("user:"), "Can only fetch user task data"
+        return self.tasks.get(task_type, [])
+
     def broker_task_decorator(
         self,
         task_type: TaskType,
         container: BlockContainer | ContractEvent | None = None,
     ) -> Callable[[Callable], AsyncTaskiqDecoratedTask]:
         """
         Dynamically create a new broker task that handles tasks of ``task_type``.
@@ -106,20 +154,20 @@
 
         Raises:
             :class:`~silverback.exceptions.ContainerTypeMismatchError`:
                 If there is a mismatch between `task_type` and the `container`
                 type it should handle.
         """
         if (
-            (task_type is TaskType.NEW_BLOCKS and not isinstance(container, BlockContainer))
+            (task_type is TaskType.NEW_BLOCK and not isinstance(container, BlockContainer))
             or (task_type is TaskType.EVENT_LOG and not isinstance(container, ContractEvent))
             or (
                 task_type
                 not in (
-                    TaskType.NEW_BLOCKS,
+                    TaskType.NEW_BLOCK,
                     TaskType.EVENT_LOG,
                 )
                 and container is not None
             )
         ):
             raise ContainerTypeMismatchError(task_type, container)
 
@@ -128,27 +176,30 @@
             labels = {"task_type": str(task_type)}
 
             # NOTE: Do *not* do `if container` because that does a `len(container)` call,
             #       which for ContractEvent queries *every single log* ever emitted, and really
             #       we only want to determine if it is not None
             if container is not None and isinstance(container, ContractEvent):
                 # Address is almost a certainty if the container is being used as a filter here.
-                if contract_address := getattr(container.contract, "address", None):
-                    labels["contract_address"] = contract_address
-                labels["event_signature"] = f"{container.abi.signature}"
+                if not (contract_address := getattr(container.contract, "address", None)):
+                    raise InvalidContainerTypeError(
+                        "Please provider a contract event from a valid contract instance."
+                    )
 
-            broker_task = self.broker.register_task(
+                labels["contract_address"] = contract_address
+                labels["event_signature"] = container.abi.signature
+
+            self.tasks[task_type].append(TaskData(name=handler.__name__, labels=labels))
+
+            return self.broker.register_task(
                 handler,
                 task_name=handler.__name__,
                 **labels,
             )
 
-            self.tasks[task_type].append(TaskData(container=container, handler=broker_task))
-            return broker_task
-
         return add_taskiq_task
 
     def on_startup(self) -> Callable:
         """
         Code to execute on one worker upon startup / restart after an error.
 
         Usage example::
@@ -224,15 +275,15 @@
 
             if start_block is not None:
                 if "_blocks_" in self.poll_settings:
                     self.poll_settings["_blocks_"]["start_block"] = start_block
                 else:
                     self.poll_settings["_blocks_"] = {"start_block": start_block}
 
-            return self.broker_task_decorator(TaskType.NEW_BLOCKS, container=container)
+            return self.broker_task_decorator(TaskType.NEW_BLOCK, container=container)
 
         elif isinstance(container, ContractEvent) and isinstance(
             container.contract, ContractInstance
         ):
             key = container.contract.address
 
             if new_block_timeout is not None:
```

### Comparing `silverback-0.4.2/silverback/exceptions.py` & `silverback-0.5.0/silverback/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Sequence
+from typing import Any
 
 from ape.exceptions import ApeException
 
 from .types import TaskType
 
 
 class ImportFromStringError(Exception):
@@ -28,16 +28,18 @@
 
 class SilverbackException(ApeException):
     """Base Exception for any Silverback runtime faults."""
 
 
 # TODO: `ExceptionGroup` added in Python 3.11
 class StartupFailure(SilverbackException):
-    def __init__(self, *exceptions: Sequence[Exception]):
-        if error_str := "\n".join(str(e) for e in exceptions):
+    def __init__(self, *exceptions: Exception | str):
+        if len(exceptions) == 1 and isinstance(exceptions[0], str):
+            super().__init__(exceptions[0])
+        elif error_str := "\n".join(str(e) for e in exceptions):
             super().__init__(f"Startup failure(s):\n{error_str}")
         else:
             super().__init__("Startup failure(s) detected. See logs for details.")
 
 
 class NoTasksAvailableError(SilverbackException):
     def __init__(self):
```

### Comparing `silverback-0.4.2/silverback/middlewares.py` & `silverback-0.5.0/silverback/middlewares.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
         try:
             task_type = TaskType(task_type_str)
         except ValueError:
             return message  # Not a silverback task
 
         # Add extra labels for our task to see what their source was
-        if task_type is TaskType.NEW_BLOCKS:
+        if task_type is TaskType.NEW_BLOCK:
             # NOTE: Necessary because we don't know the exact block class
             block = message.args[0] = self.provider.network.ecosystem.decode_block(
                 hexbytes_dict(message.args[0])
             )
             message.labels["block_number"] = str(block.number)
             message.labels["block_hash"] = block.hash.hex()
 
@@ -92,12 +92,16 @@
         if self.block_time:
             percentage_time = 100 * (result.execution_time / self.block_time)
             percent_display = f" ({percentage_time:.1f}%)"
 
         else:
             percent_display = ""
 
-        (logger.error if result.error else logger.success)(
-            f"{self._create_label(message)} " f"- {result.execution_time:.3f}s{percent_display}"
-        )
+        msg = f"{self._create_label(message)} " f"- {result.execution_time:.3f}s{percent_display}"
+        if result.is_err:
+            logger.error(msg)
+        elif message.task_name.startswith("system:"):
+            logger.debug(msg)
+        else:
+            logger.success(msg)
 
     # NOTE: Unless stdout is ignored, error traceback appears in stdout, no need for `on_error`
```

### Comparing `silverback-0.4.2/silverback/recorder.py` & `silverback-0.5.0/silverback/recorder.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/silverback/runner.py` & `silverback-0.5.0/silverback/runner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 import asyncio
 from abc import ABC, abstractmethod
 
 from ape import chain
-from ape.contracts import ContractEvent, ContractInstance
 from ape.logging import logger
 from ape.utils import ManagerAccessMixin
 from ape_ethereum.ecosystem import keccak
-from taskiq import AsyncTaskiqDecoratedTask, AsyncTaskiqTask
+from ethpm_types import EventABI
+from packaging.specifiers import SpecifierSet
+from packaging.version import Version
+from taskiq import AsyncTaskiqTask
+from taskiq.kicker import AsyncKicker
 
-from .application import SilverbackApp
+from .application import SilverbackApp, SystemConfig, TaskData
 from .exceptions import Halt, NoTasksAvailableError, NoWebsocketAvailableError, StartupFailure
 from .recorder import BaseRecorder, TaskResult
 from .state import AppDatastore, AppState
 from .subscriptions import SubscriptionType, Web3SubscriptionsManager
 from .types import TaskType
-from .utils import async_wrap_iter, hexbytes_dict
+from .utils import (
+    async_wrap_iter,
+    hexbytes_dict,
+    run_taskiq_task_group_wait_results,
+    run_taskiq_task_wait_result,
+)
 
 
 class BaseRunner(ABC):
     def __init__(
         self,
+        # TODO: Make fully stateless by replacing `app` with `broker` and `identifier`
         app: SilverbackApp,
         *args,
         max_exceptions: int = 3,
         recorder: BaseRecorder | None = None,
         **kwargs,
     ):
         self.app = app
@@ -32,14 +41,23 @@
         self.datastore = AppDatastore()
 
         self.max_exceptions = max_exceptions
         self.exceptions = 0
 
         logger.info(f"Using {self.__class__.__name__}: max_exceptions={self.max_exceptions}")
 
+    def _create_task_kicker(self, task_data: TaskData) -> AsyncKicker:
+        return AsyncKicker(
+            task_name=task_data.name, broker=self.app.broker, labels=task_data.labels
+        )
+
+    def _create_system_task_kicker(self, task_type: TaskType) -> AsyncKicker:
+        assert "system:" in str(task_type)
+        return self._create_task_kicker(TaskData(name=str(task_type), labels={}))
+
     async def _handle_task(self, task: AsyncTaskiqTask):
         result = await task.wait_result()
 
         if self.recorder:
             await self.recorder.add_result(TaskResult.from_taskiq(result))
 
         if not result.is_err:
@@ -76,23 +94,21 @@
             try:
                 await self.datastore.set_state(self.state)
 
             except Exception as err:
                 logger.error(f"Error setting state: {err}")
 
     @abstractmethod
-    async def _block_task(self, block_handler: AsyncTaskiqDecoratedTask):
+    async def _block_task(self, task_data: TaskData):
         """
         Handle a block_handler task
         """
 
     @abstractmethod
-    async def _event_task(
-        self, contract_event: ContractEvent, event_handler: AsyncTaskiqDecoratedTask
-    ):
+    async def _event_task(self, task_data: TaskData):
         """
         handle an event handler task for the given contract event
         """
 
     async def run(self):
         """
         Run the task broker client for the assembled ``SilverbackApp`` application.
@@ -102,60 +118,117 @@
 
         Raises:
             :class:`~silverback.exceptions.StartupFailure`:
                 If there was an exception during startup.
             :class:`~silverback.exceptions.NoTasksAvailableError`:
                 If there are no configured tasks to execute.
         """
+        # Initialize broker (run worker startup events)
+        await self.app.broker.startup()
+
+        # Obtain system configuration for worker
+        result = await run_taskiq_task_wait_result(
+            self._create_system_task_kicker(TaskType.SYSTEM_CONFIG)
+        )
+        if result.is_err or not isinstance(result.return_value, SystemConfig):
+            raise StartupFailure("Unable to determine system configuration of worker")
+
+        # NOTE: Increase the specifier set here if there is a breaking change to this
+        if Version(result.return_value.sdk_version) not in SpecifierSet(">=0.5.0"):
+            # TODO: set to next breaking change release before release
+            raise StartupFailure("Worker SDK version too old, please rebuild")
+
+        if not (
+            system_tasks := set(TaskType(task_name) for task_name in result.return_value.task_types)
+        ):
+            raise StartupFailure("No system tasks detected, startup failure")
+        # NOTE: Guaranteed to be at least one because of `TaskType.SYSTEM_CONFIG`
+        system_tasks_str = "\n- ".join(system_tasks)
+        logger.info(
+            f"Worker using Silverback SDK v{result.return_value.sdk_version}"
+            f", available task types:\n- {system_tasks_str}"
+        )
+
+        # NOTE: Do this for other system tasks because they may not be in older SDK versions
+        #       `if TaskType.<SYSTEM_TASK_NAME> not in system_tasks: raise StartupFailure(...)`
+        #       or handle accordingly by having default logic if it is not available
+
         # Initialize recorder (if available) and fetch state if app has been run previously
         if self.recorder:
             await self.recorder.init(app_id=self.app.identifier)
 
         if startup_state := (await self.datastore.init(app_id=self.app.identifier)):
             self.state = startup_state
 
         else:  # use empty state
             self.state = AppState(last_block_seen=-1, last_block_processed=-1)
 
-        # Initialize broker (run worker startup events)
-        await self.app.broker.startup()
-
         # Execute Silverback startup task before we init the rest
-        if startup_tasks := await asyncio.gather(
-            *(task_def.handler.kiq(self.state) for task_def in self.app.tasks[TaskType.STARTUP])
-        ):
-            results = await asyncio.gather(
-                *(startup_task.wait_result() for startup_task in startup_tasks)
+        startup_taskdata_result = await run_taskiq_task_wait_result(
+            self._create_system_task_kicker(TaskType.SYSTEM_USER_TASKDATA), TaskType.STARTUP
+        )
+
+        if startup_taskdata_result.is_err:
+            raise StartupFailure(startup_taskdata_result.error)
+
+        else:
+            startup_task_handlers = map(
+                self._create_task_kicker, startup_taskdata_result.return_value
+            )
+
+            startup_task_results = await run_taskiq_task_group_wait_results(
+                (task_handler for task_handler in startup_task_handlers), self.state
             )
 
-            if any(result.is_err for result in results):
+            if any(result.is_err for result in startup_task_results):
                 # NOTE: Abort before even starting to run
-                raise StartupFailure(*(result.error for result in results if result.is_err))
+                raise StartupFailure(
+                    *(result.error for result in startup_task_results if result.is_err)
+                )
 
             elif self.recorder:
-                converted_results = map(TaskResult.from_taskiq, results)
+                converted_results = map(TaskResult.from_taskiq, startup_task_results)
                 await asyncio.gather(*(self.recorder.add_result(r) for r in converted_results))
 
             # NOTE: No need to handle results otherwise
 
         # Create our long-running event listeners
+        new_block_taskdata_results = await run_taskiq_task_wait_result(
+            self._create_system_task_kicker(TaskType.SYSTEM_USER_TASKDATA), TaskType.NEW_BLOCK
+        )
+        if new_block_taskdata_results.is_err:
+            raise StartupFailure(new_block_taskdata_results.error)
+
+        event_log_taskdata_results = await run_taskiq_task_wait_result(
+            self._create_system_task_kicker(TaskType.SYSTEM_USER_TASKDATA), TaskType.EVENT_LOG
+        )
+        if event_log_taskdata_results.is_err:
+            raise StartupFailure(event_log_taskdata_results.error)
+
+        if (
+            len(new_block_taskdata_results.return_value)
+            == len(event_log_taskdata_results.return_value)
+            == 0  # Both are empty
+        ):
+            raise NoTasksAvailableError()
+
         # NOTE: Any propagated failure in here should be handled such that shutdown tasks also run
         # TODO: `asyncio.TaskGroup` added in Python 3.11
         listener_tasks = (
             *(
-                asyncio.create_task(self._block_task(task_def.handler))
-                for task_def in self.app.tasks[TaskType.NEW_BLOCKS]
+                asyncio.create_task(self._block_task(task_def))
+                for task_def in new_block_taskdata_results.return_value
             ),
             *(
-                asyncio.create_task(self._event_task(task_def.container, task_def.handler))
-                for task_def in self.app.tasks[TaskType.EVENT_LOG]
+                asyncio.create_task(self._event_task(task_def))
+                for task_def in event_log_taskdata_results.return_value
             ),
         )
 
-        # NOTE: Safe to do this because no tasks have been scheduled to run yet
+        # NOTE: Safe to do this because no tasks were actually scheduled to run
         if len(listener_tasks) == 0:
             raise NoTasksAvailableError()
 
         # Run until one task bubbles up an exception that should stop execution
         tasks_with_errors, tasks_running = await asyncio.wait(
             listener_tasks, return_when=asyncio.FIRST_EXCEPTION
         )
@@ -164,24 +237,38 @@
             logger.debug(f"Runtime error(s) detected, shutting down:\n{runtime_errors}")
 
         # Cancel any still running
         (task.cancel() for task in tasks_running)
         # NOTE: All listener tasks are shut down now
 
         # Execute Silverback shutdown task(s) before shutting down the broker and app
-        if shutdown_tasks := await asyncio.gather(
-            *(task_def.handler.kiq() for task_def in self.app.tasks[TaskType.SHUTDOWN])
-        ):
-            asyncio.gather(*(shutdown_task.is_ready() for shutdown_task in shutdown_tasks))
-            if any(result.is_err for result in results):
-                errors_str = "\n".join(str(result.error) for result in results if result.is_err)
+        shutdown_taskdata_result = await run_taskiq_task_wait_result(
+            self._create_system_task_kicker(TaskType.SYSTEM_USER_TASKDATA), TaskType.SHUTDOWN
+        )
+
+        if shutdown_taskdata_result.is_err:
+            raise StartupFailure(shutdown_taskdata_result.error)
+
+        else:
+            shutdown_task_handlers = map(
+                self._create_task_kicker, shutdown_taskdata_result.return_value
+            )
+
+            shutdown_task_results = await run_taskiq_task_group_wait_results(
+                (task_handler for task_handler in shutdown_task_handlers)
+            )
+
+            if any(result.is_err for result in shutdown_task_results):
+                errors_str = "\n".join(
+                    str(result.error) for result in shutdown_task_results if result.is_err
+                )
                 logger.error(f"Errors while shutting down:\n{errors_str}")
 
             elif self.recorder:
-                converted_results = map(TaskResult.from_taskiq, results)
+                converted_results = map(TaskResult.from_taskiq, shutdown_task_results)
                 await asyncio.gather(*(self.recorder.add_result(r) for r in converted_results))
 
             # NOTE: No need to handle results otherwise
 
         await self.app.broker.shutdown()
 
 
@@ -190,111 +277,122 @@
     Run a single app against a live network using a basic in-memory queue and websockets.
     """
 
     def __init__(self, app: SilverbackApp, *args, **kwargs):
         super().__init__(app, *args, **kwargs)
 
         # Check for websocket support
-        if not (ws_uri := app.chain_manager.provider.ws_uri):
+        if not (ws_uri := self.chain_manager.provider.ws_uri):
             raise NoWebsocketAvailableError()
 
         self.ws_uri = ws_uri
 
-    async def _block_task(self, block_handler: AsyncTaskiqDecoratedTask):
+    async def _block_task(self, task_data: TaskData):
+        new_block_task_kicker = self._create_task_kicker(task_data)
         sub_id = await self.subscriptions.subscribe(SubscriptionType.BLOCKS)
         logger.debug(f"Handling blocks via {sub_id}")
 
         async for raw_block in self.subscriptions.get_subscription_data(sub_id):
             block = self.provider.network.ecosystem.decode_block(hexbytes_dict(raw_block))
 
             await self._checkpoint(last_block_seen=block.number)
-            await self._handle_task(await block_handler.kiq(raw_block))
+            await self._handle_task(await new_block_task_kicker.kiq(raw_block))
             await self._checkpoint(last_block_processed=block.number)
 
-    async def _event_task(
-        self, contract_event: ContractEvent, event_handler: AsyncTaskiqDecoratedTask
-    ):
-        if not isinstance(contract_event.contract, ContractInstance):
-            # For type-checking.
-            raise ValueError("Contract instance required.")
+    async def _event_task(self, task_data: TaskData):
+        if not (contract_address := task_data.labels.get("contract_address")):
+            raise StartupFailure("Contract instance required.")
+
+        if not (event_signature := task_data.labels.get("event_signature")):
+            raise StartupFailure("No Event Signature provided.")
+
+        event_abi = EventABI.from_signature(event_signature)
+
+        event_log_task_kicker = self._create_task_kicker(task_data)
 
         sub_id = await self.subscriptions.subscribe(
             SubscriptionType.EVENTS,
-            address=contract_event.contract.address,
-            topics=["0x" + keccak(text=contract_event.abi.selector).hex()],
-        )
-        logger.debug(
-            f"Handling '{contract_event.contract.address}:{contract_event.name}' logs via {sub_id}"
+            address=contract_address,
+            topics=["0x" + keccak(text=event_abi.selector).hex()],
         )
+        logger.debug(f"Handling '{contract_address}:{event_abi.name}' logs via {sub_id}")
 
         async for raw_event in self.subscriptions.get_subscription_data(sub_id):
             event = next(  # NOTE: `next` is okay since it only has one item
-                self.provider.network.ecosystem.decode_logs(
-                    [raw_event],
-                    contract_event.abi,
-                )
+                self.provider.network.ecosystem.decode_logs([raw_event], event_abi)
             )
 
             await self._checkpoint(last_block_seen=event.block_number)
-            await self._handle_task(await event_handler.kiq(event))
+            await self._handle_task(await event_log_task_kicker.kiq(event))
             await self._checkpoint(last_block_processed=event.block_number)
 
     async def run(self):
         async with Web3SubscriptionsManager(self.ws_uri) as subscriptions:
             self.subscriptions = subscriptions
             await super().run()
 
 
-class PollingRunner(BaseRunner):
+class PollingRunner(BaseRunner, ManagerAccessMixin):
     """
     Run a single app against a live network using a basic in-memory queue.
     """
 
+    # TODO: Move block_timeout settings to Ape core config
+    # TODO: Merge polling/websocket subscriptions downstream in Ape core
+
     def __init__(self, app: SilverbackApp, *args, **kwargs):
         super().__init__(app, *args, **kwargs)
         logger.warning(
             "The polling runner makes a significant amount of requests. "
             "Do not use in production over long time periods unless you know what you're doing."
         )
 
-    async def _block_task(self, block_handler: AsyncTaskiqDecoratedTask):
-        new_block_timeout = None
-        start_block = None
-        if "_blocks_" in self.app.poll_settings:
-            block_settings = self.app.poll_settings["_blocks_"]
+    async def _block_task(self, task_data: TaskData):
+        new_block_task_kicker = self._create_task_kicker(task_data)
+
+        if block_settings := self.app.poll_settings.get("_blocks_"):
             new_block_timeout = block_settings.get("new_block_timeout")
-            start_block = block_settings.get("start_block")
+        else:
+            new_block_timeout = None
 
         new_block_timeout = (
             new_block_timeout if new_block_timeout is not None else self.app.new_block_timeout
         )
-        start_block = start_block if start_block is not None else self.app.start_block
         async for block in async_wrap_iter(
-            chain.blocks.poll_blocks(start_block=start_block, new_block_timeout=new_block_timeout)
+            chain.blocks.poll_blocks(
+                # NOTE: No start block because we should begin polling from head
+                new_block_timeout=new_block_timeout,
+            )
         ):
             await self._checkpoint(last_block_seen=block.number)
-            await self._handle_task(await block_handler.kiq(block))
+            await self._handle_task(await new_block_task_kicker.kiq(block))
             await self._checkpoint(last_block_processed=block.number)
 
-    async def _event_task(
-        self, contract_event: ContractEvent, event_handler: AsyncTaskiqDecoratedTask
-    ):
-        new_block_timeout = None
-        start_block = None
-        address = None
-        if isinstance(contract_event.contract, ContractInstance):
-            address = contract_event.contract.address
-            if address in self.app.poll_settings:
-                address_settings = self.app.poll_settings[address]
-                new_block_timeout = address_settings.get("new_block_timeout")
-                start_block = address_settings.get("start_block")
+    async def _event_task(self, task_data: TaskData):
+        if not (contract_address := task_data.labels.get("contract_address")):
+            raise StartupFailure("Contract instance required.")
+
+        if not (event_signature := task_data.labels.get("event_signature")):
+            raise StartupFailure("No Event Signature provided.")
+
+        event_abi = EventABI.from_signature(event_signature)
+
+        event_log_task_kicker = self._create_task_kicker(task_data)
+        if address_settings := self.app.poll_settings.get(contract_address):
+            new_block_timeout = address_settings.get("new_block_timeout")
+        else:
+            new_block_timeout = None
 
         new_block_timeout = (
             new_block_timeout if new_block_timeout is not None else self.app.new_block_timeout
         )
-        start_block = start_block if start_block is not None else self.app.start_block
         async for event in async_wrap_iter(
-            contract_event.poll_logs(start_block=start_block, new_block_timeout=new_block_timeout)
+            self.provider.poll_logs(
+                # NOTE: No start block because we should begin polling from head
+                address=contract_address,
+                new_block_timeout=new_block_timeout,
+                events=[event_abi],
+            )
         ):
             await self._checkpoint(last_block_seen=event.block_number)
-            await self._handle_task(await event_handler.kiq(event))
+            await self._handle_task(await event_log_task_kicker.kiq(event))
             await self._checkpoint(last_block_processed=event.block_number)
```

### Comparing `silverback-0.4.2/silverback/settings.py` & `silverback-0.5.0/silverback/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     RESULT_BACKEND_CLASS: str = ""
     RESULT_BACKEND_URI: str = ""
 
     NETWORK_CHOICE: str = ""
     SIGNER_ALIAS: str = ""
 
     NEW_BLOCK_TIMEOUT: int | None = None
-    START_BLOCK: int | None = None
 
     # Used for recorder
     RECORDER_CLASS: str | None = None
 
     model_config = SettingsConfigDict(env_prefix="SILVERBACK_", case_sensitive=True)
 
     def get_middlewares(self) -> list[TaskiqMiddleware]:
```

### Comparing `silverback-0.4.2/silverback/state.py` & `silverback-0.5.0/silverback/state.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/silverback/subscriptions.py` & `silverback-0.5.0/silverback/subscriptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/silverback/types.py` & `silverback-0.5.0/silverback/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,23 @@
 from pydantic.functional_serializers import PlainSerializer
 from typing_extensions import Annotated
 
 logger = get_logger(__name__)
 
 
 class TaskType(str, Enum):
-    STARTUP = "startup"
-    NEW_BLOCKS = "block"
-    EVENT_LOG = "event"
-    SHUTDOWN = "shutdown"
+    # System-only Tasks
+    SYSTEM_CONFIG = "system:config"
+    SYSTEM_USER_TASKDATA = "system:user-taskdata"
+
+    # User-accessible Tasks
+    STARTUP = "user:startup"
+    NEW_BLOCK = "user:new-block"
+    EVENT_LOG = "user:event-log"
+    SHUTDOWN = "user:shutdown"
 
     def __str__(self) -> str:
         return self.value
 
 
 class SilverbackID(BaseModel):
     name: str
```

### Comparing `silverback-0.4.2/silverback/utils.py` & `silverback-0.5.0/silverback/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,28 @@
 import asyncio
 import threading
-from typing import AsyncIterator, Iterator
+from typing import AsyncIterator, Iterable, Iterator
 
 from ape.types import HexBytes
+from taskiq import AsyncTaskiqDecoratedTask, TaskiqResult
+from taskiq.kicker import AsyncKicker
+
+
+async def run_taskiq_task_wait_result(
+    task_def: AsyncTaskiqDecoratedTask | AsyncKicker, *args, **kwargs
+) -> TaskiqResult:
+    task = await task_def.kiq(*args, **kwargs)
+    return await task.wait_result()
+
+
+async def run_taskiq_task_group_wait_results(
+    task_defs: Iterable[AsyncTaskiqDecoratedTask | AsyncKicker], *args, **kwargs
+) -> list[TaskiqResult]:
+    tasks = await asyncio.gather(*(task_def.kiq(*args, **kwargs) for task_def in task_defs))
+    return await asyncio.gather(*(task.wait_result() for task in tasks))
 
 
 def async_wrap_iter(it: Iterator) -> AsyncIterator:
     """Wrap blocking iterator into an asynchronous one"""
     loop = asyncio.get_event_loop()
     q: asyncio.Queue = asyncio.Queue(1)
     exception = None
```

### Comparing `silverback-0.4.2/silverback.egg-info/PKG-INFO` & `silverback-0.5.0/silverback.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.4.2
+Version: 0.5.0
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.4.2/silverback.egg-info/SOURCES.txt` & `silverback-0.5.0/silverback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `silverback-0.4.2/silverback.egg-info/requires.txt` & `silverback-0.5.0/silverback.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 click
 eth-ape<1.0,>=0.7
 ethpm-types>=0.6.10
 eth-pydantic-types
+packaging
 pydantic_settings
 taskiq[metrics]<0.12,>=0.11.3
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
```

### Comparing `silverback-0.4.2/tests/test_types.py` & `silverback-0.5.0/tests/test_types.py`

 * *Files identical despite different names*

