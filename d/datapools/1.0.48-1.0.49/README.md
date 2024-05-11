# Comparing `tmp/datapools-1.0.48.tar.gz` & `tmp/datapools-1.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.48.tar", last modified: Fri May 10 13:33:15 2024, max compression
+gzip compressed data, was "datapools-1.0.49.tar", last modified: Sat May 11 13:59:45 2024, max compression
```

## Comparing `datapools-1.0.48.tar` & `datapools-1.0.49.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.381907 datapools-1.0.48/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-10 13:33:00.000000 datapools-1.0.48/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-05-10 13:33:00.000000 datapools-1.0.48/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-10 13:33:00.000000 datapools-1.0.48/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-10 13:33:00.000000 datapools-1.0.48/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-10 13:33:15.381907 datapools-1.0.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-10 13:33:00.000000 datapools-1.0.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.369907 datapools-1.0.48/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.373907 datapools-1.0.48/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.373907 datapools-1.0.48/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.373907 datapools-1.0.48/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.373907 datapools-1.0.48/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.373907 datapools-1.0.48/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.373907 datapools-1.0.48/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.377907 datapools-1.0.48/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.377907 datapools-1.0.48/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.377907 datapools-1.0.48/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.377907 datapools-1.0.48/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.377907 datapools-1.0.48/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.377907 datapools-1.0.48/datapools/worker/plugins/freesound_org/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/freesound_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/freesound_org/freesound_org.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.377907 datapools-1.0.48/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.377907 datapools-1.0.48/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.377907 datapools-1.0.48/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.377907 datapools-1.0.48/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.381907 datapools-1.0.48/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.381907 datapools-1.0.48/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.381907 datapools-1.0.48/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16532 2024-05-10 13:33:00.000000 datapools-1.0.48/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.381907 datapools-1.0.48/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-10 13:33:15.000000 datapools-1.0.48/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-10 13:33:15.000000 datapools-1.0.48/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:33:15.000000 datapools-1.0.48/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 13:33:15.000000 datapools-1.0.48/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-10 13:33:15.000000 datapools-1.0.48/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 13:33:15.000000 datapools-1.0.48/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:33:15.381907 datapools-1.0.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-10 13:33:00.000000 datapools-1.0.48/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:15.381907 datapools-1.0.48/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:33:00.000000 datapools-1.0.48/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-10 13:33:00.000000 datapools-1.0.48/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-10 13:33:00.000000 datapools-1.0.48/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.458255 datapools-1.0.49/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-11 13:59:36.000000 datapools-1.0.49/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-05-11 13:59:36.000000 datapools-1.0.49/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-11 13:59:36.000000 datapools-1.0.49/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-11 13:59:36.000000 datapools-1.0.49/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-11 13:59:45.458255 datapools-1.0.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-11 13:59:36.000000 datapools-1.0.49/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.438255 datapools-1.0.49/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.442255 datapools-1.0.49/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.442255 datapools-1.0.49/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.446255 datapools-1.0.49/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.446255 datapools-1.0.49/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.446255 datapools-1.0.49/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.446255 datapools-1.0.49/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.446255 datapools-1.0.49/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/freesound_org/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/freesound_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/freesound_org/freesound_org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.450255 datapools-1.0.49/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16547 2024-05-11 13:59:36.000000 datapools-1.0.49/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-11 13:59:45.000000 datapools-1.0.49/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-11 13:59:45.000000 datapools-1.0.49/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 13:59:45.000000 datapools-1.0.49/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-11 13:59:45.000000 datapools-1.0.49/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-11 13:59:45.000000 datapools-1.0.49/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-11 13:59:45.000000 datapools-1.0.49/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 13:59:45.458255 datapools-1.0.49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-11 13:59:36.000000 datapools-1.0.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:45.454255 datapools-1.0.49/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 13:59:36.000000 datapools-1.0.49/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-11 13:59:36.000000 datapools-1.0.49/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-11 13:59:36.000000 datapools-1.0.49/tests/test_base.py
```

### Comparing `datapools-1.0.48/HISTORY.md` & `datapools-1.0.49/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Merge remote-tracking branch 'origin/master' into sergpsu-fixes.
+  [sergpsu]
+- Merge pull request #66 from torrentsai/sergpsu-fixes. [S]
+
+  Session validation
+- Producer task rejection bugfix. [sergpsu]
+
+
+1.0.48 (2024-05-10)
+-------------------
+- Release: version 1.0.48 🚀 [sergpsu]
 - Session vlidation. [sergpsu]
 - Merge remote-tracking branch 'origin/master' into sergpsu-fixes.
   [sergpsu]
 - Merge pull request #65 from torrentsai/sergpsu-fixes. [S]
 
   GoogleDrive structural rules
