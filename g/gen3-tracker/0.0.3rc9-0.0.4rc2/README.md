# Comparing `tmp/gen3_tracker-0.0.3rc9.tar.gz` & `tmp/gen3_tracker-0.0.4rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_tracker-0.0.3rc9.tar", last modified: Thu Apr 18 00:09:29 2024, max compression
+gzip compressed data, was "gen3_tracker-0.0.4rc2.tar", last modified: Sat May 11 18:17:12 2024, max compression
```

## Comparing `gen3_tracker-0.0.3rc9.tar` & `gen3_tracker-0.0.4rc2.tar`

### file list

```diff
@@ -1,120 +1,67 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.417907 gen3_tracker-0.0.3rc9/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.3rc9/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     2415 2024-04-18 00:09:29.417585 gen3_tracker-0.0.3rc9/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1338 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc9/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.416991 gen3_tracker-0.0.3rc9/gen3_tracker.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2415 2024-04-18 00:09:29.000000 gen3_tracker-0.0.3rc9/gen3_tracker.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     2904 2024-04-18 00:09:29.000000 gen3_tracker-0.0.3rc9/gen3_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-04-18 00:09:29.000000 gen3_tracker-0.0.3rc9/gen3_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       47 2024-04-18 00:09:29.000000 gen3_tracker-0.0.3rc9/gen3_tracker.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      186 2024-04-18 00:09:29.000000 gen3_tracker-0.0.3rc9/gen3_tracker.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       16 2024-04-18 00:09:29.000000 gen3_tracker-0.0.3rc9/gen3_tracker.egg-info/top_level.txt
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.362975 gen3_tracker-0.0.3rc9/gen3_util/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2885 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc9/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.372645 gen3_tracker-0.0.3rc9/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) 1971611142     3307 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4974 2024-04-16 23:28:35.000000 gen3_tracker-0.0.3rc9/gen3_util/access/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.380197 gen3_tracker-0.0.3rc9/gen3_util/access/policies/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_tracker-0.0.3rc9/gen3_util/access/policies/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      189 2024-02-29 16:26:49.000000 gen3_tracker-0.0.3rc9/gen3_util/access/policies/add-project-default.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142       77 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc9/gen3_util/access/policies/add-user-delete.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142       76 2024-02-26 20:40:22.000000 gen3_tracker-0.0.3rc9/gen3_util/access/policies/add-user-read.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142      199 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc9/gen3_util/access/policies/add-user-write.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142     6732 2024-04-13 10:20:42.000000 gen3_tracker-0.0.3rc9/gen3_util/access/requestor.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1052 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/access/submitter.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.381605 gen3_tracker-0.0.3rc9/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1211 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      883 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.381880 gen3_tracker-0.0.3rc9/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) 1971611142    13758 2024-04-13 10:20:22.000000 gen3_tracker-0.0.3rc9/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.382533 gen3_tracker-0.0.3rc9/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) 1971611142    10225 2024-04-13 10:20:22.000000 gen3_tracker-0.0.3rc9/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      876 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      137 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/config.yaml
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.398749 gen3_tracker-0.0.3rc9/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1457 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    12297 2024-04-16 23:15:38.000000 gen3_tracker-0.0.3rc9/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3751 2024-03-01 20:19:22.000000 gen3_tracker-0.0.3rc9/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    13433 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc9/gen3_util/files/manifest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1503 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc9/gen3_util/files/middleware.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      634 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5194 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.401024 gen3_tracker-0.0.3rc9/gen3_util/jobs/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:01:08.000000 gen3_tracker-0.0.3rc9/gen3_util/jobs/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2618 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/jobs/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/jobs/lister.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.405187 gen3_tracker-0.0.3rc9/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4438 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc9/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1415 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc9/gen3_util/meta/bundler.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     8981 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      687 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/meta/delta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2894 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/meta/differ.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      326 2023-10-19 18:01:08.000000 gen3_tracker-0.0.3rc9/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2204 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1655 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2932 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc9/gen3_util/meta/publisher.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    15444 2024-04-16 23:23:47.000000 gen3_tracker-0.0.3rc9/gen3_util/meta/skeleton.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.405413 gen3_tracker-0.0.3rc9/gen3_util/meta/tabular/
--rw-r--r--   0 walsbr   (320923486) 1971611142    11706 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc9/gen3_util/meta/tabular/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4660 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4477 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc9/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.406274 gen3_tracker-0.0.3rc9/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2778 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3696 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc9/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2341 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1496 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc9/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.408444 gen3_tracker-0.0.3rc9/gen3_util/repo/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4557 2024-04-11 18:50:38.000000 gen3_tracker-0.0.3rc9/gen3_util/repo/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    17892 2024-04-18 00:06:06.000000 gen3_tracker-0.0.3rc9/gen3_util/repo/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3726 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/repo/cloner.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     9643 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc9/gen3_util/repo/committer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/repo/history.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1427 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc9/gen3_util/repo/initializer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3168 2024-04-18 00:06:17.000000 gen3_tracker-0.0.3rc9/gen3_util/repo/puller.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4405 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc9/gen3_util/repo/pusher.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2959 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/gen3_util/repo/status.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.408944 gen3_tracker-0.0.3rc9/gen3_util/users/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:09:26.000000 gen3_tracker-0.0.3rc9/gen3_util/users/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1761 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc9/gen3_util/users/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-04-18 00:09:29.417957 gen3_tracker-0.0.3rc9/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5581 2024-04-18 00:09:18.000000 gen3_tracker-0.0.3rc9/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.343884 gen3_tracker-0.0.3rc9/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.412002 gen3_tracker-0.0.3rc9/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc9/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1091 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1066 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      454 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    12460 2024-04-13 10:20:22.000000 gen3_tracker-0.0.3rc9/tests/integration/test_commit.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      257 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/integration/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4867 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc9/tests/integration/test_foreign_bucket.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2182 2024-04-13 10:20:22.000000 gen3_tracker-0.0.3rc9/tests/integration/test_init.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     9506 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/integration/test_meta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     8848 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/integration/test_meta_skeleton.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5763 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc9/tests/integration/test_no_bucket.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1321 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc9/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.414417 gen3_tracker-0.0.3rc9/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc9/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      464 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/unit/conftest.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.414639 gen3_tracker-0.0.3rc9/tests/unit/plugins/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:45:48.000000 gen3_tracker-0.0.3rc9/tests/unit/plugins/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.414844 gen3_tracker-0.0.3rc9/tests/unit/plugins/gen3_util_plugin_foo/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1450 2023-07-07 00:45:48.000000 gen3_tracker-0.0.3rc9/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-18 00:09:29.416715 gen3_tracker-0.0.3rc9/tests/unit/tabular/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/unit/tabular/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    16696 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc9/tests/unit/tabular/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1172 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/unit/tabular/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     7826 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc9/tests/unit/tabular/test_default_columns.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1035 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/unit/tabular/test_dir_to_tabular.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1888 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/unit/tabular/test_from_tabular.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3779 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc9/tests/unit/tabular/test_to_tabular.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      737 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/unit/tabular/test_validate.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3841 2024-04-13 10:20:23.000000 gen3_tracker-0.0.3rc9/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4881 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc9/tests/unit/test_coding.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc9/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      532 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1417 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      445 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc9/tests/unit/test_job_dependencies.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      734 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/unit/test_manifest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/unit/test_validate_directory.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      625 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc9/tests/unit/test_version.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.565878 gen3_tracker-0.0.4rc2/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.4rc2/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2409 2024-05-11 18:17:12.565310 gen3_tracker-0.0.4rc2/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1524 2024-05-06 16:38:51.000000 gen3_tracker-0.0.4rc2/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.463900 gen3_tracker-0.0.4rc2/g3t/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5965 2024-05-08 22:57:00.000000 gen3_tracker-0.0.4rc2/g3t/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2891 2024-05-02 01:38:13.000000 gen3_tracker-0.0.4rc2/g3t/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.464690 gen3_tracker-0.0.4rc2/g3t/collaborator/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:09:26.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.467361 gen3_tracker-0.0.4rc2/g3t/collaborator/access/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3301 2024-04-27 12:56:43.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5079 2024-05-03 17:05:40.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.480759 gen3_tracker-0.0.4rc2/g3t/collaborator/access/policies/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/policies/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      189 2024-02-29 16:26:49.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/policies/add-project-default.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142       76 2024-02-26 20:40:22.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/policies/add-user-read.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142      204 2024-05-09 02:02:53.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/policies/add-user-write.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6802 2024-04-29 14:48:58.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/requestor.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1105 2024-05-03 17:05:40.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/access/submitter.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13639 2024-05-09 22:58:55.000000 gen3_tracker-0.0.4rc2/g3t/collaborator/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.484179 gen3_tracker-0.0.4rc2/g3t/common/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    18425 2024-05-06 14:21:17.000000 gen3_tracker-0.0.4rc2/g3t/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.485029 gen3_tracker-0.0.4rc2/g3t/config/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    10280 2024-04-29 04:46:34.000000 gen3_tracker-0.0.4rc2/g3t/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      137 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc2/g3t/config.yaml
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.487134 gen3_tracker-0.0.4rc2/g3t/gen3/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-04-27 13:15:12.000000 gen3_tracker-0.0.4rc2/g3t/gen3/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.490714 gen3_tracker-0.0.4rc2/g3t/gen3/buckets/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1314 2024-04-25 20:19:51.000000 gen3_tracker-0.0.4rc2/g3t/gen3/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      883 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc2/g3t/gen3/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc2/g3t/gen3/buckets/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3345 2024-04-30 21:12:45.000000 gen3_tracker-0.0.4rc2/g3t/gen3/indexd.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4128 2024-04-29 13:40:35.000000 gen3_tracker-0.0.4rc2/g3t/gen3/jobs.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.499875 gen3_tracker-0.0.4rc2/g3t/git/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    20188 2024-05-06 16:23:20.000000 gen3_tracker-0.0.4rc2/g3t/git/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    11558 2024-05-08 22:16:58.000000 gen3_tracker-0.0.4rc2/g3t/git/adder.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    31775 2024-05-09 02:03:59.000000 gen3_tracker-0.0.4rc2/g3t/git/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2499 2024-05-01 18:43:40.000000 gen3_tracker-0.0.4rc2/g3t/git/cloner.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1439 2024-05-03 17:05:40.000000 gen3_tracker-0.0.4rc2/g3t/git/initializer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2555 2024-05-02 22:49:35.000000 gen3_tracker-0.0.4rc2/g3t/git/snapshotter.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.507229 gen3_tracker-0.0.4rc2/g3t/meta/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5915 2024-05-03 04:59:19.000000 gen3_tracker-0.0.4rc2/g3t/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4907 2024-05-03 19:09:24.000000 gen3_tracker-0.0.4rc2/g3t/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13471 2024-05-03 19:08:14.000000 gen3_tracker-0.0.4rc2/g3t/meta/dataframer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    11125 2024-05-03 17:05:40.000000 gen3_tracker-0.0.4rc2/g3t/meta/skeleton.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4419 2024-04-22 22:58:13.000000 gen3_tracker-0.0.4rc2/g3t/meta/validator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1202 2024-04-28 11:58:11.000000 gen3_tracker-0.0.4rc2/g3t/meta/visualizer.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.544280 gen3_tracker-0.0.4rc2/g3t/projects/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2772 2024-04-26 19:19:19.000000 gen3_tracker-0.0.4rc2/g3t/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4745 2024-05-09 02:02:53.000000 gen3_tracker-0.0.4rc2/g3t/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2393 2024-05-03 17:05:40.000000 gen3_tracker-0.0.4rc2/g3t/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1548 2024-05-03 17:05:40.000000 gen3_tracker-0.0.4rc2/g3t/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.564454 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2409 2024-05-11 18:17:12.000000 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1327 2024-05-11 18:17:12.000000 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-05-11 18:17:12.000000 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       36 2024-05-11 18:17:12.000000 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      219 2024-05-11 18:17:12.000000 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        4 2024-05-11 18:17:12.000000 gen3_tracker-0.0.4rc2/gen3_tracker.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-05-11 18:17:12.565930 gen3_tracker-0.0.4rc2/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142      723 2024-05-11 18:16:51.000000 gen3_tracker-0.0.4rc2/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.448832 gen3_tracker-0.0.4rc2/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-11 18:17:12.563924 gen3_tracker-0.0.4rc2/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-05-02 22:49:35.000000 gen3_tracker-0.0.4rc2/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    20363 2024-05-01 22:45:46.000000 gen3_tracker-0.0.4rc2/tests/unit/test_flatten_fhir_example.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1267 2024-04-30 17:33:26.000000 gen3_tracker-0.0.4rc2/tests/unit/test_hash_types.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      592 2024-04-30 18:17:55.000000 gen3_tracker-0.0.4rc2/tests/unit/test_read_dvc.py
```

### Comparing `gen3_tracker-0.0.3rc9/LICENSE` & `gen3_tracker-0.0.4rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/access/__init__.py` & `gen3_tracker-0.0.4rc2/g3t/collaborator/access/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from gen3.auth import Gen3Auth
 from requests import HTTPError
 
