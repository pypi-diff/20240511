# Comparing `tmp/synapse_super_invites-0.8.1.tar.gz` & `tmp/synapse_super_invites-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapse_super_invites-0.8.1.tar", last modified: Fri Nov 24 15:59:19 2023, max compression
+gzip compressed data, was "synapse_super_invites-0.8.2.tar", last modified: Sat May 11 20:32:12 2024, max compression
```

## Comparing `synapse_super_invites-0.8.1.tar` & `synapse_super_invites-0.8.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2023-11-24 15:59:19.158569 synapse_super_invites-0.8.1/
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2023-11-24 15:59:19.148569 synapse_super_invites-0.8.1/.github/
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2023-11-24 15:59:19.148569 synapse_super_invites-0.8.1/.github/workflows/
--rw-r--r--   0 ben       (1001) ben       (1001)     1094 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.1/.github/workflows/ci.yml
--rw-r--r--   0 ben       (1001) ben       (1001)     1786 2023-11-17 16:09:10.000000 synapse_super_invites-0.8.1/.github/workflows/release.yml
--rw-r--r--   0 ben       (1001) ben       (1001)      105 2023-11-17 14:46:55.000000 synapse_super_invites-0.8.1/.gitignore
--rw-r--r--   0 ben       (1001) ben       (1001)      805 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.1/.gitlab-ci.yml
--rw-r--r--   0 ben       (1001) ben       (1001)     3704 2023-11-24 15:59:19.158569 synapse_super_invites-0.8.1/PKG-INFO
--rw-r--r--   0 ben       (1001) ben       (1001)     2955 2023-11-24 15:58:03.000000 synapse_super_invites-0.8.1/README.md
--rw-r--r--   0 ben       (1001) ben       (1001)     3628 2023-11-17 16:04:33.000000 synapse_super_invites-0.8.1/alembic.ini
--rw-r--r--   0 ben       (1001) ben       (1001)      351 2023-11-15 22:30:55.000000 synapse_super_invites-0.8.1/example_server.py
--rw-r--r--   0 ben       (1001) ben       (1001)     1680 2023-11-21 10:21:42.000000 synapse_super_invites-0.8.1/pyproject.toml
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2023-11-24 15:59:19.148569 synapse_super_invites-0.8.1/scripts-dev/
--rwxr-xr-x   0 ben       (1001) ben       (1001)      354 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.1/scripts-dev/lint.sh
--rw-r--r--   0 ben       (1001) ben       (1001)       38 2023-11-24 15:59:19.158569 synapse_super_invites-0.8.1/setup.cfg
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2023-11-24 15:59:19.148569 synapse_super_invites-0.8.1/synapse_super_invites/
--rw-r--r--   0 ben       (1001) ben       (1001)     1772 2023-11-24 15:58:20.000000 synapse_super_invites-0.8.1/synapse_super_invites/__init__.py
--rw-r--r--   0 ben       (1001) ben       (1001)     3641 2023-11-17 16:04:48.000000 synapse_super_invites-0.8.1/synapse_super_invites/alembic.ini
--rw-r--r--   0 ben       (1001) ben       (1001)      681 2023-11-17 16:03:47.000000 synapse_super_invites-0.8.1/synapse_super_invites/config.py
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2023-11-24 15:59:19.155236 synapse_super_invites-0.8.1/synapse_super_invites/migration/
--rw-r--r--   0 ben       (1001) ben       (1001)     2302 2023-11-17 13:28:20.000000 synapse_super_invites-0.8.1/synapse_super_invites/migration/env.py
--rw-r--r--   0 ben       (1001) ben       (1001)      635 2023-11-14 17:03:24.000000 synapse_super_invites-0.8.1/synapse_super_invites/migration/script.py.mako
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2023-11-24 15:59:19.155236 synapse_super_invites-0.8.1/synapse_super_invites/migration/versions/
--rw-r--r--   0 ben       (1001) ben       (1001)     3218 2023-11-15 17:11:42.000000 synapse_super_invites-0.8.1/synapse_super_invites/migration/versions/25e4ec3cea32_added_token_table.py
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2023-11-24 15:59:19.155236 synapse_super_invites-0.8.1/synapse_super_invites/model/
--rw-r--r--   0 ben       (1001) ben       (1001)     2275 2023-11-15 17:11:42.000000 synapse_super_invites-0.8.1/synapse_super_invites/model/__init__.py
--rw-r--r--   0 ben       (1001) ben       (1001)        0 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.1/synapse_super_invites/py.typed
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2023-11-24 15:59:19.155236 synapse_super_invites-0.8.1/synapse_super_invites/resource/
--rw-r--r--   0 ben       (1001) ben       (1001)      111 2023-11-17 15:43:40.000000 synapse_super_invites-0.8.1/synapse_super_invites/resource/__init__.py
--rw-r--r--   0 ben       (1001) ben       (1001)     9005 2023-11-24 15:56:58.000000 synapse_super_invites-0.8.1/synapse_super_invites/resource/base.py
--rw-r--r--   0 ben       (1001) ben       (1001)     2340 2023-11-17 13:35:26.000000 synapse_super_invites-0.8.1/synapse_super_invites/resource/redeem.py
--rw-r--r--   0 ben       (1001) ben       (1001)     4151 2023-11-17 13:35:26.000000 synapse_super_invites-0.8.1/synapse_super_invites/resource/tokens.py
--rw-r--r--   0 ben       (1001) ben       (1001)     1923 2023-11-17 13:35:26.000000 synapse_super_invites-0.8.1/synapse_super_invites/resource/web_access.py
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2023-11-24 15:59:19.155236 synapse_super_invites-0.8.1/synapse_super_invites/static/
--rw-r--r--   0 ben       (1001) ben       (1001)      556 2023-11-15 23:09:11.000000 synapse_super_invites-0.8.1/synapse_super_invites/static/index.html
--rw-r--r--   0 ben       (1001) ben       (1001)    15721 2023-11-15 22:50:38.000000 synapse_super_invites-0.8.1/synapse_super_invites/static/pure-min.css
--rw-r--r--   0 ben       (1001) ben       (1001)       57 2023-11-15 23:06:08.000000 synapse_super_invites-0.8.1/synapse_super_invites/static/script.js
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2023-11-24 15:59:19.155236 synapse_super_invites-0.8.1/synapse_super_invites.egg-info/
--rw-r--r--   0 ben       (1001) ben       (1001)     3704 2023-11-24 15:59:19.000000 synapse_super_invites-0.8.1/synapse_super_invites.egg-info/PKG-INFO
--rw-r--r--   0 ben       (1001) ben       (1001)     1159 2023-11-24 15:59:19.000000 synapse_super_invites-0.8.1/synapse_super_invites.egg-info/SOURCES.txt
--rw-r--r--   0 ben       (1001) ben       (1001)        1 2023-11-24 15:59:19.000000 synapse_super_invites-0.8.1/synapse_super_invites.egg-info/dependency_links.txt
--rw-r--r--   0 ben       (1001) ben       (1001)      135 2023-11-24 15:59:19.000000 synapse_super_invites-0.8.1/synapse_super_invites.egg-info/requires.txt
--rw-r--r--   0 ben       (1001) ben       (1001)       22 2023-11-24 15:59:19.000000 synapse_super_invites-0.8.1/synapse_super_invites.egg-info/top_level.txt
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2023-11-24 15:59:19.155236 synapse_super_invites-0.8.1/tests/
-drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2023-11-24 15:59:19.155236 synapse_super_invites-0.8.1/tests/.local/
--rw-r--r--   0 ben       (1001) ben       (1001)        0 2023-11-15 22:24:54.000000 synapse_super_invites-0.8.1/tests/.local/.gitkeep
--rw-r--r--   0 ben       (1001) ben       (1001)     1739 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.1/tests/__init__.py
--rw-r--r--   0 ben       (1001) ben       (1001)      844 2023-11-15 23:09:33.000000 synapse_super_invites-0.8.1/tests/example_cfg.yml
--rw-r--r--   0 ben       (1001) ben       (1001)      865 2023-11-17 13:28:20.000000 synapse_super_invites-0.8.1/tests/test_config.py
--rw-r--r--   0 ben       (1001) ben       (1001)    24027 2023-11-24 15:54:24.000000 synapse_super_invites-0.8.1/tests/test_integrations.py
--rw-r--r--   0 ben       (1001) ben       (1001)      864 2023-11-24 15:59:10.000000 synapse_super_invites-0.8.1/tox.ini
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.052097 synapse_super_invites-0.8.2/
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.045431 synapse_super_invites-0.8.2/.github/
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/.github/workflows/
+-rw-r--r--   0 ben       (1001) ben       (1001)     1094 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.2/.github/workflows/ci.yml
+-rw-r--r--   0 ben       (1001) ben       (1001)     1786 2023-11-17 16:09:10.000000 synapse_super_invites-0.8.2/.github/workflows/release.yml
+-rw-r--r--   0 ben       (1001) ben       (1001)      105 2023-11-17 14:46:55.000000 synapse_super_invites-0.8.2/.gitignore
+-rw-r--r--   0 ben       (1001) ben       (1001)      805 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.2/.gitlab-ci.yml
+-rw-r--r--   0 ben       (1001) ben       (1001)     4107 2024-05-11 20:32:12.052097 synapse_super_invites-0.8.2/PKG-INFO
+-rw-r--r--   0 ben       (1001) ben       (1001)     3230 2024-05-11 20:28:53.000000 synapse_super_invites-0.8.2/README.md
+-rw-r--r--   0 ben       (1001) ben       (1001)     3628 2023-11-17 16:04:33.000000 synapse_super_invites-0.8.2/alembic.ini
+-rw-r--r--   0 ben       (1001) ben       (1001)      351 2023-11-15 22:30:55.000000 synapse_super_invites-0.8.2/example_server.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     1909 2024-05-11 20:11:27.000000 synapse_super_invites-0.8.2/pyproject.toml
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/scripts-dev/
+-rwxr-xr-x   0 ben       (1001) ben       (1001)      354 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.2/scripts-dev/lint.sh
+-rw-r--r--   0 ben       (1001) ben       (1001)       38 2024-05-11 20:32:12.052097 synapse_super_invites-0.8.2/setup.cfg
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites/
+-rw-r--r--   0 ben       (1001) ben       (1001)     1986 2024-05-11 20:22:14.000000 synapse_super_invites-0.8.2/synapse_super_invites/__init__.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     3641 2023-11-17 16:04:48.000000 synapse_super_invites-0.8.2/synapse_super_invites/alembic.ini
+-rw-r--r--   0 ben       (1001) ben       (1001)      681 2023-11-17 16:03:47.000000 synapse_super_invites-0.8.2/synapse_super_invites/config.py
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites/migration/
+-rw-r--r--   0 ben       (1001) ben       (1001)     2302 2023-11-17 13:28:20.000000 synapse_super_invites-0.8.2/synapse_super_invites/migration/env.py
+-rw-r--r--   0 ben       (1001) ben       (1001)      635 2023-11-14 17:03:24.000000 synapse_super_invites-0.8.2/synapse_super_invites/migration/script.py.mako
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites/migration/versions/
+-rw-r--r--   0 ben       (1001) ben       (1001)     3218 2023-11-15 17:11:42.000000 synapse_super_invites-0.8.2/synapse_super_invites/migration/versions/25e4ec3cea32_added_token_table.py
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites/model/
+-rw-r--r--   0 ben       (1001) ben       (1001)     2275 2023-11-15 17:11:42.000000 synapse_super_invites-0.8.2/synapse_super_invites/model/__init__.py
+-rw-r--r--   0 ben       (1001) ben       (1001)        0 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.2/synapse_super_invites/py.typed
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites/resource/
+-rw-r--r--   0 ben       (1001) ben       (1001)      238 2024-05-11 20:20:17.000000 synapse_super_invites-0.8.2/synapse_super_invites/resource/__init__.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     1227 2024-05-11 20:21:11.000000 synapse_super_invites-0.8.2/synapse_super_invites/resource/base.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     1998 2024-05-11 19:52:25.000000 synapse_super_invites-0.8.2/synapse_super_invites/resource/info.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     2475 2024-05-11 19:52:03.000000 synapse_super_invites-0.8.2/synapse_super_invites/resource/redeem.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     4790 2024-05-11 20:20:17.000000 synapse_super_invites-0.8.2/synapse_super_invites/resource/tokens.py
+-rw-r--r--   0 ben       (1001) ben       (1001)     2034 2024-05-11 20:20:17.000000 synapse_super_invites-0.8.2/synapse_super_invites/resource/web_access.py
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites/static/
+-rw-r--r--   0 ben       (1001) ben       (1001)      556 2023-11-15 23:09:11.000000 synapse_super_invites-0.8.2/synapse_super_invites/static/index.html
+-rw-r--r--   0 ben       (1001) ben       (1001)    15721 2023-11-15 22:50:38.000000 synapse_super_invites-0.8.2/synapse_super_invites/static/pure-min.css
+-rw-r--r--   0 ben       (1001) ben       (1001)       57 2023-11-15 23:06:08.000000 synapse_super_invites-0.8.2/synapse_super_invites/static/script.js
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/synapse_super_invites.egg-info/
+-rw-r--r--   0 ben       (1001) ben       (1001)     4107 2024-05-11 20:32:12.000000 synapse_super_invites-0.8.2/synapse_super_invites.egg-info/PKG-INFO
+-rw-r--r--   0 ben       (1001) ben       (1001)     1198 2024-05-11 20:32:12.000000 synapse_super_invites-0.8.2/synapse_super_invites.egg-info/SOURCES.txt
+-rw-r--r--   0 ben       (1001) ben       (1001)        1 2024-05-11 20:32:12.000000 synapse_super_invites-0.8.2/synapse_super_invites.egg-info/dependency_links.txt
+-rw-r--r--   0 ben       (1001) ben       (1001)      135 2024-05-11 20:32:12.000000 synapse_super_invites-0.8.2/synapse_super_invites.egg-info/requires.txt
+-rw-r--r--   0 ben       (1001) ben       (1001)       22 2024-05-11 20:32:12.000000 synapse_super_invites-0.8.2/synapse_super_invites.egg-info/top_level.txt
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/tests/
+drwxr-xr-x   0 ben       (1001) ben       (1001)        0 2024-05-11 20:32:12.048764 synapse_super_invites-0.8.2/tests/.local/
+-rw-r--r--   0 ben       (1001) ben       (1001)        0 2023-11-15 22:24:54.000000 synapse_super_invites-0.8.2/tests/.local/.gitkeep
+-rw-r--r--   0 ben       (1001) ben       (1001)     1739 2023-11-14 11:05:58.000000 synapse_super_invites-0.8.2/tests/__init__.py
+-rw-r--r--   0 ben       (1001) ben       (1001)      844 2023-11-15 23:09:33.000000 synapse_super_invites-0.8.2/tests/example_cfg.yml
+-rw-r--r--   0 ben       (1001) ben       (1001)      865 2023-11-17 13:28:20.000000 synapse_super_invites-0.8.2/tests/test_config.py
+-rw-r--r--   0 ben       (1001) ben       (1001)    29983 2024-05-11 20:20:17.000000 synapse_super_invites-0.8.2/tests/test_integrations.py
+-rw-r--r--   0 ben       (1001) ben       (1001)      866 2024-05-11 14:59:11.000000 synapse_super_invites-0.8.2/tox.ini
```

### Comparing `synapse_super_invites-0.8.1/.github/workflows/ci.yml` & `synapse_super_invites-0.8.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/.github/workflows/release.yml` & `synapse_super_invites-0.8.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/.gitlab-ci.yml` & `synapse_super_invites-0.8.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/PKG-INFO` & `synapse_super_invites-0.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: synapse_super_invites
-Version: 0.8.1
+Version: 0.8.2
 Summary: Provides extended support for users to invite other users to rooms via an inventation token
