# Comparing `tmp/singularity-compose-0.1.18.tar.gz` & `tmp/singularity-compose-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singularity-compose-0.1.18.tar", last modified: Thu Jul 28 18:15:17 2022, max compression
+gzip compressed data, was "singularity-compose-0.1.19.tar", last modified: Sat May 11 19:07:32 2024, max compression
```

## Comparing `singularity-compose-0.1.18.tar` & `singularity-compose-0.1.19.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.527624 singularity-compose-0.1.18/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    15830 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      164 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1732 2022-07-28 18:15:17.527624 singularity-compose-0.1.18/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      758 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.523625 singularity-compose-0.1.18/scompose/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      277 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.523625 singularity-compose-0.1.18/scompose/client/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7817 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/client/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      771 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/client/build.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      926 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/client/check.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      698 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/client/config.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      853 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/client/create.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      594 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/client/down.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      535 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/client/exec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      605 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/client/logs.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      568 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/client/ps.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      922 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/client/restart.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      524 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/client/run.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      582 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/client/shell.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      833 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/client/up.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.523625 singularity-compose-0.1.18/scompose/config/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1806 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/config/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3084 2022-07-28 18:13:40.000000 singularity-compose-0.1.18/scompose/config/schema.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.523625 singularity-compose-0.1.18/scompose/logger/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       59 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/logger/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9486 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/logger/message.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4454 2022-07-28 18:13:40.000000 singularity-compose-0.1.18/scompose/logger/progress.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.527624 singularity-compose-0.1.18/scompose/project/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       29 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/project/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    22121 2022-07-28 18:13:40.000000 singularity-compose-0.1.18/scompose/project/instance.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    18158 2022-07-28 18:13:40.000000 singularity-compose-0.1.18/scompose/project/project.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.527624 singularity-compose-0.1.18/scompose/templates/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      638 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/templates/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      204 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/templates/hosts
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      240 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/templates/resolv.conf
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.527624 singularity-compose-0.1.18/scompose/tests/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.523625 singularity-compose-0.1.18/scompose/tests/configs/
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.527624 singularity-compose-0.1.18/scompose/tests/configs/cmd_args/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       77 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/configs/cmd_args/Singularity
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      128 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/configs/cmd_args/singularity-compose.yml
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.527624 singularity-compose-0.1.18/scompose/tests/configs/config_merge/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      128 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/configs/config_merge/singularity-compose-1.yml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      186 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/configs/config_merge/singularity-compose-2.yml
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.527624 singularity-compose-0.1.18/scompose/tests/configs/depends_on/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      112 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/configs/depends_on/Singularity.first
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      113 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/configs/depends_on/Singularity.second
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      112 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/configs/depends_on/Singularity.third
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      284 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/configs/depends_on/singularity-compose.yml
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.527624 singularity-compose-0.1.18/scompose/tests/configs/wrong_depends_on/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      112 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/configs/wrong_depends_on/Singularity.first
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      113 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/configs/wrong_depends_on/Singularity.second
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      112 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/configs/wrong_depends_on/Singularity.third
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      286 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/configs/wrong_depends_on/singularity-compose.yml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1875 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/test_client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1467 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/test_command_args.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3300 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/test_config.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2820 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/test_depends_on.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2542 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/tests/test_utils.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.527624 singularity-compose-0.1.18/scompose/utils/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5043 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/scompose/utils/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      958 2022-07-28 18:15:11.000000 singularity-compose-0.1.18/scompose/version.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       38 2022-07-28 18:15:17.527624 singularity-compose-0.1.18/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3844 2022-07-27 20:09:41.000000 singularity-compose-0.1.18/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-07-28 18:15:17.527624 singularity-compose-0.1.18/singularity_compose.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1732 2022-07-28 18:15:16.000000 singularity-compose-0.1.18/singularity_compose.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1903 2022-07-28 18:15:17.000000 singularity-compose-0.1.18/singularity_compose.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2022-07-28 18:15:17.000000 singularity-compose-0.1.18/singularity_compose.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2022-07-28 18:15:17.000000 singularity-compose-0.1.18/singularity_compose.egg-info/entry_points.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2022-07-27 20:13:26.000000 singularity-compose-0.1.18/singularity_compose.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      115 2022-07-28 18:15:17.000000 singularity-compose-0.1.18/singularity_compose.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        9 2022-07-28 18:15:17.000000 singularity-compose-0.1.18/singularity_compose.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    15830 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      164 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1711 2024-05-11 19:07:32.492061 singularity-compose-0.1.19/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      757 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/pyproject.toml
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/scompose/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       33 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/scompose/client/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7802 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/client/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      771 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/client/build.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      927 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/client/check.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      698 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/client/config.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      853 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/client/create.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      594 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/client/down.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      535 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/client/exec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      605 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/client/logs.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      568 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/client/ps.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      922 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/client/restart.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      524 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/client/run.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      582 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/client/shell.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      833 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/client/up.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/scompose/config/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1816 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/config/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3074 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/config/schema.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/scompose/logger/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       59 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/logger/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9486 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/logger/message.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4454 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/logger/progress.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/scompose/project/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       29 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/project/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    22389 2024-05-11 19:07:14.000000 singularity-compose-0.1.19/scompose/project/instance.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    18183 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/project/project.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/scompose/templates/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      638 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/templates/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      204 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/templates/hosts
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      239 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/templates/resolv.conf
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/scompose/tests/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/tests/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/scompose/tests/configs/
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/scompose/tests/configs/cmd_args/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       77 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/tests/configs/cmd_args/Singularity
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      128 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/tests/configs/cmd_args/singularity-compose.yml
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/scompose/tests/configs/config_merge/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      128 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/tests/configs/config_merge/singularity-compose-1.yml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      186 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/tests/configs/config_merge/singularity-compose-2.yml
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/scompose/tests/configs/depends_on/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      112 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/tests/configs/depends_on/Singularity.first
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      113 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/tests/configs/depends_on/Singularity.second
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      112 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/tests/configs/depends_on/Singularity.third
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      284 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/tests/configs/depends_on/singularity-compose.yml
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/scompose/tests/configs/wrong_depends_on/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      112 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/tests/configs/wrong_depends_on/Singularity.first
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      113 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/tests/configs/wrong_depends_on/Singularity.second
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      112 2024-03-28 17:01:42.000000 singularity-compose-0.1.19/scompose/tests/configs/wrong_depends_on/Singularity.third
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      285 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/tests/configs/wrong_depends_on/singularity-compose.yml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1862 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/tests/test_client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1415 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/tests/test_command_args.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3300 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/tests/test_config.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2767 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/tests/test_depends_on.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2544 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/tests/test_utils.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/scompose/utils/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5043 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/scompose/utils/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      958 2024-05-11 19:07:14.000000 singularity-compose-0.1.19/scompose/version.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      334 2024-05-11 19:07:32.492061 singularity-compose-0.1.19/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3830 2024-05-10 18:05:35.000000 singularity-compose-0.1.19/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2024-05-11 19:07:32.488060 singularity-compose-0.1.19/singularity_compose.egg-info/
+-rw-r--r--   0 vanessa   (1000) vanessa   (1000)     1711 2024-05-11 19:07:32.000000 singularity-compose-0.1.19/singularity_compose.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1928 2024-05-11 19:07:32.000000 singularity-compose-0.1.19/singularity_compose.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2024-05-11 19:07:32.000000 singularity-compose-0.1.19/singularity_compose.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2024-05-11 19:07:32.000000 singularity-compose-0.1.19/singularity_compose.egg-info/entry_points.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2024-03-28 17:06:16.000000 singularity-compose-0.1.19/singularity_compose.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      115 2024-05-11 19:07:32.000000 singularity-compose-0.1.19/singularity_compose.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        9 2024-05-11 19:07:32.000000 singularity-compose-0.1.19/singularity_compose.egg-info/top_level.txt
```

### Comparing `singularity-compose-0.1.18/LICENSE` & `singularity-compose-0.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `singularity-compose-0.1.18/PKG-INFO` & `singularity-compose-0.1.19/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: singularity-compose
-Version: 0.1.18
+Version: 0.1.19
 Summary: simple orchestration for singularity containers
 Home-page: http://github.com/singularityhub/singularity-compose
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 Maintainer-email: vsoch@users.noreply.github.com
 License: LICENSE
 Keywords: singularity,compose
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -27,17 +26,15 @@
 
 # Singularity Compose
 
 [![status](http://joss.theoj.org/papers/1fc2593b11b5e18df12efb59ed8757a0/status.svg)](http://joss.theoj.org/papers/1fc2593b11b5e18df12efb59ed8757a0)
 [![DOI](https://zenodo.org/badge/188852712.svg)](https://zenodo.org/badge/latestdoi/188852712)
 
 This is a simple orchestration library for Singularity containers, akin to
-Docker Compose. See the [specification](https://singularityhub.github.io/singularity-compose/#/spec/spec-1.0) 
+Docker Compose. See the [specification](https://singularityhub.github.io/singularity-compose/#/spec/spec-1.0)
 and the [documentation](https://singularityhub.github.io/singularity-compose) for
 details, or more examples below.
 
 ## Examples
 
 See our [Singularity Compose Examples](https://www.github.com/singularityhub/singularity-compose-examples) repository for
 finding or contributing examples for using scompose.
-
-
```