-from gen3_util.config import ensure_auth, Config
+from g3t.config import ensure_auth, Config
 
 
 def _ensure_auth(auth, config):
     """Create auth from config, if we don't have one already."""
     if not auth:
         assert config
         auth = ensure_auth(config=config)
```

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/access/cli.py` & `gen3_tracker-0.0.4rc2/g3t/collaborator/access/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import click
 
-from gen3_util.access import create_request
-from gen3_util.access.requestor import ls, cat, update, LogAccess
-from gen3_util.common import validate_email
-from gen3_util.config import Config, ensure_auth
-from gen3_util.repo import CLIOutput
-from gen3_util.repo import NaturalOrderGroup
+from g3t.common import validate_email
+from g3t.config import Config, ensure_auth
+from g3t.common import CLIOutput
+from g3t import NaturalOrderGroup
 
 
 @click.group(name='access', cls=NaturalOrderGroup)
 @click.pass_obj
 def access_group(config: Config):
     """Manage access requests."""
     pass
@@ -25,14 +23,16 @@
 def access_touch(config: Config,  resource_path: str, user_name: str, roles: str, steward: bool):
     """Create a request a specific role.
 
     \b
     USER_NAME (str): user's email
 
     """
+    from g3t.collaborator.access import create_request
+
     with CLIOutput(config=config) as output:
         try:
 
             msgs = validate_email(user_name)
             assert msgs == [], f"Invalid email address: {user_name} {msgs}"
 
             assert user_name, "user_name required"
@@ -57,14 +57,16 @@
 @click.option('--request_id', required=False, help='Sign only this request')
 @click.pass_obj
 def sign(config: Config, username: str, request_id: str):
     """Sign all policies for a project.
     \b
     """
     with CLIOutput(config=config) as output:
+        from g3t.collaborator.access.requestor import ls, update, LogAccess
+
         auth = ensure_auth(config=config)
         access = ls(config, mine=False, username=username, active=True, auth=auth)
         unsigned_requests = [_ for _ in access.requests if _['status'] != 'SIGNED']
 
         if len(unsigned_requests) == 0:
             output.update(LogAccess(**{
                 'msg': "No unsigned requests found"
@@ -97,14 +99,16 @@
 @access_group.command(name="ls")
 @click.option('--username', required=False, default=None, help='Sign all requests for user within a project')
 @click.option('--mine',  is_flag=True, show_default=True, default=False, help="List current user's requests. Otherwise, list all the requests the current user has access to see.")
 @click.option('--all', 'active', is_flag=True, show_default=True, default=True, help='Only unsigned requests')
 @click.pass_obj
 def access_ls(config: Config, mine: bool, active: bool, username: str):
     """List current user's requests."""
+    from g3t.collaborator.access.requestor import ls
+
     with CLIOutput(config=config) as output:
         try:
             msg = 'OK'
             access = ls(config, mine, active, username)
             if not access.requests or len(access.requests) == 0:
                 msg = 'No unsigned requests'
             output.update({'requests': access.requests, 'msg': msg})
@@ -118,9 +122,11 @@
 @click.pass_obj
 def access_cat(config: Config, request_id: str):
     """Show details of a specific request.
 
     \b
     request_id (str): uuid of an existing request
     """
+    from g3t.collaborator.access.requestor import cat
+
     with CLIOutput(config=config) as output:
         output.update(cat(config, request_id))
```

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/access/requestor.py` & `gen3_tracker-0.0.4rc2/g3t/collaborator/access/requestor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import logging
 from typing import List
 
 import yaml
 from gen3.auth import Gen3Auth
 from pydantic import BaseModel
 