+Project-URL: Homepage, https://www.acter.global/
+Project-URL: Repository, https://github.com/acterglobal/synapse-super-invites/
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matrix-synapse
 Requires-Dist: sqlalchemy
 Requires-Dist: alembic
 Requires-Dist: attrs
@@ -71,14 +73,22 @@
 
 You can confirm the installation went well by trying to access the path `/_synapse/client/super_invites/tokens` on your matrix server. If the module is available this will return with a `401` with `errCode: M_MISSING_TOKEN`. If it isn't available you will get a `404` with `"errcode: "M_UNRECOGNIZED"`.
 
 ## Usage
 
 ## Changelog
 
+**0.8.2** - 2024-05-11:
+
+- Support for receiving info about a token without redeeming it, #2
+- Fix to mark DMs as direct (includes tests), #7
+- Fix for pyproject URLs, #1, thanks to @HarHarLinks
+- Allow API caller to not disable registration token creation
+- Clean up types
+
 **0.8.1** - 2023-11-24:
 
 - ensure deleted tokens stay unaccessible -- also to the owner
 
 **0.8.0** - 2023-11-24:
 
 - documentation about how to use this with the docker-ansible-scripts
```

### Comparing `synapse_super_invites-0.8.1/README.md` & `synapse_super_invites-0.8.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -50,14 +50,22 @@
 
 You can confirm the installation went well by trying to access the path `/_synapse/client/super_invites/tokens` on your matrix server. If the module is available this will return with a `401` with `errCode: M_MISSING_TOKEN`. If it isn't available you will get a `404` with `"errcode: "M_UNRECOGNIZED"`.
 
 ## Usage
 
 ## Changelog
 
