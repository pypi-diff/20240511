# Comparing `tmp/qbraid_core-0.1.5.tar.gz` & `tmp/qbraid_core-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid_core-0.1.5.tar", last modified: Fri May 10 02:07:34 2024, max compression
+gzip compressed data, was "qbraid_core-0.1.5a0.tar", last modified: Wed Apr 24 19:20:21 2024, max compression
```

## Comparing `qbraid_core-0.1.5.tar` & `qbraid_core-0.1.5a0.tar`

### file list

```diff
@@ -1,122 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.655343 qbraid_core-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.635343 qbraid_core-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.635343 qbraid_core-0.1.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.639343 qbraid_core-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/.github/workflows/pre-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-10 02:07:34.655343 qbraid_core-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.639343 qbraid_core-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.639343 qbraid_core-0.1.5/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.639343 qbraid_core-0.1.5/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.639343 qbraid_core-0.1.5/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/_static/css/s4defs-roles.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.639343 qbraid_core-0.1.5/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/api/qbraid_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/api/qbraid_core.services.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/api/qbraid_core.system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.643343 qbraid_core-0.1.5/qbraid_core/
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-10 02:07:34.000000 qbraid_core-0.1.5/qbraid_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.643343 qbraid_core-0.1.5/qbraid_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.643343 qbraid_core-0.1.5/qbraid_core/services/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/admin/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.647343 qbraid_core-0.1.5/qbraid_core/services/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/environments/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/environments/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/environments/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/environments/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/environments/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/environments/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.647343 qbraid_core-0.1.5/qbraid_core/services/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/quantum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/quantum/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/quantum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/quantum/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/quantum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/quantum/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/quantum/proxy_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/services/quantum/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.647343 qbraid_core-0.1.5/qbraid_core/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/system/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/system/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.647343 qbraid_core-0.1.5/qbraid_core/system/magic/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/system/magic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/system/magic/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/system/magic/qbraid_magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/system/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/system/threader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/qbraid_core/system/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.651343 qbraid_core-0.1.5/qbraid_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-05-10 02:07:34.000000 qbraid_core-0.1.5/qbraid_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-10 02:07:34.000000 qbraid_core-0.1.5/qbraid_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 02:07:34.000000 qbraid_core-0.1.5/qbraid_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-10 02:07:34.000000 qbraid_core-0.1.5/qbraid_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 02:07:34.000000 qbraid_core-0.1.5/qbraid_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 02:07:34.655343 qbraid_core-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.647343 qbraid_core-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.651343 qbraid_core-0.1.5/tests/environments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/environments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.651343 qbraid_core-0.1.5/tests/environments/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/environments/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/environments/fixtures/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/environments/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/environments/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/environments/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/environments/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/environments/test_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.651343 qbraid_core-0.1.5/tests/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/quantum/test_aws_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/quantum/test_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.651343 qbraid_core-0.1.5/tests/system/
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/system/test_executables.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/system/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/system/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/system/test_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.651343 qbraid_core-0.1.5/tests/top_level/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/top_level/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/top_level/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/top_level/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/top_level/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tests/top_level/test_sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 02:07:34.651343 qbraid_core-0.1.5/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2584 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tools/create_dev_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2725 2024-05-10 02:07:25.000000 qbraid_core-0.1.5/tools/stamp_pre_release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.934040 qbraid_core-0.1.5a0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.914040 qbraid_core-0.1.5a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.914040 qbraid_core-0.1.5a0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.914040 qbraid_core-0.1.5a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/.github/workflows/pre-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-24 19:20:21.934040 qbraid_core-0.1.5a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.918040 qbraid_core-0.1.5a0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.918040 qbraid_core-0.1.5a0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.918040 qbraid_core-0.1.5a0/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.918040 qbraid_core-0.1.5a0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/_static/css/s4defs-roles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.918040 qbraid_core-0.1.5a0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/api/qbraid_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/api/qbraid_core.services.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/api/qbraid_core.system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.922040 qbraid_core-0.1.5a0/qbraid_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-24 19:20:21.000000 qbraid_core-0.1.5a0/qbraid_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.922040 qbraid_core-0.1.5a0/qbraid_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.922040 qbraid_core-0.1.5a0/qbraid_core/services/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/admin/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.926040 qbraid_core-0.1.5a0/qbraid_core/services/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/environments/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/environments/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/environments/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/environments/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/environments/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/environments/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.926040 qbraid_core-0.1.5a0/qbraid_core/services/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/quantum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/quantum/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/quantum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/quantum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/quantum/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/services/quantum/proxy_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.926040 qbraid_core-0.1.5a0/qbraid_core/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/system/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/system/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.926040 qbraid_core-0.1.5a0/qbraid_core/system/magic/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/system/magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/system/magic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/system/magic/qbraid_magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/system/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/system/threader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/qbraid_core/system/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.930040 qbraid_core-0.1.5a0/qbraid_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-24 19:20:21.000000 qbraid_core-0.1.5a0/qbraid_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-24 19:20:21.000000 qbraid_core-0.1.5a0/qbraid_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:20:21.000000 qbraid_core-0.1.5a0/qbraid_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-24 19:20:21.000000 qbraid_core-0.1.5a0/qbraid_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 19:20:21.000000 qbraid_core-0.1.5a0/qbraid_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:20:21.934040 qbraid_core-0.1.5a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.926040 qbraid_core-0.1.5a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.930040 qbraid_core-0.1.5a0/tests/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/environments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.930040 qbraid_core-0.1.5a0/tests/environments/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/environments/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/environments/fixtures/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/environments/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/environments/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/environments/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/environments/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/environments/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.930040 qbraid_core-0.1.5a0/tests/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/quantum/test_aws_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/quantum/test_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.930040 qbraid_core-0.1.5a0/tests/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/system/test_executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/system/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/system/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/system/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.930040 qbraid_core-0.1.5a0/tests/top_level/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/top_level/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/top_level/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/top_level/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/top_level/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tests/top_level/test_sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:20:21.930040 qbraid_core-0.1.5a0/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2584 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tools/create_dev_build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2725 2024-04-24 19:20:09.000000 qbraid_core-0.1.5a0/tools/stamp_pre_release.py
```

### Comparing `qbraid_core-0.1.5/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid_core-0.1.5a0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files 10% similar despite different names*