-from gen3_util.access import get_requests, get_request, create_request, update_request
-from gen3_util.config import Config, ensure_auth
+from g3t.collaborator.access import get_requests, get_request, create_request, update_request
+from g3t.config import Config, ensure_auth
 
 from importlib.resources import files, as_file
 from . import policies
 
 
 class LogAccess(BaseModel):
     endpoint: str = None
@@ -101,15 +102,15 @@
     request = update_request(auth=auth, request_id=request_id, status=status)
     return LogAccess(**{
         'endpoint': auth.endpoint,
         'request': request,
     })
 
 
-def add_user(config: Config, project_id: str, user_name: str, write: bool, delete: bool) -> LogAccess:
+def add_user(config: Config, project_id: str, user_name: str, write: bool, delete: bool, auth: Gen3Auth) -> LogAccess:
     """Add user to project by assigning them policies."""
 
     # implement read from resource_path
     policies_ = []
     file_names = ['add-user-read.yaml']
     if write:
         file_names.append('add-user-write.yaml')
@@ -122,47 +123,50 @@
             with open(file_path) as f:
                 policies_.extend([_ for _ in yaml.safe_load(f)['policies']])
 
     requests = []
     request_ids = []
     for policy in policies_:
         policy = format_policy(policy, project_id, user_name)
-        requests.append(cp(request=policy, config=config).request)
+        requests.append(cp(request=policy, config=config, auth=auth).request)
         request_ids.append(requests[-1]['request_id'])
 
-    commands = ["g3t utilities access sign"]
+    commands = ["g3t collaborator add <user> --approve"]
     msg = f"An authorized user must approve these requests to  add {user_name} to {project_id}"
 
     return LogAccess(**{
         'requests': requests,
         'commands': commands,
         'msg': msg,
     })
 
 
 def rm_user(config: Config, project_id: str, user_name: str) -> LogAccess:
     """Revoke user from project's policies."""
 
     # implement read from resource_path
     policies_ = []
-    file_names = ['add-user-read.yaml', 'add-user-write.yaml', 'add-user-delete.yaml']
+    file_names = ['add-user-read.yaml', 'add-user-write.yaml']
 
     for file_name in file_names:
         source = files(policies).joinpath(file_name)
         with as_file(source) as file_path:
             with open(file_path) as f:
                 policies_.extend([_ for _ in yaml.safe_load(f)['policies']])
 
     requests = []
     request_ids = []
     for policy in policies_:
         policy = format_policy(policy, project_id, user_name)
-        requests.append(cp(request=policy, config=config, revoke=True).request)
+        try:
+            requests.append(cp(request=policy, config=config, revoke=True).request)
+        except Exception as e:
+            logging.getLogger(__package__).warning(f"Failed to revoke {user_name} from {project_id}: {e}")
     commands = [f"g3t utilities access update {request_id} SIGNED" for request_id in request_ids]
-    msg = f"Approve these requests to add {user_name} to {project_id}"
+    msg = f"Approve these requests to rm {user_name} to {project_id}"
 
     return LogAccess(**{
         'requests': requests,
         'commands': commands,
         'msg': msg,
     })
 
@@ -182,14 +186,14 @@
     requests = []
     request_ids = []
     for policy in policies_:
         policy = format_policy(policy, project_id, user_name=None)
         requests.append(cp(request=policy, config=config, auth=auth).request)
         request_ids.append(requests[-1]['request_id'])
 
-    commands = ["g3t utilities access sign"]
-    msg = f"An authorized user must approve these requests to assign default policies to {project_id}"
+    commands = []
+    msg = "OK"
     return LogAccess(**{
         'requests': requests,
         'msg': msg,
         'commands': commands,
     })
```

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/access/submitter.py` & `gen3_tracker-0.0.4rc2/g3t/collaborator/access/submitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 
 from gen3.auth import Gen3Auth
-from gen3.submission import Gen3Submission
 
-from gen3_util import Config
-from gen3_util.config import ensure_auth
+from g3t import Config
+from g3t.config import ensure_auth
 
 
 def ensure_program_project(config: Config, project_id: str, auth: Gen3Auth = None) -> str:
     """Ensure program and project exist in sheepdog.
     """
+    # improve startup time by importing only what is needed
+    from gen3.submission import Gen3Submission
+
     if not auth:
         auth = ensure_auth(config=config)
     program, project = project_id.split('-')
     submission = Gen3Submission(auth)
     msgs = []
     programs = [_.split('/')[-1] for _ in submission.get_programs()['links']]
     if program not in programs:
```

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/buckets/__init__.py` & `gen3_tracker-0.0.4rc2/g3t/gen3/buckets/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 from gen3.auth import Gen3Auth
 
-from gen3_util.config import ensure_auth, Config
+from g3t.config import ensure_auth, Config
 
 
 def get_buckets(config: Config = None, auth: Gen3Auth = None) -> dict:
     """Fetch information about the buckets."""
     if not auth:
         assert config
         auth = ensure_auth(config=config)