+**0.8.2** - 2024-05-11:
+
+- Support for receiving info about a token without redeeming it, #2
+- Fix to mark DMs as direct (includes tests), #7
+- Fix for pyproject URLs, #1, thanks to @HarHarLinks
+- Allow API caller to not disable registration token creation
+- Clean up types
+
 **0.8.1** - 2023-11-24:
 
 - ensure deleted tokens stay unaccessible -- also to the owner
 
 **0.8.0** - 2023-11-24:
 
 - documentation about how to use this with the docker-ansible-scripts
```

### Comparing `synapse_super_invites-0.8.1/alembic.ini` & `synapse_super_invites-0.8.2/alembic.ini`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/pyproject.toml` & `synapse_super_invites-0.8.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -31,14 +31,18 @@
   "black == 23.10.0",
   "ruff == 0.1.1",
   # for publishing
   "build",
   "twine"
 ]
 
+[project.urls]
+Homepage = "https://www.acter.global/"
+Repository = "https://github.com/acterglobal/synapse-super-invites/"
+
 [build-system]
 requires = [
   "setuptools",
   "wheel",
   "setuptools_scm",
 ]
 build-backend = "setuptools.build_meta"
@@ -48,14 +52,18 @@
 
 [tool.setuptools.dynamic]
 version = {attr = "synapse_super_invites.__version__"}
 
 [tool.mypy]
 strict = true
 
+[[tool.mypy.overrides]]
+module = "tests.*"
+disable_error_code = ["attr-defined", "index", "union-attr"]
+
 [tool.ruff]
 line-length = 88
 
 # See https://docs.astral.sh/ruff/rules/#error-e
 # for error codes. The ones we ignore are:
 #  E501: Line too long (black enforces this for us)
 #  E731: do not assign a lambda expression, use a def
```

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites/__init__.py` & `synapse_super_invites-0.8.2/synapse_super_invites/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,22 @@
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 from synapse.config import ConfigError
 from synapse.module_api import ModuleApi
 from twisted.web.static import File
 
 from .config import SynapseSuperInvitesConfig, run_alembic