### Comparing `singularity-compose-0.1.18/README.md` & `singularity-compose-0.1.19/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Singularity Compose
 
 [![status](http://joss.theoj.org/papers/1fc2593b11b5e18df12efb59ed8757a0/status.svg)](http://joss.theoj.org/papers/1fc2593b11b5e18df12efb59ed8757a0)
 [![DOI](https://zenodo.org/badge/188852712.svg)](https://zenodo.org/badge/latestdoi/188852712)
 
 This is a simple orchestration library for Singularity containers, akin to
-Docker Compose. See the [specification](https://singularityhub.github.io/singularity-compose/#/spec/spec-1.0) 
+Docker Compose. See the [specification](https://singularityhub.github.io/singularity-compose/#/spec/spec-1.0)
 and the [documentation](https://singularityhub.github.io/singularity-compose) for
 details, or more examples below.
 
 ## Examples
 
 See our [Singularity Compose Examples](https://www.github.com/singularityhub/singularity-compose-examples) repository for
 finding or contributing examples for using scompose.
```

### Comparing `singularity-compose-0.1.18/scompose/client/__init__.py` & `singularity-compose-0.1.19/scompose/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python
 
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 """
 
-import scompose
 import argparse
-import sys
 import os
+import sys
+
+import scompose
 
 
 def get_parser():
     description = "Orchestration for Singularity containers"
     parser = argparse.ArgumentParser(description="Singularity Compose")
 
     # Verbosity
@@ -87,15 +88,15 @@
         help="scompose actions",
         title="actions",
         description=description,
         dest="command",
     )
 
     # print version and exit
-    version = subparsers.add_parser("version", help="show software version")
+    subparsers.add_parser("version", help="show software version")
 
     # Build
 
     build = subparsers.add_parser("build", help="Build or rebuild containers")
 
     # Check
 
@@ -108,19 +109,17 @@
         dest="preview",
         help="print compose file(s) interpolated content",
         default=False,
         action="store_true",
     )
 
     # Config
-
-    config = subparsers.add_parser("config", help="Validate and view the compose file")
+    subparsers.add_parser("config", help="Validate and view the compose file")
 
     # Create (assumes built already), Up (will also build, if able)
-
     create = subparsers.add_parser("create", help="create instances")
 
     up = subparsers.add_parser("up", help="build and start containers")
 
     restart = subparsers.add_parser("restart", help="stop and start containers.")
 
     for sub in [create, up, restart]:
@@ -185,15 +184,15 @@
         "--clear",
         dest="clear",
         help="clear existing logs.",
         default=False,
         action="store_true",
     )
 
-    ps = subparsers.add_parser("ps", help="list instances")
+    subparsers.add_parser("ps", help="list instances")
 
     # Add list of names
     for sub in [build, create, down, logs, up, restart, stop]:
         sub.add_argument(
             "names", nargs="*", help="the names of the instances to target"
         )
 
@@ -220,15 +219,15 @@
         sys.exit(return_code)
 
     # If the user didn't provide any arguments, show the full help
     if len(sys.argv) == 1:
         show_help()
     try:
         args, extra = parser.parse_known_args()
-    except:
+    except Exception:
         sys.exit(0)
 
     if args.debug is True:
         os.environ["MESSAGELEVEL"] = "DEBUG"
     else:
         os.environ["MESSAGELEVEL"] = args.log_level
```

### Comparing `singularity-compose-0.1.18/scompose/client/build.py` & `singularity-compose-0.1.19/scompose/client/build.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 """
```

### Comparing `singularity-compose-0.1.18/scompose/client/check.py` & `singularity-compose-0.1.19/scompose/client/check.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 
-Copyright (C) 2021-2022 Vanessa Sochat.
+Copyright (C) 2021-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 
-from scompose.logger import bot
+import yaml
+
 from scompose.config import merge_config
 from scompose.config.schema import validate_config
-import yaml
+from scompose.logger import bot
 
 
 def main(args, parser, extra):
     """
     Validate compose files for correctness.
 
     CLI Arguments
```

### Comparing `singularity-compose-0.1.18/scompose/client/config.py` & `singularity-compose-0.1.19/scompose/client/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 """
```

### Comparing `singularity-compose-0.1.18/scompose/client/create.py` & `singularity-compose-0.1.19/scompose/client/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 """
```

### Comparing `singularity-compose-0.1.18/scompose/client/down.py` & `singularity-compose-0.1.19/scompose/client/down.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 """
```

### Comparing `singularity-compose-0.1.18/scompose/client/exec.py` & `singularity-compose-0.1.19/scompose/client/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 """
```

### Comparing `singularity-compose-0.1.18/scompose/client/logs.py` & `singularity-compose-0.1.19/scompose/client/logs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 """
```

### Comparing `singularity-compose-0.1.18/scompose/client/ps.py` & `singularity-compose-0.1.19/scompose/client/ps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 """
```

### Comparing `singularity-compose-0.1.18/scompose/client/restart.py` & `singularity-compose-0.1.19/scompose/client/up.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-
 """
 
 from scompose.project import Project
 
 
 def main(args, parser, extra):
     """bring up one or more instances. They must exist.
@@ -20,16 +19,13 @@
     """
     # Initialize the project
     project = Project(
         filename=args.file, name=args.project_name, env_file=args.env_file
     )
 
     # Create instances, and if none specified, create all
-    project.down(args.names)
-
-    # Create instances, and if none specified, create all
     project.up(
         args.names,
         writable_tmpfs=not args.read_only,
         bridge=args.bridge,
         no_resolv=args.no_resolv,
     )
```

### Comparing `singularity-compose-0.1.18/scompose/client/run.py` & `singularity-compose-0.1.19/scompose/client/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 """
```

### Comparing `singularity-compose-0.1.18/scompose/client/shell.py` & `singularity-compose-0.1.19/scompose/client/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
```

### Comparing `singularity-compose-0.1.18/scompose/client/up.py` & `singularity-compose-0.1.19/scompose/client/restart.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+
 """
 
 from scompose.project import Project
 
 
 def main(args, parser, extra):
     """bring up one or more instances. They must exist.
@@ -19,13 +20,16 @@
     """
     # Initialize the project
     project = Project(
         filename=args.file, name=args.project_name, env_file=args.env_file
     )
 
     # Create instances, and if none specified, create all
+    project.down(args.names)
+
+    # Create instances, and if none specified, create all
     project.up(
         args.names,
         writable_tmpfs=not args.read_only,
         bridge=args.bridge,
         no_resolv=args.no_resolv,
     )
```

### Comparing `singularity-compose-0.1.18/scompose/config/__init__.py` & `singularity-compose-0.1.19/scompose/config/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 
@@ -23,15 +23,15 @@
         try:
             # ensure file exists
             if not os.path.exists(f):
                 bot.exit("%s does not exist." % f)
 
             # read yaml file
             yaml_files.append(read_yaml(f, quiet=True))
-        except:  # ParserError
+        except Exception:  # ParserError
             bot.exit("Cannot parse %s, invalid yaml." % f)
 
     # merge/override yaml properties where applicable
     return _deep_merge(yaml_files)
 
 
 def _deep_merge(yaml_files):
```

### Comparing `singularity-compose-0.1.18/scompose/config/schema.py` & `singularity-compose-0.1.19/scompose/config/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 
-Copyright (C) 2021-2022 Vanessa Sochat.
+Copyright (C) 2021-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 
-import os
 import sys
 
 from jsonschema.exceptions import ValidationError
 
 from scompose.utils import read_yaml
 
 # We don't require jsonschema, so catch import error and alert user
```

### Comparing `singularity-compose-0.1.18/scompose/logger/message.py` & `singularity-compose-0.1.19/scompose/logger/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2017-2022 Vanessa Sochat.
+# Copyright (C) 2017-2024 Vanessa Sochat.
 
 # This Source Code Form is subject to the terms of the
 # Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 # with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import os
 import sys
```

### Comparing `singularity-compose-0.1.18/scompose/logger/progress.py` & `singularity-compose-0.1.19/scompose/logger/progress.py`

 * *Files identical despite different names*

### Comparing `singularity-compose-0.1.18/scompose/project/instance.py` & `singularity-compose-0.1.19/scompose/project/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 
-from scompose.logger import bot
-from scompose.utils import get_userhome
-from spython.main import get_client
-
-import shlex
 import os
 import platform
 import re
-import time
+import shlex
+
+from spython.main import get_client
+
+from scompose.logger import bot
+from scompose.utils import get_userhome
 
 
 class Instance:
     """
     A section of a singularity-compose.yml, typically includes an image
     name, volumes, build directory, and any ports or environment variables
     relevant to the instance.
@@ -30,15 +30,14 @@
     name: should correspond to the section name for the instance.
     working_dir: should be the projects working directory, where a folder
                  named according to "name" is created for the image binary.
     params: all of the parameters defined in the configuration.
     """
 
     def __init__(self, name, replica_number, working_dir, sudo=False, params=None):
-
         if not params:
             params = {}
 
         self.image = None
         self.recipe = None
         self.instance = None
         self.sudo = sudo
@@ -102,15 +101,14 @@
         including build (context and recipe). We don't pull or create
         anything here, but rather just validate that the sections
         are provided and files exist.
         """
 
         # build the container on the host from a context
         if "build" in params:
-
             if "context" not in params["build"]:
                 bot.exit("build.context section missing for %s" % self.name)
 
             # The user provided a build context
             self.context = params["build"]["context"]
 
             # The context folder must exist
@@ -121,15 +119,14 @@
 
             # The recipe must exist in the context folder
             if not os.path.exists(os.path.join(self.context, self.recipe)):
                 bot.exit("%s does not exist in %s" % (self.recipe, self.context))
 
         # An image can be pulled instead
         elif "image" in params:
-
             # If going to pull an image, the context is a folder of same name
             self.context = self.name
 
             # Image is validated when it needs to be used / pulled
             self.image = params["image"]
 
         # We are required to have build OR image
@@ -170,38 +167,46 @@
         self.network = params.get("network", {})
 
         # if not specified, set the default value for the property
         for key in ["enable", "allocate_ip"]:
             self.network[key] = self.network.get(key, True)
 
     def set_ports(self, params):
-        """set ports from the recipe to be used"""
+        """
+        set ports from the recipe to be used
+        """
         self.ports = params.get("ports", [])
 
     # Commands
 
     def set_start(self, params):
-        """set arguments to the startscript"""
+        """
+        set arguments to the startscript
+        """
         start = params.get("start", {})
         self.args = start.get("args", "")
         self.start_opts = [
             "--%s" % opt if len(opt) > 1 else "-%s" % opt
             for opt in start.get("options", [])
         ]
 
     def set_exec(self, params):
-        """set arguments for exec"""
+        """
+        set arguments for exec
+        """
         exec_group = params.get("exec", {})
         self.exec_args = exec_group.get("command", "")
         if "|" in self.exec_args:
             bot.exit("Pipes are not currently supported.")
         self.exec_opts = self._get_command_opts(exec_group.get("options", []))
 
     def set_run(self, params):
-        """set arguments for run"""
+        """
+        set arguments for run
+        """
         run_group = params.get("run", {}) or {}
         self.run_args = run_group.get("args")
         if self.run_args and "|" in self.run_args:
             bot.exit("Pipes are not currently supported.")
         self.run_opts = self._get_command_opts(run_group.get("options", []))
 
     def _get_command_opts(self, group):
@@ -217,16 +222,21 @@
         ensure they are bound correctly.
         """
         ports = ["--net"]
 
         # Fakeroot means not needing sudo
         fakeroot = "--fakeroot" in self.start_opts or "-f" in self.start_opts
 
+        # Do we have a custom type?
+        network_type = self.network.get("type")
+        if network_type is not None:
+            ports += ["--network", network_type]
+
         # If not sudo or fakeroot, we need --network none
-        if not self.sudo and not fakeroot:
+        elif not self.sudo and not fakeroot:
             ports += ["--network", "none"]
 
         for pair in self.ports:
             ports += ["--network-args", '"portmap=%s/tcp"' % pair]
 
         # Ask for a custom ip address
         if ip_address is not None and self.network["allocate_ip"]:
@@ -326,29 +336,27 @@
         # If the final image already exists, don't continue
         if os.path.exists(sif_binary):
             return
 
         # Case 1: Given an image
         if self.image is not None:
             if not os.path.exists(self.image):
-
                 # Can we pull it?
                 if re.search("(docker|library|shub|http?s)[://]", self.image):
                     bot.info("Pulling %s" % self.image)
                     self.client.pull(self.image, name=sif_binary)
 
                 else:
                     bot.exit(
                         "%s is an invalid unique resource identifier." % self.image
                     )
 
         # Case 2: Given a recipe
         elif self.recipe is not None:
-
-            # Change directory to the context
+            # Change directory to the context if it exists
             context = os.path.abspath(self.context)
             os.chdir(context)
 
             # The recipe is expected to exist in the context folder
             if not os.path.exists(self.recipe):
                 bot.exit("%s not found for build" % self.recipe)
 
@@ -368,15 +376,15 @@
                     sudo=sudo,
                     stream=True,
                 )
 
                 for line in stream:
                     print(line)
 
-            except:
+            except Exception:
                 build = "sudo singularity build %s %s" % (
                     os.path.basename(sif_binary),
                     self.recipe,
                 )
 
                 bot.warning("Issue building container, try: %s" % build)
 
@@ -392,15 +400,14 @@
         options (if they exist)
         """
         options = []
 
         if "build" in self.params:
             if "options" in self.params["build"]:
                 for option in self.params["build"]["options"]:
-
                     # if the option is a string, it's a boolean flag
                     if isinstance(option, str):
                         options.append("--%s" % option)
 
                     # Otherwise, the user set a boolean with a value or an arg
                     elif isinstance(option, dict):
                         for key, val in option.items():
@@ -495,15 +502,15 @@
             try:
                 if not self.sudo:
                     self.client._run_command(["rm", logfile], quiet=True)
                     self.client._run_command(["touch", logfile], quiet=True)
                 else:
                     self.client._run_command(["sudo", "rm", logfile], quiet=True)
                     self.client._run_command(["sudo", "touch", logfile], quiet=True)
-            except:
+            except Exception:
                 pass
 
     def _get_log_folder(self):
         """
         Get a log folder that includes a user, home, and host
         """
         home = get_userhome()
@@ -540,15 +547,15 @@
                         result = "\n".join(result.split("\n")[-tail:])
                     bot.custom(
                         prefix=self.get_replica_name(), message=ext, color="CYAN"
                     )
                     print(result)
                     bot.newline()
 
-            except:
+            except Exception:
                 pass
 
     # Create and Delete
 
     def up(self, working_dir, ip_address=None, writable_tmpfs=False):
         """
         Up is the same as create, but like Docker, we build / pull instances
@@ -575,15 +582,14 @@
 
         # Case 2: Image not built.
         if not os.path.exists(image):
             bot.exit("Image %s not found, please run build first." % image)
 
         # Finally, create the instance
         if not self.exists():
-
             bot.info("Creating %s" % self.get_replica_name())
 
             # Command options
             options = []
 
             # Volumes
             options += self._get_bind_commands()
@@ -617,15 +623,14 @@
                 options=options,
                 image=image,
                 args=self.args,
             )
 
             # If the user has exec defined, exec to it
             if self.exec_args:
-
                 # Show the command to the user
                 commands = "%s %s %s" % (
                     " ".join(self.exec_opts),
                     self.uri,
                     self.exec_args,
                 )
                 bot.debug("singularity exec %s" % commands)
@@ -637,15 +642,14 @@
                     stream=True,
                     options=self.exec_opts,
                 ):
                     print(line)
 
             # If the user has run defined, finish with the run
             if "run" in self.params:
-
                 run_args = self.run_args or ""
 
                 # Show the command to the user
                 commands = "%s %s %s" % (
                     " ".join(self.run_opts),
                     self.uri,
                     run_args,
```

### Comparing `singularity-compose-0.1.18/scompose/project/project.py` & `singularity-compose-0.1.19/scompose/project/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 
-from scompose.templates import get_template
-from scompose.logger import bot
-from scompose.utils import read_file, write_file
-from ..config import merge_config
-from spython.main import get_client
-from .instance import Instance
-from ipaddress import IPv4Network
 import json
 import os
 import re
 import subprocess
 from copy import deepcopy
+from ipaddress import IPv4Network
+
+from spython.main import get_client
+
+from scompose.logger import bot
+from scompose.templates import get_template
+from scompose.utils import read_file, write_file
+
+from ..config import merge_config
+from .instance import Instance
 
 
 class Project:
     """
     A compose project is a group of containers read in from a config file.
     """
 
     config = None
     instances = {}
 
     def __init__(self, filename=None, name=None, env_file=None):
-
         self.set_filename(filename)
         self.set_name(name)
         self.load()
         self.parse()
         self.env_file = env_file
         self.client = get_client()
         self.running = self.get_already_running()
@@ -175,15 +177,14 @@
         Parse a loaded config
         """
 
         # If a port is defined, we need root.
         self.sudo = False
 
         if self.config is not None:
-
             # If any of config has ports, and no fakeroot, must use sudo
             for name in self.config.get("instances", []):
                 params = self.config["instances"][name]
                 start_options = params.get("start", {}).get("options", {})
 
                 # If we have fakeroot, don't use sudo
                 if (
@@ -449,49 +450,47 @@
             instance.stop(timeout=timeout)
 
     # Create
 
     def create(
         self, names=None, writable_tmpfs=True, bridge="10.22.0.0/16", no_resolv=False
     ):
-
         """
         Call the create function, which defaults to the command instance.create()
         """
         return self._create(names, writable_tmpfs=writable_tmpfs, no_resolv=no_resolv)
 
     def up(
         self,
         names=None,
         writable_tmpfs=True,
         bridge="10.22.0.0/16",
         no_resolv=False,
     ):
-
         """
         Call the up function, instance.up().
 
         This will build before if a container binary does not exist.
         """
         return self._create(
             names,
             command="up",
             writable_tmpfs=writable_tmpfs,
+            bridge=bridge,
             no_resolv=no_resolv,
         )
 
     def _create(
         self,
         names,
         command="create",
         writable_tmpfs=True,
         bridge="10.22.0.0/16",
         no_resolv=False,
     ):
-
         """
         Create one or more instances.
 
         "Command" determines the sub function to call for the instance,
         which should be "create" or "up". If the user provide a list of names,
         use them, otherwise default to all instances.
```

### Comparing `singularity-compose-0.1.18/scompose/templates/__init__.py` & `singularity-compose-0.1.19/scompose/templates/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 
+import os
+
 from scompose.logger import bot
 from scompose.utils import get_installdir
 
-import os
-
 
 def get_template(name):
     """get a template by name from this directory. If does not exist,
     return None.
     """
     here = get_installdir()
     template = os.path.join(here, "templates", name)
```

### Comparing `singularity-compose-0.1.18/scompose/tests/test_client.py` & `singularity-compose-0.1.19/scompose/tests/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/python
 
-# Copyright (C) 2019-2022 Vanessa Sochat.
+# Copyright (C) 2019-2024 Vanessa Sochat.
 
 # This Source Code Form is subject to the terms of the
 # Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 # with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from scompose.project import Project
-from scompose.utils import run_command
+import os
 from time import sleep
+
 import requests
-import pytest
-import os
 
+from scompose.project import Project
+from scompose.utils import run_command
 
-def test_commands(tmp_path):
 
+def test_commands(tmp_path):
     tmpdir = os.path.join(tmp_path, "repo")
     repo = "https://github.com/singularityhub/singularity-compose-examples"
 
     # Clone the example
     run_command(["git", "clone", repo, tmpdir])
 
     # Test the simple apache example
```

### Comparing `singularity-compose-0.1.18/scompose/tests/test_command_args.py` & `singularity-compose-0.1.19/scompose/tests/test_command_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/python
 
-# Copyright (C) 2019-2022 Vanessa Sochat.
+# Copyright (C) 2019-2024 Vanessa Sochat.
 
 # This Source Code Form is subject to the terms of the
 # Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 # with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+import os
+import shutil
+from time import sleep
+
 from scompose.logger import bot
 from scompose.project import Project
-from scompose.utils import run_command
-from time import sleep
-import shutil
-import pytest
-import os
 
 here = os.path.dirname(os.path.abspath(__file__))
 
 
 def test_command_args(tmp_path):
     bot.clear()  ## Clear previously logged messages
```

### Comparing `singularity-compose-0.1.18/scompose/tests/test_config.py` & `singularity-compose-0.1.19/scompose/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 
-# Copyright (C) 2017-2022 Vanessa Sochat.
+# Copyright (C) 2017-2024 Vanessa Sochat.
 
 # This Source Code Form is subject to the terms of the
 # Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 # with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import os
 
@@ -39,16 +39,16 @@
     a = {"a": 123, "b": {"c": "d"}}
     b = {"b": {"c": "f"}}
     assert _merge(a, b) == {"a": 123, "b": {"c": "f"}}
 
 
 def test_deep_merge():
     print("Testing utils._deep_merge")
-    from scompose.utils import read_yaml
     from scompose.config import _deep_merge
+    from scompose.utils import read_yaml
 
     config_override = os.path.join(here, "configs", "config_merge")
 
     # single file
     yaml_files = [
         read_yaml(
             os.path.join(config_override, "singularity-compose-1.yml"), quiet=True
```

### Comparing `singularity-compose-0.1.18/scompose/tests/test_depends_on.py` & `singularity-compose-0.1.19/scompose/tests/test_depends_on.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 #!/usr/bin/python
 
-# Copyright (C) 2019-2022 Vanessa Sochat.
+# Copyright (C) 2019-2024 Vanessa Sochat.
 
 # This Source Code Form is subject to the terms of the
 # Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 # with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+import os
+import shutil
+from time import sleep
+
 from scompose.logger import bot
 from scompose.project import Project
-from scompose.utils import run_command
-from time import sleep
-import shutil
-import pytest
-import os
 
 here = os.path.dirname(os.path.abspath(__file__))
 
 
 def test_circular_dependency(tmp_path):
-
     depends_on = os.path.join(here, "configs", "wrong_depends_on")
     for filename in os.listdir(depends_on):
         source = os.path.join(depends_on, filename)
         dest = os.path.join(tmp_path, filename)
         print("Copying %s to %s" % (filename, dest))
         shutil.copyfile(source, dest)
```

### Comparing `singularity-compose-0.1.18/scompose/tests/test_utils.py` & `singularity-compose-0.1.19/scompose/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/python
 
-# Copyright (C) 2017-2022 Vanessa Sochat.
+# Copyright (C) 2017-2024 Vanessa Sochat.
 
 # This Source Code Form is subject to the terms of the
 # Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 # with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import os
+
 import pytest
 
 here = os.path.dirname(os.path.abspath(__file__))
 
 
 def test_write_read_files(tmp_path):
     """test_write_read_files will test the functions write_file and read_file"""
@@ -37,15 +38,16 @@
     assert not os.path.exists(tmpfile)
     with pytest.raises(TypeError):
         write_json(bad_json, tmpfile)
 
 
 def test_write_json(tmp_path):
     import json
-    from scompose.utils import write_json, read_json
+
+    from scompose.utils import read_json, write_json
 
     good_json = {"Wakkawakkawakka": [True, "2", 3]}
     tmpfile = str(tmp_path / "good_json_file.txt")
     assert not os.path.exists(tmpfile)
     write_json(good_json, tmpfile)
     with open(tmpfile, "r") as f:
         content = json.loads(f.read())
```

### Comparing `singularity-compose-0.1.18/scompose/utils/__init__.py` & `singularity-compose-0.1.19/scompose/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 
 import errno
 import json
 import os
 import pwd
 import sys
-import yaml
+from subprocess import PIPE, STDOUT, Popen
 
-from subprocess import Popen, PIPE, STDOUT
+import yaml
 
 
 def get_installdir():
     """get_installdir returns the installation directory of the application"""
     return os.path.abspath(os.path.dirname(os.path.dirname(__file__)))
```

### Comparing `singularity-compose-0.1.18/scompose/version.py` & `singularity-compose-0.1.19/scompose/version.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 
-Copyright (C) 2019-2022 Vanessa Sochat.
+Copyright (C) 2019-2024 Vanessa Sochat.
 
 This Source Code Form is subject to the terms of the
 Mozilla Public License, v. 2.0. If a copy of the MPL was not distributed
 with this file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 
-__version__ = "0.1.18"
+__version__ = "0.1.19"
 AUTHOR = "Vanessa Sochat"
 AUTHOR_EMAIL = "vsoch@users.noreply.github.com"
 NAME = "singularity-compose"
 PACKAGE_URL = "http://github.com/singularityhub/singularity-compose"
 KEYWORDS = "singularity, compose"
 DESCRIPTION = "simple orchestration for singularity containers"
 LICENSE = "LICENSE"
```

### Comparing `singularity-compose-0.1.18/setup.py` & `singularity-compose-0.1.19/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from setuptools import setup, find_packages
-import codecs
 import os
 
+from setuptools import find_packages, setup
+
 ################################################################################
 # HELPER FUNCTIONS #############################################################
 ################################################################################
 
 
 def get_lookup():
     """get version by way of sregistry.version, returns a
@@ -20,25 +20,25 @@
 
 
 # Read in requirements
 def get_reqs(lookup=None, key="INSTALL_REQUIRES"):
     """get requirements, mean reading in requirements and versions from
     the lookup obtained with get_lookup"""
 
-    if lookup == None:
+    if lookup is None:
         lookup = get_lookup()
 
     install_requires = []
     for module in lookup[key]:
         module_name = module[0]
         module_meta = module[1]
         if "exact_version" in module_meta:
             dependency = "%s==%s" % (module_name, module_meta["exact_version"])
         elif "min_version" in module_meta:
-            if module_meta["min_version"] == None:
+            if module_meta["min_version"] is None:
                 dependency = module_name
             else:
                 dependency = "%s>=%s" % (module_name, module_meta["min_version"])
         install_requires.append(dependency)
     return install_requires
 
 
@@ -61,15 +61,14 @@
 
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 
 if __name__ == "__main__":
-
     INSTALL_REQUIRES = get_reqs(lookup)
     INSTALL_REQUIRES_ALL = get_reqs(lookup, "INSTALL_REQUIRES_ALL")
     INSTALL_REQUIRES_CHECKS = get_reqs(lookup, "INSTALL_REQUIRES_CHECKS")
     TESTS_REQUIRES = get_reqs(lookup, "TESTS_REQUIRES")
 
     setup(
         name=NAME,
```

### Comparing `singularity-compose-0.1.18/singularity_compose.egg-info/PKG-INFO` & `singularity-compose-0.1.19/singularity_compose.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: singularity-compose
-Version: 0.1.18
+Version: 0.1.19
 Summary: simple orchestration for singularity containers
 Home-page: http://github.com/singularityhub/singularity-compose
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 Maintainer-email: vsoch@users.noreply.github.com
 License: LICENSE
 Keywords: singularity,compose
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
@@ -27,17 +26,15 @@
 
 # Singularity Compose
 
 [![status](http://joss.theoj.org/papers/1fc2593b11b5e18df12efb59ed8757a0/status.svg)](http://joss.theoj.org/papers/1fc2593b11b5e18df12efb59ed8757a0)
 [![DOI](https://zenodo.org/badge/188852712.svg)](https://zenodo.org/badge/latestdoi/188852712)
 
 This is a simple orchestration library for Singularity containers, akin to
-Docker Compose. See the [specification](https://singularityhub.github.io/singularity-compose/#/spec/spec-1.0) 
+Docker Compose. See the [specification](https://singularityhub.github.io/singularity-compose/#/spec/spec-1.0)
 and the [documentation](https://singularityhub.github.io/singularity-compose) for
 details, or more examples below.
 
 ## Examples
 
 See our [Singularity Compose Examples](https://www.github.com/singularityhub/singularity-compose-examples) repository for
 finding or contributing examples for using scompose.
-
-
```

### Comparing `singularity-compose-0.1.18/singularity_compose.egg-info/SOURCES.txt` & `singularity-compose-0.1.19/singularity_compose.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
+setup.cfg
 setup.py
 scompose/__init__.py
 scompose/version.py
 scompose/client/__init__.py
 scompose/client/build.py
 scompose/client/check.py
 scompose/client/config.py
```