@@ -21,17 +21,19 @@
             "see quay.io/cdis/fence:feature_bucket_info_endpoint "
         )
 
     assert response.status_code == 200, (response.status_code, response.content)
     return response.json()
 
 
-def get_program_bucket(config: Config, program: str, auth: Gen3Auth = None) -> str:
+def get_program_bucket(config: Config, auth: Gen3Auth = None) -> str:
     """Get the bucket for a program."""
     buckets = get_buckets(config=config, auth=auth)
     bucket_name = None
+    program = config.gen3.program
     for k, v in buckets['S3_BUCKETS'].items():
+        assert 'programs' in v, f"no configured programs in fence buckets {v} {buckets}"
         if program in v['programs']:
             bucket_name = k
             break
     # assert bucket_name, f"could not find bucket for {program}"
     return bucket_name
```

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/buckets/cli.py` & `gen3_tracker-0.0.4rc2/g3t/gen3/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/buckets/lister.py` & `gen3_tracker-0.0.4rc2/g3t/gen3/buckets/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/common/__init__.py` & `gen3_tracker-0.0.4rc2/g3t/common/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,53 @@
 import csv
 import json
 import logging
 import os
 import pathlib
+import re
 import shutil
+import sys
 import uuid
 import zipfile
 from datetime import datetime
 from hashlib import md5
 from typing import Mapping, Iterator, Dict, TextIO, Generator
 from urllib.parse import urlparse
 
+import click
+import dateutil
 import orjson
 import yaml
+from dateutil.tz import tzutc
 from fhir.resources.identifier import Identifier
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
 
 import io
 import gzip
-from gen3_util import Config, ACED_NAMESPACE
+
+from g3t import Config
+
+# see https://github.com/uc-cdis/indexd/blob/1ae3fea6569e8765d5b7247123b66bde9ce4c39c/indexd/index/blueprint.py#L35-L42
+ACCEPTABLE_HASHES = {
+    "md5": re.compile(r"^[0-9a-f]{32}$").match,
+    "sha1": re.compile(r"^[0-9a-f]{40}$").match,
+    "sha256": re.compile(r"^[0-9a-f]{64}$").match,
+    "sha512": re.compile(r"^[0-9a-f]{128}$").match,
+    "crc": re.compile(r"^[0-9a-f]{8}$").match,
+    "etag": re.compile(r"^[0-9a-f]{32}(-\d+)?$").match,
+}
+
+# Define color constants
+INFO_COLOR = 'yellow'
+ERROR_COLOR = 'red'
+SUCCESS_COLOR = 'green'
 
 PROJECT_DIR = '.g3t'
-PROJECT_DIRECTORIES = [PROJECT_DIR, 'META/']  # 'DATA/',
+PROJECT_DIRECTORIES = [PROJECT_DIR, 'META/', 'MANIFEST/', 'logs/']
 PROJECT_README = """
 # Data Directory
 
 Welcome to the data directory! This repository contains important data files for our project. Before you proceed, please take note of the following guidelines to ensure the security and integrity of our data.
 
 ## Important Note: Do Not Check in Protected Files
 
@@ -46,17 +67,18 @@
 3. **Security Awareness:** Be aware of the sensitivity of the data stored here and take necessary precautions to protect it from unauthorized access.
 
 
 Thank you for your cooperation in maintaining the security and confidentiality of our data.
 """
 
 
-def print_formatted(config: Config, output: Mapping) -> None:
+def print_formatted(config, output: Mapping) -> None:
     """Print the output, using configured output format"""
-
+    from g3t import Config
+    config: Config = config
     if config.output.format == "yaml":
         print(yaml.dump(output, sort_keys=False))
     elif config.output.format == "json":
         print(
             orjson.dumps(
                 output, default=pydantic_encoder, option=orjson.OPT_INDENT_2
             ).decode()
@@ -132,14 +154,16 @@
         return True
     except Exception as e:  # noqa
         return False
 
 
 def _file_opener(file_path):
     """Open file appropriately."""
+    if isinstance(file_path, str):
+        file_path = pathlib.Path(file_path)
     if file_path.name.endswith('gz'):
         fp = io.TextIOWrapper(io.BufferedReader(gzip.GzipFile(file_path)))  # noqa
     else:
         fp = open(file_path, "rb")
     return fp
 
 
@@ -172,28 +196,31 @@
     def __exit__(self, exc_type, exc_value, exc_tb):
         """Close all open files."""
         for _ in self.emitters.values():
             _.close()
             if self.verbose:
                 self.logger.info(f"closed {_.name}")
 
-    def emit(self, name: str) -> TextIO:
+    def emit(self, name: str, file_mode: str = None) -> TextIO:
         """Maintain a hash of open files."""
+        if not file_mode:
+            file_mode = self.file_mode
         if name not in self.emitters:
-            self.emitters[name] = open(self.output_path / f"{name}.ndjson", self.file_mode)
+            self.emitters[name] = open(self.output_path / f"{name}.ndjson", file_mode)
             if self.verbose:
                 self.logger.info(f"opened {self.emitters[name].name}")
 
             # If the user already has metadata in the resource file but wants to add
-            # another file the the first line will create a 2nd record on the same line causing the commit step to error
-            if os.path.getsize(self.emitters[name].name) > 0:
-                self.emitters[name].seek(self.emitters[name].tell() - 1, os.SEEK_SET)
-                last_char = self.emitters[name].read()
-                if last_char == "}":
-                    self.emitters[name].write("\n")
+            # another file the first line will create a 2nd record on the same line causing the commit step to error
+            if file_mode != 'a':
+                if os.path.getsize(self.emitters[name].name) > 0:
+                    self.emitters[name].seek(self.emitters[name].tell() - 1, os.SEEK_SET)
+                    last_char = self.emitters[name].read()
+                    if last_char == "}":
+                        self.emitters[name].write("\n")
         return self.emitters[name]
 
 
 def validate_project_id(project_id) -> list[str]:
     """Ensure that the project_id is valid"""
     msgs = []
     if not project_id:
@@ -274,14 +301,15 @@
     if _.system:
         return f"{_.system}|{_.value}"
     return _.value
 
 
 def create_id(resource, project_id) -> str:
     """Return id from identifier and project_id."""
+    from g3t import ACED_NAMESPACE
     assert resource, "resource required"
     assert project_id, "project_id required"
     identifier_string = identifier_to_string(resource.identifier)
     return str(uuid.uuid5(ACED_NAMESPACE, f"{project_id}/{resource.resource_type}/{identifier_string}"))
 
 
 class Commit(BaseModel):
@@ -304,15 +332,14 @@
     """The path to the manifest file."""
     meta_path: pathlib.Path = None
     """The path to the meta zip file."""
 
 
 class Push(BaseModel):
     """A list of commits."""
-
     config: Config
     """The config."""
 
     commits: list[Commit] = []
     """A list of commits in this push."""
 
     published_timestamp: datetime = None
@@ -407,7 +434,119 @@
     if md5:
         _['md5'] = md5
     if is_metadata:
         _['is_metadata'] = is_metadata
     if is_snapshot:
         _['is_snapshot'] = is_snapshot
     return _
+
+
+class CommandOutput(object):
+    """Output object for commands."""
+    def __init__(self):
+        self.obj = None
+        self.exit_code = 0
+
+    def update(self, obj):
+        """Update output with obj."""
+        self.obj = obj
+
+
+class CLIOutput:
+    """Ensure output, exceptions and exit code are returned to user consistently."""
+    from g3t import Config
+    def __init__(self, config: Config, exit_on_error: bool = True):
+        self.output = CommandOutput()
+        self.config = config
+        self.exit_on_error = exit_on_error
+
+    def __enter__(self):
+        return self.output
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        rc = 0
+        _ = {}
+        if self.output.obj is not None:
+            if isinstance(self.output.obj, dict):
+                _.update(self.output.obj)
+            elif isinstance(self.output.obj, list):
+                _ = self.output.obj
+            elif isinstance(self.output.obj, int):
+                _ = {'count': self.output.obj}
+            elif hasattr(self.output.obj, 'model_dump'):
+                _.update(self.output.obj.model_dump())
+            else:
+                _.update(self.output.obj.dict())
+        rc = self.output.exit_code
+        if exc_type is not None:
+            if isinstance(self.output.obj, dict):
+                _['exception'] = f"{str(exc_val)}"
+            elif isinstance(self.output.obj, list):
+                _.append(f"{str(exc_val)}")
+            else:
+                _.update({'exception': f"{str(exc_val)}"})
+            rc = 1
+            logging.getLogger(__name__).exception(exc_val)
+        if isinstance(_, dict) and 'msg' not in _:
+            if rc == 1:
+                _['msg'] = 'FAIL'
+            else:
+                _['msg'] = 'OK'
+        prune = []
+        if isinstance(_, dict):
+            for k, v in _.items():
+                if not v:
+                    prune.append(k)
+            for k in prune:
+                del _[k]
+        print_formatted(self.config, _)
+        self.output.exit_code = rc
+        if rc != 0 and self.exit_on_error:
+            exit(rc)
+
+
+def assert_config(config: Config):
+    """Ensure that the config exists, if called without help"""
+    try:
+        if '--help' in sys.argv:
+            return
+        exists = (pathlib.Path('.g3t') / 'config.yaml').exists()
+        msg = "project_id and profile are required"
+        if not exists:
+            msg = f"Config file config.yaml not found in {pathlib.Path('.g3t')}"
+        assert config.gen3.project_id and config.gen3.profile, f"ERROR {msg}, have you run 'g3t init'?"
+    except Exception as e:
+        click.secho(str(e), fg='red')
+        if config.debug:
+            raise e
+        sys.exit(1)
+
+
+def parse_iso_tz_date(date_str: str) -> str:
+    """Parse an iso date string."""
+    # parse the string into a datetime object
+    date_obj = dateutil.parser.parse(date_str)
+    # if the date string doesn't have a timezone, you can add one
+    if date_obj.tzinfo is None:
+        date_obj = date_obj.replace(tzinfo=tzutc())
+    # convert the datetime object back into an ISO formatted string with timezone
+    return date_obj.isoformat()
+
+
+def filter_dicts(data, pattern):
+    """Filter a list of dictionaries based on a pattern."""
+    pattern = re.compile(pattern)
+
+    if not isinstance(data, list):
+        data = [data]
+
+    def match_pattern(value):
+        if isinstance(value, str):
+            return pattern.search(value) is not None
+        elif isinstance(value, dict):
+            return any(match_pattern(v) for v in value.values())
+        elif isinstance(value, list):
+            return any(match_pattern(v) for v in value)
+        else:
+            return False
+
+    return [d for d in data if any(match_pattern(v) for v in d.values())]
```

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/config/__init__.py` & `gen3_tracker-0.0.4rc2/g3t/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 import importlib.resources as pkg_resources
 import requests
 import yaml
 from gen3.auth import Gen3Auth
 from gen3.file import Gen3File
 from gen3.index import Gen3Index
 