-from .resource import RedeemResource, TokensResource, WebAccessResource
+from .resource import (
+    RedeemResource,
+    TokenInfoResource,
+    TokensResource,
+    WebAccessResource,
+)
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 PKG_DIR = os.path.dirname(os.path.realpath(__file__))
 
 
 class SynapseSuperInvites:
     def __init__(self, config: SynapseSuperInvitesConfig, api: ModuleApi):
         # Keep a reference to the config and Module API
@@ -23,14 +28,18 @@
         self._sessions = sessionmaker(engine)
         self._api = api
         self._config = config
         self.setup()
 
     def setup(self) -> None:
         self._api.register_web_resource(
+            "/_synapse/client/super_invites/info",
+            TokenInfoResource(self._config, self._api, self._sessions),
+        )
+        self._api.register_web_resource(
             "/_synapse/client/super_invites/tokens",
             TokensResource(self._config, self._api, self._sessions),
         )
         self._api.register_web_resource(
             "/_synapse/client/super_invites/redeem",
             RedeemResource(self._config, self._api, self._sessions),
         )
```

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites/alembic.ini` & `synapse_super_invites-0.8.2/synapse_super_invites/alembic.ini`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites/config.py` & `synapse_super_invites-0.8.2/synapse_super_invites/config.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites/migration/env.py` & `synapse_super_invites-0.8.2/synapse_super_invites/migration/env.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites/migration/script.py.mako` & `synapse_super_invites-0.8.2/synapse_super_invites/migration/script.py.mako`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites/migration/versions/25e4ec3cea32_added_token_table.py` & `synapse_super_invites-0.8.2/synapse_super_invites/migration/versions/25e4ec3cea32_added_token_table.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites/model/__init__.py` & `synapse_super_invites-0.8.2/synapse_super_invites/model/__init__.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites/resource/redeem.py` & `synapse_super_invites-0.8.2/synapse_super_invites/resource/redeem.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,20 @@
                     room_id=room.nameOrAlias,
                     new_membership="join",
                 )
                 invited_rooms.append(room.nameOrAlias)
 
             if token.create_dm:
                 dm_data = await self.api.create_room(
-                    my_id, config={"preset": "trusted_private_chat", "invite": [owner]}
+                    my_id,
+                    config={
+                        "preset": "trusted_private_chat",
+                        "invite": [owner],
+                        "is_direct": True,
+                    },
                 )
                 invited_rooms.append(dm_data[0])
 
             # keep the accepted record
             session.add(Accepted(token=token, user=my_id))
             session.flush()
```

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites/resource/tokens.py` & `synapse_super_invites-0.8.2/synapse_super_invites/resource/tokens.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any
+
 from sqlalchemy import func, select
 from synapse.http.servlet import parse_json_object_from_request, parse_string
 from synapse.http.site import SynapseRequest
 from synapse.types import JsonDict, Tuple  # type: ignore[attr-defined]
 
 from synapse_super_invites.model import Room, Token
 