```

### Comparing `datapools-1.0.48/LICENSE` & `datapools-1.0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/PKG-INFO` & `datapools-1.0.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.48
+Version: 1.0.49
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.48/README.md` & `datapools-1.0.49/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/api.py` & `datapools-1.0.49/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/cli.py` & `datapools-1.0.49/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/common/backend_api.py` & `datapools-1.0.49/datapools/common/backend_api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/common/queues/__init__.py` & `datapools-1.0.49/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/common/queues/rabbitmq.py` & `datapools-1.0.49/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/common/queues/types.py` & `datapools-1.0.49/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/common/session_manager.py` & `datapools-1.0.49/datapools/common/session_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,69 +21,76 @@
 
 class Session:
     id: str
 
     def __init__(self, session_id, redis_inst):
         self.id = session_id
         self.redis = redis_inst
+        self.meta_key = SessionManager.get_meta_key(self.id)
+        self.urls_key = SessionManager.get_urls_key(self.id)
+        self.content_key = SessionManager.get_content_key(self.id)
 
     def get_meta(self):
-        raw = self.redis.hgetall(SessionManager.get_meta_key(self.id))
+        raw = self.redis.hgetall(self.meta_key)
         res = {
             "hint_id": raw[b"hint_id"].decode(),
             "url": raw[b"url"].decode(),
             "total_tasks": int(raw[b"total_tasks"]),
             "complete_tasks": int(raw[b"complete_tasks"]),
             "failed_tasks": int(raw[b"failed_tasks"]),
             "rejected_tasks": int(raw[b"rejected_tasks"]),
             "crawled_content": int(raw[b"crawled_content"]),
             "evaluated_content": int(raw[b"evaluated_content"]),
             "status": int(raw[b"status"] if b"status" in raw else SessionStatus.NORMAL.value),
         }
         return res
 
     def set_status(self, status: SessionStatus):
-        self.redis.hset(SessionManager.get_meta_key(self.id), "status", status.value)
+        self.redis.hset(self.meta_key, "status", status.value)
 
     def is_stopped(self):
-        status = self.redis.hget(SessionManager.get_meta_key(self.id), "status")
+        status = self.redis.hget(self.meta_key, "status")
         return status is not None and int(status) == SessionStatus.STOPPED.value
 
     def add_url(self, url):
         # urls are stored in sets
-        res = self.redis.sadd(SessionManager.get_urls_key(self.id), url)
+        res = self.redis.sadd(self.urls_key, url)
         if res:
-            self.redis.hincrby(SessionManager.get_meta_key(self.id), "total_tasks", 1)
+            self.redis.hincrby(self.meta_key, "total_tasks", 1)
         return res == 1
 
     def has_url(self, url):
-        res = self.redis.sismember(SessionManager.get_urls_key(self.id), url)
+        res = self.redis.sismember(self.urls_key, url)
         # logger.info( f'has_url {res=} {type(res)=}')
         return res
 
     def add_content(self, url):
-        return self.redis.sadd(SessionManager.get_content_key(self.id), url)
+        return self.redis.sadd(self.content_key, url)
 
     def has_content(self, url):
-        return self.redis.sismember(SessionManager.get_content_key(self.id), url)
+        return self.redis.sismember(self.content_key, url)
 
     def inc_complete_urls(self):
-        self.redis.hincrby(SessionManager.get_meta_key(self.id), "complete_tasks", 1)
+        self.redis.hincrby(self.meta_key, "complete_tasks", 1)
 
     def inc_failed_urls(self):
-        self.redis.hincrby(SessionManager.get_meta_key(self.id), "failed_tasks", 1)
+        self.redis.hincrby(self.meta_key, "failed_tasks", 1)
 
     def inc_rejected_urls(self):
-        self.redis.hincrby(SessionManager.get_meta_key(self.id), "rejected_tasks", 1)
+        self.redis.hincrby(self.meta_key, "rejected_tasks", 1)
 
     def inc_crawled_content(self):
-        self.redis.hincrby(SessionManager.get_meta_key(self.id), "crawled_content", 1)
+        self.redis.hincrby(self.meta_key, "crawled_content", 1)
 
     def inc_evaluated_content(self):
-        self.redis.hincrby(SessionManager.get_meta_key(self.id), "evaluated_content", 1)
+        self.redis.hincrby(self.meta_key, "evaluated_content", 1)
+
+    def exists(self):
+        res = self.redis.exists(self.meta_key)
+        return res
 
 
 class SessionManager:
     def __init__(self, host, port=6379, db=0, protocol=3):
         self.redis = redis.Redis(host=host, port=port, db=db, protocol=protocol)
 
     def is_ready(self) -> bool:
```

### Comparing `datapools-1.0.48/datapools/common/stoppable.py` & `datapools-1.0.49/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/common/storage/base_storage.py` & `datapools-1.0.49/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/common/storage/file_storage.py` & `datapools-1.0.49/datapools/common/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.49/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.49/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/common/types.py` & `datapools-1.0.49/datapools/common/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/producer/base_producer.py` & `datapools-1.0.49/datapools/producer/base_producer.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # from enum import Enum
 from typing import List, Optional
 
 from ..common.backend_api import BackendAPI, BackendAPIException
 from ..common.logger import logger
 from ..common.queues import GenericQueue, QueueMessage, QueueMessageType, QueueRole, QueueTopicMessage
-from ..common.session_manager import SessionManager
+from ..common.session_manager import SessionManager, Session
 from ..common.stoppable import Stoppable
 from ..common.storage.file_storage import FileStorage
 from ..common.types import BaseProducerSettings, InvalidUsageException
 from ..worker.utils import get_storage_invalidation_topic
 
 # from .rules import DatapoolRulesChecker
 
@@ -82,34 +82,29 @@
     async def router_loop(self):
         try:
             while not await self.is_stopped():
                 message = await self.eval_queue.pop(timeout=1)
                 if message:
                     qm = QueueMessage.decode(message.body)
                     try:
-                        if not self.session_manager.has(qm.session_id):
-                            logger.info(f"session is deleted {qm.session_id=}")
-                            await self.eval_queue.mark_done(message)
-                            continue
-
                         session = self.session_manager.get(qm.session_id)
                         if session is None or session.is_stopped():
-                            logger.info(f"session is stopped {qm.session_id=} {message.message_id}")
+                            logger.info(f"session is deleted or stopped {qm.session_id=} {message.message_id}")
                             await self.eval_queue.mark_done(message)
                             continue
 
                         if qm.type == QueueMessageType.Task:
                             task = qm.data
                             logger.info(f"Producer got: {task}")
 
                             # TODO: this storage must be associated with the worker!
                             #   For example, storage path or url can be formatted accordingly to worker id
                             worker_storage = FileStorage(self.cfg.WORKER_STORAGE_PATH)
                             raw_data = await worker_storage.get(task["storage_id"])