-import gen3_util
-from gen3_util import Config
-from gen3_util.common import read_yaml, PROJECT_DIRECTORIES, PROJECT_DIR, PROJECT_README
+import g3t
+from g3t import Config
+from g3t.common import read_yaml, PROJECT_DIRECTORIES, PROJECT_DIR, PROJECT_README
 
 
 def gen_client_ini_path() -> pathlib.Path:
     """Return path to gen3-client ini file. See https://bit.ly/3NbKGi4"""
     return pathlib.Path(pathlib.Path.home() / ".gen3" / "gen3_client_config.ini")
 
 
@@ -150,14 +150,15 @@
 
         logging.getLogger(__name__).error(msg)
         raise AssertionError(msg)
 
     return auth
 
 
+# TODO - unused, deprecate?
 def gen3_services(config: Config) -> tuple[Gen3File, Gen3Index, dict, Gen3Auth]:
     """Create Gen3 Services."""
     auth = ensure_auth(config=config)
     assert auth, f"Failed to set auth {config.gen3.profile}"
     file_client = Gen3File(auth_provider=auth)
     index_client = Gen3Index(auth_provider=auth)
     user = auth.curl('/user/user').json()
@@ -204,18 +205,18 @@
         if _.exists():
             return Config(**read_yaml(_))
 
     # use default
 
     # different pkg_resources open for 3.9
     if sys.version_info[:3] <= (3, 9):
-        _config = Config(**yaml.safe_load(pkg_resources.open_text(gen3_util, 'config.yaml').read()))
+        _config = Config(**yaml.safe_load(pkg_resources.open_text(g3t, 'config.yaml').read()))
     else:
         # https://docs.python.org/3.11/library/importlib.resources.html#importlib.resources.open_text
-        _config = Config(**yaml.safe_load(pkg_resources.files(gen3_util).joinpath('config.yaml').open().read()))
+        _config = Config(**yaml.safe_load(pkg_resources.files(g3t).joinpath('config.yaml').open().read()))
 
     # No config file found in directory or parents.
     _config.no_config_found = True
     return _config
 
 
 def custom(path: [str, pathlib.Path]):
@@ -225,14 +226,15 @@
 
     return Config(**read_yaml(path))
 
 
 def init(config: Config, project_id: str) -> Generator[str, None, None]:
     """Create an empty repository, adjust and write config file"""
 
+    logger = logging.getLogger(__name__)
     assert project_id, "project_id is missing"
     assert project_id.count('-') == 1, f"{project_id} should have a single '-' delimiter."
 
     existing_dirs = []
     for _ in PROJECT_DIRECTORIES:
         if pathlib.Path(_).exists():
             existing_dirs.append(_)
@@ -240,26 +242,26 @@
 
     if existing_dirs:
         yield f"Directory already exists {existing_dirs}"
     else:
         yield f"Created project directories {PROJECT_DIRECTORIES}"
 
     config.gen3.project_id = project_id
-    config.state_dir = pathlib.Path(PROJECT_DIR) / 'state'
-    config.state_dir.mkdir(parents=True, exist_ok=True)
+    config.work_dir = pathlib.Path(PROJECT_DIR) / 'work'
+    config.work_dir.mkdir(parents=True, exist_ok=True)
 