@@ -59,14 +61,15 @@
         return 200, {"tokens": tokens}
 
     async def _async_render_POST(self, request: SynapseRequest) -> Tuple[int, JsonDict]:
         requester = await self.api.get_user_by_req(request, allow_guest=False)
         payload = parse_json_object_from_request(request)
         token_id = payload.get("token", None)
         create_dm = payload.get("create_dm", False)
+        as_registration_token = payload.get("as_registration_token", True)
 
         token_data = None
         with self.db.begin() as session:
             rooms = [
                 session.merge(Room(nameOrAlias=key)) for key in payload.get("rooms", [])
             ]
 
@@ -92,16 +95,27 @@
                 )
                 session.add(token)
 
             session.flush()
 
             token_data = serialize_token(token)
 
-        if self.config.generate_registration_token:
-            token_id = token_data["token"]
-            # FIXME: it'd be great if we didn't have to resort to using internal args...
-            if not (await self.api._store.registration_token_is_valid(token_id)):
-                await self.api._store.create_registration_token(
-                    token=token_id, uses_allowed=None, expiry_time=None
-                )
+        registration_token: dict[Any, Any] = {}
+        if as_registration_token:
+            if not self.config.generate_registration_token:
+                registration_token["valid"] = False
+                registration_token["reason"] = "NOT_ENABLED"
+            else:
+                token_id = token_data["token"]
+                # FIXME: it'd be great if we didn't have to resort to using internal args...
+                if not (await self.api._store.registration_token_is_valid(token_id)):
+                    await self.api._store.create_registration_token(
+                        token=token_id, uses_allowed=None, expiry_time=None
+                    )
+                    registration_token["valid"] = True
+                else:
+                    registration_token["valid"] = True
+        else:
+            registration_token["valid"] = False
+            registration_token["reason"] = "NOT_REQUESTED"
 
-        return 200, {"token": token_data}
+        return 200, {"token": token_data, "registration_token": registration_token}
```

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites/resource/web_access.py` & `synapse_super_invites-0.8.2/synapse_super_invites/resource/web_access.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     DirectServeHtmlResource,
     finish_request,
     logger,
     set_clickjacking_protection_headers,
 )
 from synapse.http.site import SynapseRequest
 from synapse.module_api import ModuleApi
-from synapse.types import Any, JsonDict, Tuple  # type: ignore[attr-defined]
+from synapse.types import Any, Tuple  # type: ignore[attr-defined]
 
 
 class WebAccessResource(DirectServeHtmlResource):
     def __init__(
         self,
         api: ModuleApi,
     ):
@@ -25,32 +25,32 @@
     ) -> None:
         """Implements _AsyncResource._send_response"""
         # We expect to get bytes for us to write
         assert isinstance(response_object, bytes)
         js_bytes = response_object
 
         # The response code must always be set, for logging purposes.
-        request.setResponseCode(code)
+        request.setResponseCode(code)  # type: ignore[no-untyped-call]
 
         # could alternatively use request.notifyFinish() and flip a flag when
         # the Deferred fires, but since the flag is RIGHT THERE it seems like
         # a waste.
         if request._disconnected:
             logger.warning(
                 "Not sending response to request %s, already disconnected.", request
             )
             return None
 
-        request.setHeader(b"Content-Type", b"text/javascript; charset=utf-8")
-        request.setHeader(b"Content-Length", b"%d" % (len(js_bytes),))
+        request.setHeader(b"Content-Type", b"text/javascript; charset=utf-8")  # type: ignore[no-untyped-call]
+        request.setHeader(b"Content-Length", b"%d" % (len(js_bytes),))  # type: ignore[no-untyped-call]
 
         # Ensure this content cannot be embedded.
         set_clickjacking_protection_headers(request)
 
-        request.write(js_bytes)
+        request.write(js_bytes)  # type: ignore[no-untyped-call]
         finish_request(request)
 
-    async def _async_render_GET(self, request: SynapseRequest) -> Tuple[int, JsonDict]:
+    async def _async_render_GET(self, request: SynapseRequest) -> Tuple[int, str]:
         # ensure logged int
         _requester = await self.api.get_user_by_req(request, allow_guest=False)
-        access_token = await self.api._auth.get_access_token_from_request(request)
+        access_token = self.api._auth.get_access_token_from_request(request)
         return 200, 'startApp("{t}")'.format(t=access_token)
```

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites/static/index.html` & `synapse_super_invites-0.8.2/synapse_super_invites/static/index.html`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites/static/pure-min.css` & `synapse_super_invites-0.8.2/synapse_super_invites/static/pure-min.css`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites.egg-info/PKG-INFO` & `synapse_super_invites-0.8.2/synapse_super_invites.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
-Name: synapse-super-invites
-Version: 0.8.1
+Name: synapse_super_invites
+Version: 0.8.2
 Summary: Provides extended support for users to invite other users to rooms via an inventation token
+Project-URL: Homepage, https://www.acter.global/
+Project-URL: Repository, https://github.com/acterglobal/synapse-super-invites/
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matrix-synapse
 Requires-Dist: sqlalchemy
 Requires-Dist: alembic
 Requires-Dist: attrs
@@ -71,14 +73,22 @@
 
 You can confirm the installation went well by trying to access the path `/_synapse/client/super_invites/tokens` on your matrix server. If the module is available this will return with a `401` with `errCode: M_MISSING_TOKEN`. If it isn't available you will get a `404` with `"errcode: "M_UNRECOGNIZED"`.
 
 ## Usage
 
 ## Changelog
 
