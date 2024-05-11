# Comparing `tmp/osw-0.8.1.tar.gz` & `tmp/osw-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osw-0.8.1.tar", last modified: Fri Jun  9 16:39:45 2023, max compression
+gzip compressed data, was "osw-0.9.0.tar", last modified: Tue Jun 13 05:48:03 2023, max compression
```

## Comparing `osw-0.8.1.tar` & `osw-0.9.0.tar`

### file list

```diff
@@ -1,109 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.249094 osw-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-09 16:39:08.000000 osw-0.8.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.225094 osw-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.229094 osw-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-09 16:39:08.000000 osw-0.8.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-09 16:39:08.000000 osw-0.8.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-09 16:39:08.000000 osw-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-09 16:39:08.000000 osw-0.8.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 16:39:08.000000 osw-0.8.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-09 16:39:08.000000 osw-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-09 16:39:08.000000 osw-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-09 16:39:08.000000 osw-0.8.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-09 16:39:08.000000 osw-0.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-09 16:39:08.000000 osw-0.8.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-06-09 16:39:08.000000 osw-0.8.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-06-09 16:39:08.000000 osw-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-09 16:39:45.249094 osw-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-09 16:39:08.000000 osw-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 16:39:08.000000 osw-0.8.1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.233094 osw-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-09 16:39:08.000000 osw-0.8.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.233094 osw-0.8.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 16:39:08.000000 osw-0.8.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-09 16:39:08.000000 osw-0.8.1/docs/auth.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 16:39:08.000000 osw-0.8.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 16:39:08.000000 osw-0.8.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-06-09 16:39:08.000000 osw-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-09 16:39:08.000000 osw-0.8.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-09 16:39:08.000000 osw-0.8.1/docs/controller.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-09 16:39:08.000000 osw-0.8.1/docs/dev.md
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-09 16:39:08.000000 osw-0.8.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 16:39:08.000000 osw-0.8.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-09 16:39:08.000000 osw-0.8.1/docs/model.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 16:39:08.000000 osw-0.8.1/docs/osw.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 16:39:08.000000 osw-0.8.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-09 16:39:08.000000 osw-0.8.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 16:39:08.000000 osw-0.8.1/docs/tools.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.237094 osw-0.8.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-09 16:39:08.000000 osw-0.8.1/examples/accounts.pwd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-09 16:39:08.000000 osw-0.8.1/examples/controller_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-09 16:39:08.000000 osw-0.8.1/examples/create_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-09 16:39:08.000000 osw-0.8.1/examples/create_page_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.237094 osw-0.8.1/examples/data_processing/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-09 16:39:08.000000 osw-0.8.1/examples/data_processing/local_jsonpath_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-09 16:39:08.000000 osw-0.8.1/examples/database_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-09 16:39:08.000000 osw-0.8.1/examples/entity_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-09 16:39:08.000000 osw-0.8.1/examples/load_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-06-09 16:39:08.000000 osw-0.8.1/examples/local_editing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-06-09 16:39:08.000000 osw-0.8.1/examples/ontology_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-06-09 16:39:08.000000 osw-0.8.1/examples/page_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-09 16:39:08.000000 osw-0.8.1/examples/register_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-09 16:39:08.000000 osw-0.8.1/examples/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-09 16:39:08.000000 osw-0.8.1/examples/store_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-09 16:39:08.000000 osw-0.8.1/examples/update_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-09 16:39:08.000000 osw-0.8.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.225094 osw-0.8.1/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.237094 osw-0.8.1/nb/quantities/
--rw-r--r--   0 runner    (1001) docker     (123)   123529 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/Quantities.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.237094 osw-0.8.1/nb/quantities/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   107607 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/broader.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59112 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/buildDictionaryTest.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   152865 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/httpRequest.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/idea.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/querys.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-06-09 16:39:08.000000 osw-0.8.1/nb/quantities/archive/searchRunaways.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.241094 osw-0.8.1/nb/translations/
--rw-r--r--   0 runner    (1001) docker     (123)   404547 2023-06-09 16:39:08.000000 osw-0.8.1/nb/translations/DeeplTranslate.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-09 16:39:08.000000 osw-0.8.1/nb/translations/JsObjectToJson.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-09 16:39:08.000000 osw-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-09 16:39:45.253094 osw-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-09 16:39:08.000000 osw-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.225094 osw-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.241094 osw-0.8.1/src/osw/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.245094 osw-0.8.1/src/osw/controller/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/controller/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/controller/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/controller/page_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    22113 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.249094 osw-0.8.1/src/osw/model/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/model/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/model/page_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/model/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/sparql_client_smw.py
--rw-r--r--   0 runner    (1001) docker     (123)    37510 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/wiki_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    22013 2023-06-09 16:39:08.000000 osw-0.8.1/src/osw/wtsite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.245094 osw-0.8.1/src/osw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-09 16:39:45.000000 osw-0.8.1/src/osw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-09 16:39:45.000000 osw-0.8.1/src/osw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:39:45.000000 osw-0.8.1/src/osw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:39:44.000000 osw-0.8.1/src/osw.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-09 16:39:45.000000 osw-0.8.1/src/osw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-09 16:39:45.000000 osw-0.8.1/src/osw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.249094 osw-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-09 16:39:08.000000 osw-0.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-09 16:39:08.000000 osw-0.8.1/tests/controller_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:39:45.249094 osw-0.8.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-09 16:39:08.000000 osw-0.8.1/tests/integration/db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-09 16:39:08.000000 osw-0.8.1/tests/integration/login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-09 16:39:08.000000 osw-0.8.1/tests/integration/store_and_load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-09 16:39:08.000000 osw-0.8.1/tests/sparql_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-09 16:39:08.000000 osw-0.8.1/tests/test_credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-09 16:39:08.000000 osw-0.8.1/tests/test_osl.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-09 16:39:08.000000 osw-0.8.1/tests/test_wiki_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-09 16:39:08.000000 osw-0.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.371859 osw-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-13 05:47:30.000000 osw-0.9.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.335859 osw-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.347859 osw-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-13 05:47:30.000000 osw-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-13 05:47:30.000000 osw-0.9.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-13 05:47:30.000000 osw-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 05:47:30.000000 osw-0.9.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 05:47:30.000000 osw-0.9.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-13 05:47:30.000000 osw-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-13 05:47:30.000000 osw-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-13 05:47:30.000000 osw-0.9.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 05:47:30.000000 osw-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-13 05:47:30.000000 osw-0.9.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-06-13 05:47:30.000000 osw-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-06-13 05:47:30.000000 osw-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-13 05:48:03.371859 osw-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-13 05:47:30.000000 osw-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 05:47:30.000000 osw-0.9.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.351859 osw-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 05:47:30.000000 osw-0.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.351859 osw-0.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 05:47:30.000000 osw-0.9.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 05:47:30.000000 osw-0.9.0/docs/auth.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 05:47:30.000000 osw-0.9.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 05:47:30.000000 osw-0.9.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-06-13 05:47:30.000000 osw-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 05:47:30.000000 osw-0.9.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-13 05:47:30.000000 osw-0.9.0/docs/controller.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-13 05:47:30.000000 osw-0.9.0/docs/dev.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-13 05:47:30.000000 osw-0.9.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 05:47:30.000000 osw-0.9.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 05:47:30.000000 osw-0.9.0/docs/model.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 05:47:30.000000 osw-0.9.0/docs/osw.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 05:47:30.000000 osw-0.9.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 05:47:30.000000 osw-0.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 05:47:30.000000 osw-0.9.0/docs/tools.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.355859 osw-0.9.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-13 05:47:30.000000 osw-0.9.0/examples/accounts.pwd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-13 05:47:30.000000 osw-0.9.0/examples/controller_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 05:47:30.000000 osw-0.9.0/examples/create_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-13 05:47:30.000000 osw-0.9.0/examples/create_page_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.355859 osw-0.9.0/examples/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-13 05:47:30.000000 osw-0.9.0/examples/data_processing/local_jsonpath_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-13 05:47:30.000000 osw-0.9.0/examples/database_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-06-13 05:47:30.000000 osw-0.9.0/examples/entity_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19104 2023-06-13 05:47:30.000000 osw-0.9.0/examples/gui_local_slot_editing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-13 05:47:30.000000 osw-0.9.0/examples/load_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-06-13 05:47:30.000000 osw-0.9.0/examples/ontology_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-06-13 05:47:30.000000 osw-0.9.0/examples/page_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-13 05:47:30.000000 osw-0.9.0/examples/register_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-13 05:47:30.000000 osw-0.9.0/examples/settings.example.json
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-13 05:47:30.000000 osw-0.9.0/examples/store_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-13 05:47:30.000000 osw-0.9.0/examples/update_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-13 05:47:30.000000 osw-0.9.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.339859 osw-0.9.0/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.355859 osw-0.9.0/nb/quantities/
+-rw-r--r--   0 runner    (1001) docker     (123)   123529 2023-06-13 05:47:30.000000 osw-0.9.0/nb/quantities/Quantities.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.359859 osw-0.9.0/nb/quantities/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-06-13 05:47:30.000000 osw-0.9.0/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   107607 2023-06-13 05:47:30.000000 osw-0.9.0/nb/quantities/archive/broader.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    59112 2023-06-13 05:47:30.000000 osw-0.9.0/nb/quantities/archive/buildDictionaryTest.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   152865 2023-06-13 05:47:30.000000 osw-0.9.0/nb/quantities/archive/httpRequest.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-06-13 05:47:30.000000 osw-0.9.0/nb/quantities/archive/idea.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-06-13 05:47:30.000000 osw-0.9.0/nb/quantities/archive/querys.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-06-13 05:47:30.000000 osw-0.9.0/nb/quantities/archive/searchRunaways.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.359859 osw-0.9.0/nb/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)   404547 2023-06-13 05:47:30.000000 osw-0.9.0/nb/translations/DeeplTranslate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-13 05:47:30.000000 osw-0.9.0/nb/translations/JsObjectToJson.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-13 05:47:30.000000 osw-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-13 05:48:03.371859 osw-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-13 05:47:30.000000 osw-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.339859 osw-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.363860 osw-0.9.0/src/osw/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.367859 osw-0.9.0/src/osw/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/controller/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/controller/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/controller/page_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23078 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.367859 osw-0.9.0/src/osw/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/model/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/model/page_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/model/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/sparql_client_smw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.367859 osw-0.9.0/src/osw/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23448 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/utils/data_import_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37510 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/wiki_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33792 2023-06-13 05:47:30.000000 osw-0.9.0/src/osw/wtsite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.363860 osw-0.9.0/src/osw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-13 05:48:03.000000 osw-0.9.0/src/osw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-13 05:48:03.000000 osw-0.9.0/src/osw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:48:03.000000 osw-0.9.0/src/osw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:48:03.000000 osw-0.9.0/src/osw.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-13 05:48:03.000000 osw-0.9.0/src/osw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 05:48:03.000000 osw-0.9.0/src/osw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.371859 osw-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-13 05:47:30.000000 osw-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-13 05:47:30.000000 osw-0.9.0/tests/controller_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-13 05:47:30.000000 osw-0.9.0/tests/data_import_utility_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:03.371859 osw-0.9.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-13 05:47:30.000000 osw-0.9.0/tests/integration/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 05:47:30.000000 osw-0.9.0/tests/integration/login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-13 05:47:30.000000 osw-0.9.0/tests/integration/store_and_load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-13 05:47:30.000000 osw-0.9.0/tests/sparql_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-13 05:47:30.000000 osw-0.9.0/tests/test_credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-13 05:47:30.000000 osw-0.9.0/tests/test_osl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-13 05:47:30.000000 osw-0.9.0/tests/test_wiki_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-13 05:47:30.000000 osw-0.9.0/tox.ini
```

### Comparing `osw-0.8.1/.coveragerc` & `osw-0.9.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/.github/workflows/ci.yml` & `osw-0.9.0/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
   test:
     needs: prepare
     strategy:
       matrix:
         python:
         - "3.8"  # oldest Python supported by PSF