-    state_dir_git_ignore = config.state_dir / ".gitignore"
-    if not pathlib.Path(state_dir_git_ignore).exists():
-        with open(state_dir_git_ignore, 'w') as f:
-            f.write("*\n!README.md")
-
-    meta_dir_git_ignore = "META/.gitignore"
-    if not pathlib.Path(meta_dir_git_ignore).exists():
-        with open(meta_dir_git_ignore, 'w') as f:
-            f.write("*\n!README.md")
+    work_dir_git_ignore = config.work_dir / ".gitignore"
+    if not pathlib.Path(work_dir_git_ignore).exists():
+        with open(work_dir_git_ignore, 'w') as f:
+            f.write("*\n!README.md\n!.gitignore\n")
+
+    # meta_dir_git_ignore = "META/.gitignore"
+    # if not pathlib.Path(meta_dir_git_ignore).exists():
+    #     with open(meta_dir_git_ignore, 'w') as f:
+    #         f.write("*\n!README.md")
 
     for readme in [PROJECT_DIR + '/README.md', "META/README.md"]:
         if not pathlib.Path(readme).exists():
             path = pathlib.Path(readme)
             with open(path, 'w') as f:
                 f.write(PROJECT_README)
```

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/meta/__init__.py` & `gen3_tracker-0.0.4rc2/g3t/meta/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import importlib
 import logging
 import pathlib
-from typing import Iterator, Any, Optional
+from collections import defaultdict
+from typing import Iterator, Any, Optional, Callable
 
 # TODO fix me, make configurable
 from fhir.resources import FHIRAbstractModel
+from fhir.resources.bundle import BundleEntry
+from nested_lookup import nested_lookup
 from pydantic.v1 import ValidationError, validator
 from pydantic import BaseModel, ConfigDict
-from gen3_util.common import is_json_extension, read_json
+
+from g3t.common import is_json_extension, read_json, read_ndjson_file
 
 FHIR_CLASSES = importlib.import_module('fhir.resources')
 
 logger = logging.getLogger(__name__)
 
 
 class ParseResult(BaseModel):
@@ -60,29 +64,29 @@
     else:
         _path = parse_result.path
         offset = 0
         if parse_result.resource.entry and len(parse_result.resource.entry) > 0:
             for _ in parse_result.resource.entry:
                 if _ is None:
                     break
-                if hasattr(_, 'resource'):  # BundleEntry
+                if hasattr(_, 'resource') and _.resource:  # BundleEntry
                     yield ParseResult(path=_path, resource=_.resource, offset=offset, exception=None, json_obj=_.resource.dict())
                 elif hasattr(_, 'item'):  # ListEntry
                     yield ParseResult(path=_path, resource=_.item, offset=offset, exception=None, json_obj=_.item.dict())
                 else:
                     yield ParseResult(path=_path, resource=_.item, offset=offset, exception=None, json_obj=_.item.dict())
                 offset += 1
     pass
 
 
 def _has_entries(_: ParseResult):
     """FHIR types Bundles List have entries"""
     if _.resource is None:
         return False
-    return _.resource.resource_type in ["Bundle", "List"] and _.resource.entry is not None
+    return _.resource.resource_type in ["List"] and _.resource.entry is not None
 
 
 def directory_reader(directory_path: str,
                      recurse: bool = True,
                      validate: bool = False) -> Iterator[ParseResult]:
 
     """Extract FHIR resources from directory
@@ -112,7 +116,39 @@
             parse_result = parse_obj(json_obj, validate=validate)
             parse_result.path = input_file
             parse_result.offset = offset
             parse_result.json_obj = json_obj
             offset += 1
             for _ in _entry_iterator(parse_result):
                 yield _
+
+
+def aggregate(metadata_path: pathlib.Path | str) -> dict:
+    """Aggregate metadata counts resourceType(count)-count->resourceType(count)."""
+
+    nested_dict: Callable[[], defaultdict[str, defaultdict]] = lambda: defaultdict(defaultdict)
+
+    if not isinstance(metadata_path, pathlib.Path):
+        metadata_path = pathlib.Path(metadata_path)
+    summary = nested_dict()
+    for path in sorted(metadata_path.glob("*.ndjson")):
+        for _ in read_ndjson_file(path):
+
+            resource_type = _['resourceType']
+            if 'count' not in summary[resource_type]:
+                summary[resource_type]['count'] = 0
+            summary[resource_type]['count'] += 1
+
+            refs = nested_lookup('reference', _)
+            for ref in refs:
+                # A codeable reference is an object with a codeable concept and a reference
+                if isinstance(ref, dict):
+                    ref = ref['reference']
+                ref_resource_type = ref.split('/')[0]
+                if 'references' not in summary[resource_type]:
+                    summary[resource_type]['references'] = nested_dict()
+                dst = summary[resource_type]['references'][ref_resource_type]
+                if 'count' not in dst:
+                    dst['count'] = 0
+                dst['count'] += 1
+
+    return summary
```

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/meta/uploader.py` & `gen3_tracker-0.0.4rc2/g3t/gen3/jobs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,26 @@
-import logging
+import asyncio
 import pathlib
+import sys
 import tempfile
 import urllib
 import uuid
 from datetime import datetime
 from urllib.parse import urlparse
+from zipfile import ZipFile
 
-import requests
+from gen3.auth import Gen3Auth
 from gen3.file import Gen3File
 from gen3.index import Gen3Index
+from gen3.jobs import Gen3Jobs
 
-from gen3_util.buckets import get_program_bucket
-from gen3_util.config import Config, ensure_auth
-from zipfile import ZipFile
-
-from gen3_util import ACED_NAMESPACE
-from gen3_util.meta.importer import md5sum
-
-from gen3_util.files.uploader import _upload_file_to_signed_url  # noqa
-
-logger = logging.getLogger(__name__)
-
-
-def _update_indexd(id_, bucket_name, duplicate_check, index_client, md5_sum, object_name,
-                   program, project, metadata, size):
-    hashes = {'md5': md5_sum}
-    guid = id_
-    metadata = {
-        **metadata,
-        **hashes}
-    # SYNC
-    existing_record = None
-    s3_url = f"s3://{bucket_name}/{guid}/{object_name}"
-    if duplicate_check:
-        try:
-            existing_record = index_client.get_record(guid=guid)
-        except Exception: # noqa
-            pass
-        if existing_record:
-            skip_delete = all([
-                existing_record['hashes']['md5'] == md5sum,
-                s3_url in existing_record['urls']
-            ])
-            if not skip_delete:
-                # SYNC
-                logger.debug(f"Deleting existing record {guid}")
-                index_client.delete_record(guid=guid)
-                existing_record = None
-    if not existing_record:
-        try:
-            existing_record = index_client.create_record(
-                did=guid,
-                hashes=hashes,
-                size=size,
-                authz=[f'/programs/{program}/projects/{project}'],
-                file_name=object_name,
-                metadata=metadata,
-                urls=[s3_url]  # TODO make a DRS URL
-            )
-        except (requests.exceptions.HTTPError, AssertionError) as e:
-            if not ('already exists' in str(e)):
-                raise e
-            logger.info(f"indexd record already exists, continuing upload. {guid}")
-    return existing_record
+from g3t import Config, ACED_NAMESPACE
+from g3t.common import Push, Commit
+from g3t.gen3.indexd import write_indexd
+from g3t.git import calculate_hash, DVC, run_command, DVCMeta, DVCItem, modified_date
 
 
 def _validate_parameters(from_: str) -> pathlib.Path:
 
     assert len(urlparse(from_).scheme) == 0, f"{from_} appears to be an url. url to url cp not supported"
 
     return from_