-                            await self.process_content(qm.session_id, raw_data, task)
+                            await self.process_content(session, raw_data, task)
 
                             if not self.is_shared_storage():
                                 # tell worker that his storage item can be removed
                                 await self.topics_queue.push(
                                     QueueTopicMessage(
                                         get_storage_invalidation_topic(task["worker_id"]),
                                         {"storage_id": task["storage_id"]},
@@ -119,35 +114,35 @@
                             logger.info("base_producer: stop task received")
                             self.stop_task_received.set()
                         else:
                             raise Exception(f"!!!!!!!!!!!!!!! BUG: unexpected {message=} {qm=}")
 
                         await self.eval_queue.mark_done(message)
                     except BackendAPIException as e:
-                        logger.error(str(e))
-                        await self.eval_queue.reject(message)
+                        logger.error("Catched BackendAPIException")
+                        logger.error(traceback.format_exc())
+                        await self.eval_queue.reject(message, requeue=False)
                         await asyncio.sleep(5)
                     except Exception as e:
-                        logger.error(f"Catched: {traceback.format_exc()}")
-                        logger.error(f"failed evaluate {e}")
-                        await self.eval_queue.reject(message)
+                        logger.error("Catched Exception")
+                        logger.error(traceback.format_exc())
+                        await self.eval_queue.reject(message, requeue=False)
 
         except Exception as e:
             logger.error(f"Catched: {traceback.format_exc()}")
             logger.error(f"!!!!!!! Exception in Datapools::router_loop() {e}")
 
-    async def process_content(self, session_id, raw_data, task):
+    async def process_content(self, session: Session, raw_data, task):
         # path = os.path.join(self.cfg.STORAGE_PATH, str(datapool_id))
         if not self.is_shared_storage():
             path = self.cfg.STORAGE_PATH
             if not os.path.exists(path):
                 os.mkdir(path)
             storage = FileStorage(path)
             # put data into persistent storage
             await storage.put(task["storage_id"], raw_data)
 
-        session = self.session_manager.get(session_id)
-        if session is not None:
+        if session.exists():  # session may have been deleted while processing content
             session.inc_evaluated_content()
 
     def is_shared_storage(self):
         return self.cfg.STORAGE_PATH is None or self.cfg.WORKER_STORAGE_PATH == self.cfg.STORAGE_PATH
```

### Comparing `datapools-1.0.48/datapools/scheduler/scheduler.py` & `datapools-1.0.49/datapools/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.49/datapools/worker/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.49/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/worker/plugins/default/default.py` & `datapools-1.0.49/datapools/worker/plugins/default/default.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.49/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/worker/plugins/freesound_org/freesound_org.py` & `datapools-1.0.49/datapools/worker/plugins/freesound_org/freesound_org.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.49/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.49/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.49/datapools/worker/plugins/s3/s3.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.49/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.49/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.49/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 from typing import Optional, Tuple
 
-from playwright.async_api import async_playwright
+from playwright.async_api import async_playwright, Page
 
 from ....common.logger import logger
 from ....common.storage import BaseStorage
 from ....common.types import CrawlerContent, CrawlerDemoUser, DatapoolContentType
 from ..base_plugin import BasePlugin, BaseTag, CachedPairs, WorkerTask
 
 
 class WikipediaPlugin(BasePlugin):
     users = CachedPairs()
+    history_page: Page
+    user_page: Page
 
     def __init__(self, ctx, demo_tag=False):
         super().__init__(ctx)
         self.demo_tag = BaseTag(demo_tag)
 
     @staticmethod
     def is_supported(url):
         u = BasePlugin.parse_url(url)
         return BasePlugin.is_same_or_subdomain(u.netloc, "wikipedia.org")
 
     async def process(self, task: WorkerTask):
         logger.info(f"wikipedia::process({task.url})")
 
         async with async_playwright() as playwright:
-            self.webkit = playwright.chromium
-            self.browser = await self.webkit.launch()
-            self.context = await self.browser.new_context()
-            self.page = await self.context.new_page()
-            self.history_page = await self.context.new_page()
-            self.user_page = await self.context.new_page()
+            browser = await playwright.chromium.launch()
+            context = await browser.new_context()
+            page = await context.new_page()
+            self.history_page = await context.new_page()
+            self.user_page = await context.new_page()
 
             logger.info(f"loading url {task.url}")
-            await self.page.goto(str(task.url))
+            await page.goto(str(task.url))
 
             p = BasePlugin.parse_url(task.url)
 
             if not self.demo_tag.is_valid():
-                platform_tag = await self.get_platform_tag(p.netloc, self.page, 3600)
+                platform_tag = await self.get_platform_tag(p.netloc, page, 3600)
             else:
                 platform_tag = self.demo_tag
 
             # get text of the page as plain text
-            bodys = self.page.locator("body")
+            bodys = page.locator("body")
             body = bodys.nth(0)
             body_text = await body.inner_text()
 
             # locate "History" link
-            history_url_loc = await self.page.locator("#ca-history a").all()
+            history_url_loc = await page.locator("#ca-history a").all()
             if len(history_url_loc) > 0:
                 history_url = await history_url_loc[0].get_attribute("href")
                 history_url = BasePlugin.get_local_url(history_url, task.url)
                 # TODO: shared ownership to be implemented later
                 #       for now use the creator of the article as the copyright owner.
                 #       Commented code below is more or less valid
                 # users = await self._collect_users(history_url)
@@ -86,15 +87,15 @@
                         tag_keepout=creator_tag.is_keepout() if creator_tag is not None else False,
                         type=DatapoolContentType.Text,
                         storage_id=storage_id,
                         url=task.url,
                     )
 
             # parsing links as back tasks
-            async for yielded in self.parse_links(self.page):
+            async for yielded in self.parse_links(page):
                 yield yielded
 
     async def _get_article_creator(self, history_url) -> Tuple[Optional[BaseTag], Optional[str]]:
         """
         get the earliest user from the history list.
         """
         history_url += "&dir=prev"
```

### Comparing `datapools-1.0.48/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.49/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/datapools/worker/worker.py` & `datapools-1.0.49/datapools/worker/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
             logger.error(traceback.format_exc())
 
     async def _process_todo_message(self, message):
         qm = QueueMessage.decode(message.body)
 
         if not self.session_manager.has(qm.session_id):
             logger.error(f"Session not found {qm.session_id}")
-            await self.todo_queue.reject(message)
+            await self.todo_queue.reject(message, requeue=False)
             return
 
         if qm.type == QueueMessageType.Task:
             done = False
 
             task = WorkerTask(url=qm.data["url"], content_type=qm.data.get("content_type"))
             logger.info(f"got {task=} {qm.session_id=}")
```

### Comparing `datapools-1.0.48/datapools.egg-info/PKG-INFO` & `datapools-1.0.49/datapools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.48
+Version: 1.0.49
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.48/datapools.egg-info/SOURCES.txt` & `datapools-1.0.49/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/setup.py` & `datapools-1.0.49/setup.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.48/tests/test_base.py` & `datapools-1.0.49/tests/test_base.py`

 * *Files identical despite different names*