```diff
@@ -26,8 +26,16 @@
       required: true
 
   - type: textarea
     attributes:
       label: Suggestions (Optional)
       description: We warmly welcome any recommendations on potential fixes, insights, or considerations that contributors should keep in mind when working to resolve this issue.
     validations:
-      required: false
+      required: false
+
+  - type: checkboxes
+    id: agreement
+    attributes:
+      label: 'Please confirm the following:'
+      options:
+        - label: 'I have searched the existing issues and confirm this is a new bug report.'
+          required: true
```

### Comparing `qbraid_core-0.1.5/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid_core-0.1.5a0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files 24% similar despite different names*

```diff
@@ -18,8 +18,17 @@
       required: true
   
   - type: textarea
     attributes:
       label: Implementation (Optional)
       description: "Do you have an idea for how this could be implemented? Please include those details here."
     validations:
-      required: false
+      required: false
+
+  - type: checkboxes
+    id: agreement
+    attributes:
+      label: 'Please confirm the following:'
+      description: 'Understanding that feature requests are evaluated for their applicability and benefit to the community, and not all requests may be implemented.'
+      options:
+        - label: 'I have searched the existing issues and confirm this is a new feature request.'
+          required: true
```

### Comparing `qbraid_core-0.1.5/.github/workflows/docs.yml` & `qbraid_core-0.1.5a0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/.github/workflows/format.yml` & `qbraid_core-0.1.5a0/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/.github/workflows/main.yml` & `qbraid_core-0.1.5a0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/.github/workflows/pre-release.yml` & `qbraid_core-0.1.5a0/.github/workflows/pre-release.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/.github/workflows/publish.yml` & `qbraid_core-0.1.5a0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/.gitignore` & `qbraid_core-0.1.5a0/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/LICENSE` & `qbraid_core-0.1.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/PKG-INFO` & `qbraid_core-0.1.5a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.5
+Version: 0.1.5a0
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
-Author: qBraid Development Team
-Author-email: contact@qbraid.com
+Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
 Project-URL: Launch on Lab, https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid-Lab.git
 Keywords: qbraid,quantum,cloud