@@ -75,73 +29,107 @@
 def cp(config: Config,
        from_: str,
        project_id: str,
        ignore_state: bool,
        auth=None,
        user=None,
        object_name=None,
+       bucket_name=None,
        metadata: dict = {}
        ):
     """Copy meta to bucket, used by etl_pod job"""
     from_ = _validate_parameters(str(from_))
     if not isinstance(from_, pathlib.Path):
         from_ = pathlib.Path(from_)
 
-    if not auth:
-        auth = ensure_auth(config=config)
-
-    index_client = Gen3Index(auth_provider=auth)
-    file_client = Gen3File(auth_provider=auth)
+    assert auth, "auth is required"
 
     metadata = dict({'submitter': None, 'metadata_version': '0.0.1', 'is_metadata': True} | metadata)
     if not metadata['submitter']:
         if not user:
             user = auth.curl('/user/user').json()
         metadata['submitter'] = user['name']
 
     program, project = project_id.split('-')
 
-    bucket_name = get_program_bucket(config, program, auth=auth)
     assert bucket_name, f"could not find bucket for {program}"
 
-    with tempfile.TemporaryDirectory() as temp_dir:
-        if from_.is_dir():
-            temp_dir = pathlib.Path(temp_dir)
-
-            if not object_name:
-                now = datetime.now().strftime("%Y%m%d-%H%M%S")
-                object_name = f'_{project_id}-{now}_meta.zip'
-
-            zipfile_path = temp_dir / object_name
-            with ZipFile(zipfile_path, 'w') as zip_object:
-                for _ in from_.glob("*.ndjson"):
-                    zip_object.write(_)
-        else:
-            zipfile_path = pathlib.Path(from_)
-            if not object_name:
-                object_name = str(zipfile_path)
-
-        stat = zipfile_path.stat()
-        md5_sum = md5sum(zipfile_path)
-        id_ = str(uuid.uuid5(ACED_NAMESPACE, object_name))
-
-        metadata = _update_indexd(
-            id_,
-            bucket_name,
-            ignore_state,
-            index_client,
-            md5_sum,
-            object_name,
-            program,
-            project,
-            metadata,
-            stat.st_size
-        )
+    temp_dir = config.work_dir
+    temp_dir = pathlib.Path(temp_dir)
 
-        document = file_client.upload_file_to_guid(guid=id_, file_name=object_name, bucket=bucket_name)
-        assert 'url' in document, document
-        signed_url = urllib.parse.unquote(document['url'])
+    if not object_name:
+        now = datetime.now().strftime("%Y%m%d-%H%M%S")
+        object_name = f'_{project_id}-{now}_meta.zip'
+
+    zipfile_path = temp_dir / object_name
+    with ZipFile(zipfile_path, 'w') as zip_object:
+        for _ in from_.glob("*.ndjson"):
+            zip_object.write(_)
+
+    stat = zipfile_path.stat()
+    md5_sum = calculate_hash('md5', zipfile_path)
+    my_dvc = DVC(
+            meta=DVCMeta(),
+            outs=[
+                DVCItem(
+                    path=object_name,
+                    md5=md5_sum,
+                    hash='md5',
+                    modified=modified_date(zipfile_path),
+                    size=stat.st_size,
 
-        file_name = pathlib.Path(zipfile_path)
+                )
+            ]
+        )
 
-        _upload_file_to_signed_url(file_name, md5_sum, metadata, signed_url)
-        return {'msg': f"Uploaded {file_name} to {bucket_name} {id_}", "object_id": id_}
+    metadata = write_indexd(
+        auth=auth,
+        project_id=project_id,
+        bucket_name=bucket_name,
+        overwrite=False,
+        restricted_project_id=None,
+        dvc=my_dvc,
+    )
+
+    # document = file_client.upload_file_to_guid(guid=id_, file_name=object_name, bucket=bucket_name)
+    # print(document, file=sys.stderr)
+
+    run_command(f"gen3-client upload-single --bucket {bucket_name} --guid {my_dvc.object_id} --file {zipfile_path} --profile {config.gen3.profile}", no_capture=False)
+
+    return {'msg': f"Uploaded {zipfile_path} to {bucket_name}", "object_id": my_dvc.object_id, "object_name": object_name}
+
+
+def publish_commits(config: Config, wait: bool, auth: Gen3Auth, bucket_name: str) -> dict:
+    """Publish commits to the portal."""
+
+    # TODO legacy fhir-import-export job: copies meta to bucket and triggers job,
+    #  meta information is already in git REPO,
+    #  we should consider changing the fhir_import_export job to use the git REPO
+
+    user = auth.curl('/user/user').json()
+
+    # copy meta to bucket
+    upload_result = cp(
+        config=config,
+        from_='META',
+        project_id=config.gen3.project_id,
+        ignore_state=True,
+        auth=auth,
+        user=user,
+        bucket_name=bucket_name
+    )
+
+    object_id = upload_result['object_id']
+
+    push = Push(config=config)
+    jobs_client = Gen3Jobs(auth_provider=auth)
+
+    push.commits.append(Commit(object_id=object_id, message='From g3t-git', meta_path=upload_result['object_name'], commit_id=object_id))
+    args = {'push': push.model_dump(), 'project_id': config.gen3.project_id, 'method': 'put'}
+
+    if wait:
+        _ = asyncio.run(jobs_client.async_run_job_and_wait('fhir_import_export', args))
+        _ = {'output': _}
+    else:
+        _ = jobs_client.create_job('fhir_import_export', args)
+        _ = {'output': _}
+    return _
```

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/meta/validator.py` & `gen3_tracker-0.0.4rc2/g3t/meta/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 import orjson
 from fhir.resources.coding import Coding
 from fhir.resources.identifier import Identifier
 from fhir.resources.reference import Reference
 from nested_lookup import nested_lookup
 from pydantic import BaseModel, ConfigDict
 
-from gen3_util.config import Config
-from gen3_util.meta import directory_reader, ParseResult
+from g3t.meta import ParseResult, directory_reader
 
 
 class ValidateDirectoryResult(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     """Results of FHIR validation of directory."""
     resources: dict
     exceptions: List[ParseResult]
@@ -66,15 +65,15 @@
     assert 'http' not in self.reference, f"Absolute references not supported {self}"
     assert len(self.reference.split('/')) == 2, f"Does not appear to be Relative reference {self}"
 
     # call the original dict() method
     return orig_reference_dict(self, *args, **kwargs)
 
 
-def validate(config: Config, directory_path: pathlib.Path) -> ValidateDirectoryResult:
+def validate(directory_path: pathlib.Path) -> ValidateDirectoryResult:
     """Check FHIR data, accumulate results."""
     exceptions = []
     resources = defaultdict(int)
     # add resources to bundle
     references = []
     ids = []
```

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/projects/__init__.py` & `gen3_tracker-0.0.4rc2/g3t/projects/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Any, Union
 from collections import defaultdict
 
 from gen3.auth import Gen3Auth
 from pydantic import BaseModel
 