-        - "3.10"  # newest Python that is stable
+        - "3.11"  # newest Python that is stable
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
     runs-on: ${{ matrix.platform }}
     steps:
       - uses: actions/checkout@v3
```

### Comparing `osw-0.8.1/.github/workflows/docs.yml` & `osw-0.9.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/.gitignore` & `osw-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/.pre-commit-config.yaml` & `osw-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/CONTRIBUTING.md` & `osw-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/LICENSE.txt` & `osw-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/PKG-INFO` & `osw-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: osw
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python toolset for data processing, queries, wikicode generation and page manipulation
 Home-page: https://github.com/OpenSemanticLab/osw-python
 Author: "Simon Stier"
 Author-email: simon.stier@isc.fraunhofer.de
 License: AGPL-3.0-or-later
 Project-URL: Documentation, https://opensemanticlab.github.io/osw-python/
 Project-URL: Source, https://github.com/OpenSemanticLab/osw-python
 Project-URL: Changelog, https://github.com/OpenSemanticLab/osw-python/blob/main/CHANGELOG.md
 Project-URL: Download, https://pypi.org/project/osw/#files
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: dataimport
 Provides-Extra: DB
+Provides-Extra: UI
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 <!-- These are examples of badges you might want to add to your README:
      please update the URLs accordingly
 
 [![Built Status](https://api.cirrus-ci.com/github/<USER>/osw.svg?branch=main)](https://cirrus-ci.com/github/<USER>/osw)
```

### Comparing `osw-0.8.1/README.md` & `osw-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/docs/Makefile` & `osw-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/docs/conf.py` & `osw-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/docs/index.md` & `osw-0.9.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/examples/controller_logic.py` & `osw-0.9.0/examples/controller_logic.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/examples/create_page_package.py` & `osw-0.9.0/examples/create_page_package.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/examples/data_processing/local_jsonpath_queries.py` & `osw-0.9.0/examples/data_processing/local_jsonpath_queries.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/examples/database_access.py` & `osw-0.9.0/examples/database_access.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/examples/entity_manipulation.py` & `osw-0.9.0/examples/entity_manipulation.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/examples/load_entity.py` & `osw-0.9.0/examples/load_entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/examples/local_editing.py` & `osw-0.9.0/examples/gui_local_slot_editing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,9 @@
-"""
-# todo: docstring erzeugen
-
-verwende: beispiel create page package
-https://github.com/OpenSemanticLab/osw-python/blob/main/examples/create_page_package.py
-in wtsite neuen parameter hinzufügen --> label als file name:
-dumpy_empty_slots = False
-https://github.com/OpenSemanticLab/osw-python/blob/main/src/osw/wtsite.py#L112
-"""
+"""This script provides a GUI for downloading an OSW instances page slots, editing
+them locally and uploading them again."""
 import json
 import os
 
 # import yaml
 from pathlib import Path
 from typing import Union
 
@@ -37,40 +30,47 @@
 LWD_DEFAULT = Path(os.getcwd()).parent / "data"
 SETTINGS_FILE_PATH_DEFAULT = os.path.join(
     os.path.dirname(os.path.abspath(__file__)), "settings.json"
 )
 CREDENTIALS_FILE_PATH_DEFAULT = os.path.join(
     os.path.dirname(os.path.abspath(__file__)), "accounts.pwd.yaml"
 )
+PACKAGE_INFO_FILE_NAME = "packages.json"
+# Sub folder to store the slot content of the page in. If None, the content is stored
+#  in the root folder alongside the package info file.
+SUB_LEVEL = None  # "content"
+# Whether to store the page content in a sub folder named after the namespace
+NAMESPACE_AS_FOLDER = False
 
 
 # Definition of functions
 def str_or_none(value):
     if str(value) == "" or value is None:
         return str("None")
     else:
         return str(value)
 
 
-def create_config_from_setting(settings_: dict):
+def create_config_from_setting(settings_: dict) -> WtPage.PageDumpConfig:
     config_ = WtPage.PageDumpConfig(
         target_dir=settings_["local_working_directory"],
+        namespace_as_folder=settings_["namespace_as_folder"],
         dump_empty_slots=settings_["dump_empty_slots"],
         page_name_as_filename=settings_["page_name_as_filename"],
     )
     return config_
 
 
-def create_page_package(
+def save_as_page_package(
     full_page_name_str,
     wtsite_inst: WtSite,
     dump_config_inst: WtPage.PageDumpConfig,
     label_str: str = None,
     top_level: str = None,
-    sub_level: str = "content",
+    sub_level: str = None,  # "content"
     author: Union[str, list] = "Open Semantic World",
 ):
     if top_level is None:
         top_level = full_page_name_str.split(":")[-1]
     package_repo_org = "OpenSemanticWorld-Packages"
     package_repo = f"{top_level}.{sub_level}"
     package_id = f"{top_level}.{sub_level}"
@@ -85,358 +85,411 @@
         target_dir = os.path.join(working_dir, top_level)
     if isinstance(author, list):
         author_list = author
     elif isinstance(author, str):
         author_list = [author]
     else:
         author_list = [""]
-
+    if package_subdir is None:
+        base_url = (
+            f"https://raw.githubusercontent.com/{package_repo_org}/"
+            f"{package_repo}/{package_branch}/"
+        )
+        content_path = target_dir
+    else:
+        base_url = (
+            f"https://raw.githubusercontent.com/{package_repo_org}/"
+            f"{package_repo}/{package_branch}/{package_subdir}/"
+        )
+        content_path = os.path.join(target_dir, package_subdir)
     bundle = package.PagePackageBundle(
         publisher=publisher,
         author=author_list,
         language="en",
         publisherURL=f"https://github.com/{package_repo_org}/{package_repo}",
         packages={
             f"{package_name}": package.PagePackage(
                 globalID=f"{package_id}",
                 label=package_name,
                 version="0.0.1",
                 description="Created by the GUI for local editing of OSW pages",
-                baseURL=f"https://raw.githubusercontent.com/{package_repo_org}/"
-                f"{package_repo}/{package_branch}/{package_subdir}/",
+                baseURL=base_url,
             )
         },
     )
+    config = package.PagePackageConfig(
+        name=package_name,
+        config_path=os.path.join(target_dir, PACKAGE_INFO_FILE_NAME),
+        content_path=content_path,
+        bundle=bundle,
+        titles=[full_page_name_str],
+    )
     wtsite_inst.create_page_package(
-        config=package.PagePackageConfig(
-            name=package_name,
-            config_path=os.path.join(target_dir, "packages.json"),
-            content_path=os.path.join(target_dir, package_subdir),
-            bundle=bundle,
-            titles=[full_page_name_str],
-        ),
+        config=config,
         dump_config=dump_config_inst,
         debug=False,
     )
+    return {"Page package bundle": bundle, "Page package config": config}
 
 
-# Predefining some variables before execution
-settings_file_path = SETTINGS_FILE_PATH_DEFAULT
-if os.path.exists(settings_file_path):
-    with open(settings_file_path, "r") as f:
-        settings = json.load(f)
-    settings_read_from_file = True
-else:
-    settings = {
-        "credentials_file_path": str(CREDENTIALS_FILE_PATH_DEFAULT),
-        "local_working_directory": str(LWD_DEFAULT),
-        "settings_file_path": str(SETTINGS_FILE_PATH_DEFAULT),
-        "target_page": TARGET_PAGE_DEFAULT,
-        "dump_empty_slots": DUMP_EMPTY_SLOTS_DEFAULT,
-        "page_name_as_filename": True,
-        "slots_to_upload": SLOTS_TO_UPLOAD_DEFAULT,
-        "domain": "",
-    }
-    settings_read_from_file = False
+if __name__ == "__main__":
+    # Predefining some variables before execution
+    settings_file_path = SETTINGS_FILE_PATH_DEFAULT
+    if os.path.exists(settings_file_path):
+        with open(settings_file_path, "r") as f:
+            settings = json.load(f)
+        settings_read_from_file = True
+    else:
+        settings = {
+            "credentials_file_path": str(CREDENTIALS_FILE_PATH_DEFAULT),
+            "local_working_directory": str(LWD_DEFAULT),
+            "settings_file_path": str(SETTINGS_FILE_PATH_DEFAULT),
+            "target_page": TARGET_PAGE_DEFAULT,
+            "namespace_as_folder": NAMESPACE_AS_FOLDER,
+            "dump_empty_slots": DUMP_EMPTY_SLOTS_DEFAULT,
+            "page_name_as_filename": True,
+            "slots_to_upload": SLOTS_TO_UPLOAD_DEFAULT,
+            "domain": "",
+        }
+        settings_read_from_file = False
 
-domains, accounts = read_domains_from_credentials_file(
-    settings["credentials_file_path"]
-)
-domain = domains[0]
-if settings_read_from_file:
-    settings["domain"] = domain
+    domains, accounts = read_domains_from_credentials_file(
+        settings["credentials_file_path"]
+    )
+    if "wiki-dev.open-semantic-lab.org" in domains:
+        domain = "wiki-dev.open-semantic-lab.org"
+    else:
+        domain = domains[0]
+    if settings_read_from_file:
+        settings["domain"] = domain
 
-wtsite_obj = WtSite.from_domain(
-    domain=domains[0], password_file="", credentials=accounts[domains[0]]
-)
-osw_obj = OSW(site=wtsite_obj)
+    wtsite_obj = WtSite.from_domain(
+        domain=domain, password_file="", credentials=accounts[domain]
+    )
+    osw_obj = OSW(site=wtsite_obj)
 
-full_page_name = settings["target_page"].split("/")[-1].replace("_", " ")
-page = wtsite_obj.get_WtPage(full_page_name)
-label_set = False
-label = None
-
-# ----- GUI Definition -----
-# Setting the theme of the GUI
-psg.theme(GUI_THEME)
-# Settings
-settings_layout = [
-    [psg.Text("Settings", font=("Helvetica", 20))],
-    [
-        psg.Column(
-            [
-                [
-                    psg.Text("Settings file"),
-                ],
-                [
-                    psg.Text("Credentials file"),
-                ],
-                [
-                    psg.Text("Local working directory"),
-                ],
-            ]
-        ),
-        psg.Column(
-            [
-                [
-                    psg.In(
-                        size=(50, 1),
-                        enable_events=True,
-                        key="-SETTINGS-",
-                        default_text=settings["settings_file_path"],
-                    ),
-                    psg.FileBrowse(button_text="Browse", key="-BROWSE_SETTINGS-"),
-                    psg.Button("Load", key="-LOAD_SETTINGS-"),
-                    psg.Button("Save", key="-SAVE_SETTINGS-"),
-                ],
-                [
-                    psg.In(
-                        size=(50, 1),
-                        enable_events=True,
-                        key="-CREDENTIALS-",
-                        default_text=settings["credentials_file_path"],
-                    ),
-                    psg.FileBrowse(button_text="Browse", key="-BROWSE_CREDENTIALS-"),
-                ],
-                [
-                    psg.In(
-                        size=(50, 1),
-                        enable_events=True,
-                        key="-LWD-",
-                        default_text=settings["local_working_directory"],
-                    ),
-                    psg.FolderBrowse(button_text="Browse", key="-BROWSE_LWD-"),
-                ],
-            ]
-        ),
-    ],
-    [psg.HSeparator()],
-]
-# Actions
-actions_layout = [
+    full_page_name = settings["target_page"].split("/")[-1].replace("_", " ")
+    page = wtsite_obj.get_WtPage(full_page_name)
+    label_set = False
+    label = None
+    slots_downloaded = False
+    dump_config = create_config_from_setting(settings)
+
+    # ----- GUI Definition -----
+    # Setting the theme of the GUI
+    psg.theme(GUI_THEME)
+    # Settings
+    settings_layout = [
+        [psg.Text("Settings", font=("Helvetica", 20))],
+        [
+            psg.Column(
+                [
+                    [
+                        psg.Text("Settings file"),
+                    ],
+                    [
+                        psg.Text("Credentials file"),
+                    ],
+                    [
+                        psg.Text("Local working directory"),
+                    ],
+                ]
+            ),
+            psg.Column(
+                [
+                    [
+                        psg.In(
+                            size=(50, 1),
+                            enable_events=True,
+                            key="-SETTINGS-",
+                            default_text=settings["settings_file_path"],
+                        ),
+                        psg.FileBrowse(button_text="Browse", key="-BROWSE_SETTINGS-"),
+                        psg.Button("Load", key="-LOAD_SETTINGS-"),
+                        psg.Button("Save", key="-SAVE_SETTINGS-"),
+                    ],
+                    [
+                        psg.In(
+                            size=(50, 1),
+                            enable_events=True,
+                            key="-CREDENTIALS-",
+                            default_text=settings["credentials_file_path"],
+                        ),
+                        psg.FileBrowse(
+                            button_text="Browse", key="-BROWSE_CREDENTIALS-"
+                        ),
+                    ],
+                    [
+                        psg.In(
+                            size=(50, 1),
+                            enable_events=True,
+                            key="-LWD-",
+                            default_text=settings["local_working_directory"],
+                        ),
+                        psg.FolderBrowse(button_text="Browse", key="-BROWSE_LWD-"),
+                    ],
+                ]
+            ),
+        ],
+        [psg.HSeparator()],
+    ]
     # Actions
-    [psg.Text("Actions", font=("Helvetica", 20))],
-    # Target OSW instance
-    [psg.Text("Target OSW instance", font=("Helvetica", 16))],
-    [psg.Text("List of domains is read from accounts.pwd.yaml!")],
-    [psg.Combo(domains, default_value=domains[0], key="-DOMAIN-", enable_events=True)],
-    # Target page
-    [psg.Text("Target page", font=("Helvetica", 16))],
-    [
-        psg.Column(
-            [
-                [psg.Text("Address, within selected OSW instance")],
-                [psg.Text("First label of the OSW page:")],
-            ]
-        ),
-        psg.Column(
-            [
-                [
-                    psg.InputText(
-                        size=(50, 1),
-                        default_text=settings["target_page"],
-                        key="-ADDRESS-",
-                    ),
-                    psg.Button("Load page"),
-                ],
-                [
-                    # A display element that will show the label of the OSW page
-                    psg.Multiline(size=(50, 1), key="-LABEL-", no_scrollbar=True)
-                ],
-            ]
-        ),
-    ],
-    # [
-    #     psg.HSeparator()
-    # ],
-    # Slots to download
-    [psg.Text("Slots to download", font=("Helvetica", 16))],
-    [
-        psg.Column(
-            [
-                [
-                    psg.Radio(
-                        "Include empty slots",
-                        group_id="-RADIO1-",
-                        default=settings["dump_empty_slots"],
-                        key="-INC_EMPTY-",
-                        enable_events=True,
-                    )
-                ],
-                [
-                    psg.Radio(
-                        "Exclude empty slots",
-                        group_id="-RADIO1-",
-                        default=(not settings["dump_empty_slots"]),
-                        key="-EXC_EMPTY-",
-                        enable_events=True,
-                    )
-                ],
-                [psg.Button("Download selected", key="-DL-")],
-                [psg.Multiline(size=(20, 1), key="-DL_RES-", no_scrollbar=True)],
-            ]
-        ),
-    ],
-    # [
-    #     psg.HSeparator()
-    # ],
-    # Slots to upload
-    [psg.Text("Slots to upload", font=("Helvetica", 16))],
-    [
-        psg.Column(
-            [
-                [psg.Button("(De)Select all", key="-UL_SEL-")],
-                [
-                    psg.Listbox(
-                        values=SLOTS.keys(),
-                        default_values=settings["slots_to_upload"],
-                        size=(20, 10),
-                        key="-UL_LIST-",
-                        select_mode=psg.LISTBOX_SELECT_MODE_MULTIPLE,
-                        enable_events=True,
-                        no_scrollbar=True,
-                    )
-                ],
-                [psg.Button("Upload selected", key="-UL-")],
-                [psg.Multiline(size=(20, 1), key="-UL_RES-", no_scrollbar=True)],
+    actions_layout = [
+        # Actions
+        [psg.Text("Actions", font=("Helvetica", 20))],
+        # Target OSW instance
+        [psg.Text("Target OSW instance", font=("Helvetica", 16))],
+        [psg.Text("List of domains is read from accounts.pwd.yaml!")],
+        [psg.Combo(domains, default_value=domain, key="-DOMAIN-", enable_events=True)],
+        # Target page
+        [psg.Text("Target page", font=("Helvetica", 16))],
+        [
+            psg.Column(
+                [
+                    [psg.Text("Address, within selected OSW instance")],
+                    [psg.Text("First label of the OSW page:")],
+                ]
+            ),
+            psg.Column(
+                [
+                    [
+                        psg.InputText(
+                            size=(50, 1),
+                            default_text=settings["target_page"],
+                            key="-ADDRESS-",
+                        ),
+                        psg.Button("Load page"),
+                    ],
+                    [
+                        # A display element that will show the label of the OSW page
+                        psg.Multiline(size=(50, 1), key="-LABEL-", no_scrollbar=True)
+                    ],
+                ]
+            ),
+        ],
+        # [
+        #     psg.HSeparator()
+        # ],
+        # Slots to download
+        [psg.Text("Slots to download", font=("Helvetica", 16))],
+        [
+            psg.Column(
+                [
+                    [
+                        psg.Radio(
+                            "Include empty slots",
+                            group_id="-RADIO1-",
+                            default=settings["dump_empty_slots"],
+                            key="-INC_EMPTY-",
+                            enable_events=True,
+                        )
+                    ],
+                    [
+                        psg.Radio(
+                            "Exclude empty slots",
+                            group_id="-RADIO1-",
+                            default=(not settings["dump_empty_slots"]),
+                            key="-EXC_EMPTY-",
+                            enable_events=True,
+                        )
+                    ],
+                    [psg.Button("Download selected", key="-DL-")],
+                    [psg.Multiline(size=(20, 1), key="-DL_RES-", no_scrollbar=True)],
+                ]
+            ),
+        ],
+        # [
+        #     psg.HSeparator()
+        # ],
+        # Slots to upload
+        [psg.Text("Slots to upload", font=("Helvetica", 16))],
+        [
+            psg.Column(
+                [
+                    [psg.Button("(De)Select all", key="-UL_SEL-")],
+                    [
+                        psg.Listbox(
+                            values=SLOTS.keys(),
+                            default_values=settings["slots_to_upload"],
+                            size=(20, 10),
+                            key="-UL_LIST-",
+                            select_mode=psg.LISTBOX_SELECT_MODE_MULTIPLE,
+                            enable_events=True,
+                            no_scrollbar=True,
+                        )
+                    ],
+                    [psg.Button("Upload selected", key="-UL-")],
+                    [psg.Multiline(size=(20, 1), key="-UL_RES-", no_scrollbar=True)],
+                ]
+            )
+        ],
+    ]
+    output_layout = [
+        [psg.HSeparator()],
+        # Output
+        [psg.Text("Debug output", font=("Helvetica", 20))],
+        [psg.Multiline(key="-OUTPUT-", size=(100, 10))],
+    ]
+    # The full layout
+    layout = settings_layout + actions_layout
+    if DEBUG:
+        layout += output_layout
+    # Create the window
+    window = psg.Window("OSW local editing GUI", layout)
+    # Create an event loop
+    while True:
+        event, values = window.read()
+        # End program if user closes window or
+        # presses the OK button
+        if event == "OK" or event == psg.WIN_CLOSED:
+            break
+        elif event == "-SETTINGS-":
+            settings["settings_file_path"] = values["-SETTINGS-"]
+        elif event == "-LOAD_SETTINGS-":
+            # update settings
+            with open(settings["settings_file_path"], "r") as f:
+                settings = json.load(f)
+            # update GUI
+            window["-CREDENTIALS-"].update(settings["credentials_file_path"]),
+            window["-LWD-"].update(settings["local_working_directory"])
+            window["-DOMAIN-"].update(settings["domain"])
+            window["-ADDRESS-"].update(settings["target_page"])
+            window["-INC_EMPTY-"].update(settings["dump_empty_slots"])
+            window["-EXC_EMPTY-"].update(not settings["dump_empty_slots"])
+            indices = [
+                i
+                for i, x in enumerate(SLOTS.keys())
+                if x in settings["slots_to_upload"]
             ]
-        )
-    ],
-]
-output_layout = [
-    [psg.HSeparator()],
-    # Output
-    [psg.Text("Debug output", font=("Helvetica", 20))],
-    [psg.Multiline(key="-OUTPUT-", size=(100, 10))],
-]
-# The full layout
-layout = settings_layout + actions_layout
-if DEBUG:
-    layout += output_layout
-# Create the window
-window = psg.Window("OSW local editing GUI", layout)
-# Create an event loop
-while True:
-    event, values = window.read()
-    # End program if user closes window or
-    # presses the OK button
-    if event == "OK" or event == psg.WIN_CLOSED:
-        break
-    elif event == "-SETTINGS-":
-        settings["settings_file_path"] = values["-SETTINGS-"]
-    elif event == "-LOAD_SETTINGS-":
-        # update settings
-        with open(settings["settings_file_path"], "r") as f:
-            settings = json.load(f)
-        # update GUI
-        window["-CREDENTIALS-"].update(settings["credentials_file_path"]),
-        window["-LWD-"].update(settings["local_working_directory"])
-        window["-DOMAIN-"].update(settings["domain"])
-        window["-ADDRESS-"].update(settings["target_page"])
-        window["-INC_EMPTY-"].update(settings["dump_empty_slots"])
-        window["-EXC_EMPTY-"].update(not settings["dump_empty_slots"])
-        indices = [
-            i for i, x in enumerate(SLOTS.keys()) if x in settings["slots_to_upload"]
-        ]
-        window["-UL_LIST-"].update(set_to_index=indices)
-        settings_read_from_file = True
-    elif event == "-SAVE_SETTINGS-":
-        with open(settings["settings_file_path"], "w") as f:
-            json.dump(settings, f, indent=4)
-    elif event == "-CREDENTIALS-":
-        settings["credentials_file_path"] = values["-CREDENTIALS-"]
-        domains, accounts = read_domains_from_credentials_file(
-            settings["credentials_file_path"]
-        )
-        window["-DOMAIN-"].update(values=domains)
-    elif event == "-LWD-":
-        settings["local_working_directory"] = values["-LWD-"]
-    elif event == "-DOMAIN-":
-        settings["domain"] = values["-DOMAIN-"]
-        domain = settings["domain"].split("//")[-1]
-        wtsite_obj = WtSite.from_domain(
-            domain=settings["domain"],
-            password_file="",
-            credentials=accounts[settings["domain"]],
-        )
-        osw_obj = OSW(site=wtsite_obj)
-    elif event == "Load page":
-        full_page_name = values["-ADDRESS-"].split("/")[-1].replace("_", " ")
-        if (values["-ADDRESS-"].find("/wiki/") != -1) or (
-            values["-ADDRESS-"].find("/w/") != -1
-        ):
-            settings["target_page"] = values["-ADDRESS-"]
-        else:
-            settings["target_page"] = "https://" + domain + "/wiki/" + full_page_name
-        if values["-ADDRESS-"].find(settings["domain"]) == -1:
-            window["-LABEL-"].update("Page not on selected domain!")
-            label_set = False
-        else:
-            # use connection
-            page = wtsite_obj.get_WtPage(full_page_name)
-            if page.exists:
-                jsondata = page.get_slot_content("jsondata")
-                if jsondata is None:
-                    window["-LABEL-"].update("Slot 'jsondata' is empty!")
-                    label_set = False
-                else:
-                    label = jsondata["label"][0]["text"]
-                    window["-LABEL-"].update(label)
-                    label_set = True
+            window["-UL_LIST-"].update(set_to_index=indices)
+            settings_read_from_file = True
+        elif event == "-SAVE_SETTINGS-":
+            with open(settings["settings_file_path"], "w") as f:
+                json.dump(settings, f, indent=4)
+        elif event == "-CREDENTIALS-":
+            settings["credentials_file_path"] = values["-CREDENTIALS-"]
+            domains, accounts = read_domains_from_credentials_file(
+                settings["credentials_file_path"]
+            )
+            window["-DOMAIN-"].update(values=domains)
+        elif event == "-LWD-":
+            settings["local_working_directory"] = values["-LWD-"]
+        elif event == "-DOMAIN-":
+            settings["domain"] = values["-DOMAIN-"]
+            domain = settings["domain"].split("//")[-1]
+            wtsite_obj = WtSite.from_domain(
+                domain=settings["domain"],
+                password_file="",
+                credentials=accounts[settings["domain"]],
+            )
+            osw_obj = OSW(site=wtsite_obj)
+        elif event == "Load page":
+            window["-LABEL-"].update("Loading page...")
+            window["-DL_RES-"].update("")
+            full_page_name = values["-ADDRESS-"].split("/")[-1].replace("_", " ")
+            if (values["-ADDRESS-"].find("/wiki/") != -1) or (
+                values["-ADDRESS-"].find("/w/") != -1
+            ):
+                settings["target_page"] = values["-ADDRESS-"]
             else:
-                window["-LABEL-"].update("Page does not exist!")
+                settings["target_page"] = (
+                    "https://" + domain + "/wiki/" + full_page_name
+                )
+            if values["-ADDRESS-"].find(settings["domain"]) == -1:
+                window["-LABEL-"].update("Page not on selected domain!")
                 label_set = False
-    elif event == "-EXC_EMPTY-" or event == "-INC_EMPTY-":
-        settings["dump_empty_slots"] = values["-INC_EMPTY-"]
-    elif event == "-DL-":
-        if label_set:
-            dump_config = create_config_from_setting(settings)
-            # _ = page.dump(dump_config)
-            create_page_package(
-                full_page_name_str=full_page_name,
-                wtsite_inst=wtsite_obj,
-                dump_config_inst=dump_config,
-                label_str=label,
-                author=accounts[domains[0]]["username"],
+            else:
+                # use connection
+                page = wtsite_obj.get_WtPage(full_page_name)
+                if page.exists:
+                    jsondata = page.get_slot_content("jsondata")
+                    if jsondata is None:
+                        window["-LABEL-"].update("Slot 'jsondata' is empty!")
+                        label_set = False
+                    else:
+                        label = jsondata["label"][0]["text"]
+                        window["-LABEL-"].update(label)
+                        label_set = True
+                else:
+                    window["-LABEL-"].update("Page does not exist!")
+                    label_set = False
+        elif event == "-EXC_EMPTY-" or event == "-INC_EMPTY-":
+            settings["dump_empty_slots"] = values["-INC_EMPTY-"]
+        elif event == "-DL-":
+            window["-DL_RES-"].update("Downloading slots...")
+            if label_set:
+                dump_config = create_config_from_setting(settings)
+                _ = save_as_page_package(
+                    full_page_name_str=full_page_name,
+                    wtsite_inst=wtsite_obj,
+                    dump_config_inst=dump_config,
+                    label_str=label,
+                    sub_level=SUB_LEVEL,
+                    author=accounts[domains[0]]["username"],
+                )
+                slots_downloaded = True
+                window["-DL_RES-"].update("Slots downloaded!")
+            else:
+                window["-DL_RES-"].update("No page loaded!")
+        elif event == "-UL_SEL-":
+            indices = list(window["-UL_LIST-"].get_indexes())
+            # All selected: deselect all
+            if indices == list(range(len(SLOTS.keys()))):
+                window["-UL_LIST-"].update(set_to_index=[])
+                settings["slots_to_upload"] = []
+            else:
+                window["-UL_LIST-"].update(set_to_index=list(range(len(SLOTS.keys()))))
+                settings["slots_to_upload"] = list(SLOTS.keys())
+        elif event == "-UL_LIST-":
+            indices = list(window["-UL_LIST-"].get_indexes())
+            settings["slots_to_upload"] = np_array(list(SLOTS.keys()))[indices].tolist()
+        elif event == "-UL-":
+            slots_to_upload = settings["slots_to_upload"]
+            if not label_set:
+                window["-UL_RES-"].update("No page loaded!")
+            elif len(slots_to_upload) == 0:
+                window["-UL_RES-"].update("No slots selected!")
+            else:
+                if not slots_downloaded:
+                    window["-UL_RES-"].update("No slots downloaded!")
+                    dump_config = create_config_from_setting(settings)
+                window["-UL_RES-"].update("Uploading slots...")
+                if SUB_LEVEL is None:
+                    storage_path = Path(dump_config.target_dir)
+                else:
+                    storage_path = Path(dump_config.target_dir).parent
+                pages = wtsite_obj.read_page_package(
+                    storage_path=storage_path,
+                    packages_info_file_name=PACKAGE_INFO_FILE_NAME,
+                    selected_slots=slots_to_upload,
+                    debug=False,
+                )
+                param = wtsite_obj.UploadPageParam(pages=pages, parallel=False)
+                wtsite_obj.upload_page(param)
+                # Success:
+                window["-UL_RES-"].update("Slots uploaded!")
+                # Report in the download section that the slots have been uploaded to
+                #  remind the user that he eventually has to re-download the slots
+                window["-DL_RES-"].update("Slots uploaded!")
+
+        # Some debugging output functionality
+        if DEBUG:
+            values_str = "\n".join(
+                [
+                    f"{key}: {str_or_none(value)}"
+                    for key, value in values.items()
+                    if key != "-OUTPUT-"
+                ]
             )
-            window["-DL_RES-"].update("Slots downloaded!")
-        else:
-            window["-DL_RES-"].update("No page loaded!")
-    elif event == "-UL_SEL-":
-        indices = list(window["-UL_LIST-"].get_indexes())
-        # All selected: deselect all
-        if indices == list(range(len(SLOTS.keys()))):
-            window["-UL_LIST-"].update(set_to_index=[])
-        else:
-            window["-UL_LIST-"].update(set_to_index=list(range(len(SLOTS.keys()))))
-    elif event == "-UL_LIST-":
-        indices = list(window["-UL_LIST-"].get_indexes())
-        settings["slots_to_upload"] = np_array(list(SLOTS.keys()))[indices].tolist()
-    elif event == "-UL-":
-        pass
-        # Success:
-        # window["-UL_RES-"].update("Slots uploaded!")
-        window["-UL_RES-"].update("Not yet implemented!")
-        # todo: no slot selected
+            listbox_selected_items_str = "\n".join(settings["slots_to_upload"])
 
-    # Some debugging output functionality
-    if DEBUG:
-        values_str = "\n".join(
-            [
-                f"{key}: {str_or_none(value)}"
-                for key, value in values.items()
-                if key != "-OUTPUT-"
-            ]
-        )
-        listbox_selected_items_str = "\n".join(settings["slots_to_upload"])
-
-        window["-OUTPUT-"].update(
-            f"Last event: {event}\n"
-            f"-----------\n"
-            f"Values:\n"
-            f"-------\n"
-            f"{values_str}"
-            f"\nListbox values:\n"
-            f"{listbox_selected_items_str}"
-        )
+            window["-OUTPUT-"].update(
+                f"Last event: {event}\n"
+                f"-----------\n"
+                f"Values:\n"
+                f"-------\n"
+                f"{values_str}"
+                f"\nListbox values:\n"
+                f"{listbox_selected_items_str}"
+            )
 
-window.close()
+    window.close()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `osw-0.8.1/examples/ontology_import.py` & `osw-0.9.0/examples/ontology_import.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/examples/page_manipulation.py` & `osw-0.9.0/examples/page_manipulation.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/examples/register_model.py` & `osw-0.9.0/examples/register_model.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/examples/settings.json` & `osw-0.9.0/examples/settings.example.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {"'namespace_as_folder'": 'False'}*

```diff
@@ -1,12 +1,13 @@
 {
     "credentials_file_path": "C:/Users/gold/github/osw-python/examples/accounts.pwd.yaml",
     "domain": "wiki-dev.open-semantic-lab.org",
     "dump_empty_slots": false,
     "local_working_directory": "C:\\Users\\gold\\github\\osw-python\\data",
+    "namespace_as_folder": false,
     "page_name_as_filename": true,
     "settings_file_path": "C:\\Users\\gold\\github\\osw-python\\examples\\settings.json",
     "slots_to_upload": [
         "main",
         "jsondata",
         "jsonschema",
         "header_template"
```

### Comparing `osw-0.8.1/examples/store_entity.py` & `osw-0.9.0/examples/store_entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/examples/update_local_model.py` & `osw-0.9.0/examples/update_local_model.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/nb/quantities/Quantities.ipynb` & `osw-0.9.0/nb/quantities/Quantities.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb` & `osw-0.9.0/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/nb/quantities/archive/broader.ipynb` & `osw-0.9.0/nb/quantities/archive/broader.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/nb/quantities/archive/buildDictionaryTest.ipynb` & `osw-0.9.0/nb/quantities/archive/buildDictionaryTest.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/nb/quantities/archive/httpRequest.ipynb` & `osw-0.9.0/nb/quantities/archive/httpRequest.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/nb/quantities/archive/idea.ipynb` & `osw-0.9.0/nb/quantities/archive/idea.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/nb/quantities/archive/querys.ipynb` & `osw-0.9.0/nb/quantities/archive/querys.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/nb/quantities/archive/searchRunaways.ipynb` & `osw-0.9.0/nb/quantities/archive/searchRunaways.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/nb/translations/DeeplTranslate.ipynb` & `osw-0.9.0/nb/translations/DeeplTranslate.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/nb/translations/JsObjectToJson.ipynb` & `osw-0.9.0/nb/translations/JsObjectToJson.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/setup.cfg` & `osw-0.9.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -39,27 +39,31 @@
 	typing_extensions
 	dataclasses
 	pathlib
 	sphinx
 	chardet
 	matplotlib
 	scipy
-	pysimplegui
+	dask
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
-DB = sqlalchemy; psycopg2
+dataimport = geopy; deepl
+DB = psycopg2; sqlalchemy
+UI = pysimplegui
 testing = 
-	setuptools~=63.4.1
-	pytest~=7.1.2
+	setuptools
+	pytest
 	pytest-cov
+	geopy
+	deepl
 	sqlalchemy
 	psycopg2
 
 [options.entry_points]
 
 [tool:pytest]
 addopts =
```

### Comparing `osw-0.8.1/setup.py` & `osw-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/src/osw/auth.py` & `osw-0.9.0/src/osw/auth.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,27 +12,39 @@
 
 class CredentialManager(OswBaseModel):
     """Handles credentials"""
 
     cred_filepath: Union[Union[str, FilePath], List[Union[str, FilePath]]]
     """yaml file with credentials for osw and connected services"""
 
-    class Credential(OswBaseModel):
-        """_summary_
+    class BaseCredential(OswBaseModel):
+        """Abstract base class for credentials"""
 
-        Parameters
-        ----------
-        username:
-            the user identifier
-        password:
-            the users password
-        """
+        iri: str
+        """the iri the credential is valid for"""
+
+    class UserPwdCredential(BaseCredential):
+        """a username - password credential"""
 
         username: str
+        """the user identifier"""
         password: str
+        """the users password"""
+
+    class OAuth1Credential(BaseCredential):
+        """OAuth1 credentials. See https://requests-oauthlib.readthedocs.io/en/latest/oauth1_workflow.html"""
+
+        consumer_token: str
+        """consumer token"""
+        consumer_secret: str
+        """consumer secret """
+        access_token: str
+        """access token"""
+        access_secret: str
+        """access secret"""
 
     class CredentialFallback(Enum):
         """Modes of handling missing credentials
 
         Attributes
         ----------
         none:
@@ -41,69 +53,69 @@
             use getpass to ask for credentials
         """
 
         ask = "ask"  # use getpass to ask for credentials
         none = "none"  # throw error
 
     class CredentialConfig(OswBaseModel):
-        """Reads credentials from a yaml file
-
-        Parameters
-        ----------
-        iri:
-            internationalized resource identifier / address of the service, may contain protocol, domain, port and path
-            matches by "contains" returning the shortest match
-        fallback:
-            The fallback strategy if no credential was found for the given origin
-        """
+        """Reads credentials from a yaml file"""
 
         iri: str
+        """internationalized resource identifier / address of the service, may contain protocol, domain, port and path
+            matches by "contains" returning the shortest match"""
         fallback: Optional[CredentialManager.CredentialFallback] = "none"
+        """The fallback strategy if no credential was found for the given origin"""
 
-    def get_credential(self, config: CredentialConfig) -> Credential:
+    def get_credential(self, config: CredentialConfig) -> BaseCredential:
         """Reads credentials from a yaml file
 
         Parameters
         ----------
         config:
             see CredentialConfig
 
         Returns
         -------
         credential :
-            Credential, contain attributes 'username' and 'password'.
+            Credential, contain attributes 'username' and 'password' and the matching iri.
         """
         filepaths = self.cred_filepath
         if type(filepaths) is not list:
             filepaths = [filepaths]
 
         match_iri = ""
         cred = None
         for filepath in filepaths:
             if filepath != "":
                 with open(filepath, "r") as stream:
                     try:
                         accounts = yaml.safe_load(stream)
                         for iri in accounts.keys():
                             if config.iri in iri:
-                                if match_iri == "" or len(match_iri) > len(iri):
+                                if match_iri == "" or len(match_iri) > len(
+                                    iri
+                                ):  # use the less specific match
                                     match_iri = iri
-                                    cred = CredentialManager.Credential(
+                                    cred = CredentialManager.UserPwdCredential(
                                         username=accounts[iri]["username"],
                                         password=accounts[iri]["password"],
+                                        iri=match_iri
+                                        if len(match_iri) > len(iri)
+                                        else iri  # use the more specific iri
+                                        # ToDo: add support for OAuth1Credential
                                     )
                     except yaml.YAMLError as exc:
                         print(exc)
         if cred is None:
             if config.fallback is CredentialManager.CredentialFallback.ask:
                 print(
                     f"No credentials for {config.iri} found. Please use the prompt to login"
                 )
                 username = input("Enter username")
                 password = getpass.getpass("Enter password")
-                cred = CredentialManager.Credential(
+                cred = CredentialManager.UserPwdCredential(
                     username=username, password=password
                 )
         return cred
 
 
 CredentialManager.CredentialConfig.update_forward_refs()
```

### Comparing `osw-0.8.1/src/osw/controller/__init__.py` & `osw-0.9.0/src/osw/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/src/osw/controller/database.py` & `osw-0.9.0/src/osw/controller/database.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/src/osw/controller/page_package.py` & `osw-0.9.0/src/osw/controller/page_package.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 from typing import Union
 
 from pydantic import FilePath
 
 import osw.model.page_package as model
+from osw.auth import CredentialManager
 from osw.model import page_package as package
 from osw.model.static import OswBaseModel
 from osw.wtsite import WtSite
 
 
 class PagePackageController(model.PagePackageMetaData):
     """Adds controller logic to a package definitions to create / update it"""
@@ -32,17 +33,21 @@
 
         Parameters
         ----------
         creation_config
             see PagePackageController.CreationConfig
         """
         # Create a WtSite instance to load pages from the specified domain
-        wtsite = WtSite.from_domain(
-            domain=creation_config.domain,
-            password_file=creation_config.credentials_file_path,
+        wtsite = WtSite(
+            WtSite.WtSiteConfig(
+                iri=creation_config.domain,
+                cred_mngr=CredentialManager(
+                    cred_filepath=creation_config.credentials_file_path
+                ),
+            )
         )
         # Create a PagePackageBundle instance
         bundle = package.PagePackageBundle(
             publisher=self.publisher,
             author=self.author,
             language=self.language,
             publisherURL=f"https://github.com/{self.repo_org}/{self.repo}",
```

### Comparing `osw-0.8.1/src/osw/core.py` & `osw-0.9.0/src/osw/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 import platform
 import re
 import sys
 from enum import Enum
 from typing import List, Optional, Union
 from uuid import UUID
 
+import dask
+from dask.diagnostics import ProgressBar
 from jsonpath_ng.ext import parse
 from pydantic import BaseModel, Field, create_model
 from pydantic.main import ModelMetaclass
 
 import osw.model.entity as model
+from osw.utils.util import BufferedPrint
 from osw.wtsite import WtSite
 
 
 class OswClassMetaclass(ModelMetaclass):
     def __new__(cls, name, bases, dic, osl_template, osl_footer_template):
         base_footer_cls = type(
             dic["__qualname__"] + "Footer",
@@ -465,57 +468,82 @@
             entity = cls(**jsondata)
 
         return entity
 
     class StoreEntityParam(model.OswBaseModel):
         entities: Union[model.Entity, List[model.Entity]]
         namespace: Optional[str]
+        parallel: Optional[bool] = False
 
     def store_entity(
         self, param: Union[StoreEntityParam, model.Entity, List[model.Entity]]
     ) -> None:
-        """stores the given datasclass instance as OSW page by calling BaseModel.json()
+        """stores the given dataclass instance as OSW page by calling BaseModel.json()
 
         Parameters
         ----------
-        entity
-            StoreParam, the datasclass instance or a list of instances
+        param:
+            StoreEntityParam, the dataclass instance or a list of instances
         """
 
         namespace = None
+        parallel = False
         entity = param
         if isinstance(param, OSW.StoreEntityParam):
             entity = param.entities
             namespace = param.namespace
-
+            parallel = param.parallel
         if not isinstance(entity, list):
             entity = [entity]
+        # entity is a list
         max_index = len(entity)
-        for index, e in enumerate(entity):
-            if namespace is None and isinstance(e, model.Item):
-                namespace = "Item"
-            if namespace is not None:
-                entity_title = namespace + ":" + OSW.get_osw_id(e.uuid)
+        if max_index >= 5:
+            parallel = True
+
+        def store_entity(index_, e_, namespace_=namespace):
+            if namespace_ is None and isinstance(e_, model.Item):
+                namespace_ = "Item"
+            if namespace_ is not None:
+                entity_title = namespace_ + ":" + OSW.get_osw_id(e_.uuid)
                 page = self.site.get_WtPage(entity_title)
                 jsondata = json.loads(
-                    e.json(exclude_none=True)
+                    e_.json(exclude_none=True)
                 )  # use pydantic serialization, skip none values
                 page.set_slot_content("jsondata", jsondata)
             else:
                 print("Error: Unsupported entity type")
                 return
-
             page.set_slot_content(
                 "header", "{{#invoke:Entity|header}}"
             )  # required for json parsing and header rendering
             page.set_slot_content(
                 "footer", "{{#invoke:Entity|footer}}"
             )  # required for footer rendering
             page.edit()
-            print(f"({index}/{max_index}) Entity stored at {page.get_url()}")
+            msg = f"({index_+1}/{max_index}) Entity stored at " f"{page.get_url()}."
+            if parallel:
+                print(msg, file=message_buffer)
+            else:
+                print(msg)
+
+        tasks = []
+        for index, e in enumerate(entity):
+            if not parallel:
+                store_entity(index, e)
+            else:
+                tasks.append(dask.delayed(store_entity)(index, e))
+        if parallel:
+            message_buffer = BufferedPrint()
+            print(
+                "(Parallel execution) Storing entities. Log will be printed after "
+                "completion."
+            )
+            with ProgressBar():
+                dask.compute(*tasks)
+            message_buffer.flush()
 
     def delete_entity(self, entity, comment: str = None):
         """deletes the given entity from the OSW instance
 
         Parameters
         ----------
         entity
```

### Comparing `osw-0.8.1/src/osw/model/entity.py` & `osw-0.9.0/src/osw/model/entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/src/osw/model/page_package.py` & `osw-0.9.0/src/osw/model/page_package.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/src/osw/model/static.py` & `osw-0.9.0/src/osw/model/static.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 This module is to be imported in the dynamically created and updated entity.py module.
 """
-from typing import Type, TypeVar
+from typing import Type, TypeVar, Union
 
 from pydantic import BaseModel
 
 T = TypeVar("T", bound=BaseModel)
 
 
 class OswBaseModel(BaseModel):
@@ -14,18 +14,18 @@
         for key in ("_osl_template", "_osl_footer"):
             if hasattr(self, key):
                 d[key] = getattr(self, key)
                 # Include selected private properties. note: private properties are not
                 #  considered as discriminator
         return d
 
-    def cast(self, cls: Type[T]) -> T:
+    def cast(self, cls: Union[Type[T], type]) -> T:
         return cls(**self.dict())
 
-    def cast_none_to_default(self, cls: Type[T]) -> T:
+    def cast_none_to_default(self, cls: Union[Type[T], type]) -> T:
         """Casting self into target class. If the passed attribute is None or solely
         includes None values, the attribute is not passed to the instance of the
         target class, which will then fall back to the default."""
 
         def test_if_empty_list_or_none(obj) -> bool:
             if obj is None:
                 return True
```

### Comparing `osw-0.8.1/src/osw/sparql_client_smw.py` & `osw-0.9.0/src/osw/sparql_client_smw.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/src/osw/wiki_tools.py` & `osw-0.9.0/src/osw/wiki_tools.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/src/osw.egg-info/PKG-INFO` & `osw-0.9.0/src/osw.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: osw
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python toolset for data processing, queries, wikicode generation and page manipulation
 Home-page: https://github.com/OpenSemanticLab/osw-python
 Author: "Simon Stier"
 Author-email: simon.stier@isc.fraunhofer.de
 License: AGPL-3.0-or-later
 Project-URL: Documentation, https://opensemanticlab.github.io/osw-python/
 Project-URL: Source, https://github.com/OpenSemanticLab/osw-python
 Project-URL: Changelog, https://github.com/OpenSemanticLab/osw-python/blob/main/CHANGELOG.md
 Project-URL: Download, https://pypi.org/project/osw/#files
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: dataimport
 Provides-Extra: DB
+Provides-Extra: UI
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 <!-- These are examples of badges you might want to add to your README:
      please update the URLs accordingly
 
 [![Built Status](https://api.cirrus-ci.com/github/<USER>/osw.svg?branch=main)](https://cirrus-ci.com/github/<USER>/osw)
```

### Comparing `osw-0.8.1/src/osw.egg-info/SOURCES.txt` & `osw-0.9.0/src/osw.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -36,20 +36,20 @@
 docs/_static/.gitignore
 examples/accounts.pwd.yaml
 examples/controller_logic.py
 examples/create_entity.py
 examples/create_page_package.py
 examples/database_access.py
 examples/entity_manipulation.py
+examples/gui_local_slot_editing.py
 examples/load_entity.py
-examples/local_editing.py
 examples/ontology_import.py
 examples/page_manipulation.py
 examples/register_model.py
-examples/settings.json
+examples/settings.example.json
 examples/store_entity.py
 examples/update_local_model.py
 examples/data_processing/local_jsonpath_queries.py
 nb/quantities/Quantities.ipynb
 nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb
 nb/quantities/archive/broader.ipynb
 nb/quantities/archive/buildDictionaryTest.ipynb
@@ -75,16 +75,20 @@
 src/osw/controller/database.py
 src/osw/controller/entity.py
 src/osw/controller/page_package.py
 src/osw/model/__init__.py
 src/osw/model/entity.py
 src/osw/model/page_package.py
 src/osw/model/static.py
+src/osw/utils/__init__.py
+src/osw/utils/data_import_utility.py
+src/osw/utils/util.py
 tests/conftest.py
 tests/controller_mixin.py
+tests/data_import_utility_test.py
 tests/sparql_client_test.py
 tests/test_credential_manager.py
 tests/test_osl.py
 tests/test_wiki_tools.py
 tests/integration/db_test.py
 tests/integration/login_test.py
 tests/integration/store_and_load_test.py
```

### Comparing `osw-0.8.1/tests/conftest.py` & `osw-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/tests/controller_mixin.py` & `osw-0.9.0/tests/controller_mixin.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/tests/integration/db_test.py` & `osw-0.9.0/tests/integration/db_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 def test_connect_and_query(
     wiki_domain, wiki_username, wiki_password, db_username, db_password
 ):
     site = mwclient.Site(host=wiki_domain)
     site.login(username=wiki_username, password=wiki_password)
-    wtsite = WtSite(site)
+    wtsite = WtSite(WtSite.WtSiteLegacyConfig(site=site))
     osw = OSW(site=wtsite)
 
     osw.fetch_schema(
         OSW.FetchSchemaParam(
             schema_title="Category:OSW02590972aeba46d7864ed492c0c11384",  # Host
             mode="replace",
         )
@@ -77,12 +77,14 @@
     db = osw.load_entity("Item:OSWb8cc7705e17c47b19331fdb045bfbca8")  # postgres
     db = db.cast(model.Database)
 
     # cast into controller and execute function
     db = db.cast(controller.DatabaseController)
     db.connect(
         controller.DatabaseController.ConnectionConfig(
-            cm=CredentialManager.Credential(username=db_username, password=db_password),
+            cm=CredentialManager.UserPwdCredential(
+                iri="", username=db_username, password=db_password
+            ),
             osw=osw,
         )
     )
     db.execute("SELECT * FROM public.sensors ORDER BY sensor_id ASC")
```

### Comparing `osw-0.8.1/tests/integration/store_and_load_test.py` & `osw-0.9.0/tests/integration/store_and_load_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # run with: tox -e test -- --wiki_domain domain --wiki_username user --wiki_password pass
 
 
 def test_store_and_load(wiki_domain, wiki_username, wiki_password):
     site = mwclient.Site(host=wiki_domain)
     site.login(username=wiki_username, password=wiki_password)
-    wtsite = WtSite(site)
+    wtsite = WtSite(WtSite.WtSiteLegacyConfig(site=site))
     osw = OSW(site=wtsite)
 
     my_entity = model.Item(label=[model.Label(text="MyItem")])
 
     osw.store_entity(my_entity)
 
     my_entity2 = osw.load_entity("Item:" + OSW.get_osw_id(my_entity.uuid))
```

### Comparing `osw-0.8.1/tests/sparql_client_test.py` & `osw-0.9.0/tests/sparql_client_test.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/tests/test_credential_manager.py` & `osw-0.9.0/tests/test_credential_manager.py`

 * *Files identical despite different names*

### Comparing `osw-0.8.1/tox.ini` & `osw-0.9.0/tox.ini`

 * *Files identical despite different names*