@@ -23,15 +22,14 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: urllib3
 Requires-Dist: ipython
-Requires-Dist: numpy
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx<7.4.0,>=7.2.6; extra == "docs"
@@ -66,17 +64,14 @@
 
 1. Create a qBraid account or log in to your existing account by visiting
    [account.qbraid.com](https://account.qbraid.com/)
 2. Copy your API Key token from the left side of
     your [account page](https://account.qbraid.com/):
 3. Save your API key from step 2 in local configuration file `~/.qbraid/qbraidrc`, where `~` corresponds to your home (`$HOME`) directory:
 
-| :warning: Account credentials are saved in plain text, so only do so if you are using a trusted device. |
-|:---------------------------|
-
 ```shell
 [default]
 api-key = YOUR_KEY
 url = https://api.qbraid.com/api
 ```
 
 Or generate your `~/.qbraid/qbraidrc` file via the qbraid-core Python interface:
```

### Comparing `qbraid_core-0.1.5/README.md` & `qbraid_core-0.1.5a0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,17 +25,14 @@
 
 1. Create a qBraid account or log in to your existing account by visiting
    [account.qbraid.com](https://account.qbraid.com/)
 2. Copy your API Key token from the left side of
     your [account page](https://account.qbraid.com/):
 3. Save your API key from step 2 in local configuration file `~/.qbraid/qbraidrc`, where `~` corresponds to your home (`$HOME`) directory:
 
-| :warning: Account credentials are saved in plain text, so only do so if you are using a trusted device. |
-|:---------------------------|
-
 ```shell
 [default]
 api-key = YOUR_KEY
 url = https://api.qbraid.com/api
 ```
 
 Or generate your `~/.qbraid/qbraidrc` file via the qbraid-core Python interface:
```

### Comparing `qbraid_core-0.1.5/docs/Makefile` & `qbraid_core-0.1.5a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/docs/_static/cards/jupyter.png` & `qbraid_core-0.1.5a0/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/docs/_static/cards/python.png` & `qbraid_core-0.1.5a0/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/docs/_static/cards/terminal.png` & `qbraid_core-0.1.5a0/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/docs/_static/css/custom.css` & `qbraid_core-0.1.5a0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/docs/_static/css/s4defs-roles.css` & `qbraid_core-0.1.5a0/docs/_static/css/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/docs/_static/favicon.ico` & `qbraid_core-0.1.5a0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/docs/_static/logo.png` & `qbraid_core-0.1.5a0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/docs/conf.py` & `qbraid_core-0.1.5a0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/docs/index.rst` & `qbraid_core-0.1.5a0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/docs/make.bat` & `qbraid_core-0.1.5a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/pyproject.toml` & `qbraid_core-0.1.5a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 [build-system]
 requires = ["setuptools >= 61.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-core"
-version = "0.1.5"
-authors = [{name = "qBraid Development Team"}, {email = "contact@qbraid.com"}]
+version = "0.1.5-alpha"
+authors = [
+    {name = "qBraid Development Team", email = "contact@qbraid.com"},
+]
 description = "Python library with core abstractions for software development in the qBraid ecosystem."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["qbraid", "quantum", "cloud"]
 license = {text = "Proprietary"}
 classifiers = [
     "Intended Audience :: Developers",
@@ -19,15 +21,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-dependencies = ["requests", "urllib3", "ipython", "numpy"]
+dependencies = ["requests", "urllib3", "ipython"]
 
 [project.urls]
 Homepage = "https://www.qbraid.com/"
 Documentation = "https://docs.qbraid.com/projects/core/en/latest/"
 "Bug Tracker" = "https://github.com/qBraid/qBraid-Lab/issues"
 Discord = "https://discord.gg/KugF6Cnncm"
 "Launch on Lab" = "https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid-Lab.git"
```

### Comparing `qbraid_core-0.1.5/qbraid_core/__init__.py` & `qbraid_core-0.1.5a0/qbraid_core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -122,23 +122,7 @@
     "QbraidException",
     "AuthError",
     "ConfigError",
     "RequestsApiError",
     "ResourceNotFoundError",
     "UserNotFoundError",
 ]
-
-_lazy_mods = ["services", "system"]
-
-
-def __getattr__(name):
-    if name in _lazy_mods:
-        import importlib  # pylint: disable=import-outside-toplevel
-
-        module = importlib.import_module(f".{name}", __name__)
-        globals()[name] = module
-        return module
-    raise AttributeError(f"module {__name__!r} has no attribute {name!r}")
-
-
-def __dir__():
-    return sorted(__all__ + _lazy_mods)
```

### Comparing `qbraid_core-0.1.5/qbraid_core/_compat.py` & `qbraid_core-0.1.5a0/qbraid_core/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/client.py` & `qbraid_core-0.1.5a0/qbraid_core/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/config.py` & `qbraid_core-0.1.5a0/qbraid_core/config.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/context.py` & `qbraid_core-0.1.5a0/qbraid_core/context.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/exceptions.py` & `qbraid_core-0.1.5a0/qbraid_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/registry.py` & `qbraid_core-0.1.5a0/qbraid_core/registry.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/retry.py` & `qbraid_core-0.1.5a0/qbraid_core/retry.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/services/admin/client.py` & `qbraid_core-0.1.5a0/qbraid_core/services/admin/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/services/environments/__init__.py` & `qbraid_core-0.1.5a0/qbraid_core/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/services/environments/client.py` & `qbraid_core-0.1.5a0/qbraid_core/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/services/environments/create.py` & `qbraid_core-0.1.5a0/qbraid_core/services/environments/create.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/services/environments/magic.py` & `qbraid_core-0.1.5a0/qbraid_core/services/environments/magic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/services/environments/paths.py` & `qbraid_core-0.1.5a0/qbraid_core/services/environments/paths.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/services/environments/state.py` & `qbraid_core-0.1.5a0/qbraid_core/services/environments/state.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/services/environments/validate.py` & `qbraid_core-0.1.5a0/qbraid_core/services/environments/validate.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/services/quantum/__init__.py` & `qbraid_core-0.1.5a0/qbraid_core/services/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/services/quantum/adapter.py` & `qbraid_core-0.1.5a0/qbraid_core/services/quantum/adapter.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/services/quantum/proxy.py` & `qbraid_core-0.1.5a0/qbraid_core/services/quantum/proxy.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/services/quantum/proxy_braket.py` & `qbraid_core-0.1.5a0/qbraid_core/services/quantum/proxy_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/sessions.py` & `qbraid_core-0.1.5a0/qbraid_core/sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/system/__init__.py` & `qbraid_core-0.1.5a0/qbraid_core/system/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/system/exceptions.py` & `qbraid_core-0.1.5a0/qbraid_core/system/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/system/executables.py` & `qbraid_core-0.1.5a0/qbraid_core/system/executables.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/system/generic.py` & `qbraid_core-0.1.5a0/qbraid_core/system/generic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/system/magic/manager.py` & `qbraid_core-0.1.5a0/qbraid_core/system/magic/manager.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/system/magic/qbraid_magic.py` & `qbraid_core-0.1.5a0/qbraid_core/system/magic/qbraid_magic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/system/packages.py` & `qbraid_core-0.1.5a0/qbraid_core/system/packages.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/system/threader.py` & `qbraid_core-0.1.5a0/qbraid_core/system/threader.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core/system/versions.py` & `qbraid_core-0.1.5a0/qbraid_core/system/versions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/qbraid_core.egg-info/PKG-INFO` & `qbraid_core-0.1.5a0/qbraid_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.5
+Version: 0.1.5a0
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
-Author: qBraid Development Team
-Author-email: contact@qbraid.com
+Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
 Project-URL: Launch on Lab, https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid-Lab.git
 Keywords: qbraid,quantum,cloud
@@ -23,15 +22,14 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: urllib3
 Requires-Dist: ipython
-Requires-Dist: numpy
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx<7.4.0,>=7.2.6; extra == "docs"
@@ -66,17 +64,14 @@
 
 1. Create a qBraid account or log in to your existing account by visiting
    [account.qbraid.com](https://account.qbraid.com/)
 2. Copy your API Key token from the left side of
     your [account page](https://account.qbraid.com/):
 3. Save your API key from step 2 in local configuration file `~/.qbraid/qbraidrc`, where `~` corresponds to your home (`$HOME`) directory:
 
-| :warning: Account credentials are saved in plain text, so only do so if you are using a trusted device. |
-|:---------------------------|
-
 ```shell
 [default]
 api-key = YOUR_KEY
 url = https://api.qbraid.com/api
 ```
 
 Or generate your `~/.qbraid/qbraidrc` file via the qbraid-core Python interface:
```

### Comparing `qbraid_core-0.1.5/qbraid_core.egg-info/SOURCES.txt` & `qbraid_core-0.1.5a0/qbraid_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 qbraid_core/__init__.py
 qbraid_core/_compat.py
 qbraid_core/_version.py
 qbraid_core/client.py
 qbraid_core/config.py
 qbraid_core/context.py
 qbraid_core/exceptions.py
-qbraid_core/py.typed
 qbraid_core/registry.py
 qbraid_core/retry.py
 qbraid_core/sessions.py
 qbraid_core.egg-info/PKG-INFO
 qbraid_core.egg-info/SOURCES.txt
 qbraid_core.egg-info/dependency_links.txt
 qbraid_core.egg-info/requires.txt
@@ -52,19 +51,17 @@
 qbraid_core/services/environments/magic.py
 qbraid_core/services/environments/paths.py
 qbraid_core/services/environments/state.py
 qbraid_core/services/environments/validate.py
 qbraid_core/services/quantum/__init__.py
 qbraid_core/services/quantum/adapter.py
 qbraid_core/services/quantum/client.py
-qbraid_core/services/quantum/compat.py
 qbraid_core/services/quantum/exceptions.py
 qbraid_core/services/quantum/proxy.py
 qbraid_core/services/quantum/proxy_braket.py
-qbraid_core/services/quantum/runner.py
 qbraid_core/system/__init__.py
 qbraid_core/system/exceptions.py
 qbraid_core/system/executables.py
 qbraid_core/system/generic.py
 qbraid_core/system/packages.py
 qbraid_core/system/threader.py
 qbraid_core/system/versions.py
```

### Comparing `qbraid_core-0.1.5/tests/environments/fixtures/environments.py` & `qbraid_core-0.1.5a0/tests/environments/fixtures/environments.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/environments/test_client.py` & `qbraid_core-0.1.5a0/tests/environments/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/environments/test_create.py` & `qbraid_core-0.1.5a0/tests/environments/test_create.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/environments/test_paths.py` & `qbraid_core-0.1.5a0/tests/environments/test_paths.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/environments/test_state.py` & `qbraid_core-0.1.5a0/tests/environments/test_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/environments/test_validate.py` & `qbraid_core-0.1.5a0/tests/environments/test_validate.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/quantum/test_aws_configure.py` & `qbraid_core-0.1.5a0/tests/quantum/test_aws_configure.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/quantum/test_proxy.py` & `qbraid_core-0.1.5a0/tests/quantum/test_proxy.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/system/test_executables.py` & `qbraid_core-0.1.5a0/tests/system/test_executables.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/system/test_generic.py` & `qbraid_core-0.1.5a0/tests/system/test_generic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/system/test_packages.py` & `qbraid_core-0.1.5a0/tests/system/test_packages.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/system/test_versions.py` & `qbraid_core-0.1.5a0/tests/system/test_versions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/top_level/test_client.py` & `qbraid_core-0.1.5a0/tests/top_level/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/top_level/test_compat.py` & `qbraid_core-0.1.5a0/tests/top_level/test_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/top_level/test_config.py` & `qbraid_core-0.1.5a0/tests/top_level/test_config.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/top_level/test_context.py` & `qbraid_core-0.1.5a0/tests/top_level/test_context.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tests/top_level/test_sessions.py` & `qbraid_core-0.1.5a0/tests/top_level/test_sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tools/create_dev_build.sh` & `qbraid_core-0.1.5a0/tools/create_dev_build.sh`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.5/tools/stamp_pre_release.py` & `qbraid_core-0.1.5a0/tools/stamp_pre_release.py`

 * *Files identical despite different names*