-from gen3_util.config import ensure_auth, Config
+from g3t.config import ensure_auth, Config
 
 
 class ProjectSummary(BaseModel):
     """Summary of a project."""
     exists: bool = False
     """Project exists in sheepdog flag"""
     permissions: list[dict[str, Any]] = []
```

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/projects/cli.py` & `gen3_tracker-0.0.4rc2/g3t/projects/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import sys
+
 import click
 
-from gen3_util.access.submitter import ensure_program_project
-from gen3_util.config import Config, ensure_auth
-from gen3_util.projects.lister import ls
-from gen3_util.projects.remover import rm, empty
-from gen3_util.repo import CLIOutput, ENV_VARIABLE_PREFIX
-from gen3_util.repo import NaturalOrderGroup
+from g3t.collaborator.access.submitter import ensure_program_project
+from g3t.common import CLIOutput, assert_config, ERROR_COLOR
+from g3t.config import Config, ensure_auth
+from g3t.projects.lister import ls
+from g3t.projects.remover import rm, empty
+from g3t import NaturalOrderGroup, ENV_VARIABLE_PREFIX
 
 
 @click.group(name='projects', cls=NaturalOrderGroup)
 @click.pass_obj
 def project_group(config: Config):
     """Manage Gen3 projects."""
     pass
@@ -24,14 +26,16 @@
     with CLIOutput(config=config) as output:
         try:
             auth = ensure_auth(config=config)
             output.update(ls(config, auth=auth, full=verbose))
         except Exception as e:
             output.update({'msg': str(e)})
             output.exit_code = 1
+            if config.debug:
+                raise e
 
 
 @project_group.command(name="create")
 @click.option('--all', 'all_projects', default=False, show_default=True, is_flag=True,
               help="Create all projects")
 @click.argument('resource', default=None, required=False)
 @click.pass_obj
@@ -52,51 +56,69 @@
                 resources = ls(config, auth=auth, full=True)
                 for k, v in resources.projects.items():
                     if not v.exists:
                         _ = k.split('/')
                         assert len(_) == 5, f"Invalid resource: >{k}< {len(_)}"
                         project_ids.append(f"{_[2]}-{_[4]}")
             else:
-                assert resource, "resource is required"
+                if not resource:
+                    resource = config.gen3.authz
+                    if config.debug:
+                        click.secho(f"No resource provided, using current project {resource}", fg='yellow',
+                                    file=sys.stderr)
                 _ = resource.split('/')
-                assert len(_) == 5, f"Invalid resource: >{k}< {len(_)}"
+                assert len(_) == 5, f"Invalid resource: >{_}< {len(_)}"
                 project_ids.append(f"{_[2]}-{_[4]}")
 
             assert len(project_ids) > 0, "No projects found"
             submitter_msgs = []
             for policy_id in project_ids:
-                click.secho(f"Creating {policy_id}", fg='yellow')
+                if config.debug:
+                    click.secho(f"Creating {policy_id}", fg='yellow')
                 submitter_msgs.append(ensure_program_project(config, policy_id, auth=auth))
-
+            output.update({'msg': f"OK created {resource}"})
         except Exception as e:
-            output.update({'msg': str(e)})
+            click.secho(str(e), fg=ERROR_COLOR, file=sys.stderr)
             output.exit_code = 1
+            if config.debug:
+                raise e
 
 
 @project_group.command(name="empty")
 @click.option('--project_id', default=None, show_default=True,
               help="Gen3 program-project", envvar=f"{ENV_VARIABLE_PREFIX}PROJECT_ID")
+@click.option('--confirm', default=None, show_default=True,
+              help="Enter 'empty' to confirm", envvar=f"{ENV_VARIABLE_PREFIX}PROJECT_ID")
 @click.pass_obj
-def project_empty(config: Config, project_id: str):
+def project_empty(config: Config, project_id: str, confirm: str):
     """Empty all metadata (graph, flat) for a project."""
     with CLIOutput(config=config) as output:
         try:
+            assert confirm == 'empty', "Please confirm by entering --confirm empty"
+            if not project_id:
+                project_id = config.gen3.project_id
+                click.secho(f"No project_id provided, using current project {project_id}", fg='yellow',
+                            file=sys.stderr)
             _ = empty(config, project_id)
             _['msg'] = f"Emptied {project_id}"
             output.update(_)
         except Exception as e:
             output.update({'msg': str(e)})
             output.exit_code = 1
+            if config.debug:
+                raise e
 
 
 @project_group.command(name="rm")
 @click.option('--project_id', default=None, show_default=True,
               help="Gen3 program-project", envvar=f"{ENV_VARIABLE_PREFIX}PROJECT_ID")
 @click.pass_obj
 def project_rm(config: Config, project_id: str):
     """Remove empty project."""
     with CLIOutput(config=config) as output:
         try:
             output.update(rm(config, project_id))
         except Exception as e:
             output.update({'msg': str(e)})
             output.exit_code = 1
+            if config.debug:
+                raise e
```

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/projects/lister.py` & `gen3_tracker-0.0.4rc2/g3t/projects/lister.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from gen3.auth import Gen3Auth
-from gen3.submission import Gen3Submission
 
-from gen3_util.config import Config, ensure_auth
-from gen3_util.projects import ProjectSummaries, get_projects, ProjectSummary
+from g3t.config import Config, ensure_auth
+from g3t.projects import ProjectSummaries, get_projects, ProjectSummary
 
 
 def ls(config: Config, resource_filter: str = None, msgs: list[str] = [], auth: Gen3Auth = None, full: bool = True) -> ProjectSummaries:
     """List projects."""
+    # improve startup time by importing only what is needed
+    from gen3.submission import Gen3Submission
 
     if not auth:
         auth = ensure_auth(config=config)
     submission = Gen3Submission(auth)
 
     projects = get_projects(auth, submission)
```

### Comparing `gen3_tracker-0.0.3rc9/gen3_util/repo/initializer.py` & `gen3_tracker-0.0.4rc2/g3t/git/initializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from gen3.submission import Gen3Submission
 
-from gen3_util.access.requestor import add_policies
-from gen3_util.config import ensure_auth
-from gen3_util.projects.lister import ls as project_ls
-
-
-def project_exists(project_id: str, auth) -> list[str]:
-    pass
+from g3t.collaborator.access.requestor import add_policies
+from g3t.config import ensure_auth
+from g3t.projects.lister import ls as project_ls
 
 
 def initialize_project_server_side(config, project_id, auth=None):
     """Initialize a project in the current directory."""
+    # improve startup time by importing only what is needed
+    from gen3.submission import Gen3Submission
+
     if auth is None:
         if not config.gen3.profile:
             return ["Disconnected mode, skipping server side initialization"]
         auth = ensure_auth(config=config)
 
     logs = []
     program, project = project_id.split('-')
@@ -27,10 +25,11 @@
         sheepdog = [_ for _ in links if _ == f"/v0/submission/{program}/{project}"]
         if len(sheepdog) > 0:
             logs.append(f"Project already exists on server: {program}-{project}")
         else:
             logs.append(f"Pending request for project creation. Admin must sign access request for: /{program}/projects/{project}")
     else:
         _ = add_policies(config, project_id, auth=auth)
+        # print(_)
         policy_msgs.extend([_.msg, f"See {_.commands}"])
         logs.extend(policy_msgs)
     return logs
```