+**0.8.2** - 2024-05-11:
+
+- Support for receiving info about a token without redeeming it, #2
+- Fix to mark DMs as direct (includes tests), #7
+- Fix for pyproject URLs, #1, thanks to @HarHarLinks
+- Allow API caller to not disable registration token creation
+- Clean up types
+
 **0.8.1** - 2023-11-24:
 
 - ensure deleted tokens stay unaccessible -- also to the owner
 
 **0.8.0** - 2023-11-24:
 
 - documentation about how to use this with the docker-ansible-scripts
```

### Comparing `synapse_super_invites-0.8.1/synapse_super_invites.egg-info/SOURCES.txt` & `synapse_super_invites-0.8.2/synapse_super_invites.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 synapse_super_invites.egg-info/top_level.txt
 synapse_super_invites/migration/env.py
 synapse_super_invites/migration/script.py.mako
 synapse_super_invites/migration/versions/25e4ec3cea32_added_token_table.py
 synapse_super_invites/model/__init__.py
 synapse_super_invites/resource/__init__.py
 synapse_super_invites/resource/base.py
+synapse_super_invites/resource/info.py
 synapse_super_invites/resource/redeem.py
 synapse_super_invites/resource/tokens.py
 synapse_super_invites/resource/web_access.py
 synapse_super_invites/static/index.html
 synapse_super_invites/static/pure-min.css
 synapse_super_invites/static/script.js
 tests/__init__.py
```

### Comparing `synapse_super_invites-0.8.1/tests/__init__.py` & `synapse_super_invites-0.8.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/tests/example_cfg.yml` & `synapse_super_invites-0.8.2/tests/example_cfg.yml`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/tests/test_config.py` & `synapse_super_invites-0.8.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `synapse_super_invites-0.8.1/tests/test_integrations.py` & `synapse_super_invites-0.8.2/tests/test_integrations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any
+
 from matrix_synapse_testutils.unittest import (  # type: ignore[import-untyped]
     HomeserverTestCase,
     override_config,
 )
 from synapse.rest import admin
 from synapse.rest.client import login, profile, register, room, sync
 from synapse.server import HomeServer
@@ -49,14 +51,37 @@
     # create a room with the given access_token, return the roomId
     def create_room(self, user_id: str) -> str:
         room_id: str = self.get_success(
             self.module_api.create_room(user_id=user_id, config={}, ratelimit=False)
         )[0]
         return room_id
 
+    # create a room with the given access_token, return the roomId
+    def create_public_room(self, user_id: str) -> str:
+        room_id: str = self.get_success(
+            self.module_api.create_room(
+                user_id=user_id,
+                config={"preset": "public_chat", "visibility": "public"},
+                ratelimit=False,
+            )
+        )[0]
+        return room_id
+
+    def getState(
+        self, room_data: dict[Any, Any], type_key: str, state_key: str | None
+    ) -> Any | None:
+        for e in reversed(room_data.get("timeline", {}).get("events", [])):
+            if e.get("type") == type_key:
+                if state_key is not None:
+                    if e.get("state_key") == state_key:
+                        return e.get("content")
+                else:
+                    return e.get("content")
+        return None
+
 
 class SimpleInviteTests(SuperInviteHomeserverTestCase):
     @override_config(DEFAULT_CONFIG)  # type: ignore[misc]
     def test_edit_invite_token_rooms(self) -> None:
         m_id = self.register_user("meeko", "password")
         m_access_token = self.login("meeko", "password")
 
@@ -152,14 +177,28 @@
 
         # redeem the new token
 
         _f_id = self.register_user("flit", "flit")
         f_access_token = self.login("flit", "flit")
 
         channel = self.make_request(
+            "GET",
+            "/_synapse/client/super_invites/info?token={token}".format(token=token),
+            access_token=f_access_token,
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        # list the rooms we were invited to
+
+        self.assertEqual(channel.json_body["rooms_count"], 3)
+        self.assertEqual(channel.json_body["create_dm"], False)
+        self.assertEqual(channel.json_body["has_redeemed"], False)
+        self.assertEqual(channel.json_body["inviter"]["user_id"], "@meeko:test")
+        self.assertEqual(channel.json_body["inviter"]["display_name"], "meeko")
+
+        channel = self.make_request(
             "POST",
             "/_synapse/client/super_invites/redeem?token={token}".format(token=token),
             access_token=f_access_token,
         )
         self.assertEqual(channel.code, 200, msg=channel.result)
         # list the rooms we were invited to
         self.assertCountEqual(channel.json_body["rooms"], rooms_to_invite)
@@ -170,24 +209,108 @@
             "/_synapse/client/super_invites/tokens?token={token}".format(token=token),
             access_token=m_access_token,
         )
         self.assertEqual(channel.code, 200, msg=channel.result)
         token_data = channel.json_body["token"]
         self.assertEquals(token_data["accepted_count"], 1)
 
+        channel = self.make_request(
+            "GET",
+            "/_synapse/client/super_invites/info?token={token}".format(token=token),
+            access_token=f_access_token,
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        self.assertEqual(channel.json_body["has_redeemed"], True)
+
         # and flit was invited to these, too:
         channel = self.make_request(
             "GET", "/_matrix/client/v3/sync", access_token=f_access_token
         )
         self.assertEqual(channel.code, 200, msg=channel.result)
         self.assertEqual(channel.json_body["rooms"].get("invite"), None)
         self.assertCountEqual(
             channel.json_body["rooms"]["join"].keys(), rooms_to_invite
         )
 
+    @override_config(DEFAULT_CONFIG)  # type: ignore[misc]
+    def test_simple_can_join_public_room_test(self) -> None:
+        m_id = self.register_user("meeko", "password")
+        m_access_token = self.login("meeko", "password")
+
+        # this is our new backend.
+        channel = self.make_request(
+            "GET", "/_synapse/client/super_invites/tokens", access_token=m_access_token
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        self.assertEqual(channel.json_body["tokens"], [])
+
+        # creating five channel
+        _roomA = self.create_room(m_id)
+        roomB = self.create_public_room(m_id)  # this is public
+        roomC = self.create_room(m_id)
+        roomD = self.create_room(m_id)
+        _roomE = self.create_room(m_id)
+
+        rooms_to_invite = [
+            roomB,
+            roomC,
+            roomD,
+        ]
+        # create a new one for testing.
+        channel = self.make_request(
+            "POST",
+            "/_synapse/client/super_invites/tokens",
+            access_token=m_access_token,
+            content={"rooms": rooms_to_invite},
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        token_data = channel.json_body["token"]
+        self.assertCountEqual(token_data["rooms"], rooms_to_invite)
+        self.assertEquals(token_data["accepted_count"], 0)
+        self.assertFalse(token_data["create_dm"])
+        token = token_data["token"]
+
+        # redeem the new token
+
+        _f_id = self.register_user("flit", "flit")
+        f_access_token = self.login("flit", "flit")
+
+        channel = self.make_request(
+            "POST",
+            "/_synapse/client/super_invites/redeem?token={token}".format(token=token),
+            access_token=f_access_token,
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        # list the rooms we were invited to
+        self.assertCountEqual(channel.json_body["rooms"], rooms_to_invite)
+
+        # we see it has been redeemed
+        channel = self.make_request(
+            "GET",
+            "/_synapse/client/super_invites/tokens?token={token}".format(token=token),
+            access_token=m_access_token,
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        token_data = channel.json_body["token"]
+        self.assertEquals(token_data["accepted_count"], 1)
+
+        # and flit was invited to these, too:
+        channel = self.make_request(
+            "GET", "/_matrix/client/v3/sync", access_token=f_access_token
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        self.assertEqual(channel.json_body["rooms"].get("invite"), None)
+        self.assertCountEqual(
+            channel.json_body["rooms"]["join"].keys(), rooms_to_invite
+        )
+        # ensure the dm matches what we are expecting
+        public_room = channel.json_body["rooms"]["join"][roomB]
+        join_rule = self.getState(public_room, "m.room.join_rules", None)
+        self.assertEquals(join_rule["join_rule"], "public", join_rule)
+
     @override_config(
         {
             "enable_registration": True,
             "registration_requires_token": True,
             "modules": [
                 {
                     "module": "synapse_super_invites.SynapseSuperInvites",
@@ -215,25 +338,99 @@
             "POST",
             "/_synapse/client/super_invites/tokens",
             {"rooms": []},
             access_token=m_access_token,
         )
         self.assertEqual(channel.code, 200, msg=channel.result)
         token = channel.json_body["token"]
+        registration_token = channel.json_body["registration_token"]
+        self.assertTrue(registration_token["valid"])
 
         # let's see if the token exists and is valid
         channel = self.make_request(
             "GET",
             "/_matrix/client/v1/register/m.login.registration_token/validity?token={token}".format(
                 token=token["token"]
             ),
         )
         self.assertEqual(channel.code, 200, msg=channel.result)
         self.assertTrue(channel.json_body["valid"])
 
+        # create a new token for testing, no registration
+        channel = self.make_request(
+            "POST",
+            "/_synapse/client/super_invites/tokens",
+            {"rooms": [], "as_registration_token": False},
+            access_token=m_access_token,
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        token = channel.json_body["token"]
+        registration_token = channel.json_body["registration_token"]
+        self.assertFalse(registration_token["valid"])
+        self.assertEquals(registration_token["reason"], "NOT_REQUESTED")
+
+        # let's see if the token exists and is valid
+        channel = self.make_request(
+            "GET",
+            "/_matrix/client/v1/register/m.login.registration_token/validity?token={token}".format(
+                token=token["token"]
+            ),
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        self.assertFalse(channel.json_body["valid"])
+
+    @override_config(
+        {
+            "enable_registration": True,
+            "registration_requires_token": True,
+            "modules": [
+                {
+                    "module": "synapse_super_invites.SynapseSuperInvites",
+                    "config": {
+                        "sql_url": "sqlite:///",
+                        "generate_registration_token": False,
+                    },
+                }
+            ],
+        }
+    )  # type: ignore[misc]
+    def test_simple_invite_as_registration_token_not_available_test(self) -> None:
+        _m_id = self.register_user("meeko", "password")
+        m_access_token = self.login("meeko", "password")
+
+        # this is our new backend.
+        channel = self.make_request(
+            "GET", "/_synapse/client/super_invites/tokens", access_token=m_access_token
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        self.assertEqual(channel.json_body["tokens"], [])
+
+        # create a new token for testing.
+        channel = self.make_request(
+            "POST",
+            "/_synapse/client/super_invites/tokens",
+            {"rooms": [], "as_registration_token": True},
+            access_token=m_access_token,
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        token = channel.json_body["token"]
+        registration_token = channel.json_body["registration_token"]
+        self.assertFalse(registration_token["valid"])
+        self.assertEquals(registration_token["reason"], "NOT_ENABLED")
+
+        # let's see if the token exists and is valid
+        channel = self.make_request(
+            "GET",
+            "/_matrix/client/v1/register/m.login.registration_token/validity?token={token}".format(
+                token=token["token"]
+            ),
+        )
+        self.assertEqual(channel.code, 200, msg=channel.result)
+        self.assertFalse(channel.json_body["valid"])
+
     @override_config(DEFAULT_CONFIG)  # type: ignore[misc]
     def test_simple_invite_token_only_dm_test(self) -> None:
         _m_id = self.register_user("meeko", "password")
         m_access_token = self.login("meeko", "password")
 
         # this is our new backend.
         channel = self.make_request(
@@ -293,14 +490,25 @@
             "GET", "/_matrix/client/v3/sync", access_token=f_access_token
         )
         self.assertEqual(channel.code, 200, msg=channel.result)
         # we are the author of the DM, so we aren't invited, but just added
         self.assertEqual(channel.json_body["rooms"].get("invite"), None)
         self.assertCountEqual(channel.json_body["rooms"]["join"].keys(), [new_dm])
 
+        # ensure the dm matches what we are expecting
+        dm = channel.json_body["rooms"]["join"][new_dm]
+        join_rule = self.getState(dm, "m.room.join_rules", None)
+        self.assertEquals(join_rule["join_rule"], "invite", join_rule)
+
+        # and the other has been invited, too
+        member = self.getState(dm, "m.room.member", "@meeko:test")
+        self.assertEquals(member.get("membership"), "invite", member)
+        # to the DM
+        self.assertEquals(member.get("is_direct"), True, member)
+
     @override_config(DEFAULT_CONFIG)  # type: ignore[misc]
     def test_simple_invite_token_with_dm_test(self) -> None:
         m_id = self.register_user("meeko", "password")
         m_access_token = self.login("meeko", "password")
 
         # this is our new backend.
         channel = self.make_request(
@@ -497,97 +705,34 @@
         # and it doesn't show up in the user listing
         channel = self.make_request(
             "GET", "/_synapse/client/super_invites/tokens", access_token=m_access_token
         )
         self.assertEqual(channel.code, 200, msg=channel.result)
         self.assertEqual(channel.json_body["tokens"], [])
 
-        # redeem the new token
+        # trying to redeem token
         _f_id = self.register_user("flit", "flit")
         f_access_token = self.login("flit", "flit")
 
-        # and it can't be redeemed
+        # and it can't be found
         channel = self.make_request(
-            "POST",
-            "/_synapse/client/super_invites/redeem?token={token}".format(token=token),
+            "GET",
+            "/_synapse/client/super_invites/info?token={token}".format(token=token),
             access_token=f_access_token,
         )
-        self.assertEqual(channel.code, 404, msg=channel.result)
-
-    @override_config(DEFAULT_CONFIG)  # type: ignore[misc]
-    def test_deletion_cant_create_again(self) -> None:
-        _m_id = self.register_user("meeko", "password")
-        m_access_token = self.login("meeko", "password")
+        self.assertEqual(channel.code, 403, msg=channel.result)  # access denied
 
-        # this is our new backend.
-        channel = self.make_request(
-            "GET", "/_synapse/client/super_invites/tokens", access_token=m_access_token
-        )
-        self.assertEqual(channel.code, 200, msg=channel.result)
-        self.assertEqual(channel.json_body["tokens"], [])
-
-        # create a new one for testing.
+        # and it can't be redeemed
         channel = self.make_request(
             "POST",
-            "/_synapse/client/super_invites/tokens",
-            access_token=m_access_token,
-            content={"rooms": [], "create_dm": True},
-        )
-        self.assertEqual(channel.code, 200, msg=channel.result)
-        token_data = channel.json_body["token"]
-        self.assertEquals(token_data["accepted_count"], 0)
-        self.assertTrue(token_data["create_dm"])
-        token = token_data["token"]
-
-        channel = self.make_request(
-            "GET", "/_synapse/client/super_invites/tokens", access_token=m_access_token
-        )
-        self.assertEqual(channel.code, 200, msg=channel.result)
-        self.assertEqual(len(channel.json_body["tokens"]), 1)
-
-        # we can access it
-        channel = self.make_request(
-            "GET",
-            "/_synapse/client/super_invites/tokens?token={token}".format(token=token),
-            access_token=m_access_token,
-        )
-        self.assertEqual(channel.code, 200, msg=channel.result)
-
-        # delete it
-        channel = self.make_request(
-            "DELETE",
-            "/_synapse/client/super_invites/tokens?token={token}".format(token=token),
-            access_token=m_access_token,
-        )
-        self.assertEqual(channel.code, 200, msg=channel.result)
-
-        # we can't access it
-        channel = self.make_request(
-            "GET",
-            "/_synapse/client/super_invites/tokens?token={token}".format(token=token),
-            access_token=m_access_token,
+            "/_synapse/client/super_invites/redeem?token={token}".format(token=token),
+            access_token=f_access_token,
         )
         self.assertEqual(channel.code, 404, msg=channel.result)
 
-        # and it doesn't show up in the user listing
-        channel = self.make_request(
-            "GET", "/_synapse/client/super_invites/tokens", access_token=m_access_token
-        )
-        self.assertEqual(channel.code, 200, msg=channel.result)
-        self.assertEqual(channel.json_body["tokens"], [])
-
-        # and creating it again fails
-        channel = self.make_request(
-            "POST",
-            "/_synapse/client/super_invites/tokens",
-            access_token=m_access_token,
-            content={"rooms": [], "create_dm": True, "token": token},
-        )
-        self.assertEqual(channel.code, 403, msg=channel.result)
-
     @override_config(DEFAULT_CONFIG)  # type: ignore[misc]
     def test_cant_redeem_my_own(self) -> None:
         _m_id = self.register_user("meeko", "password")
         m_access_token = self.login("meeko", "password")
 
         # this is our new backend.
         channel = self.make_request(
```

### Comparing `synapse_super_invites-0.8.1/tox.ini` & `synapse_super_invites-0.8.2/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -46,12 +46,12 @@
 [testenv:publish]
 
 extras = dev
 
 allowlist_externals = rm
 
 commands =
-  rm -rf dist
+  rm -rf dist/*
   python -m build --sdist
   python -m build --wheel
   twine check dist/*
   twine upload dist/*
```

